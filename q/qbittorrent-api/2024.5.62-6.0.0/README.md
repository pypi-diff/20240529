# Comparing `tmp/qbittorrent_api-2024.5.62.tar.gz` & `tmp/qbittorrent-api-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbittorrent_api-2024.5.62.tar", last modified: Wed May 29 16:59:16 2024, max compression
+gzip compressed data, was "dist/qbittorrent-api-6.0.0.tar", last modified: Thu Apr 23 04:02:29 2020, max compression
```

## Comparing `qbittorrent_api-2024.5.62.tar` & `qbittorrent-api-6.0.0.tar`

### file list

```diff
@@ -1,104 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:59:16.404876 qbittorrent_api-2024.5.62/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:59:16.388876 qbittorrent_api-2024.5.62/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:59:16.388876 qbittorrent_api-2024.5.62/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:59:16.388876 qbittorrent_api-2024.5.62/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/.github/workflows/pre-commit-update.yml
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13051 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19629 2024-05-29 16:59:16.404876 qbittorrent_api-2024.5.62/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:59:16.388876 qbittorrent_api-2024.5.62/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:59:16.388876 qbittorrent_api-2024.5.62/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:59:16.392876 qbittorrent_api-2024.5.62/docs/source/apidoc/
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/apidoc/app.rst
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/apidoc/attrdict.rst
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/apidoc/auth.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/apidoc/client.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/apidoc/definitions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/apidoc/log.rst
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/apidoc/request.rst
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/apidoc/rss.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/apidoc/search.rst
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/apidoc/sync.rst
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/apidoc/torrentcreator.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/apidoc/torrents.rst
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/apidoc/transfer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/apidoc/version.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/behavior&configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/performance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/docs/source/spelling_wordlist
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 16:59:16.404876 qbittorrent_api-2024.5.62/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:59:16.384876 qbittorrent_api-2024.5.62/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:59:16.400876 qbittorrent_api-2024.5.62/src/qbittorrent_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19629 2024-05-29 16:59:16.000000 qbittorrent_api-2024.5.62/src/qbittorrent_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-29 16:59:16.000000 qbittorrent_api-2024.5.62/src/qbittorrent_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:59:16.000000 qbittorrent_api-2024.5.62/src/qbittorrent_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-29 16:59:16.000000 qbittorrent_api-2024.5.62/src/qbittorrent_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 16:59:16.000000 qbittorrent_api-2024.5.62/src/qbittorrent_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:59:16.396876 qbittorrent_api-2024.5.62/src/qbittorrentapi/
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/_attrdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/_version_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/log.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    43186 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14273 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/rss.py
--rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/torrentcreator.py
--rw-r--r--   0 runner    (1001) docker     (127)   107307 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/torrents.py
--rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/src/qbittorrentapi/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:59:16.400876 qbittorrent_api-2024.5.62/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:59:16.400876 qbittorrent_api-2024.5.62/tests/_resources/
--rw-r--r--   0 runner    (1001) docker     (127)   324876 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/_resources/kubuntu-22.04.3-desktop-amd64.iso.torrent
--rw-r--r--   0 runner    (1001) docker     (127)   343556 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/_resources/kubuntu-22.04.4-desktop-amd64.iso.torrent
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/_resources/root_folder.torrent
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/_resources/server.crt
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/_resources/server.key
--rw-r--r--   0 runner    (1001) docker     (127)   292338 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/_resources/ubuntu-22.04.1-desktop-amd64.iso.torrent
--rw-r--r--   0 runner    (1001) docker     (127)   244236 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/_resources/xubuntu-22.04.4-desktop-amd64.iso.torrent
--rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    25725 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/test_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/test_rss.py
--rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    19744 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/test_torrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/test_torrentcreator.py
--rw-r--r--   0 runner    (1001) docker     (127)    53064 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/test_torrents.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/test_zzz_last_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-29 16:59:08.000000 qbittorrent_api-2024.5.62/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (116)     2016 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    35149 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      145 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    23199 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    17763 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    23199 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      696 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       49 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       15 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/qbittorrentapi/
+-rw-r--r--   0 runner    (1001) docker     (116)       81 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3655 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2408 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10851 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7416 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2930 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1786 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26761 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1771 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/log.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11711 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13759 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/responses.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5813 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/rss.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6711 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/search.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1801 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/sync.py
+-rw-r--r--   0 runner    (1001) docker     (116)    30791 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/torrents.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4224 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1525 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/setup.py
```

### Comparing `qbittorrent_api-2024.5.62/src/qbittorrentapi/exceptions.py` & `qbittorrent-api-6.0.0/qbittorrentapi/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,140 +1,156 @@
-from __future__ import annotations
-
-from requests.exceptions import HTTPError as RequestsHTTPError
 from requests.exceptions import RequestException
 
 
 class APIError(Exception):
-    """Base error for all exceptions from this Client."""
-
-
-class UnsupportedQbittorrentVersion(APIError):
-    """Connected qBittorrent is not fully supported by this Client."""
+    """
+    Base error for all exceptions from this Client.
+    """
+    pass
 
 
 class FileError(IOError, APIError):
-    """Base class for all exceptions for file handling."""
+    """
+    Base class for all exceptions for file handling.
+    """
+    pass
 
 
 class TorrentFileError(FileError):
-    """Base class for all exceptions for torrent files."""
+    """
+    Base class for all exceptions for torrent files.
+    """
+    pass
 
 
 class TorrentFileNotFoundError(TorrentFileError):
-    """Specified torrent file does not appear to exist."""
+    """
+    Specified torrent file does not appear to exist.
+    """
+    pass
 
 
 class TorrentFilePermissionError(TorrentFileError):
-    """Permission was denied to read the specified torrent file."""
+    """
+    Permission was denied to read the specified torrent file.
+    """
+    pass
 
 
 class APIConnectionError(RequestException, APIError):
-    """Base class for all communications errors including HTTP errors."""
+    """
+    Base class for all communications errors including HTTP errors.
+    """
+    pass
 
 
 class LoginFailed(APIConnectionError):
-    """This can technically be raised with any request since log in may be attempted for
-    any request and could fail."""
+    """
+    This can technically be raised with any request since log in may be attempted for any request and could fail.
+    """
+    pass
 
 
-class HTTPError(RequestsHTTPError, APIConnectionError):
+class HTTPError(APIConnectionError):
     """
-    Base error for all HTTP errors.
-
-    All errors following a successful connection to qBittorrent are returned as HTTP
-    statuses.
+    Base error for all HTTP errors. All errors following a successful connection to qBittorrent are returned as HTTP statuses.
     """
-
-    http_status_code: int
+    pass
 
 
 class HTTP4XXError(HTTPError):
-    """Base error for all HTTP 4XX statuses."""
+    """
+    Base error for all HTTP 4XX statuses.
+    """
+    pass
 
 
 class HTTP5XXError(HTTPError):
-    """Base error for all HTTP 5XX statuses."""
+    """
+    Base error for all HTTP 5XX statuses.
+    """
+    pass
 
 
 class HTTP400Error(HTTP4XXError):
-    """HTTP 400 Status."""
-
-    http_status_code: int = 400
+    pass
 
 
 class HTTP401Error(HTTP4XXError):
-    """HTTP 401 Status."""
-
-    http_status_code: int = 401
+    pass
 
 
 class HTTP403Error(HTTP4XXError):
-    """HTTP 403 Status."""
-
-    http_status_code: int = 403
+    pass
 
 
 class HTTP404Error(HTTP4XXError):
-    """HTTP 404 Status."""
-
-    http_status_code: int = 404
-
-
-class HTTP405Error(HTTP4XXError):
-    """HTTP 405 Status."""
-
-    http_status_code: int = 405
+    pass
 
 
 class HTTP409Error(HTTP4XXError):
-    """HTTP 409 Status."""
-
-    http_status_code: int = 409
+    pass
 
 
 class HTTP415Error(HTTP4XXError):
-    """HTTP 415 Status."""
-
-    http_status_code: int = 415
+    pass
 
 
 class HTTP500Error(HTTP5XXError):
-    """HTTP 500 Status."""
-
-    http_status_code: int = 500
+    pass
 
 
 class MissingRequiredParameters400Error(HTTP400Error):
-    """Endpoint call is missing one or more required parameters."""
+    """
+    Endpoint call is missing one or more required parameters.
+    """
+    pass
 
 
 class InvalidRequest400Error(HTTP400Error):
-    """One or more endpoint arguments are malformed."""
+    """
+    One or more endpoint arguments are malformed.
+    """
+    pass
 
 
 class Unauthorized401Error(HTTP401Error):
-    """Primarily reserved for XSS and host header issues."""
+    """
+    Primarily reserved for XSS and host header issues.
+    """
+    pass
 
 
 class Forbidden403Error(HTTP403Error):
-    """Not logged in, IP has been banned, or calling an API method that isn't public."""
+    """
+    Not logged in, IP has been banned, or calling an API method that isn't public.
+    """
+    pass
 
 
 class NotFound404Error(HTTP404Error):
-    """This should mean qBittorrent couldn't find a torrent for the torrent hash."""
-
-
-class MethodNotAllowed405Error(HTTP405Error):
-    """HTTP method is not supported for the API endpoint."""
+    """
+    This should mean qBittorrent couldn't find a torrent for the torrent hash.
+    It is also possible this means the endpoint doesn't exist in qBittorrent...but that also means this Client has a bug.
+    """
+    pass
 
 
 class Conflict409Error(HTTP409Error):
-    """Returned if arguments don't make sense specific to the endpoint."""
+    """
+    Returned if arguments don't make sense specific to the endpoint.
+    """
+    pass
 
 
 class UnsupportedMediaType415Error(HTTP415Error):
-    """``torrents/add`` endpoint will return this for invalid URL(s) or files."""
+    """
+    torrents/add endpoint will return this for invalid URL(s) or files.
+    """
+    pass
 
 
 class InternalServerError500Error(HTTP500Error):
-    """Returned if qBittorrent errors internally while processing the request."""
+    """
+    Returned if qBittorent craps on itself while processing the request...
+    """
+    pass
```

