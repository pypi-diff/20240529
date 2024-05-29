# Comparing `tmp/volatility3-2.5.2.tar.gz` & `tmp/volatility3-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/volatility3-2.5.2.tar", last modified: Wed Jan 31 21:21:38 2024, max compression
+gzip compressed data, was "dist/volatility3-2.7.0.tar", last modified: Wed May 29 19:24:25 2024, max compression
```

## Comparing `volatility3-2.5.2.tar` & `volatility3-2.7.0.tar`

### file list

```diff
@@ -1,367 +1,380 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-01-31 21:21:33.000000 volatility3-2.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-31 21:21:33.000000 volatility3-2.5.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-01-31 21:21:33.000000 volatility3-2.5.2/.style.yapf
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-01-31 21:21:33.000000 volatility3-2.5.2/API_CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-01-31 21:21:33.000000 volatility3-2.5.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-01-31 21:21:33.000000 volatility3-2.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-31 21:21:33.000000 volatility3-2.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-01-31 21:21:38.000000 volatility3-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-01-31 21:21:33.000000 volatility3-2.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   107414 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/_static/vol.png
--rw-r--r--   0 runner    (1001) docker     (127)    12683 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/basics.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20892 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/complex-plugin.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/getting-started-linux-tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/getting-started-mac-tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/getting-started-windows-tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17983 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/simple-plugin.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/symbol-tables.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14020 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/using-as-a-library.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/vol-cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/vol2to3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-01-31 21:21:33.000000 volatility3-2.5.2/doc/source/volshell.rst
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-31 21:21:33.000000 volatility3-2.5.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-31 21:21:33.000000 volatility3-2.5.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-31 21:21:33.000000 volatility3-2.5.2/requirements-minimal.txt
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-31 21:21:33.000000 volatility3-2.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 21:21:38.000000 volatility3-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-01-31 21:21:33.000000 volatility3-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-01-31 21:21:33.000000 volatility3-2.5.2/test/test_volatility.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      290 2024-01-31 21:21:33.000000 volatility3-2.5.2/vol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-01-31 21:21:33.000000 volatility3-2.5.2/vol.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    30867 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16346 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/cli/text_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/cli/volargparse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/cli/volshell/
--rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/cli/volshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22614 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/cli/volshell/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/cli/volshell/linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/cli/volshell/mac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/cli/volshell/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/automagic/
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/automagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/automagic/construct_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/automagic/linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     9990 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/automagic/mac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/automagic/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/automagic/pdbscan.py
--rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/automagic/stacker.py
--rw-r--r--   0 runner    (1001) docker     (127)    21689 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/automagic/symbol_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/automagic/symbol_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/automagic/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27291 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/configuration/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/constants/linux/
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/constants/linux/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/constants/windows/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/constants/windows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/interfaces/automagic.py
--rw-r--r--   0 runner    (1001) docker     (127)    32153 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/interfaces/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13139 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/interfaces/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29149 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/interfaces/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15109 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/interfaces/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/interfaces/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/interfaces/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/interfaces/symbols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/avml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/cloudstorage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/layers/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/crash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/elf.py
--rw-r--r--   0 runner    (1001) docker     (127)    18781 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/intel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/leechcore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/lime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/msf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/physical.py
--rw-r--r--   0 runner    (1001) docker     (127)    21705 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/qemu.py
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/layers/scanners/
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/scanners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/scanners/multiregexp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/segmented.py
--rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/vmware.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/layers/xen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/objects/
--rw-r--r--   0 runner    (1001) docker     (127)    38335 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/objects/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/objects/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/banners.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/configwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/frameworkinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/isfinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/layerwriter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/check_afinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/check_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/check_idt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/check_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/check_syscall.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/elfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/envars.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/iomem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/keyboard_notifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16867 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/kmsg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/lsmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/lsof.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/malfind.py
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/mountinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/psaux.py
--rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/pslist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/psscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/pstree.py
--rw-r--r--   0 runner    (1001) docker     (127)    23947 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/sockstat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/tty_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/linux/vmayarascan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/check_syscall.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/check_sysctl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/check_trap_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/ifconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/kauth_listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/kauth_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/kevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/list_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/lsmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/lsof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/malfind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/netstat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/proc_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/psaux.py
--rw-r--r--   0 runner    (1001) docker     (127)    12273 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/pslist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/pstree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/socket_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/timers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/trustedbsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/mac/vfsevents.py
--rw-r--r--   0 runner    (1001) docker     (127)    12737 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/timeliner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/bigpools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/cachedump.py
--rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/crashinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/devicetree.py
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/dlllist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/driverirp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/drivermodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/driverscan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14607 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/dumpfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/envars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/filescan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/getservicesids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/getsids.py
--rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/hashdump.py
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/joblinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/ldrmodules.py
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/lsadump.py
--rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/malfind.py
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/mbrscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/mftscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/modscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8595 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/mutantscan.py
--rw-r--r--   0 runner    (1001) docker     (127)    22464 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/netscan.py
--rw-r--r--   0 runner    (1001) docker     (127)    29324 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/netstat.py
--rw-r--r--   0 runner    (1001) docker     (127)    19513 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/poolscanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/privileges.py
--rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/pslist.py
--rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/psscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/pstree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/registry/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13749 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/registry/hivelist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/registry/hivescan.py
--rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/registry/printkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/registry/userassist.json
--rw-r--r--   0 runner    (1001) docker     (127)    13895 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/registry/userassist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    44438 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/sids_and_privileges.json
--rw-r--r--   0 runner    (1001) docker     (127)    24892 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/skeleton_key_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/ssdt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/svcscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/symlinkscan.py
--rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/vadinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/vadwalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/vadyarascan.py
--rw-r--r--   0 runner    (1001) docker     (127)    10694 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/verinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/windows/virtmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/plugins/yarascan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)    17644 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/renderers/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/renderers/format_hints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/symbols/
--rw-r--r--   0 runner    (1001) docker     (127)    12502 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/symbols/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/generic/qemu.json
--rw-r--r--   0 runner    (1001) docker     (127)    34330 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/intermed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/symbols/linux/
--rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/linux/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/linux/bash32.json
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/linux/bash64.json
--rw-r--r--   0 runner    (1001) docker     (127)    20166 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/linux/elf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/symbols/linux/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)    57515 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/linux/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/linux/extensions/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/linux/extensions/elf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/linux/xen.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/symbols/mac/
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/mac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/symbols/mac/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)    18156 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/mac/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/native.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3321 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/bigpools/
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/bigpools/bigpools-vista-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/bigpools/bigpools-vista-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/bigpools/bigpools-win10-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/bigpools/bigpools-win10-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/bigpools/bigpools-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/bigpools/bigpools-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/callbacks-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/callbacks-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/crash.json
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/crash64.json
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/crash_common.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/
--rwxr-xr-x   0 runner    (1001) docker     (127)    51146 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/crash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/kdbg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/mbr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/mft.py
--rw-r--r--   0 runner    (1001) docker     (127)     9429 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/pe.py
--rw-r--r--   0 runner    (1001) docker     (127)    18187 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/services.py
--rw-r--r--   0 runner    (1001) docker     (127)    34527 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/kdbg.json
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/kerb_ecrypt.json
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/mbr.json
--rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/mft.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/
--rw-r--r--   0 runner    (1001) docker     (127)    13878 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-vista-sp12-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)    13878 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-vista-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-vista-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)    18938 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-10240-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-10586-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)    13869 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-14393-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)    15056 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-15063-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)    18936 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-15063-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)    15583 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-16299-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)    15583 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-17134-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)    13869 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-17134-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)    15583 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-17763-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)    15583 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-18362-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-18363-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-19041-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)     9778 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-19041-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)    18953 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win7-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)    18934 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win7-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)    18953 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win8-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win8-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)    18955 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win81-19935-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)    18953 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win81-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win81-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)    40049 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/pdb.json
--rw-r--r--   0 runner    (1001) docker     (127)    44458 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/pdbconv.py
--rw-r--r--   0 runner    (1001) docker     (127)    22162 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/pdbutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    21124 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/pe.json
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/poolheader-x64-win7.json
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/poolheader-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/poolheader-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/registry.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/services/
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-vista-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-vista-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-win10-15063-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-win10-15063-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-win10-16299-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-win10-16299-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-win8-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-win8-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-xp-2003-x64.json
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-xp-x86.json
--rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/windows/versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/framework/symbols/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/plugins/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/plugins/linux/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/plugins/mac/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/plugins/mac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/plugins/windows/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/plugins/windows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/plugins/windows/registry/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/plugins/windows/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/plugins/windows/registry/certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/plugins/windows/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/schemas/schema-0.1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/schemas/schema-2.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/schemas/schema-2.1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/schemas/schema-4.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/schemas/schema-4.1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/schemas/schema-6.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/schemas/schema-6.1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    10535 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/schemas/schema-6.2.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3/symbols/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-01-31 21:21:33.000000 volatility3-2.5.2/volatility3/symbols/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-01-31 21:21:37.000000 volatility3-2.5.2/volatility3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14959 2024-01-31 21:21:38.000000 volatility3-2.5.2/volatility3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 21:21:37.000000 volatility3-2.5.2/volatility3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-31 21:21:37.000000 volatility3-2.5.2/volatility3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-31 21:21:37.000000 volatility3-2.5.2/volatility3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-31 21:21:37.000000 volatility3-2.5.2/volatility3.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-01-31 21:21:33.000000 volatility3-2.5.2/volshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-01-31 21:21:33.000000 volatility3-2.5.2/volshell.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-29 19:24:19.000000 volatility3-2.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-29 19:24:19.000000 volatility3-2.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-29 19:24:19.000000 volatility3-2.7.0/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-29 19:24:19.000000 volatility3-2.7.0/API_CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-29 19:24:19.000000 volatility3-2.7.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-29 19:24:19.000000 volatility3-2.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-29 19:24:19.000000 volatility3-2.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-29 19:24:25.000000 volatility3-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-05-29 19:24:19.000000 volatility3-2.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   107414 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/_static/vol.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12683 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20892 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/complex-plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/getting-started-linux-tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/getting-started-mac-tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/getting-started-windows-tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17983 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/simple-plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/symbol-tables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14020 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/using-as-a-library.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/vol-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/vol2to3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-05-29 19:24:19.000000 volatility3-2.7.0/doc/source/volshell.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-29 19:24:19.000000 volatility3-2.7.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-29 19:24:19.000000 volatility3-2.7.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-29 19:24:19.000000 volatility3-2.7.0/requirements-minimal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-29 19:24:19.000000 volatility3-2.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:24:25.000000 volatility3-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-29 19:24:19.000000 volatility3-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    14040 2024-05-29 19:24:19.000000 volatility3-2.7.0/test/test_volatility.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      290 2024-05-29 19:24:19.000000 volatility3-2.7.0/vol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-05-29 19:24:19.000000 volatility3-2.7.0/vol.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    33901 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/cli/text_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16628 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/cli/text_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/cli/volargparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/cli/volshell/
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/cli/volshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22614 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/cli/volshell/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/cli/volshell/linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/cli/volshell/mac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/cli/volshell/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/automagic/
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/automagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/automagic/construct_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/automagic/linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9990 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/automagic/mac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/automagic/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/automagic/pdbscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/automagic/stacker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21689 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/automagic/symbol_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/automagic/symbol_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/automagic/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27291 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/configuration/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/constants/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/constants/linux/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/constants/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/constants/windows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/interfaces/automagic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32153 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/interfaces/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13179 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/interfaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29149 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/interfaces/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15109 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/interfaces/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/interfaces/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/interfaces/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/interfaces/symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/avml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/cloudstorage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/layers/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/crash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/intel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/leechcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/lime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/msf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/physical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21705 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/qemu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/layers/scanners/
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/scanners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/scanners/multiregexp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/segmented.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/vmware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/layers/xen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)    38335 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/objects/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/objects/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/banners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/configwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/frameworkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/isfinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/layerwriter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/check_afinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/check_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/check_idt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/check_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/check_syscall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/elfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/envars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/iomem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/keyboard_notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20521 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/kmsg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/library_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/lsmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/lsof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/malfind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/mountinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/psaux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/pslist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/psscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/pstree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23949 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/sockstat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/tty_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/linux/vmayarascan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/check_syscall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/check_sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/check_trap_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/dmesg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/ifconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/kauth_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/kauth_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/kevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/list_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/lsmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/lsof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/malfind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/netstat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/proc_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/psaux.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12273 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/pslist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/pstree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/socket_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/timers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/trustedbsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/mac/vfsevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12737 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/timeliner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/bigpools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/cachedump.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/crashinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/devicetree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/dlllist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/driverirp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/drivermodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/driverscan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16066 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/dumpfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/envars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/filescan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/getservicesids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/getsids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16482 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/hashdump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/iat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/joblinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/ldrmodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/lsadump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/malfind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/mbrscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13941 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/mftscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/modscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8595 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/mutantscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22464 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/netscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29324 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/netstat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20397 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/poolscanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/privileges.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/pslist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/psscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/pstree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13749 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/registry/hivelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/registry/hivescan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/registry/printkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/registry/userassist.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13895 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/registry/userassist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44438 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/sids_and_privileges.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24892 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/skeleton_key_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/ssdt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/svcscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/symlinkscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/thrdscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/truecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/vadinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/vadwalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/vadyarascan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10694 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/verinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/windows/virtmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/plugins/yarascan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)    17644 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/renderers/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/renderers/format_hints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/symbols/
+-rw-r--r--   0 runner    (1001) docker     (127)    13966 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/symbols/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/generic/qemu.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34689 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/intermed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/symbols/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/linux/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/linux/bash32.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/linux/bash64.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23687 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/linux/elf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/symbols/linux/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)    62158 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/linux/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/linux/extensions/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15024 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/linux/extensions/elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/linux/xen.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/symbols/mac/
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/mac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/symbols/mac/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)    18322 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/mac/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/native.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3321 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/bigpools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/bigpools/bigpools-vista-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/bigpools/bigpools-vista-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/bigpools/bigpools-win10-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/bigpools/bigpools-win10-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/bigpools/bigpools-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/bigpools/bigpools-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/callbacks-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/callbacks-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/crash.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/crash64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/crash_common.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    52421 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/crash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/kdbg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/mbr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/mft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9429 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/pe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18187 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34527 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/kdbg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/kerb_ecrypt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/mbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/mft.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/
+-rw-r--r--   0 runner    (1001) docker     (127)    13878 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-vista-sp12-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13878 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-vista-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-vista-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18938 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-10240-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-10586-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13869 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-14393-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15056 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-15063-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18936 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-15063-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15583 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-16299-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15583 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-17134-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13869 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-17134-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15583 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-17763-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15583 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-18362-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-18363-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-19041-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9778 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-19041-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18953 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win7-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18934 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win7-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18953 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win8-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win8-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18955 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win81-19935-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18953 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win81-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win81-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40049 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/pdb.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44458 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/pdbconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22162 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/pdbutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21124 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/pe.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/poolheader-x64-win7.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/poolheader-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/poolheader-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/registry.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-vista-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-vista-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-15063-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-15063-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-16299-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-16299-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-17763-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-18362-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-18362-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-19041-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-19041-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-25398-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win8-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win8-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-xp-2003-x64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-xp-x86.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/windows/versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/framework/symbols/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/plugins/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/plugins/linux/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/plugins/mac/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/plugins/mac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/plugins/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/plugins/windows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/plugins/windows/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/plugins/windows/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/plugins/windows/registry/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/plugins/windows/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/schemas/schema-0.1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/schemas/schema-2.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/schemas/schema-2.1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/schemas/schema-4.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/schemas/schema-4.1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/schemas/schema-6.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/schemas/schema-6.1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10535 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/schemas/schema-6.2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/schemas/schema-6.3.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3/symbols/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-29 19:24:19.000000 volatility3-2.7.0/volatility3/symbols/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15731 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 19:24:25.000000 volatility3-2.7.0/volatility3.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-05-29 19:24:19.000000 volatility3-2.7.0/volshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-29 19:24:19.000000 volatility3-2.7.0/volshell.spec
```

### Comparing `volatility3-2.5.2/.gitignore` & `volatility3-2.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/.readthedocs.yml` & `volatility3-2.7.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/.style.yapf` & `volatility3-2.7.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/API_CHANGES.md` & `volatility3-2.7.0/API_CHANGES.md`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/CITATION.cff` & `volatility3-2.7.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/LICENSE.txt` & `volatility3-2.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/PKG-INFO` & `volatility3-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volatility3
-Version: 2.5.2
+Version: 2.7.0
 Summary: Memory forensics framework
 Home-page: https://github.com/volatilityfoundation/volatility3/
 Author: Volatility Foundation
 Author-email: volatility@volatilityfoundation.org
 License: VSL
 Project-URL: Bug Tracker, https://github.com/volatilityfoundation/volatility3/issues
 Project-URL: Documentation, https://volatility3.readthedocs.io/
```

### Comparing `volatility3-2.5.2/README.md` & `volatility3-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/Makefile` & `volatility3-2.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/make.bat` & `volatility3-2.7.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/_static/favicon.ico` & `volatility3-2.7.0/doc/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/_static/vol.png` & `volatility3-2.7.0/doc/source/_static/vol.png`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/basics.rst` & `volatility3-2.7.0/doc/source/basics.rst`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/complex-plugin.rst` & `volatility3-2.7.0/doc/source/complex-plugin.rst`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/conf.py` & `volatility3-2.7.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/getting-started-linux-tutorial.rst` & `volatility3-2.7.0/doc/source/getting-started-linux-tutorial.rst`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/getting-started-mac-tutorial.rst` & `volatility3-2.7.0/doc/source/getting-started-mac-tutorial.rst`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/getting-started-windows-tutorial.rst` & `volatility3-2.7.0/doc/source/getting-started-windows-tutorial.rst`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/glossary.rst` & `volatility3-2.7.0/doc/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/index.rst` & `volatility3-2.7.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/simple-plugin.rst` & `volatility3-2.7.0/doc/source/simple-plugin.rst`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/symbol-tables.rst` & `volatility3-2.7.0/doc/source/symbol-tables.rst`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/using-as-a-library.rst` & `volatility3-2.7.0/doc/source/using-as-a-library.rst`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/vol-cli.rst` & `volatility3-2.7.0/doc/source/vol-cli.rst`

 * *Files 8% similar despite different names*

```diff
@@ -139,7 +139,22 @@
 **<plugin>**
     The name of the plugin to execute (these are usually categorized by
     the operating system, such as `windows.pslist.PsList`).  Any substring
     that uniquely matches the desired plugin name can be used.  As such
     `hivescan` would match `windows.registry.hivescan.HiveScan`, but
     `pslist` is ambiguous because it could match `windows.pslist` or
     `linux.pslist`.
+
+Overriding options
+------------------
+
+The default values for the command line interface are defined by constants within the code,
+but can be overridden by creating a JSON file (`%APPDATA%/volatility3/vol.json` for Windows
+systems, or `~/.config/volatility3/vol.json` or `volshell.json` for all others).
+
+The format of this file is a JSON dictionary, containing the options above and their value.
+It should be noted that the ordering is (`<` means is overridden by):
+
+`in-built default value < config file value < command line parameter`
+
+It should also be noted that boolean flags (such as `offline`) that are overridden as true will
+not be unset by not specifying the command line flag.
```

### Comparing `volatility3-2.5.2/doc/source/vol2to3.rst` & `volatility3-2.7.0/doc/source/vol2to3.rst`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/doc/source/volshell.rst` & `volatility3-2.7.0/doc/source/volshell.rst`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/requirements-dev.txt` & `volatility3-2.7.0/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# The following packages are required for core functionality.
-pefile>=2023.2.7
+# Include the minimal requirements
+-r requirements-minimal.txt
 
 # The following packages are optional.
 # If certain packages are not necessary, place a comment (#) at the start of the line.
 
 # This is required for the yara plugins
 yara-python>=3.8.0
 
 # This is required for several plugins that perform malware analysis and disassemble code.
 # It can also improve accuracy of Windows 8 and later memory samples.
 capstone>=3.0.5
 
 # This is required by plugins that decrypt passwords, password hashes, etc.
 pycryptodome
 
-# This can improve error messages regarding improperly configured ISF files,
-# but is only recommended for development
-jsonschema>=2.3.0
-
 # This is required for memory acquisition via leechcore/pcileech.
 leechcorepyc>=2.4.0
+
+# This is required for memory analysis on a Amazon/MinIO S3 and Google Cloud object storage
+gcsfs>=2023.1.0
+s3fs>=2023.1.0
```

### Comparing `volatility3-2.5.2/setup.py` & `volatility3-2.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/test/test_volatility.py` & `volatility3-2.7.0/test/test_volatility.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 
 #
 # IMPORTS
 #
 
 import os
+import re
 import subprocess
 import sys
 import shutil
 import tempfile
 import hashlib
 import ntpath
 import json
@@ -185,14 +186,24 @@
     rc, out, err = runvol_plugin("windows.svcscan.SvcScan", image, volatility, python)
 
     assert out.find(b"Microsoft ACPI Driver") != -1
     assert out.count(b"\n") > 250
     assert rc == 0
 
 
+def test_windows_thrdscan(image, volatility, python):
+    rc, out, err = runvol_plugin("windows.thrdscan.ThrdScan", image, volatility, python)
+    # find pid 4 (of system process) which starts with lowest tids
+    assert out.find(b"\t4\t8") != -1
+    assert out.find(b"\t4\t12") != -1
+    assert out.find(b"\t4\t16") != -1
+    #assert out.find(b"this raieses AssertionError") != -1
+    assert rc == 0
+
+
 def test_windows_privileges(image, volatility, python):
     rc, out, err = runvol_plugin(
         "windows.privileges.Privs", image, volatility, python, pluginargs=["--pid", "4"]
     )
 
     assert out.find(b"SeCreateTokenPrivilege") != -1
     assert out.find(b"SeCreateGlobalPrivilege") != -1
@@ -327,14 +338,40 @@
     out = out.lower()
 
     assert out.find(b"__kernel__") != -1
     assert out.count(b"\n") >= 5
     assert rc == 0
 
 
+def test_linux_library_list(image, volatility, python):
+    rc, out, err = runvol_plugin(
+        "linux.library_list.LibraryList", image, volatility, python
+    )
+
+    assert re.search(
+        rb"NetworkManager\s2363\s0x7f52cdda0000\s/lib/x86_64-linux-gnu/libnss_files.so.2",
+        out,
+    )
+    assert re.search(
+        rb"gnome-settings-\s3807\s0x7f7e660b5000\s/lib/x86_64-linux-gnu/libbz2.so.1.0",
+        out,
+    )
+    assert re.search(
+        rb"gdu-notificatio\s3878\s0x7f25ce33e000\s/usr/lib/x86_64-linux-gnu/libXau.so.6",
+        out,
+    )
+    assert re.search(
+        rb"bash\s8600\s0x7fe78a85f000\s/lib/x86_64-linux-gnu/libnss_files.so.2",
+        out,
+    )
+
+    assert out.count(b"\n") >= 2677
+    assert rc == 0
+
+
 # MAC
 
 
 def test_mac_pslist(image, volatility, python):
     rc, out, err = runvol_plugin("mac.pslist.PsList", image, volatility, python)
     out = out.lower()
```

### Comparing `volatility3-2.5.2/vol.spec` & `volatility3-2.7.0/vol.spec`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/__init__.py` & `volatility3-2.7.0/volatility3/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/cli/__init__.py` & `volatility3-2.7.0/volatility3/cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 import io
 import json
 import logging
 import os
 import sys
 import tempfile
 import traceback
-from typing import Any, Dict, Type, Union
+from typing import Any, Dict, List, Tuple, Type, Union
 from urllib import parse, request
 
+from volatility3.cli import text_filter
 import volatility3.plugins
 import volatility3.symbols
 from volatility3 import framework
 from volatility3.cli import text_renderer, volargparse
 from volatility3.framework import (
     automagic,
     configuration,
@@ -101,14 +102,17 @@
         renderers = dict(
             [
                 (x.name.lower(), x)
                 for x in framework.class_subclasses(text_renderer.CLIRenderer)
             ]
         )
 
+        # Load up system defaults
+        delayed_logs, default_config = self.load_system_defaults("vol.json")
+
         parser = volargparse.HelpfulArgParser(
             add_help=False,
             prog=self.CLI_NAME,
             description="An open-source memory forensics framework",
         )
         parser.add_argument(
             "-h",
@@ -226,54 +230,69 @@
         )
         parser.add_argument(
             "--offline",
             help="Do not search online for additional JSON files",
             default=False,
             action="store_true",
         )
+        parser.add_argument(
+            "--filters",
+            help="List of filters to apply to the output (in the form of [+-]columname,pattern[!])",
+            default=[],
+            action="append",
+        )
+
+        parser.set_defaults(**default_config)
 
         # We have to filter out help, otherwise parse_known_args will trigger the help message before having
         # processed the plugin choice or had the plugin subparser added.
         known_args = [arg for arg in sys.argv if arg != "--help" and arg != "-h"]
         partial_args, _ = parser.parse_known_args(known_args)
 
         banner_output = sys.stdout
         if renderers[partial_args.renderer].structured_output:
             banner_output = sys.stderr
         banner_output.write(f"Volatility 3 Framework {constants.PACKAGE_VERSION}\n")
 
-        if partial_args.plugin_dirs:
-            volatility3.plugins.__path__ = [
-                os.path.abspath(p) for p in partial_args.plugin_dirs.split(";")
-            ] + constants.PLUGINS_PATH
-
-        if partial_args.symbol_dirs:
-            volatility3.symbols.__path__ = [
-                os.path.abspath(p) for p in partial_args.symbol_dirs.split(";")
-            ] + constants.SYMBOL_BASEPATHS
-
-        if partial_args.cache_path:
-            constants.CACHE_PATH = partial_args.cache_path
-
+        ### Start up logging
         if partial_args.log:
             file_logger = logging.FileHandler(partial_args.log)
             file_logger.setLevel(1)
             file_formatter = logging.Formatter(
                 datefmt="%y-%m-%d %H:%M:%S",
                 fmt="%(asctime)s %(name)-12s %(levelname)-8s %(message)s",
             )
             file_logger.setFormatter(file_formatter)
             rootlog.addHandler(file_logger)
             vollog.info("Logging started")
+
+        self.order_extra_verbose_levels()
         if partial_args.verbosity < 3:
             if partial_args.verbosity < 1:
                 sys.tracebacklimit = None
-            console.setLevel(30 - (partial_args.verbosity * 10))
+            console.setLevel(logging.WARNING - (partial_args.verbosity * 10))
         else:
-            console.setLevel(10 - (partial_args.verbosity - 2))
+            console.setLevel(logging.DEBUG - (partial_args.verbosity - 2))
+
+        for level, msg in delayed_logs:
+            vollog.log(level, msg)
+
+        ### Alter constants if necessary
+        if partial_args.plugin_dirs:
+            volatility3.plugins.__path__ = [
+                os.path.abspath(p) for p in partial_args.plugin_dirs.split(";")
+            ] + constants.PLUGINS_PATH
+
+        if partial_args.symbol_dirs:
+            volatility3.symbols.__path__ = [
+                os.path.abspath(p) for p in partial_args.symbol_dirs.split(";")
+            ] + constants.SYMBOL_BASEPATHS
+
+        if partial_args.cache_path:
+            constants.CACHE_PATH = partial_args.cache_path
 
         vollog.info(f"Volatility plugins path: {volatility3.plugins.__path__}")
         vollog.info(f"Volatility symbols path: {volatility3.symbols.__path__}")
 
         # Set the PARALLELISM
         if partial_args.parallelism == "processes":
             constants.PARALLELISM = constants.Parallelism.Multiprocessing
@@ -440,15 +459,18 @@
                 1,
                 f"Unable to validate the plugin requirements: {[x for x in excp.unsatisfied]}\n",
             )
 
         try:
             # Construct and run the plugin
             if constructed:
-                renderers[args.renderer]().render(constructed.run())
+                grid = constructed.run()
+                renderer = renderers[args.renderer]()
+                renderer.filter = text_filter.CLIFilter(grid, args.filters)
+                renderer.render(grid)
         except exceptions.VolatilityException as excp:
             self.process_exceptions(excp)
 
     @classmethod
     def location_from_file(cls, filename: str) -> str:
         """Returns the URL location from a file parameter (which may be a URL)
 
@@ -459,14 +481,58 @@
             The URL for the location of the file
         """
         vollog.debug(
             f"{__name__}.location_from_file has been deprecated and moved to requirements.URIRequirement.location_from_file"
         )
         return requirements.URIRequirement.location_from_file(filename)
 
+    def load_system_defaults(
+        self, filename: str
+    ) -> Tuple[List[Tuple[int, str]], Dict[str, Any]]:
+        """Modify the main configuration based on the default configuration override"""
+        # Build the config path
+        default_config_path = os.path.join(
+            os.path.expanduser("~"), ".config", "volatility3", filename
+        )
+        if sys.platform == "win32":
+            default_config_path = os.path.join(
+                os.environ.get("APPDATA", os.path.expanduser("~")),
+                "volatility3",
+                filename,
+            )
+
+        delayed_logs = []
+
+        # Process it if the files exist
+        if os.path.exists(default_config_path):
+            with open(default_config_path, "rb") as config_json:
+                result = json.load(config_json)
+            if not isinstance(result, dict):
+                delayed_logs.append(
+                    (
+                        logging.INFO,
+                        f"Default configuration file {default_config_path} does not contain a dictionary",
+                    )
+                )
+            else:
+                delayed_logs.append(
+                    (
+                        logging.INFO,
+                        f"Loading default configuration options from {default_config_path}",
+                    )
+                )
+                delayed_logs.append(
+                    (
+                        logging.DEBUG,
+                        f"Loaded configuration: {json.dumps(result, indent = 2, sort_keys = True)}",
+                    )
+                )
+                return delayed_logs, result
+        return delayed_logs, {}
+
     def process_exceptions(self, excp):
         """Provide useful feedback if an exception occurs during a run of a plugin."""
         # Ensure there's nothing in the cache
         sys.stdout.write("\n\n")
         sys.stdout.flush()
         sys.stderr.flush()
 
@@ -627,14 +693,25 @@
                         # We must be the plugin, so name it appropriately:
                         config_path = plugin_config_path
                     extended_path = interfaces.configuration.path_join(
                         config_path, requirement.name
                     )
                     context.config[extended_path] = value
 
+    def order_extra_verbose_levels(self):
+        for level, level_value in enumerate(
+            [
+                constants.LOGLEVEL_V,
+                constants.LOGLEVEL_VV,
+                constants.LOGLEVEL_VVV,
+                constants.LOGLEVEL_VVVV,
+            ]
+        ):
+            logging.addLevelName(level_value, f"DETAIL {level+1}")
+
     def file_handler_class_factory(self, direct=True):
         output_dir = self.output_dir
 
         class CLIFileHandler(interfaces.plugins.FileHandlerInterface):
             def _get_final_filename(self):
                 """Gets the final filename"""
                 if output_dir is None:
@@ -759,15 +836,19 @@
                     additional["action"] = "store_true"
                     if "type" in additional:
                         del additional["type"]
             elif isinstance(
                 requirement,
                 volatility3.framework.configuration.requirements.ListRequirement,
             ):
-                additional["type"] = requirement.element_type
+                # Allow a list of integers, specified with the convenient 0x hexadecimal format
+                if requirement.element_type == int:
+                    additional["type"] = lambda x: int(x, 0)
+                else:
+                    additional["type"] = requirement.element_type
                 nargs = "*" if requirement.optional else "+"
                 additional["nargs"] = nargs
             elif isinstance(
                 requirement,
                 volatility3.framework.configuration.requirements.ChoiceRequirement,
             ):
                 additional["type"] = str
```

### Comparing `volatility3-2.5.2/volatility3/cli/text_renderer.py` & `volatility3-2.7.0/volatility3/cli/text_renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import json
 import logging
 import random
 import string
 import sys
 from functools import wraps
 from typing import Any, Callable, Dict, List, Tuple
+from volatility3.cli import text_filter
 
 from volatility3.framework import interfaces, renderers
 from volatility3.framework.renderers import format_hints
 
 vollog = logging.getLogger(__name__)
 
 try:
@@ -130,14 +131,15 @@
 
 
 class CLIRenderer(interfaces.renderers.Renderer):
     """Class to add specific requirements for CLI renderers."""
 
     name = "unnamed"
     structured_output = False
+    filter: text_filter.CLIFilter = None
 
 
 class QuickTextRenderer(CLIRenderer):
     _type_renderers = {
         format_hints.Bin: optional(lambda x: f"0b{x:b}"),
         format_hints.Hex: optional(lambda x: f"0x{x:x}"),
         format_hints.HexBytes: optional(hex_bytes_as_text),
@@ -168,14 +170,17 @@
         line = []
         for column in grid.columns:
             # Ignore the type because namedtuples don't realize they have accessible attributes
             line.append(f"{column.name}")
         outfd.write("\n{}\n".format("\t".join(line)))
 
         def visitor(node: interfaces.renderers.TreeNode, accumulator):
+            if self.filter and self.filter.filter(node.values):
+                return accumulator
+
             accumulator.write("\n")
             # Nodes always have a path value, giving them a path_depth of at least 1, we use max just in case
             accumulator.write(
                 "*" * max(0, node.path_depth - 1)
                 + ("" if (node.path_depth <= 1) else " ")
             )
             line = []
@@ -302,14 +307,18 @@
             node: interfaces.renderers.TreeNode,
             accumulator: List[Tuple[int, Dict[interfaces.renderers.Column, bytes]]],
         ) -> List[Tuple[int, Dict[interfaces.renderers.Column, bytes]]]:
             # Nodes always have a path value, giving them a path_depth of at least 1, we use max just in case
             max_column_widths[tree_indent_column] = max(
                 max_column_widths.get(tree_indent_column, 0), node.path_depth
             )
+
+            if self.filter and self.filter.filter(node.values):
+                return accumulator
+
             line = {}
             for column_index in range(len(grid.columns)):
                 column = grid.columns[column_index]
                 renderer = self._type_renderers.get(
                     column.type, self._type_renderers["default"]
                 )
                 data = renderer(node.values[column_index])
```

### Comparing `volatility3-2.5.2/volatility3/cli/volargparse.py` & `volatility3-2.7.0/volatility3/cli/volargparse.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/cli/volshell/__init__.py` & `volatility3-2.7.0/volatility3/cli/volshell/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,22 @@
     contexts,
     exceptions,
     interfaces,
     plugins,
 )
 
 # Make sure we log everything
+
+rootlog = logging.getLogger()
 vollog = logging.getLogger()
 vollog.setLevel(0)
-# Trim the console down by default
 console = logging.StreamHandler()
 console.setLevel(logging.WARNING)
 formatter = logging.Formatter("%(levelname)-8s %(name)-12s: %(message)s")
+# Trim the console down by default
 console.setFormatter(formatter)
 vollog.addHandler(console)
 
 
 class VolShell(cli.CommandLine):
     """Program to allow interactive interaction with a memory image.
 
@@ -49,14 +51,17 @@
         determining the plugin to run and then running it."""
         sys.stdout.write(
             f"Volshell (Volatility 3 Framework) {constants.PACKAGE_VERSION}\n"
         )
 
         framework.require_interface_version(2, 0, 0)
 
+        # Load up system defaults
+        delayed_logs, default_config = self.load_system_defaults("volshell.json")
+
         parser = argparse.ArgumentParser(
             prog=self.CLI_NAME,
             description="A tool for interactivate forensic analysis of memory images",
         )
         parser.add_argument(
             "-c",
             "--config",
@@ -142,14 +147,20 @@
         )
         parser.add_argument(
             "--cache-path",
             help=f"Change the default path ({constants.CACHE_PATH}) used to store the cache",
             default=constants.CACHE_PATH,
             type=str,
         )
+        parser.add_argument(
+            "--offline",
+            help="Do not search online for additional JSON files",
+            default=False,
+            action="store_true",
+        )
 
         # Volshell specific flags
         os_specific = parser.add_mutually_exclusive_group(required=False)
         os_specific.add_argument(
             "-w",
             "--windows",
             default=False,
@@ -163,18 +174,43 @@
             action="store_true",
             help="Run a Linux volshell",
         )
         os_specific.add_argument(
             "-m", "--mac", default=False, action="store_true", help="Run a Mac volshell"
         )
 
+        parser.set_defaults(**default_config)
+
         # We have to filter out help, otherwise parse_known_args will trigger the help message before having
         # processed the plugin choice or had the plugin subparser added.
         known_args = [arg for arg in sys.argv if arg != "--help" and arg != "-h"]
         partial_args, _ = parser.parse_known_args(known_args)
+
+        ### Start up logging
+        if partial_args.log:
+            file_logger = logging.FileHandler(partial_args.log)
+            file_logger.setLevel(0)
+            file_formatter = logging.Formatter(
+                datefmt="%y-%m-%d %H:%M:%S",
+                fmt="%(asctime)s %(name)-12s %(levelname)-8s %(message)s",
+            )
+            file_logger.setFormatter(file_formatter)
+            vollog.addHandler(file_logger)
+            vollog.info("Logging started")
+
+        self.order_extra_verbose_levels()
+        if partial_args.verbosity < 3:
+            console.setLevel(logging.WARNING - (partial_args.verbosity * 10))
+        else:
+            console.setLevel(logging.DEBUG - (partial_args.verbosity - 2))
+
+        for level, msg in delayed_logs:
+            vollog.log(level, msg)
+
+        ### Alter constants if necessary
         if partial_args.plugin_dirs:
             volatility3.plugins.__path__ = [
                 os.path.abspath(p) for p in partial_args.plugin_dirs.split(";")
             ] + constants.PLUGINS_PATH
 
         if partial_args.symbol_dirs:
             volatility3.symbols.__path__ = [
@@ -183,33 +219,20 @@
 
         if partial_args.cache_path:
             constants.CACHE_PATH = partial_args.cache_path
 
         vollog.info(f"Volatility plugins path: {volatility3.plugins.__path__}")
         vollog.info(f"Volatility symbols path: {volatility3.symbols.__path__}")
 
-        if partial_args.log:
-            file_logger = logging.FileHandler(partial_args.log)
-            file_logger.setLevel(0)
-            file_formatter = logging.Formatter(
-                datefmt="%y-%m-%d %H:%M:%S",
-                fmt="%(asctime)s %(name)-12s %(levelname)-8s %(message)s",
-            )
-            file_logger.setFormatter(file_formatter)
-            vollog.addHandler(file_logger)
-            vollog.info("Logging started")
-
-        if partial_args.verbosity < 3:
-            console.setLevel(30 - (partial_args.verbosity * 10))
-        else:
-            console.setLevel(10 - (partial_args.verbosity - 2))
-
         if partial_args.clear_cache:
             framework.clear_cache()
 
+        if partial_args.offline:
+            constants.OFFLINE = partial_args.offline
+
         # Do the initialization
         ctx = contexts.Context()  # Construct a blank context
         failures = framework.import_files(
             volatility3.plugins, True
         )  # Will not log as console's default level is WARNING
         if failures:
             parser.epilog = (
```

### Comparing `volatility3-2.5.2/volatility3/cli/volshell/generic.py` & `volatility3-2.7.0/volatility3/cli/volshell/generic.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/cli/volshell/linux.py` & `volatility3-2.7.0/volatility3/cli/volshell/linux.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/cli/volshell/mac.py` & `volatility3-2.7.0/volatility3/cli/volshell/mac.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/cli/volshell/windows.py` & `volatility3-2.7.0/volatility3/cli/volshell/windows.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/__init__.py` & `volatility3-2.7.0/volatility3/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/automagic/__init__.py` & `volatility3-2.7.0/volatility3/framework/automagic/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/automagic/construct_layers.py` & `volatility3-2.7.0/volatility3/framework/automagic/construct_layers.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/automagic/linux.py` & `volatility3-2.7.0/volatility3/framework/automagic/linux.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/automagic/mac.py` & `volatility3-2.7.0/volatility3/framework/automagic/mac.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/automagic/module.py` & `volatility3-2.7.0/volatility3/framework/automagic/module.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/automagic/pdbscan.py` & `volatility3-2.7.0/volatility3/framework/automagic/pdbscan.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/automagic/stacker.py` & `volatility3-2.7.0/volatility3/framework/automagic/stacker.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/automagic/symbol_cache.py` & `volatility3-2.7.0/volatility3/framework/automagic/symbol_cache.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/automagic/symbol_finder.py` & `volatility3-2.7.0/volatility3/framework/automagic/symbol_finder.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/automagic/windows.py` & `volatility3-2.7.0/volatility3/framework/automagic/windows.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/configuration/requirements.py` & `volatility3-2.7.0/volatility3/framework/configuration/requirements.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/constants/__init__.py` & `volatility3-2.7.0/volatility3/framework/constants/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,37 +40,41 @@
     ] + SYMBOL_BASEPATHS
 
 BANG = "!"
 """Constant used to delimit table names from type names when referring to a symbol"""
 
 # We use the SemVer 2.0.0 versioning scheme
 VERSION_MAJOR = 2  # Number of releases of the library with a breaking change
-VERSION_MINOR = 5  # Number of changes that only add to the interface
-VERSION_PATCH = 2  # Number of changes that do not change the interface
+VERSION_MINOR = 7  # Number of changes that only add to the interface
+VERSION_PATCH = 0  # Number of changes that do not change the interface
 VERSION_SUFFIX = ""
 
 # TODO: At version 2.0.0, remove the symbol_shift feature
 
 PACKAGE_VERSION = (
     ".".join([str(x) for x in [VERSION_MAJOR, VERSION_MINOR, VERSION_PATCH]])
     + VERSION_SUFFIX
 )
 """The canonical version of the volatility3 package"""
 
 AUTOMAGIC_CONFIG_PATH = "automagic"
 """The root section within the context configuration for automagic values"""
 
+LOGLEVEL_INFO = 20
+"""Logging level for information data, showed when use the requests any logging: -v"""
+LOGLEVEL_DEBUG = 10
+"""Logging level for debugging data, showed when the user requests more logging detail: -vv"""
 LOGLEVEL_V = 9
-"""Logging level for a single -v"""
+"""Logging level for the lowest "extra" level of logging: -vvv"""
 LOGLEVEL_VV = 8
-"""Logging level for -vv"""
+"""Logging level for two levels of detail: -vvvv"""
 LOGLEVEL_VVV = 7
-"""Logging level for -vvv"""
+"""Logging level for three levels of detail: -vvvvv"""
 LOGLEVEL_VVVV = 6
-"""Logging level for -vvvv"""
+"""Logging level for four levels of detail: -vvvvvv"""
 
 CACHE_PATH = os.path.join(os.path.expanduser("~"), ".cache", "volatility3")
 """Default path to store cached data"""
 
 SQLITE_CACHE_PERIOD = "-3 days"
 """SQLite time modifier for how long each item is valid in the cache for"""
```

### Comparing `volatility3-2.5.2/volatility3/framework/constants/linux/__init__.py` & `volatility3-2.7.0/volatility3/framework/constants/linux/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # This file is Copyright 2019 Volatility Foundation and licensed under the Volatility Software License 1.0
 # which is available at https://www.volatilityfoundation.org/license/vsl-v1.0
 #
 """Volatility 3 Linux Constants.
 
 Linux-specific values that aren't found in debug symbols
 """
+from enum import IntEnum
 
 KERNEL_NAME = "__kernel__"
 
-# arch/x86/include/asm/page_types.h
-PAGE_SHIFT = 12
 """The value hard coded from the Linux Kernel (hence not extracted from the layer itself)"""
 
 # include/linux/sched.h
 PF_KTHREAD = 0x00200000  # I'm a kernel thread
 
 # Standard well-defined IP protocols.
 # ref: include/uapi/linux/in.h
@@ -277,7 +276,29 @@
     "audit_read",
     "perfmon",
     "bpf",
     "checkpoint_restore",
 )
 
 ELF_MAX_EXTRACTION_SIZE = 1024 * 1024 * 1024 * 4 - 1
+
+
+class ELF_IDENT(IntEnum):
+    """ELF header e_ident indexes"""
+
+    EI_MAG0 = 0
+    EI_MAG1 = 1
+    EI_MAG2 = 2
+    EI_MAG3 = 3
+    EI_CLASS = 4
+    EI_DATA = 5
+    EI_VERSION = 6
+    EI_OSABI = 7
+    EI_PAD = 8
+
+
+class ELF_CLASS(IntEnum):
+    """ELF header class types"""
+
+    ELFCLASSNONE = 0
+    ELFCLASS32 = 1
+    ELFCLASS64 = 2
```

### Comparing `volatility3-2.5.2/volatility3/framework/contexts/__init__.py` & `volatility3-2.7.0/volatility3/framework/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/exceptions.py` & `volatility3-2.7.0/volatility3/framework/exceptions.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/interfaces/__init__.py` & `volatility3-2.7.0/volatility3/framework/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/interfaces/automagic.py` & `volatility3-2.7.0/volatility3/framework/interfaces/automagic.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/interfaces/configuration.py` & `volatility3-2.7.0/volatility3/framework/interfaces/configuration.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/interfaces/context.py` & `volatility3-2.7.0/volatility3/framework/interfaces/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     def object(
         self,
         object_type: Union[str, "interfaces.objects.Template"],
         layer_name: str,
         offset: int,
         native_layer_name: str = None,
         **arguments,
-    ):
+    ) -> "interfaces.objects.ObjectInterface":
         """Object factory, takes a context, symbol, offset and optional
         layer_name.
 
         Looks up the layer_name in the context, finds the object template based on the symbol,
         and constructs an object using the object template on the layer at the offset.
 
         Args:
```

### Comparing `volatility3-2.5.2/volatility3/framework/interfaces/layers.py` & `volatility3-2.7.0/volatility3/framework/interfaces/layers.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/interfaces/objects.py` & `volatility3-2.7.0/volatility3/framework/interfaces/objects.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/interfaces/plugins.py` & `volatility3-2.7.0/volatility3/framework/interfaces/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     @abstractmethod
     def close(self):
         """Method that commits the file and fixes the final filename for use"""
 
     @staticmethod
     def sanitize_filename(filename: str) -> str:
         """Sanititizes the filename to ensure only a specific whitelist of characters is allowed through"""
-        allowed = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789.- ()[]\{\}!$%^:#~?<>,|"
+        allowed = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789.- ()[]{}!$%^:#~?<>,|"
         result = ""
         for char in filename:
             if char in allowed:
                 result += char
             else:
                 result += "?"
         return result
```

### Comparing `volatility3-2.5.2/volatility3/framework/interfaces/renderers.py` & `volatility3-2.7.0/volatility3/framework/interfaces/renderers.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/interfaces/symbols.py` & `volatility3-2.7.0/volatility3/framework/interfaces/symbols.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/layers/avml.py` & `volatility3-2.7.0/volatility3/framework/layers/avml.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/layers/cloudstorage.py` & `volatility3-2.7.0/volatility3/framework/layers/cloudstorage.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 try:
     import gcsfs
 
     HAS_GCSFS = True
 except ImportError:
     HAS_GCSFS = False
 
-from volatility3.framework import exceptions
 from volatility3.framework.layers import resources
 
 vollog = logging.getLogger(__file__)
 
 if HAS_S3FS:
 
     class S3FileSystemHandler(resources.VolatilityHandler):
```

### Comparing `volatility3-2.5.2/volatility3/framework/layers/crash.py` & `volatility3-2.7.0/volatility3/framework/layers/crash.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,19 @@
     def stack(
         cls,
         context: interfaces.context.ContextInterface,
         layer_name: str,
         progress_callback: constants.ProgressCallback = None,
     ) -> Optional[interfaces.layers.DataLayerInterface]:
         for layer in [WindowsCrashDump32Layer, WindowsCrashDump64Layer]:
-            with contextlib.suppress(WindowsCrashDumpFormatException):
+            try:
                 layer.check_header(context.layers[layer_name])
                 new_name = context.layers.free_layer_name(layer.__name__)
                 context.config[
                     interfaces.configuration.path_join(new_name, "base_layer")
                 ] = layer_name
                 return layer(context, new_name, new_name)
+            except WindowsCrashDumpFormatException as excp:
+                vollog.log(
+                    constants.LOGLEVEL_VVVV, f"Exception reading crashdump: {excp}"
+                )
         return None
```

### Comparing `volatility3-2.5.2/volatility3/framework/layers/elf.py` & `volatility3-2.7.0/volatility3/framework/layers/elf.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 # which is available at https://www.volatilityfoundation.org/license/vsl-v1.0
 #
 import logging
 import struct
 from typing import Optional
 
 from volatility3.framework import exceptions, interfaces, constants
+from volatility3.framework.constants.linux import ELF_CLASS
 from volatility3.framework.layers import segmented
 from volatility3.framework.symbols import intermed
 
+
 vollog = logging.getLogger(__name__)
 
 
 class ElfFormatException(exceptions.LayerException):
     """Thrown when an error occurs with the underlying ELF file format."""
 
 
 class Elf64Layer(segmented.SegmentedLayer):
     """A layer that supports the Elf64 format as documented at: http://ftp.openwatcom.org/devel/docs/elf-64-gen.pdf"""
 
     _header_struct = struct.Struct("<IBBB")
     MAGIC = 0x464C457F  # "\x7fELF"
-    ELF_CLASS = 2
+    ELF_CLASS = ELF_CLASS.ELFCLASS64
 
     def __init__(
         self, context: interfaces.context.ContextInterface, config_path: str, name: str
     ) -> None:
         # Create a custom SymbolSpace
         self._elf_table_name = intermed.IntermediateSymbolTable.create(
             context, config_path, "linux", "elf"
@@ -46,16 +48,25 @@
         for pindex in range(ehdr.e_phnum):
             phdr = self.context.object(
                 self._elf_table_name + constants.BANG + "Elf64_Phdr",
                 layer_name=self._base_layer,
                 offset=ehdr.e_phoff + (pindex * ehdr.e_phentsize),
             )
             # We only want PT_TYPES with valid sizes
+            try:
+                ptype = phdr.p_type.description
+            except ValueError:
+                vollog.log(
+                    constants.LOGLEVEL_VVVV,
+                    f"Skipping unknown ELF program header type: {phdr.p_type}",
+                )
+                continue
+
             if (
-                phdr.p_type.lookup() == "PT_LOAD"
+                ptype == "PT_LOAD"
                 and phdr.p_filesz == phdr.p_memsz
                 and phdr.p_filesz > 0
             ):
                 # Cast these to ints to ensure the offsets don't need reconstructing
                 segments.append(
                     (
                         int(phdr.p_paddr),
```

### Comparing `volatility3-2.5.2/volatility3/framework/layers/intel.py` & `volatility3-2.7.0/volatility3/framework/layers/intel.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,23 +65,35 @@
         # These can vary depending on the type of space
         self._index_shift = int(
             math.ceil(math.log2(struct.calcsize(self._entry_format)))
         )
 
     @classproperty
     @functools.lru_cache()
+    def page_shift(cls) -> int:
+        """Page shift for the intel memory layers."""
+        return cls._page_size_in_bits
+
+    @classproperty
+    @functools.lru_cache()
     def page_size(cls) -> int:
         """Page size for the intel memory layers.
 
         All Intel layers work on 4096 byte pages
         """
         return 1 << cls._page_size_in_bits
 
     @classproperty
     @functools.lru_cache()
+    def page_mask(cls) -> int:
+        """Page mask for the intel memory layers."""
+        return ~(cls.page_size - 1)
+
+    @classproperty
+    @functools.lru_cache()
     def bits_per_register(cls) -> int:
         """Returns the bits_per_register to determine the range of an
         IntelTranslationLayer."""
         return cls._bits_per_register
 
     @classproperty
     @functools.lru_cache()
```

### Comparing `volatility3-2.5.2/volatility3/framework/layers/leechcore.py` & `volatility3-2.7.0/volatility3/framework/layers/leechcore.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/layers/lime.py` & `volatility3-2.7.0/volatility3/framework/layers/lime.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/layers/linear.py` & `volatility3-2.7.0/volatility3/framework/layers/linear.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/layers/msf.py` & `volatility3-2.7.0/volatility3/framework/layers/msf.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/layers/physical.py` & `volatility3-2.7.0/volatility3/framework/layers/physical.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/layers/qemu.py` & `volatility3-2.7.0/volatility3/framework/layers/qemu.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/layers/registry.py` & `volatility3-2.7.0/volatility3/framework/layers/registry.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/layers/resources.py` & `volatility3-2.7.0/volatility3/framework/layers/resources.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/layers/scanners/__init__.py` & `volatility3-2.7.0/volatility3/framework/layers/scanners/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/layers/scanners/multiregexp.py` & `volatility3-2.7.0/volatility3/framework/layers/scanners/multiregexp.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/layers/segmented.py` & `volatility3-2.7.0/volatility3/framework/layers/segmented.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/layers/vmware.py` & `volatility3-2.7.0/volatility3/framework/layers/vmware.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/layers/xen.py` & `volatility3-2.7.0/volatility3/framework/layers/xen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import logging
 import struct
 from typing import Optional
 
 from volatility3.framework import constants, interfaces, exceptions
 from volatility3.framework.layers import elf
 from volatility3.framework.symbols import intermed
+from volatility3.framework.constants.linux import ELF_CLASS
 
 vollog = logging.getLogger(__name__)
 
 
 class XenCoreDumpLayer(elf.Elf64Layer):
     """A layer that supports the Xen Dump-Core format as documented at: https://xenbits.xen.org/docs/4.6-testing/misc/dump-core-format.txt"""
 
     _header_struct = struct.Struct("<IBBB")
     MAGIC = 0x464C457F  # "\x7fELF"
-    ELF_CLASS = 2
+    ELF_CLASS = ELF_CLASS.ELFCLASS64
 
     def __init__(
         self, context: interfaces.context.ContextInterface, config_path: str, name: str
     ) -> None:
         # Create a custom SymbolSpace
         self._elf_table_name = intermed.IntermediateSymbolTable.create(
             context, config_path, "linux", "elf"
@@ -111,20 +112,18 @@
                             entry.pfn * page_size,
                             pages_hdr.sh_offset + (entry_index * page_size),
                             page_size,
                             page_size,
                         )
                     )
         elif p2m_data and pfn_data:
-            raise elf.ElfFormatException(
-                self.name, f"Both P2M and PFN in Xen Core Dump"
-            )
+            raise elf.ElfFormatException(self.name, "Both P2M and PFN in Xen Core Dump")
         else:
             raise elf.ElfFormatException(
-                self.name, f"Neither P2M nor PFN in Xen Core Dump"
+                self.name, "Neither P2M nor PFN in Xen Core Dump"
             )
 
         if len(segments) == 0:
             raise elf.ElfFormatException(
                 self.name, f"No ELF segments defined in {self._base_layer}"
             )
```

### Comparing `volatility3-2.5.2/volatility3/framework/objects/__init__.py` & `volatility3-2.7.0/volatility3/framework/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/objects/templates.py` & `volatility3-2.7.0/volatility3/framework/objects/templates.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/objects/utility.py` & `volatility3-2.7.0/volatility3/framework/objects/utility.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/__init__.py` & `volatility3-2.7.0/volatility3/framework/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/banners.py` & `volatility3-2.7.0/volatility3/framework/plugins/banners.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/configwriter.py` & `volatility3-2.7.0/volatility3/framework/plugins/configwriter.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/frameworkinfo.py` & `volatility3-2.7.0/volatility3/framework/plugins/frameworkinfo.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/isfinfo.py` & `volatility3-2.7.0/volatility3/framework/plugins/isfinfo.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/layerwriter.py` & `volatility3-2.7.0/volatility3/framework/plugins/layerwriter.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/bash.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/bash.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/capabilities.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/capabilities.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/check_afinfo.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/check_afinfo.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/check_creds.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/check_creds.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/check_idt.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/check_idt.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/check_modules.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/check_modules.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/check_syscall.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/check_syscall.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/elfs.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/elfs.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,26 @@
 from volatility3.framework import constants, interfaces, renderers
 from volatility3.framework.configuration import requirements
 from volatility3.framework.interfaces import plugins
 from volatility3.framework.objects import utility
 from volatility3.framework.renderers import format_hints
 from volatility3.framework.symbols import intermed
 from volatility3.framework.symbols.linux.extensions import elf
+from volatility3.framework.constants.linux import ELF_MAX_EXTRACTION_SIZE
 from volatility3.plugins.linux import pslist
 
+
 vollog = logging.getLogger(__name__)
 
 
 class Elfs(plugins.PluginInterface):
     """Lists all memory mapped ELF files for all processes."""
 
     _required_framework_version = (2, 0, 0)
-    _version = (2, 0, 0)
+    _version = (2, 0, 1)
 
     @classmethod
     def get_requirements(cls) -> List[interfaces.configuration.RequirementInterface]:
         return [
             requirements.ModuleRequirement(
                 name="kernel",
                 description="Linux kernel",
@@ -78,39 +80,47 @@
         elf_object = context.object(
             elf_table_name + constants.BANG + "Elf",
             offset=vma.vm_start,
             layer_name=layer_name,
         )
 
         if not elf_object.is_valid():
+            vollog.debug("ELF object to be dumped is not valid")
             return None
 
         sections = {}
         # TODO: Apply more effort to reconstruct ELF, e.g.: https://github.com/enbarberis/core2ELF64 ?
         for phdr in elf_object.get_program_headers():
-            if phdr.p_type != 1:  # PT_LOAD = 1
+            try:
+                if phdr.p_type.description != "PT_LOAD":
+                    continue
+            except ValueError:
+                vollog.log(
+                    constants.LOGLEVEL_VVVV,
+                    f"Skipping unknown ELF program header type: {phdr.p_type}",
+                )
                 continue
 
             start = phdr.p_vaddr
             size = phdr.p_memsz
             end = start + size
 
             # Use complete memory pages for dumping
-            # If start isn't a multiple of 4096, stick to the highest multiple < start
-            # If end isn't a multiple of 4096, stick to the lowest multiple > end
-            if start % 4096:
-                start = start & ~0xFFF
+            # If start isn't a multiple of a page, stick to the highest multiple < start
+            # If end isn't a multiple of a page, stick to the lowest multiple > end
+            if start % proc_layer.page_size:
+                start = start & proc_layer.page_mask
 
-            if end % 4096:
-                end = (end & ~0xFFF) + 4096
+            if end % proc_layer.page_size:
+                end = (end & proc_layer.page_mask) + proc_layer.page_size
 
             real_size = end - start
 
             # Check if ELF has a legitimate size
-            if real_size < 0 or real_size > constants.linux.ELF_MAX_EXTRACTION_SIZE:
+            if real_size < 0 or real_size > ELF_MAX_EXTRACTION_SIZE:
                 raise ValueError(f"The claimed size of the ELF is invalid: {real_size}")
 
             sections[start] = real_size
 
         elf_data = b""
         for section_start in sorted(sections.keys()):
             read_size = sections[section_start]
@@ -136,20 +146,15 @@
 
             proc_layer = self.context.layers[proc_layer_name]
 
             name = utility.array_to_string(task.comm)
 
             for vma in task.mm.get_vma_iter():
                 hdr = proc_layer.read(vma.vm_start, 4, pad=True)
-                if not (
-                    hdr[0] == 0x7F
-                    and hdr[1] == 0x45
-                    and hdr[2] == 0x4C
-                    and hdr[3] == 0x46
-                ):
+                if hdr != b"\x7fELF":
                     continue
 
                 path = vma.get_name(self.context, task)
 
                 file_output = "Disabled"
                 if self.config["dump"]:
                     file_handle = self.elf_dump(
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/envars.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/envars.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/iomem.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/iomem.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/keyboard_notifiers.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/keyboard_notifiers.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/kmsg.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/kmsg.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file is Copyright 2021 Volatility Foundation and licensed under the Volatility Software License 1.0
 # which is available at https://www.volatilityfoundation.org/license/vsl-v1.0
 #
+import re
 import logging
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Generator, Iterator, List, Tuple
 
 from volatility3.framework import (
     class_subclasses,
     constants,
-    contexts,
+    exceptions,
     interfaces,
     renderers,
 )
 from volatility3.framework.configuration import requirements
-from volatility3.framework.interfaces import plugins
 from volatility3.framework.objects import utility
 
 vollog = logging.getLogger(__name__)
 
 
 class DescStateEnum(Enum):
     desc_miss = -1  # ID mismatch (pseudo state)
@@ -78,15 +78,15 @@
         conditions to that specific kernel implementation.
 
         Args:
             context: The volatility3 context on which to operate
             config: Core configuration
 
         Yields:
-            kmsg records
+            The kmsg records. Same as run()
         """
         vmlinux = context.modules[config["kernel"]]
 
         kmsg_inst = None  # type: ignore
         for subclass in class_subclasses(cls):
             if not subclass.symtab_checks(vmlinux=vmlinux):
                 vollog.log(
@@ -98,36 +98,45 @@
 
             vollog.log(
                 constants.LOGLEVEL_VVVV,
                 "Kmsg implementation '%s' matches!",
                 subclass.__name__,
             )
             kmsg_inst = subclass(context=context, config=config)
-            # More than one class could be executed for an specific kernel
-            # version i.e. Netfilter Ingress hooks
-            # We expect just one implementation to be executed for an specific kernel
             yield from kmsg_inst.run()
+            # So far, it only allows a single implementation to be executed for each
+            # specific kernel.
             break
 
         if kmsg_inst is None:
-            vollog.error("Unsupported Netfilter kernel implementation")
+            vollog.error("Unsupported kernel ring buffer implementation")
 
     @abstractmethod
     def run(self) -> Iterator[Tuple[str, str, str, str, str]]:
-        """Walks through the specific kernel implementation."""
+        """Walks through the specific kernel implementation.
+
+        Returns:
+            tuple:
+                facility [str]: The log facility: kern, user, etc. See FACILITIES
+                level [str]: The log level: info, debug, etc. See LEVELS
+                timestamp [str]: The message timestamp. See nsec_to_sec_str()
+                caller [str]: The caller ID: CPU(1) or Task(1234). See get_caller()
+                line [str]: The log message.
+        """
 
     @classmethod
     @abstractmethod
     def symtab_checks(cls, vmlinux: interfaces.context.ModuleInterface) -> bool:
         """This method on each sublasss will be called to evaluate if the kernel
         being analyzed fulfill the type & symbols requirements for the implementation.
         The first class returning True will be instantiated and called via the
         run() method.
 
-        :return: True is the kernel being analysed fulfill the class requirements.
+        Returns:
+            bool: True if the kernel being analyzed fulfill the class requirements.
         """
 
     def get_string(self, addr: int, length: int) -> str:
         txt = self._context.layers[self.layer_name].read(addr, length)  # type: ignore
         return txt.decode(encoding="utf8", errors="replace")
 
     def nsec_to_sec_str(self, nsec: int) -> str:
@@ -139,33 +148,33 @@
         #   While the kernel print_time function will result in 17.110365.
         #   This might seem insignificant but it could cause some issues
         #   when compared with userland tool results or when used in
         #   timelines.
         return "%lu.%06lu" % (nsec / 1000000000, (nsec % 1000000000) / 1000)
 
     def get_timestamp_in_sec_str(self, obj) -> str:
-        # obj could be printk_log or printk_info
+        # obj could be log, printk_log or printk_info
         return self.nsec_to_sec_str(obj.ts_nsec)
 
     def get_caller(self, obj):
         # In some kernel versions, it's only available if CONFIG_PRINTK_CALLER is defined.
         # caller_id is a member of printk_log struct from 5.1 to the latest 5.9
         # From kernels 5.10 on, it's a member of printk_info struct
         if obj.has_member("caller_id"):
             return self.get_caller_text(obj.caller_id)
         else:
-            return ""
+            return renderers.NotAvailableValue()
 
     def get_caller_text(self, caller_id):
         caller_name = "CPU" if caller_id & 0x80000000 else "Task"
         caller = "%s(%u)" % (caller_name, caller_id & ~0x80000000)
         return caller
 
     def get_prefix(self, obj) -> Tuple[int, int, str, str]:
-        # obj could be printk_log or printk_info
+        # obj could be log, printk_log or printk_info
         return (
             obj.facility,
             obj.level,
             self.get_timestamp_in_sec_str(obj),
             self.get_caller(obj),
         )
 
@@ -182,123 +191,202 @@
         if facility < len(cls.FACILITIES):
             return cls.FACILITIES[facility]
         else:
             vollog.debug(f"Facility {facility} unknown")
             return str(facility)
 
 
-class KmsgLegacy(ABCKmsg):
-    """Linux kernels prior to v5.10, the ringbuffer is initially kept in
-    __log_buf, and log_buf is a pointer to the former. __log_buf is declared as
-    a char array but it actually contains an array of printk_log structs.
-    The length of this array is defined in the kernel KConfig configuration via
-    the CONFIG_LOG_BUF_SHIFT value as a power of 2.
-    This can also be modified by the log_buf_len kernel boot parameter.
-    In SMP systems with more than 64 CPUs this ringbuffer size is dynamically
-    allocated according the number of CPUs based on the value of
-    CONFIG_LOG_CPU_MAX_BUF_SHIFT, and the log_buf pointer is updated
-    consequently to the new buffer.
-    In that case, the original static buffer in __log_buf is unused.
+class Kmsg_pre_3_5(ABCKmsg):
+    """The kernel ring buffer (log_buf) is a char array that sequentially stores
+    log lines, each separated by newline (LF) characters. i.e:
+
+        <6>[ 9565.250411] line1!\\n<6>[ 9565.250412] line2\\n...
+
     """
 
     @classmethod
     def symtab_checks(cls, vmlinux) -> bool:
-        return vmlinux.has_type("printk_log")
+        return (
+            vmlinux.has_symbol("log_end")
+            and not vmlinux.has_symbol("log_first_idx")
+            and not (
+                vmlinux.has_type("log")
+                and vmlinux.get_type("log").has_member("ts_nsec")
+            )
+        )
+
+    def run(self) -> Iterator[Tuple[str, str, str, str, str]]:
+        log_buf_ptr = self.vmlinux.object_from_symbol(symbol_name="log_buf")
+        log_buf_len = self.vmlinux.object_from_symbol(symbol_name="log_buf_len")
+        log_buf = utility.pointer_to_string(log_buf_ptr, count=log_buf_len)
+        log_end = self.vmlinux.object_from_symbol(symbol_name="log_end")
+
+        if log_end > log_buf_len:
+            start = log_end - log_buf_len
+            first_half = log_buf[start:]
+            second_half = log_buf[:start]
+            log_buf = first_half + second_half
+
+        log_buf_lines = log_buf.splitlines()
+
+        for log_buf_line in log_buf_lines:
+            m = re.match(r"<(\d+)>\[\s*(\d+\.\d+)\]\s(.*?)$", log_buf_line)
+            if not m:
+                # If there was a wrap-around in the ring buffer, it will find
+                # remnants at the top. As those remnants do not conform to the
+                # expected line format, they are discarded
+                continue
 
-    def get_text_from_printk_log(self, msg) -> str:
-        msg_offset = msg.vol.offset + self.vmlinux.get_type("printk_log").size
+            level_facility_str, timestamp_str, line = m.groups()
+            level_facility = int(level_facility_str)
+            # The lower 3 bit are the log level, the rest are the log facility
+            level = level_facility & 7
+            facility = level_facility >> 3
+            level_txt = self.get_level_text(level)
+            facility_txt = self.get_facility_text(facility)
+            caller = renderers.NotAvailableValue()
+            yield facility_txt, level_txt, timestamp_str, caller, line
+
+
+class Kmsg_3_5_to_3_11(ABCKmsg):
+    """While 'log_buf' is declared as a pointer and '__log_buf' as a char array,
+    it essentially holds an array of 'log' structs.
+    """
+
+    @classmethod
+    def symtab_checks(cls, vmlinux) -> bool:
+        return (
+            vmlinux.has_type("log")
+            and vmlinux.get_type("log").has_member("ts_nsec")
+            and vmlinux.has_symbol("log_first_idx")
+        )
+
+    def _get_log_struct_name(self):
+        return "log"
+
+    def get_text_from_log(self, msg) -> str:
+        log_struct_name = self._get_log_struct_name()
+        log_struct_size = self.vmlinux.get_type(log_struct_name).size
+        msg_offset = msg.vol.offset + log_struct_size
         return self.get_string(msg_offset, msg.text_len)
 
     def get_log_lines(self, msg) -> Generator[str, None, None]:
         if msg.text_len > 0:
-            text = self.get_text_from_printk_log(msg)
+            text = self.get_text_from_log(msg)
             yield from text.splitlines()
 
     def get_dict_lines(self, msg) -> Generator[str, None, None]:
         if msg.dict_len == 0:
             return None
-        dict_offset = (
-            msg.vol.offset + self.vmlinux.get_type("printk_log").size + msg.text_len
-        )
+
+        log_struct_name = self._get_log_struct_name()
+        log_struct_size = self.vmlinux.get_type(log_struct_name).size
+        dict_offset = msg.vol.offset + log_struct_size + msg.text_len
         dict_data = self._context.layers[self.layer_name].read(
             dict_offset, msg.dict_len
         )
         for chunk in dict_data.split(b"\x00"):
             yield " " + chunk.decode()
 
     def run(self) -> Iterator[Tuple[str, str, str, str, str]]:
-        log_buf_ptr = self.vmlinux.object_from_symbol(symbol_name="log_buf")
-        if log_buf_ptr == 0:
-            # This is weird, let's fallback to check the static ringbuffer.
-            log_buf_ptr = self.vmlinux.object_from_symbol(
-                symbol_name="__log_buf"
-            ).vol.offset
-            if log_buf_ptr == 0:
-                raise ValueError("Log buffer is not available")
+        # First, the ring buffer size is determined in the kernel configuration
+        # by CONFIG_LOG_BUF_SHIFT. This static buffer is held in the '__log_buf'
+        # global variable, with 'log_buf' serving as a pointer to it.
+        # The user can also update this size using 'log_buf_len' in the
+        # kernel boot parameters. Additionally, in SMP systems with over 64 CPUs,
+        # the ring buffer size dynamically allocates based on the number of CPUs,
+        # following CONFIG_LOG_CPU_MAX_BUF_SHIFT.
+        # In the last two cases mentioned above, the 'log_buf' pointer is
+        # updated to this new buffer. The original static buffer in '__log_buf'
+        # remains unused. Therefore, it is crucial to read from 'log_buf' rather
+        # than '__log_buf'.
+
+        log_buf_ptr = self.vmlinux.object_from_symbol("log_buf")
+        log_buf_len = self.vmlinux.object_from_symbol("log_buf_len")
+
+        log_first_idx = int(self.vmlinux.object_from_symbol("log_first_idx"))
+        log_next_idx = int(self.vmlinux.object_from_symbol("log_next_idx"))
+
+        log_struct_name = self._get_log_struct_name()
 
-        log_first_idx = int(
-            self.vmlinux.object_from_symbol(symbol_name="log_first_idx")
-        )
         cur_idx = log_first_idx
-        end_idx = None  # We don't need log_next_idx here. See below msg.len == 0
-        while cur_idx != end_idx:
-            end_idx = log_first_idx
+        if log_first_idx < log_next_idx:
+            end_idx = log_next_idx
+        else:
+            end_idx = log_buf_len
+
+        while cur_idx < end_idx:
             msg_offset = log_buf_ptr + cur_idx  # type: ignore
-            msg = self.vmlinux.object(object_type="printk_log", offset=msg_offset)
+            msg = self.vmlinux.object(object_type=log_struct_name, offset=msg_offset)
             if msg.len == 0:
-                # As per kernel/printk/printk.c:
+                # As per kernel/printk.c:
                 # A length == 0 for the next message indicates a wrap-around to
                 # the beginning of the buffer.
                 cur_idx = 0
+                end_idx = log_next_idx
             else:
                 facility, level, timestamp, caller = self.get_prefix(msg)
                 level_txt = self.get_level_text(level)
                 facility_txt = self.get_facility_text(facility)
 
                 for line in self.get_log_lines(msg):
                     yield facility_txt, level_txt, timestamp, caller, line
                 for line in self.get_dict_lines(msg):
                     yield facility_txt, level_txt, timestamp, caller, line
 
                 cur_idx += msg.len
 
 
-class KmsgFiveTen(ABCKmsg):
-    """In 5.10 the kernel ringbuffer implementation changed.
+class Kmsg_3_11_to_5_10(Kmsg_3_5_to_3_11):
+    """Starting from version 3.11, the struct 'log' was renamed to 'printk_log'.
+    While 'log_buf' is declared as a pointer and '__log_buf' as a char array,
+    it essentially holds an array of 'printk_log' structs.
+    """
+
+    @classmethod
+    def symtab_checks(cls, vmlinux) -> bool:
+        return vmlinux.has_type("printk_log")
+
+    def _get_log_struct_name(self):
+        return "printk_log"
+
+
+class Kmsg_5_10_to_(ABCKmsg):
+    """In 5.10 the kernel ring buffer implementation changed.
     Previously only one process should read /proc/kmsg and it is permanently
     open and periodically read by the syslog daemon.
     A high level structure 'printk_ringbuffer' was added to represent the printk
-    ringbuffer which actually contains two ringbuffers. The descriptor ring
+    ring buffer which actually contains two ring buffers. The descriptor ring
     'desc_ring' contains the records' metadata, text offsets and states.
     The data block ring 'text_data_ring' contains the records' text strings.
     A pointer to the high level structure is kept in the prb pointer which is
-    initialized to a static ringbuffer.
+    initialized to a static ring buffer.
 
     .. code-block:: c
 
         static struct printk_ringbuffer *prb = &printk_rb_static;
 
-    In SMP systems with more than 64 CPUs this ringbuffer size is dynamically
+    In SMP systems with more than 64 CPUs this ring buffer size is dynamically
     allocated according the number of CPUs based on the value of
     CONFIG_LOG_CPU_MAX_BUF_SHIFT. The prb pointer is updated consequently to
-    this dynamic ringbuffer in setup_log_buf().
+    this dynamic ring buffer in setup_log_buf().
 
     .. code-block:: c
 
         prb = &printk_rb_dynamic;
 
-    Behind scenes, log_buf is still used as external buffer.
-    When the static printk_ringbuffer struct is initialized, _DEFINE_PRINTKRB
-    sets text_data_ring.data pointer to the address in log_buf which points to
-    the static buffer __log_buff.
-    If a dynamic ringbuffer takes place, setup_log_buf() sets
-    text_data_ring.data of printk_rb_dynamic to the new allocated external
-    buffer via the prb_init function.
-    In that case, the original external static buffer in __log_buf and
-    printk_rb_static are unused.
+    Behind scenes, 'log_buf' is still used as external buffer.
+    When the static 'printk_ringbuffer' struct is initialized, _DEFINE_PRINTKRB
+    sets text_data_ring.data pointer to the address in 'log_buf' which points
+    to the static buffer '__log_buf'.
+    If a dynamic ring buffer takes place, setup_log_buf() sets
+    text_data_ring.data of 'printk_rb_dynamic' to the new allocated external
+    buffer via the 'prb_init' function.
+    In that case, the original external static buffer in '__log_buf' and
+    'printk_rb_static' are unused.
 
     .. code-block:: c
 
         new_log_buf = memblock_alloc(new_log_buf_len, LOG_ALIGN);
         prb_init(&printk_rb_dynamic, new_log_buf, ...);
         log_buf = new_log_buf;
         prb = &printk_rb_dynamic;
@@ -348,15 +436,15 @@
 
         dict_text = utility.array_to_string(info.dev_info.device)
         if dict_text:
             yield f" DEVICE={dict_text}"
 
     def run(self) -> Iterator[Tuple[str, str, str, str, str]]:
         # static struct printk_ringbuffer *prb = &printk_rb_static;
-        ringbuffers = self.vmlinux.object_from_symbol(symbol_name="prb").dereference()
+        ringbuffers = self.vmlinux.object_from_symbol("prb").dereference()
 
         desc_ring = ringbuffers.desc_ring
         text_data_ring = ringbuffers.text_data_ring
         desc_count = 1 << desc_ring.count_bits
 
         array_type = self.vmlinux.symbol_table_name + constants.BANG + "array"
 
@@ -403,20 +491,20 @@
                 for line in self.get_dict_lines(info):
                     yield facility_txt, level_txt, timestamp, caller, line
 
             cur_id += 1
             cur_id &= desc_id_mask
 
 
-class Kmsg(plugins.PluginInterface):
+class Kmsg(interfaces.plugins.PluginInterface):
     """Kernel log buffer reader"""
 
-    _required_framework_version = (2, 0, 0)
+    _required_framework_version = (2, 6, 0)
 
-    _version = (1, 0, 1)
+    _version = (1, 0, 2)
 
     @classmethod
     def get_requirements(cls) -> List[interfaces.configuration.RequirementInterface]:
         return [
             requirements.ModuleRequirement(
                 name="kernel",
                 description="Linux kernel",
@@ -425,14 +513,21 @@
         ]
 
     def _generator(self) -> Iterator[Tuple[int, Tuple[str, str, str, str, str]]]:
         for values in ABCKmsg.run_all(context=self.context, config=self.config):
             yield (0, values)
 
     def run(self):
+        if not self.context.symbol_space.verify_table_versions(
+            "dwarf2json", lambda version, _: (not version) or version > (0, 4, 1)
+        ):
+            raise exceptions.SymbolSpaceError(
+                "Invalid symbol table, please ensure the ISF table produced by dwarf2json was produced using a version > 0.4.1"
+            )
+
         return renderers.TreeGrid(
             [
                 ("facility", str),
                 ("level", str),
                 ("timestamp", str),
                 ("caller", str),
                 ("line", str),
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/lsmod.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/lsmod.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/lsof.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/lsof.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/malfind.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/malfind.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/mountinfo.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/mountinfo.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/proc.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/proc.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/psaux.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/psaux.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/pslist.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/pslist.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class PsList(interfaces.plugins.PluginInterface):
     """Lists the processes present in a particular linux memory image."""
 
     _required_framework_version = (2, 0, 0)
 
-    _version = (2, 2, 0)
+    _version = (2, 2, 1)
 
     @classmethod
     def get_requirements(cls) -> List[interfaces.configuration.RequirementInterface]:
         return [
             requirements.ModuleRequirement(
                 name="kernel",
                 description="Linux kernel",
@@ -79,19 +79,19 @@
             return lambda _: False
 
     @classmethod
     def get_task_fields(
         cls, task: interfaces.objects.ObjectInterface, decorate_comm: bool = False
     ) -> Tuple[int, int, int, str]:
         """Extract the fields needed for the final output
+
         Args:
             task: A task object from where to get the fields.
-            decorate_comm: If True, it decorates the comm string of
-                            - User threads: in curly brackets,
-                            - Kernel threads: in square brackets
+            decorate_comm: If True, it decorates the comm string of user threads in curly brackets,
+                           and of Kernel threads in square brackets.
                            Defaults to False.
         Returns:
             A tuple with the fields to show in the plugin output.
         """
         pid = task.tgid
         tid = task.pid
         ppid = task.parent.tgid if task.parent else 0
@@ -124,28 +124,30 @@
         if not proc_layer_name:
             # if we can't build a proc layer we can't
             # extract the elf
             return renderers.NotApplicableValue()
         else:
             # Find the vma that belongs to the main ELF of the process
             file_output = "Error outputting file"
-            for v in task.mm.get_mmap_iter():
+            for v in task.mm.get_vma_iter():
                 if v.vm_start == task.mm.start_code:
                     file_handle = elfs.Elfs.elf_dump(
                         self.context,
                         proc_layer_name,
                         elf_table_name,
                         v,
                         task,
                         self.open,
                     )
                     if file_handle:
                         file_output = str(file_handle.preferred_filename)
                         file_handle.close()
                     break
+            else:
+                file_output = "VMA start matching task start_code not found"
         return file_output
 
     def _generator(
         self,
         pid_filter: Callable[[Any], bool],
         include_threads: bool = False,
         decorate_comm: bool = False,
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/psscan.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/psscan.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     EXIT_TRACE = EXIT_ZOMBIE | EXIT_DEAD
 
 
 class PsScan(interfaces.plugins.PluginInterface):
     """Scans for processes present in a particular linux image."""
 
     _required_framework_version = (2, 0, 0)
-    _version = (1, 0, 0)
+    _version = (1, 0, 1)
 
     @classmethod
     def get_requirements(cls) -> List[interfaces.configuration.RequirementInterface]:
         return [
             requirements.ModuleRequirement(
                 name="kernel",
                 description="Linux kernel",
@@ -135,15 +135,15 @@
             vollog.error(
                 f"Kernel layer has no dependencies, meaning there is no memory layer for this plugin to scan."
             )
             raise exceptions.LayerException(
                 kernel_layer_name, f"Layer {kernel_layer_name} has no dependencies"
             )
         memory_layer_name = kernel_layer.dependencies[0]
-        memory_layer = context.layers[kernel_layer.dependencies[0]]
+        memory_layer = context.layers[memory_layer_name]
 
         # scan the memory_layer for these needles
         for address, _ in memory_layer.scan(
             context, scanners.MultiStringScanner(needles)
         ):
             # create task in the memory_layer
             ptask = context.object(
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/pstree.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/pstree.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/sockstat.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/sockstat.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     ) -> Tuple[objects.StructType, Tuple[str, str, str], Dict]:
         """Takes a kernel generic `sock` object and processes it with its respective socket family
 
         Args:
             sock: Kernel generic `sock` object
 
         Returns a tuple with:
-            sock: The respective kernel's \*_sock object for that socket family
+            sock: The respective kernel's \\*_sock object for that socket family
             sock_stat: A tuple with the source and destination (address and port) along with its state string
             socket_filter: A dictionary with information about the socket filter
         """
         family = sock.get_family()
         socket_filter = {}
         sock_handler = self._sock_family_handlers.get(family)
         if sock_handler:
@@ -497,15 +497,15 @@
         Yields:
             task: Kernel's task object
             netns_id: Network namespace ID
             fd_num: File descriptor number
             family: Socket family string (AF_UNIX, AF_INET, etc)
             sock_type: Socket type string (STREAM, DGRAM, etc)
             protocol: Protocol string (UDP, TCP, etc)
-            sock_fields: A tuple with the \*_sock object, the sock stats and the extended info dictionary
+            sock_fields: A tuple with the \\*_sock object, the sock stats and the extended info dictionary
         """
         vmlinux = context.modules[symbol_table]
 
         sfop_addr = vmlinux.object_from_symbol("socket_file_ops").vol.offset
         dfop_addr = vmlinux.object_from_symbol("sockfs_dentry_operations").vol.offset
 
         fd_generator = lsof.Lsof.list_fds(context, vmlinux.name, filter_func)
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/tty_check.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/tty_check.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/linux/vmayarascan.py` & `volatility3-2.7.0/volatility3/framework/plugins/linux/vmayarascan.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/bash.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/bash.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/check_syscall.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/check_syscall.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/check_sysctl.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/check_sysctl.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/check_trap_table.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/check_trap_table.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/ifconfig.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/ifconfig.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/kauth_listeners.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/kauth_listeners.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/kauth_scopes.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/kauth_scopes.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/kevents.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/kevents.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/list_files.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/list_files.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/lsmod.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/lsmod.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/lsof.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/lsof.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/malfind.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/malfind.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/mount.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/mount.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/netstat.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/netstat.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/proc_maps.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/drivermodule.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,85 @@
 # This file is Copyright 2019 Volatility Foundation and licensed under the Volatility Software License 1.0
 # which is available at https://www.volatilityfoundation.org/license/vsl-v1.0
 #
-
+from typing import Iterator, List, Tuple
 from volatility3.framework import renderers, interfaces
 from volatility3.framework.configuration import requirements
-from volatility3.framework.objects import utility
 from volatility3.framework.renderers import format_hints
-from volatility3.plugins.mac import pslist
+from volatility3.plugins.windows import ssdt, driverscan
+
+# built in Windows-components that trigger false positives
+KNOWN_DRIVERS = ["ACPI_HAL", "PnpManager", "RAW", "WMIxWDM", "Win32k", "Fs_Rec"]
 
 
-class Maps(interfaces.plugins.PluginInterface):
-    """Lists process memory ranges that potentially contain injected code."""
+class DriverModule(interfaces.plugins.PluginInterface):
+    """Determines if any loaded drivers were hidden by a rootkit"""
 
     _required_framework_version = (2, 0, 0)
+    _version = (1, 0, 0)
 
     @classmethod
-    def get_requirements(cls):
+    def get_requirements(cls) -> List[interfaces.configuration.RequirementInterface]:
         return [
             requirements.ModuleRequirement(
                 name="kernel",
-                description="Kernel module for the OS",
+                description="Windows kernel",
                 architectures=["Intel32", "Intel64"],
             ),
             requirements.PluginRequirement(
-                name="pslist", plugin=pslist.PsList, version=(3, 0, 0)
+                name="ssdt", plugin=ssdt.SSDT, version=(1, 0, 0)
             ),
-            requirements.ListRequirement(
-                name="pid",
-                description="Filter on specific process IDs",
-                element_type=int,
-                optional=True,
+            requirements.PluginRequirement(
+                name="driverscan", plugin=driverscan.DriverScan, version=(1, 0, 0)
             ),
         ]
 
-    def _generator(self, tasks):
-        for task in tasks:
-            process_name = utility.array_to_string(task.p_comm)
-            process_pid = task.p_pid
-
-            for vma in task.get_map_iter():
-                path = vma.get_path(
-                    self.context,
-                    self.context.modules[self.config["kernel"]].symbol_table_name,
-                )
-                if path == "":
-                    path = vma.get_special_path()
+    def _generator(self) -> Iterator[Tuple]:
+        """
+        Attempt to match each driver's start code address to a known kernel module
+        A common rootkit technique is to register drivers from modules that are hidden,
+        which allows us to detect the disconnect between a malicious driver and its hidden module.
+        """
+        kernel = self.context.modules[self.config["kernel"]]
+
+        collection = ssdt.SSDT.build_module_collection(
+            self.context, kernel.layer_name, kernel.symbol_table_name
+        )
+
+        for driver in driverscan.DriverScan.scan_drivers(
+            self.context, kernel.layer_name, kernel.symbol_table_name
+        ):
+            # we do not care about actual symbol names, we just want to know if the driver points to a known module
+            module_symbols = list(
+                collection.get_module_symbols_by_absolute_location(driver.DriverStart)
+            )
+            if not module_symbols:
+                (
+                    driver_name,
+                    service_key,
+                    name,
+                ) = driverscan.DriverScan.get_names_for_driver(driver)
+
+                known_exception = driver_name in KNOWN_DRIVERS
 
                 yield (
                     0,
                     (
-                        process_pid,
-                        process_name,
-                        format_hints.Hex(vma.links.start),
-                        format_hints.Hex(vma.links.end),
-                        vma.get_perms(),
-                        path,
+                        format_hints.Hex(driver.vol.offset),
+                        known_exception,
+                        driver_name,
+                        service_key,
+                        name,
                     ),
                 )
 
-    def run(self):
-        filter_func = pslist.PsList.create_pid_filter(self.config.get("pid", None))
-        list_tasks = pslist.PsList.get_list_tasks(
-            self.config.get("pslist_method", pslist.PsList.pslist_methods[0])
-        )
-
+    def run(self) -> renderers.TreeGrid:
         return renderers.TreeGrid(
             [
-                ("PID", int),
-                ("Process", str),
-                ("Start", format_hints.Hex),
-                ("End", format_hints.Hex),
-                ("Protection", str),
-                ("Map Name", str),
+                ("Offset", format_hints.Hex),
+                ("Known Exception", bool),
+                ("Driver Name", str),
+                ("Service Key", str),
+                ("Alternative Name", str),
             ],
-            self._generator(
-                list_tasks(self.context, self.config["kernel"], filter_func=filter_func)
-            ),
+            self._generator(),
         )
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/psaux.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/psaux.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/pslist.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/pslist.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/pstree.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/pstree.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/socket_filters.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/socket_filters.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/timers.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/timers.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/trustedbsd.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/trustedbsd.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/mac/vfsevents.py` & `volatility3-2.7.0/volatility3/framework/plugins/mac/vfsevents.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/timeliner.py` & `volatility3-2.7.0/volatility3/framework/plugins/timeliner.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/bigpools.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/bigpools.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/cachedump.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/cachedump.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/callbacks.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/callbacks.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/cmdline.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/cmdline.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/crashinfo.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/crashinfo.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/devicetree.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/devicetree.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/dlllist.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/dlllist.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from volatility3.framework import constants, exceptions, interfaces, renderers
 from volatility3.framework.configuration import requirements
 from volatility3.framework.renderers import conversion, format_hints
 from volatility3.framework.symbols import intermed
 from volatility3.framework.symbols.windows.extensions import pe
 from volatility3.plugins import timeliner
-from volatility3.plugins.windows import info, pslist
+from volatility3.plugins.windows import info, pslist, psscan
 
 vollog = logging.getLogger(__name__)
 
 
 class DllList(interfaces.plugins.PluginInterface, timeliner.TimeLinerInterface):
     """Lists the loaded modules in a particular windows memory image."""
 
@@ -33,22 +33,30 @@
                 description="Windows kernel",
                 architectures=["Intel32", "Intel64"],
             ),
             requirements.VersionRequirement(
                 name="pslist", component=pslist.PsList, version=(2, 0, 0)
             ),
             requirements.VersionRequirement(
+                name="psscan", component=psscan.PsScan, version=(1, 1, 0)
+            ),
+            requirements.VersionRequirement(
                 name="info", component=info.Info, version=(1, 0, 0)
             ),
             requirements.ListRequirement(
                 name="pid",
                 element_type=int,
                 description="Process IDs to include (all other processes are excluded)",
                 optional=True,
             ),
+            requirements.IntRequirement(
+                name="offset",
+                description="Process offset in the physical address space",
+                optional=True,
+            ),
             requirements.BooleanRequirement(
                 name="dump",
                 description="Extract listed DLLs",
                 default=False,
                 optional=True,
             ),
         ]
@@ -217,27 +225,39 @@
             )
             yield (description, timeliner.TimeLinerType.CREATED, row_data[6])
 
     def run(self):
         filter_func = pslist.PsList.create_pid_filter(self.config.get("pid", None))
         kernel = self.context.modules[self.config["kernel"]]
 
+        if self.config["offset"]:
+            procs = psscan.PsScan.scan_processes(
+                self.context,
+                kernel.layer_name,
+                kernel.symbol_table_name,
+                filter_func=psscan.PsScan.create_offset_filter(
+                    self.context,
+                    kernel.layer_name,
+                    self.config["offset"],
+                ),
+            )
+        else:
+            procs = pslist.PsList.list_processes(
+                context=self.context,
+                layer_name=kernel.layer_name,
+                symbol_table=kernel.symbol_table_name,
+                filter_func=filter_func,
+            )
+
         return renderers.TreeGrid(
             [
                 ("PID", int),
                 ("Process", str),
                 ("Base", format_hints.Hex),
                 ("Size", format_hints.Hex),
                 ("Name", str),
                 ("Path", str),
                 ("LoadTime", datetime.datetime),
                 ("File output", str),
             ],
-            self._generator(
-                pslist.PsList.list_processes(
-                    context=self.context,
-                    layer_name=kernel.layer_name,
-                    symbol_table=kernel.symbol_table_name,
-                    filter_func=filter_func,
-                )
-            ),
+            self._generator(procs=procs),
         )
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/driverirp.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/driverirp.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,18 @@
                 driver_name = renderers.NotApplicableValue()
 
             for i, address in enumerate(driver.MajorFunction):
                 module_symbols = collection.get_module_symbols_by_absolute_location(
                     address
                 )
 
+                module_found = False
+
                 for module_name, symbol_generator in module_symbols:
+                    module_found = True
                     symbols_found = False
 
                     for symbol in symbol_generator:
                         symbols_found = True
                         yield (
                             0,
                             (
@@ -107,14 +110,27 @@
                                 MAJOR_FUNCTIONS[i],
                                 format_hints.Hex(address),
                                 module_name,
                                 renderers.NotAvailableValue(),
                             ),
                         )
 
+                if not module_found:
+                    yield (
+                        0,
+                        (
+                            format_hints.Hex(driver.vol.offset),
+                            driver_name,
+                            MAJOR_FUNCTIONS[i],
+                            format_hints.Hex(address),
+                            renderers.NotAvailableValue(),
+                            renderers.NotAvailableValue(),
+                        ),
+                    )
+
     def run(self):
         return renderers.TreeGrid(
             [
                 ("Offset", format_hints.Hex),
                 ("Driver Name", str),
                 ("IRP", str),
                 ("Address", format_hints.Hex),
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/drivermodule.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/vadwalk.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,93 @@
-# This file is Copyright 2019 Volatility Foundation and licensed under the Volatility Software License 1.0
+# This file is Copyright 2022 Volatility Foundation and licensed under the Volatility Software License 1.0
 # which is available at https://www.volatilityfoundation.org/license/vsl-v1.0
 #
-from typing import Iterator, List, Tuple
-from volatility3.framework import renderers, interfaces
+
+import logging
+from typing import Generator, Iterator, List, Tuple
+
+from volatility3.framework import interfaces, renderers
 from volatility3.framework.configuration import requirements
+from volatility3.framework.objects import utility
 from volatility3.framework.renderers import format_hints
-from volatility3.plugins.windows import ssdt, driverscan
+from volatility3.plugins.windows import pslist, vadinfo
 
-# built in Windows-components that trigger false positives
-KNOWN_DRIVERS = ["ACPI_HAL", "PnpManager", "RAW", "WMIxWDM", "Win32k", "Fs_Rec"]
+vollog = logging.getLogger(__name__)
 
 
-class DriverModule(interfaces.plugins.PluginInterface):
-    """Determines if any loaded drivers were hidden by a rootkit"""
+class VadWalk(interfaces.plugins.PluginInterface):
+    """Walk the VAD tree."""
 
     _required_framework_version = (2, 0, 0)
     _version = (1, 0, 0)
 
     @classmethod
     def get_requirements(cls) -> List[interfaces.configuration.RequirementInterface]:
         return [
             requirements.ModuleRequirement(
                 name="kernel",
                 description="Windows kernel",
                 architectures=["Intel32", "Intel64"],
             ),
             requirements.PluginRequirement(
-                name="ssdt", plugin=ssdt.SSDT, version=(1, 0, 0)
+                name="pslist", plugin=pslist.PsList, version=(2, 0, 0)
             ),
             requirements.PluginRequirement(
-                name="driverscan", plugin=driverscan.DriverScan, version=(1, 0, 0)
+                name="vadinfo", plugin=vadinfo.VadInfo, version=(2, 0, 0)
+            ),
+            requirements.ListRequirement(
+                name="pid",
+                element_type=int,
+                description="Process IDs to include (all other processes are excluded)",
+                optional=True,
             ),
         ]
 
-    def _generator(self) -> Iterator[Tuple]:
-        """
-        Attempt to match each driver's start code address to a known kernel module
-        A common rootkit technique is to register drivers from modules that are hidden,
-        which allows us to detect the disconnect between a malicious driver and its hidden module.
-        """
-        kernel = self.context.modules[self.config["kernel"]]
-
-        collection = ssdt.SSDT.build_module_collection(
-            self.context, kernel.layer_name, kernel.symbol_table_name
-        )
-
-        for driver in driverscan.DriverScan.scan_drivers(
-            self.context, kernel.layer_name, kernel.symbol_table_name
-        ):
-            # we do not care about actual symbol names, we just want to know if the driver points to a known module
-            module_symbols = list(
-                collection.get_module_symbols_by_absolute_location(driver.DriverStart)
-            )
-            if not module_symbols:
-                (
-                    driver_name,
-                    service_key,
-                    name,
-                ) = driverscan.DriverScan.get_names_for_driver(driver)
-
-                known_exception = driver_name in KNOWN_DRIVERS
-
-                yield (
-                    0,
-                    (
-                        format_hints.Hex(driver.vol.offset),
-                        known_exception,
-                        driver_name,
-                        service_key,
-                        name,
-                    ),
-                )
+    def _generator(
+        self, procs: Generator[interfaces.objects.ObjectInterface, None, None]
+    ) -> Iterator[Tuple]:
+        for proc in procs:
+            for vad in vadinfo.VadInfo.list_vads(proc):
+                if vad:
+                    yield (
+                        0,
+                        (
+                            proc.UniqueProcessId,
+                            utility.array_to_string(proc.ImageFileName),
+                            format_hints.Hex(vad.vol.offset),
+                            format_hints.Hex(
+                                vad.get_parent()
+                                & self.context.layers[vad.vol.layer_name].address_mask
+                            ),
+                            format_hints.Hex(vad.get_left_child()),
+                            format_hints.Hex(vad.get_right_child()),
+                            format_hints.Hex(vad.get_start()),
+                            format_hints.Hex(vad.get_end()),
+                            vad.get_tag(),
+                        ),
+                    )
 
     def run(self) -> renderers.TreeGrid:
+        kernel = self.context.modules[self.config["kernel"]]
+        filter_func = pslist.PsList.create_pid_filter(self.config.get("pid", None))
+
         return renderers.TreeGrid(
             [
+                ("PID", int),
+                ("Process", str),
                 ("Offset", format_hints.Hex),
-                ("Known Exception", bool),
-                ("Driver Name", str),
-                ("Service Key", str),
-                ("Alternative Name", str),
+                ("Parent", format_hints.Hex),
+                ("Left", format_hints.Hex),
+                ("Right", format_hints.Hex),
+                ("Start", format_hints.Hex),
+                ("End", format_hints.Hex),
+                ("Tag", str),
             ],
-            self._generator(),
+            self._generator(
+                pslist.PsList.list_processes(
+                    context=self.context,
+                    layer_name=kernel.layer_name,
+                    symbol_table=kernel.symbol_table_name,
+                    filter_func=filter_func,
+                )
+            ),
         )
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/driverscan.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/driverscan.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/dumpfiles.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/dumpfiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file is Copyright 2020 Volatility Foundation and licensed under the Volatility Software License 1.0
 # which is available at https://www.volatilityfoundation.org/license/vsl-v1.0
 #
 
 import logging
 import ntpath
+import re
 from typing import List, Tuple, Type, Optional, Generator
 
 from volatility3.framework import interfaces, renderers, exceptions, constants
 from volatility3.framework.configuration import requirements
-from volatility3.framework.renderers import format_hints
+from volatility3.framework.renderers import format_hints, UnreadableValue
 from volatility3.plugins.windows import handles
 from volatility3.plugins.windows import pslist
 
 vollog = logging.getLogger(__name__)
 
 FILE_DEVICE_DISK = 0x7
 FILE_DEVICE_NETWORK_FILE_SYSTEM = 0x14
@@ -49,14 +50,25 @@
                 optional=True,
             ),
             requirements.IntRequirement(
                 name="physaddr",
                 description="Dump a single _FILE_OBJECT at this physical address",
                 optional=True,
             ),
+            requirements.StringRequirement(
+                name="filter",
+                description="Dump files matching regular expression FILTER",
+                optional=True,
+            ),
+            requirements.BooleanRequirement(
+                name="ignore-case",
+                description="Ignore case in filter match",
+                default=False,
+                optional=True,
+            ),
             requirements.VersionRequirement(
                 name="pslist", component=pslist.PsList, version=(2, 0, 0)
             ),
             requirements.VersionRequirement(
                 name="handles", component=handles.Handles, version=(1, 0, 0)
             ),
         ]
@@ -204,14 +216,18 @@
                     obj_name
                 ),  # temporary, so its easier to visualize output
                 file_output,
             )
 
     def _generator(self, procs: List, offsets: List):
         kernel = self.context.modules[self.config["kernel"]]
+        file_re = None
+        if self.config["filter"]:
+            flags = re.I if self.config["ignore-case"] else 0
+            file_re = re.compile(self.config["filter"], flags)
 
         if procs:
             # The handles plugin doesn't expose any staticmethod/classmethod, and it also requires stashing
             # private variables, so we need an instance (for now, anyway). We _could_ call Handles._generator()
             # to do some of the other work that is duplicated here, but then we'd need to parse the TreeGrid
             # results instead of just dealing with them as direct objects here.
             handles_plugin = handles.Handles(
@@ -239,14 +255,22 @@
                     continue
 
                 for entry in handles_plugin.handles(object_table):
                     try:
                         obj_type = entry.get_object_type(type_map, cookie)
                         if obj_type == "File":
                             file_obj = entry.Body.cast("_FILE_OBJECT")
+
+                            if file_re:
+                                name = file_obj.file_name_with_device()
+                                if isinstance(name, UnreadableValue):
+                                    continue
+                                if not file_re.search(name):
+                                    continue
+
                             for result in self.process_file_object(
                                 self.context, kernel.layer_name, self.open, file_obj
                             ):
                                 yield (0, result)
                     except exceptions.InvalidAddressException:
                         vollog.log(
                             constants.LOGLEVEL_VVV,
@@ -268,14 +292,21 @@
                             )
                         else:
                             continue
 
                         if not file_obj.is_valid():
                             continue
 
+                        if file_re:
+                            name = file_obj.file_name_with_device()
+                            if isinstance(name, UnreadableValue):
+                                continue
+                            if not file_re.search(name):
+                                continue
+
                         for result in self.process_file_object(
                             self.context, kernel.layer_name, self.open, file_obj
                         ):
                             yield (0, result)
                     except exceptions.InvalidAddressException:
                         vollog.log(
                             constants.LOGLEVEL_VVV,
@@ -311,14 +342,19 @@
     def run(self):
         # a list of tuples (<int>, <bool>) where <int> is the address and <bool> is True for virtual.
         offsets = list()
         # a list of processes matching the pid filter. all files for these process(es) will be dumped.
         procs = list()
         kernel = self.context.modules[self.config["kernel"]]
 
+        if self.config["filter"] and (
+            self.config["virtaddr"] or self.config["physaddr"]
+        ):
+            raise ValueError("Cannot use filter flag with an address flag")
+
         if self.config.get("virtaddr", None) is not None:
             offsets.append((self.config["virtaddr"], True))
         elif self.config.get("physaddr", None) is not None:
             offsets.append((self.config["physaddr"], False))
         else:
             filter_func = pslist.PsList.create_pid_filter(
                 [self.config.get("pid", None)]
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/envars.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/envars.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/filescan.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/filescan.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/getservicesids.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/getservicesids.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/getsids.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/getsids.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/handles.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/handles.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 from typing import List, Optional, Dict
 
 from volatility3.framework import constants, exceptions, renderers, interfaces, symbols
 from volatility3.framework.configuration import requirements
 from volatility3.framework.objects import utility
 from volatility3.framework.renderers import format_hints
-from volatility3.plugins.windows import pslist
+from volatility3.plugins.windows import pslist, psscan
 
 vollog = logging.getLogger(__name__)
 
 try:
     import capstone
 
     has_capstone = True
@@ -39,22 +39,30 @@
         # Since we're calling the plugin, make sure we have the plugin's requirements
         return [
             requirements.ModuleRequirement(
                 name="kernel",
                 description="Windows kernel",
                 architectures=["Intel32", "Intel64"],
             ),
+            requirements.PluginRequirement(
+                name="pslist", plugin=pslist.PsList, version=(2, 0, 0)
+            ),
+            requirements.VersionRequirement(
+                name="psscan", component=psscan.PsScan, version=(1, 1, 0)
+            ),
             requirements.ListRequirement(
                 name="pid",
                 element_type=int,
                 description="Process IDs to include (all other processes are excluded)",
                 optional=True,
             ),
-            requirements.PluginRequirement(
-                name="pslist", plugin=pslist.PsList, version=(2, 0, 0)
+            requirements.IntRequirement(
+                name="offset",
+                description="Process offset in the physical address space",
+                optional=True,
             ),
         ]
 
     def _decode_pointer(self, value, magic):
         """Windows encodes pointers to objects and decodes them on the fly
         before using them.
 
@@ -412,26 +420,38 @@
                     ),
                 )
 
     def run(self):
         filter_func = pslist.PsList.create_pid_filter(self.config.get("pid", None))
         kernel = self.context.modules[self.config["kernel"]]
 
+        if self.config["offset"]:
+            procs = psscan.PsScan.scan_processes(
+                self.context,
+                kernel.layer_name,
+                kernel.symbol_table_name,
+                filter_func=psscan.PsScan.create_offset_filter(
+                    self.context,
+                    kernel.layer_name,
+                    self.config["offset"],
+                ),
+            )
+        else:
+            procs = pslist.PsList.list_processes(
+                context=self.context,
+                layer_name=kernel.layer_name,
+                symbol_table=kernel.symbol_table_name,
+                filter_func=filter_func,
+            )
+
         return renderers.TreeGrid(
             [
                 ("PID", int),
                 ("Process", str),
                 ("Offset", format_hints.Hex),
                 ("HandleValue", format_hints.Hex),
                 ("Type", str),
                 ("GrantedAccess", format_hints.Hex),
                 ("Name", str),
             ],
-            self._generator(
-                pslist.PsList.list_processes(
-                    self.context,
-                    kernel.layer_name,
-                    kernel.symbol_table_name,
-                    filter_func=filter_func,
-                )
-            ),
+            self._generator(procs=procs),
         )
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/hashdump.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/hashdump.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/info.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/info.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/joblinks.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/joblinks.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/ldrmodules.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/ldrmodules.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/lsadump.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/lsadump.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/malfind.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/malfind.py`

 * *Files 5% similar despite different names*

```diff
@@ -137,24 +137,38 @@
                 data = proc_layer.read(vad.get_start(), 64, pad=True)
                 yield vad, data
 
     def _generator(self, procs):
         # determine if we're on a 32 or 64 bit kernel
         kernel = self.context.modules[self.config["kernel"]]
 
+        # set refined criteria to know when to add to "Notes" column
+        refined_criteria = {
+            b"MZ": "MZ header",
+            b"\x55\x8B": "PE header",
+            b"\x55\x48": "Function prologue",
+            b"\x55\x89": "Function prologue",
+        }
+
         is_32bit_arch = not symbols.symbol_table_is_64bit(
             self.context, kernel.symbol_table_name
         )
 
         for proc in procs:
+            # by default, "Notes" column will be set to N/A
+            notes = renderers.NotApplicableValue()
             process_name = utility.array_to_string(proc.ImageFileName)
 
             for vad, data in self.list_injections(
                 self.context, kernel.layer_name, kernel.symbol_table_name, proc
             ):
+                # Check for unique headers and update "Notes" column if criteria is met
+                if data[0:2] in refined_criteria:
+                    notes = refined_criteria[data[0:2]]
+
                 # if we're on a 64 bit kernel, we may still need 32 bit disasm due to wow64
                 if is_32bit_arch or proc.get_is_wow64():
                     architecture = "intel"
                 else:
                     architecture = "intel64"
 
                 disasm = interfaces.renderers.Disassembly(
@@ -192,14 +206,15 @@
                                 kernel.symbol_table_name,
                             ),
                             vadinfo.winnt_protections,
                         ),
                         vad.get_commit_charge(),
                         vad.get_private_memory(),
                         file_output,
+                        notes,
                         format_hints.HexBytes(data),
                         disasm,
                     ),
                 )
 
     def run(self):
         filter_func = pslist.PsList.create_pid_filter(self.config.get("pid", None))
@@ -212,14 +227,15 @@
                 ("Start VPN", format_hints.Hex),
                 ("End VPN", format_hints.Hex),
                 ("Tag", str),
                 ("Protection", str),
                 ("CommitCharge", int),
                 ("PrivateMemory", int),
                 ("File output", str),
+                ("Notes", str),
                 ("Hexdump", format_hints.HexBytes),
                 ("Disasm", interfaces.renderers.Disassembly),
             ],
             self._generator(
                 pslist.PsList.list_processes(
                     context=self.context,
                     layer_name=kernel.layer_name,
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/mbrscan.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/mbrscan.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/memmap.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/memmap.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/mftscan.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/mftscan.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,30 +34,29 @@
         ]
 
     def _generator(self):
         layer = self.context.layers[self.config["primary"]]
 
         # Yara Rule to scan for MFT Header Signatures
         rules = yarascan.YaraScan.process_yara_options(
-            {"yara_rules": "/FILE0|FILE\*|BAAD/"}
+            {"yara_rules": "/FILE0|FILE\\*|BAAD/"}
         )
 
         # Read in the Symbol File
         symbol_table = intermed.IntermediateSymbolTable.create(
             context=self.context,
             config_path=self.config_path,
             sub_path="windows",
             filename="mft",
             class_types={"FILE_NAME_ENTRY": mft.MFTFileName, "MFT_ENTRY": mft.MFTEntry},
         )
 
         # get each of the individual Field Sets
         mft_object = symbol_table + constants.BANG + "MFT_ENTRY"
         attribute_object = symbol_table + constants.BANG + "ATTRIBUTE"
-        header_object = symbol_table + constants.BANG + "ATTR_HEADER"
         si_object = symbol_table + constants.BANG + "STANDARD_INFORMATION_ENTRY"
         fn_object = symbol_table + constants.BANG + "FILE_NAME_ENTRY"
 
         # Scan the layer for Raw MFT records and parse the fields
         for offset, _rule_name, _name, _value in layer.scan(
             context=self.context, scanner=yarascan.YaraScanner(rules=rules)
         ):
@@ -194,15 +193,15 @@
         ]
 
     def _generator(self):
         layer = self.context.layers[self.config["primary"]]
 
         # Yara Rule to scan for MFT Header Signatures
         rules = yarascan.YaraScan.process_yara_options(
-            {"yara_rules": "/FILE0|FILE\*|BAAD/"}
+            {"yara_rules": "/FILE0|FILE\\*|BAAD/"}
         )
 
         # Read in the Symbol File
         symbol_table = intermed.IntermediateSymbolTable.create(
             context=self.context,
             config_path=self.config_path,
             sub_path="windows",
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/modscan.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/modscan.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/modules.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/modules.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/mutantscan.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/mutantscan.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/netscan.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/netscan.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/netstat.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/netstat.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/poolscanner.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/poolscanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,32 @@
             ),
             # processes on windows starting with windows 8
             PoolConstraint(
                 b"Proc",
                 type_name=symbol_table + constants.BANG + "_EPROCESS",
                 object_type="Process",
                 size=(600, None),
+                skip_type_test=True,
+                page_type=PoolType.PAGED | PoolType.NONPAGED | PoolType.FREE,
+            ),
+            # threads on windows before windows8
+            PoolConstraint(
+                b"Thr\xe5",  # -> “protected” allocation, MSB is set.
+                type_name=symbol_table + constants.BANG + "_ETHREAD",
+                object_type="Thread",
+                size=(600, None),  # -> 0x0258 - size of struct in win5.1
+                skip_type_test=True,
+                page_type=PoolType.PAGED | PoolType.NONPAGED | PoolType.FREE,
+            ),
+            # threads on windows starting with windows8
+            PoolConstraint(
+                b"Thre",
+                type_name=symbol_table + constants.BANG + "_ETHREAD",
+                object_type="Thread",
+                size=(600, None),  # -> 0x0258 - size of struct in win5.1
                 page_type=PoolType.PAGED | PoolType.NONPAGED | PoolType.FREE,
             ),
             # files on windows before windows 8
             PoolConstraint(
                 b"Fil\xe5",
                 type_name=symbol_table + constants.BANG + "_FILE_OBJECT",
                 object_type="File",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/privileges.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/privileges.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/pslist.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/pslist.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/psscan.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/psscan.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,14 +56,83 @@
                 description="Display physical offset instead of virtual",
                 default=False,
                 optional=True,
             ),
         ]
 
     @classmethod
+    def physical_offset_from_virtual(cls, context, layer_name, proc):
+        """Calculate the physical offset from the virtual offset of a process.
+
+        Args:
+            context: The context containing layers and modules information.
+            layer_name: The name of the layer containing the process memory.
+            proc: The process object for which to calculate the physical offset.
+
+        Returns:
+            int: The physical offset of the process.
+        Raises:
+            TypeError: If the primary layer is not an Intel layer.
+        """
+        memory = context.layers[layer_name]
+
+        if not isinstance(memory, layers.intel.Intel):
+            raise TypeError("Primary layer is not an intel layer")
+
+        (_, _, ph_offset, _, _) = list(
+            memory.mapping(offset=proc.vol.offset, length=0)
+        )[0]
+
+        return ph_offset
+
+    @classmethod
+    def create_offset_filter(
+        cls,
+        context: interfaces.context.ContextInterface,
+        layer_name: str,
+        offset: int = None,
+        physical: bool = True,
+        exclude: bool = False,
+    ) -> Callable[[interfaces.objects.ObjectInterface], bool]:
+        """A factory for producing filter functions that filter based on the physical offset of the process.
+
+        Args:
+            offset: A number that is the physical offset to be filtered out
+            exclude: Accept only tasks that are not the offset argument
+
+        Returns:
+            Filter function to be passed to the list of processes.
+        """
+        filter_func = lambda _: False
+
+        if offset:
+            if physical:
+                if exclude:
+                    filter_func = (
+                        lambda proc: cls.physical_offset_from_virtual(
+                            context, layer_name, proc
+                        )
+                        == offset
+                    )
+                else:
+                    filter_func = (
+                        lambda proc: cls.physical_offset_from_virtual(
+                            context, layer_name, proc
+                        )
+                        != offset
+                    )
+            else:
+                if exclude:
+                    filter_func = lambda proc: proc.vol.offset == offset
+                else:
+                    filter_func = lambda proc: proc.vol.offset != offset
+
+        return filter_func
+
+    @classmethod
     def scan_processes(
         cls,
         context: interfaces.context.ContextInterface,
         layer_name: str,
         symbol_table: str,
         filter_func: Callable[
             [interfaces.objects.ObjectInterface], bool
```

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/registry/hivelist.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/registry/hivelist.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/registry/hivescan.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/registry/hivescan.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/registry/printkey.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/registry/printkey.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/registry/userassist.json` & `volatility3-2.7.0/volatility3/framework/plugins/windows/registry/userassist.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/registry/userassist.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/registry/userassist.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/sessions.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/sessions.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/sids_and_privileges.json` & `volatility3-2.7.0/volatility3/framework/plugins/windows/sids_and_privileges.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/skeleton_key_check.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/skeleton_key_check.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/ssdt.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/ssdt.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/strings.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/strings.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/symlinkscan.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/symlinkscan.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/vadinfo.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/vadinfo.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/vadyarascan.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/vadyarascan.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/verinfo.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/verinfo.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/windows/virtmap.py` & `volatility3-2.7.0/volatility3/framework/plugins/windows/virtmap.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/plugins/yarascan.py` & `volatility3-2.7.0/volatility3/framework/plugins/yarascan.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/renderers/__init__.py` & `volatility3-2.7.0/volatility3/framework/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/renderers/conversion.py` & `volatility3-2.7.0/volatility3/framework/renderers/conversion.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/renderers/format_hints.py` & `volatility3-2.7.0/volatility3/framework/renderers/format_hints.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/__init__.py` & `volatility3-2.7.0/volatility3/framework/symbols/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 # This file is Copyright 2019 Volatility Foundation and licensed under the Volatility Software License 1.0
 # which is available at https://www.volatilityfoundation.org/license/vsl-v1.0
 #
 
 import collections
 import collections.abc
+import datetime
 import enum
 import logging
-from typing import Any, Dict, Iterable, Iterator, TypeVar, List
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Iterator,
+    Optional,
+    Tuple,
+    TypeVar,
+    List,
+)
 
 from volatility3.framework import constants, exceptions, interfaces, objects
 
 vollog = logging.getLogger(__name__)
 
 SymbolSpaceReturnType = TypeVar(
     "SymbolSpaceReturnType",
@@ -109,14 +120,50 @@
 
     def remove(self, key: str) -> None:
         """Removes a named symbol_list from the space."""
         # Reset the resolved list, since we're removing some symbols
         self._resolved = {}
         del self._dict[key]
 
+    def verify_table_versions(
+        self,
+        producer: str,
+        validator: Callable[[Optional[Tuple], Optional[datetime.datetime]], bool],
+        tables: List[str] = None,
+    ) -> bool:
+        """Verifies the producer metadata and version of tables
+
+        Args:
+            producer: String name of a table producer to have validation performed
+            validator: callable that takes an optional version and an optional datetime that returns False if table is invalid
+
+        Returns:
+            False if an invalid table was found or True if no invalid table was found
+        """
+        if tables is None:
+            tables = self._dict.keys()
+        for table_name in tables:
+            table = self._dict[table_name]
+            if not table.producer:
+                vollog.debug(
+                    f"Symbol table {table_name} could not be validated because no producer metadata was found"
+                )
+                continue
+            if table.producer.name == producer:
+                # Run the verification
+                if not validator(
+                    table.producer.version,
+                    table.producer.datetime,
+                ):
+                    vollog.debug(f"Symbol table {table_name} does not pass validator")
+                    return False
+            else:
+                continue
+        return True
+
     ### Resolution functions
 
     class UnresolvedTemplate(objects.templates.ReferenceTemplate):
         """Class to highlight when missing symbols are present.
 
         This class is identical to a reference template, but differentiable by its classname.
         It will output a debug log to indicate when it has been instantiated and with what name.
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/generic/__init__.py` & `volatility3-2.7.0/volatility3/framework/symbols/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/generic/qemu.json` & `volatility3-2.7.0/volatility3/framework/symbols/generic/qemu.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/intermed.py` & `volatility3-2.7.0/volatility3/framework/symbols/intermed.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,15 @@
             )
         return versions[max(supported_versions)]
 
     symbols = _construct_delegate_function("symbols", True)
     types = _construct_delegate_function("types", True)
     enumerations = _construct_delegate_function("enumerations", True)
     metadata = _construct_delegate_function("metadata", True)
+    producer = _construct_delegate_function("producer", True)
     clear_symbol_cache = _construct_delegate_function("clear_symbol_cache")
     get_type = _construct_delegate_function("get_type")
     get_symbol = _construct_delegate_function("get_symbol")
     get_enumeration = _construct_delegate_function("get_enumeration")
     get_type_class = _construct_delegate_function("get_type_class")
     set_type_class = _construct_delegate_function("set_type_class")
     del_type_class = _construct_delegate_function("del_type_class")
@@ -368,14 +369,22 @@
 
     @property
     def metadata(self) -> Optional[interfaces.symbols.MetadataInterface]:
         """Returns a metadata object containing information about the symbol
         table."""
         return None
 
+    @property
+    def producer(self) -> Optional["metadata.ProducerMetadata"]:
+        """Returns a metadata object containing information about the symbol
+        table."""
+        return metadata.ProducerMetadata(
+            self._json_object.get("metadata", {}).get("producer", {})
+        )
+
     def clear_symbol_cache(self) -> None:
         """Clears the symbol cache of the symbol table."""
         self._symbol_cache.clear()
 
 
 class Version1Format(ISFormatTable):
     """Class for storing intermediate debugging data as objects and classes."""
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/linux/__init__.py` & `volatility3-2.7.0/volatility3/framework/symbols/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/linux/bash32.json` & `volatility3-2.7.0/volatility3/framework/symbols/linux/bash32.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/linux/bash64.json` & `volatility3-2.7.0/volatility3/framework/symbols/linux/bash64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/linux/elf.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win7-x64.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7160416666666667%*

 * *Differences: {"'base_types'": "{'long': {'signed': False}, 'pointer': OrderedDict([('kind', 'int'), ('size', "*

 * *                 "8), ('signed', False), ('endian', 'little')]), 'unsigned int': "*

 * *                 "OrderedDict([('kind', 'int'), ('size', 4), ('signed', False), ('endian', "*

 * *                 "'little')]), 'unsigned be short': OrderedDict([('kind', 'int'), ('size', 2), "*

 * *                 "('signed', False), ('endian', 'big')]), delete: ['char', 'unsigned long long']}",*

 * * "'enums'": "{replace: OrderedDict([('TCP […]*

```diff
@@ -1,965 +1,715 @@
 {
     "base_types": {
-        "char": {
-            "endian": "little",
-            "kind": "char",
-            "signed": true,
-            "size": 1
-        },
         "long": {
             "endian": "little",
             "kind": "int",
-            "signed": true,
+            "signed": false,
             "size": 4
         },
         "long long": {
             "endian": "little",
             "kind": "int",
             "signed": true,
             "size": 8
         },
+        "pointer": {
+            "endian": "little",
+            "kind": "int",
+            "signed": false,
+            "size": 8
+        },
+        "unsigned be short": {
+            "endian": "big",
+            "kind": "int",
+            "signed": false,
+            "size": 2
+        },
         "unsigned char": {
             "endian": "little",
             "kind": "char",
             "signed": false,
             "size": 1
         },
-        "unsigned long": {
+        "unsigned int": {
             "endian": "little",
             "kind": "int",
             "signed": false,
             "size": 4
         },
-        "unsigned long long": {
+        "unsigned long": {
             "endian": "little",
             "kind": "int",
             "signed": false,
-            "size": 8
+            "size": 4
         },
         "unsigned short": {
             "endian": "little",
             "kind": "int",
             "signed": false,
             "size": 2
         }
     },
     "enums": {
-        "EtypeEnum": {
-            "base": "unsigned short",
+        "TCPStateEnum": {
+            "base": "long",
             "constants": {
-                "ET_CORE": 4,
-                "ET_DYN": 3,
-                "ET_EXEC": 2,
-                "ET_HIPROC": 65535,
-                "ET_LOPROC": 65280,
-                "ET_NONE": 0,
-                "ET_REL": 1
-            },
-            "size": 2
-        },
-        "PtypeEnum": {
-            "base": "unsigned long",
-            "constants": {
-                "PT_DYNAMIC": 2,
-                "PT_HIOS": 1879048191,
-                "PT_HIPROC": 2147483647,
-                "PT_INTERP": 3,
-                "PT_LOAD": 1,
-                "PT_LOOS": 1610612736,
-                "PT_LOWPROC": 1879048192,
-                "PT_NOTE": 4,
-                "PT_NULL": 0,
-                "PT_PHDR": 6,
-                "PT_SHLIB": 5,
-                "PT_TLS": 7
+                "CLOSED": 0,
+                "CLOSE_WAIT": 7,
+                "CLOSING": 8,
+                "DELETE_TCB": 13,
+                "ESTABLISHED": 4,
+                "FIN_WAIT1": 5,
+                "FIN_WAIT2": 6,
+                "LAST_ACK": 9,
+                "LISTENING": 1,
+                "SYN_RCVD": 3,
+                "SYN_SENT": 2,
+                "TIME_WAIT": 12
             },
             "size": 4
         }
     },
     "metadata": {
-        "format": "6.1.0",
+        "format": "6.0.0",
         "producer": {
-            "datetime": "2019-10-21T22:52:00",
-            "name": "ikelos-by-hand",
+            "datetime": "2020-06-12T14:00:00",
+            "name": "japhlange-by-hand",
             "version": "0.0.1"
         }
     },
     "symbols": {},
     "user_types": {
-        "Elf": {
+        "_ADDRINFO": {
             "fields": {
-                "e_ident": {
+                "Local": {
                     "offset": 0,
                     "type": {
-                        "count": 16,
-                        "kind": "array",
+                        "kind": "pointer",
                         "subtype": {
-                            "kind": "base",
-                            "name": "unsigned char"
+                            "kind": "struct",
+                            "name": "_LOCAL_ADDRESS"
+                        }
+                    }
+                },
+                "Remote": {
+                    "offset": 16,
+                    "type": {
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_IN_ADDR"
                         }
                     }
                 }
             },
             "kind": "struct",
-            "size": 16
+            "size": 24
         },
-        "Elf32_Dyn": {
+        "_INETAF": {
             "fields": {
-                "d_ptr": {
-                    "offset": 4,
+                "AddressFamily": {
+                    "offset": 20,
                     "type": {
                         "kind": "base",
-                        "name": "unsigned long"
+                        "name": "unsigned short"
                     }
-                },
-                "d_tag": {
-                    "offset": 0,
+                }
+            },
+            "kind": "struct",
+            "size": 22
+        },
+        "_INET_COMPARTMENT": {
+            "fields": {
+                "ProtocolCompartment": {
+                    "offset": 32,
                     "type": {
-                        "kind": "base",
-                        "name": "long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_PROTOCOL_COMPARTMENT"
+                        }
                     }
                 }
             },
             "kind": "struct",
-            "size": 8
+            "size": 48
         },
-        "Elf32_Ehdr": {
+        "_INET_COMPARTMENT_SET": {
             "fields": {
-                "e_ehsize": {
-                    "offset": 40,
+                "InetCompartment": {
+                    "offset": 328,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_INET_COMPARTMENT"
+                        }
                     }
-                },
-                "e_entry": {
-                    "offset": 24,
+                }
+            },
+            "kind": "struct",
+            "size": 384
+        },
+        "_INET_PORT_POOL": {
+            "fields": {
+                "PortAssignments": {
+                    "offset": 160,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "count": 256,
+                        "kind": "array",
+                        "subtype": {
+                            "kind": "pointer",
+                            "subtype": {
+                                "kind": "struct",
+                                "name": "_PORT_ASSIGNMENT"
+                            }
+                        }
                     }
                 },
-                "e_flags": {
-                    "offset": 36,
+                "PortBitMap": {
+                    "offset": 144,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "kind": "struct",
+                        "name": "nt_symbols!_RTL_BITMAP"
                     }
-                },
-                "e_ident": {
+                }
+            },
+            "kind": "struct",
+            "size": 11200
+        },
+        "_IN_ADDR": {
+            "fields": {
+                "addr4": {
                     "offset": 0,
                     "type": {
-                        "count": 16,
+                        "count": 4,
                         "kind": "array",
                         "subtype": {
                             "kind": "base",
                             "name": "unsigned char"
                         }
                     }
                 },
-                "e_machine": {
-                    "offset": 18,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
-                    }
-                },
-                "e_phentsize": {
-                    "offset": 42,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
-                    }
-                },
-                "e_phnum": {
-                    "offset": 44,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
-                    }
-                },
-                "e_phoff": {
-                    "offset": 28,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "e_shentsize": {
-                    "offset": 46,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
-                    }
-                },
-                "e_shnum": {
-                    "offset": 48,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
-                    }
-                },
-                "e_shoff": {
-                    "offset": 32,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "e_shstrndx": {
-                    "offset": 50,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
-                    }
-                },
-                "e_type": {
-                    "offset": 16,
-                    "type": {
-                        "kind": "enum",
-                        "name": "EtypeEnum"
-                    }
-                },
-                "e_version": {
-                    "offset": 20,
+                "addr6": {
+                    "offset": 0,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "count": 16,
+                        "kind": "array",
+                        "subtype": {
+                            "kind": "base",
+                            "name": "unsigned char"
+                        }
                     }
                 }
             },
             "kind": "struct",
-            "size": 52
+            "size": 6
         },
-        "Elf32_LinkMap": {
+        "_LARGE_INTEGER": {
             "fields": {
-                "l_addr": {
-                    "offset": 0,
+                "HighPart": {
+                    "offset": 4,
                     "type": {
                         "kind": "base",
-                        "name": "unsigned long"
+                        "name": "long"
                     }
                 },
-                "l_ld": {
-                    "offset": 8,
+                "LowPart": {
+                    "offset": 0,
                     "type": {
                         "kind": "base",
                         "name": "unsigned long"
                     }
                 },
-                "l_name": {
-                    "offset": 4,
+                "QuadPart": {
+                    "offset": 0,
                     "type": {
                         "kind": "base",
-                        "name": "unsigned long"
+                        "name": "long long"
                     }
                 },
-                "l_next": {
-                    "offset": 12,
+                "u": {
+                    "offset": 0,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "kind": "struct",
+                        "name": "__unnamed_2"
                     }
-                },
-                "l_prev": {
+                }
+            },
+            "kind": "union",
+            "size": 8
+        },
+        "_LOCAL_ADDRESS": {
+            "fields": {
+                "pData": {
                     "offset": 16,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "pointer",
+                            "subtype": {
+                                "kind": "struct",
+                                "name": "_IN_ADDR"
+                            }
+                        }
                     }
                 }
             },
             "kind": "struct",
-            "size": 20
+            "size": 24
         },
-        "Elf32_Note": {
+        "_PARTITION": {
             "fields": {
-                "n_descsz": {
-                    "offset": 4,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "n_namesz": {
-                    "offset": 0,
+                "Endpoints": {
+                    "offset": 8,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "nt_symbols!_RTL_DYNAMIC_HASH_TABLE"
+                        }
                     }
                 },
-                "n_type": {
-                    "offset": 8,
+                "UnknownHashTable": {
+                    "offset": 16,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "nt_symbols!_RTL_DYNAMIC_HASH_TABLE"
+                        }
                     }
                 }
             },
             "kind": "struct",
-            "size": 12
+            "size": 128
         },
-        "Elf32_Phdr": {
+        "_PARTITION_TABLE": {
             "fields": {
-                "p_align": {
-                    "offset": 28,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "p_filesz": {
-                    "offset": 16,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "p_flags": {
-                    "offset": 24,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "p_memsz": {
-                    "offset": 20,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "p_offset": {
-                    "offset": 4,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "p_paddr": {
-                    "offset": 12,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "p_type": {
+                "Partitions": {
                     "offset": 0,
                     "type": {
-                        "kind": "enum",
-                        "name": "PtypeEnum"
-                    }
-                },
-                "p_vaddr": {
-                    "offset": 8,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "count": 1,
+                        "kind": "array",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_PARTITION"
+                        }
                     }
                 }
             },
             "kind": "struct",
-            "size": 32
+            "size": 128
         },
-        "Elf32_Rel": {
+        "_PORT_ASSIGNMENT": {
             "fields": {
-                "r_info": {
-                    "offset": 4,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "r_offset": {
-                    "offset": 0,
+                "InPaBigPoolBase": {
+                    "offset": 32,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_PORT_ASSIGNMENT_LIST"
+                        }
                     }
                 }
             },
             "kind": "struct",
-            "size": 8
+            "size": 40
         },
-        "Elf32_Rela": {
+        "_PORT_ASSIGNMENT_ENTRY": {
             "fields": {
-                "r_addend": {
+                "Entry": {
                     "offset": 8,
                     "type": {
-                        "kind": "base",
-                        "name": "long"
-                    }
-                },
-                "r_info": {
-                    "offset": 4,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "r_offset": {
-                    "offset": 0,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "base",
+                            "name": "void"
+                        }
                     }
                 }
             },
             "kind": "struct",
-            "size": 12
+            "size": 16
         },
-        "Elf32_Shdr": {
+        "_PORT_ASSIGNMENT_LIST": {
             "fields": {
-                "sh_addr": {
-                    "offset": 12,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "sh_addralign": {
-                    "offset": 32,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "sh_entsize": {
-                    "offset": 36,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "sh_flags": {
-                    "offset": 8,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "sh_info": {
-                    "offset": 28,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "sh_link": {
-                    "offset": 24,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "sh_name": {
+                "Assignments": {
                     "offset": 0,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "sh_offset": {
-                    "offset": 16,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "sh_size": {
-                    "offset": 20,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "sh_type": {
-                    "offset": 4,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "count": 256,
+                        "kind": "array",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_PORT_ASSIGNMENT_ENTRY"
+                        }
                     }
                 }
             },
             "kind": "struct",
-            "size": 40
+            "size": 4096
         },
-        "Elf32_Sym": {
+        "_PROTOCOL_COMPARTMENT": {
             "fields": {
-                "st_info": {
-                    "offset": 12,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned char"
-                    }
-                },
-                "st_name": {
+                "PortPool": {
                     "offset": 0,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "st_other": {
-                    "offset": 13,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned char"
-                    }
-                },
-                "st_shndx": {
-                    "offset": 14,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
-                    }
-                },
-                "st_size": {
-                    "offset": 8,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
-                    }
-                },
-                "st_value": {
-                    "offset": 4,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_INET_PORT_POOL"
+                        }
                     }
                 }
             },
             "kind": "struct",
             "size": 16
         },
-        "Elf64_Dyn": {
+        "_SYN_OWNER": {
             "fields": {
-                "d_ptr": {
-                    "offset": 8,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
-                    }
-                },
-                "d_tag": {
-                    "offset": 0,
+                "Process": {
+                    "offset": 40,
                     "type": {
-                        "kind": "base",
-                        "name": "long long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "nt_symbols!_EPROCESS"
+                        }
                     }
                 }
             },
             "kind": "struct",
-            "size": 16
+            "size": 48
         },
-        "Elf64_Ehdr": {
+        "_TCP_ENDPOINT": {
             "fields": {
-                "e_ehsize": {
-                    "offset": 52,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
-                    }
-                },
-                "e_entry": {
-                    "offset": 24,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
-                    }
-                },
-                "e_flags": {
-                    "offset": 48,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "e_ident": {
-                    "offset": 0,
+                "AddrInfo": {
+                    "offset": 32,
                     "type": {
-                        "count": 16,
-                        "kind": "array",
+                        "kind": "pointer",
                         "subtype": {
-                            "kind": "base",
-                            "name": "unsigned char"
+                            "kind": "struct",
+                            "name": "_ADDRINFO"
                         }
                     }
                 },
-                "e_machine": {
-                    "offset": 18,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
-                    }
-                },
-                "e_phentsize": {
-                    "offset": 54,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
-                    }
-                },
-                "e_phnum": {
-                    "offset": 56,
+                "CreateTime": {
+                    "offset": 0,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
+                        "kind": "union",
+                        "name": "_LARGE_INTEGER"
                     }
                 },
-                "e_phoff": {
-                    "offset": 32,
+                "InetAF": {
+                    "offset": 24,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_INETAF"
+                        }
                     }
                 },
-                "e_shentsize": {
-                    "offset": 58,
+                "ListEntry": {
+                    "offset": 40,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
+                        "kind": "union",
+                        "name": "nt_symbols!_LIST_ENTRY"
                     }
                 },
-                "e_shnum": {
-                    "offset": 60,
+                "LocalPort": {
+                    "offset": 108,
                     "type": {
                         "kind": "base",
-                        "name": "unsigned short"
+                        "name": "unsigned be short"
                     }
                 },
-                "e_shoff": {
-                    "offset": 40,
+                "Owner": {
+                    "offset": 568,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "nt_symbols!_EPROCESS"
+                        }
                     }
                 },
-                "e_shstrndx": {
-                    "offset": 62,
+                "RemotePort": {
+                    "offset": 110,
                     "type": {
                         "kind": "base",
-                        "name": "unsigned short"
+                        "name": "unsigned be short"
                     }
                 },
-                "e_type": {
-                    "offset": 16,
+                "State": {
+                    "offset": 104,
                     "type": {
                         "kind": "enum",
-                        "name": "EtypeEnum"
-                    }
-                },
-                "e_version": {
-                    "offset": 20,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "name": "TCPStateEnum"
                     }
                 }
             },
             "kind": "struct",
-            "size": 64
+            "size": 576
         },
-        "Elf64_LinkMap": {
+        "_TCP_LISTENER": {
             "fields": {
-                "l_addr": {
-                    "offset": 0,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
-                    }
-                },
-                "l_ld": {
-                    "offset": 16,
+                "CreateTime": {
+                    "offset": 32,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
+                        "kind": "union",
+                        "name": "_LARGE_INTEGER"
                     }
                 },
-                "l_name": {
-                    "offset": 8,
+                "InetAF": {
+                    "offset": 96,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_INETAF"
+                        }
                     }
                 },
-                "l_next": {
-                    "offset": 24,
+                "LocalAddr": {
+                    "offset": 88,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_LOCAL_ADDRESS"
+                        }
                     }
                 },
-                "l_prev": {
-                    "offset": 32,
+                "Next": {
+                    "offset": 112,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 40
-        },
-        "Elf64_Note": {
-            "fields": {
-                "n_descsz": {
-                    "offset": 4,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_TCP_LISTENER"
+                        }
                     }
                 },
-                "n_namesz": {
-                    "offset": 0,
+                "Owner": {
+                    "offset": 40,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "nt_symbols!_EPROCESS"
+                        }
                     }
                 },
-                "n_type": {
-                    "offset": 8,
+                "Port": {
+                    "offset": 106,
                     "type": {
                         "kind": "base",
-                        "name": "unsigned long"
+                        "name": "unsigned be short"
                     }
                 }
             },
             "kind": "struct",
-            "size": 12
+            "size": 108
         },
-        "Elf64_Phdr": {
+        "_TCP_SYN_ENDPOINT": {
             "fields": {
-                "p_align": {
-                    "offset": 48,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
-                    }
-                },
-                "p_filesz": {
-                    "offset": 32,
+                "CreateTime": {
+                    "offset": 0,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
+                        "kind": "union",
+                        "name": "_LARGE_INTEGER"
                     }
                 },
-                "p_flags": {
-                    "offset": 4,
+                "InetAF": {
+                    "offset": 72,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_INETAF"
+                        }
                     }
                 },
-                "p_memsz": {
-                    "offset": 40,
+                "ListEntry": {
+                    "offset": 16,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
+                        "kind": "union",
+                        "name": "nt_symbols!_LIST_ENTRY"
                     }
                 },
-                "p_offset": {
-                    "offset": 8,
+                "LocalAddr": {
+                    "offset": 80,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_LOCAL_ADDRESS"
+                        }
                     }
                 },
-                "p_paddr": {
-                    "offset": 24,
+                "LocalPort": {
+                    "offset": 124,
                     "type": {
                         "kind": "base",
-                        "name": "unsigned long long"
+                        "name": "unsigned be short"
                     }
                 },
-                "p_type": {
-                    "offset": 0,
+                "Owner": {
+                    "offset": 88,
                     "type": {
-                        "kind": "enum",
-                        "name": "PtypeEnum"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_SYN_OWNER"
+                        }
                     }
                 },
-                "p_vaddr": {
-                    "offset": 16,
+                "RemoteAddress": {
+                    "offset": 104,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 56
-        },
-        "Elf64_Rel": {
-            "fields": {
-                "r_info": {
-                    "offset": 8,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_IN_ADDR"
+                        }
                     }
                 },
-                "r_offset": {
-                    "offset": 0,
+                "RemotePort": {
+                    "offset": 126,
                     "type": {
                         "kind": "base",
-                        "name": "unsigned long long"
+                        "name": "unsigned be short"
                     }
                 }
             },
             "kind": "struct",
-            "size": 16
+            "size": 128
         },
-        "Elf64_Rela": {
+        "_TCP_TIMEWAIT_ENDPOINT": {
             "fields": {
-                "r_addend": {
-                    "offset": 16,
-                    "type": {
-                        "kind": "base",
-                        "name": "long long"
-                    }
-                },
-                "r_info": {
-                    "offset": 8,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
-                    }
-                },
-                "r_offset": {
+                "CreateTime": {
                     "offset": 0,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 24
-        },
-        "Elf64_Shdr": {
-            "fields": {
-                "sh_addr": {
-                    "offset": 16,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
+                        "kind": "union",
+                        "name": "_LARGE_INTEGER"
                     }
                 },
-                "sh_addralign": {
+                "InetAF": {
                     "offset": 48,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
-                    }
-                },
-                "sh_entsize": {
-                    "offset": 56,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "sh_flags": {
-                    "offset": 8,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
-                    }
-                },
-                "sh_info": {
-                    "offset": 44,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_INETAF"
+                        }
                     }
                 },
-                "sh_link": {
-                    "offset": 40,
+                "ListEntry": {
+                    "offset": 0,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "kind": "union",
+                        "name": "nt_symbols!_LIST_ENTRY"
                     }
                 },
-                "sh_name": {
-                    "offset": 0,
+                "LocalAddr": {
+                    "offset": 80,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_LOCAL_ADDRESS"
+                        }
                     }
                 },
-                "sh_offset": {
-                    "offset": 24,
+                "LocalPort": {
+                    "offset": 72,
                     "type": {
                         "kind": "base",
-                        "name": "unsigned long long"
+                        "name": "unsigned be short"
                     }
                 },
-                "sh_size": {
-                    "offset": 32,
+                "RemoteAddress": {
+                    "offset": 88,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_IN_ADDR"
+                        }
                     }
                 },
-                "sh_type": {
-                    "offset": 4,
+                "RemotePort": {
+                    "offset": 74,
                     "type": {
                         "kind": "base",
-                        "name": "unsigned long"
+                        "name": "unsigned be short"
                     }
                 }
             },
             "kind": "struct",
-            "size": 64
+            "size": 96
         },
-        "Elf64_Sym": {
+        "_UDP_ENDPOINT": {
             "fields": {
-                "st_info": {
-                    "offset": 4,
+                "CreateTime": {
+                    "offset": 88,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned char"
+                        "kind": "union",
+                        "name": "_LARGE_INTEGER"
                     }
                 },
-                "st_name": {
-                    "offset": 0,
+                "InetAF": {
+                    "offset": 32,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_INETAF"
+                        }
                     }
                 },
-                "st_other": {
-                    "offset": 5,
+                "LocalAddr": {
+                    "offset": 96,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned char"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_LOCAL_ADDRESS"
+                        }
                     }
                 },
-                "st_shndx": {
-                    "offset": 6,
+                "Next": {
+                    "offset": 136,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_UDP_ENDPOINT"
+                        }
                     }
                 },
-                "st_size": {
-                    "offset": 16,
+                "Owner": {
+                    "offset": 40,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned long long"
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "nt_symbols!_EPROCESS"
+                        }
                     }
                 },
-                "st_value": {
-                    "offset": 8,
+                "Port": {
+                    "offset": 128,
                     "type": {
                         "kind": "base",
-                        "name": "unsigned long long"
+                        "name": "unsigned be short"
                     }
                 }
             },
             "kind": "struct",
-            "size": 24
+            "size": 138
         }
     }
 }
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/linux/extensions/__init__.py` & `volatility3-2.7.0/volatility3/framework/symbols/linux/extensions/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,70 +3,139 @@
 #
 
 import collections.abc
 import logging
 import socket as socket_module
 from typing import Generator, Iterable, Iterator, Optional, Tuple, List
 
-from volatility3.framework import constants
+from volatility3.framework import constants, exceptions, objects, interfaces, symbols
 from volatility3.framework.constants.linux import SOCK_TYPES, SOCK_FAMILY
 from volatility3.framework.constants.linux import IP_PROTOCOLS, IPV6_PROTOCOLS
 from volatility3.framework.constants.linux import TCP_STATES, NETLINK_PROTOCOLS
 from volatility3.framework.constants.linux import ETH_PROTOCOLS, BLUETOOTH_STATES
 from volatility3.framework.constants.linux import BLUETOOTH_PROTOCOLS, SOCKET_STATES
 from volatility3.framework.constants.linux import CAPABILITIES
-from volatility3.framework import exceptions, objects, interfaces, symbols
 from volatility3.framework.layers import linear
 from volatility3.framework.objects import utility
 from volatility3.framework.symbols import generic, linux, intermed
 from volatility3.framework.symbols.linux.extensions import elf
 
 vollog = logging.getLogger(__name__)
 
 # Keep these in a basic module, to prevent import cycles when symbol providers require them
 
 
 class module(generic.GenericIntelProcess):
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._mod_mem_type = None  # Initialize _mod_mem_type to None for memoization
+
+    @property
+    def mod_mem_type(self):
+        """Return the mod_mem_type enum choices if available or an empty dict if not"""
+        # mod_mem_type and module_memory were added in kernel 6.4 which replaces
+        # module_layout for storing the information around core_layout etc.
+        # see commit ac3b43283923440900b4f36ca5f9f0b1ca43b70e for more information
+
+        if self._mod_mem_type is None:
+            try:
+                self._mod_mem_type = self._context.symbol_space.get_enumeration(
+                    self.get_symbol_table_name() + constants.BANG + "mod_mem_type"
+                ).choices
+            except exceptions.SymbolError:
+                vollog.debug(
+                    f"Unable to find mod_mem_type enum. This message can be ignored for kernels < 6.4"
+                )
+                # set to empty dict to show that the enum was not found, and so shouldn't be searched for again
+                self._mod_mem_type = {}
+        return self._mod_mem_type
+
     def get_module_base(self):
-        if self.has_member("core_layout"):
+        if self.has_member("mem"):  # kernels 6.4+
+            try:
+                return self.mem[self.mod_mem_type["MOD_TEXT"]].base
+            except KeyError:
+                raise AttributeError(
+                    "module -> get_module_base: Unable to get module base. Cannot read base from MOD_TEXT."
+                )
+        elif self.has_member("core_layout"):
             return self.core_layout.base
-        else:
+        elif self.has_member("module_core"):
             return self.module_core
+        raise AttributeError("module -> get_module_base: Unable to get module base")
 
     def get_init_size(self):
-        if self.has_member("init_layout"):
+        if self.has_member("mem"):  # kernels 6.4+
+            try:
+                return (
+                    self.mem[self.mod_mem_type["MOD_INIT_TEXT"]].size
+                    + self.mem[self.mod_mem_type["MOD_INIT_DATA"]].size
+                    + self.mem[self.mod_mem_type["MOD_INIT_RODATA"]].size
+                )
+            except KeyError:
+                raise AttributeError(
+                    "module -> get_init_size: Unable to determine .init section size of module. Cannot read size of MOD_INIT_TEXT, MOD_INIT_DATA, and MOD_INIT_RODATA"
+                )
+        elif self.has_member("init_layout"):
             return self.init_layout.size
         elif self.has_member("init_size"):
             return self.init_size
         raise AttributeError(
             "module -> get_init_size: Unable to determine .init section size of module"
         )
 
     def get_core_size(self):
-        if self.has_member("core_layout"):
+        if self.has_member("mem"):  # kernels 6.4+
+            try:
+                return (
+                    self.mem[self.mod_mem_type["MOD_TEXT"]].size
+                    + self.mem[self.mod_mem_type["MOD_DATA"]].size
+                    + self.mem[self.mod_mem_type["MOD_RODATA"]].size
+                    + self.mem[self.mod_mem_type["MOD_RO_AFTER_INIT"]].size
+                )
+            except KeyError:
+                raise AttributeError(
+                    "module -> get_core_size: Unable to determine core size of module. Cannot read size of MOD_TEXT, MOD_DATA, MOD_RODATA, and MOD_RO_AFTER_INIT."
+                )
+        elif self.has_member("core_layout"):
             return self.core_layout.size
         elif self.has_member("core_size"):
             return self.core_size
         raise AttributeError(
             "module -> get_core_size: Unable to determine core size of module"
         )
 
     def get_module_core(self):
-        if self.has_member("core_layout"):
+        if self.has_member("mem"):  # kernels 6.4+
+            try:
+                return self.mem[self.mod_mem_type["MOD_TEXT"]].base
+            except KeyError:
+                raise AttributeError(
+                    "module -> get_module_core: Unable to get module core. Cannot read base from MOD_TEXT."
+                )
+        elif self.has_member("core_layout"):
             return self.core_layout.base
         elif self.has_member("module_core"):
             return self.module_core
         raise AttributeError("module -> get_module_core: Unable to get module core")
 
     def get_module_init(self):
-        if self.has_member("init_layout"):
+        if self.has_member("mem"):  # kernels 6.4+
+            try:
+                return self.mem[self.mod_mem_type["MOD_INIT_TEXT"]].base
+            except KeyError:
+                raise AttributeError(
+                    "module -> get_module_core: Unable to get module init. Cannot read base from MOD_INIT_TEXT."
+                )
+        elif self.has_member("init_layout"):
             return self.init_layout.base
         elif self.has_member("module_init"):
             return self.module_init
-        raise AttributeError("module -> get_module_core: Unable to get module init")
+        raise AttributeError("module -> get_module_init: Unable to get module init")
 
     def get_name(self):
         """Get the name of the module as a string"""
         return utility.array_to_string(self.name)
 
     def _get_sect_count(self, grp):
         """Try to determine the number of valid sections"""
@@ -358,15 +427,15 @@
         # Create seen set if it does not exist, e.g. on the first call into this recursive function. This
         # must be None or an existing set of addresses for MTEs that have already been processed or that
         # should otherwise be ignored. If parsing from the root node for example this should be None on the
         # first call. If you needed to parse all nodes downwards from part of the tree this should still be
         # None. If however you wanted to parse from a node, but ignore some parts of the tree below it then
         # this could be populated with the addresses of the nodes you wish to ignore.
 
-        if seen == None:
+        if seen is None:
             seen = set()
 
         # protect against unlikely loop
         if maple_tree_entry in seen:
             vollog.warning(
                 f"The mte {hex(maple_tree_entry)} has all ready been seen, no further results will be produced for this node."
             )
@@ -443,39 +512,64 @@
             # unkown maple node type
             raise AttributeError(
                 f"Unkown Maple Tree node type {node_type} at offset {hex(pointer)}."
             )
 
 
 class mm_struct(objects.StructType):
+
+    # TODO: As of version 3.0.0 this method should be removed
     def get_mmap_iter(self) -> Iterable[interfaces.objects.ObjectInterface]:
-        """Returns an iterator for the mmap list member of an mm_struct."""
+        """
+        Deprecated: Use either get_vma_iter() or _get_mmap_iter().
+        """
+        vollog.warning(
+            "This method has been deprecated in favour of using the get_vma_iter() method."
+        )
+        yield from self.get_vma_iter()
+
+    def _get_mmap_iter(self) -> Iterable[interfaces.objects.ObjectInterface]:
+        """Returns an iterator for the mmap list member of an mm_struct. Use this only if
+        required, get_vma_iter() will choose the correct _get_maple_tree_iter() or
+        _get_mmap_iter() automatically as required."""
 
         if not self.has_member("mmap"):
             raise AttributeError(
-                "get_mmap_iter called on mm_struct where no mmap member exists."
+                "_get_mmap_iter called on mm_struct where no mmap member exists."
             )
         if not self.mmap:
             return None
         yield self.mmap
 
         seen = {self.mmap.vol.offset}
         link = self.mmap.vm_next
 
         while link != 0 and link.vol.offset not in seen:
             yield link
             seen.add(link.vol.offset)
             link = link.vm_next
 
+    # TODO: As of version 3.0.0 this method should be removed
     def get_maple_tree_iter(self) -> Iterable[interfaces.objects.ObjectInterface]:
-        """Returns an iterator for the mm_mt member of an mm_struct."""
+        """
+        Deprecated: Use either get_vma_iter() or _get_maple_tree_iter().
+        """
+        vollog.warning(
+            "This method has been deprecated in favour of using the get_vma_iter() method."
+        )
+        yield from self.get_vma_iter()
+
+    def _get_maple_tree_iter(self) -> Iterable[interfaces.objects.ObjectInterface]:
+        """Returns an iterator for the mm_mt member of an mm_struct. Use this only if
+        required, get_vma_iter() will choose the correct _get_maple_tree_iter() or
+        get_mmap_iter() automatically as required."""
 
         if not self.has_member("mm_mt"):
             raise AttributeError(
-                "get_maple_tree_iter called on mm_struct where no mm_mt member exists."
+                "_get_maple_tree_iter called on mm_struct where no mm_mt member exists."
             )
         symbol_table_name = self.get_symbol_table_name()
         for vma_pointer in self.mm_mt.get_slot_iter():
             # convert pointer to vm_area_struct and yield
             vma = self._context.object(
                 symbol_table_name + constants.BANG + "vm_area_struct",
                 layer_name=self.vol.native_layer_name,
@@ -483,17 +577,17 @@
             )
             yield vma
 
     def get_vma_iter(self) -> Iterable[interfaces.objects.ObjectInterface]:
         """Returns an iterator for the VMAs in an mm_struct. Automatically choosing the mmap or mm_mt as required."""
 
         if self.has_member("mmap"):
-            yield from self.get_mmap_iter()
+            yield from self._get_mmap_iter()
         elif self.has_member("mm_mt"):
-            yield from self.get_maple_tree_iter()
+            yield from self._get_maple_tree_iter()
         else:
             raise AttributeError("Unable to find mmap or mm_mt in mm_struct")
 
 
 class super_block(objects.StructType):
     # include/linux/kdev_t.h
     MINORBITS = 20
@@ -608,15 +702,16 @@
     # used by malfind
     def get_flags(self) -> str:
         return self._parse_flags(self.vm_flags, self.extended_flags)
 
     def get_page_offset(self) -> int:
         if self.vm_file == 0:
             return 0
-        return self.vm_pgoff << constants.linux.PAGE_SHIFT
+        parent_layer = self._context.layers[self.vol.layer_name]
+        return self.vm_pgoff << parent_layer.page_shift
 
     def get_name(self, context, task):
         if self.vm_file != 0:
             fname = linux.LinuxUtilities.path_for_file(context, task, self.vm_file)
         elif self.vm_start <= task.mm.start_brk and self.vm_end >= task.mm.brk:
             fname = "[heap]"
         elif self.vm_start <= task.mm.start_stack <= self.vm_end:
@@ -637,15 +732,15 @@
         flags_str = self.get_protection()
 
         if flags_str == "rwx":
             ret = True
         elif flags_str == "r-x" and self.vm_file.dereference().vol.offset == 0:
             ret = True
         elif proclayer and "x" in flags_str:
-            for i in range(self.vm_start, self.vm_end, 1 << constants.linux.PAGE_SHIFT):
+            for i in range(self.vm_start, self.vm_end, proclayer.page_size):
                 try:
                     if proclayer.is_dirty(i):
                         vollog.warning(
                             f"Found malicious (dirty+exec) page at {hex(i)} !"
                         )
                         # We do not attempt to find other dirty+exec pages once we have found one
                         ret = True
@@ -1038,25 +1133,25 @@
 
         return self.has_member("mnt_parent")
 
     def is_equal(self, vfsmount_ptr) -> bool:
         """Helper to make sure it is comparing two pointers to 'vfsmount'.
 
         Depending on the kernel version, the calling object (self) could be
-        a 'vfsmount \*' (<3.3.8) or a 'vfsmount' (>=3.3.8). This way we trust
+        a 'vfsmount \\*' (<3.3.8) or a 'vfsmount' (>=3.3.8). This way we trust
         in the framework "auto" dereferencing ability to assure that when we
         reach this point 'self' will be a 'vfsmount' already and self.vol.offset
-        a 'vfsmount \*' and not a 'vfsmount \*\*'. The argument must be a 'vfsmount \*'.
+        a 'vfsmount \\*' and not a 'vfsmount \\*\\*'. The argument must be a 'vfsmount \\*'.
         Typically, it's called from do_get_path().
 
         Args:
-            vfsmount_ptr (vfsmount \*): A pointer to a 'vfsmount'
+            vfsmount_ptr (vfsmount *): A pointer to a 'vfsmount'
 
         Raises:
-            exceptions.VolatilityException: If vfsmount_ptr is not a 'vfsmount \*'
+            exceptions.VolatilityException: If vfsmount_ptr is not a 'vfsmount \\*'
 
         Returns:
             bool: 'True' if the given argument points to the the same 'vfsmount'
             as 'self'.
         """
         if type(vfsmount_ptr) == objects.Pointer:
             return self.vol.offset == vfsmount_ptr
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/linux/extensions/bash.py` & `volatility3-2.7.0/volatility3/framework/symbols/linux/extensions/bash.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/linux/extensions/elf.py` & `volatility3-2.7.0/volatility3/framework/symbols/linux/extensions/elf.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 # which is available at https://www.volatilityfoundation.org/license/vsl-v1.0
 #
 
 from typing import Dict, Tuple
 import logging
 
 from volatility3.framework import constants
+from volatility3.framework.constants.linux import (
+    ELF_IDENT,
+    ELF_CLASS,
+)
 from volatility3.framework import objects, interfaces, exceptions
 
 vollog = logging.getLogger(__name__)
 
 
 class elf(objects.StructType):
     """
@@ -55,21 +59,23 @@
         if magic != 0x464C457F:  # e.g. ELF
             return None
 
         # We need to read the EI_CLASS (0x4 offset)
         ei_class = self._context.object(
             symbol_table_name + constants.BANG + "unsigned char",
             layer_name=layer_name,
-            offset=object_info.offset + 0x4,
+            offset=object_info.offset + ELF_IDENT.EI_CLASS,
         )
 
-        if ei_class == 1:
+        if ei_class == ELF_CLASS.ELFCLASS32:
             self._type_prefix = "Elf32_"
-        elif ei_class == 2:
+            self._ei_class_size = 32
+        elif ei_class == ELF_CLASS.ELFCLASS64:
             self._type_prefix = "Elf64_"
+            self._ei_class_size = 64
         else:
             raise ValueError(f"Unsupported ei_class value {ei_class}")
 
         # Construct the full header
         self._hdr = self._context.object(
             symbol_table_name + constants.BANG + self._type_prefix + "Ehdr",
             layer_name=layer_name,
@@ -136,44 +142,145 @@
                 + self._type_prefix
                 + "Shdr"
             ),
             count=self.e_shnum,
         )
         return section_headers
 
+    def get_link_maps(self, kernel_symbol_table_name):
+        """Get the ELF link map objects for the given VMA address
+
+        Args:
+            kernel_symbol_table_name (str): Kernel symbol table name
+
+        Yields:
+            The ELF link map objects
+        """
+        got_entry_size = self._ei_class_size // 8
+
+        elf_symbol_table = self.get_symbol_table_name()
+
+        link_maps_seen = set()
+        for phdr in self.get_program_headers():
+            try:
+                if phdr.p_type.description != "PT_DYNAMIC":
+                    continue
+            except ValueError:
+                vollog.log(
+                    constants.LOGLEVEL_VVVV,
+                    f"Skipping unknown ELF program header type: {phdr.p_type}",
+                )
+                continue
+
+            for dsec in phdr.dynamic_sections():
+                try:
+                    if dsec.d_tag.description != "DT_PLTGOT":
+                        continue
+                except ValueError:
+                    vollog.log(
+                        constants.LOGLEVEL_VVVV,
+                        f"Skipping unknown ELF dynamic section type: {dsec.d_tag}",
+                    )
+                    continue
+
+                got_start = dsec.d_ptr
+
+                # link_map is stored at the second GOT entry
+                link_map_addr = got_start + got_entry_size
+
+                # It needs the kernel symbol table to create a pointer
+                link_map_ptr = self._context.object(
+                    kernel_symbol_table_name + constants.BANG + "pointer",
+                    offset=link_map_addr,
+                    layer_name=self.vol.layer_name,
+                )
+                if not link_map_ptr:
+                    vollog.log(
+                        constants.LOGLEVEL_VVVV,
+                        f"Invalid ELF link map pointer at 0x{link_map_addr:x}",
+                    )
+                    continue
+
+                linkmap_symname = (
+                    elf_symbol_table + constants.BANG + self._type_prefix + "LinkMap"
+                )
+                try:
+                    link_map = self._context.object(
+                        object_type=linkmap_symname,
+                        offset=link_map_ptr,
+                        layer_name=self.vol.layer_name,
+                    )
+                except exceptions.InvalidAddressException:
+                    vollog.log(
+                        constants.LOGLEVEL_VVVV,
+                        f"Invalid ELF link map address at 0x{link_map_ptr:x}",
+                    )
+                    continue
+
+                while link_map and link_map.vol.offset != 0:
+                    if link_map.vol.offset in link_maps_seen:
+                        break
+                    link_maps_seen.add(link_map.vol.offset)
+
+                    yield link_map
+
+                    try:
+                        link_map = self._context.object(
+                            object_type=linkmap_symname,
+                            offset=link_map.l_next,
+                            layer_name=self.vol.layer_name,
+                        )
+                    except exceptions.InvalidAddressException:
+                        vollog.log(
+                            constants.LOGLEVEL_VVVV,
+                            f"ELF link map linked list is corrupt at 0x{self.vol.offset:x}",
+                        )
+                        break
+
     def _find_symbols(self):
         dt_strtab = None
         dt_symtab = None
         dt_strent = None
 
         for phdr in self.get_program_headers():
+            # Find PT_DYNAMIC segment
             try:
-                # Find PT_DYNAMIC segment
-                if str(phdr.p_type.description) != "PT_DYNAMIC":
+                if phdr.p_type.description != "PT_DYNAMIC":
                     continue
             except ValueError:
-                # If the p_type value is outside the ones declared in the enumeration, an
-                # exception is raised
-                return None
+                vollog.log(
+                    constants.LOGLEVEL_VVVV,
+                    f"Skipping unknown ELF program header type: {phdr.p_type}",
+                )
+                continue
 
             # This section contains pointers to the strtab, symtab, and strent sections
             for dsec in phdr.dynamic_sections():
-                if dsec.d_tag == 5:
+                try:
+                    dtag = dsec.d_tag.description
+                except ValueError:
+                    vollog.log(
+                        constants.LOGLEVEL_VVVV,
+                        f"Skipping unknown ELF dynamic section type: {dsec.d_tag}",
+                    )
+                    continue
+
+                if dtag == "DT_STRTAB":
                     dt_strtab = dsec.d_ptr
 
-                elif dsec.d_tag == 6:
+                elif dtag == "DT_SYMTAB":
                     dt_symtab = dsec.d_ptr
 
-                elif dsec.d_tag == 11:
+                elif dtag == "DT_SYMENT":
                     # Size of the symtab symbol entry
                     dt_strent = dsec.d_ptr
 
             break
 
-        if dt_strtab is None or dt_symtab is None or dt_strent is None:
+        if not (dt_strtab and dt_symtab and dt_strent):
             return None
 
         self._cached_symtab = dt_symtab
         self._cached_strtab = dt_strtab
 
         # Calculate number of symbol entries assuming that strtab follows symtab
         if dt_symtab < dt_strtab:
@@ -270,27 +377,39 @@
     @type_prefix.setter
     def type_prefix(self, prefix):
         self._type_prefix = prefix
 
     def get_vaddr(self):
         offset = self.__getattr__("p_vaddr")
 
-        if self._parent_e_type == 3:  # ET_DYN
-            offset = self._parent_offset + offset
+        try:
+            if self._parent_e_type.description == "ET_DYN":
+                offset = self._parent_offset + offset
+        except ValueError:
+            # Unknown ELF object file type. Anyway, if the ELF object file type is not a
+            # shared object (ET_DYN), the virtual address is 'p_vaddr'.
+            vollog.log(
+                constants.LOGLEVEL_VVVV,
+                f"Skipping unknown ELF object type: {self._parent_e_type}",
+            )
 
         return offset
 
     def dynamic_sections(self):
         # sanity check
         try:
-            if str(self.p_type.description) != "PT_DYNAMIC":
+            if self.p_type.description != "PT_DYNAMIC":
                 return None
         except ValueError:
             # If the value is outside the ones declared in the enumeration, an
             # exception is raised
+            vollog.log(
+                constants.LOGLEVEL_VVVV,
+                f"Skipping unknown ELF program header type: {self.p_type}",
+            )
             return None
 
         # the buffer of array starts at elf_base + our virtual address ( offset )
         arr_start = self.get_vaddr()
 
         symbol_table_name = self.get_symbol_table_name()
 
@@ -310,14 +429,34 @@
 
             yield dyn
 
             if dyn.d_tag == 0:
                 break
 
 
+class elf_linkmap(objects.StructType):
+    def get_name(self):
+        try:
+            buf = self._context.layers.read(self.vol.layer_name, self.l_name, 256)
+        except exceptions.PagedInvalidAddressException:
+            # Protection against memory smear
+            vollog.log(
+                constants.LOGLEVEL_VVVV,
+                f"Invalid l_name address for ELF link map at 0x{self.vol.offset:x}",
+            )
+            return None
+
+        idx = buf.find(b"\x00")
+        if idx != -1:
+            buf = buf[:idx]
+        return buf.decode()
+
+
 class_types = {
     "Elf": elf,
     "Elf64_Phdr": elf_phdr,
     "Elf32_Phdr": elf_phdr,
     "Elf32_Sym": elf_sym,
     "Elf64_Sym": elf_sym,
+    "Elf32_LinkMap": elf_linkmap,
+    "Elf64_LinkMap": elf_linkmap,
 }
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/linux/xen.json` & `volatility3-2.7.0/volatility3/framework/symbols/linux/xen.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/mac/__init__.py` & `volatility3-2.7.0/volatility3/framework/symbols/mac/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,22 @@
         self.set_type_class("proc", extensions.proc)
         self.set_type_class("fileglob", extensions.fileglob)
         self.set_type_class("vnode", extensions.vnode)
         self.set_type_class("vm_map_entry", extensions.vm_map_entry)
         self.set_type_class("vm_map_object", extensions.vm_map_object)
         self.set_type_class("socket", extensions.socket)
         self.set_type_class("inpcb", extensions.inpcb)
-        self.set_type_class("queue_entry", extensions.queue_entry)
         self.set_type_class("ifnet", extensions.ifnet)
         self.set_type_class("sockaddr_dl", extensions.sockaddr_dl)
         self.set_type_class("sockaddr", extensions.sockaddr)
         self.set_type_class("sysctl_oid", extensions.sysctl_oid)
         self.set_type_class("kauth_scope", extensions.kauth_scope)
+        # https://developer.apple.com/documentation/kernel/queue_head_t
+        self.set_type_class("queue_entry", extensions.queue_entry)
+        self.optional_set_type_class("queue_head_t", extensions.queue_entry)
 
 
 class MacUtilities(interfaces.configuration.VersionableInterface):
     """Class with multiple useful mac functions."""
 
     """
     Version History:
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/mac/extensions/__init__.py` & `volatility3-2.7.0/volatility3/framework/symbols/mac/extensions/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -486,30 +486,32 @@
 
         yielded = 0
 
         seen = set()
 
         for attr in ["next", "prev"]:
             with contextlib.suppress(exceptions.InvalidAddressException):
-                n = getattr(self, attr).dereference().cast(type_name)
-
-                while n is not None and n.vol.offset != list_head:
-                    if n.vol.offset in seen:
+                queue_element = getattr(self, attr).dereference().cast(type_name)
+                while (
+                    queue_element is not None
+                    and queue_element.vol.offset != list_head.vol.offset
+                ):
+                    if queue_element.vol.offset in seen:
                         break
 
-                    yield n
+                    yield queue_element
 
-                    seen.add(n.vol.offset)
+                    seen.add(queue_element.vol.offset)
 
                     yielded = yielded + 1
                     if yielded == max_size:
                         return None
 
-                    n = (
-                        getattr(n.member(attr=member_name), attr)
+                    queue_element = (
+                        getattr(queue_element.member(attr=member_name), attr)
                         .dereference()
                         .cast(type_name)
                     )
 
 
 class ifnet(objects.StructType):
     def sockaddr_dl(self):
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/native.py` & `volatility3-2.7.0/volatility3/framework/symbols/native.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/__init__.py` & `volatility3-2.7.0/volatility3/framework/symbols/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/bigpools/bigpools-vista-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/bigpools/bigpools-vista-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/bigpools/bigpools-vista-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/bigpools/bigpools-vista-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/bigpools/bigpools-win10-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/bigpools/bigpools-win10-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/bigpools/bigpools-win10-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/bigpools/bigpools-win10-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/bigpools/bigpools-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/bigpools/bigpools-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/bigpools/bigpools-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/bigpools/bigpools-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/callbacks-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/callbacks-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/callbacks-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/callbacks-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/crash.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/crash.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/crash64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/crash64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/crash_common.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/crash_common.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/__init__.py` & `volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -488,17 +488,55 @@
 
     def get_name(self) -> str:
         """Get the object's name from the object header."""
         header = self.get_object_header()
         return header.NameInfo.Name.String  # type: ignore
 
 
-class ETHREAD(objects.StructType):
+class ETHREAD(objects.StructType, pool.ExecutiveObject):
     """A class for executive thread objects."""
 
+    def is_valid(self) -> bool:
+        """Determine if the object is valid."""
+
+        try:
+            # validation by TID:
+            if self.Cid.UniqueThread % 4 != 0:  # NT tids are divisible by 4
+                return False
+
+            # validation by PID of parent process:
+            if self.Cid.UniqueProcess % 4 != 0:
+                return False
+
+            # validation by thread creation time:
+            if (
+                self.Cid.UniqueProcess != 4
+            ):  # The System process (PID 4) has no create time
+                ctime = self.get_create_time()
+                if not isinstance(ctime, datetime.datetime):
+                    return False
+
+                if not (1998 < ctime.year < 2030):
+                    return False
+
+        except exceptions.InvalidAddressException:
+            return False
+
+        # passed all validations
+        return True
+
+    def get_create_time(self):
+        # For Windows XPs
+        if self.has_member("ThreadsProcess"):
+            return conversion.wintime_to_datetime(self.CreateTime.QuadPart >> 3)
+        return conversion.wintime_to_datetime(self.CreateTime.QuadPart)
+
+    def get_exit_time(self):
+        return conversion.wintime_to_datetime(self.ExitTime.QuadPart)
+
     def owning_process(self) -> interfaces.objects.ObjectInterface:
         """Return the EPROCESS that owns this thread."""
 
         # For Windows XPs
         if self.has_member("ThreadsProcess"):
             return self.ThreadsProcess.dereference().cast("_EPROCESS")
         # For Windows Vista and later versions
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/crash.py` & `volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/crash.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/kdbg.py` & `volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/kdbg.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/mbr.py` & `volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/mbr.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/mft.py` & `volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/mft.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/network.py` & `volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/network.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/pe.py` & `volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/pe.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/pool.py` & `volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/pool.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/registry.py` & `volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/registry.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/extensions/services.py` & `volatility3-2.7.0/volatility3/framework/symbols/windows/extensions/services.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/kdbg.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/kdbg.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/kerb_ecrypt.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/kerb_ecrypt.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/mbr.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/mbr.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/mft.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/mft.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-vista-sp12-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-vista-sp12-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-vista-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-vista-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-vista-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-vista-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-10240-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-10240-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-10586-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-10586-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-14393-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-14393-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-15063-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-15063-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-15063-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-15063-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-16299-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-16299-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-17134-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-17134-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-17134-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-17134-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-17763-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-17763-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-18362-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-18362-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-18363-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-18363-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-19041-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-19041-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-19041-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-19041-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win10-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win10-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win7-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win8-x64.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997688492063492%*

 * *Differences: {"'user_types'": "{'_TCP_SYN_ENDPOINT': {'fields': {'Owner': {'offset': 64}, 'InetAF': {'offset': "*

 * *                 "48}, 'LocalPort': {'offset': 100}, 'RemotePort': {'offset': 102}, 'LocalAddr': "*

 * *                 "{'offset': 56}, 'RemoteAddress': {'offset': 80}}, 'size': 104}, "*

 * *                 "'_TCP_TIMEWAIT_ENDPOINT': {'fields': {'InetAF': {'offset': 24}, 'LocalPort': "*

 * *                 "{'offset': 48}, 'RemotePort': {'offset': 50}, 'LocalAddr': {'offset': 56}, "*

 * *                 "'RemoteAddress': {' […]*

```diff
@@ -104,23 +104,23 @@
             },
             "kind": "struct",
             "size": 24
         },
         "_INETAF": {
             "fields": {
                 "AddressFamily": {
-                    "offset": 20,
+                    "offset": 24,
                     "type": {
                         "kind": "base",
                         "name": "unsigned short"
                     }
                 }
             },
             "kind": "struct",
-            "size": 22
+            "size": 26
         },
         "_INET_COMPARTMENT": {
             "fields": {
                 "ProtocolCompartment": {
                     "offset": 32,
                     "type": {
                         "kind": "pointer",
@@ -149,29 +149,29 @@
             },
             "kind": "struct",
             "size": 384
         },
         "_INET_PORT_POOL": {
             "fields": {
                 "PortAssignments": {
-                    "offset": 160,
+                    "offset": 176,
                     "type": {
                         "count": 256,
                         "kind": "array",
                         "subtype": {
                             "kind": "pointer",
                             "subtype": {
                                 "kind": "struct",
                                 "name": "_PORT_ASSIGNMENT"
                             }
                         }
                     }
                 },
                 "PortBitMap": {
-                    "offset": 144,
+                    "offset": 160,
                     "type": {
                         "kind": "struct",
                         "name": "nt_symbols!_RTL_BITMAP"
                     }
                 }
             },
             "kind": "struct",
@@ -381,15 +381,15 @@
             },
             "kind": "struct",
             "size": 48
         },
         "_TCP_ENDPOINT": {
             "fields": {
                 "AddrInfo": {
-                    "offset": 32,
+                    "offset": 24,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_ADDRINFO"
                         }
                     }
@@ -398,15 +398,15 @@
                     "offset": 0,
                     "type": {
                         "kind": "union",
                         "name": "_LARGE_INTEGER"
                     }
                 },
                 "InetAF": {
-                    "offset": 24,
+                    "offset": 16,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_INETAF"
                         }
                     }
@@ -415,52 +415,52 @@
                     "offset": 40,
                     "type": {
                         "kind": "union",
                         "name": "nt_symbols!_LIST_ENTRY"
                     }
                 },
                 "LocalPort": {
-                    "offset": 108,
+                    "offset": 112,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 },
                 "Owner": {
-                    "offset": 568,
+                    "offset": 592,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "nt_symbols!_EPROCESS"
                         }
                     }
                 },
                 "RemotePort": {
-                    "offset": 110,
+                    "offset": 114,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 },
                 "State": {
-                    "offset": 104,
+                    "offset": 108,
                     "type": {
                         "kind": "enum",
                         "name": "TCPStateEnum"
                     }
                 }
             },
             "kind": "struct",
-            "size": 576
+            "size": 600
         },
         "_TCP_LISTENER": {
             "fields": {
                 "CreateTime": {
-                    "offset": 32,
+                    "offset": 64,
                     "type": {
                         "kind": "union",
                         "name": "_LARGE_INTEGER"
                     }
                 },
                 "InetAF": {
                     "offset": 96,
@@ -519,15 +519,15 @@
                     "offset": 0,
                     "type": {
                         "kind": "union",
                         "name": "_LARGE_INTEGER"
                     }
                 },
                 "InetAF": {
-                    "offset": 72,
+                    "offset": 48,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_INETAF"
                         }
                     }
@@ -536,72 +536,72 @@
                     "offset": 16,
                     "type": {
                         "kind": "union",
                         "name": "nt_symbols!_LIST_ENTRY"
                     }
                 },
                 "LocalAddr": {
-                    "offset": 80,
+                    "offset": 56,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_LOCAL_ADDRESS"
                         }
                     }
                 },
                 "LocalPort": {
-                    "offset": 124,
+                    "offset": 100,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 },
                 "Owner": {
-                    "offset": 88,
+                    "offset": 64,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_SYN_OWNER"
                         }
                     }
                 },
                 "RemoteAddress": {
-                    "offset": 104,
+                    "offset": 80,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_IN_ADDR"
                         }
                     }
                 },
                 "RemotePort": {
-                    "offset": 126,
+                    "offset": 102,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 }
             },
             "kind": "struct",
-            "size": 128
+            "size": 104
         },
         "_TCP_TIMEWAIT_ENDPOINT": {
             "fields": {
                 "CreateTime": {
                     "offset": 0,
                     "type": {
                         "kind": "union",
                         "name": "_LARGE_INTEGER"
                     }
                 },
                 "InetAF": {
-                    "offset": 48,
+                    "offset": 24,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_INETAF"
                         }
                     }
@@ -610,50 +610,50 @@
                     "offset": 0,
                     "type": {
                         "kind": "union",
                         "name": "nt_symbols!_LIST_ENTRY"
                     }
                 },
                 "LocalAddr": {
-                    "offset": 80,
+                    "offset": 56,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_LOCAL_ADDRESS"
                         }
                     }
                 },
                 "LocalPort": {
-                    "offset": 72,
+                    "offset": 48,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 },
                 "RemoteAddress": {
-                    "offset": 88,
+                    "offset": 64,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_IN_ADDR"
                         }
                     }
                 },
                 "RemotePort": {
-                    "offset": 74,
+                    "offset": 50,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 }
             },
             "kind": "struct",
-            "size": 96
+            "size": 72
         },
         "_UDP_ENDPOINT": {
             "fields": {
                 "CreateTime": {
                     "offset": 88,
                     "type": {
                         "kind": "union",
@@ -705,11 +705,11 @@
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 }
             },
             "kind": "struct",
-            "size": 138
+            "size": 130
         }
     }
 }
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win7-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win7-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win8-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win81-x64.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987261284722223%*

 * *Differences: {"'user_types'": "{'_UDP_ENDPOINT': {'fields': {'Port': {'offset': 120}, 'Next': {'offset': "*

 * *                 "112}}}, '_TCP_ENDPOINT': {'fields': {'Owner': {'offset': 600}}, 'size': 608}, "*

 * *                 "'_PORT_ASSIGNMENT_ENTRY': {'size': 24}, '_PORT_ASSIGNMENT_LIST': {'size': 6144}}"}*

```diff
@@ -327,15 +327,15 @@
                             "kind": "base",
                             "name": "void"
                         }
                     }
                 }
             },
             "kind": "struct",
-            "size": 16
+            "size": 24
         },
         "_PORT_ASSIGNMENT_LIST": {
             "fields": {
                 "Assignments": {
                     "offset": 0,
                     "type": {
                         "count": 256,
@@ -344,15 +344,15 @@
                             "kind": "struct",
                             "name": "_PORT_ASSIGNMENT_ENTRY"
                         }
                     }
                 }
             },
             "kind": "struct",
-            "size": 4096
+            "size": 6144
         },
         "_PROTOCOL_COMPARTMENT": {
             "fields": {
                 "PortPool": {
                     "offset": 0,
                     "type": {
                         "kind": "pointer",
@@ -422,15 +422,15 @@
                     "offset": 112,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 },
                 "Owner": {
-                    "offset": 592,
+                    "offset": 600,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "nt_symbols!_EPROCESS"
                         }
                     }
@@ -447,15 +447,15 @@
                     "type": {
                         "kind": "enum",
                         "name": "TCPStateEnum"
                     }
                 }
             },
             "kind": "struct",
-            "size": 600
+            "size": 608
         },
         "_TCP_LISTENER": {
             "fields": {
                 "CreateTime": {
                     "offset": 64,
                     "type": {
                         "kind": "union",
@@ -677,15 +677,15 @@
                         "subtype": {
                             "kind": "struct",
                             "name": "_LOCAL_ADDRESS"
                         }
                     }
                 },
                 "Next": {
-                    "offset": 136,
+                    "offset": 112,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_UDP_ENDPOINT"
                         }
                     }
@@ -697,15 +697,15 @@
                         "subtype": {
                             "kind": "struct",
                             "name": "nt_symbols!_EPROCESS"
                         }
                     }
                 },
                 "Port": {
-                    "offset": 128,
+                    "offset": 120,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 }
             },
             "kind": "struct",
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win8-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win8-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win81-19935-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win81-19935-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win81-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/netscan/netscan-win81-x86.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9457583085317461%*

 * *Differences: {"'base_types'": "{'pointer': {'size': 4}}",*

 * * "'metadata'": "{'producer': {'datetime': '2020-05-29T19:28:34'}}",*

 * * "'user_types'": "{'_TCP_SYN_ENDPOINT': {'fields': {'Owner': {'offset': 32}, 'ListEntry': "*

 * *                 "{'offset': 8}, 'InetAF': {'offset': 24}, 'LocalPort': {'offset': 60}, "*

 * *                 "'RemotePort': {'offset': 62}, 'LocalAddr': {'offset': 28}, 'RemoteAddress': "*

 * *                 "{'offset': 40}}, 'size': 64}, '_TCP_TIMEWAIT_ENDPOINT': {'fields': {'ListEntry': "*

 * *                 "{' […]*

```diff
@@ -12,15 +12,15 @@
             "signed": true,
             "size": 8
         },
         "pointer": {
             "endian": "little",
             "kind": "int",
             "signed": false,
-            "size": 8
+            "size": 4
         },
         "unsigned be short": {
             "endian": "big",
             "kind": "int",
             "signed": false,
             "size": 2
         },
@@ -68,15 +68,15 @@
             },
             "size": 4
         }
     },
     "metadata": {
         "format": "6.0.0",
         "producer": {
-            "datetime": "2020-06-12T14:00:00",
+            "datetime": "2020-05-29T19:28:34",
             "name": "japhlange-by-hand",
             "version": "0.0.1"
         }
     },
     "symbols": {},
     "user_types": {
         "_ADDRINFO": {
@@ -88,98 +88,39 @@
                         "subtype": {
                             "kind": "struct",
                             "name": "_LOCAL_ADDRESS"
                         }
                     }
                 },
                 "Remote": {
-                    "offset": 16,
+                    "offset": 12,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_IN_ADDR"
                         }
                     }
                 }
             },
             "kind": "struct",
-            "size": 24
+            "size": 16
         },
         "_INETAF": {
             "fields": {
                 "AddressFamily": {
-                    "offset": 24,
+                    "offset": 12,
                     "type": {
                         "kind": "base",
                         "name": "unsigned short"
                     }
                 }
             },
             "kind": "struct",
-            "size": 26
-        },
-        "_INET_COMPARTMENT": {
-            "fields": {
-                "ProtocolCompartment": {
-                    "offset": 32,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_PROTOCOL_COMPARTMENT"
-                        }
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 48
-        },
-        "_INET_COMPARTMENT_SET": {
-            "fields": {
-                "InetCompartment": {
-                    "offset": 328,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_INET_COMPARTMENT"
-                        }
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 384
-        },
-        "_INET_PORT_POOL": {
-            "fields": {
-                "PortAssignments": {
-                    "offset": 176,
-                    "type": {
-                        "count": 256,
-                        "kind": "array",
-                        "subtype": {
-                            "kind": "pointer",
-                            "subtype": {
-                                "kind": "struct",
-                                "name": "_PORT_ASSIGNMENT"
-                            }
-                        }
-                    }
-                },
-                "PortBitMap": {
-                    "offset": 160,
-                    "type": {
-                        "kind": "struct",
-                        "name": "nt_symbols!_RTL_BITMAP"
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 11200
+            "size": 14
         },
         "_IN_ADDR": {
             "fields": {
                 "addr4": {
                     "offset": 0,
                     "type": {
                         "count": 4,
@@ -238,158 +179,50 @@
             },
             "kind": "union",
             "size": 8
         },
         "_LOCAL_ADDRESS": {
             "fields": {
                 "pData": {
-                    "offset": 16,
+                    "offset": 12,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "pointer",
                             "subtype": {
                                 "kind": "struct",
                                 "name": "_IN_ADDR"
                             }
                         }
                     }
                 }
             },
             "kind": "struct",
-            "size": 24
-        },
-        "_PARTITION": {
-            "fields": {
-                "Endpoints": {
-                    "offset": 8,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "nt_symbols!_RTL_DYNAMIC_HASH_TABLE"
-                        }
-                    }
-                },
-                "UnknownHashTable": {
-                    "offset": 16,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "nt_symbols!_RTL_DYNAMIC_HASH_TABLE"
-                        }
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 128
-        },
-        "_PARTITION_TABLE": {
-            "fields": {
-                "Partitions": {
-                    "offset": 0,
-                    "type": {
-                        "count": 1,
-                        "kind": "array",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_PARTITION"
-                        }
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 128
-        },
-        "_PORT_ASSIGNMENT": {
-            "fields": {
-                "InPaBigPoolBase": {
-                    "offset": 32,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_PORT_ASSIGNMENT_LIST"
-                        }
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 40
-        },
-        "_PORT_ASSIGNMENT_ENTRY": {
-            "fields": {
-                "Entry": {
-                    "offset": 8,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "base",
-                            "name": "void"
-                        }
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 24
-        },
-        "_PORT_ASSIGNMENT_LIST": {
-            "fields": {
-                "Assignments": {
-                    "offset": 0,
-                    "type": {
-                        "count": 256,
-                        "kind": "array",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_PORT_ASSIGNMENT_ENTRY"
-                        }
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 6144
-        },
-        "_PROTOCOL_COMPARTMENT": {
-            "fields": {
-                "PortPool": {
-                    "offset": 0,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_INET_PORT_POOL"
-                        }
-                    }
-                }
-            },
-            "kind": "struct",
             "size": 16
         },
         "_SYN_OWNER": {
             "fields": {
                 "Process": {
-                    "offset": 40,
+                    "offset": 24,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "nt_symbols!_EPROCESS"
                         }
                     }
                 }
             },
             "kind": "struct",
-            "size": 48
+            "size": 14
         },
         "_TCP_ENDPOINT": {
             "fields": {
                 "AddrInfo": {
-                    "offset": 24,
+                    "offset": 12,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_ADDRINFO"
                         }
                     }
@@ -398,318 +231,298 @@
                     "offset": 0,
                     "type": {
                         "kind": "union",
                         "name": "_LARGE_INTEGER"
                     }
                 },
                 "InetAF": {
-                    "offset": 16,
+                    "offset": 8,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_INETAF"
                         }
                     }
                 },
                 "ListEntry": {
-                    "offset": 40,
+                    "offset": 20,
                     "type": {
                         "kind": "union",
                         "name": "nt_symbols!_LIST_ENTRY"
                     }
                 },
                 "LocalPort": {
-                    "offset": 112,
+                    "offset": 60,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 },
                 "Owner": {
-                    "offset": 600,
+                    "offset": 424,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "nt_symbols!_EPROCESS"
                         }
                     }
                 },
                 "RemotePort": {
-                    "offset": 114,
+                    "offset": 62,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 },
                 "State": {
-                    "offset": 108,
+                    "offset": 56,
                     "type": {
                         "kind": "enum",
                         "name": "TCPStateEnum"
                     }
                 }
             },
             "kind": "struct",
-            "size": 608
+            "size": 428
         },
         "_TCP_LISTENER": {
             "fields": {
                 "CreateTime": {
-                    "offset": 64,
+                    "offset": 32,
                     "type": {
                         "kind": "union",
                         "name": "_LARGE_INTEGER"
                     }
                 },
                 "InetAF": {
-                    "offset": 96,
+                    "offset": 56,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_INETAF"
                         }
                     }
                 },
                 "LocalAddr": {
-                    "offset": 88,
+                    "offset": 52,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_LOCAL_ADDRESS"
                         }
                     }
                 },
-                "Next": {
-                    "offset": 112,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_TCP_LISTENER"
-                        }
-                    }
-                },
                 "Owner": {
-                    "offset": 40,
+                    "offset": 24,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "nt_symbols!_EPROCESS"
                         }
                     }
                 },
                 "Port": {
-                    "offset": 106,
+                    "offset": 62,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 }
             },
             "kind": "struct",
-            "size": 108
+            "size": 64
         },
         "_TCP_SYN_ENDPOINT": {
             "fields": {
                 "CreateTime": {
                     "offset": 0,
                     "type": {
                         "kind": "union",
                         "name": "_LARGE_INTEGER"
                     }
                 },
                 "InetAF": {
-                    "offset": 48,
+                    "offset": 24,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_INETAF"
                         }
                     }
                 },
                 "ListEntry": {
-                    "offset": 16,
+                    "offset": 8,
                     "type": {
                         "kind": "union",
                         "name": "nt_symbols!_LIST_ENTRY"
                     }
                 },
                 "LocalAddr": {
-                    "offset": 56,
+                    "offset": 28,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_LOCAL_ADDRESS"
                         }
                     }
                 },
                 "LocalPort": {
-                    "offset": 100,
+                    "offset": 60,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 },
                 "Owner": {
-                    "offset": 64,
+                    "offset": 32,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_SYN_OWNER"
                         }
                     }
                 },
                 "RemoteAddress": {
-                    "offset": 80,
+                    "offset": 40,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_IN_ADDR"
                         }
                     }
                 },
                 "RemotePort": {
-                    "offset": 102,
+                    "offset": 62,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 }
             },
             "kind": "struct",
-            "size": 104
+            "size": 64
         },
         "_TCP_TIMEWAIT_ENDPOINT": {
             "fields": {
                 "CreateTime": {
                     "offset": 0,
                     "type": {
                         "kind": "union",
                         "name": "_LARGE_INTEGER"
                     }
                 },
                 "InetAF": {
-                    "offset": 24,
+                    "offset": 12,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_INETAF"
                         }
                     }
                 },
                 "ListEntry": {
-                    "offset": 0,
+                    "offset": 20,
                     "type": {
                         "kind": "union",
                         "name": "nt_symbols!_LIST_ENTRY"
                     }
                 },
                 "LocalAddr": {
-                    "offset": 56,
+                    "offset": 32,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_LOCAL_ADDRESS"
                         }
                     }
                 },
                 "LocalPort": {
-                    "offset": 48,
+                    "offset": 28,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 },
                 "RemoteAddress": {
-                    "offset": 64,
+                    "offset": 36,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_IN_ADDR"
                         }
                     }
                 },
                 "RemotePort": {
-                    "offset": 50,
+                    "offset": 30,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 }
             },
             "kind": "struct",
-            "size": 72
+            "size": 40
         },
         "_UDP_ENDPOINT": {
             "fields": {
                 "CreateTime": {
-                    "offset": 88,
+                    "offset": 48,
                     "type": {
                         "kind": "union",
                         "name": "_LARGE_INTEGER"
                     }
                 },
                 "InetAF": {
-                    "offset": 32,
+                    "offset": 20,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_INETAF"
                         }
                     }
                 },
                 "LocalAddr": {
-                    "offset": 96,
+                    "offset": 56,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_LOCAL_ADDRESS"
                         }
                     }
                 },
-                "Next": {
-                    "offset": 112,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_UDP_ENDPOINT"
-                        }
-                    }
-                },
                 "Owner": {
-                    "offset": 40,
+                    "offset": 24,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "nt_symbols!_EPROCESS"
                         }
                     }
                 },
                 "Port": {
-                    "offset": 120,
+                    "offset": 72,
                     "type": {
                         "kind": "base",
                         "name": "unsigned be short"
                     }
                 }
             },
             "kind": "struct",
-            "size": 130
+            "size": 74
         }
     }
 }
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/netscan/netscan-win81-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-vista-x86.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7416666666666666%*

 * *Differences: {"'base_types'": "{delete: ['unsigned be short', 'long long']}",*

 * * "'enums'": "{replace: OrderedDict([('StateEnum', OrderedDict([('base', 'long'), ('constants', "*

 * *            "OrderedDict([('SERVICE_START_PENDING', 2), ('SERVICE_STOP_PENDING', 3), "*

 * *            "('SERVICE_STOPPED', 1), ('SERVICE_CONTINUE_PENDING', 5), ('SERVICE_PAUSE_PENDING', "*

 * *            "6), ('SERVICE_PAUSED', 7), ('SERVICE_RUNNING', 4)])), ('size', 4)])), ('StartEnum', "*

 * *            "OrderedDict([('base', 'long'), ('constants', OrderedD […]*

```diff
@@ -2,32 +2,20 @@
     "base_types": {
         "long": {
             "endian": "little",
             "kind": "int",
             "signed": false,
             "size": 4
         },
-        "long long": {
-            "endian": "little",
-            "kind": "int",
-            "signed": true,
-            "size": 8
-        },
         "pointer": {
             "endian": "little",
             "kind": "int",
             "signed": false,
             "size": 4
         },
-        "unsigned be short": {
-            "endian": "big",
-            "kind": "int",
-            "signed": false,
-            "size": 2
-        },
         "unsigned char": {
             "endian": "little",
             "kind": "char",
             "signed": false,
             "size": 1
         },
         "unsigned int": {
@@ -46,483 +34,222 @@
             "endian": "little",
             "kind": "int",
             "signed": false,
             "size": 2
         }
     },
     "enums": {
-        "TCPStateEnum": {
+        "StartEnum": {
             "base": "long",
             "constants": {
-                "CLOSED": 0,
-                "CLOSE_WAIT": 7,
-                "CLOSING": 8,
-                "DELETE_TCB": 13,
-                "ESTABLISHED": 4,
-                "FIN_WAIT1": 5,
-                "FIN_WAIT2": 6,
-                "LAST_ACK": 9,
-                "LISTENING": 1,
-                "SYN_RCVD": 3,
-                "SYN_SENT": 2,
-                "TIME_WAIT": 12
+                "SERVICE_AUTO_START": 2,
+                "SERVICE_BOOT_START": 0,
+                "SERVICE_DEMAND_START": 3,
+                "SERVICE_DISABLED": 4,
+                "SERVICE_SYSTEM_START": 1
+            },
+            "size": 4
+        },
+        "StateEnum": {
+            "base": "long",
+            "constants": {
+                "SERVICE_CONTINUE_PENDING": 5,
+                "SERVICE_PAUSED": 7,
+                "SERVICE_PAUSE_PENDING": 6,
+                "SERVICE_RUNNING": 4,
+                "SERVICE_START_PENDING": 2,
+                "SERVICE_STOPPED": 1,
+                "SERVICE_STOP_PENDING": 3
             },
             "size": 4
         }
     },
     "metadata": {
-        "format": "6.0.0",
+        "format": "4.1.0",
         "producer": {
-            "datetime": "2020-05-29T19:28:34",
-            "name": "japhlange-by-hand",
+            "datetime": "2019-04-17T13:45:16.417006",
+            "name": "vtypes_to_json.py",
             "version": "0.0.1"
         }
     },
     "symbols": {},
     "user_types": {
-        "_ADDRINFO": {
+        "_SERVICE_HEADER": {
             "fields": {
-                "Local": {
-                    "offset": 0,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_LOCAL_ADDRESS"
-                        }
-                    }
-                },
-                "Remote": {
+                "ServiceRecord": {
                     "offset": 12,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
-                            "name": "_IN_ADDR"
-                        }
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 16
-        },
-        "_INETAF": {
-            "fields": {
-                "AddressFamily": {
-                    "offset": 12,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned short"
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 14
-        },
-        "_IN_ADDR": {
-            "fields": {
-                "addr4": {
-                    "offset": 0,
-                    "type": {
-                        "count": 4,
-                        "kind": "array",
-                        "subtype": {
-                            "kind": "base",
-                            "name": "unsigned char"
+                            "name": "_SERVICE_RECORD"
                         }
                     }
                 },
-                "addr6": {
+                "Tag": {
                     "offset": 0,
                     "type": {
-                        "count": 16,
+                        "count": 4,
                         "kind": "array",
                         "subtype": {
                             "kind": "base",
                             "name": "unsigned char"
                         }
                     }
                 }
             },
             "kind": "struct",
-            "size": 6
-        },
-        "_LARGE_INTEGER": {
-            "fields": {
-                "HighPart": {
-                    "offset": 4,
-                    "type": {
-                        "kind": "base",
-                        "name": "long"
-                    }
-                },
-                "LowPart": {
-                    "offset": 0,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned long"
-                    }
-                },
-                "QuadPart": {
-                    "offset": 0,
-                    "type": {
-                        "kind": "base",
-                        "name": "long long"
-                    }
-                },
-                "u": {
-                    "offset": 0,
-                    "type": {
-                        "kind": "struct",
-                        "name": "__unnamed_2"
-                    }
-                }
-            },
-            "kind": "union",
-            "size": 8
-        },
-        "_LOCAL_ADDRESS": {
-            "fields": {
-                "pData": {
-                    "offset": 12,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "pointer",
-                            "subtype": {
-                                "kind": "struct",
-                                "name": "_IN_ADDR"
-                            }
-                        }
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 16
-        },
-        "_SYN_OWNER": {
-            "fields": {
-                "Process": {
-                    "offset": 24,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "nt_symbols!_EPROCESS"
-                        }
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 14
+            "size": 12
         },
-        "_TCP_ENDPOINT": {
+        "_SERVICE_LIST_ENTRY": {
             "fields": {
-                "AddrInfo": {
-                    "offset": 12,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_ADDRINFO"
-                        }
-                    }
-                },
-                "CreateTime": {
+                "Blink": {
                     "offset": 0,
                     "type": {
-                        "kind": "union",
-                        "name": "_LARGE_INTEGER"
-                    }
-                },
-                "InetAF": {
-                    "offset": 8,
-                    "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
-                            "name": "_INETAF"
+                            "name": "_SERVICE_LIST_ENTRY"
                         }
                     }
                 },
-                "ListEntry": {
-                    "offset": 20,
-                    "type": {
-                        "kind": "union",
-                        "name": "nt_symbols!_LIST_ENTRY"
-                    }
-                },
-                "LocalPort": {
-                    "offset": 60,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned be short"
-                    }
-                },
-                "Owner": {
-                    "offset": 424,
+                "Flink": {
+                    "offset": 4,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
-                            "name": "nt_symbols!_EPROCESS"
+                            "name": "_SERVICE_LIST_ENTRY"
                         }
                     }
-                },
-                "RemotePort": {
-                    "offset": 62,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned be short"
-                    }
-                },
-                "State": {
-                    "offset": 56,
-                    "type": {
-                        "kind": "enum",
-                        "name": "TCPStateEnum"
-                    }
                 }
             },
             "kind": "struct",
-            "size": 428
+            "size": 8
         },
-        "_TCP_LISTENER": {
+        "_SERVICE_PROCESS": {
             "fields": {
-                "CreateTime": {
-                    "offset": 32,
-                    "type": {
-                        "kind": "union",
-                        "name": "_LARGE_INTEGER"
-                    }
-                },
-                "InetAF": {
-                    "offset": 56,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_INETAF"
-                        }
-                    }
-                },
-                "LocalAddr": {
-                    "offset": 52,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_LOCAL_ADDRESS"
-                        }
-                    }
-                },
-                "Owner": {
-                    "offset": 24,
+                "BinaryPath": {
+                    "offset": 8,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
-                            "kind": "struct",
-                            "name": "nt_symbols!_EPROCESS"
+                            "kind": "base",
+                            "name": "unsigned short"
                         }
                     }
                 },
-                "Port": {
-                    "offset": 62,
+                "ProcessId": {
+                    "offset": 12,
                     "type": {
                         "kind": "base",
-                        "name": "unsigned be short"
+                        "name": "unsigned int"
                     }
                 }
             },
             "kind": "struct",
-            "size": 64
+            "size": 12
         },
-        "_TCP_SYN_ENDPOINT": {
+        "_SERVICE_RECORD": {
             "fields": {
-                "CreateTime": {
-                    "offset": 0,
-                    "type": {
-                        "kind": "union",
-                        "name": "_LARGE_INTEGER"
-                    }
-                },
-                "InetAF": {
-                    "offset": 24,
+                "DisplayName": {
+                    "offset": 8,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
-                            "kind": "struct",
-                            "name": "_INETAF"
+                            "kind": "base",
+                            "name": "unsigned short"
                         }
                     }
                 },
-                "ListEntry": {
-                    "offset": 8,
-                    "type": {
-                        "kind": "union",
-                        "name": "nt_symbols!_LIST_ENTRY"
-                    }
-                },
-                "LocalAddr": {
+                "DriverName": {
                     "offset": 28,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
-                            "kind": "struct",
-                            "name": "_LOCAL_ADDRESS"
+                            "kind": "base",
+                            "name": "unsigned short"
                         }
                     }
                 },
-                "LocalPort": {
-                    "offset": 60,
+                "Order": {
+                    "offset": 12,
                     "type": {
                         "kind": "base",
-                        "name": "unsigned be short"
-                    }
-                },
-                "Owner": {
-                    "offset": 32,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_SYN_OWNER"
-                        }
-                    }
-                },
-                "RemoteAddress": {
-                    "offset": 40,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_IN_ADDR"
-                        }
+                        "name": "unsigned int"
                     }
                 },
-                "RemotePort": {
-                    "offset": 62,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned be short"
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 64
-        },
-        "_TCP_TIMEWAIT_ENDPOINT": {
-            "fields": {
-                "CreateTime": {
+                "PrevEntry": {
                     "offset": 0,
                     "type": {
-                        "kind": "union",
-                        "name": "_LARGE_INTEGER"
-                    }
-                },
-                "InetAF": {
-                    "offset": 12,
-                    "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
-                            "name": "_INETAF"
+                            "name": "_SERVICE_RECORD"
                         }
                     }
                 },
-                "ListEntry": {
-                    "offset": 20,
+                "ServiceList": {
+                    "offset": 92,
                     "type": {
-                        "kind": "union",
-                        "name": "nt_symbols!_LIST_ENTRY"
+                        "kind": "struct",
+                        "name": "_SERVICE_LIST_ENTRY"
                     }
                 },
-                "LocalAddr": {
-                    "offset": 32,
+                "ServiceName": {
+                    "offset": 4,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
-                            "kind": "struct",
-                            "name": "_LOCAL_ADDRESS"
+                            "kind": "base",
+                            "name": "unsigned short"
                         }
                     }
                 },
-                "LocalPort": {
+                "ServiceProcess": {
                     "offset": 28,
                     "type": {
-                        "kind": "base",
-                        "name": "unsigned be short"
-                    }
-                },
-                "RemoteAddress": {
-                    "offset": 36,
-                    "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
-                            "name": "_IN_ADDR"
+                            "name": "_SERVICE_PROCESS"
                         }
                     }
                 },
-                "RemotePort": {
-                    "offset": 30,
-                    "type": {
-                        "kind": "base",
-                        "name": "unsigned be short"
-                    }
-                }
-            },
-            "kind": "struct",
-            "size": 40
-        },
-        "_UDP_ENDPOINT": {
-            "fields": {
-                "CreateTime": {
-                    "offset": 48,
-                    "type": {
-                        "kind": "union",
-                        "name": "_LARGE_INTEGER"
-                    }
-                },
-                "InetAF": {
-                    "offset": 20,
+                "Start": {
+                    "offset": 60,
                     "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_INETAF"
-                        }
+                        "kind": "enum",
+                        "name": "StartEnum"
                     }
                 },
-                "LocalAddr": {
-                    "offset": 56,
+                "State": {
+                    "offset": 36,
                     "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_LOCAL_ADDRESS"
-                        }
+                        "kind": "enum",
+                        "name": "StateEnum"
                     }
                 },
-                "Owner": {
+                "Tag": {
                     "offset": 24,
                     "type": {
-                        "kind": "pointer",
+                        "count": 4,
+                        "kind": "array",
                         "subtype": {
-                            "kind": "struct",
-                            "name": "nt_symbols!_EPROCESS"
+                            "kind": "base",
+                            "name": "unsigned char"
                         }
                     }
                 },
-                "Port": {
-                    "offset": 72,
+                "Type": {
+                    "offset": 32,
                     "type": {
                         "kind": "base",
-                        "name": "unsigned be short"
+                        "name": "unsigned long"
                     }
                 }
             },
             "kind": "struct",
-            "size": 74
+            "size": 92
         }
     }
 }
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/pdb.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/pdb.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/pdbconv.py` & `volatility3-2.7.0/volatility3/framework/symbols/windows/pdbconv.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/pdbutil.py` & `volatility3-2.7.0/volatility3/framework/symbols/windows/pdbutil.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/pe.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/pe.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/poolheader-x64-win7.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/poolheader-x64-win7.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/poolheader-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/poolheader-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/poolheader-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/poolheader-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/registry.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/registry.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-vista-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-vista-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-vista-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-xp-2003-x64.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9896780303030305%*

 * *Differences: {"'base_types'": "{'pointer': {'size': 8}}",*

 * * "'user_types'": "{'_SERVICE_LIST_ENTRY': {'fields': {'Flink': {'offset': 16}}, 'size': 16}, "*

 * *                 "'_SERVICE_PROCESS': {'fields': {'BinaryPath': {'offset': 16}, 'ProcessId': "*

 * *                 "{'offset': 24}}, 'size': 24}, '_SERVICE_HEADER': {'fields': {'ServiceRecord': "*

 * *                 "{'offset': 16}}, 'size': 16}, '_SERVICE_RECORD': {'fields': {'ServiceList': "*

 * *                 "{'offset': 0}, 'DisplayName': {'offset': 16}, 'ServiceProcess': { […]*

```diff
@@ -6,15 +6,15 @@
             "signed": false,
             "size": 4
         },
         "pointer": {
             "endian": "little",
             "kind": "int",
             "signed": false,
-            "size": 4
+            "size": 8
         },
         "unsigned char": {
             "endian": "little",
             "kind": "char",
             "signed": false,
             "size": 1
         },
@@ -72,15 +72,15 @@
         }
     },
     "symbols": {},
     "user_types": {
         "_SERVICE_HEADER": {
             "fields": {
                 "ServiceRecord": {
-                    "offset": 12,
+                    "offset": 16,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_SERVICE_RECORD"
                         }
                     }
@@ -94,162 +94,152 @@
                             "kind": "base",
                             "name": "unsigned char"
                         }
                     }
                 }
             },
             "kind": "struct",
-            "size": 12
+            "size": 16
         },
         "_SERVICE_LIST_ENTRY": {
             "fields": {
                 "Blink": {
                     "offset": 0,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_SERVICE_LIST_ENTRY"
                         }
                     }
                 },
                 "Flink": {
-                    "offset": 4,
+                    "offset": 16,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_SERVICE_LIST_ENTRY"
                         }
                     }
                 }
             },
             "kind": "struct",
-            "size": 8
+            "size": 16
         },
         "_SERVICE_PROCESS": {
             "fields": {
                 "BinaryPath": {
-                    "offset": 8,
+                    "offset": 16,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "base",
                             "name": "unsigned short"
                         }
                     }
                 },
                 "ProcessId": {
-                    "offset": 12,
+                    "offset": 24,
                     "type": {
                         "kind": "base",
                         "name": "unsigned int"
                     }
                 }
             },
             "kind": "struct",
-            "size": 12
+            "size": 24
         },
         "_SERVICE_RECORD": {
             "fields": {
                 "DisplayName": {
-                    "offset": 8,
+                    "offset": 16,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "base",
                             "name": "unsigned short"
                         }
                     }
                 },
                 "DriverName": {
-                    "offset": 28,
+                    "offset": 48,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "base",
                             "name": "unsigned short"
                         }
                     }
                 },
                 "Order": {
-                    "offset": 12,
+                    "offset": 24,
                     "type": {
                         "kind": "base",
                         "name": "unsigned int"
                     }
                 },
-                "PrevEntry": {
-                    "offset": 0,
-                    "type": {
-                        "kind": "pointer",
-                        "subtype": {
-                            "kind": "struct",
-                            "name": "_SERVICE_RECORD"
-                        }
-                    }
-                },
                 "ServiceList": {
-                    "offset": 92,
+                    "offset": 0,
                     "type": {
                         "kind": "struct",
                         "name": "_SERVICE_LIST_ENTRY"
                     }
                 },
                 "ServiceName": {
-                    "offset": 4,
+                    "offset": 8,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "base",
                             "name": "unsigned short"
                         }
                     }
                 },
                 "ServiceProcess": {
-                    "offset": 28,
+                    "offset": 48,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_SERVICE_PROCESS"
                         }
                     }
                 },
                 "Start": {
-                    "offset": 60,
+                    "offset": 84,
                     "type": {
                         "kind": "enum",
                         "name": "StartEnum"
                     }
                 },
                 "State": {
-                    "offset": 36,
+                    "offset": 60,
                     "type": {
                         "kind": "enum",
                         "name": "StateEnum"
                     }
                 },
                 "Tag": {
-                    "offset": 24,
+                    "offset": 32,
                     "type": {
                         "count": 4,
                         "kind": "array",
                         "subtype": {
                             "kind": "base",
                             "name": "unsigned char"
                         }
                     }
                 },
                 "Type": {
-                    "offset": 32,
+                    "offset": 56,
                     "type": {
                         "kind": "base",
                         "name": "unsigned long"
                     }
                 }
             },
             "kind": "struct",
-            "size": 92
+            "size": 84
         }
     }
 }
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-win10-15063-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-15063-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-win10-15063-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-15063-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-win10-16299-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-16299-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-win10-16299-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-16299-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-win8-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win8-x64.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-win8-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win8-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-xp-2003-x64.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-win10-25398-x64.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868607954545455%*

 * *Differences: {"'metadata'": "{'producer': {'name': 'David McDonald', 'datetime': '2023-11-16T15:05:35-06:00'}}",*

 * * "'user_types'": "{'_SERVICE_PROCESS': {'fields': {'BinaryPath': {'offset': 24}, 'ProcessId': "*

 * *                 "{'offset': 40}}, 'size': 40}, '_SERVICE_RECORD': {'fields': {'DisplayName': "*

 * *                 "{'offset': 64}, 'ServiceProcess': {'offset': 336}, 'Start': {'offset': 36}, "*

 * *                 "'State': {'offset': 84}, 'ServiceName': {'offset': 56}, 'DriverName': {'offset': "*

 * *                 "296}, […]*

```diff
@@ -62,16 +62,16 @@
             },
             "size": 4
         }
     },
     "metadata": {
         "format": "4.1.0",
         "producer": {
-            "datetime": "2019-04-17T13:45:16.417006",
-            "name": "vtypes_to_json.py",
+            "datetime": "2023-11-16T15:05:35-06:00",
+            "name": "David McDonald",
             "version": "0.0.1"
         }
     },
     "symbols": {},
     "user_types": {
         "_SERVICE_HEADER": {
             "fields": {
@@ -125,99 +125,109 @@
             },
             "kind": "struct",
             "size": 16
         },
         "_SERVICE_PROCESS": {
             "fields": {
                 "BinaryPath": {
-                    "offset": 16,
+                    "offset": 24,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "base",
                             "name": "unsigned short"
                         }
                     }
                 },
                 "ProcessId": {
-                    "offset": 24,
+                    "offset": 40,
                     "type": {
                         "kind": "base",
                         "name": "unsigned int"
                     }
                 }
             },
             "kind": "struct",
-            "size": 24
+            "size": 40
         },
         "_SERVICE_RECORD": {
             "fields": {
                 "DisplayName": {
-                    "offset": 16,
+                    "offset": 64,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "base",
                             "name": "unsigned short"
                         }
                     }
                 },
                 "DriverName": {
-                    "offset": 48,
+                    "offset": 296,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "base",
                             "name": "unsigned short"
                         }
                     }
                 },
                 "Order": {
-                    "offset": 24,
+                    "offset": 32,
                     "type": {
                         "kind": "base",
                         "name": "unsigned int"
                     }
                 },
+                "PrevEntry": {
+                    "offset": 16,
+                    "type": {
+                        "kind": "pointer",
+                        "subtype": {
+                            "kind": "struct",
+                            "name": "_SERVICE_RECORD"
+                        }
+                    }
+                },
                 "ServiceList": {
                     "offset": 0,
                     "type": {
                         "kind": "struct",
                         "name": "_SERVICE_LIST_ENTRY"
                     }
                 },
                 "ServiceName": {
-                    "offset": 8,
+                    "offset": 56,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "base",
                             "name": "unsigned short"
                         }
                     }
                 },
                 "ServiceProcess": {
-                    "offset": 48,
+                    "offset": 336,
                     "type": {
                         "kind": "pointer",
                         "subtype": {
                             "kind": "struct",
                             "name": "_SERVICE_PROCESS"
                         }
                     }
                 },
                 "Start": {
-                    "offset": 84,
+                    "offset": 36,
                     "type": {
                         "kind": "enum",
                         "name": "StartEnum"
                     }
                 },
                 "State": {
-                    "offset": 60,
+                    "offset": 84,
                     "type": {
                         "kind": "enum",
                         "name": "StateEnum"
                     }
                 },
                 "Tag": {
                     "offset": 32,
@@ -227,19 +237,19 @@
                         "subtype": {
                             "kind": "base",
                             "name": "unsigned char"
                         }
                     }
                 },
                 "Type": {
-                    "offset": 56,
+                    "offset": 80,
                     "type": {
                         "kind": "base",
                         "name": "unsigned long"
                     }
                 }
             },
             "kind": "struct",
-            "size": 84
+            "size": 336
         }
     }
 }
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/services/services-xp-x86.json` & `volatility3-2.7.0/volatility3/framework/symbols/windows/services/services-xp-x86.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/windows/versions.py` & `volatility3-2.7.0/volatility3/framework/symbols/windows/versions.py`

 * *Files 12% similar despite different names*

```diff
@@ -147,19 +147,53 @@
         ("ObHeaderCookie", None, True),
         ("_HANDLE_TABLE", "HandleCount", False),
         ("_EPROCESS", "KeepAliveCounter", False),
         ("_EPROCESS", "ControlFlowGuardEnabled", False),
     ],
 )
 
+is_win10_17763_or_later = OsDistinguisher(
+    version_check=lambda x: x >= (10, 0, 17763),
+    fallback_checks=[
+        ("_EPROCESS", "TrustletIdentity", False),
+        ("ParentSecurityDomain", None, True),
+    ],
+)
+
+is_win10_18362_or_later = OsDistinguisher(
+    version_check=lambda x: x >= (10, 0, 18362),
+    fallback_checks=[
+        ("ObHeaderCookie", None, True),
+        ("_CM_CACHED_VALUE_INDEX", None, False),
+        ("_WNF_PROCESS_CONTEXT", None, True),
+    ],
+)
+
 is_win10_18363_or_later = OsDistinguisher(
     version_check=lambda x: x >= (10, 0, 18363),
     fallback_checks=[("_KQOS_GROUPING_SETS", None, True)],
 )
 
+is_win10_19041_or_later = OsDistinguisher(
+    version_check=lambda x: x >= (10, 0, 19041),
+    fallback_checks=[
+        ("_EPROCESS", "TimerResolutionIgnore", True),
+        ("_EPROCESS", "VmProcessorHostTransition", True),
+        ("_KQOS_GROUPING_SETS", None, True),
+    ],
+)
+
+is_win10_25398_or_later = OsDistinguisher(
+    version_check=lambda x: x >= (10, 0, 25398),
+    fallback_checks=[
+        ("_EPROCESS", "MmSlabIdentity", True),
+        ("_EPROCESS", "EnableProcessImpersonationLogging", True),
+    ],
+)
+
 is_windows_10 = OsDistinguisher(
     version_check=lambda x: x >= (10, 0),
     fallback_checks=[("ObHeaderCookie", None, True)],
 )
 
 is_windows_8_or_later = OsDistinguisher(
     version_check=lambda x: x >= (6, 2),
```

### Comparing `volatility3-2.5.2/volatility3/framework/symbols/wrappers.py` & `volatility3-2.7.0/volatility3/framework/symbols/wrappers.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/plugins/__init__.py` & `volatility3-2.7.0/volatility3/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/plugins/linux/__init__.py` & `volatility3-2.7.0/volatility3/plugins/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/plugins/mac/__init__.py` & `volatility3-2.7.0/volatility3/plugins/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/plugins/windows/__init__.py` & `volatility3-2.7.0/volatility3/plugins/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/plugins/windows/registry/__init__.py` & `volatility3-2.7.0/volatility3/plugins/windows/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/plugins/windows/registry/certificates.py` & `volatility3-2.7.0/volatility3/plugins/windows/registry/certificates.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/plugins/windows/statistics.py` & `volatility3-2.7.0/volatility3/plugins/windows/statistics.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/schemas/__init__.py` & `volatility3-2.7.0/volatility3/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/schemas/schema-0.1.0.json` & `volatility3-2.7.0/volatility3/schemas/schema-0.1.0.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/schemas/schema-2.0.0.json` & `volatility3-2.7.0/volatility3/schemas/schema-2.0.0.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/schemas/schema-2.1.0.json` & `volatility3-2.7.0/volatility3/schemas/schema-2.1.0.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/schemas/schema-4.0.0.json` & `volatility3-2.7.0/volatility3/schemas/schema-4.0.0.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/schemas/schema-4.1.0.json` & `volatility3-2.7.0/volatility3/schemas/schema-4.1.0.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/schemas/schema-6.0.0.json` & `volatility3-2.7.0/volatility3/schemas/schema-6.0.0.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/schemas/schema-6.1.0.json` & `volatility3-2.7.0/volatility3/schemas/schema-6.1.0.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3/schemas/schema-6.2.0.json` & `volatility3-2.7.0/volatility3/schemas/schema-6.2.0.json`

 * *Files identical despite different names*

### Comparing `volatility3-2.5.2/volatility3.egg-info/PKG-INFO` & `volatility3-2.7.0/volatility3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volatility3
-Version: 2.5.2
+Version: 2.7.0
 Summary: Memory forensics framework
 Home-page: https://github.com/volatilityfoundation/volatility3/
 Author: Volatility Foundation
 Author-email: volatility@volatilityfoundation.org
 License: VSL
 Project-URL: Bug Tracker, https://github.com/volatilityfoundation/volatility3/issues
 Project-URL: Documentation, https://volatility3.readthedocs.io/
```

### Comparing `volatility3-2.5.2/volatility3.egg-info/SOURCES.txt` & `volatility3-2.7.0/volatility3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 volatility3.egg-info/PKG-INFO
 volatility3.egg-info/SOURCES.txt
 volatility3.egg-info/dependency_links.txt
 volatility3.egg-info/entry_points.txt
 volatility3.egg-info/requires.txt
 volatility3.egg-info/top_level.txt
 volatility3/cli/__init__.py
+volatility3/cli/text_filter.py
 volatility3/cli/text_renderer.py
 volatility3/cli/volargparse.py
 volatility3/cli/volshell/__init__.py
 volatility3/cli/volshell/generic.py
 volatility3/cli/volshell/linux.py
 volatility3/cli/volshell/mac.py
 volatility3/cli/volshell/windows.py
@@ -118,14 +119,15 @@
 volatility3/framework/plugins/linux/check_modules.py
 volatility3/framework/plugins/linux/check_syscall.py
 volatility3/framework/plugins/linux/elfs.py
 volatility3/framework/plugins/linux/envars.py
 volatility3/framework/plugins/linux/iomem.py
 volatility3/framework/plugins/linux/keyboard_notifiers.py
 volatility3/framework/plugins/linux/kmsg.py
+volatility3/framework/plugins/linux/library_list.py
 volatility3/framework/plugins/linux/lsmod.py
 volatility3/framework/plugins/linux/lsof.py
 volatility3/framework/plugins/linux/malfind.py
 volatility3/framework/plugins/linux/mountinfo.py
 volatility3/framework/plugins/linux/proc.py
 volatility3/framework/plugins/linux/psaux.py
 volatility3/framework/plugins/linux/pslist.py
@@ -135,14 +137,15 @@
 volatility3/framework/plugins/linux/tty_check.py
 volatility3/framework/plugins/linux/vmayarascan.py
 volatility3/framework/plugins/mac/__init__.py
 volatility3/framework/plugins/mac/bash.py
 volatility3/framework/plugins/mac/check_syscall.py
 volatility3/framework/plugins/mac/check_sysctl.py
 volatility3/framework/plugins/mac/check_trap_table.py
+volatility3/framework/plugins/mac/dmesg.py
 volatility3/framework/plugins/mac/ifconfig.py
 volatility3/framework/plugins/mac/kauth_listeners.py
 volatility3/framework/plugins/mac/kauth_scopes.py
 volatility3/framework/plugins/mac/kevents.py
 volatility3/framework/plugins/mac/list_files.py
 volatility3/framework/plugins/mac/lsmod.py
 volatility3/framework/plugins/mac/lsof.py
@@ -171,14 +174,15 @@
 volatility3/framework/plugins/windows/dumpfiles.py
 volatility3/framework/plugins/windows/envars.py
 volatility3/framework/plugins/windows/filescan.py
 volatility3/framework/plugins/windows/getservicesids.py
 volatility3/framework/plugins/windows/getsids.py
 volatility3/framework/plugins/windows/handles.py
 volatility3/framework/plugins/windows/hashdump.py
+volatility3/framework/plugins/windows/iat.py
 volatility3/framework/plugins/windows/info.py
 volatility3/framework/plugins/windows/joblinks.py
 volatility3/framework/plugins/windows/ldrmodules.py
 volatility3/framework/plugins/windows/lsadump.py
 volatility3/framework/plugins/windows/malfind.py
 volatility3/framework/plugins/windows/mbrscan.py
 volatility3/framework/plugins/windows/memmap.py
@@ -196,14 +200,16 @@
 volatility3/framework/plugins/windows/sessions.py
 volatility3/framework/plugins/windows/sids_and_privileges.json
 volatility3/framework/plugins/windows/skeleton_key_check.py
 volatility3/framework/plugins/windows/ssdt.py
 volatility3/framework/plugins/windows/strings.py
 volatility3/framework/plugins/windows/svcscan.py
 volatility3/framework/plugins/windows/symlinkscan.py
+volatility3/framework/plugins/windows/thrdscan.py
+volatility3/framework/plugins/windows/truecrypt.py
 volatility3/framework/plugins/windows/vadinfo.py
 volatility3/framework/plugins/windows/vadwalk.py
 volatility3/framework/plugins/windows/vadyarascan.py
 volatility3/framework/plugins/windows/verinfo.py
 volatility3/framework/plugins/windows/virtmap.py
 volatility3/framework/plugins/windows/registry/__init__.py
 volatility3/framework/plugins/windows/registry/hivelist.py
@@ -293,14 +299,20 @@
 volatility3/framework/symbols/windows/netscan/netscan-win81-x86.json
 volatility3/framework/symbols/windows/services/services-vista-x64.json
 volatility3/framework/symbols/windows/services/services-vista-x86.json
 volatility3/framework/symbols/windows/services/services-win10-15063-x64.json
 volatility3/framework/symbols/windows/services/services-win10-15063-x86.json
 volatility3/framework/symbols/windows/services/services-win10-16299-x64.json
 volatility3/framework/symbols/windows/services/services-win10-16299-x86.json
+volatility3/framework/symbols/windows/services/services-win10-17763-x86.json
+volatility3/framework/symbols/windows/services/services-win10-18362-x64.json
+volatility3/framework/symbols/windows/services/services-win10-18362-x86.json
+volatility3/framework/symbols/windows/services/services-win10-19041-x64.json
+volatility3/framework/symbols/windows/services/services-win10-19041-x86.json
+volatility3/framework/symbols/windows/services/services-win10-25398-x64.json
 volatility3/framework/symbols/windows/services/services-win8-x64.json
 volatility3/framework/symbols/windows/services/services-win8-x86.json
 volatility3/framework/symbols/windows/services/services-xp-2003-x64.json
 volatility3/framework/symbols/windows/services/services-xp-x86.json
 volatility3/plugins/__init__.py
 volatility3/plugins/linux/__init__.py
 volatility3/plugins/mac/__init__.py
@@ -313,8 +325,9 @@
 volatility3/schemas/schema-2.0.0.json
 volatility3/schemas/schema-2.1.0.json
 volatility3/schemas/schema-4.0.0.json
 volatility3/schemas/schema-4.1.0.json
 volatility3/schemas/schema-6.0.0.json
 volatility3/schemas/schema-6.1.0.json
 volatility3/schemas/schema-6.2.0.json
+volatility3/schemas/schema-6.3.0.json
 volatility3/symbols/__init__.py
```

### Comparing `volatility3-2.5.2/volshell.spec` & `volatility3-2.7.0/volshell.spec`

 * *Files identical despite different names*

