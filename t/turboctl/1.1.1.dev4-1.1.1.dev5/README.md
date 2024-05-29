# Comparing `tmp/turboctl-1.1.1.dev4.tar.gz` & `tmp/turboctl-1.1.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turboctl-1.1.1.dev4.tar", last modified: Thu May 23 12:55:08 2024, max compression
+gzip compressed data, was "turboctl-1.1.1.dev5.tar", last modified: Wed May 29 10:58:37 2024, max compression
```

## Comparing `turboctl-1.1.1.dev4.tar` & `turboctl-1.1.1.dev5.tar`

### file list

```diff
@@ -1,175 +1,176 @@
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.262217 turboctl-1.1.1.dev4/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      104 2024-05-23 12:25:42.000000 turboctl-1.1.1.dev4/.gitignore
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.254217 turboctl-1.1.1.dev4/.hypothesis/
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.254217 turboctl-1.1.1.dev4/.hypothesis/examples/
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.254217 turboctl-1.1.1.dev4/.hypothesis/examples/098af05827140584/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/098af05827140584/236d65b6820cb9eb
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/098af05827140584/8f344065c6e31a55
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/098af05827140584/ebec0feb4a7296ef
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.254217 turboctl-1.1.1.dev4/.hypothesis/examples/3ef5c497a7146f5f/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/3ef5c497a7146f5f/37b7d6a6935710cc
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.254217 turboctl-1.1.1.dev4/.hypothesis/examples/6c152343fd7da806/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/6c152343fd7da806/37b7d6a6935710cc
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/6c152343fd7da806/bf2177f7c1c50efa
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/6c152343fd7da806/ebec0feb4a7296ef
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.254217 turboctl-1.1.1.dev4/.hypothesis/examples/719feafe55d6092a/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        5 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/719feafe55d6092a/008e1630a9922afd
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/719feafe55d6092a/27ed25acd9ac2252
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       12 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/719feafe55d6092a/88e1a36747cf7ba7
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/719feafe55d6092a/ecd6acb5382280fa
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        5 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/719feafe55d6092a/f8a0b55de165f0f7
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.254217 turboctl-1.1.1.dev4/.hypothesis/examples/79a409375dd4d4e2/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/79a409375dd4d4e2/0e3c5a512caa470e
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       27 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/79a409375dd4d4e2/1532c3657cb335c2
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/79a409375dd4d4e2/37b7d6a6935710cc
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       35 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/79a409375dd4d4e2/4b332aaacb70845a
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/79a409375dd4d4e2/8f344065c6e31a55
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/79a409375dd4d4e2/a92d75b981cc1d16
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.254217 turboctl-1.1.1.dev4/.hypothesis/examples/7ae13c50088acc79/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        8 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/7ae13c50088acc79/1157f47c0c21cc58
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        9 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/7ae13c50088acc79/5d9857cd134a7d76
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        6 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/7ae13c50088acc79/7f584f87e4c8748c
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/7ae13c50088acc79/bf2177f7c1c50efa
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        6 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/7ae13c50088acc79/bf9e0341c6723c0c
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/0b64596632c348d1
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        9 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/2a7de3a2e977d1bf
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        8 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/3159c3254a05fa28
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/563c99e486a45858
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/5be7ff32ddb1da60
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/658062a505f9a78d
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/71ebd30c888b37de
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/868d8d368a4a202b
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        8 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/91bd8eded23b9c4f
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/93e42aab04fa7201
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/9b6919dfe6d4ee68
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/a7ab860d9dd19a4f
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/d20a55593bc9dcb6
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/dd2d6fdd18636fda
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/e02700d5d11c71d4
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       26 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/e2d9c31bc45f7328
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/f62638bcbdd30c0d
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/examples/991880036e4bf226/f95b844e14efffe0
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.254217 turboctl-1.1.1.dev4/.hypothesis/unicode_data/
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/.hypothesis/unicode_data/11.0.0/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    20358 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/.hypothesis/unicode_data/11.0.0/charmap.json.gz
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      308 2024-05-23 12:53:17.000000 turboctl-1.1.1.dev4/.readthedocs.yaml
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1964 2024-05-23 12:55:08.262217 turboctl-1.1.1.dev4/PKG-INFO
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1448 2024-05-23 12:54:59.000000 turboctl-1.1.1.dev4/README.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1740 2024-05-23 12:45:14.000000 turboctl-1.1.1.dev4/TODO
--rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)      845 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/add-to-path
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.254217 turboctl-1.1.1.dev4/doc/
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/doc/sphinx/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      634 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/Makefile
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/doc/sphinx/_static/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      509 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/_static/custom.css
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    40547 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/advanced_UI.png
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      753 2024-05-23 12:43:53.000000 turboctl-1.1.1.dev4/doc/sphinx/changelog.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     3498 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/conf.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     8337 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/errata.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1436 2024-05-23 12:54:59.000000 turboctl-1.1.1.dev4/doc/sphinx/index.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1449 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/installation.rst
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/doc/sphinx/modules/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       78 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/hacks.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      388 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/index.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      163 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/main.rst
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/doc/sphinx/modules/telegram/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       99 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/telegram/api.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      128 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/telegram/codes.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      140 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/telegram/datatypes.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      227 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/telegram/index.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      108 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/telegram/parser.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      115 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/telegram/telegram.rst
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/doc/sphinx/modules/ui/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      108 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/ui/advanced_tui.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      117 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/ui/command_line_ui.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      123 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/ui/control_interface.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       84 2024-05-23 12:15:41.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/ui/docs.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      251 2024-05-23 12:16:35.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/ui/index.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       99 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/ui/queuefile.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      111 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/ui/status_format.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       87 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/ui/table.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       93 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/ui/widgets.rst
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/doc/sphinx/modules/virtualpump/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      153 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/virtualpump/hardware_component.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      292 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/virtualpump/index.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      545 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/virtualpump/parameter_component.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      150 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/virtualpump/virtualconnection.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      132 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules/virtualpump/virtualpump.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      557 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/modules.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      276 2024-05-23 10:52:05.000000 turboctl-1.1.1.dev4/doc/sphinx/requirements.txt
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    40532 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/doc/sphinx/simple_UI.png
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     8290 2024-05-23 11:35:23.000000 turboctl-1.1.1.dev4/doc/sphinx/usage.rst
--rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)      617 2024-05-23 12:21:02.000000 turboctl-1.1.1.dev4/make-docs
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     2588 2024-05-23 12:21:38.000000 turboctl-1.1.1.dev4/make_readme.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      286 2024-05-23 12:04:43.000000 turboctl-1.1.1.dev4/makefile
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      748 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/pyproject.toml
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       38 2024-05-23 12:55:08.262217 turboctl-1.1.1.dev4/setup.cfg
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/test_turboctl/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/__init__.py
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/test_turboctl/run_tests/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5303 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/run_tests/run_tests.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1590 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/run_tests/test_run_tests.py
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/test_turboctl/telegram/
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.254217 turboctl-1.1.1.dev4/test_turboctl/telegram/.hypothesis/
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.254217 turboctl-1.1.1.dev4/test_turboctl/telegram/.hypothesis/unicode_data/
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/test_turboctl/telegram/.hypothesis/unicode_data/11.0.0/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    20358 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/telegram/.hypothesis/unicode_data/11.0.0/charmap.json.gz
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/telegram/__init__.py
--rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)     3923 2020-07-24 18:46:53.000000 turboctl-1.1.1.dev4/test_turboctl/telegram/test_api.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     6031 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/telegram/test_codes.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    16462 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/test_turboctl/telegram/test_datatypes.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    13853 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/telegram/test_parser.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    17431 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev4/test_turboctl/telegram/test_telegram.py
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/test_turboctl/ui/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/ui/__init.py__
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     6682 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/ui/test_abstractui.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     3594 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/ui/test_command_parser.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     2359 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/ui/test_correct_error_message.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    10038 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/ui/test_output.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     4136 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/ui/test_table.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5049 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/ui/test_tui.py
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/test_turboctl/virtualpump/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/virtualpump/__init__.py
--rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)    15397 2020-07-24 14:54:13.000000 turboctl-1.1.1.dev4/test_turboctl/virtualpump/test_hardware_component.py
--rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)    18089 2020-07-22 11:34:05.000000 turboctl-1.1.1.dev4/test_turboctl/virtualpump/test_parameter_component.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     4253 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/virtualpump/test_virtualconnection.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5580 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/test_turboctl/virtualpump/test_virtualpump.py
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/turboctl/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      234 2024-05-23 12:54:21.000000 turboctl-1.1.1.dev4/turboctl/__init__.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5512 2024-05-23 11:34:07.000000 turboctl-1.1.1.dev4/turboctl/__main__.py
--rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     2631 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/turboctl/hacks.py
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.258217 turboctl-1.1.1.dev4/turboctl/telegram/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       78 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/turboctl/telegram/__init__.py
--rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     3972 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/turboctl/telegram/api.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    21340 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev4/turboctl/telegram/codes.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    17240 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/turboctl/telegram/datatypes.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     8444 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/turboctl/telegram/errors.txt
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    22442 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev4/turboctl/telegram/parameters.txt
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    18964 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/turboctl/telegram/parser.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    25563 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev4/turboctl/telegram/telegram.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     2972 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/turboctl/telegram/warnings.txt
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.262217 turboctl-1.1.1.dev4/turboctl/ui/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       70 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/turboctl/ui/__init__.py
--rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)     4670 2021-01-12 12:53:24.000000 turboctl-1.1.1.dev4/turboctl/ui/advanced_tui.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    19889 2024-05-23 11:35:55.000000 turboctl-1.1.1.dev4/turboctl/ui/command_line_ui.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     9720 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/turboctl/ui/control_interface.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      293 2024-05-23 12:17:25.000000 turboctl-1.1.1.dev4/turboctl/ui/docs.py
--rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)     3385 2020-07-03 12:38:41.000000 turboctl-1.1.1.dev4/turboctl/ui/queuefile.py
--rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     2862 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/turboctl/ui/status_format.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     6331 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev4/turboctl/ui/table.py
--rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)    21497 2021-01-12 12:53:13.000000 turboctl-1.1.1.dev4/turboctl/ui/widgets.py
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.262217 turboctl-1.1.1.dev4/turboctl/virtualpump/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       97 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/turboctl/virtualpump/__init__.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    18730 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev4/turboctl/virtualpump/hardware_component.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    15479 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/turboctl/virtualpump/parameter_component.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     7900 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/turboctl/virtualpump/virtualconnection.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     4241 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev4/turboctl/virtualpump/virtualpump.py
--rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     1051 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev4/turboctl-run
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:55:08.262217 turboctl-1.1.1.dev4/turboctl.egg-info/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1964 2024-05-23 12:55:08.000000 turboctl-1.1.1.dev4/turboctl.egg-info/PKG-INFO
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5449 2024-05-23 12:55:08.000000 turboctl-1.1.1.dev4/turboctl.egg-info/SOURCES.txt
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        1 2024-05-23 12:55:08.000000 turboctl-1.1.1.dev4/turboctl.egg-info/dependency_links.txt
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       52 2024-05-23 12:55:08.000000 turboctl-1.1.1.dev4/turboctl.egg-info/entry_points.txt
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       52 2024-05-23 12:55:08.000000 turboctl-1.1.1.dev4/turboctl.egg-info/requires.txt
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       32 2024-05-23 12:55:08.000000 turboctl-1.1.1.dev4/turboctl.egg-info/top_level.txt
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.543383 turboctl-1.1.1.dev5/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      104 2024-05-23 12:25:42.000000 turboctl-1.1.1.dev5/.gitignore
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.507383 turboctl-1.1.1.dev5/.hypothesis/
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.507383 turboctl-1.1.1.dev5/.hypothesis/examples/
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.511383 turboctl-1.1.1.dev5/.hypothesis/examples/098af05827140584/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/098af05827140584/236d65b6820cb9eb
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/098af05827140584/8f344065c6e31a55
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/098af05827140584/ebec0feb4a7296ef
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.511383 turboctl-1.1.1.dev5/.hypothesis/examples/3ef5c497a7146f5f/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/3ef5c497a7146f5f/37b7d6a6935710cc
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.515383 turboctl-1.1.1.dev5/.hypothesis/examples/6c152343fd7da806/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/6c152343fd7da806/37b7d6a6935710cc
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/6c152343fd7da806/bf2177f7c1c50efa
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/6c152343fd7da806/ebec0feb4a7296ef
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.515383 turboctl-1.1.1.dev5/.hypothesis/examples/719feafe55d6092a/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        5 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/719feafe55d6092a/008e1630a9922afd
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/719feafe55d6092a/27ed25acd9ac2252
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       12 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/719feafe55d6092a/88e1a36747cf7ba7
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/719feafe55d6092a/ecd6acb5382280fa
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        5 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/719feafe55d6092a/f8a0b55de165f0f7
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.515383 turboctl-1.1.1.dev5/.hypothesis/examples/79a409375dd4d4e2/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/79a409375dd4d4e2/0e3c5a512caa470e
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       27 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/79a409375dd4d4e2/1532c3657cb335c2
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/79a409375dd4d4e2/37b7d6a6935710cc
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       35 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/79a409375dd4d4e2/4b332aaacb70845a
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/79a409375dd4d4e2/8f344065c6e31a55
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/79a409375dd4d4e2/a92d75b981cc1d16
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.515383 turboctl-1.1.1.dev5/.hypothesis/examples/7ae13c50088acc79/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        8 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/7ae13c50088acc79/1157f47c0c21cc58
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        9 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/7ae13c50088acc79/5d9857cd134a7d76
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        6 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/7ae13c50088acc79/7f584f87e4c8748c
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/7ae13c50088acc79/bf2177f7c1c50efa
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        6 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/7ae13c50088acc79/bf9e0341c6723c0c
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.519383 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/0b64596632c348d1
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        9 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/2a7de3a2e977d1bf
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        8 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/3159c3254a05fa28
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/563c99e486a45858
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/5be7ff32ddb1da60
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/658062a505f9a78d
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/71ebd30c888b37de
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/868d8d368a4a202b
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        8 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/91bd8eded23b9c4f
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/93e42aab04fa7201
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/9b6919dfe6d4ee68
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/a7ab860d9dd19a4f
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/d20a55593bc9dcb6
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/dd2d6fdd18636fda
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/e02700d5d11c71d4
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       26 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/e2d9c31bc45f7328
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/f62638bcbdd30c0d
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/examples/991880036e4bf226/f95b844e14efffe0
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.511383 turboctl-1.1.1.dev5/.hypothesis/unicode_data/
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.519383 turboctl-1.1.1.dev5/.hypothesis/unicode_data/11.0.0/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    20358 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/.hypothesis/unicode_data/11.0.0/charmap.json.gz
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      431 2024-05-29 10:58:35.000000 turboctl-1.1.1.dev5/.readthedocs.yaml
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1964 2024-05-29 10:58:37.543383 turboctl-1.1.1.dev5/PKG-INFO
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1448 2024-05-29 10:58:35.000000 turboctl-1.1.1.dev5/README.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1902 2024-05-29 10:56:07.000000 turboctl-1.1.1.dev5/TODO
+-rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)      845 2024-05-28 13:36:38.000000 turboctl-1.1.1.dev5/add-to-path
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.511383 turboctl-1.1.1.dev5/doc/
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.519383 turboctl-1.1.1.dev5/doc/sphinx/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      634 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/Makefile
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.519383 turboctl-1.1.1.dev5/doc/sphinx/_static/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      509 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/_static/custom.css
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    40547 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/advanced_UI.png
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      704 2024-05-29 10:45:39.000000 turboctl-1.1.1.dev5/doc/sphinx/changelog.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     4164 2024-05-29 10:21:32.000000 turboctl-1.1.1.dev5/doc/sphinx/conf.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     8337 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/errata.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1437 2024-05-29 10:58:35.000000 turboctl-1.1.1.dev5/doc/sphinx/index.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1356 2024-05-28 12:56:02.000000 turboctl-1.1.1.dev5/doc/sphinx/installation.rst
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.523383 turboctl-1.1.1.dev5/doc/sphinx/modules/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      111 2024-05-24 12:18:24.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/global_constants.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       78 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/hacks.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      412 2024-05-24 12:17:40.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/index.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      163 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/main.rst
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.523383 turboctl-1.1.1.dev5/doc/sphinx/modules/telegram/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       99 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/telegram/api.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      128 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/telegram/codes.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      140 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/telegram/datatypes.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      227 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/telegram/index.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      108 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/telegram/parser.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      115 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/telegram/telegram.rst
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.527383 turboctl-1.1.1.dev5/doc/sphinx/modules/ui/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      108 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/ui/advanced_tui.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      117 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/ui/command_line_ui.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      123 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/ui/control_interface.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      238 2024-05-24 12:07:44.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/ui/index.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       99 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/ui/queuefile.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      111 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/ui/status_format.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       87 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/ui/table.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       93 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/ui/widgets.rst
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.527383 turboctl-1.1.1.dev5/doc/sphinx/modules/virtualpump/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      153 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/virtualpump/hardware_component.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      292 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/virtualpump/index.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      545 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/virtualpump/parameter_component.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      150 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/virtualpump/virtualconnection.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      132 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules/virtualpump/virtualpump.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      557 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/modules.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      230 2024-05-23 13:27:16.000000 turboctl-1.1.1.dev5/doc/sphinx/requirements.txt
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      153 2024-05-29 10:58:35.000000 turboctl-1.1.1.dev5/doc/sphinx/reverse_sphinx_path.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    40532 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/doc/sphinx/simple_UI.png
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     8297 2024-05-29 10:34:12.000000 turboctl-1.1.1.dev5/doc/sphinx/usage.rst
+-rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)      238 2024-05-29 10:02:12.000000 turboctl-1.1.1.dev5/make-docs
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     4867 2024-05-29 09:59:45.000000 turboctl-1.1.1.dev5/make_files.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      339 2024-05-28 13:08:06.000000 turboctl-1.1.1.dev5/makefile
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      868 2024-05-29 10:58:35.000000 turboctl-1.1.1.dev5/pyproject.toml
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       38 2024-05-29 10:58:37.543383 turboctl-1.1.1.dev5/setup.cfg
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.527383 turboctl-1.1.1.dev5/test_turboctl/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/__init__.py
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.527383 turboctl-1.1.1.dev5/test_turboctl/run_tests/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5303 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/run_tests/run_tests.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1590 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/run_tests/test_run_tests.py
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.531383 turboctl-1.1.1.dev5/test_turboctl/telegram/
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.511383 turboctl-1.1.1.dev5/test_turboctl/telegram/.hypothesis/
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.511383 turboctl-1.1.1.dev5/test_turboctl/telegram/.hypothesis/unicode_data/
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.531383 turboctl-1.1.1.dev5/test_turboctl/telegram/.hypothesis/unicode_data/11.0.0/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    20358 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/telegram/.hypothesis/unicode_data/11.0.0/charmap.json.gz
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/telegram/__init__.py
+-rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)     3923 2020-07-24 18:46:53.000000 turboctl-1.1.1.dev5/test_turboctl/telegram/test_api.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     6031 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/telegram/test_codes.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    16462 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/test_turboctl/telegram/test_datatypes.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    13853 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/telegram/test_parser.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    17431 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev5/test_turboctl/telegram/test_telegram.py
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.531383 turboctl-1.1.1.dev5/test_turboctl/ui/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/ui/__init.py__
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     6682 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/ui/test_abstractui.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     3594 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/ui/test_command_parser.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     2359 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/ui/test_correct_error_message.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    10038 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/ui/test_output.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     4136 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/ui/test_table.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5049 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/ui/test_tui.py
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.531383 turboctl-1.1.1.dev5/test_turboctl/virtualpump/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/virtualpump/__init__.py
+-rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)    15397 2020-07-24 14:54:13.000000 turboctl-1.1.1.dev5/test_turboctl/virtualpump/test_hardware_component.py
+-rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)    18089 2020-07-22 11:34:05.000000 turboctl-1.1.1.dev5/test_turboctl/virtualpump/test_parameter_component.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     4253 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/virtualpump/test_virtualconnection.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5580 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/test_turboctl/virtualpump/test_virtualpump.py
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.535383 turboctl-1.1.1.dev5/turboctl/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      134 2024-05-24 12:19:03.000000 turboctl-1.1.1.dev5/turboctl/__init__.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5550 2024-05-29 10:37:14.000000 turboctl-1.1.1.dev5/turboctl/__main__.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     2250 2024-05-29 10:29:12.000000 turboctl-1.1.1.dev5/turboctl/global_constants.py
+-rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     2631 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/turboctl/hacks.py
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.539383 turboctl-1.1.1.dev5/turboctl/telegram/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       78 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/turboctl/telegram/__init__.py
+-rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     3972 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/turboctl/telegram/api.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    21340 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev5/turboctl/telegram/codes.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    17240 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/turboctl/telegram/datatypes.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     8444 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/turboctl/telegram/errors.txt
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    22442 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev5/turboctl/telegram/parameters.txt
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    18964 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/turboctl/telegram/parser.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    25563 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev5/turboctl/telegram/telegram.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     2972 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/turboctl/telegram/warnings.txt
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.539383 turboctl-1.1.1.dev5/turboctl/ui/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       70 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/turboctl/ui/__init__.py
+-rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)     4670 2021-01-12 12:53:24.000000 turboctl-1.1.1.dev5/turboctl/ui/advanced_tui.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    19911 2024-05-24 11:59:57.000000 turboctl-1.1.1.dev5/turboctl/ui/command_line_ui.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     9720 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/turboctl/ui/control_interface.py
+-rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)     3385 2020-07-03 12:38:41.000000 turboctl-1.1.1.dev5/turboctl/ui/queuefile.py
+-rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     2862 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/turboctl/ui/status_format.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     6331 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev5/turboctl/ui/table.py
+-rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)    21497 2021-01-12 12:53:13.000000 turboctl-1.1.1.dev5/turboctl/ui/widgets.py
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.543383 turboctl-1.1.1.dev5/turboctl/virtualpump/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       97 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/turboctl/virtualpump/__init__.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    18730 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev5/turboctl/virtualpump/hardware_component.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    15479 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/turboctl/virtualpump/parameter_component.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     7900 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/turboctl/virtualpump/virtualconnection.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     4241 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev5/turboctl/virtualpump/virtualpump.py
+-rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)      280 2024-05-29 10:12:27.000000 turboctl-1.1.1.dev5/turboctl-run
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-29 10:58:37.543383 turboctl-1.1.1.dev5/turboctl.egg-info/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1964 2024-05-29 10:58:37.000000 turboctl-1.1.1.dev5/turboctl.egg-info/PKG-INFO
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5500 2024-05-29 10:58:37.000000 turboctl-1.1.1.dev5/turboctl.egg-info/SOURCES.txt
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        1 2024-05-29 10:58:37.000000 turboctl-1.1.1.dev5/turboctl.egg-info/dependency_links.txt
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       52 2024-05-29 10:58:37.000000 turboctl-1.1.1.dev5/turboctl.egg-info/entry_points.txt
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       52 2024-05-29 10:58:37.000000 turboctl-1.1.1.dev5/turboctl.egg-info/requires.txt
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       32 2024-05-29 10:58:37.000000 turboctl-1.1.1.dev5/turboctl.egg-info/top_level.txt
```

### Comparing `turboctl-1.1.1.dev4/.hypothesis/unicode_data/11.0.0/charmap.json.gz` & `turboctl-1.1.1.dev5/.hypothesis/unicode_data/11.0.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/PKG-INFO` & `turboctl-1.1.1.dev5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: turboctl
-Version: 1.1.1.dev4
+Version: 1.1.1.dev5
 Summary: TurboCtl is a RS-232 controller for a Leybold TURBOVAC i or iX turbovacuum pump.
 Author: Feliks Kivelä
 License: GPL-3.0-or-later
-Project-URL: Homepage, https://github.com/fkivela/TurboCtl
+Project-URL: homepage, https://github.com/fkivela/TurboCtl
 Keywords: RS-232,Turbovac
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Requires-Dist: pyserial
 Requires-Dist: tabulate
 Provides-Extra: urwid
 Requires-Dist: urwid; extra == "urwid"
 Provides-Extra: test
 Requires-Dist: hypothesis; extra == "test"
 
-.. Note: This file is automatically generated by make_readme.py.
+.. Note: This file was automatically generated by make_files.py.
 .. To make changes to this file, edit that instead of this.
 
 TurboCtl
 ========
 
 TurboCtl is a RS-232 controller for a Leybold TURBOVAC i or iX turbovacuum
 pump. It was written in Python 3 and is intended for Linux operating systems.
@@ -43,15 +43,15 @@
 
 The GitHub home page of the TurboCtl project can be found
 `here <https://github.com/fkivela/TurboCtl>`__.
 
 Version
 -------
 
-This is version 1.1.1.dev4 of TurboCtl.
+This is version 1.1.1.dev5 of TurboCtl.
 
 License
 -------
 
 TurboCtl is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `turboctl-1.1.1.dev4/README.rst` & `turboctl-1.1.1.dev5/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. Note: This file is automatically generated by make_readme.py.
+.. Note: This file was automatically generated by make_files.py.
 .. To make changes to this file, edit that instead of this.
 
 TurboCtl
 ========
 
 TurboCtl is a RS-232 controller for a Leybold TURBOVAC i or iX turbovacuum
 pump. It was written in Python 3 and is intended for Linux operating systems.
@@ -26,15 +26,15 @@
 
 The GitHub home page of the TurboCtl project can be found
 `here <https://github.com/fkivela/TurboCtl>`__.
 
 Version
 -------
 
-This is version 1.1.1.dev4 of TurboCtl.
+This is version 1.1.1.dev5 of TurboCtl.
 
 License
 -------
 
 TurboCtl is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `turboctl-1.1.1.dev4/TODO` & `turboctl-1.1.1.dev5/TODO`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,32 @@
 TODO
 
 Soon:
-- Make a GitHub release?
-- Make sure PyPI links & other instructions in the docs work
+- Add TurboCtl to conda-forge
+- Add a message telling to install Urwid when TurboCtl is run without Urwid being installed or the -s argument being used
+- Find out which files exactly are included in the package on PyPI and remove unnecessary ones such as documentation
+- Add "p" as an alias for the "pump" command
+- Update the instructional pictures in the Usage section of the documentation
 
 Later:
-- Add TurboCtl to conda-forge
-- Add an error message when Urwid is not installed
-- Remove unnecessary dev files from the distributed package
-- Add an alias to the pump command
-- Update the usage pics
-- Update tests
-- Fix double colons in Sphinx-generated parameter lists.
-- Reformat alias lists to match the usage page.
-- Make sure the program crashes elegantly when e.g. it cannot connect to the
-  pump.
-- Add commands to set the setpoint (most important), save data, read errors
-  etc.
-- Move singledispatchmethod to datatypes.py.
-- Run pylint/pycodestyle.
-- Make sure there are no TODO tags anywhere is the code.
-- Replace custom scrollbar implementation with the new Urwid one
+- Update the tests
+- Fix double colons in Sphinx-generated parameter lists
+- Reformat the aliases in the in-program help (h commanmd) to match the Usage page (i.e. move the aliases from the end of the command description to the start)
+- Make sure the program crashes elegantly when e.g. it cannot connect to the pump
+- Add commands to set the setpoint (most important), save data, read errors etc.
+- Run pylint/pycodestyle
+- Make sure there are no TODO tags anywhere in the code
+- Replace the custom scrollbar implementation with the new Urwid one
 
 Perhaps at some point:
 - Make sure only one user can control the pump at a time
 - Improve the parser so that e.g. "list p [1, 2]" is valid syntax.
   The command parser could also be moved into a separate class, so that it
   could be tested more easily. Also, parser.py might be simplified by using
   the parsing modules in the standard library.
-- Document the format in parameters.txt better? This might even be turned into
-  e.g. a CSV file.
-- Document individual enum members in codes.py.
+- Document the format in parameters.txt better? This might even be turned into e.g. a CSV file.
+- Document individual enum members in codes.py
 - Rename WrongNumError to NumberError or something?
-- Open the output of the info and help commands with less if a specific
-  argument is given?
-- The docstrings of the read/write_parameter methods say
-  "Raises ValueError if number or index have invalid values". Clarify this.
-- Add instructions for importing the API/control interface (and also add 
-  those to the turboctl namespace)
-- Fix the bug where closing TurboCtl in screen doesn't erase the UI text.
+- Open the output of the info and help commands with less if a specific argument is given?
+- The docstrings of the read/write_parameter methods say "Raises ValueError if number or index have invalid values". Clarify this.
+- Add instructions for importing the API/control interface (and also add those to the turboctl namespace)
+- Fix the bug where closing TurboCtl in screen doesn't erase the UI text
```

### Comparing `turboctl-1.1.1.dev4/add-to-path` & `turboctl-1.1.1.dev5/add-to-path`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/doc/sphinx/Makefile` & `turboctl-1.1.1.dev5/doc/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/doc/sphinx/advanced_UI.png` & `turboctl-1.1.1.dev5/doc/sphinx/advanced_UI.png`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/doc/sphinx/changelog.rst` & `turboctl-1.1.1.dev5/doc/sphinx/changelog.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Changelog
 =========
 
 This page documents what's new in each updated version of TurboCtl.
 
-Version 1.1.1
--------------
+Version 1.1.1 (2024-05-29)
+--------------------------
 
-* Moved TurboCtl documentation to `Read the Docs <https://turboctl.readthedocs.io/en/latest/index.html>`_.
+* Moved TurboCtl documentation to `Read the Docs`_.
   Previously documentation could be viewed online via https://html-preview.github.io/, but this broke some links.
 * Added the :option:`-d` command line argument.
 
 
-Version 1.1.0
--------------
+Version 1.1.0 (2024-05-22)
+--------------------------
 
 * Starting TurboCtl now maintains the on/off state of the pump instead of always turning the pump on.
 * Made TurboCtl available on PyPI_ and updated the installation instructions.
 * Added the :option:`docs` and :option:`reset` commands.
 * Made several other small improvements and fixes.
-
-.. _PyPI: https://pypi.org/project/turboctl/
```

### Comparing `turboctl-1.1.1.dev4/doc/sphinx/conf.py` & `turboctl-1.1.1.dev5/doc/sphinx/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 # Configuration file for the Sphinx documentation builder.
 #
 # This file only contains a selection of the most common options. For a full
 # list see the documentation:
 # http://www.sphinx-doc.org/en/master/config
 
+
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#
-# import os
-# import sys
-# sys.path.insert(0, os.path.abspath('.'))
 
-# The TurboCtl directory should already be in $PATH.
+from pathlib import Path
+import sys
+
+# We need to do the path management here because Read the Docs doesn't support
+# the use of a makefile.
+# Add this directory to the path so that we can import reverse_sphinx_path. 
+sphinx_path = Path('__file__').parent.resolve()
+# This doesn't work if we don't convert the path to a string!
+sys.path.append(str(sphinx_path))
+
+from reverse_sphinx_path import REVERSE_SPHINX_PATH
+
+# With REVERSE_SPHINX_PATH we can add the TurboCtl directory to the path and
+# import turboctl. 
+TurboCtl_path = Path(REVERSE_SPHINX_PATH).resolve()
+sys.path.append(str(TurboCtl_path))
+
 
 # -- Project information -----------------------------------------------------
-import turboctl
+from turboctl import global_constants
 
 project = 'TurboCtl'
-author = 'Feliks Kivelä'
-version = turboctl.__version__
-copyright = turboctl.copyright
-# The copyright variable is automatically written to the HTML footer.
+author = global_constants.AUTHOR
+version = global_constants.VERSION
+project_copyright = global_constants.COPYRIGHT
+
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 
@@ -76,14 +89,21 @@
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
+# This included at the end of every rst source file. 
+rst_epilog = f"""
+.. _GitHub: {global_constants.GITHUB_URL}
+.. _PyPI: {global_constants.PYPI_URL}
+.. _`Read the Docs`: {global_constants.DOCS_URL}
+"""
+
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 
 html_theme = 'alabaster'
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `turboctl-1.1.1.dev4/doc/sphinx/errata.rst` & `turboctl-1.1.1.dev5/doc/sphinx/errata.rst`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/doc/sphinx/index.rst` & `turboctl-1.1.1.dev5/doc/sphinx/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. Note: This file is automatically generated by make_readme.py.
+.. Note: This file was automatically generated by make_files.py.
 .. To make changes to this file, edit that instead of this.
 
 TurboCtl
 ========
 
 TurboCtl is a RS-232 controller for a Leybold TURBOVAC i or iX turbovacuum
 pump. It was written in Python 3 and is intended for Linux operating systems.
@@ -14,14 +14,15 @@
 
    installation.rst
    usage.rst
    modules.rst
    errata.rst
    changelog.rst
 
+
 Author
 ------
 
 TurboCtl was written by Feliks Kivelä.
 The author can be contacted at firstname.lastname@aalto.fi
 (with the "ä" replaced by an "a").
 
@@ -32,15 +33,15 @@
 
 The GitHub home page of the TurboCtl project can be found
 `here <https://github.com/fkivela/TurboCtl>`__.
 
 Version
 -------
 
-This is version 1.1.1.dev4 of TurboCtl.
+This is version 1.1.1.dev5 of TurboCtl.
 
 License
 -------
 
 TurboCtl is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `turboctl-1.1.1.dev4/doc/sphinx/installation.rst` & `turboctl-1.1.1.dev5/doc/sphinx/installation.rst`

 * *Files 15% similar despite different names*

```diff
@@ -51,11 +51,9 @@
 the command
 
 ::
 
     sudo adduser <username> dialout
 
 
-.. _PyPI: https://pypi.org/project/turboctl/
 .. _Urwid: http://urwid.org/
 .. _Hypothesis: https://hypothesis.readthedocs.io/en/latest/
-.. _GitHub: https://github.com/fkivela/TurboCtl
```

### Comparing `turboctl-1.1.1.dev4/doc/sphinx/modules/virtualpump/parameter_component.rst` & `turboctl-1.1.1.dev5/doc/sphinx/modules/virtualpump/parameter_component.rst`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/doc/sphinx/modules.rst` & `turboctl-1.1.1.dev5/doc/sphinx/modules.rst`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/doc/sphinx/simple_UI.png` & `turboctl-1.1.1.dev5/doc/sphinx/simple_UI.png`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/doc/sphinx/usage.rst` & `turboctl-1.1.1.dev5/doc/sphinx/usage.rst`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                     
     If TurboCtl is run without the :option:`-s` argument, a more advanced UI will be used.
                     
 .. option:: -n, --no-poll
 
     Don't send automatic telegrams to the pump.
                     
-    The pump automatically turns off if it doesn't receive any commands for about 10 seconds.
+    The pump automatically turns off if it doesn't receive a "turn on" command for about 10 seconds.
     Normally TurboCtl sends automatic telegrams to the pump at regular intervals in order to prevent this from happening, and also to keep the status screen in the advanced UI updated.
     This argument prevents these automatic telegrams from being sent.
 
 .. option:: -t, --test
 
     Instead of running the TurboCtl program, run all automatic tests for it.
```

### Comparing `turboctl-1.1.1.dev4/pyproject.toml` & `turboctl-1.1.1.dev5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Note: This file was automatically generated by make_files.py.
+# To make changes to this file, edit that instead of this.
+
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "turboctl"
 description = "TurboCtl is a RS-232 controller for a Leybold TURBOVAC i or iX turbovacuum pump."
@@ -16,16 +19,16 @@
 dynamic = ["version"]
 
 [project.optional-dependencies]
 urwid = ["urwid"]
 test = ["hypothesis"]
 
 [project.urls]
-Homepage = "https://github.com/fkivela/TurboCtl"
+homepage = "https://github.com/fkivela/TurboCtl"
 
 [project.scripts]
 turboctl = "turboctl.__main__:main"
 
 [tool.setuptools.packages.find]
 
 [tool.setuptools.dynamic]
-version = {attr = "turboctl.__version__"}
+version = {attr = "turboctl.VERSION"}
```

### Comparing `turboctl-1.1.1.dev4/test_turboctl/run_tests/run_tests.py` & `turboctl-1.1.1.dev5/test_turboctl/run_tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/run_tests/test_run_tests.py` & `turboctl-1.1.1.dev5/test_turboctl/run_tests/test_run_tests.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/telegram/.hypothesis/unicode_data/11.0.0/charmap.json.gz` & `turboctl-1.1.1.dev5/test_turboctl/telegram/.hypothesis/unicode_data/11.0.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/telegram/test_api.py` & `turboctl-1.1.1.dev5/test_turboctl/telegram/test_api.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/telegram/test_codes.py` & `turboctl-1.1.1.dev5/test_turboctl/telegram/test_codes.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/telegram/test_datatypes.py` & `turboctl-1.1.1.dev5/test_turboctl/telegram/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/telegram/test_parser.py` & `turboctl-1.1.1.dev5/test_turboctl/telegram/test_parser.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/telegram/test_telegram.py` & `turboctl-1.1.1.dev5/test_turboctl/telegram/test_telegram.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/ui/test_abstractui.py` & `turboctl-1.1.1.dev5/test_turboctl/ui/test_abstractui.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/ui/test_command_parser.py` & `turboctl-1.1.1.dev5/test_turboctl/ui/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/ui/test_correct_error_message.py` & `turboctl-1.1.1.dev5/test_turboctl/ui/test_correct_error_message.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/ui/test_output.py` & `turboctl-1.1.1.dev5/test_turboctl/ui/test_output.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/ui/test_table.py` & `turboctl-1.1.1.dev5/test_turboctl/ui/test_table.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/ui/test_tui.py` & `turboctl-1.1.1.dev5/test_turboctl/ui/test_tui.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/virtualpump/test_hardware_component.py` & `turboctl-1.1.1.dev5/test_turboctl/virtualpump/test_hardware_component.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/virtualpump/test_parameter_component.py` & `turboctl-1.1.1.dev5/test_turboctl/virtualpump/test_parameter_component.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/virtualpump/test_virtualconnection.py` & `turboctl-1.1.1.dev5/test_turboctl/virtualpump/test_virtualconnection.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/test_turboctl/virtualpump/test_virtualpump.py` & `turboctl-1.1.1.dev5/test_turboctl/virtualpump/test_virtualpump.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/__main__.py` & `turboctl-1.1.1.dev5/turboctl/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """This is the main script used to run TurboCtl."""
 
 import argparse
 import sys
+import webbrowser
 
+from turboctl.global_constants import DOCS_URL
 from turboctl.ui import status_format
 from turboctl.ui.command_line_ui import CommandLineUI
-from turboctl.ui.docs import docs
 from turboctl.ui.queuefile import QueueFile
 from turboctl.virtualpump.virtualpump import VirtualPump
 from test_turboctl.run_tests.run_tests import run_tests
 
 
 ### Command-line arguments ###
 
@@ -36,28 +37,28 @@
                          action='store_true')
 vpump_group.add_argument('-p', '--port', 
                          help='the address of the serial port device')
 
 # Automatic polling can be disabled with this argument in all modes (even
 # though this doesn't do anything in doc/test mode).
 parser.add_argument('-n', '--no-poll',
-                    help=('do not poll the status of the pump by sending '
-                          'automatic telegrams'), 
+                    help=('do not send automatic telegrams that keep the '
+                          'pump on'), 
                     action='store_true')
 
 args = parser.parse_args()
 
 
 ### The main part of the script ###
 
 def main():
     """Execute the script."""
 
     if args.docs:
-        docs()
+        webbrowser.open(DOCS_URL)
         return
 
     if args.test:
         run_tests()
         return
     
     try:
```

### Comparing `turboctl-1.1.1.dev4/turboctl/hacks.py` & `turboctl-1.1.1.dev5/turboctl/hacks.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/telegram/api.py` & `turboctl-1.1.1.dev5/turboctl/telegram/api.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/telegram/codes.py` & `turboctl-1.1.1.dev5/turboctl/telegram/codes.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/telegram/datatypes.py` & `turboctl-1.1.1.dev5/turboctl/telegram/datatypes.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/telegram/errors.txt` & `turboctl-1.1.1.dev5/turboctl/telegram/errors.txt`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/telegram/parameters.txt` & `turboctl-1.1.1.dev5/turboctl/telegram/parameters.txt`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/telegram/parser.py` & `turboctl-1.1.1.dev5/turboctl/telegram/parser.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/telegram/telegram.py` & `turboctl-1.1.1.dev5/turboctl/telegram/telegram.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/telegram/warnings.txt` & `turboctl-1.1.1.dev5/turboctl/telegram/warnings.txt`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/ui/advanced_tui.py` & `turboctl-1.1.1.dev5/turboctl/ui/advanced_tui.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/ui/command_line_ui.py` & `turboctl-1.1.1.dev5/turboctl/ui/command_line_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import ast
 import inspect
 from pathlib import Path
 # Importing readline adds command editing etc. to the input function.
 import readline  # pylint: disable=unused-import
 import sys
 import textwrap
+import webbrowser
 
-from turboctl import __version__
+from turboctl.global_constants import DOCS_URL, VERSION
 from turboctl.telegram.parser import PARAMETERS, ERRORS, WARNINGS
 from turboctl.ui.control_interface import ControlInterface
-from turboctl.ui.docs import docs
 from turboctl.ui.table import table
 
 
 class CommandLineUI:
     """A simple command-line UI.
 
     Instances of this class should be closed after they are no longer
@@ -146,15 +146,15 @@
         # Replacing sys.stdin and sys.stdout would be simpler, but
         # could lead to unintended consequences, and would e.g.
         # prevent using multiple CommandLineUIs at once.
 
         self.control_interface = ControlInterface(port, auto_update)
         self.debug = False
         self.verbose = False
-        self.intro = (f"Welcome to TurboCtl v. {__version__}! "
+        self.intro = (f"Welcome to TurboCtl v. {VERSION}! "
                       f"Type 'help' for a list of commands.")
         self.prompt = '>> '
         self._stop_flag = False
 
     def __enter__(self):
         """Called upon entering a ``with`` block; returns *self*."""
         return self
@@ -313,15 +313,15 @@
             string = ('Valid commands:\n'
                       + textwrap.indent(description_str, self.indent))
 
         self.print(string)
 
     def cmd_docs(self):
         """Open TurboCtl documentation in a web browser."""
-        docs()
+        webbrowser.open(DOCS_URL)
 
     def _helpstring(self, cmdname):
         """Return a help message describing the usage of *cmdname*."""
         method = self._get_method(cmdname)
         argstr = self._argstring(method)
         aliasstr = self._alias_string(cmdname)
         docstr = inspect.getdoc(method)
```

### Comparing `turboctl-1.1.1.dev4/turboctl/ui/control_interface.py` & `turboctl-1.1.1.dev5/turboctl/ui/control_interface.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/ui/queuefile.py` & `turboctl-1.1.1.dev5/turboctl/ui/queuefile.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/ui/status_format.py` & `turboctl-1.1.1.dev5/turboctl/ui/status_format.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/ui/table.py` & `turboctl-1.1.1.dev5/turboctl/ui/table.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/ui/widgets.py` & `turboctl-1.1.1.dev5/turboctl/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/virtualpump/hardware_component.py` & `turboctl-1.1.1.dev5/turboctl/virtualpump/hardware_component.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/virtualpump/parameter_component.py` & `turboctl-1.1.1.dev5/turboctl/virtualpump/parameter_component.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/virtualpump/virtualconnection.py` & `turboctl-1.1.1.dev5/turboctl/virtualpump/virtualconnection.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl/virtualpump/virtualpump.py` & `turboctl-1.1.1.dev5/turboctl/virtualpump/virtualpump.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev4/turboctl.egg-info/PKG-INFO` & `turboctl-1.1.1.dev5/turboctl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: turboctl
-Version: 1.1.1.dev4
+Version: 1.1.1.dev5
 Summary: TurboCtl is a RS-232 controller for a Leybold TURBOVAC i or iX turbovacuum pump.
 Author: Feliks Kivelä
 License: GPL-3.0-or-later
-Project-URL: Homepage, https://github.com/fkivela/TurboCtl
+Project-URL: homepage, https://github.com/fkivela/TurboCtl
 Keywords: RS-232,Turbovac
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Requires-Dist: pyserial
 Requires-Dist: tabulate
 Provides-Extra: urwid
 Requires-Dist: urwid; extra == "urwid"
 Provides-Extra: test
 Requires-Dist: hypothesis; extra == "test"
 
-.. Note: This file is automatically generated by make_readme.py.
+.. Note: This file was automatically generated by make_files.py.
 .. To make changes to this file, edit that instead of this.
 
 TurboCtl
 ========
 
 TurboCtl is a RS-232 controller for a Leybold TURBOVAC i or iX turbovacuum
 pump. It was written in Python 3 and is intended for Linux operating systems.
@@ -43,15 +43,15 @@
 
 The GitHub home page of the TurboCtl project can be found
 `here <https://github.com/fkivela/TurboCtl>`__.
 
 Version
 -------
 
-This is version 1.1.1.dev4 of TurboCtl.
+This is version 1.1.1.dev5 of TurboCtl.
 
 License
 -------
 
 TurboCtl is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `turboctl-1.1.1.dev4/turboctl.egg-info/SOURCES.txt` & `turboctl-1.1.1.dev5/turboctl.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .gitignore
 .readthedocs.yaml
 README.rst
 TODO
 add-to-path
 make-docs
-make_readme.py
+make_files.py
 makefile
 pyproject.toml
 turboctl-run
 .hypothesis/examples/098af05827140584/236d65b6820cb9eb
 .hypothesis/examples/098af05827140584/8f344065c6e31a55
 .hypothesis/examples/098af05827140584/ebec0feb4a7296ef
 .hypothesis/examples/3ef5c497a7146f5f/37b7d6a6935710cc
@@ -55,30 +55,31 @@
 doc/sphinx/changelog.rst
 doc/sphinx/conf.py
 doc/sphinx/errata.rst
 doc/sphinx/index.rst
 doc/sphinx/installation.rst
 doc/sphinx/modules.rst
 doc/sphinx/requirements.txt
+doc/sphinx/reverse_sphinx_path.py
 doc/sphinx/simple_UI.png
 doc/sphinx/usage.rst
 doc/sphinx/_static/custom.css
+doc/sphinx/modules/global_constants.rst
 doc/sphinx/modules/hacks.rst
 doc/sphinx/modules/index.rst
 doc/sphinx/modules/main.rst
 doc/sphinx/modules/telegram/api.rst
 doc/sphinx/modules/telegram/codes.rst
 doc/sphinx/modules/telegram/datatypes.rst
 doc/sphinx/modules/telegram/index.rst
 doc/sphinx/modules/telegram/parser.rst
 doc/sphinx/modules/telegram/telegram.rst
 doc/sphinx/modules/ui/advanced_tui.rst
 doc/sphinx/modules/ui/command_line_ui.rst
 doc/sphinx/modules/ui/control_interface.rst
-doc/sphinx/modules/ui/docs.rst
 doc/sphinx/modules/ui/index.rst
 doc/sphinx/modules/ui/queuefile.rst
 doc/sphinx/modules/ui/status_format.rst
 doc/sphinx/modules/ui/table.rst
 doc/sphinx/modules/ui/widgets.rst
 doc/sphinx/modules/virtualpump/hardware_component.rst
 doc/sphinx/modules/virtualpump/index.rst
@@ -105,14 +106,15 @@
 test_turboctl/virtualpump/__init__.py
 test_turboctl/virtualpump/test_hardware_component.py
 test_turboctl/virtualpump/test_parameter_component.py
 test_turboctl/virtualpump/test_virtualconnection.py
 test_turboctl/virtualpump/test_virtualpump.py
 turboctl/__init__.py
 turboctl/__main__.py
+turboctl/global_constants.py
 turboctl/hacks.py
 turboctl.egg-info/PKG-INFO
 turboctl.egg-info/SOURCES.txt
 turboctl.egg-info/dependency_links.txt
 turboctl.egg-info/entry_points.txt
 turboctl.egg-info/requires.txt
 turboctl.egg-info/top_level.txt
@@ -125,15 +127,14 @@
 turboctl/telegram/parser.py
 turboctl/telegram/telegram.py
 turboctl/telegram/warnings.txt
 turboctl/ui/__init__.py
 turboctl/ui/advanced_tui.py
 turboctl/ui/command_line_ui.py
 turboctl/ui/control_interface.py
-turboctl/ui/docs.py
 turboctl/ui/queuefile.py
 turboctl/ui/status_format.py
 turboctl/ui/table.py
 turboctl/ui/widgets.py
 turboctl/virtualpump/__init__.py
 turboctl/virtualpump/hardware_component.py
 turboctl/virtualpump/parameter_component.py
```

