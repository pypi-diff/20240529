# Comparing `tmp/vss-cli-2024.6.0.dev0.tar.gz` & `tmp/vss-cli-2024.6.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vss-cli-2024.6.0.dev0.tar", last modified: Mon May 27 16:01:16 2024, max compression
+gzip compressed data, was "vss-cli-2024.6.0.dev4.tar", last modified: Wed May 29 17:57:30 2024, max compression
```

## Comparing `vss-cli-2024.6.0.dev0.tar` & `vss-cli-2024.6.0.dev4.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.038016 vss-cli-2024.6.0.dev0/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13950 2024-05-27 16:01:16.038016 vss-cli-2024.6.0.dev0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10991 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-27 16:01:16.038016 vss-cli-2024.6.0.dev0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3827 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.022016 vss-cli-2024.6.0.dev0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5569 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/tests/test_vss_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.026016 vss-cli-2024.6.0.dev0/vss_cli/
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19671 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/autocompletion.py
--rw-rw-rw-   0 root         (0) root         (0)     7659 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    65652 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)    15583 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.026016 vss-cli-2024.6.0.dev0/vss_cli/data/
--rw-rw-rw-   0 root         (0) root         (0)     4500 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/data/clib.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4288 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/data/clone.yaml
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/data/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2892 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/data/image.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2926 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/data/shell.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4198 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/data/template.yaml
--rw-rw-rw-   0 root         (0) root         (0)    25960 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/data_types.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/hcio.py
--rw-rw-rw-   0 root         (0) root         (0)    12512 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.030016 vss-cli-2024.6.0.dev0/vss_cli/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 16:01:11.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15976 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/account.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/completion.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2024-05-24 16:04:34.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.034016 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8906 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/callbacks.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/contentlib.py
--rw-rw-rw-   0 root         (0) root         (0)     2813 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     3133 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/floppy.py
--rw-rw-rw-   0 root         (0) root         (0)     8680 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/helper.py
--rw-rw-rw-   0 root         (0) root         (0)     3287 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     3046 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/iso.py
--rw-rw-rw-   0 root         (0) root         (0)     3477 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/net.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/os.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/rel_args.py
--rw-rw-rw-   0 root         (0) root         (0)     9604 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/rel_opts.py
--rw-rw-rw-   0 root         (0) root         (0)     3790 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/template.py
--rw-rw-rw-   0 root         (0) root         (0)   150500 2024-05-24 16:04:34.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/vm.py
--rw-rw-rw-   0 root         (0) root         (0)     1907 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/vmdks.py
--rw-rw-rw-   0 root         (0) root         (0)    10871 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/configure.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/key.py
--rw-rw-rw-   0 root         (0) root         (0)     3010 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/message.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     4310 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/ovf.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/plugins.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/raw.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.034016 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/change.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/export.py
--rw-rw-rw-   0 root         (0) root         (0)     2372 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     2362 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     2860 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/new.py
--rw-rw-rw-   0 root         (0) root         (0)     2366 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/restore.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/retirement.py
--rw-rw-rw-   0 root         (0) root         (0)     3307 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/snapshot.py
--rw-rw-rw-   0 root         (0) root         (0)     2246 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/vmdk.py
--rw-rw-rw-   0 root         (0) root         (0)     1614 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/service.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/shell.py
--rw-rw-rw-   0 root         (0) root         (0)     2325 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/status.py
--rw-rw-rw-   0 root         (0) root         (0)     6761 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/stor.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/token.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/upgrade.py
--rw-rw-rw-   0 root         (0) root         (0)     2775 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/vpn.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/rel_opts.py
--rw-rw-rw-   0 root         (0) root         (0)     2864 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/sstatus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.034016 vss-cli-2024.6.0.dev0/vss_cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    75203 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/utils/emoji.py
--rw-rw-rw-   0 root         (0) root         (0)     2929 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/utils/threading.py
--rw-rw-rw-   0 root         (0) root         (0)     4734 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/vss.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/vssconst.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.034016 vss-cli-2024.6.0.dev0/vss_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13950 2024-05-27 16:01:15.000000 vss-cli-2024.6.0.dev0/vss_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2476 2024-05-27 16:01:16.000000 vss-cli-2024.6.0.dev0/vss_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 16:01:15.000000 vss-cli-2024.6.0.dev0/vss_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-27 16:01:15.000000 vss-cli-2024.6.0.dev0/vss_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 16:01:15.000000 vss-cli-2024.6.0.dev0/vss_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      732 2024-05-27 16:01:16.000000 vss-cli-2024.6.0.dev0/vss_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-27 16:01:16.000000 vss-cli-2024.6.0.dev0/vss_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:57:30.729580 vss-cli-2024.6.0.dev4/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13950 2024-05-29 17:57:30.729580 vss-cli-2024.6.0.dev4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10991 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-29 17:57:30.733580 vss-cli-2024.6.0.dev4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3827 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:57:30.709580 vss-cli-2024.6.0.dev4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5569 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/tests/test_vss_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:57:30.713580 vss-cli-2024.6.0.dev4/vss_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19671 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/autocompletion.py
+-rw-rw-rw-   0 root         (0) root         (0)     7659 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev4/vss_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    67343 2024-05-29 17:56:49.000000 vss-cli-2024.6.0.dev4/vss_cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15583 2024-05-29 17:56:49.000000 vss-cli-2024.6.0.dev4/vss_cli/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:57:30.717580 vss-cli-2024.6.0.dev4/vss_cli/data/
+-rw-rw-rw-   0 root         (0) root         (0)     4500 2024-05-29 17:56:49.000000 vss-cli-2024.6.0.dev4/vss_cli/data/clib.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4288 2024-05-29 17:56:49.000000 vss-cli-2024.6.0.dev4/vss_cli/data/clone.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/data/config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/data/image.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2926 2024-05-29 17:56:49.000000 vss-cli-2024.6.0.dev4/vss_cli/data/shell.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2024-05-29 17:56:49.000000 vss-cli-2024.6.0.dev4/vss_cli/data/template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    25960 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev4/vss_cli/data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/hcio.py
+-rw-rw-rw-   0 root         (0) root         (0)    12512 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:57:30.721580 vss-cli-2024.6.0.dev4/vss_cli/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 17:57:25.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15976 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/completion.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2024-05-24 16:04:34.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:57:30.725580 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8906 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/callbacks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/contentlib.py
+-rw-rw-rw-   0 root         (0) root         (0)     2813 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3133 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/floppy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8680 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3287 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/iso.py
+-rw-rw-rw-   0 root         (0) root         (0)     3477 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/net.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/os.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/rel_args.py
+-rw-rw-rw-   0 root         (0) root         (0)     9604 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/rel_opts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3790 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/template.py
+-rw-rw-rw-   0 root         (0) root         (0)   150500 2024-05-24 16:04:34.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/vm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1907 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/vmdks.py
+-rw-rw-rw-   0 root         (0) root         (0)    10871 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/key.py
+-rw-rw-rw-   0 root         (0) root         (0)     3010 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4310 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/ovf.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/raw.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:57:30.725580 vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/change.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/export.py
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/new.py
+-rw-rw-rw-   0 root         (0) root         (0)     2366 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/restore.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/retirement.py
+-rw-rw-rw-   0 root         (0) root         (0)     3307 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/snapshot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2246 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/vmdk.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     2325 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/status.py
+-rw-rw-rw-   0 root         (0) root         (0)     6761 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/stor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/token.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/upgrade.py
+-rw-rw-rw-   0 root         (0) root         (0)     4507 2024-05-29 17:56:49.000000 vss-cli-2024.6.0.dev4/vss_cli/plugins/vpn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/rel_opts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/sstatus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:57:30.725580 vss-cli-2024.6.0.dev4/vss_cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    75203 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/utils/emoji.py
+-rw-rw-rw-   0 root         (0) root         (0)     2929 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/utils/threading.py
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/vss.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/vssconst.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev4/vss_cli/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:57:30.729580 vss-cli-2024.6.0.dev4/vss_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13950 2024-05-29 17:57:30.000000 vss-cli-2024.6.0.dev4/vss_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2476 2024-05-29 17:57:30.000000 vss-cli-2024.6.0.dev4/vss_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 17:57:30.000000 vss-cli-2024.6.0.dev4/vss_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-29 17:57:30.000000 vss-cli-2024.6.0.dev4/vss_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 17:57:30.000000 vss-cli-2024.6.0.dev4/vss_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      732 2024-05-29 17:57:30.000000 vss-cli-2024.6.0.dev4/vss_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 17:57:30.000000 vss-cli-2024.6.0.dev4/vss_cli.egg-info/top_level.txt
```

### Comparing `vss-cli-2024.6.0.dev0/LICENSE` & `vss-cli-2024.6.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/PKG-INFO` & `vss-cli-2024.6.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vss-cli
-Version: 2024.6.0.dev0
+Version: 2024.6.0.dev4
 Summary: ITS Private Cloud Command Line Interface
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.6.0-dev0.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.6.0-dev4.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/issues
 Project-URL: Documentation, https://eis.utoronto.ca/~vss/vss-cli/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
```

### Comparing `vss-cli-2024.6.0.dev0/README.md` & `vss-cli-2024.6.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/setup.cfg` & `vss-cli-2024.6.0.dev4/setup.cfg`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/setup.py` & `vss-cli-2024.6.0.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/tests/test_vss_cli.py` & `vss-cli-2024.6.0.dev4/tests/test_vss_cli.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/autocompletion.py` & `vss-cli-2024.6.0.dev4/vss_cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/cli.py` & `vss-cli-2024.6.0.dev4/vss_cli/cli.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/config.py` & `vss-cli-2024.6.0.dev4/vss_cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -586,39 +586,60 @@
     ):
         """Get token with MFA."""
         try:
             token = token or self.get_token(
                 self.username, self.password, self.totp
             )
         except VssError as ex:
-            if (
-                500 > ex.http_code > 399
-                and 'InvalidParameterValue: otp' in ex.message
-            ):
-                # try MFA Auth
-                try:
-                    _LOGGING.debug('Requesting a new timed one-time password')
-                    _ = self.request_totp(self.username, self.password)
-                except Exception as exc:
-                    _LOGGING.warning(f'Requesting totp: {exc}')
-                    pass
-                if spinner_cls is not None:
-                    spinner_cls.stop()
-                self.totp = click.prompt(
-                    'MFA enabled. Provide Timed One-Time Password'
-                )
-                if spinner_cls is not None:
-                    spinner_cls.start()
-                try:
-                    token = token or self.get_token(
-                        self.username, self.password, self.totp
+            if 500 > ex.http_code > 399:
+                if 'InvalidParameterValue: otp' in ex.message:
+                    # try MFA Auth
+                    try:
+                        _LOGGING.debug(
+                            'Requesting a new timed one-time password'
+                        )
+                        _ = self.request_totp(self.username, self.password)
+                    except Exception as exc:
+                        _LOGGING.warning(f'Requesting totp: {exc}')
+                        pass
+                    if spinner_cls is not None:
+                        spinner_cls.stop()
+                    self.totp = click.prompt(
+                        'MFA enabled. Provide Timed One-Time Password'
                     )
-                except Exception as exc:
-                    _LOGGING.warning(f'Could not generate new token: {exc}')
-                    raise exc
+                    if spinner_cls is not None:
+                        spinner_cls.start()
+                    try:
+                        token = token or self.get_token(
+                            self.username, self.password, self.totp
+                        )
+                    except Exception as exc:
+                        _LOGGING.warning(
+                            f'Could not generate new token: {exc}'
+                        )
+                        raise exc
+                elif 'TotpEnforcement: Must enable TOTP' in ex.message:
+                    if spinner_cls is not None:
+                        spinner_cls.stop()
+                    _LOGGING.error(ex)
+                    self.echo('')
+                    self.secho('Run ', file=sys.stderr, fg='green', nl=False)
+                    self.secho(
+                        'vss-cli account --no-load set mfa mk '
+                        '{EMAIL|AUTHENTICATOR|SMS}',
+                        file=sys.stderr,
+                        fg='red',
+                        nl=False,
+                    )
+                    self.secho(' to enable MFA.', file=sys.stderr, fg='green')
+                    if spinner_cls is not None:
+                        spinner_cls.start()
+                    sys.exit(1)
+                else:
+                    raise ex
             else:
                 raise ex
         return token
 
     def _create_endpoint_config(self, token: str = None) -> ConfigEndpoint:
         """Create endpoint configuration for a given token.
 
@@ -898,14 +919,35 @@
         self.init_vss_vpn(self.vpn_server)
         _LOGGING.debug(f'{self.totp=} {self.username=} -> {self.vpn_server=}')
         rv = super().enable_vss_vpn(
             user=self.username, password=self.password, otp=self.totp
         )
         return rv
 
+    def get_vss_vpn_status(self, **kwargs) -> Dict:
+        """Get status of VPN."""
+        self.init_vss_vpn(self.vpn_server)
+        _LOGGING.debug(f'{self.username=} -> {self.vpn_server=}')
+        rv = super().get_vss_vpn_status(
+            user=self.username,
+            password=self.password,
+        )
+        return rv
+
+    def monitor_vss_vpn(self, **kwargs):
+        """Monitor VPN."""
+        self.init_vss_vpn(self.vpn_server)
+        _LOGGING.debug(f'{self.username=} -> {self.vpn_server=}')
+        rv = super().monitor_vss_vpn(
+            user=self.username,
+            password=self.password,
+            stamp=kwargs.get('stamp'),
+        )
+        return rv
+
     def disable_vss_vpn(self, **kwargs):
         """Disable VPN."""
         self.init_vss_vpn(self.vpn_server)
         _LOGGING.debug(f'{self.username=} -> {self.vpn_server=}')
         rv = super().disable_vss_vpn(
             user=self.username,
             password=self.password,
```

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/const.py` & `vss-cli-2024.6.0.dev4/vss_cli/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Constants used by VSS CLI (vss-cli)."""
 import os
 from importlib import resources
 
 PACKAGE_NAME = "vss_cli"
 
-__version__ = "2024.6.0-dev0"
+__version__ = "2024.6.0-dev4"
 
 
 DEFAULT_TIMEOUT = 30
 DEFAULT_ENDPOINT = "https://cloud-api.eis.utoronto.ca"
 DEFAULT_ENDPOINT_NAME = "cloud-api"
 DEFAULT_S3_SERVER = "https://vskey-stor.eis.utoronto.ca"
 DEFAULT_VPN_SERVER = "https://vskey-vn.eis.utoronto.ca"
```

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/data/clib.yaml` & `vss-cli-2024.6.0.dev4/vss_cli/data/clib.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from CLib 2024.6.0-dev0             #
+#     VSS-CLI Spec from CLib 2024.6.0-dev4             #
 ####################################################
 built: clib               # Required: Do not remove.
 machine:
   item: ubuntu-22.04      # Required: Source content library id OVF.
   cpu: 1                  # Optional: CPU count (Default: 1).
   memory: 1               # Optional: Memory in GB (Default: 1GB).
   name: &name Vm-Name     # Required: Target virtual machine name.
```

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/data/clone.yaml` & `vss-cli-2024.6.0.dev4/vss_cli/data/clone.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from Clone 2024.6.0-dev0             #
+#     VSS-CLI Spec from Clone 2024.6.0-dev4             #
 ####################################################
 built: clone              # Required: Do not remove.
 machine:
   source: SourceVM        # Required: Can be a vm name or a vm id.
   name: &name Vm-Name     # Required: Target virtual machine name
   disks:                  # Optional: Disks (Default: source vm disk layout)
     - capacity_gb: 40     # Optional: Disk capacity in GB (Default: source vm disk capacity)
```

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/data/config.yaml` & `vss-cli-2024.6.0.dev4/vss_cli/data/config.yaml`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/data/image.yaml` & `vss-cli-2024.6.0.dev4/vss_cli/data/image.yaml`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/data/shell.yaml` & `vss-cli-2024.6.0.dev4/vss_cli/data/shell.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec shell VM 2024.6.0-dev0             #
+#     VSS-CLI Spec shell VM 2024.6.0-dev4             #
 ####################################################
 built: os_install         # Required: Do not remove.
 machine:
   name: Vm-Name            # Required: Target virtual machine name.
   os: ubuntu64Guest              # Required: Guest Operating System name or Id.
   cpu: 1                   # Optional: CPU count (Default: 1).
   memory: 1                # Optional: Memory in GB (Default: 1GB).
```

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/data/template.yaml` & `vss-cli-2024.6.0.dev4/vss_cli/data/template.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from Template 2024.6.0-dev0        #
+#     VSS-CLI Spec from Template 2024.6.0-dev4        #
 ####################################################
 built: template           # Required: Do not remove.
 machine:
   source: NixSource                # Required: Can be a vm name or a vm id.
   name: &name Vm-Name     # Required: Target virtual machine name
   folder: MyFolder       # Optional: Folder name, path or ID (Default: source vm folder)
   disks:                  # Optional: Disks (Default: source vm disk layout)
```

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/data_types.py` & `vss-cli-2024.6.0.dev4/vss_cli/data_types.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/hcio.py` & `vss-cli-2024.6.0.dev4/vss_cli/hcio.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/helper.py` & `vss-cli-2024.6.0.dev4/vss_cli/helper.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/account.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/account.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/completion.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/completion.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/callbacks.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/callbacks.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/contentlib.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/contentlib.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/domain.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/domain.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/floppy.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/floppy.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/folder.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/folder.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/helper.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/helper.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/image.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/image.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/inventory.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/inventory.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/iso.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/iso.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/net.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/net.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/os.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/os.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/rel_args.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/rel_args.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/rel_opts.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/rel_opts.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/template.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/template.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/vm.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/vm.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/vmdks.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/compute_plugins/vmdks.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/configure.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/configure.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/key.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/key.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/message.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/message.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/misc.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/misc.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/ovf.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/ovf.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/plugins.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/raw.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/raw.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/request.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/request.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/change.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/change.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/export.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/export.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/folder.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/folder.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/image.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/image.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/inventory.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/inventory.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/new.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/new.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/restore.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/restore.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/retirement.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/retirement.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/snapshot.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/snapshot.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/vmdk.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/request_plugins/vmdk.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/service.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/service.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/shell.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/status.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/status.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/stor.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/stor.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/token.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/token.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/upgrade.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/upgrade.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/plugins/vpn.py` & `vss-cli-2024.6.0.dev4/vss_cli/plugins/vpn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """VPN related commands."""
 import logging
+import sys
+from datetime import datetime, timedelta, timezone
 
 import click
+import pytz
 
+from vss_cli import const
 from vss_cli.cli import pass_context
 from vss_cli.config import Configuration
 from vss_cli.utils.emoji import EMOJI_UNICODE
 
 _LOGGING = logging.getLogger(__name__)
 ej_rkt = EMOJI_UNICODE.get(':rocket:')
 ej_warn = EMOJI_UNICODE.get(':alien:')
@@ -32,20 +36,34 @@
 @click.option(
     '--otp', '-o', prompt='Provide Timed One-Time Password', help='OTP string'
 )
 @pass_context
 def gateway_on(ctx: Configuration, otp):
     """Enable vpn via mfa."""
     click.echo(f'Attempting to enable VPN GW: {ctx.vpn_server}')
+    status = ctx.get_vss_vpn_status()
+    _LOGGING.debug(f'{status=}')
+    if status:
+        if not status.get('usages'):
+            _LOGGING.error(
+                f'VPN GW {ctx.vpn_server} has MFA disabled.'
+                f'Enable VPN GW MFA via {ctx.vss_vpn_otp_svc_endpoint}'
+            )
+            sys.exit(1)
+        _LOGGING.info(
+            f'VPN GW {ctx.vpn_server} MFA enabled on: '
+            f'{status["usages"]} via {status["method"]}'
+        )
     with ctx.spinner(disable=ctx.debug) as spinner_cls:
         ctx.totp = otp
         try:
             rv = ctx.enable_vss_vpn()
-            _LOGGING.debug(f'{rv=}')
+            _LOGGING.debug(f'{rv}')
             spinner_cls.stop()
+            _LOGGING.warning(rv['log'])
             click.echo(
                 f'Successfully enabled. '
                 f'Ready to connect to {ctx.vpn_server} {ej_rkt}'
             )
             spinner_cls.start()
         except Exception as e:
             _LOGGING.error(f'An error occurred {ej_warn}: {e}')
@@ -55,40 +73,73 @@
 @pass_context
 def gateway_off(ctx: Configuration):
     """Disable vpn via mfa."""
     click.echo(f'Attempting to disable VPN GW: {ctx.vpn_server}')
     with ctx.spinner(disable=ctx.debug) as spinner_cls:
         try:
             rv = ctx.disable_vss_vpn()
-            _LOGGING.debug(f'{rv=}')
+            _LOGGING.debug(f'{rv}')
             spinner_cls.stop()
             click.echo('Successfully disabled VPN GW. ')
             spinner_cls.start()
         except Exception as e:
             _LOGGING.error(f'An error occurred {ej_warn}: {e}')
 
 
+@gateway.command('log', short_help='get vpn logs')
+@click.option(
+    '-t',
+    '--timestamp',
+    type=click.DateTime(formats=[const.DEFAULT_DATETIME_FMT]),
+    default=datetime.strftime(
+        datetime.now() - timedelta(hours=1), const.DEFAULT_DATETIME_FMT
+    ),
+    required=False,
+    show_default=True,
+    help='Timestamp to retrieve logs from.',
+)
+@pass_context
+def gateway_log(ctx: Configuration, timestamp):
+    """Get logs from VPN GW."""
+    with ctx.spinner(disable=ctx.debug):
+        try:
+            local_dt = pytz.timezone('America/Toronto').localize(
+                timestamp, is_dst=None
+            )
+            _LOGGING.debug(f'{local_dt=}')
+            utc_dt = local_dt.astimezone(pytz.utc)
+            _LOGGING.debug(f'{utc_dt=}')
+            rv = ctx.monitor_vss_vpn(stamp=utc_dt)
+            _LOGGING.debug(f'{rv}')
+        except Exception as e:
+            _LOGGING.error(f'An error occurred {ej_warn}: {e}')
+            sys.exit(1)
+        # iterate through log
+        for log in rv['log']:
+            click.echo(log)
+
+
 @cli.command('la', short_help='launch ui')
 @click.argument(
     'ui_type',
     type=click.Choice(
         ['ui', 'otp-svc', 'otp-enable', 'otp-disable', 'otp-monitor']
     ),
     required=True,
     default='ui',
 )
 @pass_context
 def stor_launch(ctx: Configuration, ui_type):
     """Launch web ui."""
-    cfg = ctx.get_vss_vpn_cfg()
+    _ = ctx.init_vss_vpn(ctx.vpn_server)
     lookup = {
-        'ui': cfg['endpoint'],
-        'otp-svc': cfg['otp_svc'],
-        'otp-enable': cfg['otp_enable'],
-        'otp-disable': cfg['otp_disable'],
-        'otp-monitor': cfg['otp_monitor'],
+        'ui': ctx.vss_vpn_endpoint,
+        'otp-svc': ctx.vss_vpn_otp_svc_endpoint,
+        'otp-enable': ctx.vss_vpn_otp_enable_endpoint,
+        'otp-disable': ctx.vss_vpn_otp_disable_endpoint,
+        'otp-monitor': ctx.vss_vpn_otp_monitor_endpoint,
     }
     url = lookup[ui_type]
     click.echo(f'Launching {EMOJI_UNICODE[":globe_showing_Americas:"]}: {url}')
     click.launch(
         url,
     )
```

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/rel_opts.py` & `vss-cli-2024.6.0.dev4/vss_cli/rel_opts.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/sstatus.py` & `vss-cli-2024.6.0.dev4/vss_cli/sstatus.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/utils/emoji.py` & `vss-cli-2024.6.0.dev4/vss_cli/utils/emoji.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/utils/threading.py` & `vss-cli-2024.6.0.dev4/vss_cli/utils/threading.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/validators.py` & `vss-cli-2024.6.0.dev4/vss_cli/validators.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/vss.py` & `vss-cli-2024.6.0.dev4/vss_cli/vss.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli/yaml.py` & `vss-cli-2024.6.0.dev4/vss_cli/yaml.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli.egg-info/PKG-INFO` & `vss-cli-2024.6.0.dev4/vss_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vss-cli
-Version: 2024.6.0.dev0
+Version: 2024.6.0.dev4
 Summary: ITS Private Cloud Command Line Interface
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.6.0-dev0.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.6.0-dev4.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/issues
 Project-URL: Documentation, https://eis.utoronto.ca/~vss/vss-cli/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
```

### Comparing `vss-cli-2024.6.0.dev0/vss_cli.egg-info/SOURCES.txt` & `vss-cli-2024.6.0.dev4/vss_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.6.0.dev0/vss_cli.egg-info/requires.txt` & `vss-cli-2024.6.0.dev4/vss_cli.egg-info/requires.txt`

 * *Files identical despite different names*

