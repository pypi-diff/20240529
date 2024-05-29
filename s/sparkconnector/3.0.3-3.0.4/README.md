# Comparing `tmp/sparkconnector-3.0.3.tar.gz` & `tmp/sparkconnector-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkconnector-3.0.3.tar", last modified: Wed May 22 15:06:18 2024, max compression
+gzip compressed data, was "sparkconnector-3.0.4.tar", last modified: Wed May 29 09:37:37 2024, max compression
```

## Comparing `sparkconnector-3.0.3.tar` & `sparkconnector-3.0.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:06:18.819009 sparkconnector-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-22 15:06:18.815009 sparkconnector-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:06:18.803009 sparkconnector-3.0.3/nbextension/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/nbextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:06:18.803009 sparkconnector-3.0.3/nbextension/src/
--rw-r--r--   0 runner    (1001) docker     (127)    36016 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/nbextension/src/extension.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:06:18.807009 sparkconnector-3.0.3/nbextension/src/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/nbextension/src/templates/configuring.html
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/nbextension/src/templates/connected.html
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/nbextension/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)   117229 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/nbextension/yarn.lock
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:06:18.819009 sparkconnector-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:06:18.807009 sparkconnector-3.0.3/sparkconnector/
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/sparkconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/sparkconnector/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    18054 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/sparkconnector/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/sparkconnector/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:06:18.807009 sparkconnector-3.0.3/sparkconnector/labextension/
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:06:18.811009 sparkconnector-3.0.3/sparkconnector/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/130.010d2bedc1a53ac02235.js
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/211.c41c5accd09bf179f43f.js
--rw-r--r--   0 runner    (1001) docker     (127)   190151 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/241.a7438870d8deeeebe7f0.js
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/241.a7438870d8deeeebe7f0.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   164203 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/622.93e439ac1a06053d0c2f.js
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/622.93e439ac1a06053d0c2f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11130 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/64.4bd03483bc7614f79e3a.js
--rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/747.a7fb8f39c5a4c9909e80.js
--rw-r--r--   0 runner    (1001) docker     (127)    58206 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/949.deaacecb74692372447f.js
--rw-r--r--   0 runner    (1001) docker     (127)    29924 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/98.f7f63ca7daba20996bf7.js
--rw-r--r--   0 runner    (1001) docker     (127)    19463 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/c7afd77757c0cf13826d.png
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/remoteEntry.ed5300dc3711aef48e50.js
--rw-r--r--   0 runner    (1001) docker     (127)    11726 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/sparkconnectorui.d70d9d3d69e9a6d6b156.js
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-22 15:06:07.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (127)    34135 2024-05-22 15:06:13.000000 sparkconnector-3.0.3/sparkconnector/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/sparkconnector/log4j_conf
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/sparkconnector/logreader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:06:18.811009 sparkconnector-3.0.3/sparkconnector/nbextension/
--rw-r--r--   0 runner    (1001) docker     (127)   105725 2024-05-22 15:06:18.000000 sparkconnector-3.0.3/sparkconnector/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-22 15:06:18.000000 sparkconnector-3.0.3/sparkconnector/nbextension/extension.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:06:18.815009 sparkconnector-3.0.3/sparkconnector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-22 15:06:18.000000 sparkconnector-3.0.3/sparkconnector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-22 15:06:18.000000 sparkconnector-3.0.3/sparkconnector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:06:18.000000 sparkconnector-3.0.3/sparkconnector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:05:17.000000 sparkconnector-3.0.3/sparkconnector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 15:06:18.000000 sparkconnector-3.0.3/sparkconnector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 15:06:18.000000 sparkconnector-3.0.3/sparkconnector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:06:18.811009 sparkconnector-3.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:06:18.815009 sparkconnector-3.0.3/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/authenticate.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:06:18.815009 sparkconnector-3.0.3/src/components/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/common/layout.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/common/loglist.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/common/spark-version.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:06:18.815009 sparkconnector-3.0.3/src/components/configuring/
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/configuring/choose-bundles.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/configuring/index.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/configuring/input-spark-configuration.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/configuring/selected-configuration.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/connect-failed.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/connected.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/connecting.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/lazy-panel.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/loading.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/not-attached.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/panel.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/components/theme-provider.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/labconnector.ts
--rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/store.ts
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/src/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:06:18.815009 sparkconnector-3.0.3/style/
--rw-r--r--   0 runner    (1001) docker     (127)    19463 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/style/Apache_Spark_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/style/apachespark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/style/base.css
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/style/index.css
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/style/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)   251437 2024-05-22 15:04:45.000000 sparkconnector-3.0.3/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:37:37.381422 sparkconnector-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-29 09:37:37.381422 sparkconnector-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:37:37.369422 sparkconnector-3.0.4/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/nbextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:37:37.369422 sparkconnector-3.0.4/nbextension/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    36016 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/nbextension/src/extension.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:37:37.369422 sparkconnector-3.0.4/nbextension/src/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/nbextension/src/templates/configuring.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/nbextension/src/templates/connected.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/nbextension/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)   117229 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/nbextension/yarn.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:37:37.381422 sparkconnector-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:37:37.369422 sparkconnector-3.0.4/sparkconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/sparkconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/sparkconnector/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18187 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/sparkconnector/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/sparkconnector/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:37:37.369422 sparkconnector-3.0.4/sparkconnector/labextension/
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:37:37.373422 sparkconnector-3.0.4/sparkconnector/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/130.010d2bedc1a53ac02235.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/211.c41c5accd09bf179f43f.js
+-rw-r--r--   0 runner    (1001) docker     (127)   190151 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/241.a7438870d8deeeebe7f0.js
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/241.a7438870d8deeeebe7f0.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   164203 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/622.93e439ac1a06053d0c2f.js
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/622.93e439ac1a06053d0c2f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11130 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/64.4f6ab3482ae0f30af9e9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/747.a7fb8f39c5a4c9909e80.js
+-rw-r--r--   0 runner    (1001) docker     (127)    58206 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/949.deaacecb74692372447f.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29924 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/98.f7f63ca7daba20996bf7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19463 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/c7afd77757c0cf13826d.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/remoteEntry.a7e18787315bb69da3fc.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11726 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/sparkconnectorui.d70d9d3d69e9a6d6b156.js
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-29 09:37:26.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34135 2024-05-29 09:37:31.000000 sparkconnector-3.0.4/sparkconnector/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/sparkconnector/log4j_conf
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/sparkconnector/logreader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:37:37.373422 sparkconnector-3.0.4/sparkconnector/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (127)   105725 2024-05-29 09:37:37.000000 sparkconnector-3.0.4/sparkconnector/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-29 09:37:37.000000 sparkconnector-3.0.4/sparkconnector/nbextension/extension.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:37:37.381422 sparkconnector-3.0.4/sparkconnector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-29 09:37:37.000000 sparkconnector-3.0.4/sparkconnector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-29 09:37:37.000000 sparkconnector-3.0.4/sparkconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:37:37.000000 sparkconnector-3.0.4/sparkconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:36:37.000000 sparkconnector-3.0.4/sparkconnector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 09:37:37.000000 sparkconnector-3.0.4/sparkconnector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 09:37:37.000000 sparkconnector-3.0.4/sparkconnector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:37:37.377422 sparkconnector-3.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:37:37.377422 sparkconnector-3.0.4/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/authenticate.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:37:37.377422 sparkconnector-3.0.4/src/components/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/common/layout.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/common/loglist.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/common/spark-version.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:37:37.377422 sparkconnector-3.0.4/src/components/configuring/
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/configuring/choose-bundles.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/configuring/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/configuring/input-spark-configuration.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/configuring/selected-configuration.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/connect-failed.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/connected.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/connecting.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/lazy-panel.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/loading.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/not-attached.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/panel.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/components/theme-provider.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/labconnector.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/store.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/src/types.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:37:37.381422 sparkconnector-3.0.4/style/
+-rw-r--r--   0 runner    (1001) docker     (127)    19463 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/style/Apache_Spark_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/style/apachespark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)   251437 2024-05-29 09:36:15.000000 sparkconnector-3.0.4/yarn.lock
```

### Comparing `sparkconnector-3.0.3/MANIFEST.in` & `sparkconnector-3.0.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/PKG-INFO` & `sparkconnector-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkconnector
-Version: 3.0.3
+Version: 3.0.4
 Summary: Helper to connect to CERN's Spark Clusters
 Home-page: https://github.com/swan-cern/jupyter-extensions
 Author: SWAN Admins
 License: AGPL-3.0
 Keywords: Jupyter,JupyterLab,SWAN,CERN
 Platform: Linux
 Classifier: Framework :: Jupyter
```

### Comparing `sparkconnector-3.0.3/README.md` & `sparkconnector-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/nbextension/package.json` & `sparkconnector-3.0.4/nbextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'3.0.4'"}*

```diff
@@ -24,9 +24,9 @@
     "name": "sparkconnector-nbextension",
     "scripts": {
         "build": "yarn webpack",
         "clean": "rimraf ../sparkconnector/nbextension",
         "dev": "webpack --watch --mode development --config webpack.config.js",
         "webpack": "webpack --config webpack.config.js"
     },
-    "version": "3.0.3"
+    "version": "3.0.4"
 }
```

### Comparing `sparkconnector-3.0.3/nbextension/src/extension.js` & `sparkconnector-3.0.4/nbextension/src/extension.js`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/nbextension/src/templates/configuring.html` & `sparkconnector-3.0.4/nbextension/src/templates/configuring.html`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/nbextension/src/templates/connected.html` & `sparkconnector-3.0.4/nbextension/src/templates/connected.html`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/nbextension/webpack.config.js` & `sparkconnector-3.0.4/nbextension/webpack.config.js`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/nbextension/yarn.lock` & `sparkconnector-3.0.4/nbextension/yarn.lock`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/package.json` & `sparkconnector-3.0.4/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'version'": "'3.0.4'"}*

```diff
@@ -203,9 +203,9 @@
             "csstree/validator": true,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.3"
+    "version": "3.0.4"
 }
```

### Comparing `sparkconnector-3.0.3/setup.py` & `sparkconnector-3.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/__init__.py` & `sparkconnector-3.0.4/sparkconnector/__init__.py`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/configuration.py` & `sparkconnector-3.0.4/sparkconnector/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,15 @@
     def configure(self, opts, ports):
         """ Initialize K8s configuration for Spark """
 
         conf = super(self.__class__, self).configure(opts, ports)
 
         # Set K8s configuration
         conf.set('spark.kubernetes.namespace', os.environ.get('SPARK_USER'))
+        conf.set('spark.kubernetes.container.image', 'gitlab-registry.cern.ch/db/spark-service/docker-registry/swan:alma9-20240123')
         conf.set('spark.master', self._retrieve_k8s_master(os.environ.get('KUBECONFIG')))
 
         # Configure shuffle if running on K8s with Spark 3.x.x
         if self.get_spark_version().split('.')[0]=='3':
             conf.set('spark.shuffle.service.enabled', 'false')
             conf.set('spark.dynamicAllocation.shuffleTracking.enabled', 'true')
```

### Comparing `sparkconnector-3.0.3/sparkconnector/connector.py` & `sparkconnector-3.0.4/sparkconnector/connector.py`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/labextension/package.json` & `sparkconnector-3.0.4/sparkconnector/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9778079710144927%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.a7e18787315bb69da3fc.js'}}",*

 * * "'version'": "'3.0.4'"}*

```diff
@@ -110,15 +110,15 @@
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/swan-cern/jupyter-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ed5300dc3711aef48e50.js",
+            "load": "static/remoteEntry.a7e18787315bb69da3fc.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "sparkconnector"
                 },
@@ -208,9 +208,9 @@
             "csstree/validator": true,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.3"
+    "version": "3.0.4"
 }
```

### Comparing `sparkconnector-3.0.3/sparkconnector/labextension/static/130.010d2bedc1a53ac02235.js` & `sparkconnector-3.0.4/sparkconnector/labextension/static/130.010d2bedc1a53ac02235.js`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/labextension/static/211.c41c5accd09bf179f43f.js` & `sparkconnector-3.0.4/sparkconnector/labextension/static/211.c41c5accd09bf179f43f.js`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/labextension/static/241.a7438870d8deeeebe7f0.js` & `sparkconnector-3.0.4/sparkconnector/labextension/static/241.a7438870d8deeeebe7f0.js`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/labextension/static/622.93e439ac1a06053d0c2f.js` & `sparkconnector-3.0.4/sparkconnector/labextension/static/622.93e439ac1a06053d0c2f.js`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/labextension/static/64.4bd03483bc7614f79e3a.js` & `sparkconnector-3.0.4/sparkconnector/labextension/static/64.4f6ab3482ae0f30af9e9.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,27 +1,27 @@
 "use strict";
 (self.webpackChunk_swan_cern_sparkconnector = self.webpackChunk_swan_cern_sparkconnector || []).push([
     [64], {
         2064: (e, o, t) => {
             t.r(o), t.d(o, {
                 default: () => b
             });
-            var n = t(6898),
-                s = t(6793),
-                a = t(3712),
-                r = t(2944),
+            var n = t(3039),
+                s = t(9282),
+                a = t(8690),
+                r = t(3764),
                 i = t(6029),
                 c = t.n(i),
                 l = t(2914);
             const d = c().lazy((() => Promise.all([t.e(241), t.e(98), t.e(704), t.e(262)]).then(t.bind(t, 132)))),
                 h = () => c().createElement(i.Suspense, {
                     fallback: c().createElement("div", null, "loading")
                 }, c().createElement(d, null));
             var k = t(6414),
-                u = t(7098);
+                u = t(4481);
             class p {
                 constructor(e, o) {
                     this.labApp = e, this.notebookTracker = o, this.comms = new Map, this.initConfigurationFromServer(), this.initStateHandling()
                 }
                 async initConfigurationFromServer() {
                     const e = await u.ConfigSection.create({
                             name: "sparkconnector_spark_options"
```

### Comparing `sparkconnector-3.0.3/sparkconnector/labextension/static/747.a7fb8f39c5a4c9909e80.js` & `sparkconnector-3.0.4/sparkconnector/labextension/static/747.a7fb8f39c5a4c9909e80.js`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/labextension/static/949.deaacecb74692372447f.js` & `sparkconnector-3.0.4/sparkconnector/labextension/static/949.deaacecb74692372447f.js`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/labextension/static/98.f7f63ca7daba20996bf7.js` & `sparkconnector-3.0.4/sparkconnector/labextension/static/98.f7f63ca7daba20996bf7.js`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/labextension/static/c7afd77757c0cf13826d.png` & `sparkconnector-3.0.4/sparkconnector/labextension/static/c7afd77757c0cf13826d.png`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/labextension/static/remoteEntry.ed5300dc3711aef48e50.js` & `sparkconnector-3.0.4/sparkconnector/labextension/static/remoteEntry.a7e18787315bb69da3fc.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, l, u, f, c, s, d, p, b, h, v, m, g, y = {
+    var e, r, t, a, n, o, i, l, u, c, f, d, s, p, b, h, v, m, g, y = {
             6641: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(29), t.e(64)]).then((() => () => t(2064))),
                         "./extension": () => Promise.all([t.e(29), t.e(64)]).then((() => () => t(2064))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -44,28 +44,28 @@
     }, k.d = (e, r) => {
         for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => (262 === e ? "sparkconnectorui" : e) + "." + {
         29: "eea1f800ab5b711e3856",
-        64: "4bd03483bc7614f79e3a",
+        64: "4f6ab3482ae0f30af9e9",
         98: "f7f63ca7daba20996bf7",
         130: "010d2bedc1a53ac02235",
         211: "c41c5accd09bf179f43f",
         241: "a7438870d8deeeebe7f0",
         262: "d70d9d3d69e9a6d6b156",
         544: "1c16f02b6c548b8dbdc2",
         622: "93e439ac1a06053d0c2f",
         704: "b3a8bf8e352720b20a42",
         747: "a7fb8f39c5a4c9909e80",
         949: "deaacecb74692372447f"
     } [e] + ".js?v=" + {
         29: "eea1f800ab5b711e3856",
-        64: "4bd03483bc7614f79e3a",
+        64: "4f6ab3482ae0f30af9e9",
         98: "f7f63ca7daba20996bf7",
         130: "010d2bedc1a53ac02235",
         211: "c41c5accd09bf179f43f",
         241: "a7438870d8deeeebe7f0",
         262: "d70d9d3d69e9a6d6b156",
         544: "1c16f02b6c548b8dbdc2",
         622: "93e439ac1a06053d0c2f",
@@ -80,32 +80,32 @@
             if ("object" == typeof window) return window
         }
     }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@swan-cern/sparkconnector:", k.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var i, l;
             if (void 0 !== n)
-                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var c = u[f];
-                    if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + n) {
-                        i = c;
+                for (var u = document.getElementsByTagName("script"), c = 0; c < u.length; c++) {
+                    var f = u[c];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
+                        i = f;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, k.nc && i.setAttribute("nonce", k.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
-            var s = (r, a) => {
-                    i.onerror = i.onload = null, clearTimeout(d);
+            var d = (r, a) => {
+                    i.onerror = i.onload = null, clearTimeout(s);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                d = setTimeout(s.bind(null, void 0, {
+                s = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, k.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -127,15 +127,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@material-ui/core", "4.12.4", (() => Promise.all([k.e(241), k.e(622), k.e(29), k.e(704)]).then((() => () => k(6622))))), l("@swan-cern/sparkconnector", "3.0.3", (() => Promise.all([k.e(29), k.e(64)]).then((() => () => k(2064))))), l("mobx-react-lite", "3.4.3", (() => Promise.all([k.e(29), k.e(704), k.e(544), k.e(130)]).then((() => () => k(8130))))), l("mobx", "6.10.2", (() => k.e(949).then((() => () => k(8949)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@material-ui/core", "4.12.4", (() => Promise.all([k.e(241), k.e(622), k.e(29), k.e(704)]).then((() => () => k(6622))))), l("@swan-cern/sparkconnector", "3.0.4", (() => Promise.all([k.e(29), k.e(64)]).then((() => () => k(2064))))), l("mobx-react-lite", "3.4.3", (() => Promise.all([k.e(29), k.e(704), k.e(544), k.e(130)]).then((() => () => k(8130))))), l("mobx", "6.10.2", (() => k.e(949).then((() => () => k(8949)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -185,79 +185,79 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, c, s = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (c = (typeof(f = r[i]))[0])) return !u || ("u" == s ? l > a && !n : "" == s != n);
-                if ("u" == c) {
-                    if (!u || "u" != s) return !1
+                var c, f, d = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(c = r[i]))[0])) return !u || ("u" == d ? l > a && !n : "" == d != n);
+                if ("u" == f) {
+                    if (!u || "u" != d) return !1
                 } else if (u)
-                    if (s == c)
+                    if (d == f)
                         if (l <= a) {
-                            if (f != e[l]) return !1
+                            if (c != e[l]) return !1
                         } else {
-                            if (n ? f > e[l] : f < e[l]) return !1;
-                            f != e[l] && (u = !1)
+                            if (n ? c > e[l] : c < e[l]) return !1;
+                            c != e[l] && (u = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != d && "n" != d) {
                     if (n || l <= a) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= a || c < s != n) return !1;
+                    if (l <= a || f < d != n) return !1;
                     u = !1
-                } else "s" != s && "n" != s && (u = !1, l--)
+                } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
-        var d = [],
-            p = d.pop.bind(d);
+        var s = [],
+            p = s.pop.bind(s);
         for (i = 1; i < e.length; i++) {
             var b = e[i];
-            d.push(1 == b ? p() | p() : 2 == b ? p() & p() : b ? o(b, r) : !p())
+            s.push(1 == b ? p() | p() : 2 == b ? p() & p() : b ? o(b, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
         var t = k.S[e];
         if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
+    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", c = (e, r, t, a) => {
         var n = l(e, t);
-        return o(a, n) || s(u(e, t, n, a)), d(e[t][n])
-    }, c = (e, r, t) => {
+        return o(a, n) || d(u(e, t, n, a)), s(e[t][n])
+    }, f = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
-    }, s = e => {
+    }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, d = e => (e.loaded = 1, e.get()), b = (p = e => function(r, t, a, n) {
+    }, s = e => (e.loaded = 1, e.get()), b = (p = e => function(r, t, a, n) {
         var o = k.I(r);
         return o && o.then ? o.then(e.bind(e, r, k.S[r], t, a, n)) : e(r, k.S[r], t, a, n)
-    })(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), h = p(((e, r, t, a, n) => {
-        var o = r && k.o(r, t) && c(r, t, a);
-        return o ? d(o) : n()
+    })(((e, r, t, a) => (i(e, t), c(r, 0, t, a)))), h = p(((e, r, t, a, n) => {
+        var o = r && k.o(r, t) && f(r, t, a);
+        return o ? s(o) : n()
     })), v = {}, m = {
         6029: () => b("default", "react", [1, 18, 2, 0]),
-        2944: () => b("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
-        3712: () => b("default", "@jupyterlab/apputils", [1, 4, 3, 0]),
+        3039: () => b("default", "@jupyterlab/application", [1, 4, 2, 1]),
+        3764: () => b("default", "@jupyterlab/ui-components", [1, 4, 2, 1]),
+        4481: () => b("default", "@jupyterlab/services", [1, 7, 2, 1]),
         6414: () => h("default", "mobx", [1, 6, 3, 2], (() => k.e(949).then((() => () => k(8949))))),
-        6793: () => b("default", "@jupyterlab/notebook", [1, 4, 2, 0]),
-        6898: () => b("default", "@jupyterlab/application", [1, 4, 2, 0]),
-        7098: () => b("default", "@jupyterlab/services", [1, 7, 2, 0]),
+        8690: () => b("default", "@jupyterlab/apputils", [1, 4, 3, 1]),
+        9282: () => b("default", "@jupyterlab/notebook", [1, 4, 2, 1]),
         7704: () => b("default", "react-dom", [1, 18, 2, 0]),
         5544: () => h("default", "mobx", [1, 6, 1, 0], (() => k.e(949).then((() => () => k(8949))))),
         8273: () => h("default", "mobx-react-lite", [1, 3, 2, 0], (() => Promise.all([k.e(544), k.e(211)]).then((() => () => k(8130))))),
         5659: () => h("default", "@material-ui/core", [1, 4, 12, 1], (() => k.e(622).then((() => () => k(6622))))),
         8057: () => h("default", "@material-ui/core", [1, 4, 11, 4], (() => k.e(622).then((() => () => k(6622)))))
     }, g = {
         29: [6029],
-        64: [2944, 3712, 6414, 6793, 6898, 7098],
+        64: [3039, 3764, 4481, 6414, 8690, 9282],
         262: [8273, 5659, 8057],
         544: [5544],
         704: [7704]
     }, k.f.consumes = (e, r) => {
         k.o(g, e) && g[e].forEach((e => {
             if (k.o(v, e)) return r.push(v[e]);
             var t = r => {
```

### Comparing `sparkconnector-3.0.3/sparkconnector/labextension/static/sparkconnectorui.d70d9d3d69e9a6d6b156.js` & `sparkconnector-3.0.4/sparkconnector/labextension/static/sparkconnectorui.d70d9d3d69e9a6d6b156.js`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/labextension/static/third-party-licenses.json` & `sparkconnector-3.0.4/sparkconnector/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/log4j_conf` & `sparkconnector-3.0.4/sparkconnector/log4j_conf`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/logreader.py` & `sparkconnector-3.0.4/sparkconnector/logreader.py`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector/nbextension/extension.js` & `sparkconnector-3.0.4/sparkconnector/nbextension/extension.js`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/sparkconnector.egg-info/PKG-INFO` & `sparkconnector-3.0.4/sparkconnector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkconnector
-Version: 3.0.3
+Version: 3.0.4
 Summary: Helper to connect to CERN's Spark Clusters
 Home-page: https://github.com/swan-cern/jupyter-extensions
 Author: SWAN Admins
 License: AGPL-3.0
 Keywords: Jupyter,JupyterLab,SWAN,CERN
 Platform: Linux
 Classifier: Framework :: Jupyter
```

### Comparing `sparkconnector-3.0.3/sparkconnector.egg-info/SOURCES.txt` & `sparkconnector-3.0.4/sparkconnector.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 sparkconnector/labextension/package.json
 sparkconnector/labextension/static/130.010d2bedc1a53ac02235.js
 sparkconnector/labextension/static/211.c41c5accd09bf179f43f.js
 sparkconnector/labextension/static/241.a7438870d8deeeebe7f0.js
 sparkconnector/labextension/static/241.a7438870d8deeeebe7f0.js.LICENSE.txt
 sparkconnector/labextension/static/622.93e439ac1a06053d0c2f.js
 sparkconnector/labextension/static/622.93e439ac1a06053d0c2f.js.LICENSE.txt
-sparkconnector/labextension/static/64.4bd03483bc7614f79e3a.js
+sparkconnector/labextension/static/64.4f6ab3482ae0f30af9e9.js
 sparkconnector/labextension/static/747.a7fb8f39c5a4c9909e80.js
 sparkconnector/labextension/static/949.deaacecb74692372447f.js
 sparkconnector/labextension/static/98.f7f63ca7daba20996bf7.js
 sparkconnector/labextension/static/c7afd77757c0cf13826d.png
-sparkconnector/labextension/static/remoteEntry.ed5300dc3711aef48e50.js
+sparkconnector/labextension/static/remoteEntry.a7e18787315bb69da3fc.js
 sparkconnector/labextension/static/sparkconnectorui.d70d9d3d69e9a6d6b156.js
 sparkconnector/labextension/static/style.js
 sparkconnector/labextension/static/third-party-licenses.json
 sparkconnector/nbextension/extension.js
 sparkconnector/nbextension/extension.js.LICENSE.txt
 src/index.ts
 src/labconnector.ts
```

### Comparing `sparkconnector-3.0.3/src/components/authenticate.tsx` & `sparkconnector-3.0.4/src/components/authenticate.tsx`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/components/common/layout.tsx` & `sparkconnector-3.0.4/src/components/common/layout.tsx`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/components/common/loglist.tsx` & `sparkconnector-3.0.4/src/components/common/loglist.tsx`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/components/common/spark-version.tsx` & `sparkconnector-3.0.4/src/components/common/spark-version.tsx`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/components/configuring/choose-bundles.tsx` & `sparkconnector-3.0.4/src/components/configuring/choose-bundles.tsx`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/components/configuring/index.tsx` & `sparkconnector-3.0.4/src/components/configuring/index.tsx`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/components/configuring/input-spark-configuration.tsx` & `sparkconnector-3.0.4/src/components/configuring/input-spark-configuration.tsx`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/components/configuring/selected-configuration.tsx` & `sparkconnector-3.0.4/src/components/configuring/selected-configuration.tsx`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/components/connect-failed.tsx` & `sparkconnector-3.0.4/src/components/connect-failed.tsx`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/components/connected.tsx` & `sparkconnector-3.0.4/src/components/connected.tsx`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/components/connecting.tsx` & `sparkconnector-3.0.4/src/components/connecting.tsx`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/components/panel.tsx` & `sparkconnector-3.0.4/src/components/panel.tsx`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/components/theme-provider.tsx` & `sparkconnector-3.0.4/src/components/theme-provider.tsx`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/index.ts` & `sparkconnector-3.0.4/src/index.ts`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/labconnector.ts` & `sparkconnector-3.0.4/src/labconnector.ts`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/src/store.ts` & `sparkconnector-3.0.4/src/store.ts`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/style/Apache_Spark_logo.png` & `sparkconnector-3.0.4/style/Apache_Spark_logo.png`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/style/apachespark.svg` & `sparkconnector-3.0.4/style/apachespark.svg`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/style/base.css` & `sparkconnector-3.0.4/style/base.css`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/tsconfig.json` & `sparkconnector-3.0.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `sparkconnector-3.0.3/yarn.lock` & `sparkconnector-3.0.4/yarn.lock`

 * *Files identical despite different names*

