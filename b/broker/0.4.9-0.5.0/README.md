# Comparing `tmp/broker-0.4.9.tar.gz` & `tmp/broker-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "broker-0.4.9.tar", last modified: Tue Mar 19 15:52:07 2024, max compression
+gzip compressed data, was "broker-0.5.0.tar", last modified: Wed May 29 13:47:36 2024, max compression
```

## Comparing `broker-0.4.9.tar` & `broker-0.5.0.tar`

### file list

```diff
@@ -1,94 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.918284 broker-0.4.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.906284 broker-0.4.9/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-19 15:52:00.000000 broker-0.4.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.906284 broker-0.4.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-19 15:52:00.000000 broker-0.4.9/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-19 15:52:00.000000 broker-0.4.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-19 15:52:00.000000 broker-0.4.9/.github/workflows/update_broker_image.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-19 15:52:00.000000 broker-0.4.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-19 15:52:00.000000 broker-0.4.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-19 15:52:00.000000 broker-0.4.9/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-03-19 15:52:00.000000 broker-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    47529 2024-03-19 15:52:07.918284 broker-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-03-19 15:52:01.000000 broker-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.910284 broker-0.4.9/broker/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-19 15:52:01.000000 broker-0.4.9/broker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.910284 broker-0.4.9/broker/binds/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-19 15:52:01.000000 broker-0.4.9/broker/binds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-03-19 15:52:01.000000 broker-0.4.9/broker/binds/beaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-03-19 15:52:01.000000 broker-0.4.9/broker/binds/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17619 2024-03-19 15:52:01.000000 broker-0.4.9/broker/broker.py
--rw-r--r--   0 runner    (1001) docker     (127)    14464 2024-03-19 15:52:01.000000 broker-0.4.9/broker/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-19 15:52:01.000000 broker-0.4.9/broker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19516 2024-03-19 15:52:01.000000 broker-0.4.9/broker/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8448 2024-03-19 15:52:01.000000 broker-0.4.9/broker/hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-03-19 15:52:01.000000 broker-0.4.9/broker/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.910284 broker-0.4.9/broker/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-03-19 15:52:01.000000 broker-0.4.9/broker/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32290 2024-03-19 15:52:01.000000 broker-0.4.9/broker/providers/ansible_tower.py
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-03-19 15:52:01.000000 broker-0.4.9/broker/providers/beaker.py
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-03-19 15:52:01.000000 broker-0.4.9/broker/providers/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-03-19 15:52:01.000000 broker-0.4.9/broker/providers/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    16800 2024-03-19 15:52:01.000000 broker-0.4.9/broker/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-03-19 15:52:01.000000 broker-0.4.9/broker/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.918284 broker-0.4.9/broker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    47529 2024-03-19 15:52:07.000000 broker-0.4.9/broker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-19 15:52:07.000000 broker-0.4.9/broker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 15:52:07.000000 broker-0.4.9/broker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-19 15:52:07.000000 broker-0.4.9/broker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 15:52:03.000000 broker-0.4.9/broker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-19 15:52:07.000000 broker-0.4.9/broker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-19 15:52:07.000000 broker-0.4.9/broker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-19 15:52:01.000000 broker-0.4.9/broker_settings.yaml.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.902284 broker-0.4.9/catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.910284 broker-0.4.9/catalog/system/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-19 15:52:01.000000 broker-0.4.9/catalog/system/broker.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-19 15:52:01.000000 broker-0.4.9/catalog-info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.910284 broker-0.4.9/logs/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-19 15:52:01.000000 broker-0.4.9/logs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-03-19 15:52:01.000000 broker-0.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 15:52:07.918284 broker-0.4.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.914284 broker-0.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-19 15:52:01.000000 broker-0.4.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.914284 broker-0.4.9/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.914284 broker-0.4.9/tests/data/ansible_tower/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/ansible_tower/fake_children.json
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/ansible_tower/fake_jobs.json
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/ansible_tower/fake_workflows.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/args_file.json
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/args_file.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.914284 broker-0.4.9/tests/data/beaker/
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/beaker/job_result.json
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/beaker/test_job.xml
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/broker_args.json
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/broker_args.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.906284 broker-0.4.9/tests/data/cli_scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.914284 broker-0.4.9/tests/data/cli_scenarios/beaker/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/cli_scenarios/beaker/checkout_test_job-2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/cli_scenarios/beaker/checkout_test_job.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.914284 broker-0.4.9/tests/data/cli_scenarios/containers/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8_2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/cli_scenarios/containers/execute_ch-d_ubi8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.914284 broker-0.4.9/tests/data/cli_scenarios/satlab/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/cli_scenarios/satlab/checkout_latest_rhel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/cli_scenarios/satlab/checkout_latest_sat.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/cli_scenarios/satlab/checkout_rhel91.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/cli_scenarios/satlab/checkout_sat_611.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/cli_scenarios/satlab/execute_templates_list.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.914284 broker-0.4.9/tests/data/container/
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/container/fake_containers.json
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/container/fake_images.json
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-03-19 15:52:01.000000 broker-0.4.9/tests/data/fake_inventory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.918284 broker-0.4.9/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-19 15:52:01.000000 broker-0.4.9/tests/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-03-19 15:52:01.000000 broker-0.4.9/tests/functional/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-03-19 15:52:01.000000 broker-0.4.9/tests/functional/test_rh_beaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-03-19 15:52:01.000000 broker-0.4.9/tests/functional/test_satlab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:52:07.918284 broker-0.4.9/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-03-19 15:52:01.000000 broker-0.4.9/tests/providers/test_ansible_tower.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-03-19 15:52:01.000000 broker-0.4.9/tests/providers/test_beaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-03-19 15:52:01.000000 broker-0.4.9/tests/providers/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-03-19 15:52:01.000000 broker-0.4.9/tests/test_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-03-19 15:52:01.000000 broker-0.4.9/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-19 15:52:01.000000 broker-0.4.9/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.880837 broker-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.864837 broker-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-29 13:47:29.000000 broker-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.864837 broker-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-29 13:47:29.000000 broker-0.5.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 13:47:29.000000 broker-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-29 13:47:29.000000 broker-0.5.0/.github/workflows/update_broker_image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-29 13:47:29.000000 broker-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-29 13:47:29.000000 broker-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-29 13:47:29.000000 broker-0.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-05-29 13:47:29.000000 broker-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    47837 2024-05-29 13:47:36.880837 broker-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-29 13:47:29.000000 broker-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.868836 broker-0.5.0/broker/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 13:47:29.000000 broker-0.5.0/broker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.868836 broker-0.5.0/broker/binds/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-29 13:47:29.000000 broker-0.5.0/broker/binds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-05-29 13:47:29.000000 broker-0.5.0/broker/binds/beaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-29 13:47:29.000000 broker-0.5.0/broker/binds/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-05-29 13:47:29.000000 broker-0.5.0/broker/binds/foreman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-29 13:47:29.000000 broker-0.5.0/broker/binds/hussh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-05-29 13:47:29.000000 broker-0.5.0/broker/binds/pylibssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-29 13:47:29.000000 broker-0.5.0/broker/binds/ssh2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-29 13:47:29.000000 broker-0.5.0/broker/binds/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-05-29 13:47:29.000000 broker-0.5.0/broker/broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-29 13:47:29.000000 broker-0.5.0/broker/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-29 13:47:29.000000 broker-0.5.0/broker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19885 2024-05-29 13:47:29.000000 broker-0.5.0/broker/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-29 13:47:29.000000 broker-0.5.0/broker/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-29 13:47:29.000000 broker-0.5.0/broker/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.872837 broker-0.5.0/broker/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-05-29 13:47:29.000000 broker-0.5.0/broker/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33754 2024-05-29 13:47:29.000000 broker-0.5.0/broker/providers/ansible_tower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-05-29 13:47:29.000000 broker-0.5.0/broker/providers/beaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12342 2024-05-29 13:47:29.000000 broker-0.5.0/broker/providers/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-05-29 13:47:29.000000 broker-0.5.0/broker/providers/foreman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-29 13:47:29.000000 broker-0.5.0/broker/providers/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-29 13:47:29.000000 broker-0.5.0/broker/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-29 13:47:29.000000 broker-0.5.0/broker/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.880837 broker-0.5.0/broker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    47837 2024-05-29 13:47:36.000000 broker-0.5.0/broker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-29 13:47:36.000000 broker-0.5.0/broker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:47:36.000000 broker-0.5.0/broker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-29 13:47:36.000000 broker-0.5.0/broker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:47:32.000000 broker-0.5.0/broker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-29 13:47:36.000000 broker-0.5.0/broker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 13:47:36.000000 broker-0.5.0/broker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-29 13:47:29.000000 broker-0.5.0/broker_settings.yaml.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.860837 broker-0.5.0/catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.872837 broker-0.5.0/catalog/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-29 13:47:29.000000 broker-0.5.0/catalog/system/broker.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-29 13:47:29.000000 broker-0.5.0/catalog-info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.872837 broker-0.5.0/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-29 13:47:29.000000 broker-0.5.0/logs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-05-29 13:47:29.000000 broker-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:47:36.880837 broker-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.872837 broker-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-29 13:47:29.000000 broker-0.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.872837 broker-0.5.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.872837 broker-0.5.0/tests/data/ansible_tower/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/ansible_tower/fake_children.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/ansible_tower/fake_jobs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/ansible_tower/fake_workflows.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/args_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/args_file.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.872837 broker-0.5.0/tests/data/beaker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/beaker/job_result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/beaker/test_job.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/broker_args.json
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/broker_args.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.864837 broker-0.5.0/tests/data/cli_scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.872837 broker-0.5.0/tests/data/cli_scenarios/beaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/cli_scenarios/beaker/checkout_test_job-2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/cli_scenarios/beaker/checkout_test_job.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.872837 broker-0.5.0/tests/data/cli_scenarios/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/cli_scenarios/containers/execute_ch-d_ubi8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.876837 broker-0.5.0/tests/data/cli_scenarios/satlab/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/cli_scenarios/satlab/checkout_latest_rhel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/cli_scenarios/satlab/checkout_latest_sat.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/cli_scenarios/satlab/checkout_rhel91.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/cli_scenarios/satlab/checkout_sat_613.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/cli_scenarios/satlab/execute_templates_list.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.876837 broker-0.5.0/tests/data/container/
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/container/fake_containers.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/container/fake_images.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/fake_inventory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.876837 broker-0.5.0/tests/data/foreman/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/foreman/fake_get.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/foreman/fake_hosts.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/foreman/fake_jobs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-29 13:47:29.000000 broker-0.5.0/tests/data/foreman/fake_resources.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.876837 broker-0.5.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-29 13:47:29.000000 broker-0.5.0/tests/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-05-29 13:47:29.000000 broker-0.5.0/tests/functional/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-29 13:47:29.000000 broker-0.5.0/tests/functional/test_rh_beaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-29 13:47:29.000000 broker-0.5.0/tests/functional/test_satlab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:47:36.876837 broker-0.5.0/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-29 13:47:29.000000 broker-0.5.0/tests/providers/test_ansible_tower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-29 13:47:29.000000 broker-0.5.0/tests/providers/test_beaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-29 13:47:29.000000 broker-0.5.0/tests/providers/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-29 13:47:29.000000 broker-0.5.0/tests/providers/test_foreman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-29 13:47:29.000000 broker-0.5.0/tests/test_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-29 13:47:29.000000 broker-0.5.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-29 13:47:29.000000 broker-0.5.0/tests/test_settings.py
```

### Comparing `broker-0.4.9/.github/workflows/codeql-analysis.yml` & `broker-0.5.0/.github/workflows/codeql-analysis.yml`

 * *Files 11% similar despite different names*

```diff
@@ -45,12 +45,13 @@
       - name: Setup Temp Directory
         run: mkdir broker_dir
 
       - name: Unit Tests
         env:
           BROKER_DIRECTORY: "${{ github.workspace }}/broker_dir"
         run: |
+          cp broker_settings.yaml.example ${BROKER_DIRECTORY}/broker_settings.yaml
           pip install uv
           uv pip install --system "broker[dev,docker] @ ."
           ls -l "$BROKER_DIRECTORY"
           broker --version
           pytest -v tests/ --ignore tests/functional
```

### Comparing `broker-0.4.9/.github/workflows/python-publish.yml` & `broker-0.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/.github/workflows/update_broker_image.yml` & `broker-0.5.0/.github/workflows/update_broker_image.yml`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/.gitignore` & `broker-0.5.0/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -94,7 +94,8 @@
 # pytest
 .pytest_cache/
 
 # project
 *settings.yaml
 inventory.yaml
 *.bak
+/bin/*
```

### Comparing `broker-0.4.9/LICENSE` & `broker-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/PKG-INFO` & `broker-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broker
-Version: 0.4.9
+Version: 0.5.0
 Summary: The infrastructure middleman.
 Author-email: Jacob J Callahan <jacob.callahan05@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -706,20 +706,28 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Provides-Extra: docker
 Requires-Dist: docker; extra == "docker"
 Requires-Dist: paramiko; extra == "docker"
 Provides-Extra: podman
-Requires-Dist: podman-py; extra == "podman"
+Requires-Dist: podman; extra == "podman"
 Provides-Extra: setup
 Requires-Dist: build; extra == "setup"
 Requires-Dist: twine; extra == "setup"
 Provides-Extra: ssh2-py311
 Requires-Dist: ssh2-python; extra == "ssh2-py311"
+Provides-Extra: ssh2-python
+Requires-Dist: ssh2-python; extra == "ssh2-python"
+Provides-Extra: ssh2-python312
+Requires-Dist: ssh2-python312; extra == "ssh2-python312"
+Provides-Extra: ansible-pylibssh
+Requires-Dist: ansible-pylibssh; extra == "ansible-pylibssh"
+Provides-Extra: hussh
+Requires-Dist: hussh; extra == "hussh"
 
 [![PythonPackage](https://github.com/SatelliteQE/broker/actions/workflows/python-publish.yml/badge.svg)](https://github.com/SatelliteQE/broker/actions/workflows/python-publish.yml)
 [![ContainerImage](https://github.com/SatelliteQE/broker/actions/workflows/update_broker_image.yml/badge.svg)](https://github.com/SatelliteQE/broker/actions/workflows/update_broker_image.yml)
 [![CodeQL](https://github.com/SatelliteQE/broker/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/SatelliteQE/broker/actions/workflows/codeql-analysis.yml)
 # Broker
 The infrastrucure middleman
 
@@ -831,14 +839,14 @@
 ```
 broker --output-file output.json checkout --nick rhel7
 broker --output-file inventory.json inventory
 ```
 
 **Run Broker in the background**
 
-Certain Broker actions can be run in the background, these currently are: checkout, checkin, duplicate, and execute. When running a command in this mode, it will spin up a new Broker process and no longer log to stderr. To check progress, you can still follow broker's log file.
+Certain Broker actions can be run in the background, these currently are: checkout, checkin, and execute. When running a command in this mode, it will spin up a new Broker process and no longer log to stderr. To check progress, you can still follow broker's log file.
 Note that background mode will interfere with output options for execute since it won't be able to print to stdout. Those should kept in log mode.
 ```
 broker checkout --background --nick rhel7
 broker checkin -b --all
 broker execute -b --workflow my-awesome-workflow --artifacts
 ```
```

### Comparing `broker-0.4.9/README.md` & `broker-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,14 @@
 ```
 broker --output-file output.json checkout --nick rhel7
 broker --output-file inventory.json inventory
 ```
 
 **Run Broker in the background**
 
-Certain Broker actions can be run in the background, these currently are: checkout, checkin, duplicate, and execute. When running a command in this mode, it will spin up a new Broker process and no longer log to stderr. To check progress, you can still follow broker's log file.
+Certain Broker actions can be run in the background, these currently are: checkout, checkin, and execute. When running a command in this mode, it will spin up a new Broker process and no longer log to stderr. To check progress, you can still follow broker's log file.
 Note that background mode will interfere with output options for execute since it won't be able to print to stdout. Those should kept in log mode.
 ```
 broker checkout --background --nick rhel7
 broker checkin -b --all
 broker execute -b --workflow my-awesome-workflow --artifacts
 ```
```

### Comparing `broker-0.4.9/broker/binds/beaker.py` & `broker-0.5.0/broker/binds/beaker.py`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/broker/binds/containers.py` & `broker-0.5.0/broker/binds/containers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,56 @@
 """A collection of classes to ease interaction with Docker and Podman libraries."""
 
+HEADER_SIZE = 8
+STDOUT = 1
+STDERR = 2
+
+
+def demux_output(data_bytes):
+    """Demuxes the output of a container stream into stdout and stderr streams.
+
+    Stream data is expected to be in the following format:
+    - 1 byte: stream type (1=stdout, 2=stderr)
+    - 3 bytes: padding
+    - 4 bytes: payload size (big-endian)
+    - N bytes: payload data
+    ref: https://docs.podman.io/en/latest/_static/api.html?version=v5.0#tag/containers/operation/ContainerAttachLibpod
+
+    Args:
+        data_bytes: Bytes object containing the combined stream data.
+
+    Returns:
+        A tuple containing two bytes objects: (stdout, stderr).
+    """
+    stdout = b""
+    stderr = b""
+    while len(data_bytes) >= HEADER_SIZE:
+        # Extract header information
+        header, data_bytes = data_bytes[:HEADER_SIZE], data_bytes[HEADER_SIZE:]
+        stream_type = header[0]
+        payload_size = int.from_bytes(header[4:HEADER_SIZE], "big")
+        # Check if data is sufficient for payload
+        if len(data_bytes) < payload_size:
+            break  # Incomplete frame, wait for more data
+
+        # Extract and process payload
+        payload = data_bytes[:payload_size]
+        if stream_type == STDOUT:
+            stdout += payload
+        elif stream_type == STDERR:
+            stderr += payload
+        else:
+            # todo: Handle unexpected stream types
+            pass
+
+        # Update data for next frame
+        data_bytes = data_bytes[payload_size:]
+
+    return stdout, stderr
+
 
 class ContainerBind:
     """A base class that provides common functionality for Docker and Podman containers."""
 
     _sensitive_attrs = ["password", "host_password"]
 
     def __init__(self, host=None, username=None, password=None, port=22, timeout=None):
```

### Comparing `broker-0.4.9/broker/broker.py` & `broker-0.5.0/broker/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,20 +78,21 @@
         return mp_split
 
 
 class Broker:
     """Main Broker class to be used as the primary interface for the Broker API."""
 
     # map exceptions for easier access when used as a library
-    BrokerError = exceptions.BrokerError
     AuthenticationError = exceptions.AuthenticationError
-    PermissionError = exceptions.PermissionError
-    ProviderError = exceptions.ProviderError
+    BrokerError = exceptions.BrokerError
     ConfigurationError = exceptions.ConfigurationError
     NotImplementedError = exceptions.NotImplementedError
+    PermissionError = exceptions.PermissionError
+    ProviderError = exceptions.ProviderError
+    UserError = exceptions.UserError
 
     def __init__(self, **kwargs):
         kwargs = helpers.resolve_file_args(kwargs)
         logger.debug(f"Broker instantiated with {kwargs=}")
         self._hosts = kwargs.pop("hosts", [])
         self.host_classes = {"host": Host}
         # if a nick was specified, pull in the resolved arguments
```

### Comparing `broker-0.4.9/broker/commands.py` & `broker-0.5.0/broker/commands.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,22 @@
             return retval
 
         return wrapper
 
     return decorator
 
 
+def parse_labels(provider_labels):
+    """Parse the provided label string and returns labels in a dict."""
+    return {
+        label[0]: "=".join(label[1:])
+        for label in [kv_pair.split("=") for kv_pair in provider_labels.split(",")]
+    }
+
+
 class ExceptionHandler(click.Group):
     """Wraps click group to catch and handle raised exceptions."""
 
     def __call__(self, *args, **kwargs):
         """Override the __call__ method to catch and handle exceptions."""
         try:
             res = self.main(*args, **kwargs)
@@ -152,20 +160,22 @@
     "--version",
     is_flag=True,
     help="Get broker system-level information",
 )
 def cli(version):
     """Command-line interface for interacting with providers."""
     if version:
+        from importlib.metadata import version
+
         from packaging.version import Version
-        import pkg_resources
         import requests
 
-        broker_version = pkg_resources.get_distribution("broker").version
-        # check the latest version publish to PyPi
+        broker_version = version("broker")
+
+        # Check against the latest version published to PyPi
         try:
             latest_version = Version(
                 requests.get("https://pypi.org/pypi/broker/json", timeout=60).json()["info"][
                     "version"
                 ]
             )
             if latest_version > Version(broker_version):
@@ -184,34 +194,45 @@
 
 
 @loggedcli(context_settings={"allow_extra_args": True, "ignore_unknown_options": True})
 @click.option("-b", "--background", is_flag=True, help="Run checkout in the background")
 @click.option("-n", "--nick", type=str, help="Use a nickname defined in your settings")
 @click.option("-c", "--count", type=int, help="Number of times broker repeats the checkout")
 @click.option(
+    "-l",
+    "--provider-labels",
+    type=str,
+    help="A string representing the list"
+    " of k=v pairs (comma-separated) to be used as provider resource"
+    " labels (e.g. '-l k1=v1,k2=v2,k3=v3=z4').",
+)
+@click.option(
     "--args-file",
     type=click.Path(exists=True),
     help="A json or yaml file mapping arguments to values",
 )
 @provider_options
 @click.pass_context
-def checkout(ctx, background, nick, count, args_file, **kwargs):
+def checkout(ctx, background, nick, count, args_file, provider_labels, **kwargs):
     """Checkout or "create" a Virtual Machine broker instance.
 
     COMMAND: broker checkout --workflow "workflow-name" --workflow_arg1 something
 
     COMMAND: broker checkout --nick "nickname"
     """
     broker_args = helpers.clean_dict(kwargs)
     if nick:
         broker_args["nick"] = nick
     if count:
         broker_args["_count"] = count
     if args_file:
         broker_args["args_file"] = args_file
+    if provider_labels:
+        broker_args["provider_labels"] = parse_labels(provider_labels)
+
     # if additional arguments were passed, include them in the broker args
     # strip leading -- characters
     broker_args.update(
         {
             (key[2:] if key.startswith("--") else key): val
             for key, val in zip(ctx.args[::2], ctx.args[1::2])
         }
@@ -285,14 +306,22 @@
 
 @loggedcli()
 @click.argument("vm", type=str, nargs=-1)
 @click.option("-b", "--background", is_flag=True, help="Run extend in the background")
 @click.option("--all", "all_", is_flag=True, help="Select all VMs")
 @click.option("--sequential", is_flag=True, help="Run extends sequentially")
 @click.option("--filter", type=str, help="Extend only what matches the specified filter")
+@click.option(
+    "-l",
+    "--provider-labels",
+    type=str,
+    help="A string representing the list"
+    " of k=v pairs (comma-separated) to be used as provider resource"
+    " labels (e.g. '-l k1=v1,k2=v2,k3=v3=z4').",
+)
 @provider_options
 def extend(vm, background, all_, sequential, filter, **kwargs):
     """Extend a host's lease time.
 
     COMMAND: broker extend <vm hostname>|<vm name>|<local id>|--all
     """
     broker_args = helpers.clean_dict(kwargs)
@@ -302,76 +331,54 @@
     to_extend = []
     for num, host in enumerate(inventory):
         if str(num) in vm or host["hostname"] in vm or host.get("name") in vm or all_:
             to_extend.append(Broker().reconstruct_host(host))
     Broker(hosts=to_extend, **broker_args).extend(sequential=sequential)
 
 
-@loggedcli()
-@click.argument("vm", type=str, nargs=-1)
-@click.option("-b", "--background", is_flag=True, help="Run duplicate in the background")
-@click.option("-c", "--count", type=int, help="Number of times broker repeats the duplicate")
-@click.option("--all", "all_", is_flag=True, help="Select all VMs")
-@click.option("--filter", type=str, help="Duplicate only what matches the specified filter")
-def duplicate(vm, background, count, all_, filter):
-    """Duplicate a broker-procured vm.
-
-    DEPRECATED! This will be removed in Broker 0.5. If you need this feature, please open an issue.
-
-    COMMAND: broker duplicate <vm hostname>|<local id>|all
-    """
-    logger.warning(
-        "Duplicate will be remove in Broker 0.5. If you need this feature, please open an issue."
-    )
-    if background:
-        helpers.fork_broker()
-    inventory = helpers.load_inventory(filter=filter)
-    for num, host in enumerate(inventory):
-        if str(num) in vm or host["hostname"] in vm or host.get("name") in vm or all_:
-            broker_args = host.get("_broker_args")
-            if broker_args:
-                if count:
-                    broker_args["_count"] = count
-                logger.info(f"Duplicating: {host['hostname']}")
-                broker_inst = Broker(**broker_args)
-                broker_inst.checkout()
-            else:
-                logger.warning(f"Unable to duplicate {host['hostname']}, no _broker_args found")
-
-
 @loggedcli(context_settings={"allow_extra_args": True, "ignore_unknown_options": True})
 @click.option("-b", "--background", is_flag=True, help="Run execute in the background")
 @click.option("--nick", type=str, help="Use a nickname defined in your settings")
 @click.option("--output-format", "-o", type=click.Choice(["log", "raw", "yaml"]), default="log")
 @click.option(
     "--artifacts",
     type=click.Choice(["merge", "last"]),
     help="AnsibleTower: return artifacts associated with the execution.",
 )
 @click.option(
     "--args-file",
     type=click.Path(exists=True),
     help="A json or yaml file mapping arguments to values",
 )
+@click.option(
+    "-l",
+    "--provider-labels",
+    type=str,
+    help="A string representing the list"
+    " of k=v pairs (comma-separated) to be used as provider resource"
+    " labels (e.g. '-l k1=v1,k2=v2,k3=v3=z4').",
+)
 @provider_options
 @click.pass_context
-def execute(ctx, background, nick, output_format, artifacts, args_file, **kwargs):
+def execute(ctx, background, nick, output_format, artifacts, args_file, provider_labels, **kwargs):
     """Execute an arbitrary provider action.
 
     COMMAND: broker execute --workflow "workflow-name" --workflow_arg1 something
 
     COMMAND: broker execute --nick "nickname"
     """
     broker_args = helpers.clean_dict(kwargs)
     if nick:
         broker_args["nick"] = nick
     if artifacts:
         broker_args["artifacts"] = artifacts
     if args_file:
         broker_args["args_file"] = args_file
+    if provider_labels:
+        broker_args["provider_labels"] = parse_labels(provider_labels)
     # if additional arguments were passed, include them in the broker args
     # strip leading -- characters
     broker_args.update(
         {
             (key[2:] if key.startswith("--") else key): val
             for key, val in zip(ctx.args[::2], ctx.args[1::2])
         }
```

### Comparing `broker-0.4.9/broker/exceptions.py` & `broker-0.5.0/broker/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,7 +68,19 @@
     error_code = 11
 
 
 class BeakerBindError(BrokerError):
     """Raised when a problem occurs at the Beaker bind level."""
 
     error_code = 12
+
+
+class UserError(BrokerError):
+    """Raised when a user causes an otherwise unclassified error."""
+
+    error_code = 13
+
+
+class ForemanBindError(BrokerError):
+    """Raised when a problem occurs at the Foreman bind level."""
+
+    error_code = 14
```

### Comparing `broker-0.4.9/broker/helpers.py` & `broker-0.5.0/broker/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from uuid import uuid4
 
 import click
 from logzero import logger
 import yaml
 
 from broker import exceptions, logger as b_log, settings
+from broker.binds.containers import demux_output
 
 FilterTest = namedtuple("FilterTest", "haystack needle test")
 INVENTORY_LOCK = threading.Lock()
 
 
 def clean_dict(in_dict):
     """Remove entries from a dict where value is None."""
@@ -389,15 +390,16 @@
 
 def fork_broker():
     """Fork the Broker process to run in the background."""
     pid = os.fork()
     if pid:
         logger.info(f"Running broker in the background with pid: {pid}")
         sys.exit(0)
-    update_log_level(None, None, "silent")
+    b_log.set_log_level("silent")
+    b_log.set_file_logging("silent")
 
 
 def handle_keyboardinterrupt(*args):
     """Handle keyboard interrupts gracefully.
 
     Offer the user a choice between keeping Broker alive in the background or killing it.
     """
@@ -503,20 +505,27 @@
 
     @classmethod
     def from_ssh(cls, stdout, channel):
         """Create a Result object from an SSH channel."""
         return cls(
             stdout=stdout,
             status=channel.get_exit_status(),
-            stderr=channel.read_stderr(),
+            stderr=channel.read_stderr()[1].decode("utf-8"),
         )
 
     @classmethod
-    def from_duplexed_exec(cls, duplex_exec):
-        """Create a Result object from a duplexed exec object from the docker library."""
+    def from_duplexed_exec(cls, duplex_exec, runtime=None):
+        """Create a Result object from a duplexed exec object from podman or docker."""
+        if runtime == "podman":
+            stdout, stderr = demux_output(duplex_exec[1])
+            return cls(
+                status=duplex_exec[0],
+                stdout=stdout.decode("utf-8"),
+                stderr=stderr.decode("utf-8"),
+            )
         if duplex_exec.output[0]:
             stdout = duplex_exec.output[0].decode("utf-8")
         else:
             stdout = ""
         if duplex_exec.output[1]:
             stderr = duplex_exec.output[1].decode("utf-8")
         else:
```

### Comparing `broker-0.4.9/broker/hosts.py` & `broker-0.5.0/broker/hosts.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,16 @@
         If the session object does not exist, it will be created by calling the `connect` method.
         If the host is a non-SSH-enabled container host, a `ContainerSession` object will be created instead.
         """
         # This attribute may be missing after pickling
         if not isinstance(getattr(self, "_session", None), Session):
             # Check to see if we're a non-ssh-enabled Container Host
             if hasattr(self, "_cont_inst") and not self._cont_inst.ports.get(22):
-                self._session = ContainerSession(self)
+                runtime = "podman" if "podman" in str(self._cont_inst.client) else "docker"
+                self._session = ContainerSession(self, runtime=runtime)
             else:
                 self.connect()
         return self._session
 
     def connect(
         self,
         username=None,
@@ -132,15 +133,15 @@
             ipv4_fallback=ipv4_fallback,
         )
 
     def close(self):
         """Close the SSH connection to the host."""
         # This attribute may be missing after pickling
         if isinstance(getattr(self, "_session", None), Session):
-            self._session.session.disconnect()
+            self._session.disconnect()
         self._session = None
 
     def release(self):
         """Release the host using the appropriate method for the provider."""
         raise NotImplementedError("release has not been implemented for this provider")
 
     # @cached_property
```

### Comparing `broker-0.4.9/broker/logger.py` & `broker-0.5.0/broker/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,18 +53,16 @@
 
 _sensitive = ["password", "pword", "token", "host_password"]
 logging.addLevelName("TRACE", LOG_LEVEL.TRACE)
 logzero.DEFAULT_COLORS[LOG_LEVEL.TRACE.value] = logzero.colors.Fore.MAGENTA
 
 
 def patch_awx_for_verbosity(api):
-    """Patch the awxkit API to log when we're at trace level."""
-    client = api.client
-    awx_log = client.log
-
+    """Patch the awxkit API to enable trace-level logging of API calls to Ansible provider."""
+    awx_log = api.client.log
     awx_log.parent = logzero.logger
 
     def patch(cls, name):
         func = getattr(cls, name)
 
         def the_patch(self, *args, **kwargs):
             awx_log.log(LOG_LEVEL.TRACE.value, f"Calling {self=} {func=}(*{args=}, **{kwargs=}")
@@ -112,15 +110,20 @@
 def set_file_logging(level=settings.logging.file_level, path="logs/broker.log"):
     """Set the file logging for logzero."""
     silent = False
     if level == "silent":
         silent = True
         log_level = LOG_LEVEL.INFO
     else:
-        log_level = resolve_log_level(level)
+        # Allow override of file logging level with --log-level, if the new level is lower than
+        # settings.logging.file_level. Otherwise, use the value from settings.
+        old_log_level = resolve_log_level(settings.logging.file_level)
+        new_log_level = resolve_log_level(level)
+        log_level = new_log_level if new_log_level < old_log_level else old_log_level
+
     path = BROKER_DIRECTORY.joinpath(path)
     path.parent.mkdir(parents=True, exist_ok=True)
     logzero.logfile(
         path,
         loglevel=log_level.value,
         maxBytes=1e9,
         backupCount=3,
@@ -134,16 +137,15 @@
     formatter=None,
     file_level=settings.logging.file_level,
     name=None,
     path="logs/broker.log",
 ):
     """Call logzero setup with the given settings."""
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-    if isinstance(level, str) and level.lower() == "trace":
-        patch_awx_for_verbosity(awxkit.api)
+    patch_awx_for_verbosity(awxkit.api)
     set_log_level(level)
     set_file_logging(file_level, path)
     if formatter:
         logzero.formatter(formatter)
     logzero.logger.name = name or "broker"
     logzero.logger.addFilter(RedactingFilter(_sensitive))
```

### Comparing `broker-0.4.9/broker/providers/__init__.py` & `broker-0.5.0/broker/providers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,24 +151,17 @@
             settings.validators.validate(only=section_name)
         except dynaconf.ValidationError as err:
             raise exceptions.ConfigurationError(err) from err
 
     def _set_attributes(self, obj, attrs):
         obj.__dict__.update(attrs)
 
-    def _get_params(self, arg_list, kwargs):
-        return {k: v for k, v in kwargs.items() if k in arg_list}
-
+    @abstractmethod
     def construct_host(self, host_cls, provider_params, **kwargs):
         """Construct a host object from a host class and include relevent provider params."""
-        host_inst = host_cls(**provider_params, **kwargs)
-        host_attrs = self._get_params(self._construct_params)
-        host_attrs["release"] = self._host_release
-        self._set_attributes(host_inst, host_attrs)
-        return host_inst
 
     @abstractmethod
     def provider_help(self):
         """Help options that will be added to the CLI.
 
         Anything other than 'self' and 'kwargs' will be added as a help option
         To specify a flag, set the default value to a boolean
```

### Comparing `broker-0.4.9/broker/providers/ansible_tower.py` & `broker-0.5.0/broker/providers/ansible_tower.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,22 +13,40 @@
 from broker import exceptions
 from broker.helpers import eval_filter, find_origin
 from broker.settings import settings
 
 try:
     import awxkit
 except ImportError as err:
-    raise exceptions.ProviderError(
-        provider="AnsibleTower", message="Unable to import awxkit. Is it installed?"
-    ) from err
+    raise exceptions.UserError(message="Unable to import awxkit. Is it installed?") from err
 
 from broker import helpers
 from broker.providers import Provider
 
 
+class JobExecutionError(exceptions.ProviderError):
+    """Raised when a job execution fails."""
+
+    def __init__(self, message_data=None):
+        super().__init__(
+            provider="AnsibleTower",
+            message=json.dumps(message_data, indent=2),
+        )
+
+
+class ATInventoryError(exceptions.ProviderError):
+    """Raised when we can't find the right inventory."""
+
+    def __init__(self, message_data=None):
+        super().__init__(
+            provider="AnsibleTower",
+            message=json.dumps(message_data, indent=2),
+        )
+
+
 @cache
 def get_awxkit_and_uname(config=None, root=None, url=None, token=None, uname=None, pword=None):
     """Return an awxkit api object and resolved username."""
     # Prefer token if its set, otherwise use username/password
     # auth paths for the API taken from:
     # https://github.com/ansible/awx/blob/ddb6c5d0cce60779be279b702a15a2fddfcd0724/awxkit/awxkit/cli/client.py#L85-L94
     # unit test mock structure means the root API instance can't be loaded on the same line
@@ -47,16 +65,15 @@
         versions = root.get().available_versions
         try:
             # lookup the user that authenticated with the token
             # If a username was specified in config, use that instead
             my_username = uname or versions.v2.get().me.get().results[0].username
         except (IndexError, AttributeError) as err:
             # lookup failed for whatever reason
-            raise exceptions.ProviderError(
-                provider="AnsibleTower",
+            raise exceptions.ConfigurationError(
                 message="Failed to lookup a username for the given token, please check credentials",
             ) from err
     else:  # dynaconf validators should have checked that either token or password was provided
         helpers.emit(auth_type="password")
         if datetime.now() < datetime(2023, 2, 6):
             time_based_modifier = " and will be unavailable soon"
         else:
@@ -199,44 +216,40 @@
             host_inst.__dict__.update(misc_attrs)
 
     def _translate_inventory(self, inventory):
         if isinstance(inventory, int):  # already an id, silly
             if inventory_info := self.v2.inventory.get(id=inventory):
                 return inventory_info.results[0].name
             else:
-                raise exceptions.ProviderError(
-                    provider="AnsibleTower",
+                raise ATInventoryError(
                     message=f"Unknown AnsibleTower inventory by id {inventory}",
                 )
         elif isinstance(inventory, str):
             if inventory_info := self.v2.inventory.get(search=inventory):
                 if inventory_info.count > 1:
                     # let's try to manually narrow down to one result if the api returns multiple
                     filtered = [inv for inv in inventory_info.results if inv.name == inventory]
                     if len(filtered) == 1:
                         return filtered[0].id
-                    raise exceptions.ProviderError(
-                        provider="AnsibleTower",
+                    raise ATInventoryError(
                         message=f"Ambigious AnsibleTower inventory name {inventory}",
                     )
                 elif inventory_info.count == 1:
                     return inventory_info.results.pop().id
                 else:
-                    raise exceptions.ProviderError(
-                        provider="AnsibleTower",
+                    raise ATInventoryError(
                         message=f"Unknown AnsibleTower inventory {inventory}",
                     )
         elif inv_id := getattr(inventory, "id", None):
             return inv_id
         elif inv_name := getattr(inventory, "name", None):
             return inv_name
         else:
             caller_context = inspect.stack()[1][0].f_locals
-            raise exceptions.ProviderError(
-                provider="AnsibleTower",
+            raise ATInventoryError(
                 message=f"Ambiguous AnsibleTower inventory {inventory} passed from {caller_context}",
             )
 
     def _merge_artifacts(self, at_object, strategy="last", artifacts=None):
         """Gather and merge all artifacts associated with an object and its children.
 
         :param at_object: object you want to merge
@@ -432,14 +445,33 @@
             )
             compiled = {}
             for line in extra_vars.splitlines():
                 key, val = line.split(": ")
                 compiled[key] = val
             return compiled
 
+    def _resolve_labels(self, labels, target):
+        """Fetch and return ids of the given labels.
+
+        If label does not exist, create it under the same org as the target template.
+        """
+        label_ids = []
+        for label in labels:
+            label_expanded = f"{label}={labels[label]}" if labels[label] else label
+            if result := self.v2.labels.get(name=label_expanded).results:
+                label_ids.append(result[0].id)
+            else:
+                # label does not exist yet, creating
+                result = self.v2.labels.post(
+                    {"name": label_expanded, "organization": target.summary_fields.organization.id}
+                )
+                if result:
+                    label_ids.append(result.id)
+        return label_ids
+
     @cached_property
     def inventory(self):
         """Return the current tower inventory."""
         if not self._inventory:
             return
         elif isinstance(self._inventory, int):
             # inventory already resolved as id
@@ -532,15 +564,15 @@
             host_inst = host_classes[kwargs.get("type")](**broker_args)
 
         self._set_attributes(host_inst, broker_args=broker_args, misc_attrs=broker_facts)
 
         return host_inst
 
     @Provider.register_action("workflow", "job_template")
-    def execute(self, **kwargs):  # noqa: PLR0912 - Possible TODO refactor
+    def execute(self, **kwargs):  # noqa: PLR0912,PLR0915 - Possible TODO refactor
         """Execute workflow or job template in Ansible Tower.
 
         :param kwargs: workflow or job template name passed in a string
 
         :return: dictionary containing all information about executed workflow/job template
         """
         if name := kwargs.get("workflow"):
@@ -550,38 +582,45 @@
             kwargs["_broker_origin"] = origin[0]
             if origin[1]:
                 kwargs["_jenkins_url"] = origin[1]
         elif name := kwargs.get("job_template"):
             subject = "job_template"
             get_path = self.v2.job_templates
         else:
-            raise exceptions.ProviderError(
-                provider="AnsibleTower", message="No workflow or job template specified"
-            )
+            raise exceptions.UserError(message="No workflow or job template specified")
         try:
             candidates = get_path.get(name=name).results
         except awxkit.exceptions.Unauthorized as err:
             raise exceptions.AuthenticationError(err.args[0]) from err
         if candidates:
             target = candidates.pop()
         else:
-            raise exceptions.ProviderError(
-                provider="AnsibleTower",
-                message=f"{subject.capitalize()} not found by name: {name}",
-            )
+            raise exceptions.UserError(message=f"{subject.capitalize()} not found by name: {name}")
         payload = {}
         if inventory := kwargs.pop("inventory", None):
             payload["inventory"] = inventory
             logger.info(f"Using tower inventory: {self._translate_inventory(inventory)}")
+
         elif self.inventory:
             payload["inventory"] = self.inventory
             logger.info(f"Using tower inventory: {self._translate_inventory(self.inventory)}")
         else:
             logger.info("No inventory specified, Ansible Tower will use a default.")
 
+        # provider labels handling
+
+        provider_labels = kwargs.get("provider_labels", {})
+        # include eventual common labels, specified at each level of configuration
+        # typically imported from dynaconf env vars
+        provider_labels.update(settings.get("provider_labels", {}))
+        provider_labels.update(settings.ANSIBLETOWER.get("provider_labels", {}))
+        if provider_labels:
+            payload["labels"] = self._resolve_labels(provider_labels, target)
+            kwargs["provider_labels"] = provider_labels
+
         # Save custom, non-workflow extra vars to a named variable.
         # The workflow can save these values to job artifacts / host facts.
         workflow_extra_vars = self._pull_extra_vars(target.extra_vars)
         kwargs["_broker_extra_vars"] = {
             k: v for k, v in kwargs.items() if k not in workflow_extra_vars
         }
         payload["extra_vars"] = str(kwargs)
@@ -601,17 +640,15 @@
         if job.status != "successful":
             message_data = {
                 f"{subject.capitalize()} Status": job.status,
                 "Reason(s)": self._get_failure_messages(job),
                 "URL": job_ui_url,
             }
             helpers.emit(message_data)
-            raise exceptions.ProviderError(
-                provider="AnsibleTower", message=message_data["Reason(s)"]
-            )
+            raise JobExecutionError(message_data=message_data)
         if strategy := kwargs.pop("artifacts", None):
             return self._merge_artifacts(job, strategy=strategy)
         return job
 
     def get_inventory(self, user=None):
         """Compile a list of hosts based on any inventory a user's name is mentioned."""
         user = user or self.username
@@ -624,29 +661,30 @@
         for inv in invs:
             inv_hosts = inv.get_related("hosts", page_size=200).results
             hosts.extend(inv_hosts)
         with click.progressbar(hosts, label="Compiling host information") as hosts_bar:
             compiled_host_info = [self._compile_host_info(host) for host in hosts_bar]
         return compiled_host_info
 
-    def extend(self, target_vm, new_expire_time=None):
+    def extend(self, target_vm, new_expire_time=None, provider_labels=None):
         """Run the extend workflow with defaults args.
 
         :param target_vm: This should be a host object
         """
         # check if an inventory was specified. if so overwrite the current inventory
         if new_inv := target_vm._broker_args.get("tower_inventory"):
             if new_inv != self._inventory:
                 self._inventory = new_inv
                 if hasattr(self.__dict__, "inventory"):
                     del self.inventory  # clear the cached value
         return self.execute(
             workflow=settings.ANSIBLETOWER.extend_workflow,
             target_vm=target_vm.name,
             new_expire_time=new_expire_time or settings.ANSIBLETOWER.get("new_expire_time"),
+            provider_labels=provider_labels,
         )
 
     def provider_help(
         self,
         workflows=False,
         workflow=None,
         job_templates=False,
```

### Comparing `broker-0.4.9/broker/providers/beaker.py` & `broker-0.5.0/broker/providers/beaker.py`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/broker/providers/container.py` & `broker-0.5.0/broker/providers/container.py`

 * *Files 18% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             # [{'hostPort': 1337, 'containerPort': 22, 'protocol': 'tcp', 'hostIP': ''},
             for pm in port_map:
                 if pm["containerPort"] == ssh_port:
                     return pm["hostPort"]
         elif isinstance(port_map, dict):
             # {'22/tcp': [{'HostIp': '', 'HostPort': '1337'}],
             for key, val in port_map.items():
-                if key.startswith("22"):
+                if key.startswith("22") and isinstance(val, list):
                     return val[0]["HostPort"]
 
     def _set_attributes(self, host_inst, broker_args=None, cont_inst=None):
         host_inst.__dict__.update(
             {
                 "_prov_inst": self,
                 "_cont_inst": cont_inst,
@@ -270,22 +270,39 @@
 
         if "for" in origin:
             origin = origin.split()[-1]
         envars["BROKER_ORIGIN"] = origin[0]
         if origin[1]:
             envars["JENKINS_URL"] = origin[1]
         kwargs["environment"] = envars
-        kwargs["labels"] = envars
+
+        # process eventual provider labels for each setting level
+        kwargs["provider_labels"] = kwargs.get("provider_labels", {})
+        kwargs["provider_labels"].update(settings.get("provider_labels", {}))
+        kwargs["provider_labels"].update(settings.CONTAINER.get("provider_labels", {}))
+        # prefix eventual label keys with 'broker.' to conform to the docker guidelines
+        # https://docs.docker.com/config/labels-custom-metadata/#key-format-recommendations
+        kwargs["provider_labels"] = {
+            f"broker.{label[0]}": label[1] for label in kwargs.get("provider_labels", {}).items()
+        }
+        # process eventual labels that were passed externally, split by "="
+        kwargs["provider_labels"].update(
+            {"broker.origin": origin[0], "broker.jenkins.url": origin[1]}
+        )
+        # rename the dict key to the name of the arg recognized by provider
+        kwargs["labels"] = kwargs.pop("provider_labels")
         container_inst = self.runtime.create_container(container_host, **kwargs)
         container_inst.start()
         return container_inst
 
     @Provider.register_action("container_app")
     def execute(self, container_app, **kwargs):
         """Run a container and return the raw results."""
+        if not kwargs.get("name"):
+            kwargs["name"] = self._gen_name()
         return self.runtime.execute(container_app, **kwargs)
 
     def run_wait_container(self, image_name, **kwargs):
         """Run a container and wait for it to exit."""
         cont_inst = self.run_container(image_name, **kwargs)
         cont_inst.wait(condition="excited")
         return self.runtime.get_logs(cont_inst)
```

### Comparing `broker-0.4.9/broker/providers/test_provider.py` & `broker-0.5.0/broker/providers/test_provider.py`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/broker/settings.py` & `broker-0.5.0/broker/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,51 +16,67 @@
 import click
 from dynaconf import Dynaconf, Validator
 from dynaconf.validator import ValidationError
 
 from broker.exceptions import ConfigurationError
 
 
-def init_settings(settings_path, interactive=False):
+def init_settings(settings_path, source, interactive=False, is_url=False):
     """Initialize the broker settings file."""
-    raw_url = (
-        "https://raw.githubusercontent.com/SatelliteQE/broker/master/broker_settings.yaml.example"
-    )
     proceed = not False
     if interactive:
         try:
             proceed = (
                 click.prompt(
-                    f"Download example file from GitHub?\n{raw_url}",
+                    f"Get example file from {source}?\n{source}",
                     type=click.Choice(["y", "n"]),
                     default="y",
                 )
                 == "y"
             )
         except click.core.Abort:
             # We're likely in a different non-interactive environment (container?)
             global INTERACTIVE_MODE
             proceed, INTERACTIVE_MODE = True, False
     if proceed:
-        # download example file from github
-        import requests
-
-        click.echo(f"Downloading example file from: {raw_url}")
-        raw_file = requests.get(raw_url, timeout=60)
-        settings_path.write_text(raw_file.text)
+        # get example file from source
+        if is_url:
+            import requests
+
+            click.echo(f"Downloading example file from: {source}")
+            raw_file = requests.get(source, timeout=60)
+            settings_path.write_text(raw_file.text)
+        else:
+            example_file = source.read_text()
+            settings_path.write_text(example_file)
         if INTERACTIVE_MODE:
             try:
                 click.edit(filename=str(settings_path.absolute()))
             except click.exceptions.ClickException:
                 click.secho(
                     f"Please edit the file {settings_path.absolute()} and add your settings.",
                     fg="yellow",
                 )
-    else:
-        raise ConfigurationError(f"Broker settings file not found at {settings_path.absolute()}.")
+        return True
+
+
+def init_settings_from_github(settings_path, interactive=False):
+    """Initialize the broker settings file."""
+    raw_url = (
+        "https://raw.githubusercontent.com/SatelliteQE/broker/master/broker_settings.yaml.example"
+    )
+    return init_settings(settings_path, raw_url, interactive, is_url=True)
+
+
+def init_settings_from_local_repo(settings_path, interactive=False):
+    """Initialize the broker settings file."""
+    example_path = Path(__file__).parent.parent.joinpath("broker_settings.yaml.example")
+    if not example_path.exists():
+        return
+    return init_settings(settings_path, example_path, interactive)
 
 
 INTERACTIVE_MODE = False
 # GitHub action context
 if "GITHUB_WORKFLOW" not in os.environ:
     # determine if we're being ran from a CLI
     for frame in inspect.stack()[::-1]:
@@ -80,24 +96,28 @@
 BROKER_DIRECTORY.mkdir(parents=True, exist_ok=True)
 
 settings_path = BROKER_DIRECTORY.joinpath("broker_settings.yaml")
 inventory_path = BROKER_DIRECTORY.joinpath("inventory.yaml")
 
 if not settings_path.exists():
     click.secho(f"Broker settings file not found at {settings_path.absolute()}.", fg="red")
-    init_settings(settings_path, interactive=INTERACTIVE_MODE)
+    if not (success := init_settings_from_local_repo(settings_path, interactive=INTERACTIVE_MODE)):
+        success = init_settings_from_github(settings_path, interactive=INTERACTIVE_MODE)
+    if not success:
+        raise ConfigurationError(f"Broker settings file not found at {settings_path.absolute()}.")
 
 validators = [
     Validator("HOST_USERNAME", default="root"),
     Validator("HOST_PASSWORD", default="toor"),
     Validator("HOST_CONNECTION_TIMEOUT", default=60),
     Validator("HOST_SSH_PORT", default=22),
     Validator("HOST_SSH_KEY_FILENAME", default=None),
     Validator("HOST_IPV6", default=False),
     Validator("HOST_IPV4_FALLBACK", default=True),
+    Validator("SSH_BACKEND", default="ssh2-python312"),
     Validator("LOGGING", is_type_of=dict),
     Validator(
         "LOGGING.CONSOLE_LEVEL",
         is_in=["error", "warning", "info", "debug", "trace", "silent"],
         default="info",
     ),
     Validator(
```

### Comparing `broker-0.4.9/broker.egg-info/PKG-INFO` & `broker-0.5.0/broker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broker
-Version: 0.4.9
+Version: 0.5.0
 Summary: The infrastructure middleman.
 Author-email: Jacob J Callahan <jacob.callahan05@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -706,20 +706,28 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Provides-Extra: docker
 Requires-Dist: docker; extra == "docker"
 Requires-Dist: paramiko; extra == "docker"
 Provides-Extra: podman
-Requires-Dist: podman-py; extra == "podman"
+Requires-Dist: podman; extra == "podman"
 Provides-Extra: setup
 Requires-Dist: build; extra == "setup"
 Requires-Dist: twine; extra == "setup"
 Provides-Extra: ssh2-py311
 Requires-Dist: ssh2-python; extra == "ssh2-py311"
+Provides-Extra: ssh2-python
+Requires-Dist: ssh2-python; extra == "ssh2-python"
+Provides-Extra: ssh2-python312
+Requires-Dist: ssh2-python312; extra == "ssh2-python312"
+Provides-Extra: ansible-pylibssh
+Requires-Dist: ansible-pylibssh; extra == "ansible-pylibssh"
+Provides-Extra: hussh
+Requires-Dist: hussh; extra == "hussh"
 
 [![PythonPackage](https://github.com/SatelliteQE/broker/actions/workflows/python-publish.yml/badge.svg)](https://github.com/SatelliteQE/broker/actions/workflows/python-publish.yml)
 [![ContainerImage](https://github.com/SatelliteQE/broker/actions/workflows/update_broker_image.yml/badge.svg)](https://github.com/SatelliteQE/broker/actions/workflows/update_broker_image.yml)
 [![CodeQL](https://github.com/SatelliteQE/broker/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/SatelliteQE/broker/actions/workflows/codeql-analysis.yml)
 # Broker
 The infrastrucure middleman
 
@@ -831,14 +839,14 @@
 ```
 broker --output-file output.json checkout --nick rhel7
 broker --output-file inventory.json inventory
 ```
 
 **Run Broker in the background**
 
-Certain Broker actions can be run in the background, these currently are: checkout, checkin, duplicate, and execute. When running a command in this mode, it will spin up a new Broker process and no longer log to stderr. To check progress, you can still follow broker's log file.
+Certain Broker actions can be run in the background, these currently are: checkout, checkin, and execute. When running a command in this mode, it will spin up a new Broker process and no longer log to stderr. To check progress, you can still follow broker's log file.
 Note that background mode will interfere with output options for execute since it won't be able to print to stdout. Those should kept in log mode.
 ```
 broker checkout --background --nick rhel7
 broker checkin -b --all
 broker execute -b --workflow my-awesome-workflow --artifacts
 ```
```

### Comparing `broker-0.4.9/broker.egg-info/SOURCES.txt` & `broker-0.5.0/broker.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -25,18 +25,24 @@
 broker.egg-info/entry_points.txt
 broker.egg-info/not-zip-safe
 broker.egg-info/requires.txt
 broker.egg-info/top_level.txt
 broker/binds/__init__.py
 broker/binds/beaker.py
 broker/binds/containers.py
+broker/binds/foreman.py
+broker/binds/hussh.py
+broker/binds/pylibssh.py
+broker/binds/ssh2.py
+broker/binds/utils.py
 broker/providers/__init__.py
 broker/providers/ansible_tower.py
 broker/providers/beaker.py
 broker/providers/container.py
+broker/providers/foreman.py
 broker/providers/test_provider.py
 catalog/system/broker.yaml
 logs/.gitignore
 tests/conftest.py
 tests/test_broker.py
 tests/test_helpers.py
 tests/test_settings.py
@@ -54,18 +60,23 @@
 tests/data/cli_scenarios/beaker/checkout_test_job.yaml
 tests/data/cli_scenarios/containers/checkout_ch-d_ubi8.yaml
 tests/data/cli_scenarios/containers/checkout_ch-d_ubi8_2.yaml
 tests/data/cli_scenarios/containers/execute_ch-d_ubi8.yaml
 tests/data/cli_scenarios/satlab/checkout_latest_rhel.yaml
 tests/data/cli_scenarios/satlab/checkout_latest_sat.yaml
 tests/data/cli_scenarios/satlab/checkout_rhel91.yaml
-tests/data/cli_scenarios/satlab/checkout_sat_611.yaml
+tests/data/cli_scenarios/satlab/checkout_sat_613.yaml
 tests/data/cli_scenarios/satlab/execute_templates_list.yaml
 tests/data/container/fake_containers.json
 tests/data/container/fake_images.json
+tests/data/foreman/fake_get.json
+tests/data/foreman/fake_hosts.json
+tests/data/foreman/fake_jobs.json
+tests/data/foreman/fake_resources.json
 tests/functional/README.md
 tests/functional/test_containers.py
 tests/functional/test_rh_beaker.py
 tests/functional/test_satlab.py
 tests/providers/test_ansible_tower.py
 tests/providers/test_beaker.py
-tests/providers/test_container.py
+tests/providers/test_container.py
+tests/providers/test_foreman.py
```

### Comparing `broker-0.4.9/broker_settings.yaml.example` & `broker-0.5.0/broker_settings.yaml.example`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 host_password: "<password>"
 host_ssh_port: 22
 host_ssh_key_filename: "</path/to/the/ssh-key>"
 # Default all host ssh connections to IPv6
 host_ipv6: False
 # If IPv6 connection attempts fail, fallback to IPv4
 host_ipv4_fallback: True
+ssh_backend: ssh2-python312
 # Provider settings
 AnsibleTower:
     base_url: "https://<ansible tower host>/"
     # Username is required for both token and password-based authentication
     username: "<username>"
     # token is the preferred authentication method
     token: "<AT personal access token>"
@@ -29,25 +30,43 @@
     results_limit: 50
 Container:
     instances:
         - docker:
             host_username: "<username>"
             host_password: "<plain text password>"
             host_port: None
+            runtime: docker
             default: True
         - remote:
             host: "<remote hostname>"
             host_username: "<username>"
             host_password: "<plain text password>"
-    runtime: 'docker'
+    runtime: podman
     # name used to prefix container names, used to distinguish yourself
     # if not set, then your local username will be used
     # name_prefix: test
     results_limit: 50
     auto_map_ports: False
+Foreman:
+  instances:
+    - foreman1:
+        foreman_url: https://test.fore.man
+        foreman_username: admin
+        foreman_password: secret
+        organization: ORG
+        location: LOC
+        verify: ./ca.crt
+        default: true
+    - foreman2:
+        foreman_url: https://other-test.fore.man
+        foreman_username: admin
+        foreman_password: secret
+        organization: ORG
+        location: LOC
+  name_prefix: broker
 Beaker:
     hub_url:
     max_job_wait: 24h
 TestProvider:
     instances:
         - test1:
             foo: "bar"
@@ -57,15 +76,15 @@
             override_envars: True
         - bad:
             nothing: False
     config_value: "something"
 # You can set a nickname as a shortcut for arguments
 nicks:
     rhel7:
-        workflow: "deploy-base-rhel"
+        workflow: "deploy-rhel"
         deploy_rhel_version: "7.9"
         notes: "Requested by broker"
     test_nick:
         test_action: "fake"
         arg1: "abc"
         arg2: 123
         arg3: True
```

### Comparing `broker-0.4.9/pyproject.toml` & `broker-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -44,20 +44,25 @@
     "pytest",
     "ruff"
 ]
 docker = [
     "docker",
     "paramiko"
 ]
-podman = ["podman-py"]
+podman = ["podman"]
 setup = [
     "build",
     "twine",
 ]
+
 ssh2_py311 = ["ssh2-python"]
+ssh2_python = ["ssh2-python"]
+ssh2_python312 = ["ssh2-python312"]
+ansible_pylibssh = ["ansible-pylibssh"]
+hussh = ["hussh"]
 
 [project.scripts]
 broker = "broker.commands:cli"
 
 [tool.setuptools]
 platforms = ["any"]
 zip-safe = false
```

### Comparing `broker-0.4.9/tests/data/ansible_tower/fake_children.json` & `broker-0.5.0/tests/data/ansible_tower/fake_children.json`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/tests/data/ansible_tower/fake_jobs.json` & `broker-0.5.0/tests/data/ansible_tower/fake_jobs.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904763%*

 * *Differences: {'0': "{'name': 'deploy-rhel'}"}*

```diff
@@ -1,12 +1,12 @@
 [
     {
         "extra_vars": "{\"provider\": \"rhv\", \"host_type\": \"\"}",
         "id": 343,
-        "name": "deploy-base-rhel",
+        "name": "deploy-rhel",
         "related": {
             "workflow_nodes": "/api/v2/workflow_jobs/343/workflow_nodes/"
         },
         "status": "successful",
         "type": "workflow_job",
         "url": "/api/v2/workflow_jobs/1329/"
     },
```

### Comparing `broker-0.4.9/tests/data/beaker/job_result.json` & `broker-0.5.0/tests/data/beaker/job_result.json`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/tests/data/beaker/test_job.xml` & `broker-0.5.0/tests/data/beaker/test_job.xml`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/tests/data/container/fake_containers.json` & `broker-0.5.0/tests/data/container/fake_containers.json`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/tests/data/container/fake_images.json` & `broker-0.5.0/tests/data/container/fake_images.json`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/tests/data/fake_inventory.yaml` & `broker-0.5.0/tests/data/fake_inventory.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 - _broker_args:
     deploy_rhel_version: '8.6'
     deploy_scenario: baserhel
     host_type: host
-    workflow: deploy-base-rhel
+    workflow: deploy-rhel
   _broker_provider: AnsibleTower
   _broker_provider_instance: rhv
   hostname: dhcp-111.test.example.com
   name: mahuser-rhel-8.6-6e74d20e
   tower_inventory: rhv-rhvm02
   type: host
 - _broker_args:
     deploy_rhel_version: '8.6'
     deploy_scenario: baserhel
     host_type: host
-    workflow: deploy-base-rhel
+    workflow: deploy-rhel
   _broker_provider: AnsibleTower
   _broker_provider_instance: rhv
   hostname: dhcp-121.test.example.com
   name: mahuser-rhel-8.6-be7062a8
   tower_inventory: rhv-rhvm02
   type: host
 - _broker_args: {}
```

### Comparing `broker-0.4.9/tests/functional/README.md` & `broker-0.5.0/tests/functional/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Do not attempt to use Broker while running these functional tests or you may end up with resources being checked in during the cleanup phases.
 
 **Container Tests**
 
 Setup:
 - Ensure either Docker or Podman are installed and configured either locally or on a remote host.
 - Ensure Broker's Container provider is configured with the details of the previous step.
-- Clone the [content-host-d](https://github.com/JacobCallahan/content-host-d) repository and build the UBI8 image, tagging it as `ch-d:ubi8`.
+- Clone the [content-host-d](https://github.com/JacobCallahan/content-host-d) repository and build the UBI[7-9] images, tagging them as `ubi[7-9]` respectively.
 
 **SatLab Tests**
 
 Setup:
 - Ensure you have your account credentials entered into the AnsibleTower provider section of Broker's config.
 - Make sure you have room for at least 4 hosts in your current SLA limit.
```

### Comparing `broker-0.4.9/tests/functional/test_containers.py` & `broker-0.5.0/tests/functional/test_containers.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from tempfile import NamedTemporaryFile
 import pytest
 from click.testing import CliRunner
 from broker import Broker
 from broker.commands import cli
 from broker.providers.container import Container
 from broker.settings import inventory_path
+from broker.settings import settings_path as SETTINGS_PATH
 
 SCENARIO_DIR = Path("tests/data/cli_scenarios/containers")
 
 
 @pytest.fixture(scope="module", autouse=True)
 def skip_if_not_configured():
     try:
@@ -28,23 +29,23 @@
     backup_path.rename(inventory_path)
 
 
 # ----- CLI Scenario Tests -----
 
 
 @pytest.mark.parametrize(
-    "args_file", [f for f in SCENARIO_DIR.iterdir() if f.name.startswith("checkout_")]
+    "args_file", [f for f in SCENARIO_DIR.iterdir() if f.name.startswith("checkout_")], ids=lambda f: f.name.split(".")[0]
 )
 def test_checkout_scenarios(args_file, temp_inventory):
     result = CliRunner().invoke(cli, ["checkout", "--args-file", args_file])
     assert result.exit_code == 0
 
 
 @pytest.mark.parametrize(
-    "args_file", [f for f in SCENARIO_DIR.iterdir() if f.name.startswith("execute_")]
+    "args_file", [f for f in SCENARIO_DIR.iterdir() if f.name.startswith("execute_")], ids=lambda f: f.name.split(".")[0]
 )
 def test_execute_scenarios(args_file):
     result = CliRunner().invoke(cli, ["execute", "--args-file", args_file])
     assert result.exit_code == 0
 
 
 def test_inventory_sync():
@@ -62,35 +63,37 @@
     assert result.exit_code == 0
 
 
 # ----- Broker API Tests -----
 
 
 def test_container_e2e():
-    with Broker(container_host="ubi8:latest") as c_host:
+    with Broker(container_host="ubi8:latest", provider_labels={"l1": "v1", "l2": None}) as c_host:
         assert c_host._cont_inst.top()["Processes"]
         res = c_host.execute("hostname")
         assert res.stdout.strip() == c_host.hostname
-        loc_settings_path = Path("broker_settings.yaml")
         remote_dir = "/tmp/fake"
-        c_host.session.sftp_write(loc_settings_path.name, f"{remote_dir}/")
+        c_host.session.sftp_write(str(SETTINGS_PATH), f"{remote_dir}/")
         res = c_host.execute(f"ls {remote_dir}")
-        assert str(loc_settings_path) in res.stdout
+        assert SETTINGS_PATH.name in res.stdout
         with NamedTemporaryFile() as tmp:
-            c_host.session.sftp_read(f"{remote_dir}/{loc_settings_path.name}", tmp.file.name)
+            c_host.session.sftp_read(f"{remote_dir}/{SETTINGS_PATH.name}", tmp.file.name)
             data = c_host.session.sftp_read(
-                f"{remote_dir}/{loc_settings_path.name}", return_data=True
+                f"{remote_dir}/{SETTINGS_PATH.name}", return_data=True
             )
             assert (
-                loc_settings_path.read_bytes() == Path(tmp.file.name).read_bytes()
+                SETTINGS_PATH.read_bytes() == Path(tmp.file.name).read_bytes()
             ), "Local file is different from the received one"
             assert (
-                loc_settings_path.read_bytes() == data
+                SETTINGS_PATH.read_bytes() == data
             ), "Local file is different from the received one (return_data=True)"
             assert data == Path(tmp.file.name).read_bytes(), "Received files do not match"
+        # assert labels
+        assert c_host._cont_inst.labels.get("broker.l1") == "v1"
+        assert c_host._cont_inst.labels.get("broker.l2") == ""
         # test the tail_file context manager
         tailed_file = f"{remote_dir}/tail_me.txt"
         c_host.execute(f"echo 'hello world' > {tailed_file}")
         with c_host.session.tail_file(tailed_file) as tf:
             c_host.execute(f"echo 'this is a new line' >> {tailed_file}")
         assert "this is a new line" in tf.stdout
         assert "hello world" not in tf.stdout
@@ -98,38 +101,37 @@
 
 def test_container_e2e_mp():
     with Broker(container_host="ubi8:latest", _count=7) as c_hosts:
         for c_host in c_hosts:
             assert c_host._cont_inst.top()["Processes"]
             res = c_host.execute("hostname")
             assert res.stdout.strip() == c_host.hostname
-            loc_settings_path = Path("broker_settings.yaml")
             remote_dir = "/tmp/fake"
-            c_host.session.sftp_write(loc_settings_path.name, f"{remote_dir}/")
+            c_host.session.sftp_write(str(SETTINGS_PATH), f"{remote_dir}/")
             res = c_host.execute(f"ls {remote_dir}")
-            assert str(loc_settings_path) in res.stdout
+            assert SETTINGS_PATH.name in res.stdout
             with NamedTemporaryFile() as tmp:
-                c_host.session.sftp_read(f"{remote_dir}/{loc_settings_path.name}", tmp.file.name)
+                c_host.session.sftp_read(f"{remote_dir}/{SETTINGS_PATH.name}", tmp.file.name)
                 data = c_host.session.sftp_read(
-                    f"{remote_dir}/{loc_settings_path.name}", return_data=True
+                    f"{remote_dir}/{SETTINGS_PATH.name}", return_data=True
                 )
                 assert (
-                    loc_settings_path.read_bytes() == Path(tmp.file.name).read_bytes()
+                    SETTINGS_PATH.read_bytes() == Path(tmp.file.name).read_bytes()
                 ), "Local file is different from the received one"
                 assert (
-                    loc_settings_path.read_bytes() == data
+                    SETTINGS_PATH.read_bytes() == data
                 ), "Local file is different from the received one (return_data=True)"
                 assert data == Path(tmp.file.name).read_bytes(), "Received files do not match"
 
 
 def test_broker_multi_manager():
     with Broker.multi_manager(
-        ubi7={"container_host": "ubi7:latest"},
-        ubi8={"container_host": "ubi8:latest", "_count": 2},
-        ubi9={"container_host": "ubi9:latest"},
+        ubi7={"container_host": "localhost/ubi7:latest"},
+        ubi8={"container_host": "localhost/ubi8:latest", "_count": 2},
+        ubi9={"container_host": "localhost/ubi9:latest"},
     ) as multi_hosts:
         assert "ubi7" in multi_hosts
         assert "ubi8" in multi_hosts
         assert "ubi9" in multi_hosts
         assert len(multi_hosts["ubi8"]) == 2
         assert multi_hosts["ubi7"][0]._cont_inst.top()["Processes"]
         assert (
```

### Comparing `broker-0.4.9/tests/functional/test_rh_beaker.py` & `broker-0.5.0/tests/functional/test_rh_beaker.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     yield
     CliRunner().invoke(cli, ["checkin", "--all", "--filter", '@inv._broker_provider == "Beaker"'])
     inventory_path.unlink()
     backup_path.rename(inventory_path)
 
 
 @pytest.mark.parametrize(
-    "args_file", [f for f in SCENARIO_DIR.iterdir() if f.name.startswith("checkout_")]
+    "args_file", [f for f in SCENARIO_DIR.iterdir() if f.name.startswith("checkout_")], ids=lambda f: f.name.split(".")[0]
 )
 def test_checkout_scenarios(args_file, temp_inventory):
     result = CliRunner().invoke(cli, ["checkout", "--args-file", args_file])
     assert result.exit_code == 0
 
 
 # @pytest.mark.parametrize(
-#     "args_file", [f for f in SCENARIO_DIR.iterdir() if f.name.startswith("execute_")]
+#     "args_file", [f for f in SCENARIO_DIR.iterdir() if f.name.startswith("execute_")], ids=lambda f: f.name.split(".")[0]
 # )
 # def test_execute_scenarios(args_file):
 #     result = CliRunner().invoke(cli, ["execute", "--args-file", args_file])
 #     assert result.exit_code == 0
 
 
 def test_inventory_sync():
```

### Comparing `broker-0.4.9/tests/providers/test_ansible_tower.py` & `broker-0.5.0/tests/providers/test_ansible_tower.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,33 +84,33 @@
 
 @pytest.fixture
 def tower_stub(api_stub, config_stub):
     return AnsibleTower(root=api_stub, config=config_stub)
 
 
 def test_execute(tower_stub):
-    job = tower_stub.execute(workflow="deploy-base-rhel")
+    job = tower_stub.execute(workflow="deploy-rhel")
     assert "workflow_nodes" in job.related
 
 
 def test_host_creation(tower_stub):
     bx = Broker()
-    job = tower_stub.execute(workflow="deploy-base-rhel")
+    job = tower_stub.execute(workflow="deploy-rhel")
     host = tower_stub.construct_host(job, bx.host_classes)
     assert isinstance(host, bx.host_classes["host"])
     assert host.hostname == "fake.host.test.com"
     assert host._broker_args["os_distribution_version"] == "7.8"
 
 
 def test_workflow_lookup_failure(tower_stub):
-    with pytest.raises(Broker.ProviderError) as err:
+    with pytest.raises(Broker.UserError) as err:
         tower_stub.execute(workflow="this-does-not-exist")
     assert "Workflow not found by name: this-does-not-exist" in err.value.message
 
 
 def test_host_release_dual_params(tower_stub):
     bx = Broker()
-    job = tower_stub.execute(workflow="deploy-base-rhel")
+    job = tower_stub.execute(workflow="deploy-rhel")
     host = tower_stub.construct_host(job, bx.host_classes)
     host._broker_args["source_vm"] = "fake-physical-host"
     assert host._broker_args["source_vm"] == host.name
     host.release()
```

### Comparing `broker-0.4.9/tests/providers/test_beaker.py` & `broker-0.5.0/tests/providers/test_beaker.py`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/tests/providers/test_container.py` & `broker-0.5.0/tests/providers/test_container.py`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/tests/test_broker.py` & `broker-0.5.0/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/tests/test_helpers.py` & `broker-0.5.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `broker-0.4.9/tests/test_settings.py` & `broker-0.5.0/tests/test_settings.py`

 * *Files identical despite different names*

