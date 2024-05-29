# Comparing `tmp/pyjabber-0.1.0.tar.gz` & `tmp/pyjabber-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjabber-0.1.0.tar", last modified: Wed May 29 10:09:40 2024, max compression
+gzip compressed data, was "pyjabber-0.1.1.tar", last modified: Wed May 29 10:42:16 2024, max compression
```

## Comparing `pyjabber-0.1.0.tar` & `pyjabber-0.1.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.697217 pyjabber-0.1.0/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      104 2024-05-14 08:24:48.000000 pyjabber-0.1.0/AUTHORS.rst
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     3757 2024-04-18 10:44:35.000000 pyjabber-0.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       89 2024-04-18 10:44:35.000000 pyjabber-0.1.0/HISTORY.rst
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1070 2024-04-18 10:44:35.000000 pyjabber-0.1.0/LICENSE
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      423 2024-05-23 10:28:52.000000 pyjabber-0.1.0/MANIFEST.in
--rw-r--r--   0 aaron     (1000) aaron     (1000)     3230 2024-05-29 10:09:40.697217 pyjabber-0.1.0/PKG-INFO
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     2690 2024-05-23 10:32:45.000000 pyjabber-0.1.0/README.rst
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.689216 pyjabber-0.1.0/docs/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      610 2024-05-14 08:24:48.000000 pyjabber-0.1.0/docs/Makefile
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.685217 pyjabber-0.1.0/docs/_build/
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.685217 pyjabber-0.1.0/docs/_build/html/
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.689216 pyjabber-0.1.0/docs/_build/html/_images/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)    34337 2024-05-23 07:56:59.000000 pyjabber-0.1.0/docs/_build/html/_images/arch.png
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.689216 pyjabber-0.1.0/docs/_build/html/_static/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      286 2024-05-03 06:47:04.000000 pyjabber-0.1.0/docs/_build/html/_static/file.png
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.689216 pyjabber-0.1.0/docs/_build/html/_static/img/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)   141141 2024-05-03 06:45:25.000000 pyjabber-0.1.0/docs/_build/html/_static/img/screenshot.png
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       90 2024-05-03 06:47:04.000000 pyjabber-0.1.0/docs/_build/html/_static/minus.png
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       90 2024-05-03 06:47:04.000000 pyjabber-0.1.0/docs/_build/html/_static/plus.png
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.689216 pyjabber-0.1.0/docs/_build/html/res/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)    74669 2024-05-03 10:24:23.000000 pyjabber-0.1.0/docs/_build/html/res/arch.png
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1319 2024-05-14 08:24:48.000000 pyjabber-0.1.0/docs/architecture.rst
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       28 2024-04-18 10:44:35.000000 pyjabber-0.1.0/docs/authors.rst
--rwxrwxr-x   0 aaron     (1000) aaron     (1000)     4857 2024-05-14 08:24:48.000000 pyjabber-0.1.0/docs/conf.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       33 2024-04-18 10:44:35.000000 pyjabber-0.1.0/docs/contributing.rst
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       28 2024-04-18 10:44:35.000000 pyjabber-0.1.0/docs/history.rst
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      284 2024-05-14 08:24:48.000000 pyjabber-0.1.0/docs/index.rst
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1122 2024-04-18 10:44:35.000000 pyjabber-0.1.0/docs/installation.rst
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      806 2024-04-18 10:44:35.000000 pyjabber-0.1.0/docs/make.bat
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       27 2024-04-18 10:44:35.000000 pyjabber-0.1.0/docs/readme.rst
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.689216 pyjabber-0.1.0/docs/res/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)    34337 2024-05-23 07:56:59.000000 pyjabber-0.1.0/docs/res/arch.png
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.689216 pyjabber-0.1.0/pyjabber/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      434 2024-05-29 07:51:18.000000 pyjabber-0.1.0/pyjabber/__cli__.py
--rwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 07:45:47.000000 pyjabber-0.1.0/pyjabber/__init__.py
--rwxrwxr-x   0 aaron     (1000) aaron     (1000)     1763 2024-05-29 08:48:35.000000 pyjabber-0.1.0/pyjabber/__main__.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.689216 pyjabber-0.1.0/pyjabber/db/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-05-14 08:24:48.000000 pyjabber-0.1.0/pyjabber/db/__init__.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      193 2024-05-23 08:42:46.000000 pyjabber-0.1.0/pyjabber/db/database.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      287 2024-05-21 07:13:05.000000 pyjabber-0.1.0/pyjabber/db/schema.sql
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.689216 pyjabber-0.1.0/pyjabber/features/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      235 2024-05-14 08:24:48.000000 pyjabber-0.1.0/pyjabber/features/FeatureInterface.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      384 2024-05-14 08:24:48.000000 pyjabber-0.1.0/pyjabber/features/InBandRegistration.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)    10721 2024-05-29 10:09:11.000000 pyjabber-0.1.0/pyjabber/features/PresenceFeature.py
--rwxrwxr-x   0 aaron     (1000) aaron     (1000)      254 2024-05-14 08:24:48.000000 pyjabber-0.1.0/pyjabber/features/ResourceBinding.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     3792 2024-05-29 07:24:14.000000 pyjabber-0.1.0/pyjabber/features/SASLFeature.py
--rwxrwxr-x   0 aaron     (1000) aaron     (1000)      921 2024-05-14 08:24:48.000000 pyjabber-0.1.0/pyjabber/features/StartTLSFeature.py
--rwxrwxr-x   0 aaron     (1000) aaron     (1000)     1693 2024-05-14 08:24:48.000000 pyjabber-0.1.0/pyjabber/features/StreamFeature.py
--rwxr-xr-x   0 aaron     (1000) aaron     (1000)        0 2024-04-18 10:45:47.000000 pyjabber-0.1.0/pyjabber/features/__init__.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.689216 pyjabber-0.1.0/pyjabber/network/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1681 2024-05-28 09:44:38.000000 pyjabber-0.1.0/pyjabber/network/ConnectionsManager.py
--rwxrwxr-x   0 aaron     (1000) aaron     (1000)     1217 2024-05-21 07:51:57.000000 pyjabber-0.1.0/pyjabber/network/StreamAlivenessMonitor.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     3673 2024-05-21 07:18:11.000000 pyjabber-0.1.0/pyjabber/network/XMLParser.py
--rwxrwxr-x   0 aaron     (1000) aaron     (1000)     6093 2024-05-29 07:07:17.000000 pyjabber-0.1.0/pyjabber/network/XMLProtocol.py
--rwxrwxr-x   0 aaron     (1000) aaron     (1000)      204 2024-05-14 08:24:48.000000 pyjabber-0.1.0/pyjabber/network/__init__.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.689216 pyjabber-0.1.0/pyjabber/network/certs/
--rw-------   0 aaron     (1000) aaron     (1000)     1704 2024-04-18 10:45:47.000000 pyjabber-0.1.0/pyjabber/network/certs/localhost-key.pem
--rw-r--r--   0 aaron     (1000) aaron     (1000)     1509 2024-04-18 10:45:47.000000 pyjabber-0.1.0/pyjabber/network/certs/localhost.pem
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.689216 pyjabber-0.1.0/pyjabber/plugins/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      210 2024-05-09 07:06:19.000000 pyjabber-0.1.0/pyjabber/plugins/PluginInterface.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1330 2024-05-29 07:14:22.000000 pyjabber-0.1.0/pyjabber/plugins/PluginManager.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-04-18 10:45:47.000000 pyjabber-0.1.0/pyjabber/plugins/__init__.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.689216 pyjabber-0.1.0/pyjabber/plugins/roster/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     4903 2024-05-28 10:32:22.000000 pyjabber-0.1.0/pyjabber/plugins/roster/Roster.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-04-18 10:45:47.000000 pyjabber-0.1.0/pyjabber/plugins/roster/__init__.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.689216 pyjabber-0.1.0/pyjabber/plugins/xep_0199/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-05-23 08:36:39.000000 pyjabber-0.1.0/pyjabber/plugins/xep_0199/__init__.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      838 2024-05-29 07:13:10.000000 pyjabber-0.1.0/pyjabber/plugins/xep_0199/xep_0199.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     4310 2024-05-29 07:54:04.000000 pyjabber-0.1.0/pyjabber/server.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.693217 pyjabber-0.1.0/pyjabber/stanzas/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      695 2024-04-24 10:46:33.000000 pyjabber-0.1.0/pyjabber/stanzas/IQ.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      694 2024-04-24 10:46:33.000000 pyjabber-0.1.0/pyjabber/stanzas/Message.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      261 2024-04-24 10:46:33.000000 pyjabber-0.1.0/pyjabber/stanzas/Presence.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-04-18 10:45:47.000000 pyjabber-0.1.0/pyjabber/stanzas/__init__.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.693217 pyjabber-0.1.0/pyjabber/stanzas/error/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     3427 2024-05-29 07:56:42.000000 pyjabber-0.1.0/pyjabber/stanzas/error/StanzaError.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-05-23 08:32:21.000000 pyjabber-0.1.0/pyjabber/stanzas/error/__init__.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.693217 pyjabber-0.1.0/pyjabber/stream/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     2400 2024-05-29 10:09:11.000000 pyjabber-0.1.0/pyjabber/stream/StanzaHandler.py
--rwxrwxr-x   0 aaron     (1000) aaron     (1000)     1874 2024-05-14 08:24:48.000000 pyjabber-0.1.0/pyjabber/stream/Stream.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     4989 2024-05-21 07:59:16.000000 pyjabber-0.1.0/pyjabber/stream/StreamHandler.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-05-14 08:24:48.000000 pyjabber-0.1.0/pyjabber/stream/__init__.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.693217 pyjabber-0.1.0/pyjabber/stream/schemas/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)   518638 2024-05-14 08:24:48.000000 pyjabber-0.1.0/pyjabber/stream/schemas/schemas.pkl
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.693217 pyjabber-0.1.0/pyjabber/utils/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      436 2024-05-14 08:24:48.000000 pyjabber-0.1.0/pyjabber/utils/ClarkNotation.py
--rwxr-xr-x   0 aaron     (1000) aaron     (1000)     1458 2024-04-18 10:45:47.000000 pyjabber-0.1.0/pyjabber/utils/Singleton.py
--rwxrwxr-x   0 aaron     (1000) aaron     (1000)       79 2024-04-24 10:46:33.000000 pyjabber-0.1.0/pyjabber/utils/__init__.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.693217 pyjabber-0.1.0/pyjabber/webpage/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-05-23 08:37:39.000000 pyjabber-0.1.0/pyjabber/webpage/__init__.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      846 2024-05-23 08:55:50.000000 pyjabber-0.1.0/pyjabber/webpage/adminPage.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.693217 pyjabber-0.1.0/pyjabber/webpage/api/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-05-21 07:13:05.000000 pyjabber-0.1.0/pyjabber/webpage/api/__init__.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     3778 2024-05-29 10:06:49.000000 pyjabber-0.1.0/pyjabber/webpage/api/api.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.693217 pyjabber-0.1.0/pyjabber/webpage/build/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      374 2024-05-29 09:59:12.000000 pyjabber-0.1.0/pyjabber/webpage/build/asset-manifest.json
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     3870 2024-05-29 09:59:05.000000 pyjabber-0.1.0/pyjabber/webpage/build/favicon.ico
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      649 2024-05-29 09:59:12.000000 pyjabber-0.1.0/pyjabber/webpage/build/index.html
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     5347 2024-05-29 09:59:05.000000 pyjabber-0.1.0/pyjabber/webpage/build/logo192.png
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     9664 2024-05-29 09:59:05.000000 pyjabber-0.1.0/pyjabber/webpage/build/logo512.png
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      492 2024-05-29 09:59:05.000000 pyjabber-0.1.0/pyjabber/webpage/build/manifest.json
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       67 2024-05-29 09:59:05.000000 pyjabber-0.1.0/pyjabber/webpage/build/robots.txt
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.685217 pyjabber-0.1.0/pyjabber/webpage/build/static/
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.693217 pyjabber-0.1.0/pyjabber/webpage/build/static/css/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)   415634 2024-05-29 09:59:12.000000 pyjabber-0.1.0/pyjabber/webpage/build/static/css/main.985302ea.css
--rw-rw-r--   0 aaron     (1000) aaron     (1000)   644351 2024-05-29 09:59:12.000000 pyjabber-0.1.0/pyjabber/webpage/build/static/css/main.985302ea.css.map
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.697217 pyjabber-0.1.0/pyjabber/webpage/build/static/js/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)   553134 2024-05-29 09:59:12.000000 pyjabber-0.1.0/pyjabber/webpage/build/static/js/main.4e6d336c.js
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     2020 2024-05-29 09:59:12.000000 pyjabber-0.1.0/pyjabber/webpage/build/static/js/main.4e6d336c.js.LICENSE.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)  2551226 2024-05-29 09:59:12.000000 pyjabber-0.1.0/pyjabber/webpage/build/static/js/main.4e6d336c.js.map
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:09:40.697217 pyjabber-0.1.0/pyjabber.egg-info/
--rw-r--r--   0 aaron     (1000) aaron     (1000)     3230 2024-05-29 10:09:40.000000 pyjabber-0.1.0/pyjabber.egg-info/PKG-INFO
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     2682 2024-05-29 10:09:40.000000 pyjabber-0.1.0/pyjabber.egg-info/SOURCES.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        1 2024-05-29 10:09:40.000000 pyjabber-0.1.0/pyjabber.egg-info/dependency_links.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       43 2024-05-29 10:09:40.000000 pyjabber-0.1.0/pyjabber.egg-info/entry_points.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       46 2024-05-29 10:09:40.000000 pyjabber-0.1.0/pyjabber.egg-info/requires.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        9 2024-05-29 10:09:40.000000 pyjabber-0.1.0/pyjabber.egg-info/top_level.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       38 2024-05-29 10:09:40.697217 pyjabber-0.1.0/setup.cfg
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      825 2024-05-29 10:09:35.000000 pyjabber-0.1.0/setup.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.573678 pyjabber-0.1.1/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      104 2024-05-14 08:24:48.000000 pyjabber-0.1.1/AUTHORS.rst
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     3757 2024-04-18 10:44:35.000000 pyjabber-0.1.1/CONTRIBUTING.rst
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       89 2024-04-18 10:44:35.000000 pyjabber-0.1.1/HISTORY.rst
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1070 2024-04-18 10:44:35.000000 pyjabber-0.1.1/LICENSE
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      423 2024-05-23 10:28:52.000000 pyjabber-0.1.1/MANIFEST.in
+-rw-r--r--   0 aaron     (1000) aaron     (1000)     3753 2024-05-29 10:42:16.573678 pyjabber-0.1.1/PKG-INFO
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     3213 2024-05-29 10:40:24.000000 pyjabber-0.1.1/README.rst
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.565678 pyjabber-0.1.1/docs/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      610 2024-05-14 08:24:48.000000 pyjabber-0.1.1/docs/Makefile
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.565678 pyjabber-0.1.1/docs/_build/
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.565678 pyjabber-0.1.1/docs/_build/html/
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.565678 pyjabber-0.1.1/docs/_build/html/_images/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)    34337 2024-05-23 07:56:59.000000 pyjabber-0.1.1/docs/_build/html/_images/arch.png
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.565678 pyjabber-0.1.1/docs/_build/html/_static/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      286 2024-05-03 06:47:04.000000 pyjabber-0.1.1/docs/_build/html/_static/file.png
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.565678 pyjabber-0.1.1/docs/_build/html/_static/img/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)   141141 2024-05-03 06:45:25.000000 pyjabber-0.1.1/docs/_build/html/_static/img/screenshot.png
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       90 2024-05-03 06:47:04.000000 pyjabber-0.1.1/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       90 2024-05-03 06:47:04.000000 pyjabber-0.1.1/docs/_build/html/_static/plus.png
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.565678 pyjabber-0.1.1/docs/_build/html/res/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)    74669 2024-05-03 10:24:23.000000 pyjabber-0.1.1/docs/_build/html/res/arch.png
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1319 2024-05-14 08:24:48.000000 pyjabber-0.1.1/docs/architecture.rst
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       28 2024-04-18 10:44:35.000000 pyjabber-0.1.1/docs/authors.rst
+-rwxrwxr-x   0 aaron     (1000) aaron     (1000)     4857 2024-05-14 08:24:48.000000 pyjabber-0.1.1/docs/conf.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       33 2024-04-18 10:44:35.000000 pyjabber-0.1.1/docs/contributing.rst
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       28 2024-04-18 10:44:35.000000 pyjabber-0.1.1/docs/history.rst
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      284 2024-05-14 08:24:48.000000 pyjabber-0.1.1/docs/index.rst
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1122 2024-04-18 10:44:35.000000 pyjabber-0.1.1/docs/installation.rst
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      806 2024-04-18 10:44:35.000000 pyjabber-0.1.1/docs/make.bat
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       27 2024-04-18 10:44:35.000000 pyjabber-0.1.1/docs/readme.rst
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.565678 pyjabber-0.1.1/docs/res/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)    34337 2024-05-23 07:56:59.000000 pyjabber-0.1.1/docs/res/arch.png
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.565678 pyjabber-0.1.1/pyjabber/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      434 2024-05-29 07:51:18.000000 pyjabber-0.1.1/pyjabber/__cli__.py
+-rwxrwxr-x   0 aaron     (1000) aaron     (1000)       21 2024-05-29 10:42:05.000000 pyjabber-0.1.1/pyjabber/__init__.py
+-rwxrwxr-x   0 aaron     (1000) aaron     (1000)     1770 2024-05-29 10:37:25.000000 pyjabber-0.1.1/pyjabber/__main__.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.565678 pyjabber-0.1.1/pyjabber/db/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-05-14 08:24:48.000000 pyjabber-0.1.1/pyjabber/db/__init__.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      193 2024-05-23 08:42:46.000000 pyjabber-0.1.1/pyjabber/db/database.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      287 2024-05-21 07:13:05.000000 pyjabber-0.1.1/pyjabber/db/schema.sql
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.565678 pyjabber-0.1.1/pyjabber/features/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      235 2024-05-14 08:24:48.000000 pyjabber-0.1.1/pyjabber/features/FeatureInterface.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      384 2024-05-14 08:24:48.000000 pyjabber-0.1.1/pyjabber/features/InBandRegistration.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)    10721 2024-05-29 10:09:11.000000 pyjabber-0.1.1/pyjabber/features/PresenceFeature.py
+-rwxrwxr-x   0 aaron     (1000) aaron     (1000)      254 2024-05-14 08:24:48.000000 pyjabber-0.1.1/pyjabber/features/ResourceBinding.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     3792 2024-05-29 07:24:14.000000 pyjabber-0.1.1/pyjabber/features/SASLFeature.py
+-rwxrwxr-x   0 aaron     (1000) aaron     (1000)      921 2024-05-14 08:24:48.000000 pyjabber-0.1.1/pyjabber/features/StartTLSFeature.py
+-rwxrwxr-x   0 aaron     (1000) aaron     (1000)     1693 2024-05-14 08:24:48.000000 pyjabber-0.1.1/pyjabber/features/StreamFeature.py
+-rwxr-xr-x   0 aaron     (1000) aaron     (1000)        0 2024-04-18 10:45:47.000000 pyjabber-0.1.1/pyjabber/features/__init__.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/network/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1681 2024-05-28 09:44:38.000000 pyjabber-0.1.1/pyjabber/network/ConnectionsManager.py
+-rwxrwxr-x   0 aaron     (1000) aaron     (1000)     1217 2024-05-21 07:51:57.000000 pyjabber-0.1.1/pyjabber/network/StreamAlivenessMonitor.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     3673 2024-05-21 07:18:11.000000 pyjabber-0.1.1/pyjabber/network/XMLParser.py
+-rwxrwxr-x   0 aaron     (1000) aaron     (1000)     6093 2024-05-29 07:07:17.000000 pyjabber-0.1.1/pyjabber/network/XMLProtocol.py
+-rwxrwxr-x   0 aaron     (1000) aaron     (1000)      204 2024-05-14 08:24:48.000000 pyjabber-0.1.1/pyjabber/network/__init__.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/network/certs/
+-rw-------   0 aaron     (1000) aaron     (1000)     1704 2024-04-18 10:45:47.000000 pyjabber-0.1.1/pyjabber/network/certs/localhost-key.pem
+-rw-r--r--   0 aaron     (1000) aaron     (1000)     1509 2024-04-18 10:45:47.000000 pyjabber-0.1.1/pyjabber/network/certs/localhost.pem
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/plugins/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      210 2024-05-09 07:06:19.000000 pyjabber-0.1.1/pyjabber/plugins/PluginInterface.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1330 2024-05-29 10:40:02.000000 pyjabber-0.1.1/pyjabber/plugins/PluginManager.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-04-18 10:45:47.000000 pyjabber-0.1.1/pyjabber/plugins/__init__.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/plugins/roster/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     4903 2024-05-28 10:32:22.000000 pyjabber-0.1.1/pyjabber/plugins/roster/Roster.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-04-18 10:45:47.000000 pyjabber-0.1.1/pyjabber/plugins/roster/__init__.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/plugins/xep_0199/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-05-23 08:36:39.000000 pyjabber-0.1.1/pyjabber/plugins/xep_0199/__init__.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      838 2024-05-29 07:13:10.000000 pyjabber-0.1.1/pyjabber/plugins/xep_0199/xep_0199.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     4310 2024-05-29 07:54:04.000000 pyjabber-0.1.1/pyjabber/server.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/stanzas/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      695 2024-04-24 10:46:33.000000 pyjabber-0.1.1/pyjabber/stanzas/IQ.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      694 2024-04-24 10:46:33.000000 pyjabber-0.1.1/pyjabber/stanzas/Message.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      261 2024-04-24 10:46:33.000000 pyjabber-0.1.1/pyjabber/stanzas/Presence.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-04-18 10:45:47.000000 pyjabber-0.1.1/pyjabber/stanzas/__init__.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/stanzas/error/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     3427 2024-05-29 07:56:42.000000 pyjabber-0.1.1/pyjabber/stanzas/error/StanzaError.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-05-23 08:32:21.000000 pyjabber-0.1.1/pyjabber/stanzas/error/__init__.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/stream/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     2400 2024-05-29 10:09:11.000000 pyjabber-0.1.1/pyjabber/stream/StanzaHandler.py
+-rwxrwxr-x   0 aaron     (1000) aaron     (1000)     1874 2024-05-14 08:24:48.000000 pyjabber-0.1.1/pyjabber/stream/Stream.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     4989 2024-05-21 07:59:16.000000 pyjabber-0.1.1/pyjabber/stream/StreamHandler.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-05-14 08:24:48.000000 pyjabber-0.1.1/pyjabber/stream/__init__.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/stream/schemas/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)   518638 2024-05-14 08:24:48.000000 pyjabber-0.1.1/pyjabber/stream/schemas/schemas.pkl
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/utils/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      436 2024-05-14 08:24:48.000000 pyjabber-0.1.1/pyjabber/utils/ClarkNotation.py
+-rwxr-xr-x   0 aaron     (1000) aaron     (1000)     1458 2024-04-18 10:45:47.000000 pyjabber-0.1.1/pyjabber/utils/Singleton.py
+-rwxrwxr-x   0 aaron     (1000) aaron     (1000)       79 2024-04-24 10:46:33.000000 pyjabber-0.1.1/pyjabber/utils/__init__.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/webpage/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-05-23 08:37:39.000000 pyjabber-0.1.1/pyjabber/webpage/__init__.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      846 2024-05-23 08:55:50.000000 pyjabber-0.1.1/pyjabber/webpage/adminPage.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/webpage/api/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        0 2024-05-21 07:13:05.000000 pyjabber-0.1.1/pyjabber/webpage/api/__init__.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     3778 2024-05-29 10:06:49.000000 pyjabber-0.1.1/pyjabber/webpage/api/api.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/webpage/build/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      374 2024-05-29 09:59:12.000000 pyjabber-0.1.1/pyjabber/webpage/build/asset-manifest.json
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     3870 2024-05-29 09:59:05.000000 pyjabber-0.1.1/pyjabber/webpage/build/favicon.ico
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      649 2024-05-29 09:59:12.000000 pyjabber-0.1.1/pyjabber/webpage/build/index.html
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     5347 2024-05-29 09:59:05.000000 pyjabber-0.1.1/pyjabber/webpage/build/logo192.png
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     9664 2024-05-29 09:59:05.000000 pyjabber-0.1.1/pyjabber/webpage/build/logo512.png
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      492 2024-05-29 09:59:05.000000 pyjabber-0.1.1/pyjabber/webpage/build/manifest.json
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       67 2024-05-29 09:59:05.000000 pyjabber-0.1.1/pyjabber/webpage/build/robots.txt
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.565678 pyjabber-0.1.1/pyjabber/webpage/build/static/
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/webpage/build/static/css/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)   415634 2024-05-29 09:59:12.000000 pyjabber-0.1.1/pyjabber/webpage/build/static/css/main.985302ea.css
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)   644351 2024-05-29 09:59:12.000000 pyjabber-0.1.1/pyjabber/webpage/build/static/css/main.985302ea.css.map
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.569678 pyjabber-0.1.1/pyjabber/webpage/build/static/js/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)   553134 2024-05-29 09:59:12.000000 pyjabber-0.1.1/pyjabber/webpage/build/static/js/main.4e6d336c.js
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     2020 2024-05-29 09:59:12.000000 pyjabber-0.1.1/pyjabber/webpage/build/static/js/main.4e6d336c.js.LICENSE.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)  2551226 2024-05-29 09:59:12.000000 pyjabber-0.1.1/pyjabber/webpage/build/static/js/main.4e6d336c.js.map
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-29 10:42:16.573678 pyjabber-0.1.1/pyjabber.egg-info/
+-rw-r--r--   0 aaron     (1000) aaron     (1000)     3753 2024-05-29 10:42:16.000000 pyjabber-0.1.1/pyjabber.egg-info/PKG-INFO
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     2682 2024-05-29 10:42:16.000000 pyjabber-0.1.1/pyjabber.egg-info/SOURCES.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        1 2024-05-29 10:42:16.000000 pyjabber-0.1.1/pyjabber.egg-info/dependency_links.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       43 2024-05-29 10:42:16.000000 pyjabber-0.1.1/pyjabber.egg-info/entry_points.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       46 2024-05-29 10:42:16.000000 pyjabber-0.1.1/pyjabber.egg-info/requires.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        9 2024-05-29 10:42:16.000000 pyjabber-0.1.1/pyjabber.egg-info/top_level.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       38 2024-05-29 10:42:16.573678 pyjabber-0.1.1/setup.cfg
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      855 2024-05-29 10:24:39.000000 pyjabber-0.1.1/setup.py
```

### Comparing `pyjabber-0.1.0/CONTRIBUTING.rst` & `pyjabber-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/LICENSE` & `pyjabber-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/PKG-INFO` & `pyjabber-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjabber
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python XMPP server
 Home-page: https://github.com/DinoThor/PyJabber
 Author: Aarón Raya  
 Author-email: aaron.raya.lopez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,18 +18,18 @@
 
 ========
 PyJabber
 ========
 
 
 .. image:: https://img.shields.io/pypi/v/pyjabber.svg
-        :target: https://test.pypi.org/project/pyjabber/
+        :target: https://pypi.org/project/pyjabber/
 
-.. image:: https://img.shields.io/travis/dinothor/pyjabber.svg
-        :target: https://travis-ci.com/dinothor/pyjabber
+.. image:: https://img.shields.io/github/actions/workflow/status/dinothor/pyjabber/python-app.yml
+        :target: https://github.com/DinoThor/PyJabber/actions
 
 .. image:: https://readthedocs.org/projects/pyjabber/badge/?version=latest
         :target: https://pyjabber.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 |         
@@ -42,33 +42,45 @@
 * Free software: MIT license
 * Documentation: https://pyjabber.readthedocs.io.
 
 Installation
 ------------
 .. code-block::
   
-        pip install -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ pyjabber
+        pip install pyjabber
 
 Quick start
 -----------
 .. code-block:: python
         
         from pyjabber import Server
 
         my_server = Server()
         my_server.start()
 
+or
+
 .. code-block:: python
 
-        class Server(
-            host                : str = "localhost",
-            client_port         : int = 5222,
-            server_port         : int = 5223,
-            connection_timeout  : int = 60
-        )
+        python -m pyjabber --help
+
+.. code-block::
+
+        Usage: python -m pyjabber [OPTIONS]
+
+        Options:
+          --host TEXT               Host name  [default: localhost]
+          --client_port INTEGER     Server-to-client port  [default: 5222]
+          --server_port INTEGER     Server-to-server port  [default: 5269]
+          --family [ipv4|ipv6]      (ipv4 / ipv6)  [default: ipv4]
+          --timeout INTEGER         Timeout for connection  [default: 60]
+          --log_level [INFO|DEBUG]  Log level alert  [default: INFO]
+          --log_path TEXT           Path to log dumpfile.
+          -D, --debug               Enables debug mode in Asyncio.
+          --help                    Show this message and exit.
 
 A formated logger can be added, in order to retrive the messages from the INFO, DEBUG and ERROR levels
 
 .. code-block:: python
     
     2024-05-03 11:45:51.229 | INFO     | pyjabber.server:run_server:52 - Starting server...
     2024-05-03 11:45:51.231 | INFO     | pyjabber.server:run_server:73 - Server is listening clients on ('127.0.0.1', 5222)
@@ -93,16 +105,16 @@
    * - SASL
      - Implemented
      - PLAIN
    * - Roster
      - Implemented
      - CRUD avaliable
    * - Presence
-     - Not implemented
-     - Working on it
+     - Partialy implemented
+     - subscribe, unsubscribed, initial presence and unavailable
 
 Plugins
 -------
 .. list-table::
    :widths: 25 25 50
    :header-rows: 1
```

### Comparing `pyjabber-0.1.0/docs/Makefile` & `pyjabber-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/docs/_build/html/_images/arch.png` & `pyjabber-0.1.1/docs/_build/html/_images/arch.png`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/docs/_build/html/_static/img/screenshot.png` & `pyjabber-0.1.1/docs/_build/html/_static/img/screenshot.png`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/docs/_build/html/res/arch.png` & `pyjabber-0.1.1/docs/_build/html/res/arch.png`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/docs/architecture.rst` & `pyjabber-0.1.1/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/docs/conf.py` & `pyjabber-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/docs/installation.rst` & `pyjabber-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/docs/make.bat` & `pyjabber-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/docs/res/arch.png` & `pyjabber-0.1.1/docs/res/arch.png`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/__main__.py` & `pyjabber-0.1.1/pyjabber/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 @click.command
 @click.option('--host', type=str, default='localhost', show_default=True, help='Host name')
 @click.option('--client_port', type=int, default=5222, show_default=True, help='Server-to-client port')
 @click.option('--server_port', type=int, default=5269, show_default=True, help='Server-to-server port')
 @click.option('--family', type=click.Choice(['ipv4', 'ipv6'], case_sensitive=False), default='ipv4', show_default=True, help='(ipv4 / ipv6)')
 @click.option('--timeout', type=int, default=60, show_default=True, help='Timeout for connection')
 @click.option('--log_level', type=click.Choice(['INFO', 'DEBUG'], case_sensitive=False), default='INFO', show_default=True, help='Log level alert')
-@click.option('--log_path', type=str, help='Path to log dumpfile.')
-@click.option('--debug', '-D', is_flag=True, help='Activa el modo debug.')
+@click.option('--log_path', type=str, help='Path to log dumpfile')
+@click.option('--debug', '-D', is_flag=True, help='Enables debug mode in Asyncio')
 def main(host, client_port, server_port, family, timeout, log_level, log_path, debug):
     
     logger.add(
         log_path if log_path else os.devnull,
         enqueue     = True,
         format      = "<green>{time}</green> - <level>{level}: {message}</level>",
         level       = log_level,
```

### Comparing `pyjabber-0.1.0/pyjabber/features/PresenceFeature.py` & `pyjabber-0.1.1/pyjabber/features/PresenceFeature.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/features/SASLFeature.py` & `pyjabber-0.1.1/pyjabber/features/SASLFeature.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/features/StartTLSFeature.py` & `pyjabber-0.1.1/pyjabber/features/StartTLSFeature.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/features/StreamFeature.py` & `pyjabber-0.1.1/pyjabber/features/StreamFeature.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/network/ConnectionsManager.py` & `pyjabber-0.1.1/pyjabber/network/ConnectionsManager.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/network/StreamAlivenessMonitor.py` & `pyjabber-0.1.1/pyjabber/network/StreamAlivenessMonitor.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/network/XMLParser.py` & `pyjabber-0.1.1/pyjabber/network/XMLParser.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/network/XMLProtocol.py` & `pyjabber-0.1.1/pyjabber/network/XMLProtocol.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/network/certs/localhost-key.pem` & `pyjabber-0.1.1/pyjabber/network/certs/localhost-key.pem`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/network/certs/localhost.pem` & `pyjabber-0.1.1/pyjabber/network/certs/localhost.pem`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/plugins/PluginManager.py` & `pyjabber-0.1.1/pyjabber/plugins/PluginManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,8 +33,8 @@
             return plugin.feed(self._jid, element)
         except KeyError:
             try:
                 plugin = self._plugins[tag]         #Retrive plugin from list and instance
                 self._activePlugins[tag] = plugin()
                 return self._activePlugins[tag].feed(self._jid, element)
             except KeyError: 
-                return SE.service_unavaliable()     #Plugin unavaliable
+                return SE.service_unavaliable()     #Plugin unavailable
```

### Comparing `pyjabber-0.1.0/pyjabber/plugins/roster/Roster.py` & `pyjabber-0.1.1/pyjabber/plugins/roster/Roster.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/plugins/xep_0199/xep_0199.py` & `pyjabber-0.1.1/pyjabber/plugins/xep_0199/xep_0199.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/server.py` & `pyjabber-0.1.1/pyjabber/server.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/stanzas/IQ.py` & `pyjabber-0.1.1/pyjabber/stanzas/IQ.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/stanzas/Message.py` & `pyjabber-0.1.1/pyjabber/stanzas/Message.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/stanzas/error/StanzaError.py` & `pyjabber-0.1.1/pyjabber/stanzas/error/StanzaError.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/stream/StanzaHandler.py` & `pyjabber-0.1.1/pyjabber/stream/StanzaHandler.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/stream/Stream.py` & `pyjabber-0.1.1/pyjabber/stream/Stream.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/stream/StreamHandler.py` & `pyjabber-0.1.1/pyjabber/stream/StreamHandler.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/stream/schemas/schemas.pkl` & `pyjabber-0.1.1/pyjabber/stream/schemas/schemas.pkl`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/utils/Singleton.py` & `pyjabber-0.1.1/pyjabber/utils/Singleton.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/webpage/adminPage.py` & `pyjabber-0.1.1/pyjabber/webpage/adminPage.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/webpage/api/api.py` & `pyjabber-0.1.1/pyjabber/webpage/api/api.py`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/webpage/build/favicon.ico` & `pyjabber-0.1.1/pyjabber/webpage/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/webpage/build/index.html` & `pyjabber-0.1.1/pyjabber/webpage/build/index.html`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/webpage/build/logo192.png` & `pyjabber-0.1.1/pyjabber/webpage/build/logo192.png`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/webpage/build/logo512.png` & `pyjabber-0.1.1/pyjabber/webpage/build/logo512.png`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/webpage/build/static/css/main.985302ea.css` & `pyjabber-0.1.1/pyjabber/webpage/build/static/css/main.985302ea.css`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/webpage/build/static/css/main.985302ea.css.map` & `pyjabber-0.1.1/pyjabber/webpage/build/static/css/main.985302ea.css.map`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/webpage/build/static/js/main.4e6d336c.js` & `pyjabber-0.1.1/pyjabber/webpage/build/static/js/main.4e6d336c.js`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/webpage/build/static/js/main.4e6d336c.js.LICENSE.txt` & `pyjabber-0.1.1/pyjabber/webpage/build/static/js/main.4e6d336c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber/webpage/build/static/js/main.4e6d336c.js.map` & `pyjabber-0.1.1/pyjabber/webpage/build/static/js/main.4e6d336c.js.map`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/pyjabber.egg-info/PKG-INFO` & `pyjabber-0.1.1/pyjabber.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjabber
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python XMPP server
 Home-page: https://github.com/DinoThor/PyJabber
 Author: Aarón Raya  
 Author-email: aaron.raya.lopez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,18 +18,18 @@
 
 ========
 PyJabber
 ========
 
 
 .. image:: https://img.shields.io/pypi/v/pyjabber.svg
-        :target: https://test.pypi.org/project/pyjabber/
+        :target: https://pypi.org/project/pyjabber/
 
-.. image:: https://img.shields.io/travis/dinothor/pyjabber.svg
-        :target: https://travis-ci.com/dinothor/pyjabber
+.. image:: https://img.shields.io/github/actions/workflow/status/dinothor/pyjabber/python-app.yml
+        :target: https://github.com/DinoThor/PyJabber/actions
 
 .. image:: https://readthedocs.org/projects/pyjabber/badge/?version=latest
         :target: https://pyjabber.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 |         
@@ -42,33 +42,45 @@
 * Free software: MIT license
 * Documentation: https://pyjabber.readthedocs.io.
 
 Installation
 ------------
 .. code-block::
   
-        pip install -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ pyjabber
+        pip install pyjabber
 
 Quick start
 -----------
 .. code-block:: python
         
         from pyjabber import Server
 
         my_server = Server()
         my_server.start()
 
+or
+
 .. code-block:: python
 
-        class Server(
-            host                : str = "localhost",
-            client_port         : int = 5222,
-            server_port         : int = 5223,
-            connection_timeout  : int = 60
-        )
+        python -m pyjabber --help
+
+.. code-block::
+
+        Usage: python -m pyjabber [OPTIONS]
+
+        Options:
+          --host TEXT               Host name  [default: localhost]
+          --client_port INTEGER     Server-to-client port  [default: 5222]
+          --server_port INTEGER     Server-to-server port  [default: 5269]
+          --family [ipv4|ipv6]      (ipv4 / ipv6)  [default: ipv4]
+          --timeout INTEGER         Timeout for connection  [default: 60]
+          --log_level [INFO|DEBUG]  Log level alert  [default: INFO]
+          --log_path TEXT           Path to log dumpfile.
+          -D, --debug               Enables debug mode in Asyncio.
+          --help                    Show this message and exit.
 
 A formated logger can be added, in order to retrive the messages from the INFO, DEBUG and ERROR levels
 
 .. code-block:: python
     
     2024-05-03 11:45:51.229 | INFO     | pyjabber.server:run_server:52 - Starting server...
     2024-05-03 11:45:51.231 | INFO     | pyjabber.server:run_server:73 - Server is listening clients on ('127.0.0.1', 5222)
@@ -93,16 +105,16 @@
    * - SASL
      - Implemented
      - PLAIN
    * - Roster
      - Implemented
      - CRUD avaliable
    * - Presence
-     - Not implemented
-     - Working on it
+     - Partialy implemented
+     - subscribe, unsubscribed, initial presence and unavailable
 
 Plugins
 -------
 .. list-table::
    :widths: 25 25 50
    :header-rows: 1
```

### Comparing `pyjabber-0.1.0/pyjabber.egg-info/SOURCES.txt` & `pyjabber-0.1.1/pyjabber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjabber-0.1.0/setup.py` & `pyjabber-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from setuptools import setup, find_packages
 
+import pyjabber
+
 setup(
     name='pyjabber',
-    version='0.1.0',
+    version=pyjabber.__version__,
     author='Aarón Raya  ',
     author_email='aaron.raya.lopez@gmail.com',
     description='A Python XMPP server',
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     url='https://github.com/DinoThor/PyJabber',
     packages=find_packages(),
```

