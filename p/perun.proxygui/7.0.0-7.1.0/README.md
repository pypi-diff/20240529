# Comparing `tmp/perun.proxygui-7.0.0.tar.gz` & `tmp/perun.proxygui-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun.proxygui-7.0.0.tar", last modified: Mon May 20 12:39:24 2024, max compression
+gzip compressed data, was "perun.proxygui-7.1.0.tar", last modified: Wed May 29 09:45:04 2024, max compression
```

## Comparing `perun.proxygui-7.0.0.tar` & `perun.proxygui-7.1.0.tar`

### file list

```diff
@@ -1,290 +1,290 @@
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.178197 perun.proxygui-7.0.0/
--rw-rw-rw-   0     1001 root         (0)     1560 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/LICENSE
--rw-rw-rw-   0     1001 root         (0)       46 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/MANIFEST.in
--rw-r--r--   0     1001 root         (0)     9147 2024-05-20 12:39:24.178197 perun.proxygui-7.0.0/PKG-INFO
--rw-rw-rw-   0     1001 root         (0)     8067 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/README.md
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.126197 perun.proxygui-7.0.0/perun/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.130197 perun.proxygui-7.0.0/perun/proxygui/
--rw-rw-rw-   0     1001 root         (0)        0 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/__init__.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.130197 perun.proxygui-7.0.0/perun/proxygui/api/
--rw-rw-rw-   0     1001 root         (0)        0 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/api/__init__.py
--rw-rw-rw-   0     1001 root         (0)     2478 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/api/backchannel_logout_api.py
--rw-rw-rw-   0     1001 root         (0)     7430 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/api/ban_api.py
--rw-rw-rw-   0     1001 root         (0)     4900 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/api/consent_api.py
--rw-rw-rw-   0     1001 root         (0)    10747 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/api/heuristic_api.py
--rw-rw-rw-   0     1001 root         (0)     6637 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/app.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.130197 perun.proxygui-7.0.0/perun/proxygui/gui/
--rw-rw-rw-   0     1001 root         (0)        0 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/__init__.py
--rw-rw-rw-   0     1001 root         (0)    21745 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/gui.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.130197 perun.proxygui-7.0.0/perun/proxygui/gui/static/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.126197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.122197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.130197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.130197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/
--rw-rw-rw-   0     1001 root         (0)   141520 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map
--rw-rw-rw-   0     1001 root         (0)       99 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_atoms.scss
--rw-rw-rw-   0     1001 root         (0)      612 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss
--rw-rw-rw-   0     1001 root         (0)       67 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_organisms.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.134197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/
--rw-rw-rw-   0     1001 root         (0)      688 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss
--rw-rw-rw-   0     1001 root         (0)       19 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_calendar.scss
--rw-rw-rw-   0     1001 root         (0)      949 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss
--rw-rw-rw-   0     1001 root         (0)     1663 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.134197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/
--rw-rw-rw-   0     1001 root         (0)      477 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/_icons.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.122197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.134197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/
--rw-rw-rw-   0     1001 root         (0)      631 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss
--rw-rw-rw-   0     1001 root         (0)     1451 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss
--rw-rw-rw-   0     1001 root         (0)     3089 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss
--rw-rw-rw-   0     1001 root         (0)     1617 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss
--rw-rw-rw-   0     1001 root         (0)     1776 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss
--rw-rw-rw-   0     1001 root         (0)      437 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_food-menu.scss
--rw-rw-rw-   0     1001 root         (0)      387 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_images.scss
--rw-rw-rw-   0     1001 root         (0)     2945 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss
--rw-rw-rw-   0     1001 root         (0)     2624 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss
--rw-rw-rw-   0     1001 root         (0)      713 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss
--rw-rw-rw-   0     1001 root         (0)     1899 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.134197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/
--rw-rw-rw-   0     1001 root         (0)      815 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss
--rw-rw-rw-   0     1001 root         (0)      571 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.134197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/
--rw-rw-rw-   0     1001 root         (0)      421 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_mega.scss
--rw-rw-rw-   0     1001 root         (0)      403 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_primary.scss
--rw-rw-rw-   0     1001 root         (0)     2758 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.134197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/
--rw-rw-rw-   0     1001 root         (0)      198 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_footer.scss
--rw-rw-rw-   0     1001 root         (0)      684 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss
--rw-rw-rw-   0     1001 root         (0)    29997 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css
--rw-rw-rw-   0     1001 root         (0)      244 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.126197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.138197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/
--rw-rw-rw-   0     1001 root         (0)    22637 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg
--rw-rw-rw-   0     1001 root         (0)    21057 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg
--rw-rw-rw-   0     1001 root         (0)    22481 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg
--rw-rw-rw-   0     1001 root         (0)    35533 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg
--rw-rw-rw-   0     1001 root         (0)    34805 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg
--rw-rw-rw-   0     1001 root         (0)    28733 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg
--rw-rw-rw-   0     1001 root         (0)    20267 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg
--rw-rw-rw-   0     1001 root         (0)    28025 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg
--rw-rw-rw-   0     1001 root         (0)    25884 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg
--rw-rw-rw-   0     1001 root         (0)   363233 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg
--rw-rw-rw-   0     1001 root         (0)    27013 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg
--rw-rw-rw-   0     1001 root         (0)    33321 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg
--rw-rw-rw-   0     1001 root         (0)    31511 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg
--rw-rw-rw-   0     1001 root         (0)    34010 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg
--rw-rw-rw-   0     1001 root         (0)    28152 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg
--rw-rw-rw-   0     1001 root         (0)    36726 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg
--rw-rw-rw-   0     1001 root         (0)    28663 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg
--rw-rw-rw-   0     1001 root         (0)    22030 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.142197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.154197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/
--rw-rw-rw-   0     1001 root         (0)   125046 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map
--rw-rw-rw-   0     1001 root         (0)   252563 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map
--rw-rw-rw-   0     1001 root         (0)  1052500 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map
--rw-rw-rw-   0     1001 root         (0)  1125125 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map
--rw-rw-rw-   0     1001 root         (0)  1125144 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map
--rw-rw-rw-   0     1001 root         (0)  1125123 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map
--rw-rw-rw-   0     1001 root         (0)  1125121 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map
--rw-rw-rw-   0     1001 root         (0)  1125119 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map
--rw-rw-rw-   0     1001 root         (0)  1125120 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map
--rw-rw-rw-   0     1001 root         (0)  1125147 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map
--rw-rw-rw-   0     1001 root         (0)  1125545 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map
--rw-rw-rw-   0     1001 root         (0)  1125121 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map
--rw-rw-rw-   0     1001 root         (0)  1126098 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map
--rw-rw-rw-   0     1001 root         (0)   139176 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map
--rw-rw-rw-   0     1001 root         (0)     2596 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/documentation.css
--rw-rw-rw-   0     1001 root         (0)    48080 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/print.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.158197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/
--rw-rw-rw-   0     1001 root         (0)     2596 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css
--rw-rw-rw-   0     1001 root         (0)    46987 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css
--rw-rw-rw-   0     1001 root         (0)   303728 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css
--rw-rw-rw-   0     1001 root         (0)   332353 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css
--rw-rw-rw-   0     1001 root         (0)   332557 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css
--rw-rw-rw-   0     1001 root         (0)     5778 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css
--rw-rw-rw-   0     1001 root         (0)   312236 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-custom.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-econ.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fi.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fss.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-law.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-med.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-ped.css
--rw-rw-rw-   0     1001 root         (0)   341456 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-phil.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-sci.css
--rw-rw-rw-   0     1001 root         (0)   341664 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style.css
--rw-rw-rw-   0     1001 root         (0)     5772 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.162197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/
--rw-rw-rw-   0     1001 root         (0)    87048 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff
--rw-rw-rw-   0     1001 root         (0)    74284 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2
--rw-rw-rw-   0     1001 root         (0)   208892 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff
--rw-rw-rw-   0     1001 root         (0)   159376 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2
--rw-rw-rw-   0     1001 root         (0)     1632 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot
--rw-rw-rw-   0     1001 root         (0)     1837 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg
--rw-rw-rw-   0     1001 root         (0)     1484 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf
--rw-rw-rw-   0     1001 root         (0)      988 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff
--rw-rw-rw-   0     1001 root         (0)    12252 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff
--rw-rw-rw-   0     1001 root         (0)     9596 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.162197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.162197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/
--rw-rw-rw-   0     1001 root         (0)    70841 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg
--rw-rw-rw-   0     1001 root         (0)     4348 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif
--rw-rw-rw-   0     1001 root         (0)      151 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/ico-external.png
--rw-rw-rw-   0     1001 root         (0)      279 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-ciisb.png
--rw-rw-rw-   0     1001 root         (0)      279 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-crc.png
--rw-rw-rw-   0     1001 root         (0)      280 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-econ.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fi.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fsps.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fss.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-law.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-med.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-ped.png
--rw-rw-rw-   0     1001 root         (0)      281 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-phil.png
--rw-rw-rw-   0     1001 root         (0)      280 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-sci.png
--rw-rw-rw-   0     1001 root         (0)      149 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-small.png
--rw-rw-rw-   0     1001 root         (0)      304 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select.png
--rw-rw-rw-   0     1001 root         (0)     7406 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/favicon.ico
--rw-rw-rw-   0     1001 root         (0)     4426 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png
--rw-rw-rw-   0     1001 root         (0)      443 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/logo.svg
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.166197 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/
--rw-rw-rw-   0     1001 root         (0)   218591 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js
--rw-rw-rw-   0     1001 root         (0)   659454 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js.map
--rw-rw-rw-   0     1001 root         (0)   337945 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/d3.js
--rw-rw-rw-   0     1001 root         (0)     2707 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/documentation.js
--rw-rw-rw-   0     1001 root         (0)     8806 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/graphs.js
--rw-rw-rw-   0     1001 root         (0)    26171 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js
--rw-rw-rw-   0     1001 root         (0)     4075 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js
--rw-rw-rw-   0     1001 root         (0)   284394 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.js
--rw-rw-rw-   0     1001 root         (0)   610160 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.126197 perun.proxygui-7.0.0/perun/proxygui/gui/static/bootstrap/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.166197 perun.proxygui-7.0.0/perun/proxygui/gui/static/bootstrap/css/
--rw-rw-rw-   0     1001 root         (0)   155845 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css
--rw-rw-rw-   0     1001 root         (0)   431289 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.166197 perun.proxygui-7.0.0/perun/proxygui/gui/static/bootstrap/js/
--rw-rw-rw-   0     1001 root         (0)    78743 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-rw-   0     1001 root         (0)   325834 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0     1001 root         (0)       78 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/campus-idp-muni.js
--rw-rw-rw-   0     1001 root         (0)     7365 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/campus-idp.css
--rw-rw-rw-   0     1001 root         (0)     4859 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/campus-idp.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.126197 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.166197 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/css/
--rw-rw-rw-   0     1001 root         (0)    73577 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/css/all.css
--rw-rw-rw-   0     1001 root         (0)    59305 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/css/all.min.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.170197 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/
--rw-rw-rw-   0     1001 root         (0)   134294 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot
--rw-rw-rw-   0     1001 root         (0)   747927 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg
--rw-rw-rw-   0     1001 root         (0)   133988 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0     1001 root         (0)    89988 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff
--rw-rw-rw-   0     1001 root         (0)    76736 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0     1001 root         (0)    34034 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot
--rw-rw-rw-   0     1001 root         (0)   144714 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg
--rw-rw-rw-   0     1001 root         (0)    33736 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0     1001 root         (0)    16276 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff
--rw-rw-rw-   0     1001 root         (0)    13224 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0     1001 root         (0)   203030 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot
--rw-rw-rw-   0     1001 root         (0)   918991 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg
--rw-rw-rw-   0     1001 root         (0)   202744 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0     1001 root         (0)   101648 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff
--rw-rw-rw-   0     1001 root         (0)    78268 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.170197 perun.proxygui-7.0.0/perun/proxygui/gui/static/images/
--rw-rw-rw-   0     1001 root         (0)      490 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/images/check.svg
--rw-rw-rw-   0     1001 root         (0)      536 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/images/circle-check-regular.svg
--rw-rw-rw-   0     1001 root         (0)      483 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/images/circle-exclamation-solid.svg
--rw-rw-rw-   0     1001 root         (0)      730 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/images/questionmark.svg
--rw-rw-rw-   0     1001 root         (0)      625 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/images/spinner.svg
--rw-rw-rw-   0     1001 root         (0)    89501 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/jquery-3.6.0.min.js
--rw-rw-rw-   0     1001 root         (0)      627 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/proxygui.css
--rw-rw-rw-   0     1001 root         (0)     1427 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/proxygui.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.126197 perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.174197 perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/
--rw-rw-rw-   0     1001 root         (0)    15836 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css
--rw-rw-rw-   0     1001 root         (0)     8266 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css
--rw-rw-rw-   0     1001 root         (0)     8862 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css
--rw-rw-rw-   0     1001 root         (0)     8873 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css
--rw-rw-rw-   0     1001 root         (0)     7692 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/selectize.css
--rw-rw-rw-   0     1001 root         (0)     8344 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/selectize.default.css
--rw-rw-rw-   0     1001 root         (0)    11438 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/selectize.legacy.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.126197 perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/js/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.174197 perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/js/standalone/
--rw-rw-rw-   0     1001 root         (0)    64906 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.174197 perun.proxygui-7.0.0/perun/proxygui/gui/templates/
--rw-rw-rw-   0     1001 root         (0)    15205 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/ConsentRegistration.html
--rw-rw-rw-   0     1001 root         (0)     9168 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/HeuristicData.html
--rw-rw-rw-   0     1001 root         (0)      747 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/IsTestingSP.html
--rw-rw-rw-   0     1001 root         (0)     3101 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/Logout.html
--rw-rw-rw-   0     1001 root         (0)     1131 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/MfaResetEmailSent.html
--rw-rw-rw-   0     1001 root         (0)     1942 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/MfaResetInitiated.html
--rw-rw-rw-   0     1001 root         (0)     1133 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html
--rw-rw-rw-   0     1001 root         (0)     1021 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/MfaResult.html
--rw-rw-rw-   0     1001 root         (0)      795 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/MissingAuth.html
--rw-rw-rw-   0     1001 root         (0)     1019 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/OidcError.html
--rw-rw-rw-   0     1001 root         (0)     1223 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/Post-logout.html
--rw-rw-rw-   0     1001 root         (0)      907 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/SPAuthorization.html
--rw-rw-rw-   0     1001 root         (0)     2490 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/_footer.html
--rw-rw-rw-   0     1001 root         (0)     8119 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/_header.html
--rw-rw-rw-   0     1001 root         (0)     1175 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/authorization.html
--rw-rw-rw-   0     1001 root         (0)     3477 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/base.html
--rw-rw-rw-   0     1001 root         (0)      734 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/logout-canceled.html
--rw-rw-rw-   0     1001 root         (0)      561 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/logout-iframe.html
--rw-rw-rw-   0     1001 root         (0)     3769 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/templates/logout-state.html
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.126197 perun.proxygui-7.0.0/perun/proxygui/gui/translations/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.126197 perun.proxygui-7.0.0/perun/proxygui/gui/translations/cs/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.174197 perun.proxygui-7.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/
--rw-rw-rw-   0     1001 root         (0)     2973 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo
--rw-rw-rw-   0     1001 root         (0)     8108 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po
--rw-rw-rw-   0     1001 root         (0)     5807 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/jwt.py
--rw-rw-rw-   0     1001 root         (0)    20231 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/logout_manager.py
--rw-rw-rw-   0     1001 root         (0)     2480 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/oauth.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.174197 perun.proxygui-7.0.0/perun/proxygui/openapi/
--rw-rw-rw-   0     1001 root         (0)     6107 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/openapi/openapi.py
--rw-rw-rw-   0     1001 root         (0)    12320 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/openapi/openapi_data.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.174197 perun.proxygui-7.0.0/perun/proxygui/openapi/schemas/
--rw-rw-rw-   0     1001 root         (0)      982 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/openapi/schemas/arguments_schemas.py
--rw-rw-rw-   0     1001 root         (0)     1401 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/openapi/schemas/response_schemas.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.174197 perun.proxygui-7.0.0/perun/proxygui/tests/
--rw-rw-rw-   0     1001 root         (0)        0 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/tests/__init__.py
--rw-rw-rw-   0     1001 root         (0)     1816 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/tests/shared_test_data.py
--rw-rw-rw-   0     1001 root         (0)     9207 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/tests/test_ban_api.py
--rw-rw-rw-   0     1001 root         (0)     6635 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/tests/test_consent_api.py
--rw-rw-rw-   0     1001 root         (0)     4713 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/tests/test_consent_db.py
--rw-rw-rw-   0     1001 root         (0)     2160 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/tests/test_consent_request_db.py
--rw-rw-rw-   0     1001 root         (0)     6877 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/tests/test_gui.py
--rw-rw-rw-   0     1001 root         (0)    23012 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/proxygui/user_manager.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.178197 perun.proxygui-7.0.0/perun/utils/
--rw-rw-rw-   0     1001 root         (0)     2496 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/ConfigStore.py
--rw-rw-rw-   0     1001 root         (0)       43 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/CustomExceptions.py
--rw-rw-rw-   0     1001 root         (0)     2555 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/CustomRPHandler.py
--rw-rw-rw-   0     1001 root         (0)     1545 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/DatabaseService.py
--rw-rw-rw-   0     1001 root         (0)     4414 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/EmailService.py
--rw-rw-rw-   0     1001 root         (0)       96 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/Notification.py
--rw-rw-rw-   0     1001 root         (0)      816 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/Utils.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.178197 perun.proxygui-7.0.0/perun/utils/auth_event_loggig/
--rw-rw-rw-   0     1001 root         (0)     2100 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/auth_event_loggig/AuthEventLoggingDbModels.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.178197 perun.proxygui-7.0.0/perun/utils/consent_framework/
--rw-rw-rw-   0     1001 root         (0)     1241 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/consent_framework/consent.py
--rw-rw-rw-   0     1001 root         (0)     2226 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/consent_framework/consent_db.py
--rw-rw-rw-   0     1001 root         (0)     2274 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/consent_framework/consent_manager.py
--rw-rw-rw-   0     1001 root         (0)      730 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/consent_framework/consent_request.py
--rw-rw-rw-   0     1001 root         (0)     1371 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/consent_framework/consent_request_db.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.178197 perun.proxygui-7.0.0/perun/utils/logout_requests/
--rw-rw-rw-   0     1001 root         (0)     2001 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/logout_requests/BackchannelLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)      832 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/logout_requests/FrontchannelLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     3841 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/logout_requests/GraphLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     1361 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/logout_requests/LogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     2204 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/perun/utils/logout_requests/SamlLogoutRequest.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-20 12:39:24.126197 perun.proxygui-7.0.0/perun.proxygui.egg-info/
--rw-r--r--   0     1001 root         (0)     9147 2024-05-20 12:39:24.000000 perun.proxygui-7.0.0/perun.proxygui.egg-info/PKG-INFO
--rw-r--r--   0     1001 root         (0)    12805 2024-05-20 12:39:24.000000 perun.proxygui-7.0.0/perun.proxygui.egg-info/SOURCES.txt
--rw-r--r--   0     1001 root         (0)        1 2024-05-20 12:39:24.000000 perun.proxygui-7.0.0/perun.proxygui.egg-info/dependency_links.txt
--rw-r--r--   0     1001 root         (0)      427 2024-05-20 12:39:24.000000 perun.proxygui-7.0.0/perun.proxygui.egg-info/requires.txt
--rw-r--r--   0     1001 root         (0)        6 2024-05-20 12:39:24.000000 perun.proxygui-7.0.0/perun.proxygui.egg-info/top_level.txt
--rw-rw-rw-   0     1001 root         (0)       90 2024-05-20 12:39:24.178197 perun.proxygui-7.0.0/setup.cfg
--rw-rw-rw-   0     1001 root         (0)     1326 2024-05-20 12:38:56.000000 perun.proxygui-7.0.0/setup.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.413359 perun.proxygui-7.1.0/
+-rw-rw-rw-   0     1001 root         (0)     1560 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/LICENSE
+-rw-rw-rw-   0     1001 root         (0)       46 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/MANIFEST.in
+-rw-r--r--   0     1001 root         (0)     9220 2024-05-29 09:45:04.413359 perun.proxygui-7.1.0/PKG-INFO
+-rw-rw-rw-   0     1001 root         (0)     8140 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/README.md
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.353359 perun.proxygui-7.1.0/perun/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.365359 perun.proxygui-7.1.0/perun/proxygui/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/__init__.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.365359 perun.proxygui-7.1.0/perun/proxygui/api/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/api/__init__.py
+-rw-rw-rw-   0     1001 root         (0)     2478 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/api/backchannel_logout_api.py
+-rw-rw-rw-   0     1001 root         (0)     7430 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/api/ban_api.py
+-rw-rw-rw-   0     1001 root         (0)     4900 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/api/consent_api.py
+-rw-rw-rw-   0     1001 root         (0)    12819 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/api/heuristic_api.py
+-rw-rw-rw-   0     1001 root         (0)     6637 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/app.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.365359 perun.proxygui-7.1.0/perun/proxygui/gui/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/__init__.py
+-rw-rw-rw-   0     1001 root         (0)    21745 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/gui.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.365359 perun.proxygui-7.1.0/perun/proxygui/gui/static/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.353359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.353359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.365359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.365359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/
+-rw-rw-rw-   0     1001 root         (0)   141520 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map
+-rw-rw-rw-   0     1001 root         (0)       99 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_atoms.scss
+-rw-rw-rw-   0     1001 root         (0)      612 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss
+-rw-rw-rw-   0     1001 root         (0)       67 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_organisms.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.365359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/
+-rw-rw-rw-   0     1001 root         (0)      688 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss
+-rw-rw-rw-   0     1001 root         (0)       19 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_calendar.scss
+-rw-rw-rw-   0     1001 root         (0)      949 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss
+-rw-rw-rw-   0     1001 root         (0)     1663 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.365359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/
+-rw-rw-rw-   0     1001 root         (0)      477 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/_icons.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.353359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.369359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/
+-rw-rw-rw-   0     1001 root         (0)      631 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss
+-rw-rw-rw-   0     1001 root         (0)     1451 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss
+-rw-rw-rw-   0     1001 root         (0)     3089 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss
+-rw-rw-rw-   0     1001 root         (0)     1617 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss
+-rw-rw-rw-   0     1001 root         (0)     1776 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss
+-rw-rw-rw-   0     1001 root         (0)      437 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_food-menu.scss
+-rw-rw-rw-   0     1001 root         (0)      387 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_images.scss
+-rw-rw-rw-   0     1001 root         (0)     2945 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss
+-rw-rw-rw-   0     1001 root         (0)     2624 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss
+-rw-rw-rw-   0     1001 root         (0)      713 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss
+-rw-rw-rw-   0     1001 root         (0)     1899 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.369359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/
+-rw-rw-rw-   0     1001 root         (0)      815 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss
+-rw-rw-rw-   0     1001 root         (0)      571 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.369359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/
+-rw-rw-rw-   0     1001 root         (0)      421 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_mega.scss
+-rw-rw-rw-   0     1001 root         (0)      403 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_primary.scss
+-rw-rw-rw-   0     1001 root         (0)     2758 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.369359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/
+-rw-rw-rw-   0     1001 root         (0)      198 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_footer.scss
+-rw-rw-rw-   0     1001 root         (0)      684 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss
+-rw-rw-rw-   0     1001 root         (0)    29997 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css
+-rw-rw-rw-   0     1001 root         (0)      244 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.353359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.373359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/
+-rw-rw-rw-   0     1001 root         (0)    22637 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    21057 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    22481 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg
+-rw-rw-rw-   0     1001 root         (0)    35533 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    34805 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    28733 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg
+-rw-rw-rw-   0     1001 root         (0)    20267 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg
+-rw-rw-rw-   0     1001 root         (0)    28025 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg
+-rw-rw-rw-   0     1001 root         (0)    25884 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg
+-rw-rw-rw-   0     1001 root         (0)   363233 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg
+-rw-rw-rw-   0     1001 root         (0)    27013 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    33321 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    31511 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg
+-rw-rw-rw-   0     1001 root         (0)    34010 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg
+-rw-rw-rw-   0     1001 root         (0)    28152 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg
+-rw-rw-rw-   0     1001 root         (0)    36726 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg
+-rw-rw-rw-   0     1001 root         (0)    28663 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg
+-rw-rw-rw-   0     1001 root         (0)    22030 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.377359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.389359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/
+-rw-rw-rw-   0     1001 root         (0)   125046 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map
+-rw-rw-rw-   0     1001 root         (0)   252563 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map
+-rw-rw-rw-   0     1001 root         (0)  1052500 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125125 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125144 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125123 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125121 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125119 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125120 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125147 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125545 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125121 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map
+-rw-rw-rw-   0     1001 root         (0)  1126098 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map
+-rw-rw-rw-   0     1001 root         (0)   139176 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map
+-rw-rw-rw-   0     1001 root         (0)     2596 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/documentation.css
+-rw-rw-rw-   0     1001 root         (0)    48080 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/print.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.393359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/
+-rw-rw-rw-   0     1001 root         (0)     2596 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css
+-rw-rw-rw-   0     1001 root         (0)    46987 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css
+-rw-rw-rw-   0     1001 root         (0)   303728 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css
+-rw-rw-rw-   0     1001 root         (0)   332353 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css
+-rw-rw-rw-   0     1001 root         (0)   332557 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css
+-rw-rw-rw-   0     1001 root         (0)     5778 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css
+-rw-rw-rw-   0     1001 root         (0)   312236 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-custom.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-econ.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-fi.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-fss.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-law.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-med.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-ped.css
+-rw-rw-rw-   0     1001 root         (0)   341456 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-phil.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-sci.css
+-rw-rw-rw-   0     1001 root         (0)   341664 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style.css
+-rw-rw-rw-   0     1001 root         (0)     5772 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.393359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/
+-rw-rw-rw-   0     1001 root         (0)    87048 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff
+-rw-rw-rw-   0     1001 root         (0)    74284 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2
+-rw-rw-rw-   0     1001 root         (0)   208892 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff
+-rw-rw-rw-   0     1001 root         (0)   159376 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2
+-rw-rw-rw-   0     1001 root         (0)     1632 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot
+-rw-rw-rw-   0     1001 root         (0)     1837 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg
+-rw-rw-rw-   0     1001 root         (0)     1484 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf
+-rw-rw-rw-   0     1001 root         (0)      988 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff
+-rw-rw-rw-   0     1001 root         (0)    12252 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff
+-rw-rw-rw-   0     1001 root         (0)     9596 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.397359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.397359 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/
+-rw-rw-rw-   0     1001 root         (0)    70841 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg
+-rw-rw-rw-   0     1001 root         (0)     4348 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif
+-rw-rw-rw-   0     1001 root         (0)      151 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/ico-external.png
+-rw-rw-rw-   0     1001 root         (0)      279 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-ciisb.png
+-rw-rw-rw-   0     1001 root         (0)      279 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-crc.png
+-rw-rw-rw-   0     1001 root         (0)      280 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-econ.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fi.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fsps.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fss.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-law.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-med.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-ped.png
+-rw-rw-rw-   0     1001 root         (0)      281 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-phil.png
+-rw-rw-rw-   0     1001 root         (0)      280 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-sci.png
+-rw-rw-rw-   0     1001 root         (0)      149 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-small.png
+-rw-rw-rw-   0     1001 root         (0)      304 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select.png
+-rw-rw-rw-   0     1001 root         (0)     7406 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/favicon.ico
+-rw-rw-rw-   0     1001 root         (0)     4426 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png
+-rw-rw-rw-   0     1001 root         (0)      443 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/logo.svg
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.401358 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/
+-rw-rw-rw-   0     1001 root         (0)   218591 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/app.js
+-rw-rw-rw-   0     1001 root         (0)   659454 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/app.js.map
+-rw-rw-rw-   0     1001 root         (0)   337945 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/d3.js
+-rw-rw-rw-   0     1001 root         (0)     2707 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/documentation.js
+-rw-rw-rw-   0     1001 root         (0)     8806 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/graphs.js
+-rw-rw-rw-   0     1001 root         (0)    26171 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js
+-rw-rw-rw-   0     1001 root         (0)     4075 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js
+-rw-rw-rw-   0     1001 root         (0)   284394 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/jquery.js
+-rw-rw-rw-   0     1001 root         (0)   610160 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.353359 perun.proxygui-7.1.0/perun/proxygui/gui/static/bootstrap/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.401358 perun.proxygui-7.1.0/perun/proxygui/gui/static/bootstrap/css/
+-rw-rw-rw-   0     1001 root         (0)   155845 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css
+-rw-rw-rw-   0     1001 root         (0)   431289 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.401358 perun.proxygui-7.1.0/perun/proxygui/gui/static/bootstrap/js/
+-rw-rw-rw-   0     1001 root         (0)    78743 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0     1001 root         (0)   325834 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0     1001 root         (0)       78 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/campus-idp-muni.js
+-rw-rw-rw-   0     1001 root         (0)     7365 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/campus-idp.css
+-rw-rw-rw-   0     1001 root         (0)     4859 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/campus-idp.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.353359 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.401358 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/css/
+-rw-rw-rw-   0     1001 root         (0)    73577 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/css/all.css
+-rw-rw-rw-   0     1001 root         (0)    59305 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/css/all.min.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.405358 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/
+-rw-rw-rw-   0     1001 root         (0)   134294 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot
+-rw-rw-rw-   0     1001 root         (0)   747927 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg
+-rw-rw-rw-   0     1001 root         (0)   133988 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0     1001 root         (0)    89988 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff
+-rw-rw-rw-   0     1001 root         (0)    76736 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0     1001 root         (0)    34034 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot
+-rw-rw-rw-   0     1001 root         (0)   144714 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg
+-rw-rw-rw-   0     1001 root         (0)    33736 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0     1001 root         (0)    16276 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff
+-rw-rw-rw-   0     1001 root         (0)    13224 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0     1001 root         (0)   203030 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot
+-rw-rw-rw-   0     1001 root         (0)   918991 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg
+-rw-rw-rw-   0     1001 root         (0)   202744 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0     1001 root         (0)   101648 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff
+-rw-rw-rw-   0     1001 root         (0)    78268 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.405358 perun.proxygui-7.1.0/perun/proxygui/gui/static/images/
+-rw-rw-rw-   0     1001 root         (0)      490 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/images/check.svg
+-rw-rw-rw-   0     1001 root         (0)      536 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/images/circle-check-regular.svg
+-rw-rw-rw-   0     1001 root         (0)      483 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/images/circle-exclamation-solid.svg
+-rw-rw-rw-   0     1001 root         (0)      730 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/images/questionmark.svg
+-rw-rw-rw-   0     1001 root         (0)      625 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/images/spinner.svg
+-rw-rw-rw-   0     1001 root         (0)    89501 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/jquery-3.6.0.min.js
+-rw-rw-rw-   0     1001 root         (0)      627 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/proxygui.css
+-rw-rw-rw-   0     1001 root         (0)     1427 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/proxygui.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.353359 perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.405358 perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/
+-rw-rw-rw-   0     1001 root         (0)    15836 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css
+-rw-rw-rw-   0     1001 root         (0)     8266 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css
+-rw-rw-rw-   0     1001 root         (0)     8862 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css
+-rw-rw-rw-   0     1001 root         (0)     8873 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css
+-rw-rw-rw-   0     1001 root         (0)     7692 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/selectize.css
+-rw-rw-rw-   0     1001 root         (0)     8344 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/selectize.default.css
+-rw-rw-rw-   0     1001 root         (0)    11438 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/selectize.legacy.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.353359 perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/js/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.405358 perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/js/standalone/
+-rw-rw-rw-   0     1001 root         (0)    64906 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.409358 perun.proxygui-7.1.0/perun/proxygui/gui/templates/
+-rw-rw-rw-   0     1001 root         (0)    15205 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/ConsentRegistration.html
+-rw-rw-rw-   0     1001 root         (0)     9196 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/HeuristicData.html
+-rw-rw-rw-   0     1001 root         (0)      747 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/IsTestingSP.html
+-rw-rw-rw-   0     1001 root         (0)     3101 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/Logout.html
+-rw-rw-rw-   0     1001 root         (0)     1131 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/MfaResetEmailSent.html
+-rw-rw-rw-   0     1001 root         (0)     1942 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/MfaResetInitiated.html
+-rw-rw-rw-   0     1001 root         (0)     1133 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html
+-rw-rw-rw-   0     1001 root         (0)     1021 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/MfaResult.html
+-rw-rw-rw-   0     1001 root         (0)      795 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/MissingAuth.html
+-rw-rw-rw-   0     1001 root         (0)     1019 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/OidcError.html
+-rw-rw-rw-   0     1001 root         (0)     1223 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/Post-logout.html
+-rw-rw-rw-   0     1001 root         (0)      907 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/SPAuthorization.html
+-rw-rw-rw-   0     1001 root         (0)     2490 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/_footer.html
+-rw-rw-rw-   0     1001 root         (0)     8119 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/_header.html
+-rw-rw-rw-   0     1001 root         (0)     1175 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/authorization.html
+-rw-rw-rw-   0     1001 root         (0)     3477 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/base.html
+-rw-rw-rw-   0     1001 root         (0)      734 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/logout-canceled.html
+-rw-rw-rw-   0     1001 root         (0)      561 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/logout-iframe.html
+-rw-rw-rw-   0     1001 root         (0)     3769 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/templates/logout-state.html
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.353359 perun.proxygui-7.1.0/perun/proxygui/gui/translations/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.353359 perun.proxygui-7.1.0/perun/proxygui/gui/translations/cs/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.409358 perun.proxygui-7.1.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/
+-rw-rw-rw-   0     1001 root         (0)     2973 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo
+-rw-rw-rw-   0     1001 root         (0)     8108 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po
+-rw-rw-rw-   0     1001 root         (0)     5807 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/jwt.py
+-rw-rw-rw-   0     1001 root         (0)    20231 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/logout_manager.py
+-rw-rw-rw-   0     1001 root         (0)     2480 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/oauth.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.409358 perun.proxygui-7.1.0/perun/proxygui/openapi/
+-rw-rw-rw-   0     1001 root         (0)     6107 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/openapi/openapi.py
+-rw-rw-rw-   0     1001 root         (0)    12320 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/openapi/openapi_data.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.409358 perun.proxygui-7.1.0/perun/proxygui/openapi/schemas/
+-rw-rw-rw-   0     1001 root         (0)      982 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/openapi/schemas/arguments_schemas.py
+-rw-rw-rw-   0     1001 root         (0)     1401 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/openapi/schemas/response_schemas.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.409358 perun.proxygui-7.1.0/perun/proxygui/tests/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/tests/__init__.py
+-rw-rw-rw-   0     1001 root         (0)     1816 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/tests/shared_test_data.py
+-rw-rw-rw-   0     1001 root         (0)     9207 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/tests/test_ban_api.py
+-rw-rw-rw-   0     1001 root         (0)     6635 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/tests/test_consent_api.py
+-rw-rw-rw-   0     1001 root         (0)     4713 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/tests/test_consent_db.py
+-rw-rw-rw-   0     1001 root         (0)     2160 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/tests/test_consent_request_db.py
+-rw-rw-rw-   0     1001 root         (0)     6877 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/tests/test_gui.py
+-rw-rw-rw-   0     1001 root         (0)    23085 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/proxygui/user_manager.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.409358 perun.proxygui-7.1.0/perun/utils/
+-rw-rw-rw-   0     1001 root         (0)     2496 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/ConfigStore.py
+-rw-rw-rw-   0     1001 root         (0)       43 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/CustomExceptions.py
+-rw-rw-rw-   0     1001 root         (0)     2555 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/CustomRPHandler.py
+-rw-rw-rw-   0     1001 root         (0)     1545 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/DatabaseService.py
+-rw-rw-rw-   0     1001 root         (0)     4414 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/EmailService.py
+-rw-rw-rw-   0     1001 root         (0)       96 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/Notification.py
+-rw-rw-rw-   0     1001 root         (0)      816 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/Utils.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.409358 perun.proxygui-7.1.0/perun/utils/auth_event_loggig/
+-rw-rw-rw-   0     1001 root         (0)     2210 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/auth_event_loggig/AuthEventLoggingDbModels.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.413359 perun.proxygui-7.1.0/perun/utils/consent_framework/
+-rw-rw-rw-   0     1001 root         (0)     1241 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/consent_framework/consent.py
+-rw-rw-rw-   0     1001 root         (0)     2226 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/consent_framework/consent_db.py
+-rw-rw-rw-   0     1001 root         (0)     2274 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/consent_framework/consent_manager.py
+-rw-rw-rw-   0     1001 root         (0)      730 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/consent_framework/consent_request.py
+-rw-rw-rw-   0     1001 root         (0)     1371 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/consent_framework/consent_request_db.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.413359 perun.proxygui-7.1.0/perun/utils/logout_requests/
+-rw-rw-rw-   0     1001 root         (0)     2001 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/logout_requests/BackchannelLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)      832 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/logout_requests/FrontchannelLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     3841 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/logout_requests/GraphLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     1361 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/logout_requests/LogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     2204 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/perun/utils/logout_requests/SamlLogoutRequest.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 09:45:04.353359 perun.proxygui-7.1.0/perun.proxygui.egg-info/
+-rw-r--r--   0     1001 root         (0)     9220 2024-05-29 09:45:04.000000 perun.proxygui-7.1.0/perun.proxygui.egg-info/PKG-INFO
+-rw-r--r--   0     1001 root         (0)    12805 2024-05-29 09:45:04.000000 perun.proxygui-7.1.0/perun.proxygui.egg-info/SOURCES.txt
+-rw-r--r--   0     1001 root         (0)        1 2024-05-29 09:45:04.000000 perun.proxygui-7.1.0/perun.proxygui.egg-info/dependency_links.txt
+-rw-r--r--   0     1001 root         (0)      427 2024-05-29 09:45:04.000000 perun.proxygui-7.1.0/perun.proxygui.egg-info/requires.txt
+-rw-r--r--   0     1001 root         (0)        6 2024-05-29 09:45:04.000000 perun.proxygui-7.1.0/perun.proxygui.egg-info/top_level.txt
+-rw-rw-rw-   0     1001 root         (0)       90 2024-05-29 09:45:04.413359 perun.proxygui-7.1.0/setup.cfg
+-rw-rw-rw-   0     1001 root         (0)     1326 2024-05-29 09:44:25.000000 perun.proxygui-7.1.0/setup.py
```

### Comparing `perun.proxygui-7.0.0/LICENSE` & `perun.proxygui-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/PKG-INFO` & `perun.proxygui-7.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxygui
-Version: 7.0.0
+Version: 7.1.0
 Summary: Module with GUI and API for Perun ProxyIdP
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/proxyidp-gui.git
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Authlib==1.3.0
 Requires-Dist: setuptools
@@ -165,17 +165,17 @@
 
 - `HTTP OK [200]` indicating successfull load of search page
 
 **Endpoint:** `/heuristics/<user_id>`
 
 **Method:** `GET`
 
-**Description:** Used for showing gathered information about past athentications of user, and showing statistics based on that data.
+**Description:** Used for showing gathered information about past authentications of user, and showing statistics based on that data.
 
-**Performed MFA:** Gathered logs are checked if MFA was performed while handeling original logging event. Upstream ACRs values are compared to two hardcoded values: `https://refeds.org/profile/mfa` and `http://schemas.microsoft.com/claims/multipleauthn`
+**Performed MFA:** Gathered logs are checked if MFA was performed while handling the original logging event. Upstream ACRs values are compared to two hardcoded values: `https://refeds.org/profile/mfa` and `http://schemas.microsoft.com/claims/multipleauthn`. Database log for local MFA are checked apart from the upstream ACRs.
 
 **Input arguments:** ID of searched user
 
 **Result:**
 
 - `HTTP OK [200]` indicating successfull load of show page
 
@@ -235,12 +235,12 @@
 class delete_consent_schema(marshmallow.Schema):
     deleted = fields.Boolean()
     message = fields.String()
 ```
 
 - **Response / redirect / abort** - in case of these responses, scheme in response decorator can be custom (it is ignored when creating endpoint response)
 
-- **String** - redo to JSON with already created schema `string_schema` with only atribute `_text`. Then in response handeling add additional `json.loads()` wrapping function
+- **String** - redo to JSON with already created schema `string_schema` with only atribute `_text`. Then in response handling add additional `json.loads()` wrapping function
 
 ```python
 return jsonify({"_text": "Original String text"})
 ```
```

### Comparing `perun.proxygui-7.0.0/README.md` & `perun.proxygui-7.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -132,17 +132,17 @@
 
 - `HTTP OK [200]` indicating successfull load of search page
 
 **Endpoint:** `/heuristics/<user_id>`
 
 **Method:** `GET`
 
-**Description:** Used for showing gathered information about past athentications of user, and showing statistics based on that data.
+**Description:** Used for showing gathered information about past authentications of user, and showing statistics based on that data.
 
-**Performed MFA:** Gathered logs are checked if MFA was performed while handeling original logging event. Upstream ACRs values are compared to two hardcoded values: `https://refeds.org/profile/mfa` and `http://schemas.microsoft.com/claims/multipleauthn`
+**Performed MFA:** Gathered logs are checked if MFA was performed while handling the original logging event. Upstream ACRs values are compared to two hardcoded values: `https://refeds.org/profile/mfa` and `http://schemas.microsoft.com/claims/multipleauthn`. Database log for local MFA are checked apart from the upstream ACRs.
 
 **Input arguments:** ID of searched user
 
 **Result:**
 
 - `HTTP OK [200]` indicating successfull load of show page
 
@@ -202,12 +202,12 @@
 class delete_consent_schema(marshmallow.Schema):
     deleted = fields.Boolean()
     message = fields.String()
 ```
 
 - **Response / redirect / abort** - in case of these responses, scheme in response decorator can be custom (it is ignored when creating endpoint response)
 
-- **String** - redo to JSON with already created schema `string_schema` with only atribute `_text`. Then in response handeling add additional `json.loads()` wrapping function
+- **String** - redo to JSON with already created schema `string_schema` with only atribute `_text`. Then in response handling add additional `json.loads()` wrapping function
 
 ```python
 return jsonify({"_text": "Original String text"})
 ```
```

### Comparing `perun.proxygui-7.0.0/perun/proxygui/api/backchannel_logout_api.py` & `perun.proxygui-7.1.0/perun/proxygui/api/backchannel_logout_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/api/ban_api.py` & `perun.proxygui-7.1.0/perun/proxygui/api/ban_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/api/consent_api.py` & `perun.proxygui-7.1.0/perun/proxygui/api/consent_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/api/heuristic_api.py` & `perun.proxygui-7.1.0/perun/proxygui/api/heuristic_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from ipaddress import ip_address, ip_network
+
 from perun.utils.auth_event_loggig.AuthEventLoggingDbModels import (
     AuthEventLoggingTable,
     UserAgentTable,
     UserAgentRawTable,
     RequestedAcrsTable,
     LoggingSpTable,
     LoggingIdpTable,
@@ -15,15 +17,15 @@
 
 
 # Queries for fetching data from AuthEventMicroService
 class AuthEventLoggingQueries:
     def __init__(self, cfg):
         # Vars for storing arrays with DB responses
         self.auth_result = None  # Auth data, Upstream, Requested and Services
-        self.user_agents = None  # User agents and upstream logs
+        self.raw_user_agents = None  # User agents and upstream logs
         self.time_result = None  # Many AuthEvent logs
         # Nunbers of retrieved rows from DB for various data
         self.few_time_logs = cfg["heuristic_page"]["few_time_logs"]
         self.some_time_logs = cfg["heuristic_page"]["some_time_logs"]
         self.many_time_logs = cfg["heuristic_page"]["many_time_logs"]
         # DB connect string
         self.logging_db = cfg["heuristic_page"]["auth_event_logging"]["logging_db"]
@@ -46,37 +48,41 @@
             UserAgentRawTable.__table__,
             RequestedAcrsTable.__table__,
             LoggingSpTable.__table__,
             LoggingIdpTable.__table__,
             UpstreamAcrsTable.__table__,
             SessionIdTable.__table__,
         ]
+        self.private_ip_segments = cfg["heuristic_page"].get("private_ip_segments", [])
 
     # Modify ACRs value from string to list
     # '["acr1","acr2"]' -> ['acr1', 'acr2']
     # "acr1" -> ['acr1']
     def strip_acrs(self, acr):
         listed_acrs = acr.strip("][").split(",")
         for i, item in enumerate(listed_acrs):
             listed_acrs[i] = item.strip(" ").strip('"')
         return listed_acrs
 
-    # Simple function for return type of requested authenticaton
-    def requested_acr_status(self, raw_acr):
+    # Simple function for return type of requested authentication
+    def requested_acr_status(self, raw_acr, local_mfa_performed):
+        if local_mfa_performed:
+            return self.REQUEST_MFA_VALUE["required"]
+
         acr = self.strip_acrs(raw_acr)
         if not acr:
             return self.REQUEST_MFA_VALUE["other"]
         elif len(set(acr) - set(self.MFA_CONTEXTS)) == 0:
             return self.REQUEST_MFA_VALUE["required"]
         elif acr[0] in self.MFA_CONTEXTS:
             return self.REQUEST_MFA_VALUE["preferred"]
         else:
             return self.REQUEST_MFA_VALUE["other"]
 
-    # Beasic checker if MFA was performad based on upstream_acrs value
+    # Basic checker if MFA was performed based on upstream_acrs value
     def upstream_acr_status(self, acr):
         mfa_status = next((mfa for mfa in self.MFA_CONTEXTS if mfa in acr), None)
         return mfa_status is not None
 
     # Return specific number of logs from main table
     # Also joined in some requests
     def get_auth_logs(self, user_id):
@@ -85,28 +91,30 @@
             meta_data = MetaData()
             meta_data.reflect(engine)
 
             # Create all if not exists
             meta_data.create_all(cnxn, self.tables, checkfirst=True)
 
             auth_table = AuthEventLoggingTable().__table__
-            agents_table = UserAgentTable().__table__
+            agents_raw_table = UserAgentRawTable().__table__
             upstream_table = UpstreamAcrsTable().__table__
             requested_table = RequestedAcrsTable().__table__
             services_table = LoggingSpTable().__table__
 
             # Returns last 'self.short_time_logs' logs
             # for specific user, sorted
-            # by decending time joined with upstream ACRs, requested ACRs
+            # by descending time joined with upstream ACRs, requested ACRs
             # and services table
-            query = (
+
+            inner_query = (
                 select(
                     auth_table.c.day.label("day"),
                     auth_table.c.geolocation_city.label("geolocation_city"),
                     auth_table.c.geolocation_country.label("geolocation_country"),
+                    auth_table.c.local_mfa_performed.label("local_mfa_performed"),
                     auth_table.c.ip_address.label("ip_address"),
                     requested_table.c.value.label("requested_value"),
                     upstream_table.c.value.label("upstream_value"),
                     services_table.c.name.label("name"),
                     services_table.c.identifier.label("identifier"),
                 )
                 .select_from(auth_table)
@@ -115,18 +123,36 @@
                     requested_table.c.id == auth_table.c.requested_acrs_id,
                 )
                 .join(
                     upstream_table, upstream_table.c.id == auth_table.c.upstream_acrs_id
                 )
                 .join(services_table, services_table.c.id == auth_table.c.sp_id)
                 .where(auth_table.c.user_id == user_id)
-                .order_by(auth_table.c.day.desc())
+                .distinct(auth_table.c.ip_address)
+            ).alias("inner_query")
+
+            # Inner query allows to select distinct IPs and order by dates at the same time
+            outer_query = (
+                select(
+                    inner_query.c.day,
+                    inner_query.c.geolocation_city,
+                    inner_query.c.geolocation_country,
+                    inner_query.c.local_mfa_performed,
+                    inner_query.c.ip_address,
+                    inner_query.c.requested_value,
+                    inner_query.c.upstream_value,
+                    inner_query.c.name,
+                    inner_query.c.identifier,
+                )
+                .select_from(inner_query)
+                .order_by(inner_query.c.day.desc())
                 .limit(self.few_time_logs)
             )
-            response = cnxn.execute(query).fetchall()
+
+            response = cnxn.execute(outer_query).fetchall()
             self.auth_result = [r._asdict() for r in response]
 
             # Return last 'self.long_time_logs' logs
             # for user, sorted by time for logging graph
             query = (
                 auth_table.select()
                 .order_by(auth_table.c.day.desc())
@@ -136,74 +162,90 @@
             response = cnxn.execute(query).fetchall()
             self.time_result = [r._asdict() for r in response]
 
             # Returns joined values from user_agents and upstream_acrs
             # joined on auth_event_logging table
             query = (
                 select(
-                    agents_table.c.value.label("agent_value"),
+                    agents_raw_table.c.value.label("agent_value"),
                     upstream_table.c.value.label("upstream_value"),
+                    auth_table.c.local_mfa_performed.label("local_mfa_performed"),
                 )
                 .select_from(auth_table)
-                .join(agents_table, agents_table.c.id == auth_table.c.user_agent_id)
+                .join(
+                    agents_raw_table,
+                    agents_raw_table.c.id == auth_table.c.user_agent_id,
+                )
                 .join(
                     upstream_table, upstream_table.c.id == auth_table.c.upstream_acrs_id
                 )
                 .where(auth_table.c.user_id == user_id)
                 .order_by(auth_table.c.day.desc())
                 .limit(self.some_time_logs)
             )
             response = cnxn.execute(query).fetchall()
             # Returned dictionary:
             # {"agents_value": "val", "upstream_value": "val"}
-            self.user_agents = [r._asdict() for r in response]
+            self.raw_user_agents = [r._asdict() for r in response]
 
     # ----------------- Retrieving methods --------------
-    # Get information about last n cities (city name, timestamp, MFA performaed status)
+    # Get information about last n cities (city name, timestamp, MFA performed status)
     def get_last_n_cities(self):
         if self.auth_result is None:
             return []
 
         cities = []
 
-        # Retrieve relevant data from resluts
+        # Retrieve relevant data from results
         for item in self.auth_result:
-            city = item["geolocation_city"]
-            country = item["geolocation_country"]
+            city = item["geolocation_city"] or "Unknown city"
+            country = item["geolocation_country"] or "Unknown country"
             time = item["day"].strftime("%d. %m. %Y %H:%M")
             value = city + ", " + country + " (" + time + ")"
 
             cities.append(
                 {
                     "value": value,
-                    "mfa": self.upstream_acr_status(item["upstream_value"]),
+                    "mfa": self.upstream_acr_status(item["upstream_value"])
+                    or item["local_mfa_performed"],
                 }
             )
 
         return cities
 
-    # Retrieve inormation about last n IP addresses connected from
+    # Retrieve information about last n IP addresses connected from
     # (IP address, hostname lookup, MFA performed)
     def get_last_n_ips(self):
         if self.auth_result is None:
             return []
 
         ips = []
         for item in self.auth_result:
             ip = item["ip_address"]
             ip_lookup = getnameinfo((ip, 0), 0)[0]
             ip_string = ip if (ip == ip_lookup) else ip + " (" + ip_lookup + ")"
-            city = item["geolocation_city"]
-            country = item["geolocation_country"]
-            value = ip_string + ", " + city + ", " + country
+
+            private_ip_range_name = ""
+            for private_ip_range, range_name in self.private_ip_segments.items():
+                if ip_address(ip) in ip_network(private_ip_range):
+                    private_ip_range_name = range_name
+                    break
+
+            if private_ip_range_name:
+                value = f"{ip_string}, {private_ip_range_name}"
+            else:
+                city = item["geolocation_city"] or "Unknown city"
+                country = item["geolocation_country"] or "Unknown country"
+                value = f"{ip_string}, {city}, {country}"
 
             ips.append(
                 {
                     "value": value,
-                    "mfa": self.upstream_acr_status(item["upstream_value"]),
+                    "mfa": self.upstream_acr_status(item["upstream_value"])
+                    or item["local_mfa_performed"],
                 }
             )
 
         return ips
 
     # Retrive time statisctic from last n logs in AuthLogging table
     # retrun list in format to show Javascript graph [{"label": "8:00","value": 4},...]
@@ -217,59 +259,67 @@
                 "label": str(i) + ":00",
                 "value": sum(1 for item in self.time_result if item["day"].hour == i),
             }
             for i in range(1, 25)
         ]
         return json.dumps(times)
 
-    # Retieve data of used user agnets - compress same user agent and sort them by
-    # usage, MFA perfomed is True if it was performed at least once on that
+    # Retrieve data of used user agents - compress same user agent and sort them by
+    # usage, MFA performed is True if it was performed at least once on that
     # specific user agent
     def get_unique_user_agents(self):
-        if self.user_agents is None:
+        if self.raw_user_agents is None:
             return []
 
         agents = []
 
-        for item in self.user_agents:
+        for item in self.raw_user_agents:
             # Create default dictionary
-            mfa_performed = self.upstream_acr_status(item["upstream_value"])
+            mfa_performed = (
+                self.upstream_acr_status(item["upstream_value"])
+                or item["local_mfa_performed"]
+            )
             parsed_agent = str(parse(item["agent_value"]))
 
             index = next(
                 (i for i, item in enumerate(agents) if item["label"] == parsed_agent),
                 None,
             )
             if index is None:  # NEW User agent
                 agents.append(
                     {
                         "label": parsed_agent,
                         "value": 1,
                         "mfa": mfa_performed,
                     }
                 )
-            else:  # Alredy existing user agent, only actualize data
+            else:  # Already existing user agent, only update the data
                 agents[index]["value"] += 1
                 agents[index]["mfa"] |= mfa_performed
 
-        return sorted(agents, key=lambda d: d["value"], reverse=True)
+        sorted_agents = sorted(agents, key=lambda d: d["value"], reverse=True)
+
+        return sorted_agents
 
     # Retrieve data of used services, their name and identifier
     # Also with type of requested ACRs and upstream ACRs
     def get_last_n_services(self):
         if self.auth_result is None:
             return []
 
         services = []
 
         for item in self.auth_result:
-            requested_acrs = self.requested_acr_status(item["requested_value"])
+            requested_acrs = self.requested_acr_status(
+                item["requested_value"], item["local_mfa_performed"]
+            )
             upstream_acrs = self.upstream_acr_status(item["upstream_value"])
             services.append(
                 {
                     "name": item["name"],
                     "identifier": item["identifier"],
                     "requested_acrs": requested_acrs,
                     "upstream_acrs": upstream_acrs,
+                    "local_mfa_performed": item["local_mfa_performed"],
                 }
             )
         return services
```

### Comparing `perun.proxygui-7.0.0/perun/proxygui/app.py` & `perun.proxygui-7.1.0/perun/proxygui/app.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/gui.py` & `perun.proxygui-7.1.0/perun/proxygui/gui/gui.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/documentation.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/documentation.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/print.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/print.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-custom.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-custom.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-econ.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-econ.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fi.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-fi.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fss.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-fss.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-law.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-law.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-med.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-med.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-ped.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-ped.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-phil.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-phil.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style-sci.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style-sci.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/style.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/favicon.ico` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/app.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/app.js.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/d3.js` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/d3.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/documentation.js` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/documentation.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/graphs.js` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/graphs.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.js` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/jquery.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/campus-idp.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/campus-idp.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/campus-idp.js` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/campus-idp.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/css/all.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/css/all.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/css/all.min.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/images/circle-check-regular.svg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/images/circle-check-regular.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/images/questionmark.svg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/images/questionmark.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/images/spinner.svg` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/images/spinner.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/jquery-3.6.0.min.js` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/proxygui.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/proxygui.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/proxygui.js` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/proxygui.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/selectize.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/selectize.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/selectize.default.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/selectize.default.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/css/selectize.legacy.css` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/css/selectize.legacy.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js` & `perun.proxygui-7.1.0/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/ConsentRegistration.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/ConsentRegistration.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/HeuristicData.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/HeuristicData.html`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                                     </ul>
                                 </div>
                                 <div class="grid__cell size--l--5-12 col mx-5">
                                     <h5><span>{{ _("Last requested services") }}</span></h5>
                                     <ul>
                                     {% for service in sps %}
                                         <li>
-                                            {% if service.upstream_acrs %}
+                                            {% if service.upstream_acrs or service.local_mfa_performed %}
                                                 <span class="{% if cfg.css_framework == 'MUNI' %}
                                                 icon icon-user-check green {% else %}
                                                 fa fa-user-check {% endif %} success"
                                                 ></span>
                                             {% else %}
                                                 <span class="{% if cfg.css_framework == 'MUNI' %}
                                                 icon icon-user-slash  {% else %}
@@ -121,15 +121,15 @@
                                 </div>
                             </div>
                         </div>
                     {% else %}
                         <div class="content">
                             <br/>
                             <h3><span>{{ _("Specify a Perun user ID to gather data:") }}</span></h3>
-                            <form action="{{ url_for('gui.get_heuristic') }}" method="get">
+                            <form action="{{ url_for('gui.heuristics') }}" method="get">
                                 <input type="number" id="user_id" name="user_id" min="1" required placeholder="User ID">
                                 <p class="btn-wrap">
                                     <button class="btn btn-primary btn-s btn-accept"
                                             type="submit" name="submit">
                                         <span>Submit</span>
                                     </button>
                                 </p>
```

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/IsTestingSP.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/IsTestingSP.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/Logout.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/Logout.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/MfaResetEmailSent.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/MfaResetEmailSent.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/MfaResetInitiated.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/MfaResetInitiated.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/MfaResult.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/MfaResult.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/MissingAuth.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/MissingAuth.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/OidcError.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/OidcError.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/Post-logout.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/Post-logout.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/SPAuthorization.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/SPAuthorization.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/_footer.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/_footer.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/_header.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/_header.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/authorization.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/authorization.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/base.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/base.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/logout-canceled.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/logout-canceled.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/logout-iframe.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/logout-iframe.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/templates/logout-state.html` & `perun.proxygui-7.1.0/perun/proxygui/gui/templates/logout-state.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo` & `perun.proxygui-7.1.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po` & `perun.proxygui-7.1.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/jwt.py` & `perun.proxygui-7.1.0/perun/proxygui/jwt.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/logout_manager.py` & `perun.proxygui-7.1.0/perun/proxygui/logout_manager.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/oauth.py` & `perun.proxygui-7.1.0/perun/proxygui/oauth.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/openapi/openapi.py` & `perun.proxygui-7.1.0/perun/proxygui/openapi/openapi.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/openapi/openapi_data.py` & `perun.proxygui-7.1.0/perun/proxygui/openapi/openapi_data.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/openapi/schemas/arguments_schemas.py` & `perun.proxygui-7.1.0/perun/proxygui/openapi/schemas/arguments_schemas.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/openapi/schemas/response_schemas.py` & `perun.proxygui-7.1.0/perun/proxygui/openapi/schemas/response_schemas.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/tests/shared_test_data.py` & `perun.proxygui-7.1.0/perun/proxygui/tests/shared_test_data.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/tests/test_ban_api.py` & `perun.proxygui-7.1.0/perun/proxygui/tests/test_ban_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/tests/test_consent_api.py` & `perun.proxygui-7.1.0/perun/proxygui/tests/test_consent_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/tests/test_consent_db.py` & `perun.proxygui-7.1.0/perun/proxygui/tests/test_consent_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/tests/test_consent_request_db.py` & `perun.proxygui-7.1.0/perun/proxygui/tests/test_consent_request_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/tests/test_gui.py` & `perun.proxygui-7.1.0/perun/proxygui/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/proxygui/user_manager.py` & `perun.proxygui-7.1.0/perun/proxygui/user_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self._SUBJECT_ATTRIBUTE = USER_MANAGER_CFG.get(
             "perun_person_principal_names_attribute"
         )
         self._KEY_ID = USER_MANAGER_CFG["key_id"]
         self._KEYSTORE = USER_MANAGER_CFG["keystore"]
 
         if isinstance(cfg.get("heuristic_page", None), dict):
-            self._NAME_ATTRIBUTE = USER_MANAGER_CFG.get("heuristic_page", {}).get(
+            self._NAME_ATTRIBUTE = cfg.get("heuristic_page", {}).get(
                 "perun_user_name_attribute"
             )
 
         if isinstance(cfg.get("mfa_reset", None), dict):
             self.email_service = EmailService(cfg)
             self._PREFERRED_MAIL_ATTRIBUTE = cfg.get("mfa_reset", {}).get(
                 "preferred_mail_attribute"
@@ -53,16 +53,18 @@
         self.jwt_service = SingletonJWTServiceProvider.get_provider().get_service()
 
         self.logger = Logger.get_logger(__name__)
         self._cfg = USER_MANAGER_CFG
 
     def extract_user_attribute(self, attr_name: str, user_id: int) -> Any:
         user_attrs = self._ADAPTERS_MANAGER.get_user_attributes(user_id, [attr_name])
-        attr_value_candidates = user_attrs.get(attr_name, [])
-        attr_value = attr_value_candidates[0] if attr_value_candidates else None
+        attr_value_candidates = user_attrs.get(attr_name)
+        attr_value = attr_value_candidates
+        if attr_value_candidates and isinstance(attr_value_candidates, list):
+            attr_value = attr_value_candidates[0]
 
         return attr_value
 
     def _revoke_ssp_sessions(
         self,
         subject: str = None,
         session_id: str = None,
```

### Comparing `perun.proxygui-7.0.0/perun/utils/ConfigStore.py` & `perun.proxygui-7.1.0/perun/utils/ConfigStore.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/utils/CustomRPHandler.py` & `perun.proxygui-7.1.0/perun/utils/CustomRPHandler.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/utils/DatabaseService.py` & `perun.proxygui-7.1.0/perun/utils/DatabaseService.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/utils/EmailService.py` & `perun.proxygui-7.1.0/perun/utils/EmailService.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/utils/Utils.py` & `perun.proxygui-7.1.0/perun/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/utils/auth_event_loggig/AuthEventLoggingDbModels.py` & `perun.proxygui-7.1.0/perun/utils/auth_event_loggig/AuthEventLoggingDbModels.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-from sqlalchemy import (
-    Column,
-    String,
-    ForeignKey,
-    Integer,
-)
+from sqlalchemy import Column, String, ForeignKey, Integer, Boolean
 from sqlalchemy.dialects.postgresql import TIMESTAMP
 from sqlalchemy.orm import declarative_base
 
 Base = declarative_base()
 
 
 class AuthEventLoggingTable(Base):
@@ -18,14 +13,15 @@
     user = Column(String)
     user_id = Column(Integer)
     idp_id = Column(Integer, ForeignKey("logging_idp.id"))
     sp_id = Column(Integer, ForeignKey("logging_sp.id"))
     ip_address = Column(String)
     geolocation_city = Column(String)
     geolocation_country = Column(String)
+    local_mfa_performed = Column(Boolean, default=False)
     session_id = Column(Integer, ForeignKey("session_id_values.id"))
     requested_acrs_id = Column(Integer, ForeignKey("requested_acrs_values.id"))
     upstream_acrs_id = Column(Integer, ForeignKey("upstream_acrs_values.id"))
     user_agent_raw_id = Column(Integer, ForeignKey("user_agent_raw_values.id"))
     user_agent_id = Column(Integer, ForeignKey("user_agent_values.id"))
 
 
@@ -45,36 +41,36 @@
     name = Column(String)
 
 
 class SessionIdTable(Base):
     __tablename__ = "session_id_values"
 
     id = Column(Integer, primary_key=True)
-    value = Column(String)
+    value = Column(String, unique=True)
 
 
 class RequestedAcrsTable(Base):
     __tablename__ = "requested_acrs_values"
 
     id = Column(Integer, primary_key=True)
-    value = Column(String)
+    value = Column(String, unique=True)
 
 
 class UpstreamAcrsTable(Base):
     __tablename__ = "upstream_acrs_values"
 
     id = Column(Integer, primary_key=True)
-    value = Column(String)
+    value = Column(String, unique=True)
 
 
 class UserAgentRawTable(Base):
     __tablename__ = "user_agent_raw_values"
 
     id = Column(Integer, primary_key=True)
-    value = Column(String)
+    value = Column(String, unique=True)
 
 
 class UserAgentTable(Base):
     __tablename__ = "user_agent_values"
 
     id = Column(Integer, primary_key=True)
-    value = Column(String)
+    value = Column(String, unique=True)
```

### Comparing `perun.proxygui-7.0.0/perun/utils/consent_framework/consent.py` & `perun.proxygui-7.1.0/perun/utils/consent_framework/consent.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/utils/consent_framework/consent_db.py` & `perun.proxygui-7.1.0/perun/utils/consent_framework/consent_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/utils/consent_framework/consent_manager.py` & `perun.proxygui-7.1.0/perun/utils/consent_framework/consent_manager.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/utils/consent_framework/consent_request.py` & `perun.proxygui-7.1.0/perun/utils/consent_framework/consent_request.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/utils/consent_framework/consent_request_db.py` & `perun.proxygui-7.1.0/perun/utils/consent_framework/consent_request_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/utils/logout_requests/BackchannelLogoutRequest.py` & `perun.proxygui-7.1.0/perun/utils/logout_requests/BackchannelLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/utils/logout_requests/FrontchannelLogoutRequest.py` & `perun.proxygui-7.1.0/perun/utils/logout_requests/FrontchannelLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/utils/logout_requests/GraphLogoutRequest.py` & `perun.proxygui-7.1.0/perun/utils/logout_requests/GraphLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/utils/logout_requests/LogoutRequest.py` & `perun.proxygui-7.1.0/perun/utils/logout_requests/LogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun/utils/logout_requests/SamlLogoutRequest.py` & `perun.proxygui-7.1.0/perun/utils/logout_requests/SamlLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/perun.proxygui.egg-info/PKG-INFO` & `perun.proxygui-7.1.0/perun.proxygui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxygui
-Version: 7.0.0
+Version: 7.1.0
 Summary: Module with GUI and API for Perun ProxyIdP
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/proxyidp-gui.git
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Authlib==1.3.0
 Requires-Dist: setuptools
@@ -165,17 +165,17 @@
 
 - `HTTP OK [200]` indicating successfull load of search page
 
 **Endpoint:** `/heuristics/<user_id>`
 
 **Method:** `GET`
 
-**Description:** Used for showing gathered information about past athentications of user, and showing statistics based on that data.
+**Description:** Used for showing gathered information about past authentications of user, and showing statistics based on that data.
 
-**Performed MFA:** Gathered logs are checked if MFA was performed while handeling original logging event. Upstream ACRs values are compared to two hardcoded values: `https://refeds.org/profile/mfa` and `http://schemas.microsoft.com/claims/multipleauthn`
+**Performed MFA:** Gathered logs are checked if MFA was performed while handling the original logging event. Upstream ACRs values are compared to two hardcoded values: `https://refeds.org/profile/mfa` and `http://schemas.microsoft.com/claims/multipleauthn`. Database log for local MFA are checked apart from the upstream ACRs.
 
 **Input arguments:** ID of searched user
 
 **Result:**
 
 - `HTTP OK [200]` indicating successfull load of show page
 
@@ -235,12 +235,12 @@
 class delete_consent_schema(marshmallow.Schema):
     deleted = fields.Boolean()
     message = fields.String()
 ```
 
 - **Response / redirect / abort** - in case of these responses, scheme in response decorator can be custom (it is ignored when creating endpoint response)
 
-- **String** - redo to JSON with already created schema `string_schema` with only atribute `_text`. Then in response handeling add additional `json.loads()` wrapping function
+- **String** - redo to JSON with already created schema `string_schema` with only atribute `_text`. Then in response handling add additional `json.loads()` wrapping function
 
 ```python
 return jsonify({"_text": "Original String text"})
 ```
```

### Comparing `perun.proxygui-7.0.0/perun.proxygui.egg-info/SOURCES.txt` & `perun.proxygui-7.1.0/perun.proxygui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perun.proxygui-7.0.0/setup.py` & `perun.proxygui-7.1.0/setup.py`

 * *Files identical despite different names*

