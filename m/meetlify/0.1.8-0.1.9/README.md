# Comparing `tmp/meetlify-0.1.8.tar.gz` & `tmp/meetlify-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meetlify-0.1.8.tar", last modified: Sun May 26 20:39:52 2024, max compression
+gzip compressed data, was "meetlify-0.1.9.tar", last modified: Wed May 29 01:49:01 2024, max compression
```

## Comparing `meetlify-0.1.8.tar` & `meetlify-0.1.9.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.445495 meetlify-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-26 20:39:43.000000 meetlify-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-26 20:39:43.000000 meetlify-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-26 20:39:52.445495 meetlify-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-26 20:39:43.000000 meetlify-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-26 20:39:43.000000 meetlify-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-26 20:39:52.445495 meetlify-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-26 20:39:43.000000 meetlify-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.409494 meetlify-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.417495 meetlify-0.1.8/src/meetlify/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16047 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/meetups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/posts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/redirects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/robots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.417495 meetlify-0.1.8/src/meetlify/share/
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/share/configs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.413494 meetlify-0.1.8/src/meetlify/share/content/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.417495 meetlify-0.1.8/src/meetlify/share/content/images/
--rw-r--r--   0 runner    (1001) docker     (127)   128599 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/share/content/images/fatureimage.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.421495 meetlify-0.1.8/src/meetlify/share/content/meetups/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/share/content/meetups/0001.md
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/share/content/meetups/0002.md
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/share/content/meetups/0003.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.421495 meetlify-0.1.8/src/meetlify/share/content/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/share/content/pages/contact.md
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/share/content/pages/home.md
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/share/content/pages/privacy.md
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/share/content/pages/terms.md
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/share/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/sitemaps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.413494 meetlify-0.1.8/src/meetlify/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.413494 meetlify-0.1.8/src/meetlify/themes/lindau/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.413494 meetlify-0.1.8/src/meetlify/themes/lindau/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.421495 meetlify-0.1.8/src/meetlify/themes/lindau/static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   362926 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/assets/about.png
--rw-r--r--   0 runner    (1001) docker     (127)    50969 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/assets/author.png
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/assets/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/assets/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.437494 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    70329 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (127)   203221 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    51795 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   115986 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    70403 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   203225 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    51870 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   116063 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    65696 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (127)   129371 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    51369 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   129386 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    63943 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   107823 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css
--rw-r--r--   0 runner    (1001) docker     (127)   267535 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    85352 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   180381 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   107691 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   267476 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    85281 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   180217 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   281046 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   679755 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   232803 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589892 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   280259 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   679615 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   232911 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589087 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/cookiealert.css
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.437494 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   113656 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    85044 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   238987 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.441494 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)   207819 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   444579 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    80721 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   332090 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   135829 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.esm.js
--rw-r--r--   0 runner    (1001) docker     (127)   305438 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    73935 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   222455 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   145401 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)   306606 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    60635 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   220561 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/cookiealert.js
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/static/js/scripts.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.445495 meetlify-0.1.8/src/meetlify/themes/lindau/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/templates/categories.html
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/templates/category.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.445495 meetlify-0.1.8/src/meetlify/themes/lindau/templates/includes/
--rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/templates/includes/macros.html
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/templates/meetup.html
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/templates/meetups.html
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/templates/post.html
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/templates/posts.html
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/templates/sitemap-index.xml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/themes/lindau/templates/sitemap.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-26 20:39:43.000000 meetlify-0.1.8/src/meetlify/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.445495 meetlify-0.1.8/src/meetlify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-26 20:39:52.000000 meetlify-0.1.8/src/meetlify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-26 20:39:52.000000 meetlify-0.1.8/src/meetlify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 20:39:52.000000 meetlify-0.1.8/src/meetlify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-26 20:39:52.000000 meetlify-0.1.8/src/meetlify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 20:39:52.000000 meetlify-0.1.8/src/meetlify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-26 20:39:52.000000 meetlify-0.1.8/src/meetlify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 20:39:52.000000 meetlify-0.1.8/src/meetlify.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:52.445495 meetlify-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-26 20:39:43.000000 meetlify-0.1.8/tests/test_meetups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.728047 meetlify-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-29 01:48:52.000000 meetlify-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 01:48:52.000000 meetlify-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-29 01:49:01.728047 meetlify-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-29 01:48:52.000000 meetlify-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-29 01:48:52.000000 meetlify-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-29 01:49:01.728047 meetlify-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-29 01:48:52.000000 meetlify-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.692047 meetlify-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.696047 meetlify-0.1.9/src/meetlify/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16712 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/meetups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/redirects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/robots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.700047 meetlify-0.1.9/src/meetlify/share/
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/share/configs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.692047 meetlify-0.1.9/src/meetlify/share/content/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.700047 meetlify-0.1.9/src/meetlify/share/content/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   128599 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/share/content/images/fatureimage.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.700047 meetlify-0.1.9/src/meetlify/share/content/meetups/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/share/content/meetups/0001.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/share/content/meetups/0002.md
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/share/content/meetups/0003.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.700047 meetlify-0.1.9/src/meetlify/share/content/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/share/content/pages/contact.md
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/share/content/pages/home.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/share/content/pages/privacy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/share/content/pages/terms.md
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/share/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/sitemaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.692047 meetlify-0.1.9/src/meetlify/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.692047 meetlify-0.1.9/src/meetlify/themes/lindau/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.692047 meetlify-0.1.9/src/meetlify/themes/lindau/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.700047 meetlify-0.1.9/src/meetlify/themes/lindau/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   362926 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/assets/about.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50969 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/assets/author.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/assets/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/assets/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.716047 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    70329 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (127)   203221 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    51795 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   115986 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    70403 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   203225 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    51870 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   116063 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    65696 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (127)   129371 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    51369 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   129386 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    63943 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   107823 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css
+-rw-r--r--   0 runner    (1001) docker     (127)   267535 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    85352 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   180381 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   107691 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   267476 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    85281 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   180217 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   281046 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)   679755 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   232803 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   589892 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   280259 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   679615 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   232911 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   589087 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/cookiealert.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.716047 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   113656 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    85044 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   238987 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.720047 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   207819 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   444579 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    80721 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   332090 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   135829 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.esm.js
+-rw-r--r--   0 runner    (1001) docker     (127)   305438 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    73935 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   222455 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   145401 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)   306606 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    60635 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   220561 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/cookiealert.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/static/js/scripts.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.724047 meetlify-0.1.9/src/meetlify/themes/lindau/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/templates/categories.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/templates/category.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.724047 meetlify-0.1.9/src/meetlify/themes/lindau/templates/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/templates/includes/macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/templates/meetup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/templates/meetups.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/templates/post.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/templates/posts.html
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/templates/sitemap-index.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/themes/lindau/templates/sitemap.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-29 01:48:52.000000 meetlify-0.1.9/src/meetlify/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.724047 meetlify-0.1.9/src/meetlify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-29 01:49:01.000000 meetlify-0.1.9/src/meetlify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-29 01:49:01.000000 meetlify-0.1.9/src/meetlify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 01:49:01.000000 meetlify-0.1.9/src/meetlify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-29 01:49:01.000000 meetlify-0.1.9/src/meetlify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 01:49:01.000000 meetlify-0.1.9/src/meetlify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-29 01:49:01.000000 meetlify-0.1.9/src/meetlify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 01:49:01.000000 meetlify-0.1.9/src/meetlify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:49:01.724047 meetlify-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 01:48:52.000000 meetlify-0.1.9/tests/test_meetups.py
```

### Comparing `meetlify-0.1.8/LICENSE` & `meetlify-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/PKG-INFO` & `meetlify-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: meetlify
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python Package to Generate Meetup Websites
 Home-page: https://github.com/pybodensee/meetlify
-Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.8.tar.gz
+Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.9.tar.gz
 Author: Faisal Shahzad
 Author-email: pybodensee@gmail.com
 License: MIT
 Keywords: meetups,static-site-generators,seo,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
@@ -51,25 +51,25 @@
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Provides-Extra: all
-Requires-Dist: mkdocs-gen-files; extra == "all"
+Requires-Dist: wheel; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
 Requires-Dist: pymdown-extensions; extra == "all"
-Requires-Dist: black; extra == "all"
-Requires-Dist: wheel; extra == "all"
-Requires-Dist: pytest; extra == "all"
-Requires-Dist: setuptools; extra == "all"
 Requires-Dist: python-language-server[all]; extra == "all"
-Requires-Dist: mkdocstrings[python]; extra == "all"
 Requires-Dist: twine; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: black; extra == "all"
+Requires-Dist: mkdocstrings[python]; extra == "all"
 Requires-Dist: mkdocs; extra == "all"
+Requires-Dist: mkdocs-gen-files; extra == "all"
+Requires-Dist: setuptools; extra == "all"
 
 # meetlify
 
 Python based Static Site Genrators for Meetups/Meetup Webites.
 
 [![license](https://img.shields.io/pypi/l/meetlify.svg?style=flat-square "Project License: MIT")](https://github.com/pybodensee/meetlify/blob/master/LICENSE)
 [![status](https://img.shields.io/pypi/status/meetlify.svg?style=flat-square "Project Development Status")](https://github.com/pybodensee/meetlify/milestone/1)
@@ -114,14 +114,15 @@
 # Modify newly created config.json file as per your need.
 mtlfy = Meetlify(dest_=destination_path)
 mtlfy.render_home()
 mtlfy.render_404_page()
 mtlfy.render_meetups()
 mtlfy.render_posts()
 mtlfy.render_pages()
+mtlfy.render_categories()
 mtlfy.render_redirects()
 mtlfy.render_sitemaps()
 mtlfy.render_robots_txt()
 mtlfy.copy_assests()
 
 ```
```

### Comparing `meetlify-0.1.8/README.md` & `meetlify-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 # Modify newly created config.json file as per your need.
 mtlfy = Meetlify(dest_=destination_path)
 mtlfy.render_home()
 mtlfy.render_404_page()
 mtlfy.render_meetups()
 mtlfy.render_posts()
 mtlfy.render_pages()
+mtlfy.render_categories()
 mtlfy.render_redirects()
 mtlfy.render_sitemaps()
 mtlfy.render_robots_txt()
 mtlfy.copy_assests()
 
 ```
```

### Comparing `meetlify-0.1.8/setup.py` & `meetlify-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/__init__.py` & `meetlify-0.1.9/src/meetlify/__init__.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/api.py` & `meetlify-0.1.9/src/meetlify/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,23 +118,33 @@
             ),
             reverse_=True,
         )
 
         self.sitemaps = Sitemaps(
             sitemap_items_=[
                 {
-                    "name": "meetup",
+                    "name": self.configs.folders.pages,
+                    "items": self.pages[STATUS.PUBLISHED, STATUS.DONE],
+                    "robots_txt": True,
+                },
+                {
+                    "name": self.configs.folders.posts,
+                    "items": self.posts[STATUS.PUBLISHED, STATUS.DONE],
+                    "robots_txt": True,
+                },
+                {
+                    "name": self.configs.folders.meetups,
                     "items": self.meetups[STATUS.PUBLISHED, STATUS.DONE],
+                    "robots_txt": True,
                 },
-                {"name": "posts", "items": self.posts[STATUS.PUBLISHED, STATUS.DONE]},
                 {
-                    "name": "categories",
+                    "name": self.configs.folders.categories,
                     "items": self.categories[STATUS.PUBLISHED, STATUS.DONE],
+                    "robots_txt": True,
                 },
-                {"name": "pages", "items": self.pages[STATUS.PUBLISHED, STATUS.DONE]},
             ]
         )
 
         self.redirects = Redirects.from_json(Path(self.dest, "redirects.json"))
         self.robots = Robots.from_json(Path(self.dest, "robots.json"))
 
     def setup(self) -> None:
@@ -419,14 +429,23 @@
             mode="w",
             encoding="utf-8",
         ) as file:
             file.write(str(self.redirects))
             logging.info("... wrote output/redirects file")
 
     def render_robots_txt(self):
+        # Add additional sitemaps to Robots.txt if not added in robots.json
+        self.robots.add_sitemaps(
+            additional_sitems=[
+                sitemap.name
+                for sitemap in self.sitemaps[STATUS.PUBLISHED, STATUS.DONE]
+                if sitemap.robots_txt
+            ]
+        )
+
         if self.configs.robots:
             with open(
                 Path(
                     self.dest,
                     self.configs.folders.output,
                     "robots.txt",
                 ),
```

### Comparing `meetlify-0.1.8/src/meetlify/categories.py` & `meetlify-0.1.9/src/meetlify/categories.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/cli.py` & `meetlify-0.1.9/src/meetlify/cli.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/configs.py` & `meetlify-0.1.9/src/meetlify/configs.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/constants.py` & `meetlify-0.1.9/src/meetlify/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # DATABASE/CONSTANTS LIST
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 VERSION_MAJOR = 0
 VERSION_MINOR = 1
-VERSION_REVISION = 8
+VERSION_REVISION = 9
 
 FULL_VERSION = f"{VERSION_MAJOR}.{VERSION_MINOR}.{VERSION_REVISION}"
 
 
 class ExtendedEnum(Enum):
     """An extended enum class to convert list of items in an enumration."""
```

### Comparing `meetlify-0.1.8/src/meetlify/meetups.py` & `meetlify-0.1.9/src/meetlify/meetups.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/pages.py` & `meetlify-0.1.9/src/meetlify/pages.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/posts.py` & `meetlify-0.1.9/src/meetlify/posts.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/redirects.py` & `meetlify-0.1.9/src/meetlify/redirects.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/robots.py` & `meetlify-0.1.9/src/meetlify/robots.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,7 +92,10 @@
 
     @classmethod
     def from_json(cls, json_file_: Path) -> Self:
         assert isinstance(json_file_, Path)
         assert json_file_.exists()
         with codecs.open(str(json_file_), "r", encoding="utf-8") as f:
             return cls(robots_items_=json.load(f))
+
+    def add_sitemaps(self, additional_sitems: list[str]) -> None:
+        self.sitemaps += additional_sitems
```

### Comparing `meetlify-0.1.8/src/meetlify/share/__init__.py` & `meetlify-0.1.9/src/meetlify/share/__init__.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/share/configs.json` & `meetlify-0.1.9/src/meetlify/share/configs.json`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/share/content/images/fatureimage.png` & `meetlify-0.1.9/src/meetlify/share/content/images/fatureimage.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/share/content/meetups/0001.md` & `meetlify-0.1.9/src/meetlify/share/content/meetups/0001.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/share/content/meetups/0002.md` & `meetlify-0.1.9/src/meetlify/share/content/meetups/0002.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/share/content/meetups/0003.md` & `meetlify-0.1.9/src/meetlify/share/content/meetups/0003.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/share/content/pages/contact.md` & `meetlify-0.1.9/src/meetlify/share/content/pages/contact.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/share/content/pages/home.md` & `meetlify-0.1.9/src/meetlify/share/content/pages/home.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/share/content/pages/privacy.md` & `meetlify-0.1.9/src/meetlify/share/content/pages/privacy.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/share/content/pages/terms.md` & `meetlify-0.1.9/src/meetlify/share/content/pages/terms.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/sitemaps.py` & `meetlify-0.1.9/src/meetlify/sitemaps.py`

 * *Files 17% similar despite different names*

```diff
@@ -55,26 +55,28 @@
     slug: str
     last_modified: datetime
     urls: list
     images: list
     news: list
     videos: list
     status: STATUS
+    robots_txt: bool # Add to robots.txt
 
     @classmethod
     def from_dict(cls, object_: dict) -> Self:
         return cls(
             name=object_.get("name"),
             slug=object_.get("slug"),
             last_modified=object_.get("last_modified"),
             urls=object_.get("urls"),
             images=object_.get("images"),
             news=object_.get("news"),
             videos=object_.get("videos"),
             status=object_.get("status"),
+            robots_txt=object_.get("robots_txt"),
         )
 
 
 class Sitemaps:
     def __init__(self, *, sitemap_items_: list[dict]) -> None:
         self.all_sitemaps = [
             Sitemap.from_dict(
@@ -87,14 +89,15 @@
                         else datetime.now()
                     ),
                     "urls": sitemap_item.get("items"),
                     "images": [],
                     "news": [],
                     "videos": [],
                     "status": STATUS.PUBLISHED.value,
+                    "robots_txt": sitemap_item.get("robots_txt")
                 }
             )
             for sitemap_item in sitemap_items_
         ]
 
     def __getitem__(self, status_: list[STATUS] | STATUS) -> list[Sitemap]:
         if isinstance(status_, STATUS):
```

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/assets/about.png` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/assets/about.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/assets/author.png` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/assets/author.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/assets/banner.png` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/assets/banner.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/assets/favicon.png` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/assets/logo.png` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/assets/logo.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-icons.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.min.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/custom.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/css/styles.css` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/css/styles.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.esm.js` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.js` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.js.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.min.js` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/js/cookiealert.js` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/js/cookiealert.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/static/js/scripts.js` & `meetlify-0.1.9/src/meetlify/themes/lindau/static/js/scripts.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/templates/404.html` & `meetlify-0.1.9/src/meetlify/themes/lindau/templates/404.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/templates/base.html` & `meetlify-0.1.9/src/meetlify/themes/lindau/templates/base.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/templates/categories.html` & `meetlify-0.1.9/src/meetlify/themes/lindau/templates/categories.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/templates/category.html` & `meetlify-0.1.9/src/meetlify/themes/lindau/templates/category.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/templates/includes/macros.html` & `meetlify-0.1.9/src/meetlify/themes/lindau/templates/includes/macros.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/templates/index.html` & `meetlify-0.1.9/src/meetlify/themes/lindau/templates/index.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/templates/meetup.html` & `meetlify-0.1.9/src/meetlify/themes/lindau/templates/meetup.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/templates/meetups.html` & `meetlify-0.1.9/src/meetlify/themes/lindau/templates/meetups.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/templates/page.html` & `meetlify-0.1.9/src/meetlify/themes/lindau/templates/page.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/templates/post.html` & `meetlify-0.1.9/src/meetlify/themes/lindau/templates/post.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/themes/lindau/templates/posts.html` & `meetlify-0.1.9/src/meetlify/themes/lindau/templates/posts.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify/utils.py` & `meetlify-0.1.9/src/meetlify/utils.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/src/meetlify.egg-info/PKG-INFO` & `meetlify-0.1.9/src/meetlify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: meetlify
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python Package to Generate Meetup Websites
 Home-page: https://github.com/pybodensee/meetlify
-Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.8.tar.gz
+Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.9.tar.gz
 Author: Faisal Shahzad
 Author-email: pybodensee@gmail.com
 License: MIT
 Keywords: meetups,static-site-generators,seo,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
@@ -51,25 +51,25 @@
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Provides-Extra: all
-Requires-Dist: mkdocs-gen-files; extra == "all"
+Requires-Dist: wheel; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
 Requires-Dist: pymdown-extensions; extra == "all"
-Requires-Dist: black; extra == "all"
-Requires-Dist: wheel; extra == "all"
-Requires-Dist: pytest; extra == "all"
-Requires-Dist: setuptools; extra == "all"
 Requires-Dist: python-language-server[all]; extra == "all"
-Requires-Dist: mkdocstrings[python]; extra == "all"
 Requires-Dist: twine; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: black; extra == "all"
+Requires-Dist: mkdocstrings[python]; extra == "all"
 Requires-Dist: mkdocs; extra == "all"
+Requires-Dist: mkdocs-gen-files; extra == "all"
+Requires-Dist: setuptools; extra == "all"
 
 # meetlify
 
 Python based Static Site Genrators for Meetups/Meetup Webites.
 
 [![license](https://img.shields.io/pypi/l/meetlify.svg?style=flat-square "Project License: MIT")](https://github.com/pybodensee/meetlify/blob/master/LICENSE)
 [![status](https://img.shields.io/pypi/status/meetlify.svg?style=flat-square "Project Development Status")](https://github.com/pybodensee/meetlify/milestone/1)
@@ -114,14 +114,15 @@
 # Modify newly created config.json file as per your need.
 mtlfy = Meetlify(dest_=destination_path)
 mtlfy.render_home()
 mtlfy.render_404_page()
 mtlfy.render_meetups()
 mtlfy.render_posts()
 mtlfy.render_pages()
+mtlfy.render_categories()
 mtlfy.render_redirects()
 mtlfy.render_sitemaps()
 mtlfy.render_robots_txt()
 mtlfy.copy_assests()
 
 ```
```

### Comparing `meetlify-0.1.8/src/meetlify.egg-info/SOURCES.txt` & `meetlify-0.1.9/src/meetlify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.8/tests/test_meetups.py` & `meetlify-0.1.9/tests/test_meetups.py`

 * *Files identical despite different names*

