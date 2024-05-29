# Comparing `tmp/swh_objstorage-3.1.0.tar.gz` & `tmp/swh_objstorage-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh_objstorage-3.1.0.tar", last modified: Fri May 24 11:59:46 2024, max compression
+gzip compressed data, was "swh_objstorage-3.1.1.tar", last modified: Wed May 29 14:23:25 2024, max compression
```

## Comparing `swh_objstorage-3.1.0.tar` & `swh_objstorage-3.1.1.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.335599 swh_objstorage-3.1.0/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      388 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)       37 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4479 2024-05-24 11:59:46.335599 swh_objstorage-3.1.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2275 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.303599 swh_objstorage-3.1.0/bin/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     3435 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/bin/swh-objstorage-azure
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3948 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.307599 swh_objstorage-3.1.0/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.307599 swh_objstorage-3.1.0/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.307599 swh_objstorage-3.1.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      284 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5513 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/winery.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      629 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2004 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)      125 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/requirements-azure.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       16 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/requirements-libcloud.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      172 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/requirements-winery.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      308 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-05-24 11:59:46.335599 swh_objstorage-3.1.0/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.295599 swh_objstorage-3.1.0/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.311599 swh_objstorage-3.1.0/swh/objstorage/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.311599 swh_objstorage-3.1.0/swh/objstorage/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2521 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/api/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5115 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/api/server.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.311599 swh_objstorage-3.1.0/swh/objstorage/backends/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17552 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/azure.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5306 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/generator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3294 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1855 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8398 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/libcloud.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1258 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/noop.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12102 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/pathslicing.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.315599 swh_objstorage-3.1.0/swh/objstorage/backends/seaweedfs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/seaweedfs/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4060 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/seaweedfs/http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5043 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/seaweedfs/objstorage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.315599 swh_objstorage-3.1.0/swh/objstorage/backends/winery/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      191 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2076 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/database.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2857 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/gunicorn.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15484 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/objstorage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16122 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/roshard.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6856 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/rwshard.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17191 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/sharedbase.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      944 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/sleep.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.315599 swh_objstorage-3.1.0/swh/objstorage/backends/winery/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1170 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/sql/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2810 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/stats.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6455 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/throttler.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12642 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1115 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/constants.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1971 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/exc.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3472 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/factory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8960 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16465 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/multiplexer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8303 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/objstorage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.319599 swh_objstorage-3.1.0/swh/objstorage/proxies/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2367 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/proxies/readonly.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1493 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.323599 swh_objstorage-3.1.0/swh/objstorage/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15606 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/objstorage_testing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1519 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1372 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_api.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12670 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_azure.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7640 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_cloud.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4729 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      466 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      794 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_instantiation.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13803 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_multiplexer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      512 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_noop.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7192 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_pathslicing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1630 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_random_generator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10093 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_seaweedfs.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    45626 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_winery.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2761 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_pathslicer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3148 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_readonly_filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4017 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    19921 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/winery_benchmark.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6882 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/winery_testing_helpers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      903 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.331599 swh_objstorage-3.1.0/swh.objstorage.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4479 2024-05-24 11:59:46.000000 swh_objstorage-3.1.0/swh.objstorage.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4064 2024-05-24 11:59:46.000000 swh_objstorage-3.1.0/swh.objstorage.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-24 11:59:46.000000 swh_objstorage-3.1.0/swh.objstorage.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-05-24 11:59:46.000000 swh_objstorage-3.1.0/swh.objstorage.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      487 2024-05-24 11:59:46.000000 swh_objstorage-3.1.0/swh.objstorage.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-24 11:59:46.000000 swh_objstorage-3.1.0/swh.objstorage.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1253 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/tox.ini
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.327599 swh_objstorage-3.1.0/winery-test-environment/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/README.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)      209 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/ansible.cfg
--rw-r--r--   0 jenkins    (115) jenkins    (120)      955 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/bootstrap.yml
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     4204 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/build-vms.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2038 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/ceph.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3932 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/fed4fire.rspec
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      844 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/fed4fire.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1836 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/grid5000.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.327599 swh_objstorage-3.1.0/winery-test-environment/inventory/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.299599 swh_objstorage-3.1.0/winery-test-environment/inventory/group_vars/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.327599 swh_objstorage-3.1.0/winery-test-environment/inventory/group_vars/all/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      108 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/inventory/group_vars/all/rw.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       91 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/inventory/groups.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      822 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/inventory/hosts.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       84 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/inventory/osd.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       75 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/libvirt.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.327599 swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       80 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/README.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2757 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2763 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen_free.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2895 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2765 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen_linear.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      824 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/osd.yml
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1333 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/remote-tox.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1733 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/render-stats.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       40 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      198 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/rng.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2727 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/rw.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/tests.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.524975 swh_objstorage-3.1.1/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      388 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       37 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4479 2024-05-29 14:23:25.524975 swh_objstorage-3.1.1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2275 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.496976 swh_objstorage-3.1.1/bin/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     3435 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/bin/swh-objstorage-azure
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3948 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.496976 swh_objstorage-3.1.1/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.496976 swh_objstorage-3.1.1/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.496976 swh_objstorage-3.1.1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      284 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5513 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/winery.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      629 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2004 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      125 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/requirements-azure.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       16 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/requirements-libcloud.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      172 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/requirements-winery.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      308 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-05-29 14:23:25.524975 swh_objstorage-3.1.1/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.488976 swh_objstorage-3.1.1/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.500976 swh_objstorage-3.1.1/swh/objstorage/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.504976 swh_objstorage-3.1.1/swh/objstorage/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2546 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/api/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5259 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/api/server.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.504976 swh_objstorage-3.1.1/swh/objstorage/backends/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17552 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/azure.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5306 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/generator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3294 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1855 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8398 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/libcloud.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1258 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/noop.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12102 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/pathslicing.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.504976 swh_objstorage-3.1.1/swh/objstorage/backends/seaweedfs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/seaweedfs/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4060 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/seaweedfs/http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5043 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/seaweedfs/objstorage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.508976 swh_objstorage-3.1.1/swh/objstorage/backends/winery/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      191 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2076 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/database.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2857 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/gunicorn.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15484 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/objstorage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16122 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/roshard.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6856 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/rwshard.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17191 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/sharedbase.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      944 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/sleep.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.508976 swh_objstorage-3.1.1/swh/objstorage/backends/winery/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1170 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/sql/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2810 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/stats.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6455 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/throttler.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12642 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1115 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/constants.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1971 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/exc.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3472 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/factory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8960 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16931 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/multiplexer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8303 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/objstorage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.508976 swh_objstorage-3.1.1/swh/objstorage/proxies/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2367 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/proxies/readonly.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1493 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.512976 swh_objstorage-3.1.1/swh/objstorage/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15606 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/objstorage_testing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1519 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2169 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_api.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12670 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_azure.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7640 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_cloud.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4729 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      466 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      794 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_instantiation.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13803 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_multiplexer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      512 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_noop.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7192 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_pathslicing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1630 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_random_generator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10093 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_seaweedfs.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    45626 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_winery.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2761 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_pathslicer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3148 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_readonly_filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4017 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    19921 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/winery_benchmark.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6882 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/winery_testing_helpers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      903 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.520975 swh_objstorage-3.1.1/swh.objstorage.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4479 2024-05-29 14:23:25.000000 swh_objstorage-3.1.1/swh.objstorage.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4064 2024-05-29 14:23:25.000000 swh_objstorage-3.1.1/swh.objstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-29 14:23:25.000000 swh_objstorage-3.1.1/swh.objstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-05-29 14:23:25.000000 swh_objstorage-3.1.1/swh.objstorage.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      487 2024-05-29 14:23:25.000000 swh_objstorage-3.1.1/swh.objstorage.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-29 14:23:25.000000 swh_objstorage-3.1.1/swh.objstorage.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1253 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.516975 swh_objstorage-3.1.1/winery-test-environment/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/README.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      209 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/ansible.cfg
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      955 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/bootstrap.yml
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     4204 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/build-vms.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2038 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/ceph.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3932 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/fed4fire.rspec
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      844 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/fed4fire.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1836 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/grid5000.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.520975 swh_objstorage-3.1.1/winery-test-environment/inventory/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.488976 swh_objstorage-3.1.1/winery-test-environment/inventory/group_vars/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.520975 swh_objstorage-3.1.1/winery-test-environment/inventory/group_vars/all/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      108 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/inventory/group_vars/all/rw.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       91 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/inventory/groups.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      822 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/inventory/hosts.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       84 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/inventory/osd.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       75 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/libvirt.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.520975 swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       80 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/README.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2757 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2763 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen_free.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2895 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2765 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen_linear.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      824 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/osd.yml
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1333 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/remote-tox.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1733 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/render-stats.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       40 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      198 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/rng.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2727 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/rw.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/tests.yml
```

### Comparing `swh_objstorage-3.1.0/.pre-commit-config.yaml` & `swh_objstorage-3.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/CODE_OF_CONDUCT.md` & `swh_objstorage-3.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/LICENSE` & `swh_objstorage-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/PKG-INFO` & `swh_objstorage-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage
-Version: 3.1.0
+Version: 3.1.1
 Summary: Software Heritage object storage
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-objstorage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage.git
```

### Comparing `swh_objstorage-3.1.0/README.rst` & `swh_objstorage-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/bin/swh-objstorage-azure` & `swh_objstorage-3.1.1/bin/swh-objstorage-azure`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/conftest.py` & `swh_objstorage-3.1.1/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/docs/winery.rst` & `swh_objstorage-3.1.1/docs/winery.rst`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/mypy.ini` & `swh_objstorage-3.1.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/pyproject.toml` & `swh_objstorage-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/api/client.py` & `swh_objstorage-3.1.1/swh/objstorage/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
     api_exception = ObjStorageAPIError
     reraise_exceptions = [
         ObjNotFoundError,
         Error,
         ObjCorruptedError,
         NoBackendsLeftError,
+        PermissionError,
     ]
     backend_class = ObjStorageInterface
     name: str = "remote"
 
     def restore(self: ObjStorageInterface, content: bytes, obj_id: ObjId) -> None:
         return self.add(content, obj_id, check_presence=False)
```

### Comparing `swh_objstorage-3.1.0/swh/objstorage/api/server.py` & `swh_objstorage-3.1.1/swh/objstorage/api/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,19 @@
 
 
 @app.errorhandler(Error)
 def argument_error_handler(exception):
     return error_handler(exception, encode_data, status_code=400)
 
 
+@app.errorhandler(PermissionError)
+def permission_error_handler(exception):
+    return error_handler(exception, encode_data, status_code=403)
+
+
 @app.errorhandler(Exception)
 def my_error_handler(exception):
     return error_handler(exception, encode_data)
 
 
 @app.route("/")
 @timed
```

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/azure.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/azure.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/generator.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/generator.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/http.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/http.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/in_memory.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/in_memory.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/libcloud.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/libcloud.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/noop.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/noop.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/pathslicing.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/pathslicing.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/seaweedfs/http.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/seaweedfs/http.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/seaweedfs/objstorage.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/seaweedfs/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/winery/database.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/winery/database.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/winery/gunicorn.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/winery/gunicorn.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/winery/objstorage.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/winery/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/winery/roshard.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/winery/roshard.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/winery/rwshard.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/winery/rwshard.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/winery/sharedbase.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/winery/sharedbase.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/winery/sleep.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/winery/sleep.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/winery/sql/30-schema.sql` & `swh_objstorage-3.1.1/swh/objstorage/backends/winery/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/winery/stats.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/winery/stats.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/backends/winery/throttler.py` & `swh_objstorage-3.1.1/swh/objstorage/backends/winery/throttler.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/cli.py` & `swh_objstorage-3.1.1/swh/objstorage/cli.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/constants.py` & `swh_objstorage-3.1.1/swh/objstorage/constants.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/exc.py` & `swh_objstorage-3.1.1/swh/objstorage/exc.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/factory.py` & `swh_objstorage-3.1.1/swh/objstorage/factory.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/interface.py` & `swh_objstorage-3.1.1/swh/objstorage/interface.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/multiplexer.py` & `swh_objstorage-3.1.1/swh/objstorage/multiplexer.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import queue
 import threading
 from typing import Dict, Iterable, Iterator, List, Mapping, Optional, Set, Tuple, Union
 
 # note: it's required to access the statsd object form the statsd module to
 # help mocking it in tests...
 from swh.core import statsd
+from swh.core.api import RemoteException
 from swh.model.model import Sha1
 from swh.objstorage.exc import (
     NoBackendsLeftError,
     ObjCorruptedError,
     ObjNotFoundError,
     ObjStorageAPIError,
 )
@@ -187,19 +188,31 @@
         self.storages = [
             get_objstorage(**sto) if isinstance(sto, dict) else sto
             for sto in objstorages
         ]
         self.storage_threads = [ObjStorageThread(storage) for storage in self.storages]
         for thread in self.storage_threads:
             thread.start()
-        self.write_storage_threads = [
-            thread
-            for thread, storage in zip(self.storage_threads, self.storages)
-            if storage.check_config(check_write=True)
-        ]
+
+        self.write_storage_threads = []
+        for thread, storage in zip(self.storage_threads, self.storages):
+            try:
+                checked = storage.check_config(check_write=True)
+            except PermissionError:
+                checked = False
+            except RemoteException:
+                logger.warning(
+                    "Received RemoteException when calling check_config on backend %s:",
+                    storage.name,
+                    exc_info=True,
+                )
+                checked = False
+
+            if checked:
+                self.write_storage_threads.append(thread)
 
         self.read_exception_cooldown = read_exception_cooldown
         self.transient_read_exceptions = set(
             transient_read_exceptions or DEFAULT_TRANSIENT_READ_EXCEPTIONS
         )
 
         self.active_readers: Set[int] = set()
```

### Comparing `swh_objstorage-3.1.0/swh/objstorage/objstorage.py` & `swh_objstorage-3.1.1/swh/objstorage/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/proxies/readonly.py` & `swh_objstorage-3.1.1/swh/objstorage/proxies/readonly.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/pytest_plugin.py` & `swh_objstorage-3.1.1/swh/objstorage/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/objstorage_testing.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/objstorage_testing.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/test_interface.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_azure.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_azure.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_cloud.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_cloud.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_http.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_http.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_instantiation.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_instantiation.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_multiplexer.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_multiplexer.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_noop.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_noop.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_pathslicing.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_pathslicing.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_random_generator.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_random_generator.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_seaweedfs.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_seaweedfs.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_winery.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_winery.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/test_pathslicer.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/test_pathslicer.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/test_readonly_filter.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/test_readonly_filter.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/test_server.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/winery_benchmark.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/winery_benchmark.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/tests/winery_testing_helpers.py` & `swh_objstorage-3.1.1/swh/objstorage/tests/winery_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh/objstorage/utils.py` & `swh_objstorage-3.1.1/swh/objstorage/utils.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/swh.objstorage.egg-info/PKG-INFO` & `swh_objstorage-3.1.1/swh.objstorage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage
-Version: 3.1.0
+Version: 3.1.1
 Summary: Software Heritage object storage
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-objstorage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage.git
```

### Comparing `swh_objstorage-3.1.0/swh.objstorage.egg-info/SOURCES.txt` & `swh_objstorage-3.1.1/swh.objstorage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/tox.ini` & `swh_objstorage-3.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/README.md` & `swh_objstorage-3.1.1/winery-test-environment/README.md`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/bootstrap.yml` & `swh_objstorage-3.1.1/winery-test-environment/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/build-vms.sh` & `swh_objstorage-3.1.1/winery-test-environment/build-vms.sh`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/ceph.yml` & `swh_objstorage-3.1.1/winery-test-environment/ceph.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/fed4fire.rspec` & `swh_objstorage-3.1.1/winery-test-environment/fed4fire.rspec`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/fed4fire.sh` & `swh_objstorage-3.1.1/winery-test-environment/fed4fire.sh`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/grid5000.yml` & `swh_objstorage-3.1.1/winery-test-environment/grid5000.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/inventory/hosts.yml` & `swh_objstorage-3.1.1/winery-test-environment/inventory/hosts.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen.py` & `swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen_free.py` & `swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen_free.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py` & `swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen_linear.py` & `swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen_linear.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/osd.yml` & `swh_objstorage-3.1.1/winery-test-environment/osd.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/remote-tox.sh` & `swh_objstorage-3.1.1/winery-test-environment/remote-tox.sh`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/render-stats.py` & `swh_objstorage-3.1.1/winery-test-environment/render-stats.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/rw.yml` & `swh_objstorage-3.1.1/winery-test-environment/rw.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.0/winery-test-environment/tests.yml` & `swh_objstorage-3.1.1/winery-test-environment/tests.yml`

 * *Files identical despite different names*

