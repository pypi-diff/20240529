# Comparing `tmp/jam_py_v5-5.4.136.tar.gz` & `tmp/jam.py-v5-5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jam_py_v5-5.4.136.tar", last modified: Wed May 29 06:01:23 2024, max compression
+gzip compressed data, was "jam.py-v5-5.5.1.tar", last modified: Wed May 29 04:56:35 2024, max compression
```

## Comparing `jam_py_v5-5.4.136.tar` & `jam.py-v5-5.5.1.tar`

### file list

```diff
@@ -1,335 +1,335 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.169534 jam_py_v5-5.4.136/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/INSTALL
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-05-29 06:01:23.169534 jam_py_v5-5.4.136/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.105534 jam_py_v5-5.4.136/builder/
--rw-r--r--   0 runner    (1001) docker     (127)   476160 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/builder/admin.sqlite
--rw-r--r--   0 runner    (1001) docker     (127)    96256 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/builder/builder.sqlite
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.105534 jam_py_v5-5.4.136/builder/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/builder/css/project.css
--rw-r--r--   0 runner    (1001) docker     (127)  1340416 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/builder/demo.sqlite
--rw-r--r--   0 runner    (1001) docker     (127)    29348 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/builder/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.105534 jam_py_v5-5.4.136/builder/js/
--rw-r--r--   0 runner    (1001) docker     (127)   176860 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/builder/js/app_builder.js
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/builder/read.me
--rwxr-xr-x   0 runner    (1001) docker     (127)      199 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/builder/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.109534 jam_py_v5-5.4.136/demo/
--rw-r--r--   0 runner    (1001) docker     (127)   100352 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/admin.sqlite
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.109534 jam_py_v5-5.4.136/demo/css/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/css/project.css
--rw-r--r--   0 runner    (1001) docker     (127)  1340416 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/demo.sqlite
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.109534 jam_py_v5-5.4.136/demo/js/
--rw-r--r--   0 runner    (1001) docker     (127)    20163 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/js/demo.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.109534 jam_py_v5-5.4.136/demo/reports/
--rw-r--r--   0 runner    (1001) docker     (127)    11777 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/reports/customers.ods
--rw-r--r--   0 runner    (1001) docker     (127)    16387 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/reports/invoice.ods
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/reports/purchases.ods
--rwxr-xr-x   0 runner    (1001) docker     (127)      199 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.097535 jam_py_v5-5.4.136/demo/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.113534 jam_py_v5-5.4.136/demo/static/files/
--rw-r--r--   0 runner    (1001) docker     (127)   443926 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/files/SampleAudio_0.4mb2018-09-20_173200.101229.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    38183 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/files/adult-18792_6402018-09-20_172710.277885.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    41727 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/files/fashion-2082066_6402018-09-20_172551.982164.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    39451 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/files/girl-919048_6402018-09-20_172740.031997.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    40287 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/files/man-3122063_6402018-09-20_172535.467176.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    35660 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/files/model-2911330_6402018-09-20_172523.737081.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    66587 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/files/model-334739_6402018-10-03_102403.928076.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    49679 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/files/model-429733_6402018-09-20_175440.291794.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    49679 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/files/model-429733_6402019-04-25_101749.737955.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    41251 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/files/patient-841165_6402018-09-20_172615.389149.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    68392 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/files/smile-1885144_6402018-11-10_102150.945190.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    22964 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/files/stockvault-businessman-1282942018-09-20_172731.439691.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    25359 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/files/stockvault-businessman1196482018-09-20_172602.032986.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/files/sun-3588618_6402018-09-20_175413.562097.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.113534 jam_py_v5-5.4.136/demo/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/img/j.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.113534 jam_py_v5-5.4.136/demo/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)   152662 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/static/js/Chart.min.js
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/demo/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.117534 jam_py_v5-5.4.136/jam/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.117534 jam_py_v5-5.4.136/jam/admin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/admin/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    77018 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    91606 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/admin/builder_structure.info
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/admin/export_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    23406 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/admin/import_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    12464 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/admin/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.121534 jam_py_v5-5.4.136/jam/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/bin/jam-project.py
--rw-r--r--   0 runner    (1001) docker     (127)    29363 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/builder.html
--rw-r--r--   0 runner    (1001) docker     (127)    17896 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.129534 jam_py_v5-5.4.136/jam/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/admin.css
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/admin.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   154118 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-amelia.css
--rw-r--r--   0 runner    (1001) docker     (127)   128978 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-amelia.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   138575 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-cerulean.css
--rw-r--r--   0 runner    (1001) docker     (127)   115914 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-cerulean.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   140007 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-cosmo.css
--rw-r--r--   0 runner    (1001) docker     (127)   116730 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-cosmo.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   143783 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-flatly.css
--rw-r--r--   0 runner    (1001) docker     (127)   120480 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-flatly.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   138803 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-journal.css
--rw-r--r--   0 runner    (1001) docker     (127)   116103 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-journal.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-modal.css
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-modal.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   129089 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-readable.css
--rw-r--r--   0 runner    (1001) docker     (127)   108012 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-readable.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    22102 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-responsive.css
--rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-responsive.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   157033 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-slate.css
--rw-r--r--   0 runner    (1001) docker     (127)   132451 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-slate.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   139990 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-spacelab.css
--rw-r--r--   0 runner    (1001) docker     (127)   117471 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-spacelab.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   133112 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-united.css
--rw-r--r--   0 runner    (1001) docker     (127)   111493 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap-united.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   129105 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   107997 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/datepicker.css
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/datepicker.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/jam.css
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/jam.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/jam12.css
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/css/jam12.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    76439 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.129534 jam_py_v5-5.4.136/jam/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/db/db_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/db/firebird.py
--rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/db/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/db/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/db/oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/db/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/db/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/execute.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.129534 jam_py_v5-5.4.136/jam/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/img/glyphicons-halflings-white.png
--rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/img/glyphicons-halflings.png
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/img/j.ico
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/img/j.png
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/img/placeholder.png
--rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.137534 jam_py_v5-5.4.136/jam/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.137534 jam_py_v5-5.4.136/jam/js/ace/
--rw-r--r--   0 runner    (1001) docker     (127)   695915 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/ace/ace.js
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/ace/ext-searchbox.js
--rw-r--r--   0 runner    (1001) docker     (127)    31890 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/ace/mode-css.js
--rw-r--r--   0 runner    (1001) docker     (127)   101710 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/ace/mode-html.js
--rw-r--r--   0 runner    (1001) docker     (127)    31738 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/ace/mode-javascript.js
--rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/ace/mode-python.js
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/ace/mode-rst.js
--rw-r--r--   0 runner    (1001) docker     (127)   297488 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/ace/worker-css.js
--rw-r--r--   0 runner    (1001) docker     (127)   338277 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/ace/worker-html.js
--rw-r--r--   0 runner    (1001) docker     (127)   345289 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/ace/worker-javascript.js
--rw-r--r--   0 runner    (1001) docker     (127)   176860 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/admin.js
--rw-r--r--   0 runner    (1001) docker     (127)   144112 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/admin.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    20672 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/bootstrap-datepicker.js
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/bootstrap-datepicker.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    16982 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/bootstrap-modal.js
--rw-r--r--   0 runner    (1001) docker     (127)     8671 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/bootstrap-modal.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/bootstrap-modalmanager.js
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/bootstrap-modalmanager.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    62296 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)    34686 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   535294 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/jam.js
--rw-r--r--   0 runner    (1001) docker     (127)   278222 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/jam.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)    15119 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/jquery.maskedinput.js
--rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/jquery.maskedinput.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    86927 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/md5.js
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/js/md5.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    13844 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/langs.py
--rw-r--r--   0 runner    (1001) docker     (127)   178176 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/langs.sqlite
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.141534 jam_py_v5-5.4.136/jam/project/
--rw-r--r--   0 runner    (1001) docker     (127)    80896 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/project/admin.sqlite
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.141534 jam_py_v5-5.4.136/jam/project/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/project/css/project.css
--rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/project/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)      199 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/project/server.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/project/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    51112 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/server_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    42220 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.141534 jam_py_v5-5.4.136/jam/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.145534 jam_py_v5-5.4.136/jam/third_party/esprima/
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/character.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/comment_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/esprima.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/jsx_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    19998 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/jsx_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/jsx_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)   120670 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    37971 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/esprima/xhtml_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    12778 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/filelock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.145534 jam_py_v5-5.4.136/jam/third_party/jsmin/
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/jsmin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/jsmin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22889 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/jsmin/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/six.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.145534 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.145534 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/dialects/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/dialects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.149534 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    87111 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    25751 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    53901 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/default.py
--rw-r--r--   0 runner    (1001) docker     (127)    32869 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    47997 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    36074 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)    58764 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    15045 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/row.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/threadlocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.149534 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/event/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/event/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13853 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/event/attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/event/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/event/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/event/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    17563 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.149534 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/future/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/future/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/future/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12721 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.153534 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/pool/
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33086 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/pool/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/pool/dbapi_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/pool/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    14416 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/pool/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.157534 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    34222 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/coercions.py
--rw-r--r--   0 runner    (1001) docker     (127)   139738 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    26519 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    36186 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/ddl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/default_comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)    40331 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/dml.py
--rw-r--r--   0 runner    (1001) docker     (127)   158266 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    34153 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    42416 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)   164370 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)   153758 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)    99588 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/sqltypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    26190 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/traversals.py
--rw-r--r--   0 runner    (1001) docker     (127)    52521 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/type_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29908 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    24947 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/visitors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.157534 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26284 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    15939 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/deprecations.py
--rw-r--r--   0 runner    (1001) docker     (127)    50850 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/langhelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/topological.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.165534 jam_py_v5-5.4.136/jam/third_party/werkzeug/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/_reloader.py
--rw-r--r--   0 runner    (1001) docker     (127)   100436 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/datastructures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.165534 jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/
--rw-r--r--   0 runner    (1001) docker     (127)    17289 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/repr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.165534 jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/shared/console.png
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/shared/debugger.js
--rw-r--r--   0 runner    (1001) docker     (127)    88145 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/shared/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/shared/less.png
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/shared/more.png
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/shared/source.png
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/shared/style.css
--rw-r--r--   0 runner    (1001) docker     (127)    70220 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/shared/ubuntu.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    20363 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/tbtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    25188 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    21788 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/formparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    43052 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/http.py
--rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.165534 jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/http_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/lint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/proxy_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9581 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/shared_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/posixemulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    79252 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/routing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.169534 jam_py_v5-5.4.136/jam/third_party/werkzeug/secure_cookie/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/secure_cookie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/secure_cookie/securecookie.py
--rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/secure_cookie/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/security.py
--rw-r--r--   0 runner    (1001) docker     (127)    38694 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/serving.py
--rw-r--r--   0 runner    (1001) docker     (127)    39760 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/testapp.py
--rw-r--r--   0 runner    (1001) docker     (127)    39322 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/useragents.py
--rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.169534 jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/accept.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    26012 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/base_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    27784 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/base_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12829 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/common_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/etag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/user_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    84511 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)    34367 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/third_party/werkzeug/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    31651 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/jam/wsgi_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:01:23.169534 jam_py_v5-5.4.136/jam.py_v5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-05-29 06:01:23.000000 jam_py_v5-5.4.136/jam.py_v5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10112 2024-05-29 06:01:23.000000 jam_py_v5-5.4.136/jam.py_v5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:01:23.000000 jam_py_v5-5.4.136/jam.py_v5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-29 06:01:23.000000 jam_py_v5-5.4.136/jam.py_v5.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 06:01:23.169534 jam_py_v5-5.4.136/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-29 06:01:19.000000 jam_py_v5-5.4.136/setup.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.575744 jam.py-v5-5.5.1/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)       61 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/AUTHORS
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      959 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/INSTALL
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     1517 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/LICENSE
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      225 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/MANIFEST.in
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     7846 2024-05-29 04:56:35.571744 jam.py-v5-5.5.1/PKG-INFO
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     5396 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/README.rst
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.295744 jam.py-v5-5.5.1/builder/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   476160 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/builder/admin.sqlite
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    96256 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/builder/builder.sqlite
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.295744 jam.py-v5-5.5.1/builder/css/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     3995 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/builder/css/project.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)  1340416 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/builder/demo.sqlite
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    29348 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/builder/index.html
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.299744 jam.py-v5-5.5.1/builder/js/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   176860 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/builder/js/app_builder.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      742 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/builder/read.me
+-rwxrwxr-x   0 dbabic    (1000) dbabic    (1000)      199 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/builder/server.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.311744 jam.py-v5-5.5.1/demo/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   100352 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/admin.sqlite
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.311744 jam.py-v5-5.5.1/demo/css/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      425 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/css/project.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)  1340416 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/demo.sqlite
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    10165 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/index.html
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.311744 jam.py-v5-5.5.1/demo/js/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    20163 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/js/demo.js
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.311744 jam.py-v5-5.5.1/demo/reports/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    11777 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/reports/customers.ods
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    16387 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/reports/invoice.ods
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     8888 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/reports/purchases.ods
+-rwxrwxr-x   0 dbabic    (1000) dbabic    (1000)      199 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/server.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.275744 jam.py-v5-5.5.1/demo/static/
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.331744 jam.py-v5-5.5.1/demo/static/files/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   443926 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/files/SampleAudio_0.4mb2018-09-20_173200.101229.mp3
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    38183 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/files/adult-18792_6402018-09-20_172710.277885.jpg
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    41727 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/files/fashion-2082066_6402018-09-20_172551.982164.jpg
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    39451 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/files/girl-919048_6402018-09-20_172740.031997.jpg
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    40287 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/files/man-3122063_6402018-09-20_172535.467176.jpg
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    35660 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/files/model-2911330_6402018-09-20_172523.737081.jpg
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    66587 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/files/model-334739_6402018-10-03_102403.928076.jpg
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    49679 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/files/model-429733_6402018-09-20_175440.291794.jpg
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    49679 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/files/model-429733_6402019-04-25_101749.737955.jpg
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    41251 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/files/patient-841165_6402018-09-20_172615.389149.jpg
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    68392 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/files/smile-1885144_6402018-11-10_102150.945190.jpg
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    22964 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/files/stockvault-businessman-1282942018-09-20_172731.439691.jpg
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    25359 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/files/stockvault-businessman1196482018-09-20_172602.032986.jpg
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    12150 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/files/sun-3588618_6402018-09-20_175413.562097.jpg
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.331744 jam.py-v5-5.5.1/demo/static/img/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      379 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/img/j.png
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.331744 jam.py-v5-5.5.1/demo/static/js/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   152662 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/static/js/Chart.min.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)       85 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/demo/wsgi.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.343744 jam.py-v5-5.5.1/jam/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)       77 2024-05-28 03:42:54.000000 jam.py-v5-5.5.1/jam/__init__.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.351744 jam.py-v5-5.5.1/jam/admin/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)        0 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/admin/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     7429 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/admin/admin.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    77018 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/admin/builder.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    91606 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/admin/builder_structure.info
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     3800 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/admin/export_metadata.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    23406 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/admin/import_metadata.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    12464 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/admin/task.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.351744 jam.py-v5-5.5.1/jam/bin/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     1147 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/bin/jam-project.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    29363 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/builder.html
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    17896 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/common.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.395744 jam.py-v5-5.5.1/jam/css/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     3995 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/admin.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     2557 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/admin.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   154118 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-amelia.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   128978 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-amelia.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   138575 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-cerulean.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   115914 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-cerulean.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   140007 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-cosmo.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   116730 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-cosmo.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   143783 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-flatly.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   120480 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-flatly.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   138803 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-journal.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   116103 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-journal.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     4604 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-modal.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     3093 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-modal.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   129089 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-readable.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   108012 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-readable.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    22102 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-responsive.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    16634 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-responsive.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   157033 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-slate.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   132451 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-slate.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   139990 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-spacelab.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   117471 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-spacelab.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   133112 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-united.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   111493 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap-united.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   129105 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   107997 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/bootstrap.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     5076 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/datepicker.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     4094 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/datepicker.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    10993 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/jam.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     8462 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/jam.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    13624 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/jam12.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    10570 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/css/jam12.min.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    76439 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/dataset.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.399744 jam.py-v5-5.5.1/jam/db/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)        0 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/db/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      580 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/db/db_modules.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     8235 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/db/firebird.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     9431 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/db/mssql.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     7629 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/db/mysql.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     8003 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/db/oracle.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     7891 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/db/postgres.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     4969 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/db/sqlite.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     6318 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/events.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     6681 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/execute.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.403744 jam.py-v5-5.5.1/jam/img/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     8777 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/img/glyphicons-halflings-white.png
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    12799 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/img/glyphicons-halflings.png
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     1150 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/img/j.ico
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      379 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/img/j.png
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     2076 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/img/placeholder.png
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    11737 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/items.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.431744 jam.py-v5-5.5.1/jam/js/
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.451744 jam.py-v5-5.5.1/jam/js/ace/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   695915 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/ace/ace.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    16652 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/ace/ext-searchbox.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    31890 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/ace/mode-css.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   101710 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/ace/mode-html.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    31738 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/ace/mode-javascript.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     9090 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/ace/mode-python.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     5966 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/ace/mode-rst.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   297488 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/ace/worker-css.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   338277 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/ace/worker-html.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   345289 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/ace/worker-javascript.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   176860 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/admin.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   144112 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/admin.min.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    20672 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/bootstrap-datepicker.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    10159 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/bootstrap-datepicker.min.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    16982 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/bootstrap-modal.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     8671 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/bootstrap-modal.min.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    16307 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/bootstrap-modalmanager.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     8668 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/bootstrap-modalmanager.min.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    62296 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/bootstrap.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    34686 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/bootstrap.min.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   535294 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/jam.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   278222 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/jam.min.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   271751 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/jquery.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    15119 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/jquery.maskedinput.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     6605 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/jquery.maskedinput.min.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    86927 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/jquery.min.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    12297 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/md5.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     5283 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/js/md5.min.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    13844 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/langs.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   178176 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/langs.sqlite
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.455744 jam.py-v5-5.5.1/jam/project/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    80896 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/project/admin.sqlite
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.455744 jam.py-v5-5.5.1/jam/project/css/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)        0 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/project/css/project.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     8868 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/project/index.html
+-rwxrwxr-x   0 dbabic    (1000) dbabic    (1000)      199 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/project/server.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)       85 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/project/wsgi.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    51112 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/server_classes.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    42220 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/sql.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.459744 jam.py-v5-5.5.1/jam/third_party/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)        0 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/__init__.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.475744 jam.py-v5-5.5.1/jam/third_party/esprima/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     1481 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     4419 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/__main__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     4665 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/character.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     6486 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/comment_handler.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     2497 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/compat.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     2906 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/error_handler.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     4350 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/esprima.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     3339 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/jsx_nodes.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    19998 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/jsx_parser.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     1876 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/jsx_syntax.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     5597 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/messages.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    16212 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/nodes.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     1847 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/objects.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   120670 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/parser.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    37971 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/scanner.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     4334 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/syntax.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     2055 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/token.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     7470 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/tokenizer.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     1781 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/utils.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     9554 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/visitor.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     7189 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/esprima/xhtml_entities.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    12778 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/filelock.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.475744 jam.py-v5-5.5.1/jam/third_party/jsmin/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     8913 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/jsmin/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     1538 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/jsmin/__main__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    22889 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/jsmin/test.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    30628 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/six.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.483744 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     4649 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/__init__.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.483744 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/dialects/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     1349 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/dialects/__init__.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.495744 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     2036 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    87111 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/base.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    25751 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/create.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    53901 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/default.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    32869 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/events.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    47997 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/interfaces.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     3617 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/mock.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    36074 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/reflection.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    58764 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/result.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    15045 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/row.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      413 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/strategies.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     4746 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/threadlocal.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     9411 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/url.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     2421 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/util.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.499744 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/event/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      596 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/event/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     7085 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/event/api.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    13853 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/event/attr.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     9753 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/event/base.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     5904 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/event/legacy.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     8243 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/event/registry.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      506 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/events.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    17563 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/exc.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.499744 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/future/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      469 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/future/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     5119 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/future/result.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     2990 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/inspection.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    12721 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/interfaces.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     6693 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/log.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.503744 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/pool/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     1480 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/pool/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    33086 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/pool/base.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     4228 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/pool/dbapi_proxy.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     8356 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/pool/events.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    14416 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/pool/impl.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     5744 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/processors.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     2371 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/schema.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.527744 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     4481 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     9973 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/annotation.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    34222 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/base.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    21899 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/coercions.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   139738 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/compiler.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    26519 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/crud.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    36186 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/ddl.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     9639 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/default_comparator.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    40331 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/dml.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   158266 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/elements.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    10993 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/events.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     8561 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/expression.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    34153 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/functions.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     5888 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/naming.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    42416 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/operators.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     4764 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/roles.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   164370 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/schema.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   153758 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/selectable.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    99588 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/sqltypes.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    26190 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/traversals.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    52521 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/type_api.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    29908 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/util.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    24947 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/visitors.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     3377 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/types.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.535744 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     6672 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    26284 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/_collections.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    15939 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/compat.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     8156 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/deprecations.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    50850 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/langhelpers.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     6558 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/queue.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     2767 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/topological.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.547744 jam.py-v5-5.5.1/jam/third_party/werkzeug/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      502 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     6671 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/_compat.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    14351 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/_internal.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    11531 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/_reloader.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)   100436 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/datastructures.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.551744 jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    17289 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     5461 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/console.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     9621 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/repr.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.555744 jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/shared/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      507 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/shared/console.png
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     6400 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/shared/debugger.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    88145 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/shared/jquery.js
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      191 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/shared/less.png
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      200 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/shared/more.png
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      818 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/shared/source.png
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     6604 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/shared/style.css
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    70220 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/shared/ubuntu.ttf
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    20363 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/tbtools.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    25188 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/exceptions.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     2101 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/filesystem.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    21788 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/formparser.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    43052 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/http.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    14371 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/local.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.563744 jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      549 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     2240 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/dispatcher.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     7117 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/http_proxy.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    12967 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/lint.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     4471 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/profiler.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     6431 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/proxy_fix.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     9581 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/shared_data.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     3541 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/posixemulation.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    79252 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/routing.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.567744 jam.py-v5-5.5.1/jam/third_party/werkzeug/secure_cookie/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)       24 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/secure_cookie/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    12369 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/secure_cookie/securecookie.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    11703 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/secure_cookie/sessions.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     8106 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/security.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    38694 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/serving.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    39760 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/test.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     9329 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/testapp.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    39322 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/urls.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     5451 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/useragents.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    25251 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/utils.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    11344 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/websocket.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.571744 jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     1384 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/__init__.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     1760 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/accept.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     1158 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/auth.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    26012 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/base_request.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    27784 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/base_response.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    12829 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/common_descriptors.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     3466 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/cors.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    12217 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/etag.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     4343 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/json.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     1514 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/request.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     2524 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/response.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      435 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/user_agent.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    84511 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    34367 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/third_party/werkzeug/wsgi.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    31651 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/wsgi.py
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)      259 2024-05-27 05:57:49.000000 jam.py-v5-5.5.1/jam/wsgi_server.py
+drwxrwxr-x   0 dbabic    (1000) dbabic    (1000)        0 2024-05-29 04:56:35.343744 jam.py-v5-5.5.1/jam.py_v5.egg-info/
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     7846 2024-05-29 04:56:35.000000 jam.py-v5-5.5.1/jam.py_v5.egg-info/PKG-INFO
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)    10112 2024-05-29 04:56:35.000000 jam.py-v5-5.5.1/jam.py_v5.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)        1 2024-05-29 04:56:35.000000 jam.py-v5-5.5.1/jam.py_v5.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)        4 2024-05-29 04:56:35.000000 jam.py-v5-5.5.1/jam.py_v5.egg-info/top_level.txt
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)       38 2024-05-29 04:56:35.575744 jam.py-v5-5.5.1/setup.cfg
+-rw-rw-r--   0 dbabic    (1000) dbabic    (1000)     2310 2024-05-29 04:56:17.000000 jam.py-v5-5.5.1/setup.py
```

### Comparing `jam_py_v5-5.4.136/INSTALL` & `jam.py-v5-5.5.1/INSTALL`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/LICENSE` & `jam.py-v5-5.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/PKG-INFO` & `jam.py-v5-5.5.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,163 @@
 Metadata-Version: 2.1
 Name: jam.py-v5
-Version: 5.4.136
+Version: 5.5.1
 Summary: Jam.py Application Builder is an event-driven framework for the development of web database applications.
 Home-page: http://jam-py.com/
 Author: Andrew Yushev
 Author-email: andrew@jam-py.com
 License: BSD
+Description: 
+        .. image:: https://img.shields.io/pypi/v/jam.py.svg
+           :target: https://pypi.org/project/jam.py/
+           :alt: Package on PyPI
+        
+        .. image:: https://img.shields.io/pypi/pyversions/jam.py.svg
+           :target: https://pypi.python.org/pypi/jam.py
+           :alt: Supported Python Versions
+        
+        .. image:: https://readthedocs.org/projects/jam-py/badge/?version=stable
+           :target: http://jam-py.com/docs/
+           :alt: Documentation Status
+        
+        .. image:: https://api.travis-ci.org/platipusica/jam-py.png?branch=master
+           :target: http://travis-ci.org/platipusica/jam-py
+           :alt: Build Status (Travis CI)
+        
+        
+        
+        ================
+        Jam.py Application Builder (web framework)
+        ================
+        
+        
+        From an idea of a web database application to a live website in no time, for free
+        =================================================================================
+        
+        Click on the image to see the online demo
+        
+        .. figure:: demo/static/img/JAMPY_Readme.gif
+            :width: 100%
+            :align: center
+            :alt: Online demo
+            :target: https://demo.jam-py.com/
+        
+        
+        If you are not a professional programmer or an expert in databases, you can use
+        Jam.py to store, share and analyze your data.
+            
+        Please watch these videos to see how easy it is to create and setup Jam.py
+        applications.
+        
+        * `Creating CRM web database applications from start to finish in 7 minutes with Jam.py framework <https://youtu.be/vY6FTdpABa4>`_
+        * `Setting up interface of Jam.py application using Forms Dialogs <https://youtu.be/hvNZ0-a_HHw>`_
+        
+        If you are a professional, you can use Jam.py to create various tools, dashboards,
+        as well as large-scale business applications with complex internal logic.
+        Please watch the
+        `Jam.py framework applications <https://youtu.be/qkJvGlgoabU>`_  video
+        to see some applications written in Jam.py.
+        
+        More demos on PythonAnywhere:
+        
+        * `SAP Theme Demo <https://jampyapp.pythonanywhere.com/>`_
+        * `Personal Account Ledger from MS Access template <https://msaccess.pythonanywhere.com/>`_
+        * `NorthWind Traders from MS Access template (wip) <https://northwind.pythonanywhere.com/>`_
+        * `The ERP POC Demo with Italian and English translations <https://sem.pythonanywhere.com/>`_
+        * `Assets/Parts Application (wip, currently Jam V7 Demo) <https://jampy.pythonanywhere.com>`_
+        * `Machine Learning (wip) <https://mlearning.pythonanywhere.com>`_
+        * `Auto Parts Sales for Brazilian Market (Portuguese) <https://carparts.pythonanywhere.com>`_
+        * `Resourcing and Billing Application from MS Access DB (wip) <https://resourcingandbilling.pythonanywhere.com>`_
+        * `Job Positions tracking App from MS Access DB (wip) <https://positionstracking.pythonanywhere.com>`_
+        * `Kanban/Tasks Application <https://kanban.pythonanywhere.com>`_
+        * `Assets Inventory Application (wip) <https://assetinventory.pythonanywhere.com>`_
+        
+        
+        Jam.py alternative site:
+        
+        * `https://jampyapplicationbuilder.com/`
+        
+        
+        Main features
+        =============
+        
+        Jam.py is an object oriented, event driven framework with hierarchical structure, modular design
+        and very tight DB/GUI coupling. The server side of Jam.py is written in `Python <https://www.python.org">`_,
+        the client utilizes `JavaScript <https://developer.mozilla.org/en/docs/Web/JavaScript">`_,
+        `jQuery <https://jquery.com">`_ and `Bootstrap <http://getbootstrap.com/2.3.2">`_.
+        
+        * Simple, clear and efficient IDE. The development takes place in the
+          Application builder, an application written completely in Jam.py.
+        
+        * “All in the browser” framework. With Jam.py, all you need are two pages
+          in the browser, one for the project, the other for the Application builder.
+          Make changes in the Application builder, go to the project, refresh the page,
+          and see the results.
+        
+        * Supports SQLite, PostgreSQL, MySQL, Firebird, MSSQL and
+          Oracle databases. The concept of the framework allows you to migrate from
+          one database to another without changing the project.
+        
+        * Authentication, authorization, session management, roles and permissions.
+        
+        * Automatic creation and modification of database tables and SQL queries generation.
+        
+        * Data-aware controls.
+        
+        * Open framework. You can use any Javascript/Python libraries.
+        
+        * Rich, informative reports. Band-oriented report generation based on
+          `LibreOffice <https://www.libreoffice.org/>`_ templates.
+        
+        * Charts. You can use free `jsCharts <http://www.jscharts.com/>`_ library
+          or any javascript charting library to create charts to represent and analyze your application data.
+        
+        * Allows to save audit trail/change history made by users
+        
+        * Predefined css themes.
+        
+        * Develop and test locally update remotely. Jam.py has Export and Import
+          utilities that allow developer to store all metadata (database structures,
+          project parameters and code) in a file that can be loaded by another
+          application to apply all the changes.
+        
+        Documentation
+        =============
+        
+        All documentation is in the "docs" directory and online at
+        http://jam-py.com/docs/.
+        
+        Please visit http://jam-py.com/docs/intro/install.html for Python and
+        framework installation or http://jam-py.com/docs/intro/new_project.html how to create a
+        new project.
+        
+        For general discussion, ideas or similar, please visit mailgroup https://groups.google.com/g/jam-py or
+        FB page https://www.facebook.com/groups/jam.py/
+        
+        Demo application: http://demo.jam-py.com/
+        
+        
+        
+        License
+        =======
+        
+        Jam.py is licensed under the BSD License.
+        
+        Author
+        ======
+        
+        Andrew Yushev
+        
+        See also the list of `contributors <http://jam-py.com/contributors.html>`_
+        who participated in this project.
+        
+        
+        
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -22,156 +170,7 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-
-
-.. image:: https://img.shields.io/pypi/v/jam.py.svg
-   :target: https://pypi.org/project/jam.py/
-   :alt: Package on PyPI
-
-.. image:: https://img.shields.io/pypi/pyversions/jam.py.svg
-   :target: https://pypi.python.org/pypi/jam.py
-   :alt: Supported Python Versions
-
-.. image:: https://readthedocs.org/projects/jam-py/badge/?version=stable
-   :target: http://jam-py.com/docs/
-   :alt: Documentation Status
-
-.. image:: https://api.travis-ci.org/platipusica/jam-py.png?branch=master
-   :target: http://travis-ci.org/platipusica/jam-py
-   :alt: Build Status (Travis CI)
-
-
-
-================
-Jam.py Application Builder (web framework)
-================
-
-
-From an idea of a web database application to a live website in no time, for free
-=================================================================================
-
-Click on the image to see the online demo
-
-.. figure:: demo/static/img/JAMPY_Readme.gif
-    :width: 100%
-    :align: center
-    :alt: Online demo
-    :target: https://demo.jam-py.com/
-
-
-If you are not a professional programmer or an expert in databases, you can use
-Jam.py to store, share and analyze your data.
-    
-Please watch these videos to see how easy it is to create and setup Jam.py
-applications.
-
-* `Creating CRM web database applications from start to finish in 7 minutes with Jam.py framework <https://youtu.be/vY6FTdpABa4>`_
-* `Setting up interface of Jam.py application using Forms Dialogs <https://youtu.be/hvNZ0-a_HHw>`_
-
-If you are a professional, you can use Jam.py to create various tools, dashboards,
-as well as large-scale business applications with complex internal logic.
-Please watch the
-`Jam.py framework applications <https://youtu.be/qkJvGlgoabU>`_  video
-to see some applications written in Jam.py.
-
-More demos on PythonAnywhere:
-
-* `SAP Theme Demo <https://jampyapp.pythonanywhere.com/>`_
-* `Personal Account Ledger from MS Access template <https://msaccess.pythonanywhere.com/>`_
-* `NorthWind Traders from MS Access template (wip) <https://northwind.pythonanywhere.com/>`_
-* `The ERP POC Demo with Italian and English translations <https://sem.pythonanywhere.com/>`_
-* `Assets/Parts Application (wip, currently Jam V7 Demo) <https://jampy.pythonanywhere.com>`_
-* `Machine Learning (wip) <https://mlearning.pythonanywhere.com>`_
-* `Auto Parts Sales for Brazilian Market (Portuguese) <https://carparts.pythonanywhere.com>`_
-* `Resourcing and Billing Application from MS Access DB (wip) <https://resourcingandbilling.pythonanywhere.com>`_
-* `Job Positions tracking App from MS Access DB (wip) <https://positionstracking.pythonanywhere.com>`_
-* `Kanban/Tasks Application <https://kanban.pythonanywhere.com>`_
-* `Assets Inventory Application (wip) <https://assetinventory.pythonanywhere.com>`_
-
-
-Jam.py alternative site:
-
-* `https://jampyapplicationbuilder.com/`
-
-
-Main features
-=============
-
-Jam.py is an object oriented, event driven framework with hierarchical structure, modular design
-and very tight DB/GUI coupling. The server side of Jam.py is written in `Python <https://www.python.org">`_,
-the client utilizes `JavaScript <https://developer.mozilla.org/en/docs/Web/JavaScript">`_,
-`jQuery <https://jquery.com">`_ and `Bootstrap <http://getbootstrap.com/2.3.2">`_.
-
-* Simple, clear and efficient IDE. The development takes place in the
-  Application builder, an application written completely in Jam.py.
-
-* “All in the browser” framework. With Jam.py, all you need are two pages
-  in the browser, one for the project, the other for the Application builder.
-  Make changes in the Application builder, go to the project, refresh the page,
-  and see the results.
-
-* Supports SQLite, PostgreSQL, MySQL, Firebird, MSSQL and
-  Oracle databases. The concept of the framework allows you to migrate from
-  one database to another without changing the project.
-
-* Authentication, authorization, session management, roles and permissions.
-
-* Automatic creation and modification of database tables and SQL queries generation.
-
-* Data-aware controls.
-
-* Open framework. You can use any Javascript/Python libraries.
-
-* Rich, informative reports. Band-oriented report generation based on
-  `LibreOffice <https://www.libreoffice.org/>`_ templates.
-
-* Charts. You can use free `jsCharts <http://www.jscharts.com/>`_ library
-  or any javascript charting library to create charts to represent and analyze your application data.
-
-* Allows to save audit trail/change history made by users
-
-* Predefined css themes.
-
-* Develop and test locally update remotely. Jam.py has Export and Import
-  utilities that allow developer to store all metadata (database structures,
-  project parameters and code) in a file that can be loaded by another
-  application to apply all the changes.
-
-Documentation
-=============
-
-All documentation is in the "docs" directory and online at
-http://jam-py.com/docs/.
-
-Please visit http://jam-py.com/docs/intro/install.html for Python and
-framework installation or http://jam-py.com/docs/intro/new_project.html how to create a
-new project.
-
-For general discussion, ideas or similar, please visit mailgroup https://groups.google.com/g/jam-py or
-FB page https://www.facebook.com/groups/jam.py/
-
-Demo application: http://demo.jam-py.com/
-
-
-
-License
-=======
-
-Jam.py is licensed under the BSD License.
-
-Author
-======
-
-Andrew Yushev
-
-See also the list of `contributors <http://jam-py.com/contributors.html>`_
-who participated in this project.
-
-
-
```

### Comparing `jam_py_v5-5.4.136/README.rst` & `jam.py-v5-5.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/builder/admin.sqlite` & `jam.py-v5-5.5.1/builder/admin.sqlite`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/builder/builder.sqlite` & `jam.py-v5-5.5.1/builder/builder.sqlite`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/builder/css/project.css` & `jam.py-v5-5.5.1/builder/css/project.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/builder/demo.sqlite` & `jam.py-v5-5.5.1/builder/demo.sqlite`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/builder/index.html` & `jam.py-v5-5.5.1/builder/index.html`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/builder/js/app_builder.js` & `jam.py-v5-5.5.1/builder/js/app_builder.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/builder/read.me` & `jam.py-v5-5.5.1/builder/read.me`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/admin.sqlite` & `jam.py-v5-5.5.1/demo/admin.sqlite`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/demo.sqlite` & `jam.py-v5-5.5.1/demo/demo.sqlite`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/index.html` & `jam.py-v5-5.5.1/demo/index.html`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/js/demo.js` & `jam.py-v5-5.5.1/demo/js/demo.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/reports/customers.ods` & `jam.py-v5-5.5.1/demo/reports/customers.ods`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/reports/invoice.ods` & `jam.py-v5-5.5.1/demo/reports/invoice.ods`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/reports/purchases.ods` & `jam.py-v5-5.5.1/demo/reports/purchases.ods`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/files/SampleAudio_0.4mb2018-09-20_173200.101229.mp3` & `jam.py-v5-5.5.1/demo/static/files/SampleAudio_0.4mb2018-09-20_173200.101229.mp3`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/files/adult-18792_6402018-09-20_172710.277885.jpg` & `jam.py-v5-5.5.1/demo/static/files/adult-18792_6402018-09-20_172710.277885.jpg`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/files/fashion-2082066_6402018-09-20_172551.982164.jpg` & `jam.py-v5-5.5.1/demo/static/files/fashion-2082066_6402018-09-20_172551.982164.jpg`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/files/girl-919048_6402018-09-20_172740.031997.jpg` & `jam.py-v5-5.5.1/demo/static/files/girl-919048_6402018-09-20_172740.031997.jpg`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/files/man-3122063_6402018-09-20_172535.467176.jpg` & `jam.py-v5-5.5.1/demo/static/files/man-3122063_6402018-09-20_172535.467176.jpg`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/files/model-2911330_6402018-09-20_172523.737081.jpg` & `jam.py-v5-5.5.1/demo/static/files/model-2911330_6402018-09-20_172523.737081.jpg`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/files/model-334739_6402018-10-03_102403.928076.jpg` & `jam.py-v5-5.5.1/demo/static/files/model-334739_6402018-10-03_102403.928076.jpg`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/files/model-429733_6402018-09-20_175440.291794.jpg` & `jam.py-v5-5.5.1/demo/static/files/model-429733_6402018-09-20_175440.291794.jpg`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/files/model-429733_6402019-04-25_101749.737955.jpg` & `jam.py-v5-5.5.1/demo/static/files/model-429733_6402019-04-25_101749.737955.jpg`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/files/patient-841165_6402018-09-20_172615.389149.jpg` & `jam.py-v5-5.5.1/demo/static/files/patient-841165_6402018-09-20_172615.389149.jpg`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/files/smile-1885144_6402018-11-10_102150.945190.jpg` & `jam.py-v5-5.5.1/demo/static/files/smile-1885144_6402018-11-10_102150.945190.jpg`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/files/stockvault-businessman-1282942018-09-20_172731.439691.jpg` & `jam.py-v5-5.5.1/demo/static/files/stockvault-businessman-1282942018-09-20_172731.439691.jpg`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/files/stockvault-businessman1196482018-09-20_172602.032986.jpg` & `jam.py-v5-5.5.1/demo/static/files/stockvault-businessman1196482018-09-20_172602.032986.jpg`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/files/sun-3588618_6402018-09-20_175413.562097.jpg` & `jam.py-v5-5.5.1/demo/static/files/sun-3588618_6402018-09-20_175413.562097.jpg`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/demo/static/js/Chart.min.js` & `jam.py-v5-5.5.1/demo/static/js/Chart.min.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/admin/admin.py` & `jam.py-v5-5.5.1/jam/admin/admin.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/admin/builder.py` & `jam.py-v5-5.5.1/jam/admin/builder.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/admin/builder_structure.info` & `jam.py-v5-5.5.1/jam/admin/builder_structure.info`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/admin/export_metadata.py` & `jam.py-v5-5.5.1/jam/admin/export_metadata.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/admin/import_metadata.py` & `jam.py-v5-5.5.1/jam/admin/import_metadata.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/admin/task.py` & `jam.py-v5-5.5.1/jam/admin/task.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/bin/jam-project.py` & `jam.py-v5-5.5.1/jam/bin/jam-project.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/builder.html` & `jam.py-v5-5.5.1/jam/builder.html`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/common.py` & `jam.py-v5-5.5.1/jam/common.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/admin.css` & `jam.py-v5-5.5.1/jam/css/admin.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/admin.min.css` & `jam.py-v5-5.5.1/jam/css/admin.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-amelia.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-amelia.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-amelia.min.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-amelia.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-cerulean.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-cerulean.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-cerulean.min.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-cerulean.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-cosmo.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-cosmo.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-cosmo.min.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-cosmo.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-flatly.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-flatly.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-flatly.min.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-flatly.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-journal.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-journal.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-journal.min.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-journal.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-modal.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-modal.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-modal.min.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-modal.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-readable.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-readable.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-readable.min.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-readable.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-responsive.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-responsive.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-responsive.min.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-responsive.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-slate.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-slate.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-slate.min.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-slate.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-spacelab.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-spacelab.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-spacelab.min.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-spacelab.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-united.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-united.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap-united.min.css` & `jam.py-v5-5.5.1/jam/css/bootstrap-united.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap.css` & `jam.py-v5-5.5.1/jam/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/bootstrap.min.css` & `jam.py-v5-5.5.1/jam/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/datepicker.css` & `jam.py-v5-5.5.1/jam/css/datepicker.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/datepicker.min.css` & `jam.py-v5-5.5.1/jam/css/datepicker.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/jam.css` & `jam.py-v5-5.5.1/jam/css/jam.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/jam.min.css` & `jam.py-v5-5.5.1/jam/css/jam.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/jam12.css` & `jam.py-v5-5.5.1/jam/css/jam12.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/css/jam12.min.css` & `jam.py-v5-5.5.1/jam/css/jam12.min.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/dataset.py` & `jam.py-v5-5.5.1/jam/dataset.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/db/db_modules.py` & `jam.py-v5-5.5.1/jam/db/db_modules.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/db/firebird.py` & `jam.py-v5-5.5.1/jam/db/firebird.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/db/mssql.py` & `jam.py-v5-5.5.1/jam/db/mssql.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/db/mysql.py` & `jam.py-v5-5.5.1/jam/db/mysql.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/db/oracle.py` & `jam.py-v5-5.5.1/jam/db/oracle.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/db/postgres.py` & `jam.py-v5-5.5.1/jam/db/postgres.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/db/sqlite.py` & `jam.py-v5-5.5.1/jam/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/events.py` & `jam.py-v5-5.5.1/jam/events.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/execute.py` & `jam.py-v5-5.5.1/jam/execute.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/img/glyphicons-halflings-white.png` & `jam.py-v5-5.5.1/jam/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/img/glyphicons-halflings.png` & `jam.py-v5-5.5.1/jam/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/img/j.ico` & `jam.py-v5-5.5.1/jam/img/j.ico`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/img/placeholder.png` & `jam.py-v5-5.5.1/jam/img/placeholder.png`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/items.py` & `jam.py-v5-5.5.1/jam/items.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/ace/ace.js` & `jam.py-v5-5.5.1/jam/js/ace/ace.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/ace/ext-searchbox.js` & `jam.py-v5-5.5.1/jam/js/ace/ext-searchbox.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/ace/mode-css.js` & `jam.py-v5-5.5.1/jam/js/ace/mode-css.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/ace/mode-html.js` & `jam.py-v5-5.5.1/jam/js/ace/mode-html.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/ace/mode-javascript.js` & `jam.py-v5-5.5.1/jam/js/ace/mode-javascript.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/ace/mode-python.js` & `jam.py-v5-5.5.1/jam/js/ace/mode-python.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/ace/mode-rst.js` & `jam.py-v5-5.5.1/jam/js/ace/mode-rst.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/ace/worker-css.js` & `jam.py-v5-5.5.1/jam/js/ace/worker-css.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/ace/worker-html.js` & `jam.py-v5-5.5.1/jam/js/ace/worker-html.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/ace/worker-javascript.js` & `jam.py-v5-5.5.1/jam/js/ace/worker-javascript.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/admin.js` & `jam.py-v5-5.5.1/jam/js/admin.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/admin.min.js` & `jam.py-v5-5.5.1/jam/js/admin.min.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/bootstrap-datepicker.js` & `jam.py-v5-5.5.1/jam/js/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/bootstrap-datepicker.min.js` & `jam.py-v5-5.5.1/jam/js/bootstrap-datepicker.min.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/bootstrap-modal.js` & `jam.py-v5-5.5.1/jam/js/bootstrap-modal.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/bootstrap-modal.min.js` & `jam.py-v5-5.5.1/jam/js/bootstrap-modal.min.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/bootstrap-modalmanager.js` & `jam.py-v5-5.5.1/jam/js/bootstrap-modalmanager.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/bootstrap-modalmanager.min.js` & `jam.py-v5-5.5.1/jam/js/bootstrap-modalmanager.min.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/bootstrap.js` & `jam.py-v5-5.5.1/jam/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/bootstrap.min.js` & `jam.py-v5-5.5.1/jam/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/jam.js` & `jam.py-v5-5.5.1/jam/js/jam.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/jam.min.js` & `jam.py-v5-5.5.1/jam/js/jam.min.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/jquery.js` & `jam.py-v5-5.5.1/jam/js/jquery.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/jquery.maskedinput.js` & `jam.py-v5-5.5.1/jam/js/jquery.maskedinput.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/jquery.maskedinput.min.js` & `jam.py-v5-5.5.1/jam/js/jquery.maskedinput.min.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/jquery.min.js` & `jam.py-v5-5.5.1/jam/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/md5.js` & `jam.py-v5-5.5.1/jam/js/md5.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/js/md5.min.js` & `jam.py-v5-5.5.1/jam/js/md5.min.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/langs.py` & `jam.py-v5-5.5.1/jam/langs.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/langs.sqlite` & `jam.py-v5-5.5.1/jam/langs.sqlite`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/project/admin.sqlite` & `jam.py-v5-5.5.1/jam/project/admin.sqlite`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/project/index.html` & `jam.py-v5-5.5.1/jam/project/index.html`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/server_classes.py` & `jam.py-v5-5.5.1/jam/server_classes.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/sql.py` & `jam.py-v5-5.5.1/jam/sql.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/__init__.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/__init__.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/__main__.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/__main__.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/character.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/character.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/comment_handler.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/comment_handler.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/compat.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/compat.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/error_handler.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/error_handler.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/esprima.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/esprima.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/jsx_nodes.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/jsx_nodes.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/jsx_parser.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/jsx_parser.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/jsx_syntax.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/jsx_syntax.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/messages.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/messages.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/nodes.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/nodes.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/objects.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/objects.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/parser.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/parser.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/scanner.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/scanner.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/syntax.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/syntax.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/token.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/token.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/tokenizer.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/tokenizer.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/utils.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/utils.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/visitor.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/visitor.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/esprima/xhtml_entities.py` & `jam.py-v5-5.5.1/jam/third_party/esprima/xhtml_entities.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/filelock.py` & `jam.py-v5-5.5.1/jam/third_party/filelock.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/jsmin/__init__.py` & `jam.py-v5-5.5.1/jam/third_party/jsmin/__init__.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/jsmin/__main__.py` & `jam.py-v5-5.5.1/jam/third_party/jsmin/__main__.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/jsmin/test.py` & `jam.py-v5-5.5.1/jam/third_party/jsmin/test.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/six.py` & `jam.py-v5-5.5.1/jam/third_party/six.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/__init__.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/dialects/__init__.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/__init__.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/base.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/base.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/create.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/create.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/default.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/default.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/events.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/events.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/interfaces.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/interfaces.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/mock.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/mock.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/reflection.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/reflection.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/result.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/result.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/row.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/row.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/threadlocal.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/threadlocal.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/url.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/url.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/engine/util.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/engine/util.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/event/__init__.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/event/__init__.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/event/api.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/event/api.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/event/attr.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/event/attr.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/event/base.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/event/base.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/event/legacy.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/event/legacy.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/event/registry.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/event/registry.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/exc.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/exc.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/future/result.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/future/result.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/inspection.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/inspection.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/interfaces.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/interfaces.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/log.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/log.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/pool/__init__.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/pool/base.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/pool/base.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/pool/dbapi_proxy.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/pool/dbapi_proxy.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/pool/events.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/pool/events.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/pool/impl.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/pool/impl.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/processors.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/processors.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/schema.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/schema.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/__init__.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/annotation.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/annotation.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/base.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/base.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/coercions.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/coercions.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/compiler.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/compiler.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/crud.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/crud.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/ddl.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/ddl.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/default_comparator.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/default_comparator.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/dml.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/dml.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/elements.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/elements.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/events.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/events.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/expression.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/expression.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/functions.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/functions.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/naming.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/naming.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/operators.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/operators.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/roles.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/roles.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/schema.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/schema.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/selectable.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/sqltypes.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/sqltypes.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/traversals.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/traversals.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/type_api.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/type_api.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/util.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/util.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/sql/visitors.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/sql/visitors.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/types.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/__init__.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/_collections.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/_collections.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/compat.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/compat.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/deprecations.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/deprecations.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/langhelpers.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/langhelpers.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/queue.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/queue.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/sqlalchemy/util/topological.py` & `jam.py-v5-5.5.1/jam/third_party/sqlalchemy/util/topological.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/_compat.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/_compat.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/_internal.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/_internal.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/_reloader.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/_reloader.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/datastructures.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/datastructures.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/__init__.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/console.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/console.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/repr.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/repr.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/shared/debugger.js` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/shared/debugger.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/shared/jquery.js` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/shared/jquery.js`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/shared/source.png` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/shared/source.png`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/shared/style.css` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/shared/style.css`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/shared/ubuntu.ttf` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/shared/ubuntu.ttf`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/debug/tbtools.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/debug/tbtools.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/exceptions.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/exceptions.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/filesystem.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/filesystem.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/formparser.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/formparser.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/http.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/http.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/local.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/local.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/__init__.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/dispatcher.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/http_proxy.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/http_proxy.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/lint.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/lint.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/profiler.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/profiler.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/proxy_fix.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/proxy_fix.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/middleware/shared_data.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/middleware/shared_data.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/posixemulation.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/posixemulation.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/routing.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/routing.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/secure_cookie/securecookie.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/secure_cookie/securecookie.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/secure_cookie/sessions.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/secure_cookie/sessions.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/security.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/security.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/serving.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/serving.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/test.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/test.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/testapp.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/testapp.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/urls.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/urls.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/useragents.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/useragents.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/utils.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/utils.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/websocket.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/websocket.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/__init__.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/accept.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/accept.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/auth.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/auth.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/base_request.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/base_request.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/base_response.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/base_response.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/common_descriptors.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/common_descriptors.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/cors.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/cors.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/etag.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/etag.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/json.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/json.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/request.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/request.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers/response.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers/response.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/wrappers.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/wrappers.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/third_party/werkzeug/wsgi.py` & `jam.py-v5-5.5.1/jam/third_party/werkzeug/wsgi.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam/wsgi.py` & `jam.py-v5-5.5.1/jam/wsgi.py`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/jam.py_v5.egg-info/PKG-INFO` & `jam.py-v5-5.5.1/jam.py_v5.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,163 @@
 Metadata-Version: 2.1
 Name: jam.py-v5
-Version: 5.4.136
+Version: 5.5.1
 Summary: Jam.py Application Builder is an event-driven framework for the development of web database applications.
 Home-page: http://jam-py.com/
 Author: Andrew Yushev
 Author-email: andrew@jam-py.com
 License: BSD
+Description: 
+        .. image:: https://img.shields.io/pypi/v/jam.py.svg
+           :target: https://pypi.org/project/jam.py/
+           :alt: Package on PyPI
+        
+        .. image:: https://img.shields.io/pypi/pyversions/jam.py.svg
+           :target: https://pypi.python.org/pypi/jam.py
+           :alt: Supported Python Versions
+        
+        .. image:: https://readthedocs.org/projects/jam-py/badge/?version=stable
+           :target: http://jam-py.com/docs/
+           :alt: Documentation Status
+        
+        .. image:: https://api.travis-ci.org/platipusica/jam-py.png?branch=master
+           :target: http://travis-ci.org/platipusica/jam-py
+           :alt: Build Status (Travis CI)
+        
+        
+        
+        ================
+        Jam.py Application Builder (web framework)
+        ================
+        
+        
+        From an idea of a web database application to a live website in no time, for free
+        =================================================================================
+        
+        Click on the image to see the online demo
+        
+        .. figure:: demo/static/img/JAMPY_Readme.gif
+            :width: 100%
+            :align: center
+            :alt: Online demo
+            :target: https://demo.jam-py.com/
+        
+        
+        If you are not a professional programmer or an expert in databases, you can use
+        Jam.py to store, share and analyze your data.
+            
+        Please watch these videos to see how easy it is to create and setup Jam.py
+        applications.
+        
+        * `Creating CRM web database applications from start to finish in 7 minutes with Jam.py framework <https://youtu.be/vY6FTdpABa4>`_
+        * `Setting up interface of Jam.py application using Forms Dialogs <https://youtu.be/hvNZ0-a_HHw>`_
+        
+        If you are a professional, you can use Jam.py to create various tools, dashboards,
+        as well as large-scale business applications with complex internal logic.
+        Please watch the
+        `Jam.py framework applications <https://youtu.be/qkJvGlgoabU>`_  video
+        to see some applications written in Jam.py.
+        
+        More demos on PythonAnywhere:
+        
+        * `SAP Theme Demo <https://jampyapp.pythonanywhere.com/>`_
+        * `Personal Account Ledger from MS Access template <https://msaccess.pythonanywhere.com/>`_
+        * `NorthWind Traders from MS Access template (wip) <https://northwind.pythonanywhere.com/>`_
+        * `The ERP POC Demo with Italian and English translations <https://sem.pythonanywhere.com/>`_
+        * `Assets/Parts Application (wip, currently Jam V7 Demo) <https://jampy.pythonanywhere.com>`_
+        * `Machine Learning (wip) <https://mlearning.pythonanywhere.com>`_
+        * `Auto Parts Sales for Brazilian Market (Portuguese) <https://carparts.pythonanywhere.com>`_
+        * `Resourcing and Billing Application from MS Access DB (wip) <https://resourcingandbilling.pythonanywhere.com>`_
+        * `Job Positions tracking App from MS Access DB (wip) <https://positionstracking.pythonanywhere.com>`_
+        * `Kanban/Tasks Application <https://kanban.pythonanywhere.com>`_
+        * `Assets Inventory Application (wip) <https://assetinventory.pythonanywhere.com>`_
+        
+        
+        Jam.py alternative site:
+        
+        * `https://jampyapplicationbuilder.com/`
+        
+        
+        Main features
+        =============
+        
+        Jam.py is an object oriented, event driven framework with hierarchical structure, modular design
+        and very tight DB/GUI coupling. The server side of Jam.py is written in `Python <https://www.python.org">`_,
+        the client utilizes `JavaScript <https://developer.mozilla.org/en/docs/Web/JavaScript">`_,
+        `jQuery <https://jquery.com">`_ and `Bootstrap <http://getbootstrap.com/2.3.2">`_.
+        
+        * Simple, clear and efficient IDE. The development takes place in the
+          Application builder, an application written completely in Jam.py.
+        
+        * “All in the browser” framework. With Jam.py, all you need are two pages
+          in the browser, one for the project, the other for the Application builder.
+          Make changes in the Application builder, go to the project, refresh the page,
+          and see the results.
+        
+        * Supports SQLite, PostgreSQL, MySQL, Firebird, MSSQL and
+          Oracle databases. The concept of the framework allows you to migrate from
+          one database to another without changing the project.
+        
+        * Authentication, authorization, session management, roles and permissions.
+        
+        * Automatic creation and modification of database tables and SQL queries generation.
+        
+        * Data-aware controls.
+        
+        * Open framework. You can use any Javascript/Python libraries.
+        
+        * Rich, informative reports. Band-oriented report generation based on
+          `LibreOffice <https://www.libreoffice.org/>`_ templates.
+        
+        * Charts. You can use free `jsCharts <http://www.jscharts.com/>`_ library
+          or any javascript charting library to create charts to represent and analyze your application data.
+        
+        * Allows to save audit trail/change history made by users
+        
+        * Predefined css themes.
+        
+        * Develop and test locally update remotely. Jam.py has Export and Import
+          utilities that allow developer to store all metadata (database structures,
+          project parameters and code) in a file that can be loaded by another
+          application to apply all the changes.
+        
+        Documentation
+        =============
+        
+        All documentation is in the "docs" directory and online at
+        http://jam-py.com/docs/.
+        
+        Please visit http://jam-py.com/docs/intro/install.html for Python and
+        framework installation or http://jam-py.com/docs/intro/new_project.html how to create a
+        new project.
+        
+        For general discussion, ideas or similar, please visit mailgroup https://groups.google.com/g/jam-py or
+        FB page https://www.facebook.com/groups/jam.py/
+        
+        Demo application: http://demo.jam-py.com/
+        
+        
+        
+        License
+        =======
+        
+        Jam.py is licensed under the BSD License.
+        
+        Author
+        ======
+        
+        Andrew Yushev
+        
+        See also the list of `contributors <http://jam-py.com/contributors.html>`_
+        who participated in this project.
+        
+        
+        
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -22,156 +170,7 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-
-
-.. image:: https://img.shields.io/pypi/v/jam.py.svg
-   :target: https://pypi.org/project/jam.py/
-   :alt: Package on PyPI
-
-.. image:: https://img.shields.io/pypi/pyversions/jam.py.svg
-   :target: https://pypi.python.org/pypi/jam.py
-   :alt: Supported Python Versions
-
-.. image:: https://readthedocs.org/projects/jam-py/badge/?version=stable
-   :target: http://jam-py.com/docs/
-   :alt: Documentation Status
-
-.. image:: https://api.travis-ci.org/platipusica/jam-py.png?branch=master
-   :target: http://travis-ci.org/platipusica/jam-py
-   :alt: Build Status (Travis CI)
-
-
-
-================
-Jam.py Application Builder (web framework)
-================
-
-
-From an idea of a web database application to a live website in no time, for free
-=================================================================================
-
-Click on the image to see the online demo
-
-.. figure:: demo/static/img/JAMPY_Readme.gif
-    :width: 100%
-    :align: center
-    :alt: Online demo
-    :target: https://demo.jam-py.com/
-
-
-If you are not a professional programmer or an expert in databases, you can use
-Jam.py to store, share and analyze your data.
-    
-Please watch these videos to see how easy it is to create and setup Jam.py
-applications.
-
-* `Creating CRM web database applications from start to finish in 7 minutes with Jam.py framework <https://youtu.be/vY6FTdpABa4>`_
-* `Setting up interface of Jam.py application using Forms Dialogs <https://youtu.be/hvNZ0-a_HHw>`_
-
-If you are a professional, you can use Jam.py to create various tools, dashboards,
-as well as large-scale business applications with complex internal logic.
-Please watch the
-`Jam.py framework applications <https://youtu.be/qkJvGlgoabU>`_  video
-to see some applications written in Jam.py.
-
-More demos on PythonAnywhere:
-
-* `SAP Theme Demo <https://jampyapp.pythonanywhere.com/>`_
-* `Personal Account Ledger from MS Access template <https://msaccess.pythonanywhere.com/>`_
-* `NorthWind Traders from MS Access template (wip) <https://northwind.pythonanywhere.com/>`_
-* `The ERP POC Demo with Italian and English translations <https://sem.pythonanywhere.com/>`_
-* `Assets/Parts Application (wip, currently Jam V7 Demo) <https://jampy.pythonanywhere.com>`_
-* `Machine Learning (wip) <https://mlearning.pythonanywhere.com>`_
-* `Auto Parts Sales for Brazilian Market (Portuguese) <https://carparts.pythonanywhere.com>`_
-* `Resourcing and Billing Application from MS Access DB (wip) <https://resourcingandbilling.pythonanywhere.com>`_
-* `Job Positions tracking App from MS Access DB (wip) <https://positionstracking.pythonanywhere.com>`_
-* `Kanban/Tasks Application <https://kanban.pythonanywhere.com>`_
-* `Assets Inventory Application (wip) <https://assetinventory.pythonanywhere.com>`_
-
-
-Jam.py alternative site:
-
-* `https://jampyapplicationbuilder.com/`
-
-
-Main features
-=============
-
-Jam.py is an object oriented, event driven framework with hierarchical structure, modular design
-and very tight DB/GUI coupling. The server side of Jam.py is written in `Python <https://www.python.org">`_,
-the client utilizes `JavaScript <https://developer.mozilla.org/en/docs/Web/JavaScript">`_,
-`jQuery <https://jquery.com">`_ and `Bootstrap <http://getbootstrap.com/2.3.2">`_.
-
-* Simple, clear and efficient IDE. The development takes place in the
-  Application builder, an application written completely in Jam.py.
-
-* “All in the browser” framework. With Jam.py, all you need are two pages
-  in the browser, one for the project, the other for the Application builder.
-  Make changes in the Application builder, go to the project, refresh the page,
-  and see the results.
-
-* Supports SQLite, PostgreSQL, MySQL, Firebird, MSSQL and
-  Oracle databases. The concept of the framework allows you to migrate from
-  one database to another without changing the project.
-
-* Authentication, authorization, session management, roles and permissions.
-
-* Automatic creation and modification of database tables and SQL queries generation.
-
-* Data-aware controls.
-
-* Open framework. You can use any Javascript/Python libraries.
-
-* Rich, informative reports. Band-oriented report generation based on
-  `LibreOffice <https://www.libreoffice.org/>`_ templates.
-
-* Charts. You can use free `jsCharts <http://www.jscharts.com/>`_ library
-  or any javascript charting library to create charts to represent and analyze your application data.
-
-* Allows to save audit trail/change history made by users
-
-* Predefined css themes.
-
-* Develop and test locally update remotely. Jam.py has Export and Import
-  utilities that allow developer to store all metadata (database structures,
-  project parameters and code) in a file that can be loaded by another
-  application to apply all the changes.
-
-Documentation
-=============
-
-All documentation is in the "docs" directory and online at
-http://jam-py.com/docs/.
-
-Please visit http://jam-py.com/docs/intro/install.html for Python and
-framework installation or http://jam-py.com/docs/intro/new_project.html how to create a
-new project.
-
-For general discussion, ideas or similar, please visit mailgroup https://groups.google.com/g/jam-py or
-FB page https://www.facebook.com/groups/jam.py/
-
-Demo application: http://demo.jam-py.com/
-
-
-
-License
-=======
-
-Jam.py is licensed under the BSD License.
-
-Author
-======
-
-Andrew Yushev
-
-See also the list of `contributors <http://jam-py.com/contributors.html>`_
-who participated in this project.
-
-
-
```

### Comparing `jam_py_v5-5.4.136/jam.py_v5.egg-info/SOURCES.txt` & `jam.py-v5-5.5.1/jam.py_v5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jam_py_v5-5.4.136/setup.py` & `jam.py-v5-5.5.1/setup.py`

 * *Files identical despite different names*

