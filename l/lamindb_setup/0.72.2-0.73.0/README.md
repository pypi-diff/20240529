# Comparing `tmp/lamindb_setup-0.72.2.tar.gz` & `tmp/lamindb_setup-0.73.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.72.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.73.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.72.2.tar` & `lamindb_setup-0.73.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0     8499 2024-05-10 21:24:49.730141 lamindb_setup-0.72.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2024-05-10 21:24:49.730245 lamindb_setup-0.72.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-05-10 21:24:49.730323 lamindb_setup-0.72.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1219 2024-05-10 21:24:49.730400 lamindb_setup-0.72.2/.gitignore
--rw-r--r--   0        0        0     1474 2024-05-10 21:24:49.730816 lamindb_setup-0.72.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2024-05-10 21:24:49.730899 lamindb_setup-0.72.2/LICENSE
--rw-r--r--   0        0        0      265 2024-05-10 21:24:49.730963 lamindb_setup-0.72.2/README.md
--rw-r--r--   0        0        0   102229 2024-05-21 16:43:05.022906 lamindb_setup-0.72.2/docs/changelog.md
--rw-r--r--   0        0        0     2574 2024-05-10 21:24:49.732231 lamindb_setup-0.72.2/docs/hub-cloud/01-init-local-instance.ipynb
--rw-r--r--   0        0        0     3948 2024-05-10 21:24:49.732413 lamindb_setup-0.72.2/docs/hub-cloud/02-connect-local-instance.ipynb
--rw-r--r--   0        0        0    10851 2024-05-10 21:27:09.131102 lamindb_setup-0.72.2/docs/hub-cloud/03-add-managed-storage.ipynb
--rw-r--r--   0        0        0     3339 2024-05-10 21:24:49.732848 lamindb_setup-0.72.2/docs/hub-cloud/04-test-bionty.ipynb
--rw-r--r--   0        0        0     3202 2024-05-19 16:54:54.607860 lamindb_setup-0.72.2/docs/hub-cloud/05-init-hosted-instance.ipynb
--rw-r--r--   0        0        0     3886 2024-05-10 21:24:49.733461 lamindb_setup-0.72.2/docs/hub-cloud/06-connect-hosted-instance.ipynb
--rw-r--r--   0        0        0     5454 2024-05-10 21:24:49.733811 lamindb_setup-0.72.2/docs/hub-cloud/07-keep-artifacts-local.ipynb
--rw-r--r--   0        0        0     3160 2024-05-10 21:24:49.734110 lamindb_setup-0.72.2/docs/hub-cloud/test-multi-session.ipynb
--rw-r--r--   0        0        0      177 2024-05-10 21:24:49.734470 lamindb_setup-0.72.2/docs/hub-cloud/test_notebooks.py
--rw-r--r--   0        0        0     6105 2024-05-10 21:24:49.735076 lamindb_setup-0.72.2/docs/hub-prod/test-cache-management.ipynb
--rw-r--r--   0        0        0    11402 2024-05-10 21:24:49.735685 lamindb_setup-0.72.2/docs/hub-prod/test-cloud-sync.ipynb
--rw-r--r--   0        0        0     1595 2024-05-10 21:24:49.736223 lamindb_setup-0.72.2/docs/hub-prod/test-connect-anonymously.ipynb
--rw-r--r--   0        0        0     2712 2024-05-10 21:24:49.736468 lamindb_setup-0.72.2/docs/hub-prod/test-empty-init.ipynb
--rw-r--r--   0        0        0     2681 2024-05-10 21:24:49.736795 lamindb_setup-0.72.2/docs/hub-prod/test-import-schema.ipynb
--rw-r--r--   0        0        0     4394 2024-05-10 21:24:49.737035 lamindb_setup-0.72.2/docs/hub-prod/test-insufficient-user-info.ipynb
--rw-r--r--   0        0        0      994 2024-05-10 21:24:49.737170 lamindb_setup-0.72.2/docs/hub-prod/test-invalid-schema.ipynb
--rw-r--r--   0        0        0     6182 2024-05-10 21:24:49.737508 lamindb_setup-0.72.2/docs/hub-prod/test-sqlite-lock.ipynb
--rw-r--r--   0        0        0      177 2024-05-10 21:24:49.737594 lamindb_setup-0.72.2/docs/hub-prod/test_notebooks2.py
--rw-r--r--   0        0        0      120 2024-05-10 21:24:49.737664 lamindb_setup-0.72.2/docs/index.md
--rw-r--r--   0        0        0      513 2024-05-10 21:24:49.737976 lamindb_setup-0.72.2/docs/notebooks.md
--rw-r--r--   0        0        0       61 2024-05-10 21:24:49.738046 lamindb_setup-0.72.2/docs/reference.md
--rw-r--r--   0        0        0     1542 2024-05-21 16:42:57.044808 lamindb_setup-0.72.2/lamindb_setup/__init__.py
--rw-r--r--   0        0        0      846 2024-05-10 21:24:49.738940 lamindb_setup-0.72.2/lamindb_setup/_cache.py
--rw-r--r--   0        0        0      129 2024-05-10 21:24:49.739174 lamindb_setup-0.72.2/lamindb_setup/_check.py
--rw-r--r--   0        0        0     2613 2024-05-10 21:24:49.739337 lamindb_setup-0.72.2/lamindb_setup/_check_setup.py
--rw-r--r--   0        0        0     1186 2024-05-10 21:24:49.739588 lamindb_setup-0.72.2/lamindb_setup/_close.py
--rw-r--r--   0        0        0    12728 2024-05-10 21:27:09.131888 lamindb_setup-0.72.2/lamindb_setup/_connect_instance.py
--rw-r--r--   0        0        0     5524 2024-05-19 16:54:54.608343 lamindb_setup-0.72.2/lamindb_setup/_delete.py
--rw-r--r--   0        0        0     1534 2024-05-10 21:24:49.740572 lamindb_setup-0.72.2/lamindb_setup/_django.py
--rw-r--r--   0        0        0     2120 2024-05-10 21:24:49.740766 lamindb_setup-0.72.2/lamindb_setup/_exportdb.py
--rw-r--r--   0        0        0     1874 2024-05-10 21:24:49.741154 lamindb_setup-0.72.2/lamindb_setup/_importdb.py
--rw-r--r--   0        0        0    11897 2024-05-10 21:27:09.133186 lamindb_setup-0.72.2/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     8815 2024-05-10 21:24:49.741821 lamindb_setup-0.72.2/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0      940 2024-05-10 21:24:49.742316 lamindb_setup-0.72.2/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0      679 2024-05-10 21:24:49.742498 lamindb_setup-0.72.2/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1419 2024-05-10 21:27:09.133733 lamindb_setup-0.72.2/lamindb_setup/_set_managed_storage.py
--rw-r--r--   0        0        0     3670 2024-05-10 21:24:49.743106 lamindb_setup-0.72.2/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0     1568 2024-05-10 21:24:49.743380 lamindb_setup-0.72.2/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      416 2024-05-10 21:24:49.743642 lamindb_setup-0.72.2/lamindb_setup/core/__init__.py
--rw-r--r--   0        0        0     5293 2024-05-20 12:51:17.170079 lamindb_setup-0.72.2/lamindb_setup/core/_aws_credentials.py
--rw-r--r--   0        0        0     1799 2024-05-10 21:24:49.743767 lamindb_setup-0.72.2/lamindb_setup/core/_aws_storage.py
--rw-r--r--   0        0        0     2520 2024-05-10 21:24:49.743894 lamindb_setup-0.72.2/lamindb_setup/core/_deprecated.py
--rw-r--r--   0        0        0      276 2024-05-10 21:24:49.744017 lamindb_setup-0.72.2/lamindb_setup/core/_docs.py
--rw-r--r--   0        0        0     5504 2024-05-10 21:24:49.744168 lamindb_setup-0.72.2/lamindb_setup/core/_hub_client.py
--rw-r--r--   0        0        0    16352 2024-05-19 18:41:24.261649 lamindb_setup-0.72.2/lamindb_setup/core/_hub_core.py
--rw-r--r--   0        0        0     4859 2024-05-10 21:24:49.745092 lamindb_setup-0.72.2/lamindb_setup/core/_hub_crud.py
--rw-r--r--   0        0        0     1875 2024-05-10 21:24:49.745226 lamindb_setup-0.72.2/lamindb_setup/core/_hub_utils.py
--rw-r--r--   0        0        0     3141 2024-05-10 21:24:49.745514 lamindb_setup-0.72.2/lamindb_setup/core/_settings.py
--rw-r--r--   0        0        0    16949 2024-05-20 14:46:17.603753 lamindb_setup-0.72.2/lamindb_setup/core/_settings_instance.py
--rw-r--r--   0        0        0     3922 2024-05-10 21:24:49.746016 lamindb_setup-0.72.2/lamindb_setup/core/_settings_load.py
--rw-r--r--   0        0        0     2704 2024-05-10 21:24:49.746338 lamindb_setup-0.72.2/lamindb_setup/core/_settings_save.py
--rw-r--r--   0        0        0    13236 2024-05-19 16:54:54.609402 lamindb_setup-0.72.2/lamindb_setup/core/_settings_storage.py
--rw-r--r--   0        0        0     2084 2024-05-10 21:24:49.747202 lamindb_setup-0.72.2/lamindb_setup/core/_settings_store.py
--rw-r--r--   0        0        0     1344 2024-05-10 21:24:49.747359 lamindb_setup-0.72.2/lamindb_setup/core/_settings_user.py
--rw-r--r--   0        0        0     3002 2024-05-10 21:24:49.747517 lamindb_setup-0.72.2/lamindb_setup/core/_setup_bionty_sources.py
--rw-r--r--   0        0        0     6893 2024-05-10 21:24:49.747774 lamindb_setup-0.72.2/lamindb_setup/core/cloud_sqlite_locker.py
--rw-r--r--   0        0        0     3542 2024-05-16 15:52:55.373912 lamindb_setup-0.72.2/lamindb_setup/core/django.py
--rw-r--r--   0        0        0      305 2024-05-10 21:24:49.748488 lamindb_setup-0.72.2/lamindb_setup/core/exceptions.py
--rw-r--r--   0        0        0     2269 2024-05-16 15:52:55.374538 lamindb_setup-0.72.2/lamindb_setup/core/hashing.py
--rw-r--r--   0        0        0      532 2024-05-10 21:24:49.749051 lamindb_setup-0.72.2/lamindb_setup/core/types.py
--rw-r--r--   0        0        0    26339 2024-05-19 16:54:54.609931 lamindb_setup-0.72.2/lamindb_setup/core/upath.py
--rw-r--r--   0        0        0     3325 2024-05-10 21:24:49.749714 lamindb_setup-0.72.2/noxfile.py
--rw-r--r--   0        0        0     4138 2024-05-10 21:24:49.750224 lamindb_setup-0.72.2/pyproject.toml
--rw-r--r--   0        0        0     5387 2024-05-10 21:24:49.750488 lamindb_setup-0.72.2/tests/hub-cloud/test_connect_instance.py
--rw-r--r--   0        0        0      270 2024-05-10 21:24:49.751063 lamindb_setup-0.72.2/tests/hub-cloud/test_delete_instance.py
--rw-r--r--   0        0        0     5716 2024-05-10 21:24:49.751513 lamindb_setup-0.72.2/tests/hub-cloud/test_init_instance.py
--rw-r--r--   0        0        0      538 2024-05-10 21:24:49.751867 lamindb_setup-0.72.2/tests/hub-cloud/test_login.py
--rw-r--r--   0        0        0      504 2024-05-10 21:24:49.752008 lamindb_setup-0.72.2/tests/hub-cloud/test_migrate.py
--rw-r--r--   0        0        0      482 2024-05-10 21:24:49.752363 lamindb_setup-0.72.2/tests/hub-cloud/test_set_storage.py
--rw-r--r--   0        0        0      595 2024-05-10 21:24:49.752562 lamindb_setup-0.72.2/tests/hub-local/conftest.py
--rw-r--r--   0        0        0    11234 2024-05-10 21:24:49.752730 lamindb_setup-0.72.2/tests/hub-local/test_all.py
--rw-r--r--   0        0        0      772 2024-05-10 21:27:09.135946 lamindb_setup-0.72.2/tests/hub-prod/conftest.py
--rw-r--r--   0        0        0      401 2024-05-10 21:24:49.753243 lamindb_setup-0.72.2/tests/hub-prod/test_auto_connect.py
--rw-r--r--   0        0        0      193 2024-05-10 21:24:49.753482 lamindb_setup-0.72.2/tests/hub-prod/test_django.py
--rw-r--r--   0        0        0     1469 2024-05-10 21:24:49.753625 lamindb_setup-0.72.2/tests/hub-prod/test_switch_and_fallback_env.py
--rw-r--r--   0        0        0     1109 2024-05-10 21:24:49.754187 lamindb_setup-0.72.2/tests/hub-prod/test_upath.py
--rw-r--r--   0        0        0     1642 2024-05-10 21:24:49.754795 lamindb_setup-0.72.2/tests/storage/test_hashing.py
--rw-r--r--   0        0        0     2023 2024-05-10 21:24:49.755035 lamindb_setup-0.72.2/tests/storage/test_storage_access.py
--rw-r--r--   0        0        0      891 2024-05-10 21:24:49.755350 lamindb_setup-0.72.2/tests/storage/test_storage_basis.py
--rw-r--r--   0        0        0      878 2024-05-10 21:24:49.755587 lamindb_setup-0.72.2/tests/storage/test_storage_stats.py
--rw-r--r--   0        0        0     1058 2024-05-10 21:24:49.755741 lamindb_setup-0.72.2/tests/storage/test_to_url.py
--rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 lamindb_setup-0.72.2/PKG-INFO
+-rw-r--r--   0        0        0     8452 2024-05-23 08:04:22.737551 lamindb_setup-0.73.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2024-05-10 21:24:49.730245 lamindb_setup-0.73.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-05-10 21:24:49.730323 lamindb_setup-0.73.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1219 2024-05-10 21:24:49.730400 lamindb_setup-0.73.0/.gitignore
+-rw-r--r--   0        0        0     1479 2024-05-23 17:07:32.497702 lamindb_setup-0.73.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2024-05-10 21:24:49.730899 lamindb_setup-0.73.0/LICENSE
+-rw-r--r--   0        0        0      265 2024-05-10 21:24:49.730963 lamindb_setup-0.73.0/README.md
+-rw-r--r--   0        0        0   103055 2024-05-29 09:01:20.445389 lamindb_setup-0.73.0/docs/changelog.md
+-rw-r--r--   0        0        0     2574 2024-05-10 21:24:49.732231 lamindb_setup-0.73.0/docs/hub-cloud/01-init-local-instance.ipynb
+-rw-r--r--   0        0        0     3948 2024-05-10 21:24:49.732413 lamindb_setup-0.73.0/docs/hub-cloud/02-connect-local-instance.ipynb
+-rw-r--r--   0        0        0    10851 2024-05-10 21:27:09.131102 lamindb_setup-0.73.0/docs/hub-cloud/03-add-managed-storage.ipynb
+-rw-r--r--   0        0        0     3339 2024-05-10 21:24:49.732848 lamindb_setup-0.73.0/docs/hub-cloud/04-test-bionty.ipynb
+-rw-r--r--   0        0        0     3202 2024-05-23 16:27:35.767272 lamindb_setup-0.73.0/docs/hub-cloud/05-init-hosted-instance.ipynb
+-rw-r--r--   0        0        0     4716 2024-05-24 12:12:04.704910 lamindb_setup-0.73.0/docs/hub-cloud/06-connect-hosted-instance.ipynb
+-rw-r--r--   0        0        0     5454 2024-05-10 21:24:49.733811 lamindb_setup-0.73.0/docs/hub-cloud/07-keep-artifacts-local.ipynb
+-rw-r--r--   0        0        0     3160 2024-05-10 21:24:49.734110 lamindb_setup-0.73.0/docs/hub-cloud/test-multi-session.ipynb
+-rw-r--r--   0        0        0      177 2024-05-10 21:24:49.734470 lamindb_setup-0.73.0/docs/hub-cloud/test_notebooks.py
+-rw-r--r--   0        0        0     6105 2024-05-10 21:24:49.735076 lamindb_setup-0.73.0/docs/hub-prod/test-cache-management.ipynb
+-rw-r--r--   0        0        0    11402 2024-05-10 21:24:49.735685 lamindb_setup-0.73.0/docs/hub-prod/test-cloud-sync.ipynb
+-rw-r--r--   0        0        0     1595 2024-05-10 21:24:49.736223 lamindb_setup-0.73.0/docs/hub-prod/test-connect-anonymously.ipynb
+-rw-r--r--   0        0        0     2712 2024-05-10 21:24:49.736468 lamindb_setup-0.73.0/docs/hub-prod/test-empty-init.ipynb
+-rw-r--r--   0        0        0     2681 2024-05-10 21:24:49.736795 lamindb_setup-0.73.0/docs/hub-prod/test-import-schema.ipynb
+-rw-r--r--   0        0        0     4394 2024-05-10 21:24:49.737035 lamindb_setup-0.73.0/docs/hub-prod/test-insufficient-user-info.ipynb
+-rw-r--r--   0        0        0      994 2024-05-10 21:24:49.737170 lamindb_setup-0.73.0/docs/hub-prod/test-invalid-schema.ipynb
+-rw-r--r--   0        0        0     6182 2024-05-10 21:24:49.737508 lamindb_setup-0.73.0/docs/hub-prod/test-sqlite-lock.ipynb
+-rw-r--r--   0        0        0      177 2024-05-10 21:24:49.737594 lamindb_setup-0.73.0/docs/hub-prod/test_notebooks2.py
+-rw-r--r--   0        0        0      120 2024-05-10 21:24:49.737664 lamindb_setup-0.73.0/docs/index.md
+-rw-r--r--   0        0        0      513 2024-05-10 21:24:49.737976 lamindb_setup-0.73.0/docs/notebooks.md
+-rw-r--r--   0        0        0       61 2024-05-10 21:24:49.738046 lamindb_setup-0.73.0/docs/reference.md
+-rw-r--r--   0        0        0     1542 2024-05-29 09:01:09.832831 lamindb_setup-0.73.0/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0      846 2024-05-10 21:24:49.738940 lamindb_setup-0.73.0/lamindb_setup/_cache.py
+-rw-r--r--   0        0        0      129 2024-05-10 21:24:49.739174 lamindb_setup-0.73.0/lamindb_setup/_check.py
+-rw-r--r--   0        0        0     2613 2024-05-10 21:24:49.739337 lamindb_setup-0.73.0/lamindb_setup/_check_setup.py
+-rw-r--r--   0        0        0     1186 2024-05-10 21:24:49.739588 lamindb_setup-0.73.0/lamindb_setup/_close.py
+-rw-r--r--   0        0        0    12728 2024-05-10 21:27:09.131888 lamindb_setup-0.73.0/lamindb_setup/_connect_instance.py
+-rw-r--r--   0        0        0     5524 2024-05-19 16:54:54.608343 lamindb_setup-0.73.0/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0     1534 2024-05-10 21:24:49.740572 lamindb_setup-0.73.0/lamindb_setup/_django.py
+-rw-r--r--   0        0        0     2120 2024-05-10 21:24:49.740766 lamindb_setup-0.73.0/lamindb_setup/_exportdb.py
+-rw-r--r--   0        0        0     1874 2024-05-10 21:24:49.741154 lamindb_setup-0.73.0/lamindb_setup/_importdb.py
+-rw-r--r--   0        0        0    11918 2024-05-22 08:35:29.362019 lamindb_setup-0.73.0/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     8815 2024-05-22 05:34:38.996454 lamindb_setup-0.73.0/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0      940 2024-05-10 21:24:49.742316 lamindb_setup-0.73.0/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0      679 2024-05-10 21:24:49.742498 lamindb_setup-0.73.0/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1419 2024-05-10 21:27:09.133733 lamindb_setup-0.73.0/lamindb_setup/_set_managed_storage.py
+-rw-r--r--   0        0        0     3670 2024-05-10 21:24:49.743106 lamindb_setup-0.73.0/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0     1568 2024-05-10 21:24:49.743380 lamindb_setup-0.73.0/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      416 2024-05-10 21:24:49.743642 lamindb_setup-0.73.0/lamindb_setup/core/__init__.py
+-rw-r--r--   0        0        0     5293 2024-05-20 12:51:17.170079 lamindb_setup-0.73.0/lamindb_setup/core/_aws_credentials.py
+-rw-r--r--   0        0        0     1799 2024-05-10 21:24:49.743767 lamindb_setup-0.73.0/lamindb_setup/core/_aws_storage.py
+-rw-r--r--   0        0        0     2520 2024-05-10 21:24:49.743894 lamindb_setup-0.73.0/lamindb_setup/core/_deprecated.py
+-rw-r--r--   0        0        0      276 2024-05-10 21:24:49.744017 lamindb_setup-0.73.0/lamindb_setup/core/_docs.py
+-rw-r--r--   0        0        0     5504 2024-05-10 21:24:49.744168 lamindb_setup-0.73.0/lamindb_setup/core/_hub_client.py
+-rw-r--r--   0        0        0    16352 2024-05-19 18:41:24.261649 lamindb_setup-0.73.0/lamindb_setup/core/_hub_core.py
+-rw-r--r--   0        0        0     4859 2024-05-10 21:24:49.745092 lamindb_setup-0.73.0/lamindb_setup/core/_hub_crud.py
+-rw-r--r--   0        0        0     1875 2024-05-10 21:24:49.745226 lamindb_setup-0.73.0/lamindb_setup/core/_hub_utils.py
+-rw-r--r--   0        0        0     3141 2024-05-10 21:24:49.745514 lamindb_setup-0.73.0/lamindb_setup/core/_settings.py
+-rw-r--r--   0        0        0    16949 2024-05-20 14:46:17.603753 lamindb_setup-0.73.0/lamindb_setup/core/_settings_instance.py
+-rw-r--r--   0        0        0     3922 2024-05-10 21:24:49.746016 lamindb_setup-0.73.0/lamindb_setup/core/_settings_load.py
+-rw-r--r--   0        0        0     2704 2024-05-10 21:24:49.746338 lamindb_setup-0.73.0/lamindb_setup/core/_settings_save.py
+-rw-r--r--   0        0        0    13137 2024-05-23 08:04:22.738230 lamindb_setup-0.73.0/lamindb_setup/core/_settings_storage.py
+-rw-r--r--   0        0        0     2084 2024-05-10 21:24:49.747202 lamindb_setup-0.73.0/lamindb_setup/core/_settings_store.py
+-rw-r--r--   0        0        0     1344 2024-05-10 21:24:49.747359 lamindb_setup-0.73.0/lamindb_setup/core/_settings_user.py
+-rw-r--r--   0        0        0     3072 2024-05-22 08:35:29.362303 lamindb_setup-0.73.0/lamindb_setup/core/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     6893 2024-05-10 21:24:49.747774 lamindb_setup-0.73.0/lamindb_setup/core/cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     3542 2024-05-16 15:52:55.373912 lamindb_setup-0.73.0/lamindb_setup/core/django.py
+-rw-r--r--   0        0        0      305 2024-05-10 21:24:49.748488 lamindb_setup-0.73.0/lamindb_setup/core/exceptions.py
+-rw-r--r--   0        0        0     2269 2024-05-16 15:52:55.374538 lamindb_setup-0.73.0/lamindb_setup/core/hashing.py
+-rw-r--r--   0        0        0      532 2024-05-10 21:24:49.749051 lamindb_setup-0.73.0/lamindb_setup/core/types.py
+-rw-r--r--   0        0        0    28135 2024-05-24 12:12:04.705519 lamindb_setup-0.73.0/lamindb_setup/core/upath.py
+-rw-r--r--   0        0        0     3330 2024-05-23 08:04:22.738566 lamindb_setup-0.73.0/noxfile.py
+-rw-r--r--   0        0        0     4138 2024-05-10 21:24:49.750224 lamindb_setup-0.73.0/pyproject.toml
+-rw-r--r--   0        0        0     5387 2024-05-10 21:24:49.750488 lamindb_setup-0.73.0/tests/hub-cloud/test_connect_instance.py
+-rw-r--r--   0        0        0      270 2024-05-10 21:24:49.751063 lamindb_setup-0.73.0/tests/hub-cloud/test_delete_instance.py
+-rw-r--r--   0        0        0     5716 2024-05-10 21:24:49.751513 lamindb_setup-0.73.0/tests/hub-cloud/test_init_instance.py
+-rw-r--r--   0        0        0      538 2024-05-10 21:24:49.751867 lamindb_setup-0.73.0/tests/hub-cloud/test_login.py
+-rw-r--r--   0        0        0      504 2024-05-10 21:24:49.752008 lamindb_setup-0.73.0/tests/hub-cloud/test_migrate.py
+-rw-r--r--   0        0        0      482 2024-05-10 21:24:49.752363 lamindb_setup-0.73.0/tests/hub-cloud/test_set_storage.py
+-rw-r--r--   0        0        0      595 2024-05-10 21:24:49.752562 lamindb_setup-0.73.0/tests/hub-local/conftest.py
+-rw-r--r--   0        0        0    11234 2024-05-10 21:24:49.752730 lamindb_setup-0.73.0/tests/hub-local/test_all.py
+-rw-r--r--   0        0        0      772 2024-05-10 21:27:09.135946 lamindb_setup-0.73.0/tests/hub-prod/conftest.py
+-rw-r--r--   0        0        0      401 2024-05-10 21:24:49.753243 lamindb_setup-0.73.0/tests/hub-prod/test_auto_connect.py
+-rw-r--r--   0        0        0      193 2024-05-10 21:24:49.753482 lamindb_setup-0.73.0/tests/hub-prod/test_django.py
+-rw-r--r--   0        0        0     1469 2024-05-10 21:24:49.753625 lamindb_setup-0.73.0/tests/hub-prod/test_switch_and_fallback_env.py
+-rw-r--r--   0        0        0     1109 2024-05-10 21:24:49.754187 lamindb_setup-0.73.0/tests/hub-prod/test_upath.py
+-rw-r--r--   0        0        0     1642 2024-05-10 21:24:49.754795 lamindb_setup-0.73.0/tests/storage/test_hashing.py
+-rw-r--r--   0        0        0     2023 2024-05-10 21:24:49.755035 lamindb_setup-0.73.0/tests/storage/test_storage_access.py
+-rw-r--r--   0        0        0      891 2024-05-10 21:24:49.755350 lamindb_setup-0.73.0/tests/storage/test_storage_basis.py
+-rw-r--r--   0        0        0     1160 2024-05-23 17:07:32.498432 lamindb_setup-0.73.0/tests/storage/test_storage_stats.py
+-rw-r--r--   0        0        0     1058 2024-05-10 21:24:49.755741 lamindb_setup-0.73.0/tests/storage/test_to_url.py
+-rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 lamindb_setup-0.73.0/PKG-INFO
```

### Comparing `lamindb_setup-0.72.2/.github/workflows/build.yml` & `lamindb_setup-0.73.0/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,21 @@
   repository_dispatch:
     types: [build]
 
 jobs:
   # tests only on production hub
   hub-prod:
     runs-on: ubuntu-latest
-    timeout-minutes: 10
+    timeout-minutes: 6
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: "3.9" # consciously run one job on Python 3.9
+          python-version: "3.9" # run one job on 3.9
           cache: "pip"
-          cache-dependency-path: ".github/workflows/build.yml"
       - uses: aws-actions/configure-aws-credentials@v2
         with:
           aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
           aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
           aws-region: eu-central-1
       - run: pip install -U laminci
       - run: nox -s "install(group='hub-prod')"
@@ -35,28 +34,30 @@
 
   # tests both on production and staging hub
   hub-cloud:
     runs-on: ubuntu-22.04
     strategy:
       fail-fast: false
       matrix:
-        lamin_env:
-          - "staging"
-          - "prod"
-    timeout-minutes: 15
+        include:
+          - lamin_env: "prod"
+            python-version: "3.11"
+          - lamin_env: "staging"
+            python-version: "3.10" # test on 3.10
+    timeout-minutes: 6
     steps:
       - uses: aws-actions/configure-aws-credentials@v2
         with:
           aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
           aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
           aws-region: eu-central-1
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
-          python-version: "3.11" # consciously run one job on Python 3.11
+          python-version: ${{ matrix.python-version }}
           cache: "pip"
           cache-dependency-path: ".github/workflows/build.yml"
       - name: checkout laminhub
         uses: actions/checkout@v4
         with:
           repository: laminlabs/laminapp-ui
           token: ${{ secrets.GH_TOKEN_DEPLOY_LAMINAPP }}
@@ -88,20 +89,20 @@
         with:
           name: coverage--hub-cloud
           path: .coverage
 
   # test user access to storage
   storage:
     runs-on: ubuntu-latest
-    timeout-minutes: 10
+    timeout-minutes: 6
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
-          python-version: "3.10" # consciously run one job on Python 3.10
+          python-version: "3.11" # we need to run everything for coverage on 3.11
           cache: "pip"
           cache-dependency-path: ".github/workflows/build.yml"
       - run: pip install -U laminci
       - run: nox -s "install(group='storage')"
       - run: nox -s lint
       - run: nox -s storage
         env:
@@ -112,15 +113,15 @@
         with:
           name: coverage--storage
           path: .coverage
 
   # test low-level hub functionality
   hub-local:
     runs-on: ubuntu-latest
-    timeout-minutes: 10
+    timeout-minutes: 6
     steps:
       - uses: aws-actions/configure-aws-credentials@v2
         with:
           aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
           aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
           aws-region: eu-central-1
       - uses: actions/checkout@v4
@@ -135,15 +136,15 @@
         run: |
           touch .env.local
           echo "AWS_ACCESS_KEY_ID_HOSTED_S3=${{ secrets.AWS_ACCESS_KEY_ID }}" >> .env.local
           echo "AWS_SECRET_ACCESS_KEY_HOSTED_S3=${{ secrets.AWS_SECRET_ACCESS_KEY }}" >> .env.local
         working-directory: laminhub/rest-hub/supabase
       - uses: actions/setup-python@v4
         with:
-          python-version: "3.11" # consciously run one job on Python 3.11
+          python-version: "3.11" # we need to run everything for coverage on 3.11
           cache: "pip"
           cache-dependency-path: ".github/workflows/build.yml"
       - run: pip install -U laminci
       - run: nox -s "install(group='hub-local')"
       - id: cache-supabase
         uses: actions/cache@v3
         with:
@@ -161,17 +162,16 @@
   coverage:
     needs: [hub-prod, hub-cloud, storage, hub-local]
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
           cache: "pip"
-          cache-dependency-path: ".github/workflows/build.yml"
       - run: |
           pip install coverage[toml]
           pip install --no-deps .
       - uses: actions/download-artifact@v2
       - name: run coverage
         run: |
           coverage combine coverage--*/.coverage*
```

### Comparing `lamindb_setup-0.72.2/.github/workflows/latest-changes.yml` & `lamindb_setup-0.73.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/.gitignore` & `lamindb_setup-0.73.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/.pre-commit-config.yaml` & `lamindb_setup-0.73.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -45,8 +45,8 @@
               tests/hub-local/conftest.py
           )
   - repo: https://github.com/pycqa/pydocstyle
     rev: 6.1.1
     hooks:
       - id: pydocstyle
         args: # google style + __init__, see http://www.pydocstyle.org/en/stable/error_codes.html
-          - --ignore=D100,D101,D102,D103,D104,D106,D107,D203,D204,D213,D215,D400,D401,D403,D404,D406,D407,D408,D409,D412,D413
+          - --ignore=D100,D101,D102,D103,D104,D106,D107,D203,D204,D213,D215,D400,D401,D403,D404,D406,D407,D408,D409,D412,D413,D417
```

### Comparing `lamindb_setup-0.72.2/LICENSE` & `lamindb_setup-0.73.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/changelog.md` & `lamindb_setup-0.73.0/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🐛 Fix trailing slash in upload_from source | [773](https://github.com/laminlabs/lamindb-setup/pull/773) | [Koncopd](https://github.com/Koncopd) | 2024-05-23 | 0.73.0
+🚸 Make `upload_from()`, `download_to()`, and `view_tree()` more user friendly | [772](https://github.com/laminlabs/lamindb-setup/pull/772) | [falexwolf](https://github.com/falexwolf) | 2024-05-23 |
+✨ Resolve s3 bucket region even without access rights | [771](https://github.com/laminlabs/lamindb-setup/pull/771) | [Koncopd](https://github.com/Koncopd) | 2024-05-22 |
+💚 Coverage fix | [770](https://github.com/laminlabs/lamindb-setup/pull/770) | [falexwolf](https://github.com/falexwolf) | 2024-05-22 |
+👷 Fix coverage compute | [769](https://github.com/laminlabs/lamindb-setup/pull/769) | [falexwolf](https://github.com/falexwolf) | 2024-05-22 |
 🐛 Deal with migration errors when keep-artifacts-local is true | [767](https://github.com/laminlabs/lamindb-setup/pull/767) | [falexwolf](https://github.com/falexwolf) | 2024-05-20 | 0.72.2
 ♻️ Do not error if empty dict in `access_aws` | [764](https://github.com/laminlabs/lamindb-setup/pull/764) | [falexwolf](https://github.com/falexwolf) | 2024-05-19 | 0.72.1
 🐛 Keep training slash in aws cache keys | [766](https://github.com/laminlabs/lamindb-setup/pull/766) | [Koncopd](https://github.com/Koncopd) | 2024-05-19 |
 🐛 Check empty after storage record root init in delete | [763](https://github.com/laminlabs/lamindb-setup/pull/763) | [Koncopd](https://github.com/Koncopd) | 2024-05-18 |
 ✨ Call `access_aws` for all paths and cache | [762](https://github.com/laminlabs/lamindb-setup/pull/762) | [Koncopd](https://github.com/Koncopd) | 2024-05-18 | 0.72.0
 ⚡️ Speed-up file hash | [761](https://github.com/laminlabs/lamindb-setup/pull/761) | [Koncopd](https://github.com/Koncopd) | 2024-05-11 | 0.71.4
 ♻️ Account for public storage locations | [758](https://github.com/laminlabs/lamindb-setup/pull/758) | [falexwolf](https://github.com/falexwolf) | 2024-05-10 |
```

### Comparing `lamindb_setup-0.72.2/docs/hub-cloud/01-init-local-instance.ipynb` & `lamindb_setup-0.73.0/docs/hub-cloud/01-init-local-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/hub-cloud/02-connect-local-instance.ipynb` & `lamindb_setup-0.73.0/docs/hub-cloud/02-connect-local-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/hub-cloud/03-add-managed-storage.ipynb` & `lamindb_setup-0.73.0/docs/hub-cloud/03-add-managed-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/hub-cloud/04-test-bionty.ipynb` & `lamindb_setup-0.73.0/docs/hub-cloud/04-test-bionty.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/hub-cloud/05-init-hosted-instance.ipynb` & `lamindb_setup-0.73.0/docs/hub-cloud/05-init-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/hub-cloud/06-connect-hosted-instance.ipynb` & `lamindb_setup-0.73.0/docs/hub-cloud/06-connect-hosted-instance.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9899918831168831%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(1, 'target_dir.upload_from(test_dir)\\n'), (5, 'assert "*

 * *            '(target_dir / "test-dir-upload/file1").exists()\\n\')], delete: [1]}}, 9: '*

 * *            '{\'source\': {insert: [(0, \'target_dir_check = root / "test-dir-upload"\\n\'), (1, '*

 * *            "'assert not target_dir_check.exists()\\n'), (3, 'target_dir.upload_from(test_dir, "*

 * *            "create_folder=False)\\n'), (4, '\\n'), (5, 'assert target_dir_check.is_dir()\\n'), "*

 * *            '(6, \'assert (target […]*

```diff
@@ -82,33 +82,58 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "target_dir = root / \"test-dir-upload\"\n",
-                "target_dir.upload_from(test_dir, recursive=True)\n",
+                "target_dir.upload_from(test_dir)\n",
                 "\n",
                 "assert target_dir.is_dir()\n",
                 "assert (target_dir / \"test-dir-upload\").exists()\n",
+                "assert (target_dir / \"test-dir-upload/file1\").exists()\n",
                 "\n",
                 "target_dir.rmdir()\n",
                 "assert not target_dir.exists()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "target_dir.upload_from(test_dir, dir_inplace=True)\n",
+                "# test trailing slash in target_dir\n",
+                "target_dir = root / \"test-dir-upload/\"\n",
+                "assert target_dir.path.endswith(\"/\")\n",
                 "\n",
-                "assert target_dir.is_dir()\n",
-                "assert not (target_dir / \"test-dir-upload\").exists()"
+                "dest_dir = target_dir.upload_from(test_dir, create_folder=True)\n",
+                "\n",
+                "assert \"//\" not in dest_dir.path\n",
+                "assert dest_dir.as_posix() == (root / \"test-dir-upload/test-dir-upload\").as_posix()\n",
+                "assert dest_dir.is_dir()\n",
+                "\n",
+                "dest_dir.rmdir()\n",
+                "assert not dest_dir.exists()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "target_dir_check = root / \"test-dir-upload\"\n",
+                "assert not target_dir_check.exists()\n",
+                "\n",
+                "target_dir.upload_from(test_dir, create_folder=False)\n",
+                "\n",
+                "assert target_dir_check.is_dir()\n",
+                "assert (target_dir_check / \"file1\").exists()\n",
+                "assert not (target_dir_check / \"test-dir-upload\").exists()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Test that instance can not be deleted from hub:"
```

### Comparing `lamindb_setup-0.72.2/docs/hub-cloud/07-keep-artifacts-local.ipynb` & `lamindb_setup-0.73.0/docs/hub-cloud/07-keep-artifacts-local.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/hub-cloud/test-multi-session.ipynb` & `lamindb_setup-0.73.0/docs/hub-cloud/test-multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/hub-prod/test-cache-management.ipynb` & `lamindb_setup-0.73.0/docs/hub-prod/test-cache-management.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/hub-prod/test-cloud-sync.ipynb` & `lamindb_setup-0.73.0/docs/hub-prod/test-cloud-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/hub-prod/test-connect-anonymously.ipynb` & `lamindb_setup-0.73.0/docs/hub-prod/test-connect-anonymously.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/hub-prod/test-empty-init.ipynb` & `lamindb_setup-0.73.0/docs/hub-prod/test-empty-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/hub-prod/test-import-schema.ipynb` & `lamindb_setup-0.73.0/docs/hub-prod/test-import-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/hub-prod/test-insufficient-user-info.ipynb` & `lamindb_setup-0.73.0/docs/hub-prod/test-insufficient-user-info.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/hub-prod/test-invalid-schema.ipynb` & `lamindb_setup-0.73.0/docs/hub-prod/test-invalid-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/hub-prod/test-sqlite-lock.ipynb` & `lamindb_setup-0.73.0/docs/hub-prod/test-sqlite-lock.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/docs/notebooks.md` & `lamindb_setup-0.73.0/docs/notebooks.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/__init__.py` & `lamindb_setup-0.73.0/lamindb_setup/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
    settings
    core
    django
 
 """
 
-__version__ = "0.72.2"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.73.0"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import core
 from ._check_setup import _check_instance_setup
 from ._close import close
```

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_cache.py` & `lamindb_setup-0.73.0/lamindb_setup/_cache.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_check_setup.py` & `lamindb_setup-0.73.0/lamindb_setup/_check_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_close.py` & `lamindb_setup-0.73.0/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_connect_instance.py` & `lamindb_setup-0.73.0/lamindb_setup/_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_delete.py` & `lamindb_setup-0.73.0/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_django.py` & `lamindb_setup-0.73.0/lamindb_setup/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_exportdb.py` & `lamindb_setup-0.73.0/lamindb_setup/_exportdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_importdb.py` & `lamindb_setup-0.73.0/lamindb_setup/_importdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_init_instance.py` & `lamindb_setup-0.73.0/lamindb_setup/_init_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     # the managing instance?
     defaults = {
         "root": ssettings.root_as_str,
         "type": ssettings.type,
         "region": ssettings.region,
         "instance_uid": instance_uid,
         "created_by_id": current_user_id(),
+        "run": None,
     }
     if ssettings._uid is not None:
         defaults["uid"] = ssettings._uid
     storage, _ = Storage.objects.update_or_create(
         root=ssettings.root_as_str,
         defaults=defaults,
     )
```

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_migrate.py` & `lamindb_setup-0.73.0/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_register_instance.py` & `lamindb_setup-0.73.0/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_schema.py` & `lamindb_setup-0.73.0/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_set_managed_storage.py` & `lamindb_setup-0.73.0/lamindb_setup/_set_managed_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_setup_user.py` & `lamindb_setup-0.73.0/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.73.0/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_aws_credentials.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_aws_credentials.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_aws_storage.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_aws_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_deprecated.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_hub_client.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_hub_core.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_hub_core.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_hub_crud.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_hub_utils.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_settings.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_settings_instance.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_settings_load.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_settings_save.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_settings_storage.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_settings_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,41 +33,44 @@
 def base62(n_char: int) -> str:
     """Like nanoid without hyphen and underscore."""
     alphabet = string.digits + string.ascii_letters.swapcase()
     id = "".join(secrets.choice(alphabet) for i in range(n_char))
     return id
 
 
-def get_storage_region(storage_root: UPathStr) -> str | None:
-    storage_root_str = str(storage_root)
-    if storage_root_str.startswith("s3://"):
-        import botocore.session as session
+def get_storage_region(path: UPathStr) -> str | None:
+    path_str = str(path)
+    if path_str.startswith("s3://"):
+        import botocore.session
         from botocore.config import Config
-        from botocore.exceptions import NoCredentialsError
+        from botocore.exceptions import ClientError
 
         # strip the prefix and any suffixes of the bucket name
-        bucket = storage_root_str.replace("s3://", "").split("/")[0]
-        s3_session = session.get_session()
-        s3_client = s3_session.create_client("s3")
+        bucket = path_str.replace("s3://", "").split("/")[0]
+        session = botocore.session.get_session()
+        credentials = session.get_credentials()
+        if credentials is None or credentials.access_key is None:
+            config = Config(signature_version=botocore.session.UNSIGNED)
+        else:
+            config = None
+        s3_client = session.create_client("s3", config=config)
         try:
             response = s3_client.head_bucket(Bucket=bucket)
-        except NoCredentialsError:  # deal with anonymous access
-            s3_client = s3_session.create_client(
-                "s3", config=Config(signature_version=session.UNSIGNED)
-            )
-            response = s3_client.head_bucket(Bucket=bucket)
-        storage_region = response["ResponseMetadata"].get("HTTPHeaders", {})[
-            "x-amz-bucket-region"
-        ]
-        # if we want to except botcore.exceptions.ClientError to reformat an
-        # error message, this is how to do test for the "NoSuchBucket" error:
-        #     exc.response["Error"]["Code"] == "NoSuchBucket"
+        except ClientError as exc:
+            response = getattr(exc, "response", {})
+            if response.get("Error", {}).get("Code") == "404":
+                raise exc
+        region = (
+            response.get("ResponseMetadata", {})
+            .get("HTTPHeaders", {})
+            .get("x-amz-bucket-region")
+        )
     else:
-        storage_region = None
-    return storage_region
+        region = None
+    return region
 
 
 def mark_storage_root(root: UPathStr, uid: str):
     # we need to touch a 0-byte object in folder-like storage location on S3 to avoid
     # permission errors from leveraging s3fs on an empty hosted storage location
     # for consistency, we write this file everywhere
     root_upath = convert_pathlike(root)
```

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_settings_store.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_settings_user.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/_setup_bionty_sources.py` & `lamindb_setup-0.73.0/lamindb_setup/core/_setup_bionty_sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
         # when the database is not yet migrated but setup is updated
         # won't need this once lamindb is released with the new pin
         if hasattr(PublicSource, "species") and "organism" in kwargs:
             kwargs["species"] = kwargs.pop("organism")
         elif hasattr(PublicSource, "organism") and "species" in kwargs:
             kwargs["organism"] = kwargs.pop("species")
+        kwargs["run"] = None  # can't yet access tracking information
         record = PublicSource(**kwargs)
         all_records.append(record)
 
     PublicSource.objects.bulk_create(all_records, ignore_conflicts=True)
 
 
 def load_bionty_sources(isettings: InstanceSettings):
```

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/cloud_sqlite_locker.py` & `lamindb_setup-0.73.0/lamindb_setup/core/cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/django.py` & `lamindb_setup-0.73.0/lamindb_setup/core/django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/hashing.py` & `lamindb_setup-0.73.0/lamindb_setup/core/hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/types.py` & `lamindb_setup-0.73.0/lamindb_setup/core/types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/lamindb_setup/core/upath.py` & `lamindb_setup-0.73.0/lamindb_setup/core/upath.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,15 +151,18 @@
     else:
         return fsspec.FSMap(
             url, fs, check=check, create=create, missing_exceptions=missing_exceptions
         )
 
 
 def print_hook(size: int, value: int, objectname: str, action: str):
-    progress_in_percent = (value / size) * 100
+    if size == 0:
+        progress_in_percent = 100.0
+    else:
+        progress_in_percent = (value / size) * 100
     out = f"... {action} {objectname}:" f" {min(progress_in_percent, 100):4.1f}%"
     if "NBPRJ_TEST_NBPATH" not in os.environ:
         end = "\n" if progress_in_percent >= 100 else "\r"
         print(out, end=end)
 
 
 class ProgressCallback(fsspec.callbacks.Callback):
@@ -234,89 +237,123 @@
 
         self.parent = parent
 
     def parent_update(self, inc=1):
         self.parent.update_relative_value(inc)
 
     def relative_update(self, inc=1):
-        self.parent_update(inc / self.size)
+        if self.size != 0:
+            self.parent_update(inc / self.size)
+        else:
+            self.parent_update(1)
 
 
-def download_to(self, path: UPathStr, print_progress: bool = False, **kwargs):
-    """Download to a path."""
+def download_to(self, local_path: UPathStr, print_progress: bool = True, **kwargs):
+    """Download from self (a destination in the cloud) to the local path."""
+    if "recursive" not in kwargs:
+        kwargs["recursive"] = True
     if print_progress and "callback" not in kwargs:
         callback = ProgressCallback(
-            PurePosixPath(path).name, "downloading", adjust_size=True
+            PurePosixPath(local_path).name, "downloading", adjust_size=True
         )
         kwargs["callback"] = callback
 
-    self.fs.download(str(self), str(path), **kwargs)
+    self.fs.download(str(self), str(local_path), **kwargs)
 
 
 def upload_from(
     self,
-    path: UPathStr,
-    dir_inplace: bool = False,
-    print_progress: bool = False,
+    local_path: UPathStr,
+    create_folder: bool | None = None,
+    print_progress: bool = True,
     **kwargs,
-):
-    """Upload from a local path."""
-    path = Path(path)
-    path_is_dir = path.is_dir()
-    if not path_is_dir:
-        dir_inplace = False
+) -> UPath:
+    """Upload from the local path to `self` (a destination in the cloud).
+
+    If the local path is a directory, recursively upload its contents.
+
+    Args:
+        local_path: A local path of a file or directory.
+        create_folder: Only applies if `local_path` is a directory and then
+            defaults to `True`. If `True`, make a new folder in the destination
+            using the directory name of `local_path`. If `False`, upload the
+            contents of the directory to to the root-level of the destination.
+        print_progress: Print progress.
+
+    Returns:
+        The destination path.
+    """
+    local_path = Path(local_path)
+    local_path_is_dir = local_path.is_dir()
+    if create_folder is None:
+        create_folder = local_path_is_dir
+    if create_folder and not local_path_is_dir:
+        raise ValueError("create_folder can only be True if local_path is a directory")
 
     if print_progress and "callback" not in kwargs:
-        callback = ProgressCallback(path.name, "uploading")
+        callback = ProgressCallback(local_path.name, "uploading")
         kwargs["callback"] = callback
 
-    if dir_inplace:
-        source = [f for f in path.rglob("*") if f.is_file()]
-        destination = [str(self / f.relative_to(path)) for f in source]
+    if local_path_is_dir and not create_folder:
+        source = [f for f in local_path.rglob("*") if f.is_file()]
+        # convert_pathlike is needed to remove the trailing slash because
+        # UPath("s3://some-bucket/some-folder/") / "some-key"
+        # results in UPath("s3://some-bucket/some-folder//some-key")
+        # for upath 0.1.4
+        dest_root = convert_pathlike(self) if self._parts[-1] == "" else self
+        destination = [str(dest_root / f.relative_to(local_path)) for f in source]
         source = [str(f) for f in source]  # type: ignore
     else:
-        source = str(path)  # type: ignore
+        source = str(local_path)  # type: ignore
         destination = str(self)  # type: ignore
-    # this weird thing is to avoid s3fs triggering create_bucket in upload
-    # if dirs are present
-    # it allows to avoid permission error
-    if self.protocol != "s3" or not path_is_dir or dir_inplace:
-        cleanup_cache = False
-    else:
+
+    # the below lines are to avoid s3fs triggering create_bucket in upload if
+    # dirs are present it allows to avoid permission error
+    # would be easier to just
+    if self.protocol == "s3" and local_path_is_dir and create_folder:
         bucket = self._url.netloc
         if bucket not in self.fs.dircache:
             self.fs.dircache[bucket] = [{}]
             if not destination.endswith(TRAILING_SEP):  # type: ignore
                 destination += "/"
             cleanup_cache = True
         else:
             cleanup_cache = False
+    else:
+        cleanup_cache = False
 
-    self.fs.upload(source, destination, **kwargs)
+    self.fs.upload(source, destination, recursive=create_folder, **kwargs)
 
     if cleanup_cache:
         # normally this is invalidated after the upload but still better to check
         if bucket in self.fs.dircache:
             del self.fs.dircache[bucket]
 
+    if local_path_is_dir and create_folder:
+        # convert_pathlike is needed to remove the trailing slash
+        dest_root = convert_pathlike(self) if self._parts[-1] == "" else self
+        return dest_root / local_path.name
+    else:
+        return self
+
 
 def synchronize(
     self,
     objectpath: Path,
     error_no_origin: bool = True,
     print_progress: bool = False,
     callback: fsspec.callbacks.Callback | None = None,
-    **kwargs,
+    timestamp: float | None = None,
 ):
     """Sync to a local destination path."""
     # optimize the number of network requests
-    if "timestamp" in kwargs:
+    if timestamp is not None:
         is_dir = False
         exists = True
-        cloud_mts = kwargs.pop("timestamp")
+        cloud_mts = timestamp
     else:
         # perform only one network request to check existence, type and timestamp
         try:
             cloud_mts = self.modified.timestamp()
             is_dir = False
             exists = True
         except FileNotFoundError:
@@ -375,15 +412,15 @@
                 origin_file_keys.append(file_key.as_posix())
                 timestamp = stat[modified_key].timestamp()
 
                 origin = f"{self.protocol}://{file}"
                 destination = objectpath / file_key
                 child = callback.branched(origin, destination.as_posix())
                 UPath(origin, **self._kwargs).synchronize(
-                    destination, timestamp=timestamp, callback=child, **kwargs
+                    destination, callback=child, timestamp=timestamp
                 )
                 child.close()
             if destination_exists:
                 local_files = [file for file in objectpath.rglob("*") if file.is_file()]
                 if len(local_files) > len(files):
                     for file in local_files:
                         if (
@@ -396,23 +433,24 @@
                                 parent.rmdir()
         return None
 
     # synchronization logic for files
     callback = ProgressCallback.requires_progress(
         callback, print_progress, objectpath.name, "synchronizing"
     )
-    kwargs["callback"] = callback
     if objectpath.exists():
-        local_mts = objectpath.stat().st_mtime  # type: ignore
-        need_synchronize = cloud_mts > local_mts
+        local_mts_obj = objectpath.stat().st_mtime  # type: ignore
+        need_synchronize = cloud_mts > local_mts_obj
     else:
         objectpath.parent.mkdir(parents=True, exist_ok=True)
         need_synchronize = True
     if need_synchronize:
-        self.download_to(objectpath, **kwargs)
+        self.download_to(
+            objectpath, recursive=False, print_progress=False, callback=callback
+        )
         os.utime(objectpath, times=(cloud_mts, cloud_mts))
     else:
         # nothing happens if parent_update is not defined
         # because of Callback.no_op
         callback.parent_update()
 
 
@@ -473,15 +511,15 @@
         pointers = [tee] * (len(contents) - 1) + [last]
         n_files_per_dir_and_type = defaultdict(lambda: 0)  # type: ignore
         # TODO: pass strict=False to zip with python > 3.9
         for pointer, child_path in zip(pointers, contents):  # type: ignore
             if child_path.is_dir():
                 if include_dirs and child_path not in include_dirs:
                     continue
-                yield prefix + pointer + child_path.name
+                yield prefix + pointer + child_path.name + "/"
                 n_directories += 1
                 n_files_per_dir_and_type = defaultdict(lambda: 0)
                 extension = branch if pointer == tee else space
                 yield from inner(child_path, prefix=prefix + extension, level=level - 1)
             elif not only_dirs:
                 if include_paths and child_path not in include_paths:
                     continue
```

### Comparing `lamindb_setup-0.72.2/noxfile.py` & `lamindb_setup-0.73.0/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         cmds = (
             cloud_prod_installs
             + "uv pip install --system --no-deps git+https://github.com/laminlabs/wetlab"
         )
     elif group == "hub-local":
         cmds = """uv pip install --system -e ./laminhub/rest-hub"""
     # current package
-    cmds += """\nuv pip install --system .[aws,dev] lamin-cli"""
+    cmds += """\nuv pip install --system -e '.[aws,dev]' lamin-cli"""
 
     [run(session, line) for line in cmds.splitlines()]
 
 
 @nox.session
 @nox.parametrize(
     "group",
```

### Comparing `lamindb_setup-0.72.2/pyproject.toml` & `lamindb_setup-0.73.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/tests/hub-cloud/test_connect_instance.py` & `lamindb_setup-0.73.0/tests/hub-cloud/test_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/tests/hub-cloud/test_init_instance.py` & `lamindb_setup-0.73.0/tests/hub-cloud/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/tests/hub-cloud/test_login.py` & `lamindb_setup-0.73.0/tests/hub-cloud/test_login.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/tests/hub-local/conftest.py` & `lamindb_setup-0.73.0/tests/hub-local/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/tests/hub-local/test_all.py` & `lamindb_setup-0.73.0/tests/hub-local/test_all.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/tests/hub-prod/conftest.py` & `lamindb_setup-0.73.0/tests/hub-prod/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/tests/hub-prod/test_switch_and_fallback_env.py` & `lamindb_setup-0.73.0/tests/hub-prod/test_switch_and_fallback_env.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/tests/hub-prod/test_upath.py` & `lamindb_setup-0.73.0/tests/hub-prod/test_upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/tests/storage/test_hashing.py` & `lamindb_setup-0.73.0/tests/storage/test_hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/tests/storage/test_storage_access.py` & `lamindb_setup-0.73.0/tests/storage/test_storage_access.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/tests/storage/test_storage_basis.py` & `lamindb_setup-0.73.0/tests/storage/test_storage_basis.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/tests/storage/test_storage_stats.py` & `lamindb_setup-0.73.0/tests/storage/test_storage_stats.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 from __future__ import annotations
 
+from lamindb_setup.core._aws_credentials import HOSTED_REGIONS
+from lamindb_setup.core._settings_storage import get_storage_region
 from lamindb_setup.core.upath import UPath, compute_file_tree, get_stat_dir_cloud
 
 
 def test_get_stat_dir_cloud_aws():
-    string_path = "s3://lamindb-dev-datasets/iris_studies/study0_raw_images"
+    string_path = "s3://lamindata/iris_studies/study0_raw_images"
     path = UPath(string_path, anon=True)
     _, n_objects_file_tree = compute_file_tree(path)
     size, hash, hash_type, n_objects = get_stat_dir_cloud(path)
     assert n_objects == n_objects_file_tree
-    assert hash == "wVYKPpEsmmrqSpAZIRXCFg"
+    assert hash == "IVKGMfNwi8zKvnpaD_gG7w"
     assert hash_type == "md5-d"
-    assert size == 656692
+    assert size == 658465
+    assert n_objects == 51
 
 
 def test_get_stat_dir_cloud_gcp():
     string_path = "gs://rxrx1-europe-west4/images/test/HEPG2-08"
     path = UPath(string_path, anon=True)
     size, hash, hash_type, n_objects = get_stat_dir_cloud(path)
     assert n_objects == 14772
     assert hash == "6r5Hkce0UTy7X6gLeaqzBA"
     assert hash_type == "md5-d"
     assert size == 994441606
+
+
+def test_get_storage_region():
+    for region in HOSTED_REGIONS:
+        assert get_storage_region(f"s3://lamin-{region}") == region
```

### Comparing `lamindb_setup-0.72.2/tests/storage/test_to_url.py` & `lamindb_setup-0.73.0/tests/storage/test_to_url.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.72.2/PKG-INFO` & `lamindb_setup-0.73.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.72.2
+Version: 0.73.0
 Summary: Setup & configure LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.51.0
 Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django>4.2,<5.2.0
 Requires-Dist: dj_database_url>=1.3.0,<3.0.0
```

