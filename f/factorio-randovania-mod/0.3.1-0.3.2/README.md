# Comparing `tmp/factorio_randovania_mod-0.3.1.tar.gz` & `tmp/factorio_randovania_mod-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factorio_randovania_mod-0.3.1.tar", last modified: Mon May 27 13:37:45 2024, max compression
+gzip compressed data, was "factorio_randovania_mod-0.3.2.tar", last modified: Tue May 28 00:45:22 2024, max compression
```

## Comparing `factorio_randovania_mod-0.3.1.tar` & `factorio_randovania_mod-0.3.2.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.541919 factorio_randovania_mod-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.533919 factorio_randovania_mod-0.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.533919 factorio_randovania_mod-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-27 13:37:45.541919 factorio_randovania_mod-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:37:45.541919 factorio_randovania_mod-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.533919 factorio_randovania_mod-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.537919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.537919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/__pyinstaller/hook-factorio_randovania_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/configuration.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.537919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/files/
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/files/schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/locale_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.537919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/control.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/data-updates.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/data.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.533919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/graphics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.537919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/graphics/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.533919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.537919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/locale/en/
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.541919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/prototypes/
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/prototypes/burners.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/prototypes/tech.lua
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/mod_lua_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 13:37:45.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.541919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-27 13:37:45.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-27 13:37:45.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:37:45.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 13:37:45.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-27 13:37:45.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 13:37:45.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.541919 factorio_randovania_mod-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/tests/test_color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/tests/test_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.541919 factorio_randovania_mod-0.3.1/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)   117666 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/tests/test_files/patcher_a.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.535283 factorio_randovania_mod-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.527283 factorio_randovania_mod-0.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.527283 factorio_randovania_mod-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-28 00:45:22.535283 factorio_randovania_mod-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 00:45:22.535283 factorio_randovania_mod-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.523283 factorio_randovania_mod-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.527283 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.531283 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/__pyinstaller/hook-factorio_randovania_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/configuration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.531283 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/files/schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/locale_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.531283 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/control.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/data-updates.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/data.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.523283 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/graphics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.531283 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/graphics/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.523283 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.531283 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/locale/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.531283 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/prototypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/prototypes/burners.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/prototypes/modules.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/prototypes/tech.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/mod_lua_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 00:45:22.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.531283 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-28 00:45:22.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-28 00:45:22.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 00:45:22.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-28 00:45:22.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-28 00:45:22.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 00:45:22.000000 factorio_randovania_mod-0.3.2/src/factorio_randovania_mod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.531283 factorio_randovania_mod-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/tests/test_color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/tests/test_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:45:22.531283 factorio_randovania_mod-0.3.2/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)   117400 2024-05-28 00:45:12.000000 factorio_randovania_mod-0.3.2/tests/test_files/patcher_a.json
```

### Comparing `factorio_randovania_mod-0.3.1/.github/dependabot.yml` & `factorio_randovania_mod-0.3.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/.github/workflows/python.yml` & `factorio_randovania_mod-0.3.2/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/.gitignore` & `factorio_randovania_mod-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/.pre-commit-config.yaml` & `factorio_randovania_mod-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/LICENSE` & `factorio_randovania_mod-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/PKG-INFO` & `factorio_randovania_mod-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factorio-randovania-mod
-Version: 0.3.1
+Version: 0.3.2
 Summary: Generator of Factorio Randomizer mods for Randovania
 Author: Henrique Gemignani Passos Lima
 Project-URL: Homepage, https://github.com/randovania/factorio-randovania-mod
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `factorio_randovania_mod-0.3.1/pyproject.toml` & `factorio_randovania_mod-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/cli.py` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/cli.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/color_util.py` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/color_util.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/configuration.pyi` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/configuration.pyi`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/creator.py` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/creator.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/files/schema.json` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/files/schema.json`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/locale_lib.py` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/locale_lib.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/control.lua` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/control.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/data-updates.lua` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/data-updates.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/data.lua` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/data.lua`

 * *Files 16% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     -- science
     "lab"
 }
 
 require("prototypes.burners")
 require("prototypes.tech")
 require("prototypes.extra-tiers")
+require("prototypes.modules")
 
 ---- Lock all initial recipes
 
 for _, name in ipairs(kRecipesWithNewTech) do
     set_recipe_field(data.raw["recipe"][name], "enabled", false)
 end
 
@@ -170,8 +171,24 @@
 
 ---- Remove regular inserter capacity bonus from inserter-capacity-bonus-7
 remove_if(
     data.raw["technology"]["inserter-capacity-bonus-7"]["effects"],
     function(it)
         return it.type == "inserter-stack-size-bonus"
     end
-)
+)
+
+---- Make Solar and Accumulators better
+
+data.raw["solar-panel"]["solar-panel"].production = "240kW"
+data.raw["accumulator"]["accumulator"].energy_source = {
+    type = "electric",
+    buffer_capacity = "20MJ",
+    usage_priority = "tertiary",
+    input_flow_limit = "1200kW",
+    output_flow_limit = "1200kW"
+}
+
+---- Tweak Nuclear Reactor freebies 
+
+data.raw["item"]["steam-turbine"].stack_size = 50
+data.raw["item"]["nuclear-reactor"].stack_size = 5
```

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/prototypes/burners.lua` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/prototypes/burners.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/prototypes/tech.lua` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_src/prototypes/tech.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_util.py` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/lua_util.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/mod_lua_api.py` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/mod_lua_api.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/schema.py` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod/schema.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/PKG-INFO` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factorio-randovania-mod
-Version: 0.3.1
+Version: 0.3.2
 Summary: Generator of Factorio Randomizer mods for Randovania
 Author: Henrique Gemignani Passos Lima
 Project-URL: Homepage, https://github.com/randovania/factorio-randovania-mod
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/SOURCES.txt` & `factorio_randovania_mod-0.3.2/src/factorio_randovania_mod.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,12 +32,13 @@
 src/factorio_randovania_mod/lua_src/data-updates.lua
 src/factorio_randovania_mod/lua_src/data.lua
 src/factorio_randovania_mod/lua_src/info.json
 src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png
 src/factorio_randovania_mod/lua_src/locale/en/strings.cfg
 src/factorio_randovania_mod/lua_src/prototypes/burners.lua
 src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua
+src/factorio_randovania_mod/lua_src/prototypes/modules.lua
 src/factorio_randovania_mod/lua_src/prototypes/tech.lua
 tests/conftest.py
 tests/test_color_util.py
 tests/test_creator.py
 tests/test_files/patcher_a.json
```

### Comparing `factorio_randovania_mod-0.3.1/tests/test_files/patcher_a.json` & `factorio_randovania_mod-0.3.2/tests/test_files/patcher_a.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8663700810185183%*

 * *Differences: {"'configuration_identifier'": "'XXXXXXXX'",*

 * * "'recipes'": "{0: {'ingredients': {0: {'name': 'copper-plate'}, 1: {'name': 'stone-brick'}}}, 1: "*

 * *              "{'ingredients': {1: {'name': 'copper-plate'}, 2: {'name': 'small-lamp'}, delete: "*

 * *              "[3, 0]}}, 2: {'ingredients': {0: {'amount': 350}, 1: {'name': 'splitter'}}}, 3: "*

 * *              "{'ingredients': {2: {'name': 'fast-underground-belt'}, insert: [(1, "*

 * *              "OrderedDict([('name', 'concrete'), ('amount', 2), ('type', 'item')]))]}} […]*

```diff
@@ -1,71 +1,61 @@
 {
-    "configuration_identifier": "<sample>",
+    "configuration_identifier": "XXXXXXXX",
     "layout_uuid": "00000000-0000-1111-0000-000000000000",
     "recipes": [
         {
             "category": "crafting",
             "ingredients": [
                 {
                     "amount": 1,
-                    "name": "copper-ore",
+                    "name": "copper-plate",
                     "type": "item"
                 },
                 {
                     "amount": 1,
-                    "name": "iron-gear-wheel",
+                    "name": "stone-brick",
                     "type": "item"
                 }
             ],
             "recipe_name": "automation-science-pack",
             "result_amount": 1
         },
         {
             "category": "crafting",
             "ingredients": [
                 {
                     "amount": 1,
-                    "name": "copper-ore",
-                    "type": "item"
-                },
-                {
-                    "amount": 1,
                     "name": "stone",
                     "type": "item"
                 },
                 {
                     "amount": 1,
-                    "name": "discharge-defense-remote",
-                    "type": "item"
-                },
-                {
-                    "amount": 2,
-                    "name": "iron-stick",
+                    "name": "copper-plate",
                     "type": "item"
                 },
                 {
                     "amount": 1,
-                    "name": "transport-belt",
+                    "name": "small-lamp",
                     "type": "item"
                 }
             ],
             "recipe_name": "logistic-science-pack",
             "result_amount": 1
         },
         {
             "category": "crafting-with-fluid",
             "ingredients": [
                 {
-                    "amount": 150,
+                    "amount": 350,
                     "name": "water",
                     "type": "fluid"
                 },
                 {
                     "amount": 1,
-                    "name": "uranium-238",
+                    "name": "splitter",
                     "type": "item"
                 }
             ],
             "recipe_name": "military-science-pack",
             "result_amount": 1
         },
         {
@@ -73,117 +63,117 @@
             "ingredients": [
                 {
                     "amount": 10,
                     "name": "steam",
                     "type": "fluid"
                 },
                 {
+                    "amount": 2,
+                    "name": "concrete",
+                    "type": "item"
+                },
+                {
                     "amount": 1,
-                    "name": "lab",
+                    "name": "fast-underground-belt",
                     "type": "item"
                 },
                 {
                     "amount": 2,
                     "name": "hazard-concrete",
                     "type": "item"
                 }
             ],
             "recipe_name": "chemical-science-pack",
             "result_amount": 1
         },
         {
-            "category": "crafting-with-fluid",
+            "category": "crafting",
             "ingredients": [
                 {
-                    "amount": 100,
-                    "name": "water",
-                    "type": "fluid"
+                    "amount": 13,
+                    "name": "coal",
+                    "type": "item"
                 },
                 {
                     "amount": 3,
                     "name": "copper-cable",
                     "type": "item"
                 },
                 {
                     "amount": 1,
                     "name": "processing-unit",
                     "type": "item"
                 },
                 {
+                    "amount": 2,
+                    "name": "iron-gear-wheel",
+                    "type": "item"
+                },
+                {
                     "amount": 1,
-                    "name": "steam-engine",
+                    "name": "arithmetic-combinator",
                     "type": "item"
                 }
             ],
             "recipe_name": "production-science-pack",
             "result_amount": 1
         },
         {
-            "category": "crafting",
+            "category": "crafting-with-fluid",
             "ingredients": [
                 {
-                    "amount": 3,
-                    "name": "coal",
+                    "amount": 1,
+                    "name": "uranium-ore",
                     "type": "item"
                 },
                 {
-                    "amount": 7,
-                    "name": "iron-gear-wheel",
-                    "type": "item"
+                    "amount": 30,
+                    "name": "heavy-oil",
+                    "type": "fluid"
                 },
                 {
                     "amount": 2,
-                    "name": "discharge-defense-remote",
-                    "type": "item"
-                },
-                {
-                    "amount": 8,
-                    "name": "pipe",
+                    "name": "iron-stick",
                     "type": "item"
                 },
                 {
                     "amount": 1,
-                    "name": "rail",
+                    "name": "military-science-pack",
                     "type": "item"
                 },
                 {
                     "amount": 1,
-                    "name": "logistic-robot",
+                    "name": "production-science-pack",
                     "type": "item"
                 }
             ],
             "recipe_name": "utility-science-pack",
             "result_amount": 1
         },
         {
             "category": "rocket-building",
             "ingredients": [
                 {
-                    "amount": 3,
-                    "name": "energy-shield-equipment",
-                    "type": "item"
-                },
-                {
-                    "amount": 17,
-                    "name": "iron-stick",
+                    "amount": 1,
+                    "name": "coal",
                     "type": "item"
                 },
                 {
-                    "amount": 1,
-                    "name": "repair-pack",
+                    "amount": 2,
+                    "name": "copper-cable",
                     "type": "item"
                 },
                 {
                     "amount": 2,
-                    "name": "big-electric-pole",
+                    "name": "personal-roboport-equipment",
                     "type": "item"
                 },
                 {
                     "amount": 1,
-                    "name": "centrifuge",
+                    "name": "chemical-science-pack",
                     "type": "item"
                 }
             ],
             "recipe_name": "rocket-part",
             "result_amount": 1
         }
     ],
@@ -196,842 +186,850 @@
                 "count": 10,
                 "ingredients": [
                     "automation-science-pack"
                 ],
                 "time": 15
             },
             "description": "",
-            "icon": "__base__/graphics/technology/rocket-control-unit.png",
-            "icon_size": 256,
-            "locale_name": "Rocket Control Unit",
+            "icon": "__base__/graphics/icons/steam-engine.png",
+            "icon_size": 64,
+            "locale_name": "Steam Power",
             "prerequisites": [],
             "tech_name": "randovania-military",
             "unlocks": [
-                "rocket-control-unit"
+                "steam-power"
             ]
         },
         {
             "cost": {
                 "count": 10,
                 "ingredients": [
                     "automation-science-pack"
                 ],
                 "time": 10
             },
-            "description": "Provides the following in order: Inserter, Fast inserter, Stack inserter.",
-            "icon": "__base__/graphics/technology/fast-inserter.png",
+            "description": "Provides the following in order: Energy shield, Energy shield MK2.",
+            "icon": "__base__/graphics/technology/energy-shield-equipment.png",
             "icon_size": 256,
-            "locale_name": "Inserter",
+            "locale_name": "Energy Shield Equipment",
             "prerequisites": [],
             "tech_name": "randovania-automation",
             "unlocks": [
-                "inserter",
-                "fast-inserter",
-                "stack-inserter"
+                "energy-shield-equipment",
+                "energy-shield-mk2-equipment"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack"
                 ],
                 "time": 5
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/solar-energy.png",
+            "description": "Provides the following in order: Electronics, Advanced electronics, Advanced electronics 2.",
+            "icon": "__base__/graphics/technology/electronics.png",
             "icon_size": 256,
-            "locale_name": "Solar Panel",
+            "locale_name": "Electronics",
             "prerequisites": [],
             "tech_name": "randovania-steel-processing",
             "unlocks": [
-                "solar-energy"
+                "electronics",
+                "advanced-electronics",
+                "advanced-electronics-2"
             ]
         },
         {
             "cost": {
                 "count": 75,
                 "ingredients": [
                     "automation-science-pack"
                 ],
                 "time": 5
             },
             "description": "",
-            "icon": "__base__/graphics/technology/research-speed.png",
+            "icon": "__base__/graphics/technology/logistic-science-pack.png",
             "icon_size": 256,
-            "locale_name": "Research Productivity",
+            "locale_name": "Logistic Science Pack",
             "prerequisites": [],
             "tech_name": "randovania-logistic-science-pack",
             "unlocks": [
-                "research-productivity"
+                "logistic-science-pack"
             ]
         },
         {
             "cost": {
                 "count": 20,
                 "ingredients": [
                     "automation-science-pack"
                 ],
                 "time": 15
             },
             "description": "",
-            "icon": "__base__/graphics/technology/logistic-science-pack.png",
+            "icon": "__base__/graphics/technology/lamp.png",
             "icon_size": 256,
-            "locale_name": "Logistic Science Pack",
+            "locale_name": "Optics",
             "prerequisites": [],
             "tech_name": "randovania-logistics",
             "unlocks": [
-                "logistic-science-pack"
+                "optics"
             ]
         },
         {
             "cost": {
                 "count": 10,
                 "ingredients": [
                     "automation-science-pack"
                 ],
                 "time": 15
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/worker-robots-storage.png",
+            "description": "Provides the following in order: Logistics, Logistics 2, Logistics 3.",
+            "icon": "__base__/graphics/technology/logistics-1.png",
             "icon_size": 256,
-            "locale_name": "Worker Robots Storage",
+            "locale_name": "Logistics",
             "prerequisites": [],
             "tech_name": "randovania-optics",
             "unlocks": [
-                "worker-robots-storage-3"
+                "logistics",
+                "logistics-2",
+                "logistics-3"
             ]
         },
         {
             "cost": {
                 "count": 10,
                 "ingredients": [
                     "automation-science-pack"
                 ],
                 "time": 10
             },
-            "description": "Provides the following in order: Defender, Distractor, Destroyer.",
-            "icon": "__base__/graphics/technology/defender.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/electric-energy-acumulators.png",
             "icon_size": 256,
-            "locale_name": "Follower Capsule",
+            "locale_name": "Accumulator",
             "prerequisites": [],
             "tech_name": "randovania-gun-turret",
             "unlocks": [
-                "defender",
-                "distractor",
-                "destroyer"
+                "electric-energy-accumulators"
             ]
         },
         {
             "cost": {
                 "count": 10,
                 "ingredients": [
                     "automation-science-pack"
                 ],
                 "time": 10
             },
-            "description": "Provides the following in order: Logistics, Logistics 2, Logistics 3.",
-            "icon": "__base__/graphics/technology/logistics-1.png",
+            "description": "Provides the following in order: Personal battery, Personal battery MK2.",
+            "icon": "__base__/graphics/technology/battery-equipment.png",
             "icon_size": 256,
-            "locale_name": "Logistics",
+            "locale_name": "Battery Equipment",
             "prerequisites": [],
             "tech_name": "randovania-stone-wall",
             "unlocks": [
-                "logistics",
-                "logistics-2",
-                "logistics-3"
+                "battery-equipment",
+                "battery-mk2-equipment"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Personal battery, Personal battery MK2.",
-            "icon": "__base__/graphics/technology/battery-equipment.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/worker-robots-storage.png",
             "icon_size": 256,
-            "locale_name": "Battery Equipment",
+            "locale_name": "Worker Robots Storage",
             "prerequisites": [
                 "randovania-military"
             ],
-            "tech_name": "randovania-physical-projectile-damage-1",
+            "tech_name": "randovania-physical-projectile-damage-b",
             "unlocks": [
-                "battery-equipment",
-                "battery-mk2-equipment"
+                "worker-robots-storage-3"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/worker-robots-speed.png",
+            "description": "Provides the following in order: Defender, Distractor, Destroyer.",
+            "icon": "__base__/graphics/technology/defender.png",
             "icon_size": 256,
-            "locale_name": "Worker Robots Speed",
+            "locale_name": "Follower Capsule",
             "prerequisites": [
                 "randovania-military"
             ],
-            "tech_name": "randovania-weapon-shooting-speed-1",
+            "tech_name": "randovania-weapon-shooting-speed-b",
             "unlocks": [
-                "worker-robots-speed-6"
+                "defender",
+                "distractor",
+                "destroyer"
             ]
         },
         {
             "cost": {
                 "count": 30,
                 "ingredients": [
                     "automation-science-pack"
                 ],
                 "time": 15
             },
             "description": "",
-            "icon": "__base__/graphics/icons/steam-engine.png",
-            "icon_size": 64,
-            "locale_name": "Steam Power",
+            "icon": "__base__/graphics/technology/logistic-system.png",
+            "icon_size": 256,
+            "locale_name": "Logistic System",
             "prerequisites": [
                 "randovania-automation"
             ],
             "tech_name": "randovania-electronics",
             "unlocks": [
-                "steam-power"
+                "logistic-system"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/discharge-defense-equipment.png",
+            "description": "Provides the following in order: Logistics, Logistics 2, Logistics 3.",
+            "icon": "__base__/graphics/technology/logistics-1.png",
             "icon_size": 256,
-            "locale_name": "Discharge Defense Equipment",
+            "locale_name": "Logistics",
             "prerequisites": [
                 "randovania-steel-processing"
             ],
             "tech_name": "randovania-steel-axe",
             "unlocks": [
-                "discharge-defense-equipment"
+                "logistics",
+                "logistics-2",
+                "logistics-3"
             ]
         },
         {
             "cost": {
                 "count": 30,
                 "ingredients": [
                     "automation-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Automation, Automation 2, Automation 3.",
-            "icon": "__base__/graphics/technology/automation-1.png",
+            "description": "Provides the following in order: Inserter, Fast inserter, Stack inserter.",
+            "icon": "__base__/graphics/technology/fast-inserter.png",
             "icon_size": 256,
-            "locale_name": "Assembly Machine",
+            "locale_name": "Inserter",
             "prerequisites": [
                 "randovania-military",
                 "randovania-steel-processing"
             ],
             "tech_name": "randovania-heavy-armor",
             "unlocks": [
-                "automation",
-                "automation-2",
-                "automation-3"
+                "inserter",
+                "fast-inserter",
+                "stack-inserter"
             ]
         },
         {
             "cost": {
                 "count": 20,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 15
             },
-            "description": "Provides the following in order: Oil processing, Advanced oil processing.",
-            "icon": "__base__/graphics/technology/oil-gathering.png",
+            "description": "Provides the following in order: Automation, Automation 2, Automation 3.",
+            "icon": "__base__/graphics/technology/automation-1.png",
             "icon_size": 256,
-            "locale_name": "Oil Processing",
+            "locale_name": "Assembly Machine",
             "prerequisites": [
                 "randovania-military",
                 "randovania-steel-processing",
                 "randovania-logistic-science-pack"
             ],
-            "tech_name": "randovania-military-2",
+            "tech_name": "randovania-military-c",
             "unlocks": [
-                "oil-processing",
-                "advanced-oil-processing"
+                "automation",
+                "automation-2",
+                "automation-3"
             ]
         },
         {
             "cost": {
                 "count": 75,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/toolbelt.png",
+            "description": "Provides the following in order: Military, Military 2, Military 3, Military 4.",
+            "icon": "__base__/graphics/technology/military.png",
             "icon_size": 256,
-            "locale_name": "Toolbelt",
+            "locale_name": "Military",
             "prerequisites": [
                 "randovania-steel-processing",
                 "randovania-logistic-science-pack"
             ],
             "tech_name": "randovania-advanced-material-processing",
             "unlocks": [
-                "toolbelt"
+                "military",
+                "military-2",
+                "military-3",
+                "military-4"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 15
             },
-            "description": "Provides the following in order: Automation, Automation 2, Automation 3.",
-            "icon": "__base__/graphics/technology/automation-1.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/steel-processing.png",
             "icon_size": 256,
-            "locale_name": "Assembly Machine",
+            "locale_name": "Steel Processing",
             "prerequisites": [
                 "randovania-steel-processing",
                 "randovania-logistic-science-pack"
             ],
             "tech_name": "randovania-engine",
             "unlocks": [
-                "automation",
-                "automation-2",
-                "automation-3"
+                "steel-processing"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Logistics, Logistics 2, Logistics 3.",
-            "icon": "__base__/graphics/technology/logistics-1.png",
+            "description": "Provides the following in order: Automation, Automation 2, Automation 3.",
+            "icon": "__base__/graphics/technology/automation-1.png",
             "icon_size": 256,
-            "locale_name": "Logistics",
+            "locale_name": "Assembly Machine",
             "prerequisites": [
                 "randovania-logistic-science-pack"
             ],
             "tech_name": "randovania-landfill",
             "unlocks": [
-                "logistics",
-                "logistics-2",
-                "logistics-3"
+                "automation",
+                "automation-2",
+                "automation-3"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/rocket-fuel.png",
+            "description": "Provides the following in order: Defender, Distractor, Destroyer.",
+            "icon": "__base__/graphics/technology/defender.png",
             "icon_size": 256,
-            "locale_name": "Rocket Fuel",
+            "locale_name": "Follower Capsule",
             "prerequisites": [
                 "randovania-logistic-science-pack"
             ],
             "tech_name": "randovania-toolbelt",
             "unlocks": [
-                "rocket-fuel"
+                "defender",
+                "distractor",
+                "destroyer"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Productivity module, Productivity module 2, Productivity module 3.",
-            "icon": "__base__/graphics/technology/productivity-module-1.png",
+            "description": "Provides the following in order: Inserter, Fast inserter, Stack inserter.",
+            "icon": "__base__/graphics/technology/fast-inserter.png",
             "icon_size": 256,
-            "locale_name": "Productivity Module",
+            "locale_name": "Inserter",
             "prerequisites": [
                 "randovania-logistic-science-pack",
                 "randovania-logistics"
             ],
-            "tech_name": "randovania-logistics-2",
+            "tech_name": "randovania-logistics-c",
             "unlocks": [
-                "productivity-module",
-                "productivity-module-2",
-                "productivity-module-3"
+                "inserter",
+                "fast-inserter",
+                "stack-inserter"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/battery.png",
+            "icon": "__base__/graphics/technology/mining-productivity.png",
             "icon_size": 256,
-            "locale_name": "Battery",
+            "locale_name": "Mining Productivity",
             "prerequisites": [
-                "randovania-physical-projectile-damage-1"
+                "randovania-physical-projectile-damage-b"
             ],
-            "tech_name": "randovania-physical-projectile-damage-2",
+            "tech_name": "randovania-physical-projectile-damage-c",
             "unlocks": [
-                "battery"
+                "mining-productivity-4"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/worker-robots-speed.png",
+            "icon": "__base__/graphics/technology/fast-inserter.png",
             "icon_size": 256,
-            "locale_name": "Worker Robots Speed",
+            "locale_name": "Longer Handed inserter",
             "prerequisites": [
-                "randovania-weapon-shooting-speed-1"
+                "randovania-weapon-shooting-speed-b"
             ],
-            "tech_name": "randovania-weapon-shooting-speed-2",
+            "tech_name": "randovania-weapon-shooting-speed-c",
             "unlocks": [
-                "worker-robots-speed-6"
+                "longer-handed-inserter"
             ]
         },
         {
             "cost": {
                 "count": 40,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 15
             },
             "description": "",
-            "icon": "__base__/graphics/technology/braking-force.png",
+            "icon": "__base__/graphics/technology/construction-robotics.png",
             "icon_size": 256,
-            "locale_name": "Braking Force",
+            "locale_name": "Construction Robotics",
             "prerequisites": [
                 "randovania-steel-processing",
                 "randovania-logistic-science-pack",
                 "randovania-electronics"
             ],
-            "tech_name": "randovania-automation-2",
+            "tech_name": "randovania-automation-c",
             "unlocks": [
-                "braking-force-7"
+                "construction-robotics"
             ]
         },
         {
             "cost": {
                 "count": 30,
                 "ingredients": [
                     "automation-science-pack"
                 ],
                 "time": 15
             },
-            "description": "Provides the following in order: Electronics, Advanced electronics, Advanced electronics 2.",
-            "icon": "__base__/graphics/technology/electronics.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/advanced-material-processing.png",
             "icon_size": 256,
-            "locale_name": "Electronics",
+            "locale_name": "Steel Furnace",
             "prerequisites": [
                 "randovania-electronics"
             ],
             "tech_name": "randovania-fast-inserter",
             "unlocks": [
-                "electronics",
-                "advanced-electronics",
-                "advanced-electronics-2"
+                "advanced-material-processing"
             ]
         },
         {
             "cost": {
                 "count": 250,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/railway.png",
+            "description": "Provides the following in order: Energy shield, Energy shield MK2.",
+            "icon": "__base__/graphics/technology/energy-shield-equipment.png",
             "icon_size": 256,
-            "locale_name": "Railway",
+            "locale_name": "Energy Shield Equipment",
             "prerequisites": [
                 "randovania-steel-processing",
                 "randovania-logistic-science-pack",
                 "randovania-optics",
                 "randovania-electronics"
             ],
             "tech_name": "randovania-solar-energy",
             "unlocks": [
-                "railway"
+                "energy-shield-equipment",
+                "energy-shield-mk2-equipment"
             ]
         },
         {
             "cost": {
                 "count": 120,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/research-speed.png",
+            "icon": "__base__/graphics/technology/discharge-defense-equipment.png",
             "icon_size": 256,
-            "locale_name": "Research Productivity",
+            "locale_name": "Discharge Defense Equipment",
             "prerequisites": [
                 "randovania-steel-processing",
                 "randovania-logistic-science-pack",
                 "randovania-electronics"
             ],
-            "tech_name": "randovania-electric-energy-distribution-1",
+            "tech_name": "randovania-electric-energy-distribution-b",
             "unlocks": [
-                "research-productivity"
+                "discharge-defense-equipment"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 15
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/construction-robotics.png",
+            "description": "Provides the following in order: Defender, Distractor, Destroyer.",
+            "icon": "__base__/graphics/technology/defender.png",
             "icon_size": 256,
-            "locale_name": "Construction Robotics",
+            "locale_name": "Follower Capsule",
             "prerequisites": [
                 "randovania-logistic-science-pack",
                 "randovania-electronics"
             ],
             "tech_name": "randovania-circuit-network",
             "unlocks": [
-                "construction-robotics"
+                "defender",
+                "distractor",
+                "destroyer"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/concrete.png",
+            "description": "Provides the following in order: Efficiency module, Efficiency module 2, Efficiency module 3.",
+            "icon": "__base__/graphics/technology/effectivity-module-1.png",
             "icon_size": 256,
-            "locale_name": "Concrete",
+            "locale_name": "Efficiency Module",
             "prerequisites": [
-                "randovania-military-2"
+                "randovania-military-c"
             ],
-            "tech_name": "randovania-stronger-explosives-1",
+            "tech_name": "randovania-stronger-explosives-b",
             "unlocks": [
-                "concrete"
+                "effectivity-module",
+                "effectivity-module-2",
+                "effectivity-module-3"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/advanced-material-processing.png",
+            "icon": "__base__/graphics/technology/electric-energy-distribution-1.png",
             "icon_size": 256,
-            "locale_name": "Steel Furnace",
+            "locale_name": "Big Electric Pole",
             "prerequisites": [
                 "randovania-stone-wall",
-                "randovania-military-2"
+                "randovania-military-c"
             ],
             "tech_name": "randovania-gate",
             "unlocks": [
-                "advanced-material-processing"
+                "big-electric-pole"
             ]
         },
         {
             "cost": {
                 "count": 30,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 15
             },
-            "description": "Provides the following in order: Inserter, Fast inserter, Stack inserter.",
-            "icon": "__base__/graphics/technology/fast-inserter.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/railway.png",
             "icon_size": 256,
-            "locale_name": "Inserter",
+            "locale_name": "Railway",
             "prerequisites": [
                 "randovania-stone-wall",
-                "randovania-military-2"
+                "randovania-military-c"
             ],
             "tech_name": "randovania-military-science-pack",
             "unlocks": [
-                "inserter",
-                "fast-inserter",
-                "stack-inserter"
+                "railway"
             ]
         },
         {
             "cost": {
                 "count": 75,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Personal battery, Personal battery MK2.",
-            "icon": "__base__/graphics/technology/battery-equipment.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/worker-robots-storage.png",
             "icon_size": 256,
-            "locale_name": "Battery Equipment",
+            "locale_name": "Worker Robots Storage",
             "prerequisites": [
                 "randovania-engine",
-                "randovania-logistics-2"
+                "randovania-logistics-c"
             ],
             "tech_name": "randovania-railway",
             "unlocks": [
-                "battery-equipment",
-                "battery-mk2-equipment"
+                "worker-robots-storage-3"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/inserter-capacity.png",
+            "icon": "__base__/graphics/technology/automobilism.png",
             "icon_size": 256,
-            "locale_name": "Regular Inserter Capacity Bonus",
+            "locale_name": "Car",
             "prerequisites": [
                 "randovania-engine",
-                "randovania-logistics-2"
+                "randovania-logistics-c"
             ],
             "tech_name": "randovania-automobilism",
             "unlocks": [
-                "regular-inserter-capacity-bonus"
+                "automobilism"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/laser-turret.png",
+            "description": "Provides the following in order: Rocketry, Explosive rocketry.",
+            "icon": "__base__/graphics/technology/rocketry.png",
             "icon_size": 256,
-            "locale_name": "Laser Turret",
+            "locale_name": "Rocketry",
             "prerequisites": [
-                "randovania-automation-2"
+                "randovania-automation-c"
             ],
-            "tech_name": "randovania-research-speed-1",
+            "tech_name": "randovania-research-speed-b",
             "unlocks": [
-                "laser-turret"
+                "rocketry",
+                "explosive-rocketry"
             ]
         },
         {
             "cost": {
                 "count": 250,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Personal roboport, Personal roboport MK2.",
-            "icon": "__base__/graphics/technology/personal-roboport-equipment.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/military-science-pack.png",
             "icon_size": 256,
-            "locale_name": "Personal Roboport Equipment",
+            "locale_name": "Military Science Pack",
             "prerequisites": [
                 "randovania-advanced-material-processing",
-                "randovania-automation-2"
+                "randovania-automation-c"
             ],
             "tech_name": "randovania-concrete",
             "unlocks": [
-                "personal-roboport-equipment",
-                "personal-roboport-mk2-equipment"
+                "military-science-pack"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 15
             },
             "description": "",
-            "icon": "__base__/graphics/technology/steel-processing.png",
+            "icon": "__base__/graphics/technology/gun-turret.png",
             "icon_size": 256,
-            "locale_name": "Steel Processing",
+            "locale_name": "Gun Turret",
             "prerequisites": [
                 "randovania-engine",
-                "randovania-automation-2"
+                "randovania-automation-c"
             ],
             "tech_name": "randovania-fluid-handling",
             "unlocks": [
-                "steel-processing"
+                "gun-turret"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Speed module, Speed module 2, Speed module 3.",
-            "icon": "__base__/graphics/technology/speed-module-1.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/research-speed.png",
             "icon_size": 256,
-            "locale_name": "Speed Module",
+            "locale_name": "Research Speed",
             "prerequisites": [
-                "randovania-stronger-explosives-1"
+                "randovania-stronger-explosives-b"
             ],
-            "tech_name": "randovania-stronger-explosives-2",
+            "tech_name": "randovania-stronger-explosives-c",
             "unlocks": [
-                "speed-module",
-                "speed-module-2",
-                "speed-module-3"
+                "research-speed-6"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Military, Military 2, Military 3, Military 4.",
-            "icon": "__base__/graphics/technology/military.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/research-speed.png",
             "icon_size": 256,
-            "locale_name": "Military",
+            "locale_name": "Research Productivity",
             "prerequisites": [
                 "randovania-military-science-pack"
             ],
             "tech_name": "randovania-defender",
             "unlocks": [
-                "military",
-                "military-2",
-                "military-3",
-                "military-4"
+                "research-productivity"
             ]
         },
         {
             "cost": {
                 "count": 75,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/research-speed.png",
+            "description": "Provides the following in order: Military, Military 2, Military 3, Military 4.",
+            "icon": "__base__/graphics/technology/military.png",
             "icon_size": 256,
-            "locale_name": "Research Speed",
+            "locale_name": "Military",
             "prerequisites": [
                 "randovania-railway"
             ],
             "tech_name": "randovania-automated-rail-transportation",
             "unlocks": [
-                "research-speed-6"
+                "military",
+                "military-2",
+                "military-3",
+                "military-4"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/fusion-reactor-equipment.png",
+            "icon": "__base__/graphics/technology/plastics.png",
             "icon_size": 256,
-            "locale_name": "Fusion Reactor Equipment",
+            "locale_name": "Plastics",
             "prerequisites": [
-                "randovania-research-speed-1"
+                "randovania-research-speed-b"
             ],
-            "tech_name": "randovania-research-speed-2",
+            "tech_name": "randovania-research-speed-c",
             "unlocks": [
-                "fusion-reactor-equipment"
+                "plastics"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/fluid-handling.png",
+            "description": "Provides the following in order: Military, Military 2, Military 3, Military 4.",
+            "icon": "__base__/graphics/technology/military.png",
             "icon_size": 256,
-            "locale_name": "Fluid Handling",
+            "locale_name": "Military",
             "prerequisites": [
                 "randovania-railway",
                 "randovania-fluid-handling"
             ],
             "tech_name": "randovania-fluid-wagon",
             "unlocks": [
-                "fluid-handling"
+                "military",
+                "military-2",
+                "military-3",
+                "military-4"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
@@ -1058,570 +1056,562 @@
                     "automation-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/exoskeleton-equipment.png",
+            "icon": "__base__/graphics/technology/fluid-wagon.png",
             "icon_size": 256,
-            "locale_name": "Exoskeleton Equipment",
+            "locale_name": "Fluid Wagon",
             "prerequisites": [
                 "randovania-defender"
             ],
-            "tech_name": "randovania-follower-robot-count-1",
+            "tech_name": "randovania-follower-robot-count-b",
             "unlocks": [
-                "exoskeleton-equipment"
+                "fluid-wagon"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/coal-liquefaction.png",
+            "description": "Provides the following in order: Light armor, Heavy armor.",
+            "icon": "__base__/graphics/technology/heavy-armor.png",
             "icon_size": 256,
-            "locale_name": "Coal Liquefaction",
+            "locale_name": "Armor",
             "prerequisites": [
                 "randovania-automated-rail-transportation"
             ],
             "tech_name": "randovania-rail-signals",
             "unlocks": [
-                "coal-liquefaction"
+                "light-armor",
+                "heavy-armor"
             ]
         },
         {
             "cost": {
                 "count": 250,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Military, Military 2, Military 3, Military 4.",
-            "icon": "__base__/graphics/technology/military.png",
+            "description": "Provides the following in order: Efficiency module, Efficiency module 2, Efficiency module 3.",
+            "icon": "__base__/graphics/technology/effectivity-module-1.png",
             "icon_size": 256,
-            "locale_name": "Military",
+            "locale_name": "Efficiency Module",
             "prerequisites": [
-                "randovania-research-speed-2"
+                "randovania-research-speed-c"
             ],
-            "tech_name": "randovania-research-speed-3",
+            "tech_name": "randovania-research-speed-d",
             "unlocks": [
-                "military",
-                "military-2",
-                "military-3",
-                "military-4"
+                "effectivity-module",
+                "effectivity-module-2",
+                "effectivity-module-3"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Efficiency module, Efficiency module 2, Efficiency module 3.",
-            "icon": "__base__/graphics/technology/effectivity-module-1.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/uranium-ammo.png",
             "icon_size": 256,
-            "locale_name": "Efficiency Module",
+            "locale_name": "Uranium Ammo",
             "prerequisites": [
                 "randovania-oil-processing"
             ],
             "tech_name": "randovania-flammables",
             "unlocks": [
-                "effectivity-module",
-                "effectivity-module-2",
-                "effectivity-module-3"
+                "uranium-ammo"
             ]
         },
         {
             "cost": {
                 "count": 150,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/landfill.png",
+            "description": "Provides the following in order: Productivity module, Productivity module 2, Productivity module 3.",
+            "icon": "__base__/graphics/technology/productivity-module-1.png",
             "icon_size": 256,
-            "locale_name": "Landfill",
+            "locale_name": "Productivity Module",
             "prerequisites": [
                 "randovania-oil-processing"
             ],
             "tech_name": "randovania-sulfur-processing",
             "unlocks": [
-                "landfill"
+                "productivity-module",
+                "productivity-module-2",
+                "productivity-module-3"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/gun-turret.png",
+            "icon": "__base__/graphics/technology/low-density-structure.png",
             "icon_size": 256,
-            "locale_name": "Gun Turret",
+            "locale_name": "Low Density Structure",
             "prerequisites": [
                 "randovania-oil-processing"
             ],
             "tech_name": "randovania-plastics",
             "unlocks": [
-                "gun-turret"
+                "low-density-structure"
             ]
         },
         {
             "cost": {
                 "count": 300,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/mining-productivity.png",
+            "description": "Provides the following in order: Engine, Electric engine.",
+            "icon": "__base__/graphics/technology/engine.png",
             "icon_size": 256,
-            "locale_name": "Mining Productivity",
+            "locale_name": "Engine Unit",
             "prerequisites": [
-                "randovania-follower-robot-count-1"
+                "randovania-follower-robot-count-b"
             ],
-            "tech_name": "randovania-follower-robot-count-2",
+            "tech_name": "randovania-follower-robot-count-c",
             "unlocks": [
-                "mining-productivity-4"
+                "engine",
+                "electric-engine"
             ]
         },
         {
             "cost": {
                 "count": 500,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Uranium processing, Kovarex enrichment process.",
-            "icon": "__base__/graphics/technology/uranium-processing.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/sulfur-processing.png",
             "icon_size": 256,
-            "locale_name": "Uranium Processing",
+            "locale_name": "Sulfur",
             "prerequisites": [
-                "randovania-research-speed-3"
+                "randovania-research-speed-d"
             ],
-            "tech_name": "randovania-research-speed-4",
+            "tech_name": "randovania-research-speed-e",
             "unlocks": [
-                "uranium-processing",
-                "kovarex-enrichment-process"
+                "sulfur-processing"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/inserter-capacity.png",
+            "icon": "__base__/graphics/technology/electric-energy-distribution-2.png",
             "icon_size": 256,
-            "locale_name": "Stack Inserter Capacity Bonus",
+            "locale_name": "Substation",
             "prerequisites": [
                 "randovania-military-science-pack",
                 "randovania-flammables"
             ],
             "tech_name": "randovania-flamethrower",
             "unlocks": [
-                "inserter-capacity-bonus-7"
+                "electric-energy-distribution-2"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 15
             },
             "description": "",
-            "icon": "__base__/graphics/technology/electric-energy-distribution-1.png",
+            "icon": "__base__/graphics/technology/night-vision-equipment.png",
             "icon_size": 256,
-            "locale_name": "Medium Electric Pole",
+            "locale_name": "Night Vision Equipment",
             "prerequisites": [
                 "randovania-sulfur-processing"
             ],
             "tech_name": "randovania-explosives",
             "unlocks": [
-                "electric-energy-distribution-1"
+                "night-vision-equipment"
             ]
         },
         {
             "cost": {
                 "count": 150,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Rocketry, Explosive rocketry.",
-            "icon": "__base__/graphics/technology/rocketry.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/exoskeleton-equipment.png",
             "icon_size": 256,
-            "locale_name": "Rocketry",
+            "locale_name": "Exoskeleton Equipment",
             "prerequisites": [
                 "randovania-sulfur-processing"
             ],
             "tech_name": "randovania-battery",
             "unlocks": [
-                "rocketry",
-                "explosive-rocketry"
+                "exoskeleton-equipment"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 15
             },
             "description": "",
-            "icon": "__base__/graphics/technology/steel-axe.png",
+            "icon": "__base__/graphics/technology/worker-robots-speed.png",
             "icon_size": 256,
-            "locale_name": "Steel Axe",
+            "locale_name": "Worker Robots Speed",
             "prerequisites": [
                 "randovania-plastics"
             ],
             "tech_name": "randovania-advanced-electronics",
             "unlocks": [
-                "steel-axe"
+                "worker-robots-speed-6"
             ]
         },
         {
             "cost": {
                 "count": 500,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "production-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/research-speed.png",
+            "description": "Provides the following in order: Uranium processing, Kovarex enrichment process.",
+            "icon": "__base__/graphics/technology/uranium-processing.png",
             "icon_size": 256,
-            "locale_name": "Research Speed",
+            "locale_name": "Uranium Processing",
             "prerequisites": [
-                "randovania-research-speed-4"
+                "randovania-research-speed-e"
             ],
-            "tech_name": "randovania-research-speed-5",
+            "tech_name": "randovania-research-speed-f",
             "unlocks": [
-                "research-speed-6"
+                "uranium-processing",
+                "kovarex-enrichment-process"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Electronics, Advanced electronics, Advanced electronics 2.",
-            "icon": "__base__/graphics/technology/electronics.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/spidertron.png",
             "icon_size": 256,
-            "locale_name": "Electronics",
+            "locale_name": "Spidertron",
             "prerequisites": [
                 "randovania-flamethrower"
             ],
-            "tech_name": "randovania-refined-flammables-1",
+            "tech_name": "randovania-refined-flammables-b",
             "unlocks": [
-                "electronics",
-                "advanced-electronics",
-                "advanced-electronics-2"
+                "spidertron"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 15
             },
-            "description": "Provides the following in order: Productivity module, Productivity module 2, Productivity module 3.",
-            "icon": "__base__/graphics/technology/productivity-module-1.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/electric-energy-distribution-1.png",
             "icon_size": 256,
-            "locale_name": "Productivity Module",
+            "locale_name": "Medium Electric Pole",
             "prerequisites": [
-                "randovania-military-2",
+                "randovania-military-c",
                 "randovania-explosives"
             ],
             "tech_name": "randovania-cliff-explosives",
             "unlocks": [
-                "productivity-module",
-                "productivity-module-2",
-                "productivity-module-3"
+                "electric-energy-distribution-1"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/personal-laser-defense-equipment.png",
+            "icon": "__base__/graphics/technology/inserter-capacity.png",
             "icon_size": 256,
-            "locale_name": "Personal Laser Defense Equipment",
+            "locale_name": "Stack Inserter Capacity Bonus",
             "prerequisites": [
                 "randovania-military-science-pack",
                 "randovania-explosives"
             ],
             "tech_name": "randovania-land-mine",
             "unlocks": [
-                "personal-laser-defense-equipment"
+                "inserter-capacity-bonus-7"
             ]
         },
         {
             "cost": {
                 "count": 120,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 15
             },
-            "description": "Provides the following in order: Light armor, Heavy armor.",
-            "icon": "__base__/graphics/technology/heavy-armor.png",
+            "description": "Provides the following in order: Engine, Electric engine.",
+            "icon": "__base__/graphics/technology/engine.png",
             "icon_size": 256,
-            "locale_name": "Armor",
+            "locale_name": "Engine Unit",
             "prerequisites": [
                 "randovania-military-science-pack",
                 "randovania-flammables",
                 "randovania-explosives"
             ],
             "tech_name": "randovania-rocketry",
             "unlocks": [
-                "light-armor",
-                "heavy-armor"
+                "engine",
+                "electric-engine"
             ]
         },
         {
             "cost": {
                 "count": 150,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Speed module, Speed module 2, Speed module 3.",
-            "icon": "__base__/graphics/technology/speed-module-1.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/worker-robots-storage.png",
             "icon_size": 256,
-            "locale_name": "Speed Module",
+            "locale_name": "Worker Robots Storage",
             "prerequisites": [
-                "randovania-electric-energy-distribution-1",
+                "randovania-electric-energy-distribution-b",
                 "randovania-battery"
             ],
             "tech_name": "randovania-electric-energy-accumulators",
             "unlocks": [
-                "speed-module",
-                "speed-module-2",
-                "speed-module-3"
+                "worker-robots-storage-3"
             ]
         },
         {
             "cost": {
                 "count": 150,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/worker-robots-storage.png",
+            "icon": "__base__/graphics/technology/chemical-science-pack.png",
             "icon_size": 256,
-            "locale_name": "Worker Robots Storage",
+            "locale_name": "Chemical Science Pack",
             "prerequisites": [
-                "randovania-logistics-2",
+                "randovania-logistics-c",
                 "randovania-fast-inserter",
                 "randovania-advanced-electronics"
             ],
             "tech_name": "randovania-stack-inserter",
             "unlocks": [
-                "worker-robots-storage-3"
+                "chemical-science-pack"
             ]
         },
         {
             "cost": {
                 "count": 75,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 10
             },
-            "description": "Provides the following in order: Efficiency module, Efficiency module 2, Efficiency module 3.",
-            "icon": "__base__/graphics/technology/effectivity-module-1.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/mining-productivity.png",
             "icon_size": 256,
-            "locale_name": "Efficiency Module",
+            "locale_name": "Mining Productivity",
             "prerequisites": [
                 "randovania-sulfur-processing",
                 "randovania-advanced-electronics"
             ],
             "tech_name": "randovania-chemical-science-pack",
             "unlocks": [
-                "effectivity-module",
-                "effectivity-module-2",
-                "effectivity-module-3"
+                "mining-productivity-4"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/worker-robots-storage.png",
+            "icon": "__base__/graphics/technology/stone-wall.png",
             "icon_size": 256,
-            "locale_name": "Worker Robots Storage",
+            "locale_name": "Wall",
             "prerequisites": [
                 "randovania-heavy-armor",
                 "randovania-advanced-electronics"
             ],
             "tech_name": "randovania-modular-armor",
             "unlocks": [
-                "worker-robots-storage-3"
+                "stone-wall"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Energy shield, Energy shield MK2.",
-            "icon": "__base__/graphics/technology/energy-shield-equipment.png",
+            "description": "Provides the following in order: Oil processing, Advanced oil processing.",
+            "icon": "__base__/graphics/technology/oil-gathering.png",
             "icon_size": 256,
-            "locale_name": "Energy Shield Equipment",
+            "locale_name": "Oil Processing",
             "prerequisites": [
                 "randovania-advanced-electronics"
             ],
             "tech_name": "randovania-modules",
             "unlocks": [
-                "energy-shield-equipment",
-                "energy-shield-mk2-equipment"
+                "oil-processing",
+                "advanced-oil-processing"
             ]
         },
         {
             "cost": {
                 "count": 250,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 60
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/inserter-capacity.png",
+            "description": "Provides the following in order: Military, Military 2, Military 3, Military 4.",
+            "icon": "__base__/graphics/technology/military.png",
             "icon_size": 256,
-            "locale_name": "Stack Inserter Capacity Bonus",
+            "locale_name": "Military",
             "prerequisites": [
                 "randovania-advanced-electronics"
             ],
-            "tech_name": "randovania-mining-productivity-1",
+            "tech_name": "randovania-mining-productivity-b",
             "unlocks": [
-                "inserter-capacity-bonus-7"
+                "military",
+                "military-2",
+                "military-3",
+                "military-4"
             ]
         },
         {
             "cost": {
                 "count": 500,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "production-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Rocketry, Explosive rocketry.",
-            "icon": "__base__/graphics/technology/rocketry.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/worker-robots-speed.png",
             "icon_size": 256,
-            "locale_name": "Rocketry",
+            "locale_name": "Worker Robots Speed",
             "prerequisites": [
-                "randovania-research-speed-5"
+                "randovania-research-speed-f"
             ],
-            "tech_name": "randovania-research-speed-6",
+            "tech_name": "randovania-research-speed-g",
             "unlocks": [
-                "rocketry",
-                "explosive-rocketry"
+                "worker-robots-speed-6"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Productivity module, Productivity module 2, Productivity module 3.",
-            "icon": "__base__/graphics/technology/productivity-module-1.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/worker-robots-speed.png",
             "icon_size": 256,
-            "locale_name": "Productivity Module",
+            "locale_name": "Worker Robots Speed",
             "prerequisites": [
-                "randovania-refined-flammables-1"
+                "randovania-refined-flammables-b"
             ],
-            "tech_name": "randovania-refined-flammables-2",
+            "tech_name": "randovania-refined-flammables-c",
             "unlocks": [
-                "productivity-module",
-                "productivity-module-2",
-                "productivity-module-3"
+                "worker-robots-speed-6"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
@@ -1632,15 +1622,15 @@
             "description": "",
             "icon": "__base__/graphics/technology/research-speed.png",
             "icon_size": 256,
             "locale_name": "Research Speed",
             "prerequisites": [
                 "randovania-stack-inserter"
             ],
-            "tech_name": "randovania-inserter-capacity-bonus-1",
+            "tech_name": "randovania-inserter-capacity-bonus-b",
             "unlocks": [
                 "research-speed-6"
             ]
         },
         {
             "cost": {
                 "count": 100,
@@ -1649,761 +1639,768 @@
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/production-science-pack.png",
+            "icon": "__base__/graphics/technology/research-speed.png",
             "icon_size": 256,
-            "locale_name": "Production Science Pack",
+            "locale_name": "Research Productivity",
             "prerequisites": [
                 "randovania-military-science-pack",
                 "randovania-chemical-science-pack"
             ],
-            "tech_name": "randovania-military-3",
+            "tech_name": "randovania-military-d",
             "unlocks": [
-                "production-science-pack"
+                "research-productivity"
             ]
         },
         {
             "cost": {
                 "count": 300,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/military-science-pack.png",
+            "icon": "__base__/graphics/technology/atomic-bomb.png",
             "icon_size": 256,
-            "locale_name": "Military Science Pack",
+            "locale_name": "Atomic Bomb",
             "prerequisites": [
                 "randovania-chemical-science-pack"
             ],
-            "tech_name": "randovania-advanced-electronics-2",
+            "tech_name": "randovania-advanced-electronics-c",
             "unlocks": [
-                "military-science-pack"
+                "atomic-bomb"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/sulfur-processing.png",
+            "icon": "__base__/graphics/technology/laser-turret.png",
             "icon_size": 256,
-            "locale_name": "Sulfur",
+            "locale_name": "Laser Turret",
             "prerequisites": [
                 "randovania-railway",
                 "randovania-chemical-science-pack"
             ],
-            "tech_name": "randovania-braking-force-1",
+            "tech_name": "randovania-braking-force-b",
             "unlocks": [
-                "sulfur-processing"
+                "laser-turret"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/fast-inserter.png",
+            "icon": "__base__/graphics/technology/artillery.png",
             "icon_size": 256,
-            "locale_name": "Long Handed inserter",
+            "locale_name": "Artillery",
             "prerequisites": [
                 "randovania-optics",
                 "randovania-battery",
                 "randovania-chemical-science-pack"
             ],
             "tech_name": "randovania-laser",
             "unlocks": [
-                "long-handed-inserter"
+                "artillery"
             ]
         },
         {
             "cost": {
                 "count": 300,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 45
             },
-            "description": "Provides the following in order: Engine, Electric engine.",
-            "icon": "__base__/graphics/technology/engine.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/effect-transmission.png",
             "icon_size": 256,
-            "locale_name": "Engine Unit",
+            "locale_name": "Beacon",
             "prerequisites": [
                 "randovania-advanced-material-processing",
                 "randovania-chemical-science-pack"
             ],
             "tech_name": "randovania-low-density-structure",
             "unlocks": [
-                "engine",
-                "electric-engine"
+                "effect-transmission"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 45
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/oil-processing.png",
+            "description": "Provides the following in order: Productivity module, Productivity module 2, Productivity module 3.",
+            "icon": "__base__/graphics/technology/productivity-module-1.png",
             "icon_size": 256,
-            "locale_name": "Solid Fuel",
+            "locale_name": "Productivity Module",
             "prerequisites": [
-                "randovania-electric-energy-distribution-1",
+                "randovania-electric-energy-distribution-b",
                 "randovania-chemical-science-pack"
             ],
-            "tech_name": "randovania-electric-energy-distribution-2",
+            "tech_name": "randovania-electric-energy-distribution-c",
             "unlocks": [
-                "solid-fuel"
+                "productivity-module",
+                "productivity-module-2",
+                "productivity-module-3"
             ]
         },
         {
             "cost": {
                 "count": 250,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/explosives.png",
+            "icon": "__base__/graphics/technology/logistic-robotics.png",
             "icon_size": 256,
-            "locale_name": "Explosives",
+            "locale_name": "Logistic Robotics",
             "prerequisites": [
                 "randovania-advanced-material-processing",
                 "randovania-chemical-science-pack"
             ],
-            "tech_name": "randovania-advanced-material-processing-2",
+            "tech_name": "randovania-advanced-material-processing-c",
             "unlocks": [
-                "explosives"
+                "logistic-robotics"
             ]
         },
         {
             "cost": {
                 "count": 75,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/mining-productivity.png",
+            "icon": "__base__/graphics/technology/worker-robots-storage.png",
             "icon_size": 256,
-            "locale_name": "Mining Productivity",
+            "locale_name": "Worker Robots Storage",
             "prerequisites": [
                 "randovania-chemical-science-pack"
             ],
             "tech_name": "randovania-advanced-oil-processing",
             "unlocks": [
-                "mining-productivity-4"
+                "worker-robots-storage-3"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Electronics, Advanced electronics, Advanced electronics 2.",
-            "icon": "__base__/graphics/technology/electronics.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/braking-force.png",
             "icon_size": 256,
-            "locale_name": "Electronics",
+            "locale_name": "Braking Force",
             "prerequisites": [
                 "randovania-concrete",
                 "randovania-chemical-science-pack"
             ],
             "tech_name": "randovania-uranium-processing",
             "unlocks": [
-                "electronics",
-                "advanced-electronics",
-                "advanced-electronics-2"
+                "braking-force-7"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 15
             },
             "description": "",
-            "icon": "__base__/graphics/technology/gate.png",
+            "icon": "__base__/graphics/technology/inserter-capacity.png",
             "icon_size": 256,
-            "locale_name": "Gate",
+            "locale_name": "Regular Inserter Capacity Bonus",
             "prerequisites": [
                 "randovania-solar-energy",
                 "randovania-modular-armor"
             ],
             "tech_name": "randovania-solar-panel-equipment",
             "unlocks": [
-                "gate"
+                "regular-inserter-capacity-bonus"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/research-speed.png",
+            "icon": "__base__/graphics/technology/toolbelt.png",
             "icon_size": 256,
-            "locale_name": "Research Productivity",
+            "locale_name": "Toolbelt",
             "prerequisites": [
                 "randovania-modules"
             ],
             "tech_name": "randovania-speed-module",
             "unlocks": [
-                "research-productivity"
+                "toolbelt"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Defender, Distractor, Destroyer.",
-            "icon": "__base__/graphics/technology/defender.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/nuclear-power.png",
             "icon_size": 256,
-            "locale_name": "Follower Capsule",
+            "locale_name": "Nuclear Power",
             "prerequisites": [
                 "randovania-modules"
             ],
             "tech_name": "randovania-productivity-module",
             "unlocks": [
-                "defender",
-                "distractor",
-                "destroyer"
+                "nuclear-power"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/chemical-science-pack.png",
+            "icon": "__base__/graphics/technology/research-speed.png",
             "icon_size": 256,
-            "locale_name": "Chemical Science Pack",
+            "locale_name": "Research Productivity",
             "prerequisites": [
                 "randovania-modules"
             ],
             "tech_name": "randovania-effectivity-module",
             "unlocks": [
-                "chemical-science-pack"
+                "research-productivity"
             ]
         },
         {
             "cost": {
                 "count": 500,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 60
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/mining-productivity.png",
+            "description": "Provides the following in order: Efficiency module, Efficiency module 2, Efficiency module 3.",
+            "icon": "__base__/graphics/technology/effectivity-module-1.png",
             "icon_size": 256,
-            "locale_name": "Mining Productivity",
+            "locale_name": "Efficiency Module",
             "prerequisites": [
-                "randovania-mining-productivity-1"
+                "randovania-mining-productivity-b"
             ],
-            "tech_name": "randovania-mining-productivity-2",
+            "tech_name": "randovania-mining-productivity-c",
             "unlocks": [
-                "mining-productivity-4"
+                "effectivity-module",
+                "effectivity-module-2",
+                "effectivity-module-3"
             ]
         },
         {
             "cost": {
                 "count": 250,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/research-speed.png",
+            "icon": "__base__/graphics/technology/concrete.png",
             "icon_size": 256,
-            "locale_name": "Research Productivity",
+            "locale_name": "Concrete",
             "prerequisites": [
-                "randovania-inserter-capacity-bonus-1"
+                "randovania-inserter-capacity-bonus-b"
             ],
-            "tech_name": "randovania-inserter-capacity-bonus-2",
+            "tech_name": "randovania-inserter-capacity-bonus-c",
             "unlocks": [
-                "research-productivity"
+                "concrete"
             ]
         },
         {
             "cost": {
                 "count": 250,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/spidertron.png",
+            "icon": "__base__/graphics/technology/lubricant.png",
             "icon_size": 256,
-            "locale_name": "Spidertron",
+            "locale_name": "Lubricant",
             "prerequisites": [
                 "randovania-automobilism",
                 "randovania-explosives",
-                "randovania-military-3"
+                "randovania-military-d"
             ],
             "tech_name": "randovania-tank",
             "unlocks": [
-                "spidertron"
+                "lubricant"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Defender, Distractor, Destroyer.",
-            "icon": "__base__/graphics/technology/defender.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/oil-processing.png",
             "icon_size": 256,
-            "locale_name": "Follower Capsule",
+            "locale_name": "Solid Fuel",
             "prerequisites": [
                 "randovania-rocketry",
-                "randovania-military-3"
+                "randovania-military-d"
             ],
             "tech_name": "randovania-explosive-rocketry",
             "unlocks": [
-                "defender",
-                "distractor",
-                "destroyer"
+                "solid-fuel"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/logistic-robotics.png",
+            "icon": "__base__/graphics/technology/robotics.png",
             "icon_size": 256,
-            "locale_name": "Logistic Robotics",
+            "locale_name": "Flying Robot Frame",
             "prerequisites": [
-                "randovania-braking-force-1"
+                "randovania-braking-force-b"
             ],
-            "tech_name": "randovania-braking-force-2",
+            "tech_name": "randovania-braking-force-c",
             "unlocks": [
-                "logistic-robotics"
+                "robotics"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/tank.png",
+            "icon": "__base__/graphics/technology/inserter-capacity.png",
             "icon_size": 256,
-            "locale_name": "Tank",
+            "locale_name": "Regular Inserter Capacity Bonus",
             "prerequisites": [
                 "randovania-military-science-pack",
                 "randovania-laser"
             ],
-            "tech_name": "randovania-energy-weapons-damage-1",
+            "tech_name": "randovania-energy-weapons-damage-b",
             "unlocks": [
-                "tank"
+                "regular-inserter-capacity-bonus"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/lubricant.png",
+            "description": "Provides the following in order: Productivity module, Productivity module 2, Productivity module 3.",
+            "icon": "__base__/graphics/technology/productivity-module-1.png",
             "icon_size": 256,
-            "locale_name": "Lubricant",
+            "locale_name": "Productivity Module",
             "prerequisites": [
                 "randovania-military-science-pack",
                 "randovania-laser"
             ],
-            "tech_name": "randovania-laser-shooting-speed-1",
+            "tech_name": "randovania-laser-shooting-speed-b",
             "unlocks": [
-                "lubricant"
+                "productivity-module",
+                "productivity-module-2",
+                "productivity-module-3"
             ]
         },
         {
             "cost": {
                 "count": 150,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/research-speed.png",
+            "description": "Provides the following in order: Electronics, Advanced electronics, Advanced electronics 2.",
+            "icon": "__base__/graphics/technology/electronics.png",
             "icon_size": 256,
-            "locale_name": "Research Speed",
+            "locale_name": "Electronics",
             "prerequisites": [
                 "randovania-military-science-pack",
                 "randovania-laser"
             ],
             "tech_name": "randovania-laser-turret",
             "unlocks": [
-                "research-speed-6"
+                "electronics",
+                "advanced-electronics",
+                "advanced-electronics-2"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/electric-energy-distribution-1.png",
+            "description": "Provides the following in order: Oil processing, Advanced oil processing.",
+            "icon": "__base__/graphics/technology/oil-gathering.png",
             "icon_size": 256,
-            "locale_name": "Big Electric Pole",
+            "locale_name": "Oil Processing",
             "prerequisites": [
                 "randovania-defender",
-                "randovania-military-3",
+                "randovania-military-d",
                 "randovania-laser"
             ],
             "tech_name": "randovania-distractor",
             "unlocks": [
-                "big-electric-pole"
+                "oil-processing",
+                "advanced-oil-processing"
             ]
         },
         {
             "cost": {
                 "count": 300,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 45
             },
-            "description": "Provides the following in order: Modular armor, Power armor, Power armor MK2.",
-            "icon": "__base__/graphics/technology/armor-making.png",
+            "description": "Provides the following in order: Electronics, Advanced electronics, Advanced electronics 2.",
+            "icon": "__base__/graphics/technology/electronics.png",
             "icon_size": 256,
-            "locale_name": "Modular Armor",
+            "locale_name": "Electronics",
             "prerequisites": [
                 "randovania-flammables",
                 "randovania-advanced-oil-processing"
             ],
             "tech_name": "randovania-rocket-fuel",
             "unlocks": [
-                "modular-armor",
-                "power-armor",
-                "power-armor-mk2"
+                "electronics",
+                "advanced-electronics",
+                "advanced-electronics-2"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/stone-wall.png",
+            "description": "Provides the following in order: Speed module, Speed module 2, Speed module 3.",
+            "icon": "__base__/graphics/technology/speed-module-1.png",
             "icon_size": 256,
-            "locale_name": "Wall",
+            "locale_name": "Speed Module",
             "prerequisites": [
                 "randovania-advanced-oil-processing"
             ],
             "tech_name": "randovania-lubricant",
             "unlocks": [
-                "stone-wall"
+                "speed-module",
+                "speed-module-2",
+                "speed-module-3"
             ]
         },
         {
             "cost": {
                 "count": 800,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/worker-robots-storage.png",
+            "icon": "__base__/graphics/technology/inserter-capacity.png",
             "icon_size": 256,
-            "locale_name": "Worker Robots Storage",
+            "locale_name": "Stack Inserter Capacity Bonus",
             "prerequisites": [
                 "randovania-uranium-processing"
             ],
             "tech_name": "randovania-nuclear-power",
             "unlocks": [
-                "worker-robots-storage-3"
+                "inserter-capacity-bonus-7"
             ]
         },
         {
             "cost": {
                 "count": 150,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 15
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/worker-robots-speed.png",
+            "description": "Provides the following in order: Speed module, Speed module 2, Speed module 3.",
+            "icon": "__base__/graphics/technology/speed-module-1.png",
             "icon_size": 256,
-            "locale_name": "Worker Robots Speed",
+            "locale_name": "Speed Module",
             "prerequisites": [
                 "randovania-military-science-pack",
                 "randovania-solar-panel-equipment"
             ],
             "tech_name": "randovania-energy-shield-equipment",
             "unlocks": [
-                "worker-robots-speed-6"
+                "speed-module",
+                "speed-module-2",
+                "speed-module-3"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 15
             },
             "description": "",
-            "icon": "__base__/graphics/technology/mining-productivity.png",
+            "icon": "__base__/graphics/technology/oil-processing.png",
             "icon_size": 256,
-            "locale_name": "Mining Productivity",
+            "locale_name": "Oil Cracking",
             "prerequisites": [
                 "randovania-solar-panel-equipment"
             ],
             "tech_name": "randovania-night-vision-equipment",
             "unlocks": [
-                "mining-productivity-4"
+                "oil-cracking"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 15
             },
             "description": "",
-            "icon": "__base__/graphics/technology/artillery.png",
+            "icon": "__base__/graphics/technology/gate.png",
             "icon_size": 256,
-            "locale_name": "Artillery",
+            "locale_name": "Gate",
             "prerequisites": [
                 "randovania-solar-panel-equipment"
             ],
             "tech_name": "randovania-belt-immunity-equipment",
             "unlocks": [
-                "artillery"
+                "gate"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 15
             },
-            "description": "Provides the following in order: Speed module, Speed module 2, Speed module 3.",
-            "icon": "__base__/graphics/technology/speed-module-1.png",
+            "description": "Provides the following in order: Rocketry, Explosive rocketry.",
+            "icon": "__base__/graphics/technology/rocketry.png",
             "icon_size": 256,
-            "locale_name": "Speed Module",
+            "locale_name": "Rocketry",
             "prerequisites": [
                 "randovania-battery",
                 "randovania-solar-panel-equipment"
             ],
             "tech_name": "randovania-battery-equipment",
             "unlocks": [
-                "speed-module",
-                "speed-module-2",
-                "speed-module-3"
+                "rocketry",
+                "explosive-rocketry"
             ]
         },
         {
             "cost": {
                 "count": 75,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/plastics.png",
+            "icon": "__base__/graphics/technology/fluid-handling.png",
             "icon_size": 256,
-            "locale_name": "Plastics",
+            "locale_name": "Fluid Handling",
             "prerequisites": [
-                "randovania-advanced-electronics-2",
+                "randovania-advanced-electronics-c",
                 "randovania-speed-module"
             ],
-            "tech_name": "randovania-speed-module-2",
+            "tech_name": "randovania-speed-module-c",
             "unlocks": [
-                "plastics"
+                "fluid-handling"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/advanced-material-processing-2.png",
+            "icon": "__base__/graphics/technology/belt-immunity-equipment.png",
             "icon_size": 256,
-            "locale_name": "Electric Furnace",
+            "locale_name": "Belt Immunity Equipment",
             "prerequisites": [
                 "randovania-railway",
-                "randovania-advanced-material-processing-2",
+                "randovania-advanced-material-processing-c",
                 "randovania-productivity-module"
             ],
             "tech_name": "randovania-production-science-pack",
             "unlocks": [
-                "advanced-material-processing-2"
+                "belt-immunity-equipment"
             ]
         },
         {
             "cost": {
                 "count": 75,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/robotics.png",
+            "description": "Provides the following in order: Logistics, Logistics 2, Logistics 3.",
+            "icon": "__base__/graphics/technology/logistics-1.png",
             "icon_size": 256,
-            "locale_name": "Flying Robot Frame",
+            "locale_name": "Logistics",
             "prerequisites": [
-                "randovania-advanced-electronics-2",
+                "randovania-advanced-electronics-c",
                 "randovania-productivity-module"
             ],
-            "tech_name": "randovania-productivity-module-2",
+            "tech_name": "randovania-productivity-module-c",
             "unlocks": [
-                "robotics"
+                "logistics",
+                "logistics-2",
+                "logistics-3"
             ]
         },
         {
             "cost": {
                 "count": 75,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/logistic-system.png",
+            "icon": "__base__/graphics/technology/research-speed.png",
             "icon_size": 256,
-            "locale_name": "Logistic System",
+            "locale_name": "Research Productivity",
             "prerequisites": [
-                "randovania-advanced-electronics-2",
+                "randovania-advanced-electronics-c",
                 "randovania-effectivity-module"
             ],
-            "tech_name": "randovania-effectivity-module-2",
+            "tech_name": "randovania-effectivity-module-c",
             "unlocks": [
-                "logistic-system"
+                "research-productivity"
             ]
         },
         {
             "cost": {
                 "count": 1000,
                 "ingredients": [
                     "automation-science-pack",
@@ -2411,658 +2408,655 @@
                     "logistic-science-pack",
                     "production-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 60
             },
             "description": "",
-            "icon": "__base__/graphics/technology/worker-robots-speed.png",
+            "icon": "__base__/graphics/technology/solar-energy.png",
             "icon_size": 256,
-            "locale_name": "Worker Robots Speed",
+            "locale_name": "Solar Panel",
             "prerequisites": [
-                "randovania-mining-productivity-2"
+                "randovania-mining-productivity-c"
             ],
-            "tech_name": "randovania-mining-productivity-3",
+            "tech_name": "randovania-mining-productivity-d",
             "unlocks": [
-                "worker-robots-speed-6"
+                "solar-energy"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Light armor, Heavy armor.",
-            "icon": "__base__/graphics/technology/heavy-armor.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/coal-liquefaction.png",
             "icon_size": 256,
-            "locale_name": "Armor",
+            "locale_name": "Coal Liquefaction",
             "prerequisites": [
-                "randovania-energy-weapons-damage-1"
+                "randovania-energy-weapons-damage-b"
             ],
-            "tech_name": "randovania-energy-weapons-damage-2",
+            "tech_name": "randovania-energy-weapons-damage-c",
             "unlocks": [
-                "light-armor",
-                "heavy-armor"
+                "coal-liquefaction"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/cliff-explosives.png",
+            "icon": "__base__/graphics/technology/toolbelt.png",
             "icon_size": 256,
-            "locale_name": "Cliff Explosives",
+            "locale_name": "Toolbelt",
             "prerequisites": [
-                "randovania-laser-shooting-speed-1"
+                "randovania-laser-shooting-speed-b"
             ],
-            "tech_name": "randovania-laser-shooting-speed-2",
+            "tech_name": "randovania-laser-shooting-speed-c",
             "unlocks": [
-                "cliff-explosives"
+                "toolbelt"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Oil processing, Advanced oil processing.",
-            "icon": "__base__/graphics/technology/oil-gathering.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/landfill.png",
             "icon_size": 256,
-            "locale_name": "Oil Processing",
+            "locale_name": "Landfill",
             "prerequisites": [
                 "randovania-lubricant"
             ],
             "tech_name": "randovania-electric-engine",
             "unlocks": [
-                "oil-processing",
-                "advanced-oil-processing"
+                "landfill"
             ]
         },
         {
             "cost": {
                 "count": 150,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "production-science-pack"
                 ],
                 "time": 60
             },
             "description": "",
-            "icon": "__base__/graphics/technology/research-speed.png",
+            "icon": "__base__/graphics/technology/inserter-capacity.png",
             "icon_size": 256,
-            "locale_name": "Research Speed",
+            "locale_name": "Regular Inserter Capacity Bonus",
             "prerequisites": [
                 "randovania-speed-module",
                 "randovania-production-science-pack"
             ],
-            "tech_name": "randovania-automation-3",
+            "tech_name": "randovania-automation-d",
             "unlocks": [
-                "research-speed-6"
+                "regular-inserter-capacity-bonus"
             ]
         },
         {
             "cost": {
                 "count": 300,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "production-science-pack"
                 ],
                 "time": 15
             },
             "description": "",
-            "icon": "__base__/graphics/technology/electric-energy-acumulators.png",
+            "icon": "__base__/graphics/technology/rocket-control-unit.png",
             "icon_size": 256,
-            "locale_name": "Accumulator",
+            "locale_name": "Rocket Control Unit",
             "prerequisites": [
                 "randovania-lubricant",
                 "randovania-production-science-pack"
             ],
-            "tech_name": "randovania-logistics-3",
+            "tech_name": "randovania-logistics-d",
             "unlocks": [
-                "electric-energy-accumulators"
+                "rocket-control-unit"
             ]
         },
         {
             "cost": {
                 "count": 75,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "production-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Automation, Automation 2, Automation 3.",
-            "icon": "__base__/graphics/technology/automation-1.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/fast-inserter.png",
             "icon_size": 256,
-            "locale_name": "Assembly Machine",
+            "locale_name": "Long Handed inserter",
             "prerequisites": [
-                "randovania-advanced-electronics-2",
+                "randovania-advanced-electronics-c",
                 "randovania-production-science-pack"
             ],
             "tech_name": "randovania-effect-transmission",
             "unlocks": [
-                "automation",
-                "automation-2",
-                "automation-3"
+                "long-handed-inserter"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "production-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/solar-panel-equipment.png",
+            "icon": "__base__/graphics/technology/worker-robots-speed.png",
             "icon_size": 256,
-            "locale_name": "Solar Panel Equipment",
+            "locale_name": "Worker Robots Speed",
             "prerequisites": [
                 "randovania-advanced-oil-processing",
                 "randovania-production-science-pack"
             ],
             "tech_name": "randovania-coal-liquefaction",
             "unlocks": [
-                "solar-panel-equipment"
+                "worker-robots-speed-6"
             ]
         },
         {
             "cost": {
                 "count": 300,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "production-science-pack"
                 ],
                 "time": 60
             },
             "description": "",
-            "icon": "__base__/graphics/technology/inserter-capacity.png",
+            "icon": "__base__/graphics/technology/tank.png",
             "icon_size": 256,
-            "locale_name": "Regular Inserter Capacity Bonus",
+            "locale_name": "Tank",
             "prerequisites": [
-                "randovania-speed-module-2",
+                "randovania-speed-module-c",
                 "randovania-production-science-pack"
             ],
-            "tech_name": "randovania-speed-module-3",
+            "tech_name": "randovania-speed-module-d",
             "unlocks": [
-                "regular-inserter-capacity-bonus"
+                "tank"
             ]
         },
         {
             "cost": {
                 "count": 1500,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "production-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/utility-science-pack.png",
+            "icon": "__base__/graphics/technology/inserter-capacity.png",
             "icon_size": 256,
-            "locale_name": "Utility Science Pack",
+            "locale_name": "Stack Inserter Capacity Bonus",
             "prerequisites": [
                 "randovania-uranium-processing",
                 "randovania-rocket-fuel",
                 "randovania-production-science-pack"
             ],
             "tech_name": "randovania-kovarex-enrichment-process",
             "unlocks": [
-                "utility-science-pack"
+                "inserter-capacity-bonus-7"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "production-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/inserter-capacity.png",
+            "icon": "__base__/graphics/technology/cliff-explosives.png",
             "icon_size": 256,
-            "locale_name": "Stack Inserter Capacity Bonus",
+            "locale_name": "Cliff Explosives",
             "prerequisites": [
                 "randovania-nuclear-power",
                 "randovania-production-science-pack"
             ],
             "tech_name": "randovania-nuclear-fuel-reprocessing",
             "unlocks": [
-                "inserter-capacity-bonus-7"
+                "cliff-explosives"
             ]
         },
         {
             "cost": {
                 "count": 300,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "production-science-pack"
                 ],
                 "time": 60
             },
             "description": "",
-            "icon": "__base__/graphics/technology/worker-robots-storage.png",
+            "icon": "__base__/graphics/technology/fusion-reactor-equipment.png",
             "icon_size": 256,
-            "locale_name": "Worker Robots Storage",
+            "locale_name": "Fusion Reactor Equipment",
             "prerequisites": [
                 "randovania-production-science-pack",
-                "randovania-productivity-module-2"
+                "randovania-productivity-module-c"
             ],
-            "tech_name": "randovania-productivity-module-3",
+            "tech_name": "randovania-productivity-module-d",
             "unlocks": [
-                "worker-robots-storage-3"
+                "fusion-reactor-equipment"
             ]
         },
         {
             "cost": {
                 "count": 300,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "production-science-pack"
                 ],
                 "time": 60
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/toolbelt.png",
+            "description": "Provides the following in order: Personal battery, Personal battery MK2.",
+            "icon": "__base__/graphics/technology/battery-equipment.png",
             "icon_size": 256,
-            "locale_name": "Toolbelt",
+            "locale_name": "Battery Equipment",
             "prerequisites": [
                 "randovania-production-science-pack",
-                "randovania-effectivity-module-2"
+                "randovania-effectivity-module-c"
             ],
-            "tech_name": "randovania-effectivity-module-3",
+            "tech_name": "randovania-effectivity-module-d",
             "unlocks": [
-                "toolbelt"
+                "battery-equipment",
+                "battery-mk2-equipment"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Engine, Electric engine.",
-            "icon": "__base__/graphics/technology/engine.png",
+            "description": "Provides the following in order: Inserter, Fast inserter, Stack inserter.",
+            "icon": "__base__/graphics/technology/fast-inserter.png",
             "icon_size": 256,
-            "locale_name": "Engine Unit",
+            "locale_name": "Inserter",
             "prerequisites": [
                 "randovania-modular-armor",
-                "randovania-advanced-electronics-2",
+                "randovania-advanced-electronics-c",
                 "randovania-electric-engine"
             ],
             "tech_name": "randovania-power-armor",
             "unlocks": [
-                "engine",
-                "electric-engine"
+                "inserter",
+                "fast-inserter",
+                "stack-inserter"
             ]
         },
         {
             "cost": {
                 "count": 75,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Inserter, Fast inserter, Stack inserter.",
-            "icon": "__base__/graphics/technology/fast-inserter.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/research-speed.png",
             "icon_size": 256,
-            "locale_name": "Inserter",
+            "locale_name": "Research Speed",
             "prerequisites": [
                 "randovania-battery",
                 "randovania-electric-engine"
             ],
             "tech_name": "randovania-robotics",
             "unlocks": [
-                "inserter",
-                "fast-inserter",
-                "stack-inserter"
+                "research-speed-6"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/low-density-structure.png",
+            "icon": "__base__/graphics/technology/advanced-material-processing-2.png",
             "icon_size": 256,
-            "locale_name": "Low Density Structure",
+            "locale_name": "Electric Furnace",
             "prerequisites": [
-                "randovania-advanced-electronics-2",
+                "randovania-advanced-electronics-c",
                 "randovania-solar-panel-equipment",
                 "randovania-electric-engine"
             ],
             "tech_name": "randovania-exoskeleton-equipment",
             "unlocks": [
-                "low-density-structure"
+                "advanced-material-processing-2"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/land-mine.png",
+            "description": "Provides the following in order: Modular armor, Power armor, Power armor MK2.",
+            "icon": "__base__/graphics/technology/armor-making.png",
             "icon_size": 256,
-            "locale_name": "Land Mine",
+            "locale_name": "Modular Armor",
             "prerequisites": [
-                "randovania-military-3",
+                "randovania-military-d",
                 "randovania-low-density-structure",
                 "randovania-energy-shield-equipment",
                 "randovania-power-armor"
             ],
             "tech_name": "randovania-energy-shield-mk2-equipment",
             "unlocks": [
-                "land-mine"
+                "modular-armor",
+                "power-armor",
+                "power-armor-mk2"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Modular armor, Power armor, Power armor MK2.",
-            "icon": "__base__/graphics/technology/armor-making.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/production-science-pack.png",
             "icon_size": 256,
-            "locale_name": "Modular Armor",
+            "locale_name": "Production Science Pack",
             "prerequisites": [
                 "randovania-low-density-structure",
                 "randovania-battery-equipment",
                 "randovania-power-armor"
             ],
             "tech_name": "randovania-battery-mk2-equipment",
             "unlocks": [
-                "modular-armor",
-                "power-armor",
-                "power-armor-mk2"
+                "production-science-pack"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Efficiency module, Efficiency module 2, Efficiency module 3.",
-            "icon": "__base__/graphics/technology/effectivity-module-1.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/worker-robots-storage.png",
             "icon_size": 256,
-            "locale_name": "Efficiency Module",
+            "locale_name": "Worker Robots Storage",
             "prerequisites": [
-                "randovania-military-3",
+                "randovania-military-d",
                 "randovania-low-density-structure",
                 "randovania-solar-panel-equipment",
                 "randovania-laser-turret",
                 "randovania-power-armor"
             ],
             "tech_name": "randovania-personal-laser-defense-equipment",
             "unlocks": [
-                "effectivity-module",
-                "effectivity-module-2",
-                "effectivity-module-3"
+                "worker-robots-storage-3"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/fluid-wagon.png",
+            "icon": "__base__/graphics/technology/rocket-fuel.png",
             "icon_size": 256,
-            "locale_name": "Fluid Wagon",
+            "locale_name": "Rocket Fuel",
             "prerequisites": [
-                "randovania-military-3",
+                "randovania-military-d",
                 "randovania-solar-panel-equipment",
                 "randovania-laser-turret",
                 "randovania-power-armor"
             ],
             "tech_name": "randovania-discharge-defense-equipment",
             "unlocks": [
-                "fluid-wagon"
+                "rocket-fuel"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/night-vision-equipment.png",
+            "description": "Provides the following in order: Uranium processing, Kovarex enrichment process.",
+            "icon": "__base__/graphics/technology/uranium-processing.png",
             "icon_size": 256,
-            "locale_name": "Night Vision Equipment",
+            "locale_name": "Uranium Processing",
             "prerequisites": [
-                "randovania-advanced-electronics-2",
+                "randovania-advanced-electronics-c",
                 "randovania-low-density-structure",
                 "randovania-robotics"
             ],
             "tech_name": "randovania-utility-science-pack",
             "unlocks": [
-                "night-vision-equipment"
+                "uranium-processing",
+                "kovarex-enrichment-process"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/worker-robots-speed.png",
+            "description": "Provides the following in order: Modular armor, Power armor, Power armor MK2.",
+            "icon": "__base__/graphics/technology/armor-making.png",
             "icon_size": 256,
-            "locale_name": "Worker Robots Speed",
+            "locale_name": "Modular Armor",
             "prerequisites": [
                 "randovania-robotics"
             ],
             "tech_name": "randovania-construction-robotics",
             "unlocks": [
-                "worker-robots-speed-6"
+                "modular-armor",
+                "power-armor",
+                "power-armor-mk2"
             ]
         },
         {
             "cost": {
                 "count": 250,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Logistics, Logistics 2, Logistics 3.",
-            "icon": "__base__/graphics/technology/logistics-1.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/research-speed.png",
             "icon_size": 256,
-            "locale_name": "Logistics",
+            "locale_name": "Research Speed",
             "prerequisites": [
                 "randovania-robotics"
             ],
             "tech_name": "randovania-logistic-robotics",
             "unlocks": [
-                "logistics",
-                "logistics-2",
-                "logistics-3"
+                "research-speed-6"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Uranium processing, Kovarex enrichment process.",
-            "icon": "__base__/graphics/technology/uranium-processing.png",
+            "description": "Provides the following in order: Speed module, Speed module 2, Speed module 3.",
+            "icon": "__base__/graphics/technology/speed-module-1.png",
             "icon_size": 256,
-            "locale_name": "Uranium Processing",
+            "locale_name": "Speed Module",
             "prerequisites": [
                 "randovania-robotics"
             ],
-            "tech_name": "randovania-worker-robots-speed-1",
+            "tech_name": "randovania-worker-robots-speed-b",
             "unlocks": [
-                "uranium-processing",
-                "kovarex-enrichment-process"
+                "speed-module",
+                "speed-module-2",
+                "speed-module-3"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/research-speed.png",
+            "icon": "__base__/graphics/technology/steel-axe.png",
             "icon_size": 256,
-            "locale_name": "Research Productivity",
+            "locale_name": "Steel Axe",
             "prerequisites": [
                 "randovania-robotics"
             ],
-            "tech_name": "randovania-worker-robots-storage-1",
+            "tech_name": "randovania-worker-robots-storage-b",
             "unlocks": [
-                "research-productivity"
+                "steel-axe"
             ]
         },
         {
             "cost": {
                 "count": 150,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 45
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/nuclear-power.png",
+            "description": "Provides the following in order: Light armor, Heavy armor.",
+            "icon": "__base__/graphics/technology/heavy-armor.png",
             "icon_size": 256,
-            "locale_name": "Nuclear Power",
+            "locale_name": "Armor",
             "prerequisites": [
                 "randovania-explosives",
-                "randovania-military-3",
+                "randovania-military-d",
                 "randovania-utility-science-pack"
             ],
-            "tech_name": "randovania-military-4",
+            "tech_name": "randovania-military-e",
             "unlocks": [
-                "nuclear-power"
+                "light-armor",
+                "heavy-armor"
             ]
         },
         {
             "cost": {
                 "count": 300,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 45
             },
             "description": "",
-            "icon": "__base__/graphics/technology/inserter-capacity.png",
+            "icon": "__base__/graphics/technology/personal-laser-defense-equipment.png",
             "icon_size": 256,
-            "locale_name": "Stack Inserter Capacity Bonus",
+            "locale_name": "Personal Laser Defense Equipment",
             "prerequisites": [
                 "randovania-speed-module",
                 "randovania-utility-science-pack"
             ],
             "tech_name": "randovania-rocket-control-unit",
             "unlocks": [
-                "inserter-capacity-bonus-7"
+                "personal-laser-defense-equipment"
             ]
         },
         {
             "cost": {
                 "count": 200,
                 "ingredients": [
                     "automation-science-pack",
@@ -3070,172 +3064,175 @@
                     "logistic-science-pack",
                     "military-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/fast-inserter.png",
+            "icon": "__base__/graphics/technology/explosives.png",
             "icon_size": 256,
-            "locale_name": "Longer Handed inserter",
+            "locale_name": "Explosives",
             "prerequisites": [
                 "randovania-military-science-pack",
                 "randovania-power-armor",
                 "randovania-utility-science-pack"
             ],
             "tech_name": "randovania-fusion-reactor-equipment",
             "unlocks": [
-                "longer-handed-inserter"
+                "explosives"
             ]
         },
         {
             "cost": {
                 "count": 50,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/atomic-bomb.png",
+            "icon": "__base__/graphics/technology/research-speed.png",
             "icon_size": 256,
-            "locale_name": "Atomic Bomb",
+            "locale_name": "Research Productivity",
             "prerequisites": [
                 "randovania-solar-panel-equipment",
                 "randovania-construction-robotics"
             ],
             "tech_name": "randovania-personal-roboport-equipment",
             "unlocks": [
-                "atomic-bomb"
+                "research-productivity"
             ]
         },
         {
             "cost": {
                 "count": 500,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/inserter-capacity.png",
+            "icon": "__base__/graphics/technology/flamethrower.png",
             "icon_size": 256,
-            "locale_name": "Regular Inserter Capacity Bonus",
+            "locale_name": "Flamethrower",
             "prerequisites": [
                 "randovania-utility-science-pack",
                 "randovania-logistic-robotics"
             ],
             "tech_name": "randovania-logistic-system",
             "unlocks": [
-                "regular-inserter-capacity-bonus"
+                "flamethrower"
             ]
         },
         {
             "cost": {
                 "count": 100,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack"
                 ],
                 "time": 30
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/uranium-ammo.png",
+            "description": "Provides the following in order: Modular armor, Power armor, Power armor MK2.",
+            "icon": "__base__/graphics/technology/armor-making.png",
             "icon_size": 256,
-            "locale_name": "Uranium Ammo",
+            "locale_name": "Modular Armor",
             "prerequisites": [
-                "randovania-worker-robots-speed-1"
+                "randovania-worker-robots-speed-b"
             ],
-            "tech_name": "randovania-worker-robots-speed-2",
+            "tech_name": "randovania-worker-robots-speed-c",
             "unlocks": [
-                "uranium-ammo"
+                "modular-armor",
+                "power-armor",
+                "power-armor-mk2"
             ]
         },
         {
             "cost": {
                 "count": 300,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "production-science-pack"
                 ],
                 "time": 60
             },
             "description": "",
-            "icon": "__base__/graphics/technology/belt-immunity-equipment.png",
+            "icon": "__base__/graphics/technology/utility-science-pack.png",
             "icon_size": 256,
-            "locale_name": "Belt Immunity Equipment",
+            "locale_name": "Utility Science Pack",
             "prerequisites": [
-                "randovania-worker-robots-storage-1"
+                "randovania-worker-robots-storage-b"
             ],
-            "tech_name": "randovania-worker-robots-storage-2",
+            "tech_name": "randovania-worker-robots-storage-c",
             "unlocks": [
-                "belt-immunity-equipment"
+                "utility-science-pack"
             ]
         },
         {
             "cost": {
                 "count": 1000,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 45
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/automobilism.png",
+            "description": "Provides the following in order: Personal roboport, Personal roboport MK2.",
+            "icon": "__base__/graphics/technology/personal-roboport-equipment.png",
             "icon_size": 256,
-            "locale_name": "Car",
+            "locale_name": "Personal Roboport Equipment",
             "prerequisites": [
                 "randovania-uranium-processing",
                 "randovania-tank",
-                "randovania-military-4"
+                "randovania-military-e"
             ],
             "tech_name": "randovania-uranium-ammo",
             "unlocks": [
-                "automobilism"
+                "personal-roboport-equipment",
+                "personal-roboport-mk2-equipment"
             ]
         },
         {
             "cost": {
                 "count": 400,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Modular armor, Power armor, Power armor MK2.",
-            "icon": "__base__/graphics/technology/armor-making.png",
+            "description": "Provides the following in order: Automation, Automation 2, Automation 3.",
+            "icon": "__base__/graphics/technology/automation-1.png",
             "icon_size": 256,
-            "locale_name": "Modular Armor",
+            "locale_name": "Assembly Machine",
             "prerequisites": [
-                "randovania-speed-module-2",
-                "randovania-effectivity-module-2",
+                "randovania-speed-module-c",
+                "randovania-effectivity-module-c",
                 "randovania-power-armor",
-                "randovania-military-4"
+                "randovania-military-e"
             ],
             "tech_name": "randovania-power-armor-mk2",
             "unlocks": [
-                "modular-armor",
-                "power-armor",
-                "power-armor-mk2"
+                "automation",
+                "automation-2",
+                "automation-3"
             ]
         },
         {
             "cost": {
                 "count": 300,
                 "ingredients": [
                     "automation-science-pack",
@@ -3243,51 +3240,50 @@
                     "logistic-science-pack",
                     "military-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/oil-processing.png",
+            "icon": "__base__/graphics/technology/toolbelt.png",
             "icon_size": 256,
-            "locale_name": "Oil Cracking",
+            "locale_name": "Toolbelt",
             "prerequisites": [
                 "randovania-speed-module",
                 "randovania-distractor",
-                "randovania-military-4"
+                "randovania-military-e"
             ],
             "tech_name": "randovania-destroyer",
             "unlocks": [
-                "oil-cracking"
+                "toolbelt"
             ]
         },
         {
             "cost": {
                 "count": 2000,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "military-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Energy shield, Energy shield MK2.",
-            "icon": "__base__/graphics/technology/energy-shield-equipment.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/mining-productivity.png",
             "icon_size": 256,
-            "locale_name": "Energy Shield Equipment",
+            "locale_name": "Mining Productivity",
             "prerequisites": [
                 "randovania-tank",
-                "randovania-military-4"
+                "randovania-military-e"
             ],
             "tech_name": "randovania-artillery",
             "unlocks": [
-                "energy-shield-equipment",
-                "energy-shield-mk2-equipment"
+                "mining-productivity-4"
             ]
         },
         {
             "cost": {
                 "count": 5000,
                 "ingredients": [
                     "automation-science-pack",
@@ -3296,26 +3292,26 @@
                     "military-science-pack",
                     "production-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 45
             },
             "description": "",
-            "icon": "__base__/graphics/technology/lamp.png",
+            "icon": "__base__/graphics/technology/research-speed.png",
             "icon_size": 256,
-            "locale_name": "Optics",
+            "locale_name": "Research Speed",
             "prerequisites": [
                 "randovania-rocketry",
                 "randovania-kovarex-enrichment-process",
-                "randovania-military-4",
+                "randovania-military-e",
                 "randovania-rocket-control-unit"
             ],
             "tech_name": "randovania-atomic-bomb",
             "unlocks": [
-                "optics"
+                "research-speed-6"
             ]
         },
         {
             "cost": {
                 "count": 1000,
                 "ingredients": [
                     "automation-science-pack",
@@ -3329,16 +3325,16 @@
             "description": "",
             "icon": "__base__/graphics/technology/rocket-silo.png",
             "icon_size": 256,
             "locale_name": "Rocket Silo",
             "prerequisites": [
                 "randovania-concrete",
                 "randovania-rocket-fuel",
-                "randovania-speed-module-3",
-                "randovania-productivity-module-3",
+                "randovania-speed-module-d",
+                "randovania-productivity-module-d",
                 "randovania-rocket-control-unit"
             ],
             "tech_name": "randovania-rocket-silo",
             "unlocks": [
                 "rocket-silo"
             ]
         },
@@ -3351,107 +3347,101 @@
                     "logistic-science-pack",
                     "military-science-pack",
                     "production-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Military, Military 2, Military 3, Military 4.",
-            "icon": "__base__/graphics/technology/military.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/worker-robots-speed.png",
             "icon_size": 256,
-            "locale_name": "Military",
+            "locale_name": "Worker Robots Speed",
             "prerequisites": [
                 "randovania-rocketry",
-                "randovania-effectivity-module-3",
+                "randovania-effectivity-module-d",
                 "randovania-exoskeleton-equipment",
-                "randovania-military-4",
+                "randovania-military-e",
                 "randovania-rocket-control-unit",
                 "randovania-fusion-reactor-equipment"
             ],
             "tech_name": "randovania-spidertron",
             "unlocks": [
-                "military",
-                "military-2",
-                "military-3",
-                "military-4"
+                "worker-robots-speed-6"
             ]
         },
         {
             "cost": {
                 "count": 250,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 30
             },
-            "description": "Provides the following in order: Personal roboport, Personal roboport MK2.",
-            "icon": "__base__/graphics/technology/personal-roboport-equipment.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/mining-productivity.png",
             "icon_size": 256,
-            "locale_name": "Personal Roboport Equipment",
+            "locale_name": "Mining Productivity",
             "prerequisites": [
                 "randovania-utility-science-pack",
                 "randovania-personal-roboport-equipment"
             ],
             "tech_name": "randovania-personal-roboport-mk2-equipment",
             "unlocks": [
-                "personal-roboport-equipment",
-                "personal-roboport-mk2-equipment"
+                "mining-productivity-4"
             ]
         },
         {
             "cost": {
                 "count": 150,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 60
             },
-            "description": "Provides the following in order: Military, Military 2, Military 3, Military 4.",
-            "icon": "__base__/graphics/technology/military.png",
+            "description": "",
+            "icon": "__base__/graphics/technology/inserter-capacity.png",
             "icon_size": 256,
-            "locale_name": "Military",
+            "locale_name": "Stack Inserter Capacity Bonus",
             "prerequisites": [
-                "randovania-worker-robots-speed-2"
+                "randovania-worker-robots-speed-c"
             ],
-            "tech_name": "randovania-worker-robots-speed-3",
+            "tech_name": "randovania-worker-robots-speed-d",
             "unlocks": [
-                "military",
-                "military-2",
-                "military-3",
-                "military-4"
+                "inserter-capacity-bonus-7"
             ]
         },
         {
             "cost": {
                 "count": 450,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "production-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 60
             },
-            "description": "",
-            "icon": "__base__/graphics/technology/electric-energy-distribution-2.png",
+            "description": "Provides the following in order: Personal roboport, Personal roboport MK2.",
+            "icon": "__base__/graphics/technology/personal-roboport-equipment.png",
             "icon_size": 256,
-            "locale_name": "Substation",
+            "locale_name": "Personal Roboport Equipment",
             "prerequisites": [
-                "randovania-worker-robots-storage-2"
+                "randovania-worker-robots-storage-c"
             ],
-            "tech_name": "randovania-worker-robots-storage-3",
+            "tech_name": "randovania-worker-robots-storage-d",
             "unlocks": [
-                "electric-energy-distribution-2"
+                "personal-roboport-equipment",
+                "personal-roboport-mk2-equipment"
             ]
         },
         {
             "cost": {
                 "count": 2000,
                 "ingredients": [
                     "automation-science-pack",
@@ -3459,48 +3449,48 @@
                     "logistic-science-pack",
                     "production-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 30
             },
             "description": "",
-            "icon": "__base__/graphics/technology/toolbelt.png",
+            "icon": "__base__/graphics/technology/battery.png",
             "icon_size": 256,
-            "locale_name": "Toolbelt",
+            "locale_name": "Battery",
             "prerequisites": [
                 "randovania-solar-energy",
                 "randovania-electric-energy-accumulators",
                 "randovania-rocket-silo"
             ],
             "tech_name": "randovania-space-science-pack",
             "unlocks": [
-                "toolbelt"
+                "battery"
             ]
         },
         {
             "cost": {
                 "count": 250,
                 "ingredients": [
                     "automation-science-pack",
                     "chemical-science-pack",
                     "logistic-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 60
             },
             "description": "",
-            "icon": "__base__/graphics/technology/effect-transmission.png",
+            "icon": "__base__/graphics/technology/solar-panel-equipment.png",
             "icon_size": 256,
-            "locale_name": "Beacon",
+            "locale_name": "Solar Panel Equipment",
             "prerequisites": [
-                "randovania-worker-robots-speed-3"
+                "randovania-worker-robots-speed-d"
             ],
-            "tech_name": "randovania-worker-robots-speed-4",
+            "tech_name": "randovania-worker-robots-speed-e",
             "unlocks": [
-                "effect-transmission"
+                "solar-panel-equipment"
             ]
         },
         {
             "cost": {
                 "count": 500,
                 "ingredients": [
                     "automation-science-pack",
@@ -3508,20 +3498,20 @@
                     "logistic-science-pack",
                     "production-science-pack",
                     "utility-science-pack"
                 ],
                 "time": 60
             },
             "description": "",
-            "icon": "__base__/graphics/technology/flamethrower.png",
+            "icon": "__base__/graphics/technology/land-mine.png",
             "icon_size": 256,
-            "locale_name": "Flamethrower",
+            "locale_name": "Land Mine",
             "prerequisites": [
-                "randovania-worker-robots-speed-4"
+                "randovania-worker-robots-speed-e"
             ],
-            "tech_name": "randovania-worker-robots-speed-5",
+            "tech_name": "randovania-worker-robots-speed-f",
             "unlocks": [
-                "flamethrower"
+                "land-mine"
             ]
         }
     ]
 }
```

