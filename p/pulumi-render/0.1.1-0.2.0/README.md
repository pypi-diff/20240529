# Comparing `tmp/pulumi_render-0.1.1.tar.gz` & `tmp/pulumi_render-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_render-0.1.1.tar", last modified: Sun May  5 02:01:39 2024, max compression
+gzip compressed data, was "pulumi_render-0.2.0.tar", last modified: Wed May 29 04:47:11 2024, max compression
```

## Comparing `pulumi_render-0.1.1.tar` & `pulumi_render-0.2.0.tar`

### file list

```diff
@@ -1,65 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:39.073893 pulumi_render-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-05 02:01:39.073893 pulumi_render-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:39.065893 pulumi_render-0.1.1/pulumi_render/
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:39.065893 pulumi_render-0.1.1/pulumi_render/config/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:39.069893 pulumi_render-0.1.1/pulumi_render/owners/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/owners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/owners/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/owners/get_owner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/owners/list_owners.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/owners/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:39.069893 pulumi_render-0.1.1/pulumi_render/registrycredentials/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/registrycredentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/registrycredentials/get_registry_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/registrycredentials/list_registry_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/registrycredentials/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/registrycredentials/registry_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:39.073893 pulumi_render-0.1.1/pulumi_render/services/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    39491 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/auto_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)    19297 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/background_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/cron_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/custom_domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/deploys.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_background_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_cron_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_private_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_static_site.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_web_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/list_custom_domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/list_deploys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/list_env_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/list_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/list_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/list_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/list_services.py
--rw-r--r--   0 runner    (1001) docker     (127)    99395 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19185 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/private_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/scale.py
--rw-r--r--   0 runner    (1001) docker     (127)    19193 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/static_site.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/suspend.py
--rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/web_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:39.073893 pulumi_render-0.1.1/pulumi_render.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-05 02:01:39.000000 pulumi_render-0.1.1/pulumi_render.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-05 02:01:39.000000 pulumi_render-0.1.1/pulumi_render.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 02:01:39.000000 pulumi_render-0.1.1/pulumi_render.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 02:01:39.000000 pulumi_render-0.1.1/pulumi_render.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 02:01:39.000000 pulumi_render-0.1.1/pulumi_render.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 02:01:39.077893 pulumi_render-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 04:47:11.064650 pulumi_render-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-29 04:47:11.064650 pulumi_render-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 04:47:11.056650 pulumi_render-0.2.0/pulumi_render/
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 04:47:11.056650 pulumi_render-0.2.0/pulumi_render/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 04:47:11.056650 pulumi_render-0.2.0/pulumi_render/owners/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/owners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/owners/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/owners/get_owner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/owners/list_owners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/owners/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 04:47:11.056650 pulumi_render-0.2.0/pulumi_render/registrycredentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/registrycredentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/registrycredentials/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/registrycredentials/get_registry_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/registrycredentials/list_registry_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/registrycredentials/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/registrycredentials/registry_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 04:47:11.064650 pulumi_render-0.2.0/pulumi_render/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41635 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/autoscale_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17607 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/background_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/cancel_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/cancel_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17364 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/cron_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/env_vars_for_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/get_background_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/get_cron_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/get_custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/get_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/get_private_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/get_static_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/get_web_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/list_custom_domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/list_deploys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/list_env_vars_for_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/list_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/list_retrieve_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/list_retrieve_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/list_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105882 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/preview_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17553 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/private_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/refresh_custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/restart_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/rollback_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/scale_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17327 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/static_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/suspend_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17445 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pulumi_render/services/web_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 04:47:11.064650 pulumi_render-0.2.0/pulumi_render.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-29 04:47:11.000000 pulumi_render-0.2.0/pulumi_render.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-29 04:47:11.000000 pulumi_render-0.2.0/pulumi_render.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 04:47:11.000000 pulumi_render-0.2.0/pulumi_render.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 04:47:11.000000 pulumi_render-0.2.0/pulumi_render.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 04:47:11.000000 pulumi_render-0.2.0/pulumi_render.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-29 04:47:04.000000 pulumi_render-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 04:47:11.064650 pulumi_render-0.2.0/setup.cfg
```

### Comparing `pulumi_render-0.1.1/PKG-INFO` & `pulumi_render-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_render
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Pulumi package for creating and managing Render resources.
 License: Apache-2.0
 Project-URL: Homepage, https://cloudysky.software
 Project-URL: Repository, https://github.com/cloudy-sky-software/pulumi-render
 Keywords: pulumi,render,category/cloud,kind/native
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_render-0.1.1/README.md` & `pulumi_render-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.1.1/pulumi_render/__init__.py` & `pulumi_render-0.2.0/pulumi_render/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,25 +35,31 @@
   }
  },
  {
   "pkg": "render",
   "mod": "services",
   "fqn": "pulumi_render.services",
   "classes": {
-   "render:services:AutoScaling": "AutoScaling",
+   "render:services:AutoscaleService": "AutoscaleService",
    "render:services:BackgroundWorker": "BackgroundWorker",
+   "render:services:CancelDeploy": "CancelDeploy",
+   "render:services:CancelJob": "CancelJob",
    "render:services:CronJob": "CronJob",
-   "render:services:CustomDomains": "CustomDomains",
-   "render:services:Deploys": "Deploys",
-   "render:services:EnvVars": "EnvVars",
-   "render:services:Jobs": "Jobs",
+   "render:services:CustomDomain": "CustomDomain",
+   "render:services:Deploy": "Deploy",
+   "render:services:EnvVarsForService": "EnvVarsForService",
+   "render:services:Job": "Job",
+   "render:services:PreviewService": "PreviewService",
    "render:services:PrivateService": "PrivateService",
-   "render:services:Scale": "Scale",
+   "render:services:RefreshCustomDomain": "RefreshCustomDomain",
+   "render:services:RestartServer": "RestartServer",
+   "render:services:RollbackDeploy": "RollbackDeploy",
+   "render:services:ScaleService": "ScaleService",
    "render:services:StaticSite": "StaticSite",
-   "render:services:Suspend": "Suspend",
+   "render:services:SuspendService": "SuspendService",
    "render:services:WebService": "WebService"
   }
  }
 ]
 """,
     resource_packages="""
 [
```

### Comparing `pulumi_render-0.1.1/pulumi_render/_utilities.py` & `pulumi_render-0.2.0/pulumi_render/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.1.1/pulumi_render/config/__init__.pyi` & `pulumi_render-0.2.0/pulumi_render/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.1.1/pulumi_render/config/vars.py` & `pulumi_render-0.2.0/pulumi_render/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.1.1/pulumi_render/owners/get_owner.py` & `pulumi_render-0.2.0/pulumi_render/owners/get_owner.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,32 +36,32 @@
     def __await__(self):
         if False:
             yield self
         return GetOwnerResult(
             items=self.items)
 
 
-def get_owner(id: Optional[str] = None,
+def get_owner(owner_id: Optional[str] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOwnerResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the user or team
+    :param str owner_id: The ID of the user or team
     """
     __args__ = dict()
-    __args__['id'] = id
+    __args__['ownerId'] = owner_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:owners:getOwner', __args__, opts=opts, typ=GetOwnerResult).value
 
     return AwaitableGetOwnerResult(
         items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_owner)
-def get_owner_output(id: Optional[pulumi.Input[str]] = None,
+def get_owner_output(owner_id: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOwnerResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the user or team
+    :param str owner_id: The ID of the user or team
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/owners/list_owners.py` & `pulumi_render-0.2.0/pulumi_render/owners/list_owners.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def __init__(__self__, items=None):
         if items and not isinstance(items, list):
             raise TypeError("Expected argument 'items' to be a list")
         pulumi.set(__self__, "items", items)
 
     @property
     @pulumi.getter
-    def items(self) -> Sequence['outputs.ListOwnersResponse']:
+    def items(self) -> Sequence['outputs.ListOwnersItemProperties']:
         return pulumi.get(self, "items")
 
 
 class AwaitableListOwnersResult(ListOwnersResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumi_render-0.1.1/pulumi_render/provider.py` & `pulumi_render-0.2.0/pulumi_render/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.1.1/pulumi_render/registrycredentials/get_registry_credential.py` & `pulumi_render-0.2.0/pulumi_render/registrycredentials/get_registry_credential.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
+from ._enums import *
 
 __all__ = [
     'GetRegistryCredentialResult',
     'AwaitableGetRegistryCredentialResult',
     'get_registry_credential',
     'get_registry_credential_output',
 ]
@@ -22,38 +23,45 @@
     def __init__(__self__, items=None):
         if items and not isinstance(items, dict):
             raise TypeError("Expected argument 'items' to be a dict")
         pulumi.set(__self__, "items", items)
 
     @property
     @pulumi.getter
-    def items(self) -> 'outputs.GetRegistryCredentialProperties':
+    def items(self) -> 'outputs.RegistryCredential':
         return pulumi.get(self, "items")
 
 
 class AwaitableGetRegistryCredentialResult(GetRegistryCredentialResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetRegistryCredentialResult(
             items=self.items)
 
 
-def get_registry_credential(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRegistryCredentialResult:
+def get_registry_credential(registry_credential_id: Optional[str] = None,
+                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRegistryCredentialResult:
     """
     Use this data source to access information about an existing resource.
+
+    :param str registry_credential_id: The ID of the registry credential
     """
     __args__ = dict()
+    __args__['registryCredentialId'] = registry_credential_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:registrycredentials:getRegistryCredential', __args__, opts=opts, typ=GetRegistryCredentialResult).value
 
     return AwaitableGetRegistryCredentialResult(
         items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_registry_credential)
-def get_registry_credential_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRegistryCredentialResult]:
+def get_registry_credential_output(registry_credential_id: Optional[pulumi.Input[str]] = None,
+                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRegistryCredentialResult]:
     """
     Use this data source to access information about an existing resource.
+
+    :param str registry_credential_id: The ID of the registry credential
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/registrycredentials/list_registry_credentials.py` & `pulumi_render-0.2.0/pulumi_render/registrycredentials/list_registry_credentials.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
+from ._enums import *
 
 __all__ = [
     'ListRegistryCredentialsResult',
     'AwaitableListRegistryCredentialsResult',
     'list_registry_credentials',
     'list_registry_credentials_output',
 ]
@@ -22,15 +23,15 @@
     def __init__(__self__, items=None):
         if items and not isinstance(items, list):
             raise TypeError("Expected argument 'items' to be a list")
         pulumi.set(__self__, "items", items)
 
     @property
     @pulumi.getter
-    def items(self) -> Sequence['outputs.ListRegistryCredentialsItemProperties']:
+    def items(self) -> Sequence['outputs.RegistryCredential']:
         return pulumi.get(self, "items")
 
 
 class AwaitableListRegistryCredentialsResult(ListRegistryCredentialsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumi_render-0.1.1/pulumi_render/registrycredentials/outputs.py` & `pulumi_render-0.2.0/pulumi_render/owners/outputs.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,87 +4,69 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
+from ._enums import *
 
 __all__ = [
-    'GetRegistryCredentialProperties',
-    'ListRegistryCredentialsItemProperties',
+    'ListOwnersItemProperties',
+    'Owner',
 ]
 
 @pulumi.output_type
-class GetRegistryCredentialProperties(dict):
+class ListOwnersItemProperties(dict):
     def __init__(__self__, *,
-                 id: Optional[str] = None,
-                 name: Optional[str] = None,
-                 registry: Optional[str] = None,
-                 username: Optional[str] = None):
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if registry is not None:
-            pulumi.set(__self__, "registry", registry)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
+                 cursor: Optional[str] = None,
+                 owner: Optional['outputs.Owner'] = None):
+        if cursor is not None:
+            pulumi.set(__self__, "cursor", cursor)
+        if owner is not None:
+            pulumi.set(__self__, "owner", owner)
 
     @property
     @pulumi.getter
-    def id(self) -> Optional[str]:
-        return pulumi.get(self, "id")
-
-    @property
-    @pulumi.getter
-    def name(self) -> Optional[str]:
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter
-    def registry(self) -> Optional[str]:
-        return pulumi.get(self, "registry")
+    def cursor(self) -> Optional[str]:
+        return pulumi.get(self, "cursor")
 
     @property
     @pulumi.getter
-    def username(self) -> Optional[str]:
-        return pulumi.get(self, "username")
+    def owner(self) -> Optional['outputs.Owner']:
+        return pulumi.get(self, "owner")
 
 
 @pulumi.output_type
-class ListRegistryCredentialsItemProperties(dict):
+class Owner(dict):
     def __init__(__self__, *,
-                 id: Optional[str] = None,
-                 name: Optional[str] = None,
-                 registry: Optional[str] = None,
-                 username: Optional[str] = None):
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if registry is not None:
-            pulumi.set(__self__, "registry", registry)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
+                 email: str,
+                 id: str,
+                 name: str,
+                 type: 'OwnerType'):
+        pulumi.set(__self__, "email", email)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
-    def id(self) -> Optional[str]:
-        return pulumi.get(self, "id")
+    def email(self) -> str:
+        return pulumi.get(self, "email")
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[str]:
-        return pulumi.get(self, "name")
+    def id(self) -> str:
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def registry(self) -> Optional[str]:
-        return pulumi.get(self, "registry")
+    def name(self) -> str:
+        return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def username(self) -> Optional[str]:
-        return pulumi.get(self, "username")
+    def type(self) -> 'OwnerType':
+        return pulumi.get(self, "type")
```

### Comparing `pulumi_render-0.1.1/pulumi_render/registrycredentials/registry_credential.py` & `pulumi_render-0.2.0/pulumi_render/registrycredentials/registry_credential.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,106 +4,103 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from ._enums import *
 
 __all__ = ['RegistryCredentialArgs', 'RegistryCredential']
 
 @pulumi.input_type
 class RegistryCredentialArgs:
     def __init__(__self__, *,
-                 auth_token: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 owner_id: Optional[pulumi.Input[str]] = None,
-                 registry: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None):
+                 auth_token: pulumi.Input[str],
+                 owner_id: pulumi.Input[str],
+                 registry: pulumi.Input['Registry'],
+                 username: pulumi.Input[str],
+                 name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a RegistryCredential resource.
         """
-        if auth_token is not None:
-            pulumi.set(__self__, "auth_token", auth_token)
+        pulumi.set(__self__, "auth_token", auth_token)
+        pulumi.set(__self__, "owner_id", owner_id)
+        pulumi.set(__self__, "registry", registry)
+        pulumi.set(__self__, "username", username)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if owner_id is not None:
-            pulumi.set(__self__, "owner_id", owner_id)
-        if registry is not None:
-            pulumi.set(__self__, "registry", registry)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authToken")
-    def auth_token(self) -> Optional[pulumi.Input[str]]:
+    def auth_token(self) -> pulumi.Input[str]:
         return pulumi.get(self, "auth_token")
 
     @auth_token.setter
-    def auth_token(self, value: Optional[pulumi.Input[str]]):
+    def auth_token(self, value: pulumi.Input[str]):
         pulumi.set(self, "auth_token", value)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
-    @property
     @pulumi.getter(name="ownerId")
-    def owner_id(self) -> Optional[pulumi.Input[str]]:
+    def owner_id(self) -> pulumi.Input[str]:
         return pulumi.get(self, "owner_id")
 
     @owner_id.setter
-    def owner_id(self, value: Optional[pulumi.Input[str]]):
+    def owner_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "owner_id", value)
 
     @property
     @pulumi.getter
-    def registry(self) -> Optional[pulumi.Input[str]]:
+    def registry(self) -> pulumi.Input['Registry']:
         return pulumi.get(self, "registry")
 
     @registry.setter
-    def registry(self, value: Optional[pulumi.Input[str]]):
+    def registry(self, value: pulumi.Input['Registry']):
         pulumi.set(self, "registry", value)
 
     @property
     @pulumi.getter
-    def username(self) -> Optional[pulumi.Input[str]]:
+    def username(self) -> pulumi.Input[str]:
         return pulumi.get(self, "username")
 
     @username.setter
-    def username(self, value: Optional[pulumi.Input[str]]):
+    def username(self, value: pulumi.Input[str]):
         pulumi.set(self, "username", value)
 
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
 
 class RegistryCredential(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  auth_token: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  owner_id: Optional[pulumi.Input[str]] = None,
-                 registry: Optional[pulumi.Input[str]] = None,
+                 registry: Optional[pulumi.Input['Registry']] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a RegistryCredential resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[RegistryCredentialArgs] = None,
+                 args: RegistryCredentialArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Create a RegistryCredential resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param RegistryCredentialArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
@@ -117,29 +114,37 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  auth_token: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  owner_id: Optional[pulumi.Input[str]] = None,
-                 registry: Optional[pulumi.Input[str]] = None,
+                 registry: Optional[pulumi.Input['Registry']] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RegistryCredentialArgs.__new__(RegistryCredentialArgs)
 
+            if auth_token is None and not opts.urn:
+                raise TypeError("Missing required property 'auth_token'")
             __props__.__dict__["auth_token"] = auth_token
             __props__.__dict__["name"] = name
+            if owner_id is None and not opts.urn:
+                raise TypeError("Missing required property 'owner_id'")
             __props__.__dict__["owner_id"] = owner_id
+            if registry is None and not opts.urn:
+                raise TypeError("Missing required property 'registry'")
             __props__.__dict__["registry"] = registry
+            if username is None and not opts.urn:
+                raise TypeError("Missing required property 'username'")
             __props__.__dict__["username"] = username
         super(RegistryCredential, __self__).__init__(
             'render:registrycredentials:RegistryCredential',
             resource_name,
             __props__,
             opts)
 
@@ -164,30 +169,39 @@
         __props__.__dict__["owner_id"] = None
         __props__.__dict__["registry"] = None
         __props__.__dict__["username"] = None
         return RegistryCredential(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="authToken")
-    def auth_token(self) -> pulumi.Output[Optional[str]]:
+    def auth_token(self) -> pulumi.Output[str]:
         return pulumi.get(self, "auth_token")
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Output[Optional[str]]:
+    def name(self) -> pulumi.Output[str]:
+        """
+        Descriptive name for this credential
+        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="ownerId")
-    def owner_id(self) -> pulumi.Output[Optional[str]]:
+    def owner_id(self) -> pulumi.Output[str]:
         return pulumi.get(self, "owner_id")
 
     @property
     @pulumi.getter
-    def registry(self) -> pulumi.Output[Optional[str]]:
+    def registry(self) -> pulumi.Output['Registry']:
+        """
+        The registry to use this credential with
+        """
         return pulumi.get(self, "registry")
 
     @property
     @pulumi.getter
-    def username(self) -> pulumi.Output[Optional[str]]:
+    def username(self) -> pulumi.Output[str]:
+        """
+        The username associated with the credential
+        """
         return pulumi.get(self, "username")
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/_inputs.py` & `pulumi_render-0.2.0/pulumi_render/services/_inputs.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,279 +7,306 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from ._enums import *
 
 __all__ = [
-    'AutoScalingCriteriaSpecArgs',
-    'AutoScalingCriteriaArgs',
-    'BackgroundWorkerServiceDetailsParentServerPropertiesArgs',
-    'BackgroundWorkerServiceDetailsArgs',
-    'CronJobServiceDetailsArgs',
-    'DiskArgs',
+    'AutoscalingCriteriaPercentageArgs',
+    'AutoscalingCriteriaArgs',
+    'BackgroundWorkerDetailsCreateDiskPropertiesArgs',
+    'BackgroundWorkerDetailsCreateArgs',
+    'BuildFilterArgs',
+    'CronJobDetailsCreateArgs',
     'DockerDetailsArgs',
+    'EnvVarKeyGenerateValueArgs',
     'EnvVarKeyValueArgs',
+    'HeaderCreateArgs',
+    'ImageArgs',
     'NativeEnvironmentDetailsArgs',
-    'OpenPortsArgs',
-    'PrivateServiceDetailsParentServerPropertiesArgs',
-    'PrivateServiceDetailsArgs',
+    'PrivateServiceDetailsCreateDiskPropertiesArgs',
+    'PrivateServiceDetailsCreateArgs',
+    'RegistryCredentialArgs',
+    'RouteArgs',
     'SecretFileArgs',
-    'ServiceHeaderArgs',
-    'StaticSiteRouteArgs',
-    'StaticSiteServiceDetailsParentServerPropertiesArgs',
-    'StaticSiteServiceDetailsArgs',
-    'WebServiceServiceDetailsParentServerPropertiesArgs',
-    'WebServiceServiceDetailsArgs',
+    'StaticSiteDetailsCreateArgs',
+    'WebServiceDetailsCreateDiskPropertiesArgs',
+    'WebServiceDetailsCreateArgs',
 ]
 
 @pulumi.input_type
-class AutoScalingCriteriaSpecArgs:
+class AutoscalingCriteriaPercentageArgs:
     def __init__(__self__, *,
                  enabled: Optional[pulumi.Input[bool]] = None,
-                 percentage: Optional[pulumi.Input[float]] = None):
+                 percentage: pulumi.Input[int]):
         """
-        :param pulumi.Input[float] percentage: Determines when your service will be scaled. If the average resource utilization is significantly above/below the target, we will increase/decrease the number of instances.
+        :param pulumi.Input[int] percentage: Determines when your service will be scaled. If the average resource utilization is significantly above/below the target, we will increase/decrease the number of instances.
         """
-        if enabled is not None:
-            pulumi.set(__self__, "enabled", enabled)
-        if percentage is not None:
-            pulumi.set(__self__, "percentage", percentage)
+        if enabled is None:
+            enabled = False
+        pulumi.set(__self__, "enabled", enabled)
+        pulumi.set(__self__, "percentage", percentage)
 
     @property
     @pulumi.getter
-    def enabled(self) -> Optional[pulumi.Input[bool]]:
+    def enabled(self) -> pulumi.Input[bool]:
         return pulumi.get(self, "enabled")
 
     @enabled.setter
-    def enabled(self, value: Optional[pulumi.Input[bool]]):
+    def enabled(self, value: pulumi.Input[bool]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter
-    def percentage(self) -> Optional[pulumi.Input[float]]:
+    def percentage(self) -> pulumi.Input[int]:
         """
         Determines when your service will be scaled. If the average resource utilization is significantly above/below the target, we will increase/decrease the number of instances.
         """
         return pulumi.get(self, "percentage")
 
     @percentage.setter
-    def percentage(self, value: Optional[pulumi.Input[float]]):
+    def percentage(self, value: pulumi.Input[int]):
         pulumi.set(self, "percentage", value)
 
 
 @pulumi.input_type
-class AutoScalingCriteriaArgs:
+class AutoscalingCriteriaArgs:
     def __init__(__self__, *,
-                 cpu: Optional[pulumi.Input['AutoScalingCriteriaSpecArgs']] = None,
-                 memory: Optional[pulumi.Input['AutoScalingCriteriaSpecArgs']] = None):
-        if cpu is not None:
-            pulumi.set(__self__, "cpu", cpu)
-        if memory is not None:
-            pulumi.set(__self__, "memory", memory)
+                 cpu: pulumi.Input['AutoscalingCriteriaPercentageArgs'],
+                 memory: pulumi.Input['AutoscalingCriteriaPercentageArgs']):
+        pulumi.set(__self__, "cpu", cpu)
+        pulumi.set(__self__, "memory", memory)
 
     @property
     @pulumi.getter
-    def cpu(self) -> Optional[pulumi.Input['AutoScalingCriteriaSpecArgs']]:
+    def cpu(self) -> pulumi.Input['AutoscalingCriteriaPercentageArgs']:
         return pulumi.get(self, "cpu")
 
     @cpu.setter
-    def cpu(self, value: Optional[pulumi.Input['AutoScalingCriteriaSpecArgs']]):
+    def cpu(self, value: pulumi.Input['AutoscalingCriteriaPercentageArgs']):
         pulumi.set(self, "cpu", value)
 
     @property
     @pulumi.getter
-    def memory(self) -> Optional[pulumi.Input['AutoScalingCriteriaSpecArgs']]:
+    def memory(self) -> pulumi.Input['AutoscalingCriteriaPercentageArgs']:
         return pulumi.get(self, "memory")
 
     @memory.setter
-    def memory(self, value: Optional[pulumi.Input['AutoScalingCriteriaSpecArgs']]):
+    def memory(self, value: pulumi.Input['AutoscalingCriteriaPercentageArgs']):
         pulumi.set(self, "memory", value)
 
 
 @pulumi.input_type
-class BackgroundWorkerServiceDetailsParentServerPropertiesArgs:
+class BackgroundWorkerDetailsCreateDiskPropertiesArgs:
     def __init__(__self__, *,
-                 id: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+                 mount_path: pulumi.Input[str],
+                 name: pulumi.Input[str],
+                 size_gb: Optional[pulumi.Input[int]] = None):
+        """
+        :param pulumi.Input[int] size_gb: Defaults to 1
+        """
+        pulumi.set(__self__, "mount_path", mount_path)
+        pulumi.set(__self__, "name", name)
+        if size_gb is not None:
+            pulumi.set(__self__, "size_gb", size_gb)
 
     @property
-    @pulumi.getter
-    def id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "id")
+    @pulumi.getter(name="mountPath")
+    def mount_path(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "mount_path")
 
-    @id.setter
-    def id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "id", value)
+    @mount_path.setter
+    def mount_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "mount_path", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "name")
 
     @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
+    def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
+    @property
+    @pulumi.getter(name="sizeGB")
+    def size_gb(self) -> Optional[pulumi.Input[int]]:
+        """
+        Defaults to 1
+        """
+        return pulumi.get(self, "size_gb")
+
+    @size_gb.setter
+    def size_gb(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "size_gb", value)
+
 
 @pulumi.input_type
-class BackgroundWorkerServiceDetailsArgs:
+class BackgroundWorkerDetailsCreateArgs:
     def __init__(__self__, *,
-                 env: pulumi.Input['BackgroundWorkerServiceDetailsEnv'],
-                 disk: Optional[pulumi.Input['DiskArgs']] = None,
+                 env: pulumi.Input['BackgroundWorkerDetailsCreateEnv'],
+                 disk: Optional[pulumi.Input['BackgroundWorkerDetailsCreateDiskPropertiesArgs']] = None,
                  env_specific_details: Optional[pulumi.Input[Union['DockerDetailsArgs', 'NativeEnvironmentDetailsArgs']]] = None,
-                 num_instances: Optional[pulumi.Input[float]] = None,
-                 parent_server: Optional[pulumi.Input['BackgroundWorkerServiceDetailsParentServerPropertiesArgs']] = None,
-                 plan: Optional[pulumi.Input['BackgroundWorkerServiceDetailsPlan']] = None,
-                 pull_request_previews_enabled: Optional[pulumi.Input['BackgroundWorkerServiceDetailsPullRequestPreviewsEnabled']] = None,
-                 region: Optional[pulumi.Input['BackgroundWorkerServiceDetailsRegion']] = None,
-                 url: Optional[pulumi.Input[str]] = None):
+                 num_instances: Optional[pulumi.Input[int]] = None,
+                 plan: Optional[pulumi.Input['BackgroundWorkerDetailsCreatePlan']] = None,
+                 pull_request_previews_enabled: Optional[pulumi.Input['BackgroundWorkerDetailsCreatePullRequestPreviewsEnabled']] = None,
+                 region: Optional[pulumi.Input['BackgroundWorkerDetailsCreateRegion']] = None):
+        """
+        :param pulumi.Input['BackgroundWorkerDetailsCreateEnv'] env: Environment (runtime)
+        :param pulumi.Input[int] num_instances: Defaults to 1
+        :param pulumi.Input['BackgroundWorkerDetailsCreatePullRequestPreviewsEnabled'] pull_request_previews_enabled: Defaults to "no"
+        """
         pulumi.set(__self__, "env", env)
         if disk is not None:
             pulumi.set(__self__, "disk", disk)
         if env_specific_details is not None:
             pulumi.set(__self__, "env_specific_details", env_specific_details)
         if num_instances is None:
             num_instances = 1
         if num_instances is not None:
             pulumi.set(__self__, "num_instances", num_instances)
-        if parent_server is not None:
-            pulumi.set(__self__, "parent_server", parent_server)
-        if plan is None:
-            plan = 'starter'
         if plan is not None:
             pulumi.set(__self__, "plan", plan)
         if pull_request_previews_enabled is None:
             pull_request_previews_enabled = 'no'
         if pull_request_previews_enabled is not None:
             pulumi.set(__self__, "pull_request_previews_enabled", pull_request_previews_enabled)
-        if region is None:
-            region = 'oregon'
         if region is not None:
             pulumi.set(__self__, "region", region)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
-    def env(self) -> pulumi.Input['BackgroundWorkerServiceDetailsEnv']:
+    def env(self) -> pulumi.Input['BackgroundWorkerDetailsCreateEnv']:
+        """
+        Environment (runtime)
+        """
         return pulumi.get(self, "env")
 
     @env.setter
-    def env(self, value: pulumi.Input['BackgroundWorkerServiceDetailsEnv']):
+    def env(self, value: pulumi.Input['BackgroundWorkerDetailsCreateEnv']):
         pulumi.set(self, "env", value)
 
     @property
     @pulumi.getter
-    def disk(self) -> Optional[pulumi.Input['DiskArgs']]:
+    def disk(self) -> Optional[pulumi.Input['BackgroundWorkerDetailsCreateDiskPropertiesArgs']]:
         return pulumi.get(self, "disk")
 
     @disk.setter
-    def disk(self, value: Optional[pulumi.Input['DiskArgs']]):
+    def disk(self, value: Optional[pulumi.Input['BackgroundWorkerDetailsCreateDiskPropertiesArgs']]):
         pulumi.set(self, "disk", value)
 
     @property
     @pulumi.getter(name="envSpecificDetails")
     def env_specific_details(self) -> Optional[pulumi.Input[Union['DockerDetailsArgs', 'NativeEnvironmentDetailsArgs']]]:
         return pulumi.get(self, "env_specific_details")
 
     @env_specific_details.setter
     def env_specific_details(self, value: Optional[pulumi.Input[Union['DockerDetailsArgs', 'NativeEnvironmentDetailsArgs']]]):
         pulumi.set(self, "env_specific_details", value)
 
     @property
     @pulumi.getter(name="numInstances")
-    def num_instances(self) -> Optional[pulumi.Input[float]]:
+    def num_instances(self) -> Optional[pulumi.Input[int]]:
+        """
+        Defaults to 1
+        """
         return pulumi.get(self, "num_instances")
 
     @num_instances.setter
-    def num_instances(self, value: Optional[pulumi.Input[float]]):
+    def num_instances(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "num_instances", value)
 
     @property
-    @pulumi.getter(name="parentServer")
-    def parent_server(self) -> Optional[pulumi.Input['BackgroundWorkerServiceDetailsParentServerPropertiesArgs']]:
-        return pulumi.get(self, "parent_server")
-
-    @parent_server.setter
-    def parent_server(self, value: Optional[pulumi.Input['BackgroundWorkerServiceDetailsParentServerPropertiesArgs']]):
-        pulumi.set(self, "parent_server", value)
-
-    @property
     @pulumi.getter
-    def plan(self) -> Optional[pulumi.Input['BackgroundWorkerServiceDetailsPlan']]:
+    def plan(self) -> Optional[pulumi.Input['BackgroundWorkerDetailsCreatePlan']]:
         return pulumi.get(self, "plan")
 
     @plan.setter
-    def plan(self, value: Optional[pulumi.Input['BackgroundWorkerServiceDetailsPlan']]):
+    def plan(self, value: Optional[pulumi.Input['BackgroundWorkerDetailsCreatePlan']]):
         pulumi.set(self, "plan", value)
 
     @property
     @pulumi.getter(name="pullRequestPreviewsEnabled")
-    def pull_request_previews_enabled(self) -> Optional[pulumi.Input['BackgroundWorkerServiceDetailsPullRequestPreviewsEnabled']]:
+    def pull_request_previews_enabled(self) -> Optional[pulumi.Input['BackgroundWorkerDetailsCreatePullRequestPreviewsEnabled']]:
+        """
+        Defaults to "no"
+        """
         return pulumi.get(self, "pull_request_previews_enabled")
 
     @pull_request_previews_enabled.setter
-    def pull_request_previews_enabled(self, value: Optional[pulumi.Input['BackgroundWorkerServiceDetailsPullRequestPreviewsEnabled']]):
+    def pull_request_previews_enabled(self, value: Optional[pulumi.Input['BackgroundWorkerDetailsCreatePullRequestPreviewsEnabled']]):
         pulumi.set(self, "pull_request_previews_enabled", value)
 
     @property
     @pulumi.getter
-    def region(self) -> Optional[pulumi.Input['BackgroundWorkerServiceDetailsRegion']]:
+    def region(self) -> Optional[pulumi.Input['BackgroundWorkerDetailsCreateRegion']]:
         return pulumi.get(self, "region")
 
     @region.setter
-    def region(self, value: Optional[pulumi.Input['BackgroundWorkerServiceDetailsRegion']]):
+    def region(self, value: Optional[pulumi.Input['BackgroundWorkerDetailsCreateRegion']]):
         pulumi.set(self, "region", value)
 
+
+@pulumi.input_type
+class BuildFilterArgs:
+    def __init__(__self__, *,
+                 ignored_paths: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 paths: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(__self__, "ignored_paths", ignored_paths)
+        pulumi.set(__self__, "paths", paths)
+
+    @property
+    @pulumi.getter(name="ignoredPaths")
+    def ignored_paths(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        return pulumi.get(self, "ignored_paths")
+
+    @ignored_paths.setter
+    def ignored_paths(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "ignored_paths", value)
+
     @property
     @pulumi.getter
-    def url(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "url")
+    def paths(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        return pulumi.get(self, "paths")
 
-    @url.setter
-    def url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "url", value)
+    @paths.setter
+    def paths(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "paths", value)
 
 
 @pulumi.input_type
-class CronJobServiceDetailsArgs:
+class CronJobDetailsCreateArgs:
     def __init__(__self__, *,
-                 env: pulumi.Input['CronJobServiceDetailsEnv'],
+                 env: pulumi.Input['CronJobDetailsCreateEnv'],
                  schedule: pulumi.Input[str],
                  env_specific_details: Optional[pulumi.Input[Union['DockerDetailsArgs', 'NativeEnvironmentDetailsArgs']]] = None,
-                 last_successful_run_at: Optional[pulumi.Input[str]] = None,
-                 plan: Optional[pulumi.Input['CronJobServiceDetailsPlan']] = None,
-                 region: Optional[pulumi.Input['CronJobServiceDetailsRegion']] = None):
+                 plan: Optional[pulumi.Input['CronJobDetailsCreatePlan']] = None,
+                 region: Optional[pulumi.Input['CronJobDetailsCreateRegion']] = None):
+        """
+        :param pulumi.Input['CronJobDetailsCreateEnv'] env: Environment (runtime)
+        """
         pulumi.set(__self__, "env", env)
         pulumi.set(__self__, "schedule", schedule)
         if env_specific_details is not None:
             pulumi.set(__self__, "env_specific_details", env_specific_details)
-        if last_successful_run_at is not None:
-            pulumi.set(__self__, "last_successful_run_at", last_successful_run_at)
-        if plan is None:
-            plan = 'starter'
         if plan is not None:
             pulumi.set(__self__, "plan", plan)
-        if region is None:
-            region = 'oregon'
         if region is not None:
             pulumi.set(__self__, "region", region)
 
     @property
     @pulumi.getter
-    def env(self) -> pulumi.Input['CronJobServiceDetailsEnv']:
+    def env(self) -> pulumi.Input['CronJobDetailsCreateEnv']:
+        """
+        Environment (runtime)
+        """
         return pulumi.get(self, "env")
 
     @env.setter
-    def env(self, value: pulumi.Input['CronJobServiceDetailsEnv']):
+    def env(self, value: pulumi.Input['CronJobDetailsCreateEnv']):
         pulumi.set(self, "env", value)
 
     @property
     @pulumi.getter
     def schedule(self) -> pulumi.Input[str]:
         return pulumi.get(self, "schedule")
 
@@ -293,92 +320,47 @@
         return pulumi.get(self, "env_specific_details")
 
     @env_specific_details.setter
     def env_specific_details(self, value: Optional[pulumi.Input[Union['DockerDetailsArgs', 'NativeEnvironmentDetailsArgs']]]):
         pulumi.set(self, "env_specific_details", value)
 
     @property
-    @pulumi.getter(name="lastSuccessfulRunAt")
-    def last_successful_run_at(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "last_successful_run_at")
-
-    @last_successful_run_at.setter
-    def last_successful_run_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "last_successful_run_at", value)
-
-    @property
     @pulumi.getter
-    def plan(self) -> Optional[pulumi.Input['CronJobServiceDetailsPlan']]:
+    def plan(self) -> Optional[pulumi.Input['CronJobDetailsCreatePlan']]:
         return pulumi.get(self, "plan")
 
     @plan.setter
-    def plan(self, value: Optional[pulumi.Input['CronJobServiceDetailsPlan']]):
+    def plan(self, value: Optional[pulumi.Input['CronJobDetailsCreatePlan']]):
         pulumi.set(self, "plan", value)
 
     @property
     @pulumi.getter
-    def region(self) -> Optional[pulumi.Input['CronJobServiceDetailsRegion']]:
+    def region(self) -> Optional[pulumi.Input['CronJobDetailsCreateRegion']]:
         return pulumi.get(self, "region")
 
     @region.setter
-    def region(self, value: Optional[pulumi.Input['CronJobServiceDetailsRegion']]):
+    def region(self, value: Optional[pulumi.Input['CronJobDetailsCreateRegion']]):
         pulumi.set(self, "region", value)
 
 
 @pulumi.input_type
-class DiskArgs:
-    def __init__(__self__, *,
-                 mount_path: pulumi.Input[str],
-                 name: pulumi.Input[str],
-                 size_gb: Optional[pulumi.Input[float]] = None):
-        pulumi.set(__self__, "mount_path", mount_path)
-        pulumi.set(__self__, "name", name)
-        if size_gb is None:
-            size_gb = 1
-        if size_gb is not None:
-            pulumi.set(__self__, "size_gb", size_gb)
-
-    @property
-    @pulumi.getter(name="mountPath")
-    def mount_path(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "mount_path")
-
-    @mount_path.setter
-    def mount_path(self, value: pulumi.Input[str]):
-        pulumi.set(self, "mount_path", value)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter(name="sizeGB")
-    def size_gb(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "size_gb")
-
-    @size_gb.setter
-    def size_gb(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "size_gb", value)
-
-
-@pulumi.input_type
 class DockerDetailsArgs:
     def __init__(__self__, *,
                  docker_command: pulumi.Input[str],
                  docker_context: pulumi.Input[str],
-                 dockerfile_path: Optional[pulumi.Input[str]] = None):
+                 dockerfile_path: pulumi.Input[str],
+                 pre_deploy_command: Optional[pulumi.Input[str]] = None,
+                 registry_credential: Optional[pulumi.Input['RegistryCredentialArgs']] = None):
         pulumi.set(__self__, "docker_command", docker_command)
         pulumi.set(__self__, "docker_context", docker_context)
-        if dockerfile_path is not None:
-            pulumi.set(__self__, "dockerfile_path", dockerfile_path)
+        pulumi.set(__self__, "dockerfile_path", dockerfile_path)
+        if pre_deploy_command is not None:
+            pulumi.set(__self__, "pre_deploy_command", pre_deploy_command)
+        if registry_credential is not None:
+            pulumi.set(__self__, "registry_credential", registry_credential)
 
     @property
     @pulumi.getter(name="dockerCommand")
     def docker_command(self) -> pulumi.Input[str]:
         return pulumi.get(self, "docker_command")
 
     @docker_command.setter
@@ -392,69 +374,209 @@
 
     @docker_context.setter
     def docker_context(self, value: pulumi.Input[str]):
         pulumi.set(self, "docker_context", value)
 
     @property
     @pulumi.getter(name="dockerfilePath")
-    def dockerfile_path(self) -> Optional[pulumi.Input[str]]:
+    def dockerfile_path(self) -> pulumi.Input[str]:
         return pulumi.get(self, "dockerfile_path")
 
     @dockerfile_path.setter
-    def dockerfile_path(self, value: Optional[pulumi.Input[str]]):
+    def dockerfile_path(self, value: pulumi.Input[str]):
         pulumi.set(self, "dockerfile_path", value)
 
+    @property
+    @pulumi.getter(name="preDeployCommand")
+    def pre_deploy_command(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "pre_deploy_command")
+
+    @pre_deploy_command.setter
+    def pre_deploy_command(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "pre_deploy_command", value)
+
+    @property
+    @pulumi.getter(name="registryCredential")
+    def registry_credential(self) -> Optional[pulumi.Input['RegistryCredentialArgs']]:
+        return pulumi.get(self, "registry_credential")
+
+    @registry_credential.setter
+    def registry_credential(self, value: Optional[pulumi.Input['RegistryCredentialArgs']]):
+        pulumi.set(self, "registry_credential", value)
+
+
+@pulumi.input_type
+class EnvVarKeyGenerateValueArgs:
+    def __init__(__self__, *,
+                 generate_value: pulumi.Input[bool],
+                 key: pulumi.Input[str]):
+        pulumi.set(__self__, "generate_value", generate_value)
+        pulumi.set(__self__, "key", key)
+
+    @property
+    @pulumi.getter(name="generateValue")
+    def generate_value(self) -> pulumi.Input[bool]:
+        return pulumi.get(self, "generate_value")
+
+    @generate_value.setter
+    def generate_value(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "generate_value", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "key")
+
+    @key.setter
+    def key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "key", value)
+
 
 @pulumi.input_type
 class EnvVarKeyValueArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
-                 generate_value: Optional[pulumi.Input['EnvVarKeyValueGenerateValue']] = None,
-                 value: Optional[pulumi.Input[str]] = None):
+                 value: pulumi.Input[str]):
         pulumi.set(__self__, "key", key)
-        if generate_value is not None:
-            pulumi.set(__self__, "generate_value", generate_value)
-        if value is not None:
-            pulumi.set(__self__, "value", value)
+        pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Input[str]:
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
     @property
-    @pulumi.getter(name="generateValue")
-    def generate_value(self) -> Optional[pulumi.Input['EnvVarKeyValueGenerateValue']]:
-        return pulumi.get(self, "generate_value")
+    @pulumi.getter
+    def value(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "value")
 
-    @generate_value.setter
-    def generate_value(self, value: Optional[pulumi.Input['EnvVarKeyValueGenerateValue']]):
-        pulumi.set(self, "generate_value", value)
+    @value.setter
+    def value(self, value: pulumi.Input[str]):
+        pulumi.set(self, "value", value)
+
+
+@pulumi.input_type
+class HeaderCreateArgs:
+    def __init__(__self__, *,
+                 name: pulumi.Input[str],
+                 path: pulumi.Input[str],
+                 value: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] name: Header name
+        :param pulumi.Input[str] path: The request path to add the header to. Wildcards will cause headers to be applied to all matching paths.
+        :param pulumi.Input[str] value: Header value
+        """
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "path", path)
+        pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
-    def value(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> pulumi.Input[str]:
+        """
+        Header name
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
+    def path(self) -> pulumi.Input[str]:
+        """
+        The request path to add the header to. Wildcards will cause headers to be applied to all matching paths.
+        """
+        return pulumi.get(self, "path")
+
+    @path.setter
+    def path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "path", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input[str]:
+        """
+        Header value
+        """
         return pulumi.get(self, "value")
 
     @value.setter
-    def value(self, value: Optional[pulumi.Input[str]]):
+    def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
 
 
 @pulumi.input_type
+class ImageArgs:
+    def __init__(__self__, *,
+                 image_path: pulumi.Input[str],
+                 owner_id: pulumi.Input[str],
+                 registry_credential_id: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] image_path: Path to the image used for this server (e.g docker.io/library/nginx:latest).
+        :param pulumi.Input[str] owner_id: The ID of the owner for this image. This should match the owner of the service as well as the owner of any specified registry credential.
+        :param pulumi.Input[str] registry_credential_id: Optional reference to the registry credential passed to the image repository to retrieve this image.
+        """
+        pulumi.set(__self__, "image_path", image_path)
+        pulumi.set(__self__, "owner_id", owner_id)
+        if registry_credential_id is not None:
+            pulumi.set(__self__, "registry_credential_id", registry_credential_id)
+
+    @property
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> pulumi.Input[str]:
+        """
+        Path to the image used for this server (e.g docker.io/library/nginx:latest).
+        """
+        return pulumi.get(self, "image_path")
+
+    @image_path.setter
+    def image_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "image_path", value)
+
+    @property
+    @pulumi.getter(name="ownerId")
+    def owner_id(self) -> pulumi.Input[str]:
+        """
+        The ID of the owner for this image. This should match the owner of the service as well as the owner of any specified registry credential.
+        """
+        return pulumi.get(self, "owner_id")
+
+    @owner_id.setter
+    def owner_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "owner_id", value)
+
+    @property
+    @pulumi.getter(name="registryCredentialId")
+    def registry_credential_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        Optional reference to the registry credential passed to the image repository to retrieve this image.
+        """
+        return pulumi.get(self, "registry_credential_id")
+
+    @registry_credential_id.setter
+    def registry_credential_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "registry_credential_id", value)
+
+
+@pulumi.input_type
 class NativeEnvironmentDetailsArgs:
     def __init__(__self__, *,
                  build_command: pulumi.Input[str],
-                 start_command: pulumi.Input[str]):
+                 start_command: pulumi.Input[str],
+                 pre_deploy_command: Optional[pulumi.Input[str]] = None):
         pulumi.set(__self__, "build_command", build_command)
         pulumi.set(__self__, "start_command", start_command)
+        if pre_deploy_command is not None:
+            pulumi.set(__self__, "pre_deploy_command", pre_deploy_command)
 
     @property
     @pulumi.getter(name="buildCommand")
     def build_command(self) -> pulumi.Input[str]:
         return pulumi.get(self, "build_command")
 
     @build_command.setter
@@ -466,531 +588,510 @@
     def start_command(self) -> pulumi.Input[str]:
         return pulumi.get(self, "start_command")
 
     @start_command.setter
     def start_command(self, value: pulumi.Input[str]):
         pulumi.set(self, "start_command", value)
 
-
-@pulumi.input_type
-class OpenPortsArgs:
-    def __init__(__self__, *,
-                 port: Optional[pulumi.Input[float]] = None,
-                 protocol: Optional[pulumi.Input['OpenPortsProtocol']] = None):
-        if port is not None:
-            pulumi.set(__self__, "port", port)
-        if protocol is not None:
-            pulumi.set(__self__, "protocol", protocol)
-
     @property
-    @pulumi.getter
-    def port(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "port")
-
-    @port.setter
-    def port(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "port", value)
-
-    @property
-    @pulumi.getter
-    def protocol(self) -> Optional[pulumi.Input['OpenPortsProtocol']]:
-        return pulumi.get(self, "protocol")
-
-    @protocol.setter
-    def protocol(self, value: Optional[pulumi.Input['OpenPortsProtocol']]):
-        pulumi.set(self, "protocol", value)
+    @pulumi.getter(name="preDeployCommand")
+    def pre_deploy_command(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "pre_deploy_command")
+
+    @pre_deploy_command.setter
+    def pre_deploy_command(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "pre_deploy_command", value)
 
 
 @pulumi.input_type
-class PrivateServiceDetailsParentServerPropertiesArgs:
+class PrivateServiceDetailsCreateDiskPropertiesArgs:
     def __init__(__self__, *,
-                 id: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+                 mount_path: pulumi.Input[str],
+                 name: pulumi.Input[str],
+                 size_gb: Optional[pulumi.Input[int]] = None):
+        """
+        :param pulumi.Input[int] size_gb: Defaults to 1
+        """
+        pulumi.set(__self__, "mount_path", mount_path)
+        pulumi.set(__self__, "name", name)
+        if size_gb is not None:
+            pulumi.set(__self__, "size_gb", size_gb)
 
     @property
-    @pulumi.getter
-    def id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "id")
+    @pulumi.getter(name="mountPath")
+    def mount_path(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "mount_path")
 
-    @id.setter
-    def id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "id", value)
+    @mount_path.setter
+    def mount_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "mount_path", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "name")
 
     @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
+    def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
+    @property
+    @pulumi.getter(name="sizeGB")
+    def size_gb(self) -> Optional[pulumi.Input[int]]:
+        """
+        Defaults to 1
+        """
+        return pulumi.get(self, "size_gb")
+
+    @size_gb.setter
+    def size_gb(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "size_gb", value)
+
 
 @pulumi.input_type
-class PrivateServiceDetailsArgs:
+class PrivateServiceDetailsCreateArgs:
     def __init__(__self__, *,
-                 env: pulumi.Input['PrivateServiceDetailsEnv'],
-                 disk: Optional[pulumi.Input['DiskArgs']] = None,
+                 env: pulumi.Input['PrivateServiceDetailsCreateEnv'],
+                 disk: Optional[pulumi.Input['PrivateServiceDetailsCreateDiskPropertiesArgs']] = None,
                  env_specific_details: Optional[pulumi.Input[Union['DockerDetailsArgs', 'NativeEnvironmentDetailsArgs']]] = None,
-                 num_instances: Optional[pulumi.Input[float]] = None,
-                 open_ports: Optional[pulumi.Input[Sequence[pulumi.Input['OpenPortsArgs']]]] = None,
-                 parent_server: Optional[pulumi.Input['PrivateServiceDetailsParentServerPropertiesArgs']] = None,
-                 plan: Optional[pulumi.Input['PrivateServiceDetailsPlan']] = None,
-                 pull_request_previews_enabled: Optional[pulumi.Input['PrivateServiceDetailsPullRequestPreviewsEnabled']] = None,
-                 region: Optional[pulumi.Input['PrivateServiceDetailsRegion']] = None,
-                 url: Optional[pulumi.Input[str]] = None):
+                 num_instances: Optional[pulumi.Input[int]] = None,
+                 plan: Optional[pulumi.Input['PrivateServiceDetailsCreatePlan']] = None,
+                 pull_request_previews_enabled: Optional[pulumi.Input['PrivateServiceDetailsCreatePullRequestPreviewsEnabled']] = None,
+                 region: Optional[pulumi.Input['PrivateServiceDetailsCreateRegion']] = None):
+        """
+        :param pulumi.Input['PrivateServiceDetailsCreateEnv'] env: Environment (runtime)
+        :param pulumi.Input[int] num_instances: Defaults to 1
+        :param pulumi.Input['PrivateServiceDetailsCreatePullRequestPreviewsEnabled'] pull_request_previews_enabled: Defaults to "no"
+        """
         pulumi.set(__self__, "env", env)
         if disk is not None:
             pulumi.set(__self__, "disk", disk)
         if env_specific_details is not None:
             pulumi.set(__self__, "env_specific_details", env_specific_details)
         if num_instances is None:
             num_instances = 1
         if num_instances is not None:
             pulumi.set(__self__, "num_instances", num_instances)
-        if open_ports is not None:
-            pulumi.set(__self__, "open_ports", open_ports)
-        if parent_server is not None:
-            pulumi.set(__self__, "parent_server", parent_server)
-        if plan is None:
-            plan = 'starter'
         if plan is not None:
             pulumi.set(__self__, "plan", plan)
         if pull_request_previews_enabled is None:
             pull_request_previews_enabled = 'no'
         if pull_request_previews_enabled is not None:
             pulumi.set(__self__, "pull_request_previews_enabled", pull_request_previews_enabled)
-        if region is None:
-            region = 'oregon'
         if region is not None:
             pulumi.set(__self__, "region", region)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
-    def env(self) -> pulumi.Input['PrivateServiceDetailsEnv']:
+    def env(self) -> pulumi.Input['PrivateServiceDetailsCreateEnv']:
+        """
+        Environment (runtime)
+        """
         return pulumi.get(self, "env")
 
     @env.setter
-    def env(self, value: pulumi.Input['PrivateServiceDetailsEnv']):
+    def env(self, value: pulumi.Input['PrivateServiceDetailsCreateEnv']):
         pulumi.set(self, "env", value)
 
     @property
     @pulumi.getter
-    def disk(self) -> Optional[pulumi.Input['DiskArgs']]:
+    def disk(self) -> Optional[pulumi.Input['PrivateServiceDetailsCreateDiskPropertiesArgs']]:
         return pulumi.get(self, "disk")
 
     @disk.setter
-    def disk(self, value: Optional[pulumi.Input['DiskArgs']]):
+    def disk(self, value: Optional[pulumi.Input['PrivateServiceDetailsCreateDiskPropertiesArgs']]):
         pulumi.set(self, "disk", value)
 
     @property
     @pulumi.getter(name="envSpecificDetails")
     def env_specific_details(self) -> Optional[pulumi.Input[Union['DockerDetailsArgs', 'NativeEnvironmentDetailsArgs']]]:
         return pulumi.get(self, "env_specific_details")
 
     @env_specific_details.setter
     def env_specific_details(self, value: Optional[pulumi.Input[Union['DockerDetailsArgs', 'NativeEnvironmentDetailsArgs']]]):
         pulumi.set(self, "env_specific_details", value)
 
     @property
     @pulumi.getter(name="numInstances")
-    def num_instances(self) -> Optional[pulumi.Input[float]]:
+    def num_instances(self) -> Optional[pulumi.Input[int]]:
+        """
+        Defaults to 1
+        """
         return pulumi.get(self, "num_instances")
 
     @num_instances.setter
-    def num_instances(self, value: Optional[pulumi.Input[float]]):
+    def num_instances(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "num_instances", value)
 
     @property
-    @pulumi.getter(name="openPorts")
-    def open_ports(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['OpenPortsArgs']]]]:
-        return pulumi.get(self, "open_ports")
-
-    @open_ports.setter
-    def open_ports(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['OpenPortsArgs']]]]):
-        pulumi.set(self, "open_ports", value)
-
-    @property
-    @pulumi.getter(name="parentServer")
-    def parent_server(self) -> Optional[pulumi.Input['PrivateServiceDetailsParentServerPropertiesArgs']]:
-        return pulumi.get(self, "parent_server")
-
-    @parent_server.setter
-    def parent_server(self, value: Optional[pulumi.Input['PrivateServiceDetailsParentServerPropertiesArgs']]):
-        pulumi.set(self, "parent_server", value)
-
-    @property
     @pulumi.getter
-    def plan(self) -> Optional[pulumi.Input['PrivateServiceDetailsPlan']]:
+    def plan(self) -> Optional[pulumi.Input['PrivateServiceDetailsCreatePlan']]:
         return pulumi.get(self, "plan")
 
     @plan.setter
-    def plan(self, value: Optional[pulumi.Input['PrivateServiceDetailsPlan']]):
+    def plan(self, value: Optional[pulumi.Input['PrivateServiceDetailsCreatePlan']]):
         pulumi.set(self, "plan", value)
 
     @property
     @pulumi.getter(name="pullRequestPreviewsEnabled")
-    def pull_request_previews_enabled(self) -> Optional[pulumi.Input['PrivateServiceDetailsPullRequestPreviewsEnabled']]:
+    def pull_request_previews_enabled(self) -> Optional[pulumi.Input['PrivateServiceDetailsCreatePullRequestPreviewsEnabled']]:
+        """
+        Defaults to "no"
+        """
         return pulumi.get(self, "pull_request_previews_enabled")
 
     @pull_request_previews_enabled.setter
-    def pull_request_previews_enabled(self, value: Optional[pulumi.Input['PrivateServiceDetailsPullRequestPreviewsEnabled']]):
+    def pull_request_previews_enabled(self, value: Optional[pulumi.Input['PrivateServiceDetailsCreatePullRequestPreviewsEnabled']]):
         pulumi.set(self, "pull_request_previews_enabled", value)
 
     @property
     @pulumi.getter
-    def region(self) -> Optional[pulumi.Input['PrivateServiceDetailsRegion']]:
+    def region(self) -> Optional[pulumi.Input['PrivateServiceDetailsCreateRegion']]:
         return pulumi.get(self, "region")
 
     @region.setter
-    def region(self, value: Optional[pulumi.Input['PrivateServiceDetailsRegion']]):
+    def region(self, value: Optional[pulumi.Input['PrivateServiceDetailsCreateRegion']]):
         pulumi.set(self, "region", value)
 
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "url")
-
-    @url.setter
-    def url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "url", value)
-
 
 @pulumi.input_type
-class SecretFileArgs:
+class RegistryCredentialArgs:
     def __init__(__self__, *,
-                 contents: pulumi.Input[str],
-                 name: pulumi.Input[str]):
-        pulumi.set(__self__, "contents", contents)
+                 id: pulumi.Input[str],
+                 name: pulumi.Input[str],
+                 registry: pulumi.Input['RegistryCredentialRegistry'],
+                 username: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] id: Unique identifier for this credential
+        :param pulumi.Input[str] name: Descriptive name for this credential
+        :param pulumi.Input['RegistryCredentialRegistry'] registry: The registry to use this credential with
+        :param pulumi.Input[str] username: The username associated with the credential
+        """
+        pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "registry", registry)
+        pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
-    def contents(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "contents")
+    def id(self) -> pulumi.Input[str]:
+        """
+        Unique identifier for this credential
+        """
+        return pulumi.get(self, "id")
 
-    @contents.setter
-    def contents(self, value: pulumi.Input[str]):
-        pulumi.set(self, "contents", value)
+    @id.setter
+    def id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-
-@pulumi.input_type
-class ServiceHeaderArgs:
-    def __init__(__self__, *,
-                 name: pulumi.Input[str],
-                 path: pulumi.Input[str],
-                 value: pulumi.Input[str]):
         """
-        A service header object
+        Descriptive name for this credential
         """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "path", path)
-        pulumi.set(__self__, "value", value)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def path(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "path")
+    def registry(self) -> pulumi.Input['RegistryCredentialRegistry']:
+        """
+        The registry to use this credential with
+        """
+        return pulumi.get(self, "registry")
 
-    @path.setter
-    def path(self, value: pulumi.Input[str]):
-        pulumi.set(self, "path", value)
+    @registry.setter
+    def registry(self, value: pulumi.Input['RegistryCredentialRegistry']):
+        pulumi.set(self, "registry", value)
 
     @property
     @pulumi.getter
-    def value(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "value")
+    def username(self) -> pulumi.Input[str]:
+        """
+        The username associated with the credential
+        """
+        return pulumi.get(self, "username")
 
-    @value.setter
-    def value(self, value: pulumi.Input[str]):
-        pulumi.set(self, "value", value)
+    @username.setter
+    def username(self, value: pulumi.Input[str]):
+        pulumi.set(self, "username", value)
 
 
 @pulumi.input_type
-class StaticSiteRouteArgs:
+class RouteArgs:
     def __init__(__self__, *,
                  destination: pulumi.Input[str],
+                 id: pulumi.Input[str],
+                 priority: pulumi.Input[int],
                  source: pulumi.Input[str],
-                 type: pulumi.Input['StaticSiteRouteType']):
+                 type: pulumi.Input['RouteType']):
         """
-        A route object for a static site
+        :param pulumi.Input[int] priority: Redirect and Rewrite Rules are applied in priority order starting at 0
         """
         pulumi.set(__self__, "destination", destination)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "priority", priority)
         pulumi.set(__self__, "source", source)
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def destination(self) -> pulumi.Input[str]:
         return pulumi.get(self, "destination")
 
     @destination.setter
     def destination(self, value: pulumi.Input[str]):
         pulumi.set(self, "destination", value)
 
     @property
     @pulumi.getter
+    def id(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def priority(self) -> pulumi.Input[int]:
+        """
+        Redirect and Rewrite Rules are applied in priority order starting at 0
+        """
+        return pulumi.get(self, "priority")
+
+    @priority.setter
+    def priority(self, value: pulumi.Input[int]):
+        pulumi.set(self, "priority", value)
+
+    @property
+    @pulumi.getter
     def source(self) -> pulumi.Input[str]:
         return pulumi.get(self, "source")
 
     @source.setter
     def source(self, value: pulumi.Input[str]):
         pulumi.set(self, "source", value)
 
     @property
     @pulumi.getter
-    def type(self) -> pulumi.Input['StaticSiteRouteType']:
+    def type(self) -> pulumi.Input['RouteType']:
         return pulumi.get(self, "type")
 
     @type.setter
-    def type(self, value: pulumi.Input['StaticSiteRouteType']):
+    def type(self, value: pulumi.Input['RouteType']):
         pulumi.set(self, "type", value)
 
 
 @pulumi.input_type
-class StaticSiteServiceDetailsParentServerPropertiesArgs:
+class SecretFileArgs:
     def __init__(__self__, *,
-                 id: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+                 id: pulumi.Input[str],
+                 name: pulumi.Input[str]):
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
-    def id(self) -> Optional[pulumi.Input[str]]:
+    def id(self) -> pulumi.Input[str]:
         return pulumi.get(self, "id")
 
     @id.setter
-    def id(self, value: Optional[pulumi.Input[str]]):
+    def id(self, value: pulumi.Input[str]):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "name")
 
     @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
+    def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
-class StaticSiteServiceDetailsArgs:
+class StaticSiteDetailsCreateArgs:
     def __init__(__self__, *,
                  build_command: Optional[pulumi.Input[str]] = None,
-                 headers: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceHeaderArgs']]]] = None,
-                 parent_server: Optional[pulumi.Input['StaticSiteServiceDetailsParentServerPropertiesArgs']] = None,
+                 headers: Optional[pulumi.Input[Sequence[pulumi.Input['HeaderCreateArgs']]]] = None,
                  publish_path: Optional[pulumi.Input[str]] = None,
-                 pull_request_previews_enabled: Optional[pulumi.Input['StaticSiteServiceDetailsPullRequestPreviewsEnabled']] = None,
-                 routes: Optional[pulumi.Input[Sequence[pulumi.Input['StaticSiteRouteArgs']]]] = None,
-                 url: Optional[pulumi.Input[str]] = None):
+                 pull_request_previews_enabled: Optional[pulumi.Input['StaticSiteDetailsCreatePullRequestPreviewsEnabled']] = None,
+                 routes: Optional[pulumi.Input[Sequence[pulumi.Input['RouteArgs']]]] = None):
         """
-        :param pulumi.Input[str] url: The HTTPS service URL. A subdomain of onrender.com, by default.
+        :param pulumi.Input[str] publish_path: Defaults to "public"
+        :param pulumi.Input['StaticSiteDetailsCreatePullRequestPreviewsEnabled'] pull_request_previews_enabled: Defaults to "no"
         """
         if build_command is not None:
             pulumi.set(__self__, "build_command", build_command)
         if headers is not None:
             pulumi.set(__self__, "headers", headers)
-        if parent_server is not None:
-            pulumi.set(__self__, "parent_server", parent_server)
-        if publish_path is None:
-            publish_path = 'public'
         if publish_path is not None:
             pulumi.set(__self__, "publish_path", publish_path)
         if pull_request_previews_enabled is None:
             pull_request_previews_enabled = 'no'
         if pull_request_previews_enabled is not None:
             pulumi.set(__self__, "pull_request_previews_enabled", pull_request_previews_enabled)
         if routes is not None:
             pulumi.set(__self__, "routes", routes)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter(name="buildCommand")
     def build_command(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "build_command")
 
     @build_command.setter
     def build_command(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "build_command", value)
 
     @property
     @pulumi.getter
-    def headers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceHeaderArgs']]]]:
+    def headers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['HeaderCreateArgs']]]]:
         return pulumi.get(self, "headers")
 
     @headers.setter
-    def headers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceHeaderArgs']]]]):
+    def headers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['HeaderCreateArgs']]]]):
         pulumi.set(self, "headers", value)
 
     @property
-    @pulumi.getter(name="parentServer")
-    def parent_server(self) -> Optional[pulumi.Input['StaticSiteServiceDetailsParentServerPropertiesArgs']]:
-        return pulumi.get(self, "parent_server")
-
-    @parent_server.setter
-    def parent_server(self, value: Optional[pulumi.Input['StaticSiteServiceDetailsParentServerPropertiesArgs']]):
-        pulumi.set(self, "parent_server", value)
-
-    @property
     @pulumi.getter(name="publishPath")
     def publish_path(self) -> Optional[pulumi.Input[str]]:
+        """
+        Defaults to "public"
+        """
         return pulumi.get(self, "publish_path")
 
     @publish_path.setter
     def publish_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "publish_path", value)
 
     @property
     @pulumi.getter(name="pullRequestPreviewsEnabled")
-    def pull_request_previews_enabled(self) -> Optional[pulumi.Input['StaticSiteServiceDetailsPullRequestPreviewsEnabled']]:
+    def pull_request_previews_enabled(self) -> Optional[pulumi.Input['StaticSiteDetailsCreatePullRequestPreviewsEnabled']]:
+        """
+        Defaults to "no"
+        """
         return pulumi.get(self, "pull_request_previews_enabled")
 
     @pull_request_previews_enabled.setter
-    def pull_request_previews_enabled(self, value: Optional[pulumi.Input['StaticSiteServiceDetailsPullRequestPreviewsEnabled']]):
+    def pull_request_previews_enabled(self, value: Optional[pulumi.Input['StaticSiteDetailsCreatePullRequestPreviewsEnabled']]):
         pulumi.set(self, "pull_request_previews_enabled", value)
 
     @property
     @pulumi.getter
-    def routes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['StaticSiteRouteArgs']]]]:
+    def routes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RouteArgs']]]]:
         return pulumi.get(self, "routes")
 
     @routes.setter
-    def routes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['StaticSiteRouteArgs']]]]):
+    def routes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RouteArgs']]]]):
         pulumi.set(self, "routes", value)
 
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[pulumi.Input[str]]:
-        """
-        The HTTPS service URL. A subdomain of onrender.com, by default.
-        """
-        return pulumi.get(self, "url")
-
-    @url.setter
-    def url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "url", value)
-
 
 @pulumi.input_type
-class WebServiceServiceDetailsParentServerPropertiesArgs:
+class WebServiceDetailsCreateDiskPropertiesArgs:
     def __init__(__self__, *,
-                 id: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+                 mount_path: pulumi.Input[str],
+                 name: pulumi.Input[str],
+                 size_gb: Optional[pulumi.Input[int]] = None):
+        """
+        :param pulumi.Input[int] size_gb: Defaults to 1
+        """
+        pulumi.set(__self__, "mount_path", mount_path)
+        pulumi.set(__self__, "name", name)
+        if size_gb is not None:
+            pulumi.set(__self__, "size_gb", size_gb)
 
     @property
-    @pulumi.getter
-    def id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "id")
+    @pulumi.getter(name="mountPath")
+    def mount_path(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "mount_path")
 
-    @id.setter
-    def id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "id", value)
+    @mount_path.setter
+    def mount_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "mount_path", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "name")
 
     @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
+    def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
+    @property
+    @pulumi.getter(name="sizeGB")
+    def size_gb(self) -> Optional[pulumi.Input[int]]:
+        """
+        Defaults to 1
+        """
+        return pulumi.get(self, "size_gb")
+
+    @size_gb.setter
+    def size_gb(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "size_gb", value)
+
 
 @pulumi.input_type
-class WebServiceServiceDetailsArgs:
+class WebServiceDetailsCreateArgs:
     def __init__(__self__, *,
-                 env: pulumi.Input['WebServiceServiceDetailsEnv'],
-                 disk: Optional[pulumi.Input['DiskArgs']] = None,
+                 env: pulumi.Input['WebServiceDetailsCreateEnv'],
+                 disk: Optional[pulumi.Input['WebServiceDetailsCreateDiskPropertiesArgs']] = None,
                  env_specific_details: Optional[pulumi.Input[Union['DockerDetailsArgs', 'NativeEnvironmentDetailsArgs']]] = None,
                  health_check_path: Optional[pulumi.Input[str]] = None,
-                 num_instances: Optional[pulumi.Input[float]] = None,
-                 open_ports: Optional[pulumi.Input[Sequence[pulumi.Input['OpenPortsArgs']]]] = None,
-                 parent_server: Optional[pulumi.Input['WebServiceServiceDetailsParentServerPropertiesArgs']] = None,
-                 plan: Optional[pulumi.Input['WebServiceServiceDetailsPlan']] = None,
-                 pull_request_previews_enabled: Optional[pulumi.Input['WebServiceServiceDetailsPullRequestPreviewsEnabled']] = None,
-                 region: Optional[pulumi.Input['WebServiceServiceDetailsRegion']] = None,
-                 url: Optional[pulumi.Input[str]] = None):
+                 num_instances: Optional[pulumi.Input[int]] = None,
+                 plan: Optional[pulumi.Input['WebServiceDetailsCreatePlan']] = None,
+                 pull_request_previews_enabled: Optional[pulumi.Input['WebServiceDetailsCreatePullRequestPreviewsEnabled']] = None,
+                 region: Optional[pulumi.Input['WebServiceDetailsCreateRegion']] = None):
+        """
+        :param pulumi.Input['WebServiceDetailsCreateEnv'] env: Environment (runtime)
+        :param pulumi.Input[int] num_instances: Defaults to 1
+        :param pulumi.Input['WebServiceDetailsCreatePullRequestPreviewsEnabled'] pull_request_previews_enabled: Defaults to "no"
+        """
         pulumi.set(__self__, "env", env)
         if disk is not None:
             pulumi.set(__self__, "disk", disk)
         if env_specific_details is not None:
             pulumi.set(__self__, "env_specific_details", env_specific_details)
         if health_check_path is not None:
             pulumi.set(__self__, "health_check_path", health_check_path)
-        if num_instances is None:
-            num_instances = 1
         if num_instances is not None:
             pulumi.set(__self__, "num_instances", num_instances)
-        if open_ports is not None:
-            pulumi.set(__self__, "open_ports", open_ports)
-        if parent_server is not None:
-            pulumi.set(__self__, "parent_server", parent_server)
-        if plan is None:
-            plan = 'starter'
         if plan is not None:
             pulumi.set(__self__, "plan", plan)
         if pull_request_previews_enabled is None:
             pull_request_previews_enabled = 'no'
         if pull_request_previews_enabled is not None:
             pulumi.set(__self__, "pull_request_previews_enabled", pull_request_previews_enabled)
-        if region is None:
-            region = 'oregon'
         if region is not None:
             pulumi.set(__self__, "region", region)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
-    def env(self) -> pulumi.Input['WebServiceServiceDetailsEnv']:
+    def env(self) -> pulumi.Input['WebServiceDetailsCreateEnv']:
+        """
+        Environment (runtime)
+        """
         return pulumi.get(self, "env")
 
     @env.setter
-    def env(self, value: pulumi.Input['WebServiceServiceDetailsEnv']):
+    def env(self, value: pulumi.Input['WebServiceDetailsCreateEnv']):
         pulumi.set(self, "env", value)
 
     @property
     @pulumi.getter
-    def disk(self) -> Optional[pulumi.Input['DiskArgs']]:
+    def disk(self) -> Optional[pulumi.Input['WebServiceDetailsCreateDiskPropertiesArgs']]:
         return pulumi.get(self, "disk")
 
     @disk.setter
-    def disk(self, value: Optional[pulumi.Input['DiskArgs']]):
+    def disk(self, value: Optional[pulumi.Input['WebServiceDetailsCreateDiskPropertiesArgs']]):
         pulumi.set(self, "disk", value)
 
     @property
     @pulumi.getter(name="envSpecificDetails")
     def env_specific_details(self) -> Optional[pulumi.Input[Union['DockerDetailsArgs', 'NativeEnvironmentDetailsArgs']]]:
         return pulumi.get(self, "env_specific_details")
 
@@ -1005,69 +1106,48 @@
 
     @health_check_path.setter
     def health_check_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "health_check_path", value)
 
     @property
     @pulumi.getter(name="numInstances")
-    def num_instances(self) -> Optional[pulumi.Input[float]]:
+    def num_instances(self) -> Optional[pulumi.Input[int]]:
+        """
+        Defaults to 1
+        """
         return pulumi.get(self, "num_instances")
 
     @num_instances.setter
-    def num_instances(self, value: Optional[pulumi.Input[float]]):
+    def num_instances(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "num_instances", value)
 
     @property
-    @pulumi.getter(name="openPorts")
-    def open_ports(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['OpenPortsArgs']]]]:
-        return pulumi.get(self, "open_ports")
-
-    @open_ports.setter
-    def open_ports(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['OpenPortsArgs']]]]):
-        pulumi.set(self, "open_ports", value)
-
-    @property
-    @pulumi.getter(name="parentServer")
-    def parent_server(self) -> Optional[pulumi.Input['WebServiceServiceDetailsParentServerPropertiesArgs']]:
-        return pulumi.get(self, "parent_server")
-
-    @parent_server.setter
-    def parent_server(self, value: Optional[pulumi.Input['WebServiceServiceDetailsParentServerPropertiesArgs']]):
-        pulumi.set(self, "parent_server", value)
-
-    @property
     @pulumi.getter
-    def plan(self) -> Optional[pulumi.Input['WebServiceServiceDetailsPlan']]:
+    def plan(self) -> Optional[pulumi.Input['WebServiceDetailsCreatePlan']]:
         return pulumi.get(self, "plan")
 
     @plan.setter
-    def plan(self, value: Optional[pulumi.Input['WebServiceServiceDetailsPlan']]):
+    def plan(self, value: Optional[pulumi.Input['WebServiceDetailsCreatePlan']]):
         pulumi.set(self, "plan", value)
 
     @property
     @pulumi.getter(name="pullRequestPreviewsEnabled")
-    def pull_request_previews_enabled(self) -> Optional[pulumi.Input['WebServiceServiceDetailsPullRequestPreviewsEnabled']]:
+    def pull_request_previews_enabled(self) -> Optional[pulumi.Input['WebServiceDetailsCreatePullRequestPreviewsEnabled']]:
+        """
+        Defaults to "no"
+        """
         return pulumi.get(self, "pull_request_previews_enabled")
 
     @pull_request_previews_enabled.setter
-    def pull_request_previews_enabled(self, value: Optional[pulumi.Input['WebServiceServiceDetailsPullRequestPreviewsEnabled']]):
+    def pull_request_previews_enabled(self, value: Optional[pulumi.Input['WebServiceDetailsCreatePullRequestPreviewsEnabled']]):
         pulumi.set(self, "pull_request_previews_enabled", value)
 
     @property
     @pulumi.getter
-    def region(self) -> Optional[pulumi.Input['WebServiceServiceDetailsRegion']]:
+    def region(self) -> Optional[pulumi.Input['WebServiceDetailsCreateRegion']]:
         return pulumi.get(self, "region")
 
     @region.setter
-    def region(self, value: Optional[pulumi.Input['WebServiceServiceDetailsRegion']]):
+    def region(self, value: Optional[pulumi.Input['WebServiceDetailsCreateRegion']]):
         pulumi.set(self, "region", value)
 
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "url")
-
-    @url.setter
-    def url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "url", value)
-
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/auto_scaling.py` & `pulumi_render-0.2.0/pulumi_render/services/cancel_deploy.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,206 +5,178 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
-from ._inputs import *
+from ._enums import *
 
-__all__ = ['AutoScalingArgs', 'AutoScaling']
+__all__ = ['CancelDeployArgs', 'CancelDeploy']
 
 @pulumi.input_type
-class AutoScalingArgs:
+class CancelDeployArgs:
     def __init__(__self__, *,
-                 criteria: Optional[pulumi.Input['AutoScalingCriteriaArgs']] = None,
-                 enabled: Optional[pulumi.Input[bool]] = None,
-                 max: Optional[pulumi.Input[float]] = None,
-                 min: Optional[pulumi.Input[float]] = None,
+                 deploy_id: Optional[pulumi.Input[str]] = None,
                  service_id: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a AutoScaling resource.
-        :param pulumi.Input[float] max: The maximum number of instances for the service
-        :param pulumi.Input[float] min: The minimum number of instances for the service
-        :param pulumi.Input[str] service_id: (Required) The ID of the service
-        """
-        if criteria is not None:
-            pulumi.set(__self__, "criteria", criteria)
-        if enabled is not None:
-            pulumi.set(__self__, "enabled", enabled)
-        if max is not None:
-            pulumi.set(__self__, "max", max)
-        if min is not None:
-            pulumi.set(__self__, "min", min)
+        The set of arguments for constructing a CancelDeploy resource.
+        :param pulumi.Input[str] deploy_id: The ID of the deploy
+        :param pulumi.Input[str] service_id: The ID of the service
+        """
+        if deploy_id is not None:
+            pulumi.set(__self__, "deploy_id", deploy_id)
         if service_id is not None:
             pulumi.set(__self__, "service_id", service_id)
 
     @property
-    @pulumi.getter
-    def criteria(self) -> Optional[pulumi.Input['AutoScalingCriteriaArgs']]:
-        return pulumi.get(self, "criteria")
-
-    @criteria.setter
-    def criteria(self, value: Optional[pulumi.Input['AutoScalingCriteriaArgs']]):
-        pulumi.set(self, "criteria", value)
-
-    @property
-    @pulumi.getter
-    def enabled(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "enabled")
-
-    @enabled.setter
-    def enabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "enabled", value)
-
-    @property
-    @pulumi.getter
-    def max(self) -> Optional[pulumi.Input[float]]:
-        """
-        The maximum number of instances for the service
-        """
-        return pulumi.get(self, "max")
-
-    @max.setter
-    def max(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "max", value)
-
-    @property
-    @pulumi.getter
-    def min(self) -> Optional[pulumi.Input[float]]:
+    @pulumi.getter(name="deployId")
+    def deploy_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The minimum number of instances for the service
+        The ID of the deploy
         """
-        return pulumi.get(self, "min")
+        return pulumi.get(self, "deploy_id")
 
-    @min.setter
-    def min(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "min", value)
+    @deploy_id.setter
+    def deploy_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "deploy_id", value)
 
     @property
     @pulumi.getter(name="serviceId")
     def service_id(self) -> Optional[pulumi.Input[str]]:
         """
-        (Required) The ID of the service
+        The ID of the service
         """
         return pulumi.get(self, "service_id")
 
     @service_id.setter
     def service_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_id", value)
 
 
-class AutoScaling(pulumi.CustomResource):
+class CancelDeploy(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 criteria: Optional[pulumi.Input[pulumi.InputType['AutoScalingCriteriaArgs']]] = None,
-                 enabled: Optional[pulumi.Input[bool]] = None,
-                 max: Optional[pulumi.Input[float]] = None,
-                 min: Optional[pulumi.Input[float]] = None,
+                 deploy_id: Optional[pulumi.Input[str]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a AutoScaling resource with the given unique name, props, and options.
+        Create a CancelDeploy resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[float] max: The maximum number of instances for the service
-        :param pulumi.Input[float] min: The minimum number of instances for the service
-        :param pulumi.Input[str] service_id: (Required) The ID of the service
+        :param pulumi.Input[str] deploy_id: The ID of the deploy
+        :param pulumi.Input[str] service_id: The ID of the service
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[AutoScalingArgs] = None,
+                 args: Optional[CancelDeployArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a AutoScaling resource with the given unique name, props, and options.
+        Create a CancelDeploy resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param AutoScalingArgs args: The arguments to use to populate this resource's properties.
+        :param CancelDeployArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(AutoScalingArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(CancelDeployArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 criteria: Optional[pulumi.Input[pulumi.InputType['AutoScalingCriteriaArgs']]] = None,
-                 enabled: Optional[pulumi.Input[bool]] = None,
-                 max: Optional[pulumi.Input[float]] = None,
-                 min: Optional[pulumi.Input[float]] = None,
+                 deploy_id: Optional[pulumi.Input[str]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = AutoScalingArgs.__new__(AutoScalingArgs)
+            __props__ = CancelDeployArgs.__new__(CancelDeployArgs)
 
-            __props__.__dict__["criteria"] = criteria
-            __props__.__dict__["enabled"] = enabled
-            __props__.__dict__["max"] = max
-            __props__.__dict__["min"] = min
+            __props__.__dict__["deploy_id"] = deploy_id
             __props__.__dict__["service_id"] = service_id
-        super(AutoScaling, __self__).__init__(
-            'render:services:AutoScaling',
+            __props__.__dict__["commit"] = None
+            __props__.__dict__["created_at"] = None
+            __props__.__dict__["finished_at"] = None
+            __props__.__dict__["image"] = None
+            __props__.__dict__["status"] = None
+            __props__.__dict__["trigger"] = None
+            __props__.__dict__["updated_at"] = None
+        super(CancelDeploy, __self__).__init__(
+            'render:services:CancelDeploy',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'AutoScaling':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'CancelDeploy':
         """
-        Get an existing AutoScaling resource's state with the given name, id, and optional extra
+        Get an existing CancelDeploy resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = AutoScalingArgs.__new__(AutoScalingArgs)
+        __props__ = CancelDeployArgs.__new__(CancelDeployArgs)
 
-        __props__.__dict__["criteria"] = None
-        __props__.__dict__["enabled"] = None
-        __props__.__dict__["max"] = None
-        __props__.__dict__["min"] = None
-        return AutoScaling(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["commit"] = None
+        __props__.__dict__["created_at"] = None
+        __props__.__dict__["finished_at"] = None
+        __props__.__dict__["image"] = None
+        __props__.__dict__["status"] = None
+        __props__.__dict__["trigger"] = None
+        __props__.__dict__["updated_at"] = None
+        return CancelDeploy(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def criteria(self) -> pulumi.Output[Optional['outputs.AutoScalingCriteria']]:
-        return pulumi.get(self, "criteria")
+    def commit(self) -> pulumi.Output[Optional['outputs.CommitProperties']]:
+        return pulumi.get(self, "commit")
 
     @property
-    @pulumi.getter
-    def enabled(self) -> pulumi.Output[Optional[bool]]:
-        return pulumi.get(self, "enabled")
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "created_at")
+
+    @property
+    @pulumi.getter(name="finishedAt")
+    def finished_at(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "finished_at")
 
     @property
     @pulumi.getter
-    def max(self) -> pulumi.Output[Optional[float]]:
+    def image(self) -> pulumi.Output[Optional['outputs.ImageProperties']]:
         """
-        The maximum number of instances for the service
+        Image information used when creating the deploy. Not present for Git-backed deploys
         """
-        return pulumi.get(self, "max")
+        return pulumi.get(self, "image")
 
     @property
     @pulumi.getter
-    def min(self) -> pulumi.Output[Optional[float]]:
-        """
-        The minimum number of instances for the service
-        """
-        return pulumi.get(self, "min")
+    def status(self) -> pulumi.Output[Optional['Status']]:
+        return pulumi.get(self, "status")
+
+    @property
+    @pulumi.getter
+    def trigger(self) -> pulumi.Output[Optional['Trigger']]:
+        return pulumi.get(self, "trigger")
+
+    @property
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "updated_at")
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/background_worker.py` & `pulumi_render-0.2.0/pulumi_render/services/background_worker.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,259 +15,209 @@
 __all__ = ['BackgroundWorkerArgs', 'BackgroundWorker']
 
 @pulumi.input_type
 class BackgroundWorkerArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  owner_id: pulumi.Input[str],
-                 repo: pulumi.Input[str],
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
+                 build_filter: Optional[pulumi.Input['BuildFilterArgs']] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]] = None,
+                 image: Optional[pulumi.Input['ImageArgs']] = None,
+                 repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]] = None,
-                 service_details: Optional[pulumi.Input['BackgroundWorkerServiceDetailsArgs']] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None):
+                 service_details: Optional[pulumi.Input['BackgroundWorkerDetailsCreateArgs']] = None,
+                 type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a BackgroundWorker resource.
-        :param pulumi.Input[str] owner_id: The id of the owner (user/team).
+        :param pulumi.Input['ServiceCreateAutoDeploy'] auto_deploy: Defaults to "yes"
+        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository
         :param pulumi.Input[str] repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param pulumi.Input['ServiceAutoDeploy'] auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository.
-        :param pulumi.Input['ServiceNotifyOnFail'] notify_on_fail: The notification setting for this service upon deployment failure.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
         if auto_deploy is None:
-            auto_deploy = 'no'
+            auto_deploy = 'yes'
         if auto_deploy is not None:
             pulumi.set(__self__, "auto_deploy", auto_deploy)
         if branch is not None:
             pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
         if env_vars is not None:
             pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
+        if image is not None:
+            pulumi.set(__self__, "image", image)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
+        if root_dir is not None:
+            pulumi.set(__self__, "root_dir", root_dir)
         if secret_files is not None:
             pulumi.set(__self__, "secret_files", secret_files)
         if service_details is not None:
             pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
         if type is None:
             type = 'background_worker'
         if type is not None:
             pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> pulumi.Input[str]:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @owner_id.setter
     def owner_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "owner_id", value)
 
     @property
-    @pulumi.getter
-    def repo(self) -> pulumi.Input[str]:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
-        return pulumi.get(self, "repo")
-
-    @repo.setter
-    def repo(self, value: pulumi.Input[str]):
-        pulumi.set(self, "repo", value)
-
-    @property
     @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional[pulumi.Input['ServiceAutoDeploy']]:
+    def auto_deploy(self) -> Optional[pulumi.Input['ServiceCreateAutoDeploy']]:
         """
-        Whether to auto deploy the service or not upon git push.
+        Defaults to "yes"
         """
         return pulumi.get(self, "auto_deploy")
 
     @auto_deploy.setter
-    def auto_deploy(self, value: Optional[pulumi.Input['ServiceAutoDeploy']]):
+    def auto_deploy(self, value: Optional[pulumi.Input['ServiceCreateAutoDeploy']]):
         pulumi.set(self, "auto_deploy", value)
 
     @property
     @pulumi.getter
     def branch(self) -> Optional[pulumi.Input[str]]:
         """
-        If left empty, this will fall back to the default branch of the repository.
+        If left empty, this will fall back to the default branch of the repository
         """
         return pulumi.get(self, "branch")
 
     @branch.setter
     def branch(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "branch", value)
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "created_at")
-
-    @created_at.setter
-    def created_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "created_at", value)
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional[pulumi.Input['BuildFilterArgs']]:
+        return pulumi.get(self, "build_filter")
+
+    @build_filter.setter
+    def build_filter(self, value: Optional[pulumi.Input['BuildFilterArgs']]):
+        pulumi.set(self, "build_filter", value)
 
     @property
     @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]]:
+    def env_vars(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]]:
         return pulumi.get(self, "env_vars")
 
     @env_vars.setter
-    def env_vars(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]]):
+    def env_vars(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]]):
         pulumi.set(self, "env_vars", value)
 
     @property
-    @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional[pulumi.Input['ServiceNotifyOnFail']]:
+    @pulumi.getter
+    def image(self) -> Optional[pulumi.Input['ImageArgs']]:
+        return pulumi.get(self, "image")
+
+    @image.setter
+    def image(self, value: Optional[pulumi.Input['ImageArgs']]):
+        pulumi.set(self, "image", value)
+
+    @property
+    @pulumi.getter
+    def repo(self) -> Optional[pulumi.Input[str]]:
         """
-        The notification setting for this service upon deployment failure.
+        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
         """
-        return pulumi.get(self, "notify_on_fail")
+        return pulumi.get(self, "repo")
 
-    @notify_on_fail.setter
-    def notify_on_fail(self, value: Optional[pulumi.Input['ServiceNotifyOnFail']]):
-        pulumi.set(self, "notify_on_fail", value)
+    @repo.setter
+    def repo(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "repo", value)
+
+    @property
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "root_dir")
+
+    @root_dir.setter
+    def root_dir(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "root_dir", value)
 
     @property
     @pulumi.getter(name="secretFiles")
     def secret_files(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]]:
         return pulumi.get(self, "secret_files")
 
     @secret_files.setter
     def secret_files(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]]):
         pulumi.set(self, "secret_files", value)
 
     @property
     @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional[pulumi.Input['BackgroundWorkerServiceDetailsArgs']]:
+    def service_details(self) -> Optional[pulumi.Input['BackgroundWorkerDetailsCreateArgs']]:
         return pulumi.get(self, "service_details")
 
     @service_details.setter
-    def service_details(self, value: Optional[pulumi.Input['BackgroundWorkerServiceDetailsArgs']]):
+    def service_details(self, value: Optional[pulumi.Input['BackgroundWorkerDetailsCreateArgs']]):
         pulumi.set(self, "service_details", value)
 
     @property
     @pulumi.getter
-    def slug(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "slug")
-
-    @slug.setter
-    def slug(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "slug", value)
-
-    @property
-    @pulumi.getter
-    def suspended(self) -> Optional[pulumi.Input['ServiceSuspended']]:
-        return pulumi.get(self, "suspended")
-
-    @suspended.setter
-    def suspended(self, value: Optional[pulumi.Input['ServiceSuspended']]):
-        pulumi.set(self, "suspended", value)
-
-    @property
-    @pulumi.getter
-    def suspenders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "suspenders")
-
-    @suspenders.setter
-    def suspenders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "suspenders", value)
-
-    @property
-    @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
-    @property
-    @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "updated_at")
-
-    @updated_at.setter
-    def updated_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "updated_at", value)
-
 
 class BackgroundWorker(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvVarKeyValueArgs']]]]] = None,
+                 build_filter: Optional[pulumi.Input[pulumi.InputType['BuildFilterArgs']]] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union[pulumi.InputType['EnvVarKeyValueArgs'], pulumi.InputType['EnvVarKeyGenerateValueArgs']]]]]] = None,
+                 image: Optional[pulumi.Input[pulumi.InputType['ImageArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
                  owner_id: Optional[pulumi.Input[str]] = None,
                  repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretFileArgs']]]]] = None,
-                 service_details: Optional[pulumi.Input[pulumi.InputType['BackgroundWorkerServiceDetailsArgs']]] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 service_details: Optional[pulumi.Input[pulumi.InputType['BackgroundWorkerDetailsCreateArgs']]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        A background worker service
-
+        Create a BackgroundWorker resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input['ServiceAutoDeploy'] auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository.
-        :param pulumi.Input['ServiceNotifyOnFail'] notify_on_fail: The notification setting for this service upon deployment failure.
-        :param pulumi.Input[str] owner_id: The id of the owner (user/team).
+        :param pulumi.Input['ServiceCreateAutoDeploy'] auto_deploy: Defaults to "yes"
+        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository
         :param pulumi.Input[str] repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: BackgroundWorkerArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        A background worker service
-
+        Create a BackgroundWorker resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param BackgroundWorkerArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(BackgroundWorkerArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -275,63 +225,62 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvVarKeyValueArgs']]]]] = None,
+                 build_filter: Optional[pulumi.Input[pulumi.InputType['BuildFilterArgs']]] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union[pulumi.InputType['EnvVarKeyValueArgs'], pulumi.InputType['EnvVarKeyGenerateValueArgs']]]]]] = None,
+                 image: Optional[pulumi.Input[pulumi.InputType['ImageArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
                  owner_id: Optional[pulumi.Input[str]] = None,
                  repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretFileArgs']]]]] = None,
-                 service_details: Optional[pulumi.Input[pulumi.InputType['BackgroundWorkerServiceDetailsArgs']]] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 service_details: Optional[pulumi.Input[pulumi.InputType['BackgroundWorkerDetailsCreateArgs']]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = BackgroundWorkerArgs.__new__(BackgroundWorkerArgs)
 
             if auto_deploy is None:
-                auto_deploy = 'no'
+                auto_deploy = 'yes'
             __props__.__dict__["auto_deploy"] = auto_deploy
             __props__.__dict__["branch"] = branch
-            __props__.__dict__["created_at"] = created_at
+            __props__.__dict__["build_filter"] = build_filter
             __props__.__dict__["env_vars"] = env_vars
+            __props__.__dict__["image"] = image
             if name is None and not opts.urn:
                 raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
-            __props__.__dict__["notify_on_fail"] = notify_on_fail
             if owner_id is None and not opts.urn:
                 raise TypeError("Missing required property 'owner_id'")
             __props__.__dict__["owner_id"] = owner_id
-            if repo is None and not opts.urn:
-                raise TypeError("Missing required property 'repo'")
             __props__.__dict__["repo"] = repo
+            __props__.__dict__["root_dir"] = root_dir
             __props__.__dict__["secret_files"] = secret_files
             __props__.__dict__["service_details"] = service_details
-            __props__.__dict__["slug"] = slug
-            __props__.__dict__["suspended"] = suspended
-            __props__.__dict__["suspenders"] = suspenders
             if type is None:
                 type = 'background_worker'
             __props__.__dict__["type"] = type
-            __props__.__dict__["updated_at"] = updated_at
+            __props__.__dict__["created_at"] = None
+            __props__.__dict__["image_path"] = None
+            __props__.__dict__["notify_on_fail"] = None
+            __props__.__dict__["slug"] = None
+            __props__.__dict__["suspended"] = None
+            __props__.__dict__["suspenders"] = None
+            __props__.__dict__["updated_at"] = None
         super(BackgroundWorker, __self__).__init__(
             'render:services:BackgroundWorker',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -348,107 +297,116 @@
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = BackgroundWorkerArgs.__new__(BackgroundWorkerArgs)
 
         __props__.__dict__["auto_deploy"] = None
         __props__.__dict__["branch"] = None
+        __props__.__dict__["build_filter"] = None
         __props__.__dict__["created_at"] = None
         __props__.__dict__["env_vars"] = None
+        __props__.__dict__["image"] = None
+        __props__.__dict__["image_path"] = None
         __props__.__dict__["name"] = None
         __props__.__dict__["notify_on_fail"] = None
         __props__.__dict__["owner_id"] = None
         __props__.__dict__["repo"] = None
+        __props__.__dict__["root_dir"] = None
         __props__.__dict__["secret_files"] = None
         __props__.__dict__["service_details"] = None
         __props__.__dict__["slug"] = None
         __props__.__dict__["suspended"] = None
         __props__.__dict__["suspenders"] = None
         __props__.__dict__["type"] = None
         __props__.__dict__["updated_at"] = None
         return BackgroundWorker(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="autoDeploy")
     def auto_deploy(self) -> pulumi.Output[Optional['ServiceAutoDeploy']]:
-        """
-        Whether to auto deploy the service or not upon git push.
-        """
         return pulumi.get(self, "auto_deploy")
 
     @property
     @pulumi.getter
     def branch(self) -> pulumi.Output[Optional[str]]:
-        """
-        If left empty, this will fall back to the default branch of the repository.
-        """
         return pulumi.get(self, "branch")
 
     @property
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> pulumi.Output[Optional['outputs.BuildFilter']]:
+        return pulumi.get(self, "build_filter")
+
+    @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter(name="envVars")
-    def env_vars(self) -> pulumi.Output[Optional[Sequence['outputs.EnvVarKeyValue']]]:
+    def env_vars(self) -> pulumi.Output[Optional[Sequence[Any]]]:
         return pulumi.get(self, "env_vars")
 
     @property
     @pulumi.getter
+    def image(self) -> pulumi.Output[Optional['outputs.Image']]:
+        return pulumi.get(self, "image")
+
+    @property
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "image_path")
+
+    @property
+    @pulumi.getter
     def name(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="notifyOnFail")
     def notify_on_fail(self) -> pulumi.Output[Optional['ServiceNotifyOnFail']]:
-        """
-        The notification setting for this service upon deployment failure.
-        """
         return pulumi.get(self, "notify_on_fail")
 
     @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> pulumi.Output[Optional[str]]:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @property
     @pulumi.getter
     def repo(self) -> pulumi.Output[Optional[str]]:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
         return pulumi.get(self, "repo")
 
     @property
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "root_dir")
+
+    @property
     @pulumi.getter(name="secretFiles")
     def secret_files(self) -> pulumi.Output[Optional[Sequence['outputs.SecretFile']]]:
         return pulumi.get(self, "secret_files")
 
     @property
     @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> pulumi.Output[Optional['outputs.BackgroundWorkerServiceDetails']]:
+    def service_details(self) -> pulumi.Output[Optional['outputs.BackgroundWorkerDetailsOutput']]:
         return pulumi.get(self, "service_details")
 
     @property
     @pulumi.getter
     def slug(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "slug")
 
     @property
     @pulumi.getter
     def suspended(self) -> pulumi.Output[Optional['ServiceSuspended']]:
         return pulumi.get(self, "suspended")
 
     @property
     @pulumi.getter
-    def suspenders(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    def suspenders(self) -> pulumi.Output[Optional[Sequence['ServiceSuspendersItem']]]:
         return pulumi.get(self, "suspenders")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "type")
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/cron_job.py` & `pulumi_render-0.2.0/pulumi_render/services/web_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,447 +8,405 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._enums import *
 from ._inputs import *
 
-__all__ = ['CronJobArgs', 'CronJob']
+__all__ = ['WebServiceArgs', 'WebService']
 
 @pulumi.input_type
-class CronJobArgs:
+class WebServiceArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  owner_id: pulumi.Input[str],
-                 repo: pulumi.Input[str],
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
+                 build_filter: Optional[pulumi.Input['BuildFilterArgs']] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]] = None,
+                 image: Optional[pulumi.Input['ImageArgs']] = None,
+                 repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]] = None,
-                 service_details: Optional[pulumi.Input['CronJobServiceDetailsArgs']] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None):
+                 service_details: Optional[pulumi.Input['WebServiceDetailsCreateArgs']] = None,
+                 type: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a CronJob resource.
-        :param pulumi.Input[str] owner_id: The id of the owner (user/team).
+        The set of arguments for constructing a WebService resource.
+        :param pulumi.Input['ServiceCreateAutoDeploy'] auto_deploy: Defaults to "yes"
+        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository
         :param pulumi.Input[str] repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param pulumi.Input['ServiceAutoDeploy'] auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository.
-        :param pulumi.Input['ServiceNotifyOnFail'] notify_on_fail: The notification setting for this service upon deployment failure.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
         if auto_deploy is None:
-            auto_deploy = 'no'
+            auto_deploy = 'yes'
         if auto_deploy is not None:
             pulumi.set(__self__, "auto_deploy", auto_deploy)
         if branch is not None:
             pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
         if env_vars is not None:
             pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
+        if image is not None:
+            pulumi.set(__self__, "image", image)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
+        if root_dir is not None:
+            pulumi.set(__self__, "root_dir", root_dir)
         if secret_files is not None:
             pulumi.set(__self__, "secret_files", secret_files)
         if service_details is not None:
             pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
         if type is None:
-            type = 'cron_job'
+            type = 'web_service'
         if type is not None:
             pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> pulumi.Input[str]:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @owner_id.setter
     def owner_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "owner_id", value)
 
     @property
-    @pulumi.getter
-    def repo(self) -> pulumi.Input[str]:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
-        return pulumi.get(self, "repo")
-
-    @repo.setter
-    def repo(self, value: pulumi.Input[str]):
-        pulumi.set(self, "repo", value)
-
-    @property
     @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional[pulumi.Input['ServiceAutoDeploy']]:
+    def auto_deploy(self) -> Optional[pulumi.Input['ServiceCreateAutoDeploy']]:
         """
-        Whether to auto deploy the service or not upon git push.
+        Defaults to "yes"
         """
         return pulumi.get(self, "auto_deploy")
 
     @auto_deploy.setter
-    def auto_deploy(self, value: Optional[pulumi.Input['ServiceAutoDeploy']]):
+    def auto_deploy(self, value: Optional[pulumi.Input['ServiceCreateAutoDeploy']]):
         pulumi.set(self, "auto_deploy", value)
 
     @property
     @pulumi.getter
     def branch(self) -> Optional[pulumi.Input[str]]:
         """
-        If left empty, this will fall back to the default branch of the repository.
+        If left empty, this will fall back to the default branch of the repository
         """
         return pulumi.get(self, "branch")
 
     @branch.setter
     def branch(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "branch", value)
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "created_at")
-
-    @created_at.setter
-    def created_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "created_at", value)
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional[pulumi.Input['BuildFilterArgs']]:
+        return pulumi.get(self, "build_filter")
+
+    @build_filter.setter
+    def build_filter(self, value: Optional[pulumi.Input['BuildFilterArgs']]):
+        pulumi.set(self, "build_filter", value)
 
     @property
     @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]]:
+    def env_vars(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]]:
         return pulumi.get(self, "env_vars")
 
     @env_vars.setter
-    def env_vars(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]]):
+    def env_vars(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]]):
         pulumi.set(self, "env_vars", value)
 
     @property
-    @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional[pulumi.Input['ServiceNotifyOnFail']]:
+    @pulumi.getter
+    def image(self) -> Optional[pulumi.Input['ImageArgs']]:
+        return pulumi.get(self, "image")
+
+    @image.setter
+    def image(self, value: Optional[pulumi.Input['ImageArgs']]):
+        pulumi.set(self, "image", value)
+
+    @property
+    @pulumi.getter
+    def repo(self) -> Optional[pulumi.Input[str]]:
         """
-        The notification setting for this service upon deployment failure.
+        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
         """
-        return pulumi.get(self, "notify_on_fail")
+        return pulumi.get(self, "repo")
 
-    @notify_on_fail.setter
-    def notify_on_fail(self, value: Optional[pulumi.Input['ServiceNotifyOnFail']]):
-        pulumi.set(self, "notify_on_fail", value)
+    @repo.setter
+    def repo(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "repo", value)
+
+    @property
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "root_dir")
+
+    @root_dir.setter
+    def root_dir(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "root_dir", value)
 
     @property
     @pulumi.getter(name="secretFiles")
     def secret_files(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]]:
         return pulumi.get(self, "secret_files")
 
     @secret_files.setter
     def secret_files(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]]):
         pulumi.set(self, "secret_files", value)
 
     @property
     @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional[pulumi.Input['CronJobServiceDetailsArgs']]:
+    def service_details(self) -> Optional[pulumi.Input['WebServiceDetailsCreateArgs']]:
         return pulumi.get(self, "service_details")
 
     @service_details.setter
-    def service_details(self, value: Optional[pulumi.Input['CronJobServiceDetailsArgs']]):
+    def service_details(self, value: Optional[pulumi.Input['WebServiceDetailsCreateArgs']]):
         pulumi.set(self, "service_details", value)
 
     @property
     @pulumi.getter
-    def slug(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "slug")
-
-    @slug.setter
-    def slug(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "slug", value)
-
-    @property
-    @pulumi.getter
-    def suspended(self) -> Optional[pulumi.Input['ServiceSuspended']]:
-        return pulumi.get(self, "suspended")
-
-    @suspended.setter
-    def suspended(self, value: Optional[pulumi.Input['ServiceSuspended']]):
-        pulumi.set(self, "suspended", value)
-
-    @property
-    @pulumi.getter
-    def suspenders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "suspenders")
-
-    @suspenders.setter
-    def suspenders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "suspenders", value)
-
-    @property
-    @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
-    @property
-    @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "updated_at")
-
-    @updated_at.setter
-    def updated_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "updated_at", value)
 
-
-class CronJob(pulumi.CustomResource):
+class WebService(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvVarKeyValueArgs']]]]] = None,
+                 build_filter: Optional[pulumi.Input[pulumi.InputType['BuildFilterArgs']]] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union[pulumi.InputType['EnvVarKeyValueArgs'], pulumi.InputType['EnvVarKeyGenerateValueArgs']]]]]] = None,
+                 image: Optional[pulumi.Input[pulumi.InputType['ImageArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
                  owner_id: Optional[pulumi.Input[str]] = None,
                  repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretFileArgs']]]]] = None,
-                 service_details: Optional[pulumi.Input[pulumi.InputType['CronJobServiceDetailsArgs']]] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 service_details: Optional[pulumi.Input[pulumi.InputType['WebServiceDetailsCreateArgs']]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        A cron job
-
+        Create a WebService resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input['ServiceAutoDeploy'] auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository.
-        :param pulumi.Input['ServiceNotifyOnFail'] notify_on_fail: The notification setting for this service upon deployment failure.
-        :param pulumi.Input[str] owner_id: The id of the owner (user/team).
+        :param pulumi.Input['ServiceCreateAutoDeploy'] auto_deploy: Defaults to "yes"
+        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository
         :param pulumi.Input[str] repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: CronJobArgs,
+                 args: WebServiceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        A cron job
-
+        Create a WebService resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param CronJobArgs args: The arguments to use to populate this resource's properties.
+        :param WebServiceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CronJobArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(WebServiceArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvVarKeyValueArgs']]]]] = None,
+                 build_filter: Optional[pulumi.Input[pulumi.InputType['BuildFilterArgs']]] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union[pulumi.InputType['EnvVarKeyValueArgs'], pulumi.InputType['EnvVarKeyGenerateValueArgs']]]]]] = None,
+                 image: Optional[pulumi.Input[pulumi.InputType['ImageArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
                  owner_id: Optional[pulumi.Input[str]] = None,
                  repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretFileArgs']]]]] = None,
-                 service_details: Optional[pulumi.Input[pulumi.InputType['CronJobServiceDetailsArgs']]] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 service_details: Optional[pulumi.Input[pulumi.InputType['WebServiceDetailsCreateArgs']]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CronJobArgs.__new__(CronJobArgs)
+            __props__ = WebServiceArgs.__new__(WebServiceArgs)
 
             if auto_deploy is None:
-                auto_deploy = 'no'
+                auto_deploy = 'yes'
             __props__.__dict__["auto_deploy"] = auto_deploy
             __props__.__dict__["branch"] = branch
-            __props__.__dict__["created_at"] = created_at
+            __props__.__dict__["build_filter"] = build_filter
             __props__.__dict__["env_vars"] = env_vars
+            __props__.__dict__["image"] = image
             if name is None and not opts.urn:
                 raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
-            __props__.__dict__["notify_on_fail"] = notify_on_fail
             if owner_id is None and not opts.urn:
                 raise TypeError("Missing required property 'owner_id'")
             __props__.__dict__["owner_id"] = owner_id
-            if repo is None and not opts.urn:
-                raise TypeError("Missing required property 'repo'")
             __props__.__dict__["repo"] = repo
+            __props__.__dict__["root_dir"] = root_dir
             __props__.__dict__["secret_files"] = secret_files
             __props__.__dict__["service_details"] = service_details
-            __props__.__dict__["slug"] = slug
-            __props__.__dict__["suspended"] = suspended
-            __props__.__dict__["suspenders"] = suspenders
             if type is None:
-                type = 'cron_job'
+                type = 'web_service'
             __props__.__dict__["type"] = type
-            __props__.__dict__["updated_at"] = updated_at
-        super(CronJob, __self__).__init__(
-            'render:services:CronJob',
+            __props__.__dict__["created_at"] = None
+            __props__.__dict__["image_path"] = None
+            __props__.__dict__["notify_on_fail"] = None
+            __props__.__dict__["slug"] = None
+            __props__.__dict__["suspended"] = None
+            __props__.__dict__["suspenders"] = None
+            __props__.__dict__["updated_at"] = None
+        super(WebService, __self__).__init__(
+            'render:services:WebService',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'CronJob':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'WebService':
         """
-        Get an existing CronJob resource's state with the given name, id, and optional extra
+        Get an existing WebService resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = CronJobArgs.__new__(CronJobArgs)
+        __props__ = WebServiceArgs.__new__(WebServiceArgs)
 
         __props__.__dict__["auto_deploy"] = None
         __props__.__dict__["branch"] = None
+        __props__.__dict__["build_filter"] = None
         __props__.__dict__["created_at"] = None
         __props__.__dict__["env_vars"] = None
+        __props__.__dict__["image"] = None
+        __props__.__dict__["image_path"] = None
         __props__.__dict__["name"] = None
         __props__.__dict__["notify_on_fail"] = None
         __props__.__dict__["owner_id"] = None
         __props__.__dict__["repo"] = None
+        __props__.__dict__["root_dir"] = None
         __props__.__dict__["secret_files"] = None
         __props__.__dict__["service_details"] = None
         __props__.__dict__["slug"] = None
         __props__.__dict__["suspended"] = None
         __props__.__dict__["suspenders"] = None
         __props__.__dict__["type"] = None
         __props__.__dict__["updated_at"] = None
-        return CronJob(resource_name, opts=opts, __props__=__props__)
+        return WebService(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="autoDeploy")
     def auto_deploy(self) -> pulumi.Output[Optional['ServiceAutoDeploy']]:
-        """
-        Whether to auto deploy the service or not upon git push.
-        """
         return pulumi.get(self, "auto_deploy")
 
     @property
     @pulumi.getter
     def branch(self) -> pulumi.Output[Optional[str]]:
-        """
-        If left empty, this will fall back to the default branch of the repository.
-        """
         return pulumi.get(self, "branch")
 
     @property
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> pulumi.Output[Optional['outputs.BuildFilter']]:
+        return pulumi.get(self, "build_filter")
+
+    @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter(name="envVars")
-    def env_vars(self) -> pulumi.Output[Optional[Sequence['outputs.EnvVarKeyValue']]]:
+    def env_vars(self) -> pulumi.Output[Optional[Sequence[Any]]]:
         return pulumi.get(self, "env_vars")
 
     @property
     @pulumi.getter
+    def image(self) -> pulumi.Output[Optional['outputs.Image']]:
+        return pulumi.get(self, "image")
+
+    @property
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "image_path")
+
+    @property
+    @pulumi.getter
     def name(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="notifyOnFail")
     def notify_on_fail(self) -> pulumi.Output[Optional['ServiceNotifyOnFail']]:
-        """
-        The notification setting for this service upon deployment failure.
-        """
         return pulumi.get(self, "notify_on_fail")
 
     @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> pulumi.Output[Optional[str]]:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @property
     @pulumi.getter
     def repo(self) -> pulumi.Output[Optional[str]]:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
         return pulumi.get(self, "repo")
 
     @property
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "root_dir")
+
+    @property
     @pulumi.getter(name="secretFiles")
     def secret_files(self) -> pulumi.Output[Optional[Sequence['outputs.SecretFile']]]:
         return pulumi.get(self, "secret_files")
 
     @property
     @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> pulumi.Output[Optional['outputs.CronJobServiceDetails']]:
+    def service_details(self) -> pulumi.Output[Optional['outputs.WebServiceDetailsOutput']]:
         return pulumi.get(self, "service_details")
 
     @property
     @pulumi.getter
     def slug(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "slug")
 
     @property
     @pulumi.getter
     def suspended(self) -> pulumi.Output[Optional['ServiceSuspended']]:
         return pulumi.get(self, "suspended")
 
     @property
     @pulumi.getter
-    def suspenders(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    def suspenders(self) -> pulumi.Output[Optional[Sequence['ServiceSuspendersItem']]]:
         return pulumi.get(self, "suspenders")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "type")
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/custom_domains.py` & `pulumi_render-0.2.0/pulumi_render/services/rollback_deploy.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,167 +7,186 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._enums import *
 
-__all__ = ['CustomDomainsArgs', 'CustomDomains']
+__all__ = ['RollbackDeployArgs', 'RollbackDeploy']
 
 @pulumi.input_type
-class CustomDomainsArgs:
+class RollbackDeployArgs:
     def __init__(__self__, *,
-                 name: Optional[pulumi.Input[str]] = None,
+                 deploy_id: pulumi.Input[str],
                  service_id: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a CustomDomains resource.
-        :param pulumi.Input[str] service_id: (Required) The ID of the service
+        The set of arguments for constructing a RollbackDeploy resource.
+        :param pulumi.Input[str] deploy_id: The ID of the deploy to rollback to
+        :param pulumi.Input[str] service_id: The ID of the service
         """
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "deploy_id", deploy_id)
         if service_id is not None:
             pulumi.set(__self__, "service_id", service_id)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "name")
+    @pulumi.getter(name="deployId")
+    def deploy_id(self) -> pulumi.Input[str]:
+        """
+        The ID of the deploy to rollback to
+        """
+        return pulumi.get(self, "deploy_id")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @deploy_id.setter
+    def deploy_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "deploy_id", value)
 
     @property
     @pulumi.getter(name="serviceId")
     def service_id(self) -> Optional[pulumi.Input[str]]:
         """
-        (Required) The ID of the service
+        The ID of the service
         """
         return pulumi.get(self, "service_id")
 
     @service_id.setter
     def service_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_id", value)
 
 
-class CustomDomains(pulumi.CustomResource):
+class RollbackDeploy(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 name: Optional[pulumi.Input[str]] = None,
+                 deploy_id: Optional[pulumi.Input[str]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a CustomDomains resource with the given unique name, props, and options.
+        Create a RollbackDeploy resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] service_id: (Required) The ID of the service
+        :param pulumi.Input[str] deploy_id: The ID of the deploy to rollback to
+        :param pulumi.Input[str] service_id: The ID of the service
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[CustomDomainsArgs] = None,
+                 args: RollbackDeployArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a CustomDomains resource with the given unique name, props, and options.
+        Create a RollbackDeploy resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param CustomDomainsArgs args: The arguments to use to populate this resource's properties.
+        :param RollbackDeployArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CustomDomainsArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(RollbackDeployArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 name: Optional[pulumi.Input[str]] = None,
+                 deploy_id: Optional[pulumi.Input[str]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CustomDomainsArgs.__new__(CustomDomainsArgs)
+            __props__ = RollbackDeployArgs.__new__(RollbackDeployArgs)
 
-            __props__.__dict__["name"] = name
+            if deploy_id is None and not opts.urn:
+                raise TypeError("Missing required property 'deploy_id'")
+            __props__.__dict__["deploy_id"] = deploy_id
             __props__.__dict__["service_id"] = service_id
+            __props__.__dict__["commit"] = None
             __props__.__dict__["created_at"] = None
-            __props__.__dict__["domain_type"] = None
-            __props__.__dict__["public_suffix"] = None
-            __props__.__dict__["redirect_for_name"] = None
-            __props__.__dict__["server"] = None
-            __props__.__dict__["verification_status"] = None
-        super(CustomDomains, __self__).__init__(
-            'render:services:CustomDomains',
+            __props__.__dict__["finished_at"] = None
+            __props__.__dict__["image"] = None
+            __props__.__dict__["status"] = None
+            __props__.__dict__["trigger"] = None
+            __props__.__dict__["updated_at"] = None
+        super(RollbackDeploy, __self__).__init__(
+            'render:services:RollbackDeploy',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'CustomDomains':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'RollbackDeploy':
         """
-        Get an existing CustomDomains resource's state with the given name, id, and optional extra
+        Get an existing RollbackDeploy resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = CustomDomainsArgs.__new__(CustomDomainsArgs)
+        __props__ = RollbackDeployArgs.__new__(RollbackDeployArgs)
 
+        __props__.__dict__["commit"] = None
         __props__.__dict__["created_at"] = None
-        __props__.__dict__["domain_type"] = None
-        __props__.__dict__["name"] = None
-        __props__.__dict__["public_suffix"] = None
-        __props__.__dict__["redirect_for_name"] = None
-        __props__.__dict__["server"] = None
-        __props__.__dict__["verification_status"] = None
-        return CustomDomains(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["deploy_id"] = None
+        __props__.__dict__["finished_at"] = None
+        __props__.__dict__["image"] = None
+        __props__.__dict__["status"] = None
+        __props__.__dict__["trigger"] = None
+        __props__.__dict__["updated_at"] = None
+        return RollbackDeploy(resource_name, opts=opts, __props__=__props__)
+
+    @property
+    @pulumi.getter
+    def commit(self) -> pulumi.Output[Optional['outputs.CommitProperties']]:
+        return pulumi.get(self, "commit")
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "created_at")
 
     @property
-    @pulumi.getter(name="domainType")
-    def domain_type(self) -> pulumi.Output['DomainType']:
-        return pulumi.get(self, "domain_type")
+    @pulumi.getter(name="deployId")
+    def deploy_id(self) -> pulumi.Output[str]:
+        """
+        The ID of the deploy to rollback to
+        """
+        return pulumi.get(self, "deploy_id")
 
     @property
-    @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "name")
+    @pulumi.getter(name="finishedAt")
+    def finished_at(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "finished_at")
 
     @property
-    @pulumi.getter(name="publicSuffix")
-    def public_suffix(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "public_suffix")
+    @pulumi.getter
+    def image(self) -> pulumi.Output[Optional['outputs.ImageProperties']]:
+        """
+        Image information used when creating the deploy. Not present for Git-backed deploys
+        """
+        return pulumi.get(self, "image")
 
     @property
-    @pulumi.getter(name="redirectForName")
-    def redirect_for_name(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "redirect_for_name")
+    @pulumi.getter
+    def status(self) -> pulumi.Output[Optional['Status']]:
+        return pulumi.get(self, "status")
 
     @property
     @pulumi.getter
-    def server(self) -> pulumi.Output['outputs.ServerProperties']:
-        return pulumi.get(self, "server")
+    def trigger(self) -> pulumi.Output[Optional['Trigger']]:
+        return pulumi.get(self, "trigger")
 
     @property
-    @pulumi.getter(name="verificationStatus")
-    def verification_status(self) -> pulumi.Output['VerificationStatus']:
-        return pulumi.get(self, "verification_status")
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "updated_at")
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/deploys.py` & `pulumi_render-0.2.0/pulumi_render/services/env_vars_for_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,138 +5,127 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
-from ._enums import *
+from ._inputs import *
 
-__all__ = ['DeploysArgs', 'Deploys']
+__all__ = ['EnvVarsForServiceArgs', 'EnvVarsForService']
 
 @pulumi.input_type
-class DeploysArgs:
+class EnvVarsForServiceArgs:
     def __init__(__self__, *,
-                 clear_cache: Optional[pulumi.Input['ClearCache']] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]] = None,
                  service_id: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Deploys resource.
-        :param pulumi.Input[str] service_id: (Required) The ID of the service
+        The set of arguments for constructing a EnvVarsForService resource.
+        :param pulumi.Input[str] service_id: The ID of the service
         """
-        if clear_cache is None:
-            clear_cache = 'do_not_clear'
-        if clear_cache is not None:
-            pulumi.set(__self__, "clear_cache", clear_cache)
+        if env_vars is not None:
+            pulumi.set(__self__, "env_vars", env_vars)
         if service_id is not None:
             pulumi.set(__self__, "service_id", service_id)
 
     @property
-    @pulumi.getter(name="clearCache")
-    def clear_cache(self) -> Optional[pulumi.Input['ClearCache']]:
-        return pulumi.get(self, "clear_cache")
-
-    @clear_cache.setter
-    def clear_cache(self, value: Optional[pulumi.Input['ClearCache']]):
-        pulumi.set(self, "clear_cache", value)
+    @pulumi.getter(name="envVars")
+    def env_vars(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]]:
+        return pulumi.get(self, "env_vars")
+
+    @env_vars.setter
+    def env_vars(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]]):
+        pulumi.set(self, "env_vars", value)
 
     @property
     @pulumi.getter(name="serviceId")
     def service_id(self) -> Optional[pulumi.Input[str]]:
         """
-        (Required) The ID of the service
+        The ID of the service
         """
         return pulumi.get(self, "service_id")
 
     @service_id.setter
     def service_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_id", value)
 
 
-class Deploys(pulumi.CustomResource):
+class EnvVarsForService(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 clear_cache: Optional[pulumi.Input['ClearCache']] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union[pulumi.InputType['EnvVarKeyValueArgs'], pulumi.InputType['EnvVarKeyGenerateValueArgs']]]]]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a Deploys resource with the given unique name, props, and options.
+        Create a EnvVarsForService resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] service_id: (Required) The ID of the service
+        :param pulumi.Input[str] service_id: The ID of the service
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[DeploysArgs] = None,
+                 args: Optional[EnvVarsForServiceArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Deploys resource with the given unique name, props, and options.
+        Create a EnvVarsForService resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param DeploysArgs args: The arguments to use to populate this resource's properties.
+        :param EnvVarsForServiceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(DeploysArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(EnvVarsForServiceArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 clear_cache: Optional[pulumi.Input['ClearCache']] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union[pulumi.InputType['EnvVarKeyValueArgs'], pulumi.InputType['EnvVarKeyGenerateValueArgs']]]]]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = DeploysArgs.__new__(DeploysArgs)
+            __props__ = EnvVarsForServiceArgs.__new__(EnvVarsForServiceArgs)
 
-            if clear_cache is None:
-                clear_cache = 'do_not_clear'
-            __props__.__dict__["clear_cache"] = clear_cache
+            __props__.__dict__["env_vars"] = env_vars
             __props__.__dict__["service_id"] = service_id
-            __props__.__dict__["commit"] = None
-        super(Deploys, __self__).__init__(
-            'render:services:Deploys',
+        super(EnvVarsForService, __self__).__init__(
+            'render:services:EnvVarsForService',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'Deploys':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'EnvVarsForService':
         """
-        Get an existing Deploys resource's state with the given name, id, and optional extra
+        Get an existing EnvVarsForService resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = DeploysArgs.__new__(DeploysArgs)
+        __props__ = EnvVarsForServiceArgs.__new__(EnvVarsForServiceArgs)
 
-        __props__.__dict__["clear_cache"] = None
-        __props__.__dict__["commit"] = None
-        return Deploys(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["env_vars"] = None
+        return EnvVarsForService(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="clearCache")
-    def clear_cache(self) -> pulumi.Output[Optional['ClearCache']]:
-        return pulumi.get(self, "clear_cache")
-
-    @property
-    @pulumi.getter
-    def commit(self) -> pulumi.Output[Optional['outputs.Commit']]:
-        return pulumi.get(self, "commit")
+    @pulumi.getter(name="envVars")
+    def env_vars(self) -> pulumi.Output[Optional[Sequence[Any]]]:
+        return pulumi.get(self, "env_vars")
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/env_vars.py` & `pulumi_render-0.2.0/pulumi_render/services/custom_domain.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,129 +4,126 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from . import outputs
-from ._enums import *
-from ._inputs import *
 
-__all__ = ['EnvVarsArgs', 'EnvVars']
+__all__ = ['CustomDomainArgs', 'CustomDomain']
 
 @pulumi.input_type
-class EnvVarsArgs:
+class CustomDomainArgs:
     def __init__(__self__, *,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  service_id: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a EnvVars resource.
-        :param pulumi.Input[str] service_id: (Required) The ID of the service
+        The set of arguments for constructing a CustomDomain resource.
+        :param pulumi.Input[str] service_id: The ID of the service
         """
-        if env_vars is not None:
-            pulumi.set(__self__, "env_vars", env_vars)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if service_id is not None:
             pulumi.set(__self__, "service_id", service_id)
 
     @property
-    @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]]:
-        return pulumi.get(self, "env_vars")
-
-    @env_vars.setter
-    def env_vars(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]]):
-        pulumi.set(self, "env_vars", value)
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="serviceId")
     def service_id(self) -> Optional[pulumi.Input[str]]:
         """
-        (Required) The ID of the service
+        The ID of the service
         """
         return pulumi.get(self, "service_id")
 
     @service_id.setter
     def service_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_id", value)
 
 
-class EnvVars(pulumi.CustomResource):
+class CustomDomain(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvVarKeyValueArgs']]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a EnvVars resource with the given unique name, props, and options.
+        Create a CustomDomain resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] service_id: (Required) The ID of the service
+        :param pulumi.Input[str] service_id: The ID of the service
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[EnvVarsArgs] = None,
+                 args: Optional[CustomDomainArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a EnvVars resource with the given unique name, props, and options.
+        Create a CustomDomain resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param EnvVarsArgs args: The arguments to use to populate this resource's properties.
+        :param CustomDomainArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(EnvVarsArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(CustomDomainArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvVarKeyValueArgs']]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = EnvVarsArgs.__new__(EnvVarsArgs)
+            __props__ = CustomDomainArgs.__new__(CustomDomainArgs)
 
-            __props__.__dict__["env_vars"] = env_vars
+            __props__.__dict__["name"] = name
             __props__.__dict__["service_id"] = service_id
-        super(EnvVars, __self__).__init__(
-            'render:services:EnvVars',
+        super(CustomDomain, __self__).__init__(
+            'render:services:CustomDomain',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'EnvVars':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'CustomDomain':
         """
-        Get an existing EnvVars resource's state with the given name, id, and optional extra
+        Get an existing CustomDomain resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = EnvVarsArgs.__new__(EnvVarsArgs)
+        __props__ = CustomDomainArgs.__new__(CustomDomainArgs)
 
-        __props__.__dict__["env_vars"] = None
-        return EnvVars(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["name"] = None
+        return CustomDomain(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="envVars")
-    def env_vars(self) -> pulumi.Output[Optional[Sequence['outputs.EnvVarKeyValue']]]:
-        return pulumi.get(self, "env_vars")
+    @pulumi.getter
+    def name(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "name")
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/get_background_worker.py` & `pulumi_render-0.2.0/pulumi_render/services/get_background_worker.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,32 +36,32 @@
     def __await__(self):
         if False:
             yield self
         return GetBackgroundWorkerResult(
             items=self.items)
 
 
-def get_background_worker(id: Optional[str] = None,
+def get_background_worker(service_id: Optional[str] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetBackgroundWorkerResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     __args__ = dict()
-    __args__['id'] = id
+    __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getBackgroundWorker', __args__, opts=opts, typ=GetBackgroundWorkerResult).value
 
     return AwaitableGetBackgroundWorkerResult(
         items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_background_worker)
-def get_background_worker_output(id: Optional[pulumi.Input[str]] = None,
+def get_background_worker_output(service_id: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetBackgroundWorkerResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/get_cron_job.py` & `pulumi_render-0.2.0/pulumi_render/services/get_cron_job.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,32 +36,32 @@
     def __await__(self):
         if False:
             yield self
         return GetCronJobResult(
             items=self.items)
 
 
-def get_cron_job(id: Optional[str] = None,
+def get_cron_job(service_id: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCronJobResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     __args__ = dict()
-    __args__['id'] = id
+    __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getCronJob', __args__, opts=opts, typ=GetCronJobResult).value
 
     return AwaitableGetCronJobResult(
         items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_cron_job)
-def get_cron_job_output(id: Optional[pulumi.Input[str]] = None,
+def get_cron_job_output(service_id: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCronJobResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/get_custom_domain.py` & `pulumi_render-0.2.0/pulumi_render/services/get_custom_domain.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,37 +36,37 @@
     def __await__(self):
         if False:
             yield self
         return GetCustomDomainResult(
             items=self.items)
 
 
-def get_custom_domain(id: Optional[str] = None,
+def get_custom_domain(custom_domain_id_or_name: Optional[str] = None,
                       service_id: Optional[str] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCustomDomainResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID or name of the custom domain
-    :param str service_id: (Required) The ID of the service
+    :param str custom_domain_id_or_name: The ID or name of the custom domain
+    :param str service_id: The ID of the service
     """
     __args__ = dict()
-    __args__['id'] = id
+    __args__['customDomainIdOrName'] = custom_domain_id_or_name
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getCustomDomain', __args__, opts=opts, typ=GetCustomDomainResult).value
 
     return AwaitableGetCustomDomainResult(
         items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_custom_domain)
-def get_custom_domain_output(id: Optional[pulumi.Input[str]] = None,
+def get_custom_domain_output(custom_domain_id_or_name: Optional[pulumi.Input[str]] = None,
                              service_id: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCustomDomainResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID or name of the custom domain
-    :param str service_id: (Required) The ID of the service
+    :param str custom_domain_id_or_name: The ID or name of the custom domain
+    :param str service_id: The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/get_deploy.py` & `pulumi_render-0.2.0/pulumi_render/services/get_deploy.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,37 +36,37 @@
     def __await__(self):
         if False:
             yield self
         return GetDeployResult(
             items=self.items)
 
 
-def get_deploy(id: Optional[str] = None,
+def get_deploy(deploy_id: Optional[str] = None,
                service_id: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDeployResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the deploy
-    :param str service_id: (Required) The ID of the service
+    :param str deploy_id: The ID of the deploy
+    :param str service_id: The ID of the service
     """
     __args__ = dict()
-    __args__['id'] = id
+    __args__['deployId'] = deploy_id
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getDeploy', __args__, opts=opts, typ=GetDeployResult).value
 
     return AwaitableGetDeployResult(
         items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_deploy)
-def get_deploy_output(id: Optional[pulumi.Input[str]] = None,
+def get_deploy_output(deploy_id: Optional[pulumi.Input[str]] = None,
                       service_id: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDeployResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the deploy
-    :param str service_id: (Required) The ID of the service
+    :param str deploy_id: The ID of the deploy
+    :param str service_id: The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/get_job.py` & `pulumi_render-0.2.0/pulumi_render/services/get_job.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,37 +35,37 @@
     def __await__(self):
         if False:
             yield self
         return GetJobResult(
             items=self.items)
 
 
-def get_job(id: Optional[str] = None,
+def get_job(job_id: Optional[str] = None,
             service_id: Optional[str] = None,
             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetJobResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the job
-    :param str service_id: (Required) The ID of the service
+    :param str job_id: The ID of the job
+    :param str service_id: The ID of the service
     """
     __args__ = dict()
-    __args__['id'] = id
+    __args__['jobId'] = job_id
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getJob', __args__, opts=opts, typ=GetJobResult).value
 
     return AwaitableGetJobResult(
         items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_job)
-def get_job_output(id: Optional[pulumi.Input[str]] = None,
+def get_job_output(job_id: Optional[pulumi.Input[str]] = None,
                    service_id: Optional[pulumi.Input[str]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetJobResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the job
-    :param str service_id: (Required) The ID of the service
+    :param str job_id: The ID of the job
+    :param str service_id: The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/get_private_service.py` & `pulumi_render-0.2.0/pulumi_render/services/get_private_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,32 +36,32 @@
     def __await__(self):
         if False:
             yield self
         return GetPrivateServiceResult(
             items=self.items)
 
 
-def get_private_service(id: Optional[str] = None,
+def get_private_service(service_id: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPrivateServiceResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     __args__ = dict()
-    __args__['id'] = id
+    __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getPrivateService', __args__, opts=opts, typ=GetPrivateServiceResult).value
 
     return AwaitableGetPrivateServiceResult(
         items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_private_service)
-def get_private_service_output(id: Optional[pulumi.Input[str]] = None,
+def get_private_service_output(service_id: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPrivateServiceResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/get_static_site.py` & `pulumi_render-0.2.0/pulumi_render/services/get_static_site.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,32 +36,32 @@
     def __await__(self):
         if False:
             yield self
         return GetStaticSiteResult(
             items=self.items)
 
 
-def get_static_site(id: Optional[str] = None,
+def get_static_site(service_id: Optional[str] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetStaticSiteResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     __args__ = dict()
-    __args__['id'] = id
+    __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getStaticSite', __args__, opts=opts, typ=GetStaticSiteResult).value
 
     return AwaitableGetStaticSiteResult(
         items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_static_site)
-def get_static_site_output(id: Optional[pulumi.Input[str]] = None,
+def get_static_site_output(service_id: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetStaticSiteResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/get_web_service.py` & `pulumi_render-0.2.0/pulumi_render/services/get_web_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,32 +36,32 @@
     def __await__(self):
         if False:
             yield self
         return GetWebServiceResult(
             items=self.items)
 
 
-def get_web_service(id: Optional[str] = None,
+def get_web_service(service_id: Optional[str] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetWebServiceResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     __args__ = dict()
-    __args__['id'] = id
+    __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getWebService', __args__, opts=opts, typ=GetWebServiceResult).value
 
     return AwaitableGetWebServiceResult(
         items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_web_service)
-def get_web_service_output(id: Optional[pulumi.Input[str]] = None,
+def get_web_service_output(service_id: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetWebServiceResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/jobs.py` & `pulumi_render-0.2.0/pulumi_render/services/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,92 +5,93 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
-__all__ = ['JobsArgs', 'Jobs']
+__all__ = ['JobArgs', 'Job']
 
 @pulumi.input_type
-class JobsArgs:
+class JobArgs:
     def __init__(__self__, *,
-                 plan_id: pulumi.Input[str],
                  start_command: pulumi.Input[str],
+                 plan_id: Optional[pulumi.Input[str]] = None,
                  service_id: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Jobs resource.
-        :param pulumi.Input[str] service_id: (Required) The ID of the service
+        The set of arguments for constructing a Job resource.
+        :param pulumi.Input[str] service_id: The ID of the service
         """
-        pulumi.set(__self__, "plan_id", plan_id)
         pulumi.set(__self__, "start_command", start_command)
+        if plan_id is not None:
+            pulumi.set(__self__, "plan_id", plan_id)
         if service_id is not None:
             pulumi.set(__self__, "service_id", service_id)
 
     @property
-    @pulumi.getter(name="planId")
-    def plan_id(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "plan_id")
-
-    @plan_id.setter
-    def plan_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "plan_id", value)
-
-    @property
     @pulumi.getter(name="startCommand")
     def start_command(self) -> pulumi.Input[str]:
         return pulumi.get(self, "start_command")
 
     @start_command.setter
     def start_command(self, value: pulumi.Input[str]):
         pulumi.set(self, "start_command", value)
 
     @property
+    @pulumi.getter(name="planId")
+    def plan_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "plan_id")
+
+    @plan_id.setter
+    def plan_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "plan_id", value)
+
+    @property
     @pulumi.getter(name="serviceId")
     def service_id(self) -> Optional[pulumi.Input[str]]:
         """
-        (Required) The ID of the service
+        The ID of the service
         """
         return pulumi.get(self, "service_id")
 
     @service_id.setter
     def service_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_id", value)
 
 
-class Jobs(pulumi.CustomResource):
+class Job(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  plan_id: Optional[pulumi.Input[str]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  start_command: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a Jobs resource with the given unique name, props, and options.
+        Create a Job resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] service_id: (Required) The ID of the service
+        :param pulumi.Input[str] service_id: The ID of the service
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: JobsArgs,
+                 args: JobArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Jobs resource with the given unique name, props, and options.
+        Create a Job resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param JobsArgs args: The arguments to use to populate this resource's properties.
+        :param JobArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(JobsArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(JobArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -101,73 +102,77 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = JobsArgs.__new__(JobsArgs)
+            __props__ = JobArgs.__new__(JobArgs)
 
-            if plan_id is None and not opts.urn:
-                raise TypeError("Missing required property 'plan_id'")
             __props__.__dict__["plan_id"] = plan_id
             __props__.__dict__["service_id"] = service_id
             if start_command is None and not opts.urn:
                 raise TypeError("Missing required property 'start_command'")
             __props__.__dict__["start_command"] = start_command
             __props__.__dict__["created_at"] = None
             __props__.__dict__["finished_at"] = None
             __props__.__dict__["started_at"] = None
             __props__.__dict__["status"] = None
-        super(Jobs, __self__).__init__(
-            'render:services:Jobs',
+        super(Job, __self__).__init__(
+            'render:services:Job',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'Jobs':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'Job':
         """
-        Get an existing Jobs resource's state with the given name, id, and optional extra
+        Get an existing Job resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = JobsArgs.__new__(JobsArgs)
+        __props__ = JobArgs.__new__(JobArgs)
 
         __props__.__dict__["created_at"] = None
         __props__.__dict__["finished_at"] = None
         __props__.__dict__["plan_id"] = None
+        __props__.__dict__["service_id"] = None
         __props__.__dict__["start_command"] = None
         __props__.__dict__["started_at"] = None
         __props__.__dict__["status"] = None
-        return Jobs(resource_name, opts=opts, __props__=__props__)
+        return Job(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="createdAt")
-    def created_at(self) -> pulumi.Output[Optional[str]]:
+    def created_at(self) -> pulumi.Output[str]:
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter(name="finishedAt")
     def finished_at(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "finished_at")
 
     @property
     @pulumi.getter(name="planId")
     def plan_id(self) -> pulumi.Output[str]:
         return pulumi.get(self, "plan_id")
 
     @property
+    @pulumi.getter(name="serviceId")
+    def service_id(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "service_id")
+
+    @property
     @pulumi.getter(name="startCommand")
     def start_command(self) -> pulumi.Output[str]:
         return pulumi.get(self, "start_command")
 
     @property
     @pulumi.getter(name="startedAt")
     def started_at(self) -> pulumi.Output[Optional[str]]:
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/list_custom_domains.py` & `pulumi_render-0.2.0/pulumi_render/services/list_custom_domains.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def __init__(__self__, items=None):
         if items and not isinstance(items, list):
             raise TypeError("Expected argument 'items' to be a list")
         pulumi.set(__self__, "items", items)
 
     @property
     @pulumi.getter
-    def items(self) -> Sequence['outputs.ListCustomDomainsResponse']:
+    def items(self) -> Sequence['outputs.ListCustomDomainsItemProperties']:
         return pulumi.get(self, "items")
 
 
 class AwaitableListCustomDomainsResult(ListCustomDomainsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -41,15 +41,15 @@
 
 
 def list_custom_domains(service_id: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableListCustomDomainsResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str service_id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     __args__ = dict()
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:listCustomDomains', __args__, opts=opts, typ=ListCustomDomainsResult).value
 
     return AwaitableListCustomDomainsResult(
@@ -58,10 +58,10 @@
 
 @_utilities.lift_output_func(list_custom_domains)
 def list_custom_domains_output(service_id: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListCustomDomainsResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str service_id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/list_deploys.py` & `pulumi_render-0.2.0/pulumi_render/services/list_deploys.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def __init__(__self__, items=None):
         if items and not isinstance(items, list):
             raise TypeError("Expected argument 'items' to be a list")
         pulumi.set(__self__, "items", items)
 
     @property
     @pulumi.getter
-    def items(self) -> Sequence['outputs.ListDeploysResponse']:
+    def items(self) -> Sequence['outputs.ListDeploysItemProperties']:
         return pulumi.get(self, "items")
 
 
 class AwaitableListDeploysResult(ListDeploysResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -41,15 +41,15 @@
 
 
 def list_deploys(service_id: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableListDeploysResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str service_id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     __args__ = dict()
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:listDeploys', __args__, opts=opts, typ=ListDeploysResult).value
 
     return AwaitableListDeploysResult(
@@ -58,10 +58,10 @@
 
 @_utilities.lift_output_func(list_deploys)
 def list_deploys_output(service_id: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListDeploysResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str service_id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/list_env_vars.py` & `pulumi_render-0.2.0/pulumi_render/services/list_env_vars_for_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,63 +5,62 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
-from ._enums import *
 
 __all__ = [
-    'ListEnvVarsResult',
-    'AwaitableListEnvVarsResult',
-    'list_env_vars',
-    'list_env_vars_output',
+    'ListEnvVarsForServiceResult',
+    'AwaitableListEnvVarsForServiceResult',
+    'list_env_vars_for_service',
+    'list_env_vars_for_service_output',
 ]
 
 @pulumi.output_type
-class ListEnvVarsResult:
+class ListEnvVarsForServiceResult:
     def __init__(__self__, items=None):
         if items and not isinstance(items, list):
             raise TypeError("Expected argument 'items' to be a list")
         pulumi.set(__self__, "items", items)
 
     @property
     @pulumi.getter
-    def items(self) -> Sequence['outputs.ListEnvVarsResponse']:
+    def items(self) -> Sequence['outputs.EnvVarWithCursor']:
         return pulumi.get(self, "items")
 
 
-class AwaitableListEnvVarsResult(ListEnvVarsResult):
+class AwaitableListEnvVarsForServiceResult(ListEnvVarsForServiceResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return ListEnvVarsResult(
+        return ListEnvVarsForServiceResult(
             items=self.items)
 
 
-def list_env_vars(service_id: Optional[str] = None,
-                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableListEnvVarsResult:
+def list_env_vars_for_service(service_id: Optional[str] = None,
+                              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableListEnvVarsForServiceResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str service_id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     __args__ = dict()
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('render:services:listEnvVars', __args__, opts=opts, typ=ListEnvVarsResult).value
+    __ret__ = pulumi.runtime.invoke('render:services:listEnvVarsForService', __args__, opts=opts, typ=ListEnvVarsForServiceResult).value
 
-    return AwaitableListEnvVarsResult(
+    return AwaitableListEnvVarsForServiceResult(
         items=pulumi.get(__ret__, 'items'))
 
 
-@_utilities.lift_output_func(list_env_vars)
-def list_env_vars_output(service_id: Optional[pulumi.Input[str]] = None,
-                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListEnvVarsResult]:
+@_utilities.lift_output_func(list_env_vars_for_service)
+def list_env_vars_for_service_output(service_id: Optional[pulumi.Input[str]] = None,
+                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListEnvVarsForServiceResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str service_id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/list_headers.py` & `pulumi_render-0.2.0/pulumi_render/services/list_retrieve_headers.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,60 +7,60 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
 __all__ = [
-    'ListHeadersResult',
-    'AwaitableListHeadersResult',
-    'list_headers',
-    'list_headers_output',
+    'ListRetrieveHeadersResult',
+    'AwaitableListRetrieveHeadersResult',
+    'list_retrieve_headers',
+    'list_retrieve_headers_output',
 ]
 
 @pulumi.output_type
-class ListHeadersResult:
+class ListRetrieveHeadersResult:
     def __init__(__self__, items=None):
         if items and not isinstance(items, list):
             raise TypeError("Expected argument 'items' to be a list")
         pulumi.set(__self__, "items", items)
 
     @property
     @pulumi.getter
-    def items(self) -> Sequence['outputs.ListServiceHeadersResponse']:
+    def items(self) -> Sequence['outputs.ListRetrieveHeadersItemProperties']:
         return pulumi.get(self, "items")
 
 
-class AwaitableListHeadersResult(ListHeadersResult):
+class AwaitableListRetrieveHeadersResult(ListRetrieveHeadersResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return ListHeadersResult(
+        return ListRetrieveHeadersResult(
             items=self.items)
 
 
-def list_headers(service_id: Optional[str] = None,
-                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableListHeadersResult:
+def list_retrieve_headers(service_id: Optional[str] = None,
+                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableListRetrieveHeadersResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str service_id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     __args__ = dict()
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('render:services:listHeaders', __args__, opts=opts, typ=ListHeadersResult).value
+    __ret__ = pulumi.runtime.invoke('render:services:listRetrieveHeaders', __args__, opts=opts, typ=ListRetrieveHeadersResult).value
 
-    return AwaitableListHeadersResult(
+    return AwaitableListRetrieveHeadersResult(
         items=pulumi.get(__ret__, 'items'))
 
 
-@_utilities.lift_output_func(list_headers)
-def list_headers_output(service_id: Optional[pulumi.Input[str]] = None,
-                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListHeadersResult]:
+@_utilities.lift_output_func(list_retrieve_headers)
+def list_retrieve_headers_output(service_id: Optional[pulumi.Input[str]] = None,
+                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListRetrieveHeadersResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str service_id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/list_jobs.py` & `pulumi_render-0.2.0/pulumi_render/services/list_job.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,60 +7,60 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
 __all__ = [
-    'ListJobsResult',
-    'AwaitableListJobsResult',
-    'list_jobs',
-    'list_jobs_output',
+    'ListJobResult',
+    'AwaitableListJobResult',
+    'list_job',
+    'list_job_output',
 ]
 
 @pulumi.output_type
-class ListJobsResult:
+class ListJobResult:
     def __init__(__self__, items=None):
         if items and not isinstance(items, list):
             raise TypeError("Expected argument 'items' to be a list")
         pulumi.set(__self__, "items", items)
 
     @property
     @pulumi.getter
-    def items(self) -> Sequence['outputs.ListJobsResponse']:
+    def items(self) -> Sequence['outputs.ListJobItemProperties']:
         return pulumi.get(self, "items")
 
 
-class AwaitableListJobsResult(ListJobsResult):
+class AwaitableListJobResult(ListJobResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return ListJobsResult(
+        return ListJobResult(
             items=self.items)
 
 
-def list_jobs(service_id: Optional[str] = None,
-              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableListJobsResult:
+def list_job(service_id: Optional[str] = None,
+             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableListJobResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str service_id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     __args__ = dict()
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('render:services:listJobs', __args__, opts=opts, typ=ListJobsResult).value
+    __ret__ = pulumi.runtime.invoke('render:services:listJob', __args__, opts=opts, typ=ListJobResult).value
 
-    return AwaitableListJobsResult(
+    return AwaitableListJobResult(
         items=pulumi.get(__ret__, 'items'))
 
 
-@_utilities.lift_output_func(list_jobs)
-def list_jobs_output(service_id: Optional[pulumi.Input[str]] = None,
-                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListJobsResult]:
+@_utilities.lift_output_func(list_job)
+def list_job_output(service_id: Optional[pulumi.Input[str]] = None,
+                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListJobResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str service_id: (Required) The ID of the service
+    :param str service_id: The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/list_routes.py` & `pulumi_render-0.2.0/pulumi_render/services/list_services.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,60 +8,53 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._enums import *
 
 __all__ = [
-    'ListRoutesResult',
-    'AwaitableListRoutesResult',
-    'list_routes',
-    'list_routes_output',
+    'ListServicesResult',
+    'AwaitableListServicesResult',
+    'list_services',
+    'list_services_output',
 ]
 
 @pulumi.output_type
-class ListRoutesResult:
+class ListServicesResult:
     def __init__(__self__, items=None):
         if items and not isinstance(items, list):
             raise TypeError("Expected argument 'items' to be a list")
         pulumi.set(__self__, "items", items)
 
     @property
     @pulumi.getter
-    def items(self) -> Sequence['outputs.ListStaticSiteRoutesResponse']:
+    def items(self) -> Sequence['outputs.ListServicesResponse']:
         return pulumi.get(self, "items")
 
 
-class AwaitableListRoutesResult(ListRoutesResult):
+class AwaitableListServicesResult(ListServicesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return ListRoutesResult(
+        return ListServicesResult(
             items=self.items)
 
 
-def list_routes(service_id: Optional[str] = None,
-                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableListRoutesResult:
+def list_services(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableListServicesResult:
     """
     Use this data source to access information about an existing resource.
-
-    :param str service_id: (Required) The ID of the service
     """
     __args__ = dict()
-    __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('render:services:listRoutes', __args__, opts=opts, typ=ListRoutesResult).value
+    __ret__ = pulumi.runtime.invoke('render:services:listServices', __args__, opts=opts, typ=ListServicesResult).value
 
-    return AwaitableListRoutesResult(
+    return AwaitableListServicesResult(
         items=pulumi.get(__ret__, 'items'))
 
 
-@_utilities.lift_output_func(list_routes)
-def list_routes_output(service_id: Optional[pulumi.Input[str]] = None,
-                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListRoutesResult]:
+@_utilities.lift_output_func(list_services)
+def list_services_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListServicesResult]:
     """
     Use this data source to access information about an existing resource.
-
-    :param str service_id: (Required) The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/outputs.py` & `pulumi_render-0.2.0/pulumi_render/services/outputs.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,403 +8,457 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._enums import *
 
 __all__ = [
-    'AutoScalingCriteria',
-    'AutoScalingCriteriaSpec',
-    'BackgroundWorker',
-    'BackgroundWorkerServiceDetails',
-    'BackgroundWorkerServiceDetailsParentServerProperties',
-    'Commit',
-    'CronJob',
-    'CronJobServiceDetails',
+    'AutoscalingConfig',
+    'AutoscalingCriteria',
+    'AutoscalingCriteriaPercentage',
+    'BackgroundWorkerDetailsOutput',
+    'BackgroundWorkerOutput',
+    'BuildFilter',
+    'CommitProperties',
+    'CronJobDetailsOutput',
+    'CronJobOutput',
     'CustomDomain',
     'CustomDomainServerProperties',
     'Deploy',
+    'DeployCommitProperties',
+    'DeployImageProperties',
     'Disk',
     'DockerDetails',
+    'EnvVar',
+    'EnvVarKeyGenerateValue',
     'EnvVarKeyValue',
+    'EnvVarWithCursor',
     'GetBackgroundWorker',
     'GetCronJob',
     'GetPrivateService',
     'GetStaticSite',
     'GetWebService',
+    'Header',
+    'Image',
+    'ImageProperties',
     'Job',
-    'ListCustomDomainsResponse',
-    'ListDeploysResponse',
-    'ListEnvVarsResponse',
-    'ListJobsResponse',
-    'ListServiceHeadersResponse',
-    'ListServiceResponse',
-    'ListStaticSiteRoutesResponse',
+    'ListCustomDomainsItemProperties',
+    'ListDeploysItemProperties',
+    'ListJobItemProperties',
+    'ListRetrieveHeadersItemProperties',
+    'ListRetrieveRoutesItemProperties',
+    'ListServicesResponse',
     'NativeEnvironmentDetails',
-    'OpenPorts',
-    'PrivateService',
-    'PrivateServiceDetails',
-    'PrivateServiceDetailsParentServerProperties',
+    'PrivateServiceDetailsOutput',
+    'PrivateServiceOutput',
+    'RegistryCredential',
+    'Resource',
+    'Route',
     'SecretFile',
-    'ServerProperties',
-    'ServiceHeader',
-    'StaticSite',
-    'StaticSiteRoute',
-    'StaticSiteServiceDetails',
-    'StaticSiteServiceDetailsParentServerProperties',
-    'WebService',
-    'WebServiceServiceDetails',
-    'WebServiceServiceDetailsParentServerProperties',
+    'ServerPort',
+    'Service',
+    'StaticSiteDetailsOutput',
+    'StaticSiteOutput',
+    'WebServiceDetailsOutput',
+    'WebServiceOutput',
 ]
 
 @pulumi.output_type
-class AutoScalingCriteria(dict):
+class AutoscalingConfig(dict):
     def __init__(__self__, *,
-                 cpu: Optional['outputs.AutoScalingCriteriaSpec'] = None,
-                 memory: Optional['outputs.AutoScalingCriteriaSpec'] = None):
-        if cpu is not None:
-            pulumi.set(__self__, "cpu", cpu)
-        if memory is not None:
-            pulumi.set(__self__, "memory", memory)
+                 criteria: 'outputs.AutoscalingCriteria',
+                 enabled: Optional[bool] = None,
+                 max: int,
+                 min: int):
+        """
+        :param int max: The maximum number of instances for the service
+        :param int min: The minimum number of instances for the service
+        """
+        pulumi.set(__self__, "criteria", criteria)
+        if enabled is None:
+            enabled = False
+        pulumi.set(__self__, "enabled", enabled)
+        pulumi.set(__self__, "max", max)
+        pulumi.set(__self__, "min", min)
+
+    @property
+    @pulumi.getter
+    def criteria(self) -> 'outputs.AutoscalingCriteria':
+        return pulumi.get(self, "criteria")
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> bool:
+        return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
-    def cpu(self) -> Optional['outputs.AutoScalingCriteriaSpec']:
+    def max(self) -> int:
+        """
+        The maximum number of instances for the service
+        """
+        return pulumi.get(self, "max")
+
+    @property
+    @pulumi.getter
+    def min(self) -> int:
+        """
+        The minimum number of instances for the service
+        """
+        return pulumi.get(self, "min")
+
+
+@pulumi.output_type
+class AutoscalingCriteria(dict):
+    def __init__(__self__, *,
+                 cpu: 'outputs.AutoscalingCriteriaPercentage',
+                 memory: 'outputs.AutoscalingCriteriaPercentage'):
+        pulumi.set(__self__, "cpu", cpu)
+        pulumi.set(__self__, "memory", memory)
+
+    @property
+    @pulumi.getter
+    def cpu(self) -> 'outputs.AutoscalingCriteriaPercentage':
         return pulumi.get(self, "cpu")
 
     @property
     @pulumi.getter
-    def memory(self) -> Optional['outputs.AutoScalingCriteriaSpec']:
+    def memory(self) -> 'outputs.AutoscalingCriteriaPercentage':
         return pulumi.get(self, "memory")
 
 
 @pulumi.output_type
-class AutoScalingCriteriaSpec(dict):
+class AutoscalingCriteriaPercentage(dict):
     def __init__(__self__, *,
                  enabled: Optional[bool] = None,
-                 percentage: Optional[float] = None):
+                 percentage: int):
         """
-        :param float percentage: Determines when your service will be scaled. If the average resource utilization is significantly above/below the target, we will increase/decrease the number of instances.
+        :param int percentage: Determines when your service will be scaled. If the average resource utilization is significantly above/below the target, we will increase/decrease the number of instances.
         """
-        if enabled is not None:
-            pulumi.set(__self__, "enabled", enabled)
-        if percentage is not None:
-            pulumi.set(__self__, "percentage", percentage)
+        if enabled is None:
+            enabled = False
+        pulumi.set(__self__, "enabled", enabled)
+        pulumi.set(__self__, "percentage", percentage)
 
     @property
     @pulumi.getter
-    def enabled(self) -> Optional[bool]:
+    def enabled(self) -> bool:
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
-    def percentage(self) -> Optional[float]:
+    def percentage(self) -> int:
         """
         Determines when your service will be scaled. If the average resource utilization is significantly above/below the target, we will increase/decrease the number of instances.
         """
         return pulumi.get(self, "percentage")
 
 
 @pulumi.output_type
-class BackgroundWorker(dict):
-    """
-    A background worker service
-    """
+class BackgroundWorkerDetailsOutput(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "buildPlan":
+            suggest = "build_plan"
+        elif key == "envSpecificDetails":
+            suggest = "env_specific_details"
+        elif key == "numInstances":
+            suggest = "num_instances"
+        elif key == "pullRequestPreviewsEnabled":
+            suggest = "pull_request_previews_enabled"
+        elif key == "parentServer":
+            suggest = "parent_server"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in BackgroundWorkerDetailsOutput. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        BackgroundWorkerDetailsOutput.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        BackgroundWorkerDetailsOutput.__key_warning(key)
+        return super().get(key, default)
+
     def __init__(__self__, *,
-                 name: str,
-                 owner_id: str,
-                 repo: str,
-                 auto_deploy: Optional['ServiceAutoDeploy'] = None,
-                 branch: Optional[str] = None,
-                 created_at: Optional[str] = None,
-                 env_vars: Optional[Sequence['outputs.EnvVarKeyValue']] = None,
-                 notify_on_fail: Optional['ServiceNotifyOnFail'] = None,
-                 secret_files: Optional[Sequence['outputs.SecretFile']] = None,
-                 service_details: Optional['outputs.BackgroundWorkerServiceDetails'] = None,
-                 slug: Optional[str] = None,
-                 suspended: Optional['ServiceSuspended'] = None,
-                 suspenders: Optional[Sequence[str]] = None,
-                 type: Optional[str] = None,
-                 updated_at: Optional[str] = None):
+                 build_plan: str,
+                 env: 'BackgroundWorkerDetailsOutputEnv',
+                 env_specific_details: Any,
+                 num_instances: int,
+                 plan: 'BackgroundWorkerDetailsOutputPlan',
+                 pull_request_previews_enabled: 'BackgroundWorkerDetailsOutputPullRequestPreviewsEnabled',
+                 region: 'BackgroundWorkerDetailsOutputRegion',
+                 autoscaling: Optional['outputs.AutoscalingConfig'] = None,
+                 disk: Optional['outputs.Disk'] = None,
+                 parent_server: Optional['outputs.Resource'] = None):
         """
-        A background worker service
-        :param str owner_id: The id of the owner (user/team).
-        :param str repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param 'ServiceAutoDeploy' auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param str branch: If left empty, this will fall back to the default branch of the repository.
-        :param 'ServiceNotifyOnFail' notify_on_fail: The notification setting for this service upon deployment failure.
+        :param 'BackgroundWorkerDetailsOutputEnv' env: Environment (runtime)
+        :param int num_instances: For a *manually* scaled service, this is the number of instances the service is scaled to. DOES NOT indicate the number of running instances for an *autoscaled* service.
+        :param 'BackgroundWorkerDetailsOutputPlan' plan: The instance type to use for the preview instance. Note that base services with any paid instance type can't create preview instances with the `free` instance type.
         """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
-        if auto_deploy is None:
-            auto_deploy = 'no'
-        if auto_deploy is not None:
-            pulumi.set(__self__, "auto_deploy", auto_deploy)
-        if branch is not None:
-            pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
-        if env_vars is not None:
-            pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
-        if secret_files is not None:
-            pulumi.set(__self__, "secret_files", secret_files)
-        if service_details is not None:
-            pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
-        if type is None:
-            type = 'background_worker'
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
+        pulumi.set(__self__, "build_plan", build_plan)
+        pulumi.set(__self__, "env", env)
+        pulumi.set(__self__, "env_specific_details", env_specific_details)
+        pulumi.set(__self__, "num_instances", num_instances)
+        pulumi.set(__self__, "plan", plan)
+        pulumi.set(__self__, "pull_request_previews_enabled", pull_request_previews_enabled)
+        pulumi.set(__self__, "region", region)
+        if autoscaling is not None:
+            pulumi.set(__self__, "autoscaling", autoscaling)
+        if disk is not None:
+            pulumi.set(__self__, "disk", disk)
+        if parent_server is not None:
+            pulumi.set(__self__, "parent_server", parent_server)
 
     @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
+    @pulumi.getter(name="buildPlan")
+    def build_plan(self) -> str:
+        return pulumi.get(self, "build_plan")
 
     @property
-    @pulumi.getter(name="ownerId")
-    def owner_id(self) -> str:
+    @pulumi.getter
+    def env(self) -> 'BackgroundWorkerDetailsOutputEnv':
         """
-        The id of the owner (user/team).
+        Environment (runtime)
         """
-        return pulumi.get(self, "owner_id")
+        return pulumi.get(self, "env")
 
     @property
-    @pulumi.getter
-    def repo(self) -> str:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
-        return pulumi.get(self, "repo")
+    @pulumi.getter(name="envSpecificDetails")
+    def env_specific_details(self) -> Any:
+        return pulumi.get(self, "env_specific_details")
 
     @property
-    @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional['ServiceAutoDeploy']:
+    @pulumi.getter(name="numInstances")
+    def num_instances(self) -> int:
         """
-        Whether to auto deploy the service or not upon git push.
+        For a *manually* scaled service, this is the number of instances the service is scaled to. DOES NOT indicate the number of running instances for an *autoscaled* service.
         """
-        return pulumi.get(self, "auto_deploy")
+        return pulumi.get(self, "num_instances")
 
     @property
     @pulumi.getter
-    def branch(self) -> Optional[str]:
+    def plan(self) -> 'BackgroundWorkerDetailsOutputPlan':
         """
-        If left empty, this will fall back to the default branch of the repository.
+        The instance type to use for the preview instance. Note that base services with any paid instance type can't create preview instances with the `free` instance type.
         """
-        return pulumi.get(self, "branch")
+        return pulumi.get(self, "plan")
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
-        return pulumi.get(self, "created_at")
+    @pulumi.getter(name="pullRequestPreviewsEnabled")
+    def pull_request_previews_enabled(self) -> 'BackgroundWorkerDetailsOutputPullRequestPreviewsEnabled':
+        return pulumi.get(self, "pull_request_previews_enabled")
 
     @property
-    @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[Sequence['outputs.EnvVarKeyValue']]:
-        return pulumi.get(self, "env_vars")
+    @pulumi.getter
+    def region(self) -> 'BackgroundWorkerDetailsOutputRegion':
+        return pulumi.get(self, "region")
 
     @property
-    @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional['ServiceNotifyOnFail']:
-        """
-        The notification setting for this service upon deployment failure.
-        """
-        return pulumi.get(self, "notify_on_fail")
+    @pulumi.getter
+    def autoscaling(self) -> Optional['outputs.AutoscalingConfig']:
+        return pulumi.get(self, "autoscaling")
 
     @property
-    @pulumi.getter(name="secretFiles")
-    def secret_files(self) -> Optional[Sequence['outputs.SecretFile']]:
-        return pulumi.get(self, "secret_files")
+    @pulumi.getter
+    def disk(self) -> Optional['outputs.Disk']:
+        return pulumi.get(self, "disk")
 
     @property
-    @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional['outputs.BackgroundWorkerServiceDetails']:
-        return pulumi.get(self, "service_details")
+    @pulumi.getter(name="parentServer")
+    def parent_server(self) -> Optional['outputs.Resource']:
+        return pulumi.get(self, "parent_server")
+
+
+@pulumi.output_type
+class BackgroundWorkerOutput(dict):
+    def __init__(__self__, *,
+                 auto_deploy: 'ServiceAutoDeploy',
+                 created_at: str,
+                 id: str,
+                 name: str,
+                 notify_on_fail: 'ServiceNotifyOnFail',
+                 owner_id: str,
+                 root_dir: str,
+                 slug: str,
+                 suspended: 'ServiceSuspended',
+                 suspenders: Sequence['ServiceSuspendersItem'],
+                 updated_at: str,
+                 branch: Optional[str] = None,
+                 build_filter: Optional['outputs.BuildFilter'] = None,
+                 image_path: Optional[str] = None,
+                 repo: Optional[str] = None,
+                 service_details: Optional['outputs.BackgroundWorkerDetailsOutput'] = None,
+                 type: Optional[str] = None):
+        pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "created_at", created_at)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "notify_on_fail", notify_on_fail)
+        pulumi.set(__self__, "owner_id", owner_id)
+        pulumi.set(__self__, "root_dir", root_dir)
+        pulumi.set(__self__, "slug", slug)
+        pulumi.set(__self__, "suspended", suspended)
+        pulumi.set(__self__, "suspenders", suspenders)
+        pulumi.set(__self__, "updated_at", updated_at)
+        if branch is not None:
+            pulumi.set(__self__, "branch", branch)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
+        if image_path is not None:
+            pulumi.set(__self__, "image_path", image_path)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
+        if service_details is not None:
+            pulumi.set(__self__, "service_details", service_details)
+        if type is None:
+            type = 'background_worker'
+        if type is not None:
+            pulumi.set(__self__, "type", type)
 
     @property
-    @pulumi.getter
-    def slug(self) -> Optional[str]:
-        return pulumi.get(self, "slug")
+    @pulumi.getter(name="autoDeploy")
+    def auto_deploy(self) -> 'ServiceAutoDeploy':
+        return pulumi.get(self, "auto_deploy")
 
     @property
-    @pulumi.getter
-    def suspended(self) -> Optional['ServiceSuspended']:
-        return pulumi.get(self, "suspended")
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> str:
+        return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
-    def suspenders(self) -> Optional[Sequence[str]]:
-        return pulumi.get(self, "suspenders")
+    def id(self) -> str:
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def type(self) -> Optional[str]:
-        return pulumi.get(self, "type")
+    def name(self) -> str:
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[str]:
-        return pulumi.get(self, "updated_at")
-
-
-@pulumi.output_type
-class BackgroundWorkerServiceDetails(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "envSpecificDetails":
-            suggest = "env_specific_details"
-        elif key == "numInstances":
-            suggest = "num_instances"
-        elif key == "parentServer":
-            suggest = "parent_server"
-        elif key == "pullRequestPreviewsEnabled":
-            suggest = "pull_request_previews_enabled"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in BackgroundWorkerServiceDetails. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        BackgroundWorkerServiceDetails.__key_warning(key)
-        return super().__getitem__(key)
+    @pulumi.getter(name="notifyOnFail")
+    def notify_on_fail(self) -> 'ServiceNotifyOnFail':
+        return pulumi.get(self, "notify_on_fail")
 
-    def get(self, key: str, default = None) -> Any:
-        BackgroundWorkerServiceDetails.__key_warning(key)
-        return super().get(key, default)
+    @property
+    @pulumi.getter(name="ownerId")
+    def owner_id(self) -> str:
+        return pulumi.get(self, "owner_id")
 
-    def __init__(__self__, *,
-                 env: 'BackgroundWorkerServiceDetailsEnv',
-                 disk: Optional['outputs.Disk'] = None,
-                 env_specific_details: Optional[Any] = None,
-                 num_instances: Optional[float] = None,
-                 parent_server: Optional['outputs.BackgroundWorkerServiceDetailsParentServerProperties'] = None,
-                 plan: Optional['BackgroundWorkerServiceDetailsPlan'] = None,
-                 pull_request_previews_enabled: Optional['BackgroundWorkerServiceDetailsPullRequestPreviewsEnabled'] = None,
-                 region: Optional['BackgroundWorkerServiceDetailsRegion'] = None,
-                 url: Optional[str] = None):
-        pulumi.set(__self__, "env", env)
-        if disk is not None:
-            pulumi.set(__self__, "disk", disk)
-        if env_specific_details is not None:
-            pulumi.set(__self__, "env_specific_details", env_specific_details)
-        if num_instances is None:
-            num_instances = 1
-        if num_instances is not None:
-            pulumi.set(__self__, "num_instances", num_instances)
-        if parent_server is not None:
-            pulumi.set(__self__, "parent_server", parent_server)
-        if plan is None:
-            plan = 'starter'
-        if plan is not None:
-            pulumi.set(__self__, "plan", plan)
-        if pull_request_previews_enabled is None:
-            pull_request_previews_enabled = 'no'
-        if pull_request_previews_enabled is not None:
-            pulumi.set(__self__, "pull_request_previews_enabled", pull_request_previews_enabled)
-        if region is None:
-            region = 'oregon'
-        if region is not None:
-            pulumi.set(__self__, "region", region)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
+    @property
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> str:
+        return pulumi.get(self, "root_dir")
 
     @property
     @pulumi.getter
-    def env(self) -> 'BackgroundWorkerServiceDetailsEnv':
-        return pulumi.get(self, "env")
+    def slug(self) -> str:
+        return pulumi.get(self, "slug")
 
     @property
     @pulumi.getter
-    def disk(self) -> Optional['outputs.Disk']:
-        return pulumi.get(self, "disk")
+    def suspended(self) -> 'ServiceSuspended':
+        return pulumi.get(self, "suspended")
 
     @property
-    @pulumi.getter(name="envSpecificDetails")
-    def env_specific_details(self) -> Optional[Any]:
-        return pulumi.get(self, "env_specific_details")
+    @pulumi.getter
+    def suspenders(self) -> Sequence['ServiceSuspendersItem']:
+        return pulumi.get(self, "suspenders")
 
     @property
-    @pulumi.getter(name="numInstances")
-    def num_instances(self) -> Optional[float]:
-        return pulumi.get(self, "num_instances")
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> str:
+        return pulumi.get(self, "updated_at")
 
     @property
-    @pulumi.getter(name="parentServer")
-    def parent_server(self) -> Optional['outputs.BackgroundWorkerServiceDetailsParentServerProperties']:
-        return pulumi.get(self, "parent_server")
+    @pulumi.getter
+    def branch(self) -> Optional[str]:
+        return pulumi.get(self, "branch")
 
     @property
-    @pulumi.getter
-    def plan(self) -> Optional['BackgroundWorkerServiceDetailsPlan']:
-        return pulumi.get(self, "plan")
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional['outputs.BuildFilter']:
+        return pulumi.get(self, "build_filter")
 
     @property
-    @pulumi.getter(name="pullRequestPreviewsEnabled")
-    def pull_request_previews_enabled(self) -> Optional['BackgroundWorkerServiceDetailsPullRequestPreviewsEnabled']:
-        return pulumi.get(self, "pull_request_previews_enabled")
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> Optional[str]:
+        return pulumi.get(self, "image_path")
 
     @property
     @pulumi.getter
-    def region(self) -> Optional['BackgroundWorkerServiceDetailsRegion']:
-        return pulumi.get(self, "region")
+    def repo(self) -> Optional[str]:
+        return pulumi.get(self, "repo")
+
+    @property
+    @pulumi.getter(name="serviceDetails")
+    def service_details(self) -> Optional['outputs.BackgroundWorkerDetailsOutput']:
+        return pulumi.get(self, "service_details")
 
     @property
     @pulumi.getter
-    def url(self) -> Optional[str]:
-        return pulumi.get(self, "url")
+    def type(self) -> Optional[str]:
+        return pulumi.get(self, "type")
 
 
 @pulumi.output_type
-class BackgroundWorkerServiceDetailsParentServerProperties(dict):
+class BuildFilter(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "ignoredPaths":
+            suggest = "ignored_paths"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in BuildFilter. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        BuildFilter.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        BuildFilter.__key_warning(key)
+        return super().get(key, default)
+
     def __init__(__self__, *,
-                 id: Optional[str] = None,
-                 name: Optional[str] = None):
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+                 ignored_paths: Sequence[str],
+                 paths: Sequence[str]):
+        pulumi.set(__self__, "ignored_paths", ignored_paths)
+        pulumi.set(__self__, "paths", paths)
 
     @property
-    @pulumi.getter
-    def id(self) -> Optional[str]:
-        return pulumi.get(self, "id")
+    @pulumi.getter(name="ignoredPaths")
+    def ignored_paths(self) -> Sequence[str]:
+        return pulumi.get(self, "ignored_paths")
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[str]:
-        return pulumi.get(self, "name")
+    def paths(self) -> Sequence[str]:
+        return pulumi.get(self, "paths")
 
 
 @pulumi.output_type
-class Commit(dict):
+class CommitProperties(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "createdAt":
             suggest = "created_at"
 
         if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in Commit. Access the value via the '{suggest}' property getter instead.")
+            pulumi.log.warn(f"Key '{key}' not found in CommitProperties. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
-        Commit.__key_warning(key)
+        CommitProperties.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
-        Commit.__key_warning(key)
+        CommitProperties.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  created_at: Optional[str] = None,
                  id: Optional[str] = None,
                  message: Optional[str] = None):
         if created_at is not None:
@@ -427,293 +481,291 @@
     @property
     @pulumi.getter
     def message(self) -> Optional[str]:
         return pulumi.get(self, "message")
 
 
 @pulumi.output_type
-class CronJob(dict):
-    """
-    A cron job
-    """
+class CronJobDetailsOutput(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "buildPlan":
+            suggest = "build_plan"
+        elif key == "envSpecificDetails":
+            suggest = "env_specific_details"
+        elif key == "lastSuccessfulRunAt":
+            suggest = "last_successful_run_at"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in CronJobDetailsOutput. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        CronJobDetailsOutput.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        CronJobDetailsOutput.__key_warning(key)
+        return super().get(key, default)
+
     def __init__(__self__, *,
-                 name: str,
-                 owner_id: str,
-                 repo: str,
-                 auto_deploy: Optional['ServiceAutoDeploy'] = None,
-                 branch: Optional[str] = None,
-                 created_at: Optional[str] = None,
-                 env_vars: Optional[Sequence['outputs.EnvVarKeyValue']] = None,
-                 notify_on_fail: Optional['ServiceNotifyOnFail'] = None,
-                 secret_files: Optional[Sequence['outputs.SecretFile']] = None,
-                 service_details: Optional['outputs.CronJobServiceDetails'] = None,
-                 slug: Optional[str] = None,
-                 suspended: Optional['ServiceSuspended'] = None,
-                 suspenders: Optional[Sequence[str]] = None,
-                 type: Optional[str] = None,
-                 updated_at: Optional[str] = None):
+                 build_plan: str,
+                 env: 'CronJobDetailsOutputEnv',
+                 env_specific_details: Any,
+                 plan: 'CronJobDetailsOutputPlan',
+                 region: 'CronJobDetailsOutputRegion',
+                 schedule: str,
+                 last_successful_run_at: Optional[str] = None):
         """
-        A cron job
-        :param str owner_id: The id of the owner (user/team).
-        :param str repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param 'ServiceAutoDeploy' auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param str branch: If left empty, this will fall back to the default branch of the repository.
-        :param 'ServiceNotifyOnFail' notify_on_fail: The notification setting for this service upon deployment failure.
+        :param 'CronJobDetailsOutputEnv' env: Environment (runtime)
+        :param 'CronJobDetailsOutputPlan' plan: The instance type to use for the preview instance. Note that base services with any paid instance type can't create preview instances with the `free` instance type.
         """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
-        if auto_deploy is None:
-            auto_deploy = 'no'
-        if auto_deploy is not None:
-            pulumi.set(__self__, "auto_deploy", auto_deploy)
-        if branch is not None:
-            pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
-        if env_vars is not None:
-            pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
-        if secret_files is not None:
-            pulumi.set(__self__, "secret_files", secret_files)
-        if service_details is not None:
-            pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
-        if type is None:
-            type = 'cron_job'
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
+        pulumi.set(__self__, "build_plan", build_plan)
+        pulumi.set(__self__, "env", env)
+        pulumi.set(__self__, "env_specific_details", env_specific_details)
+        pulumi.set(__self__, "plan", plan)
+        pulumi.set(__self__, "region", region)
+        pulumi.set(__self__, "schedule", schedule)
+        if last_successful_run_at is not None:
+            pulumi.set(__self__, "last_successful_run_at", last_successful_run_at)
 
     @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
+    @pulumi.getter(name="buildPlan")
+    def build_plan(self) -> str:
+        return pulumi.get(self, "build_plan")
 
     @property
-    @pulumi.getter(name="ownerId")
-    def owner_id(self) -> str:
+    @pulumi.getter
+    def env(self) -> 'CronJobDetailsOutputEnv':
         """
-        The id of the owner (user/team).
+        Environment (runtime)
         """
-        return pulumi.get(self, "owner_id")
+        return pulumi.get(self, "env")
+
+    @property
+    @pulumi.getter(name="envSpecificDetails")
+    def env_specific_details(self) -> Any:
+        return pulumi.get(self, "env_specific_details")
 
     @property
     @pulumi.getter
-    def repo(self) -> str:
+    def plan(self) -> 'CronJobDetailsOutputPlan':
         """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
+        The instance type to use for the preview instance. Note that base services with any paid instance type can't create preview instances with the `free` instance type.
         """
-        return pulumi.get(self, "repo")
+        return pulumi.get(self, "plan")
 
     @property
-    @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional['ServiceAutoDeploy']:
-        """
-        Whether to auto deploy the service or not upon git push.
-        """
-        return pulumi.get(self, "auto_deploy")
+    @pulumi.getter
+    def region(self) -> 'CronJobDetailsOutputRegion':
+        return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
-    def branch(self) -> Optional[str]:
-        """
-        If left empty, this will fall back to the default branch of the repository.
-        """
-        return pulumi.get(self, "branch")
+    def schedule(self) -> str:
+        return pulumi.get(self, "schedule")
+
+    @property
+    @pulumi.getter(name="lastSuccessfulRunAt")
+    def last_successful_run_at(self) -> Optional[str]:
+        return pulumi.get(self, "last_successful_run_at")
+
+
+@pulumi.output_type
+class CronJobOutput(dict):
+    def __init__(__self__, *,
+                 auto_deploy: 'ServiceAutoDeploy',
+                 created_at: str,
+                 id: str,
+                 name: str,
+                 notify_on_fail: 'ServiceNotifyOnFail',
+                 owner_id: str,
+                 root_dir: str,
+                 slug: str,
+                 suspended: 'ServiceSuspended',
+                 suspenders: Sequence['ServiceSuspendersItem'],
+                 updated_at: str,
+                 branch: Optional[str] = None,
+                 build_filter: Optional['outputs.BuildFilter'] = None,
+                 image_path: Optional[str] = None,
+                 repo: Optional[str] = None,
+                 service_details: Optional['outputs.CronJobDetailsOutput'] = None,
+                 type: Optional[str] = None):
+        pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "created_at", created_at)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "notify_on_fail", notify_on_fail)
+        pulumi.set(__self__, "owner_id", owner_id)
+        pulumi.set(__self__, "root_dir", root_dir)
+        pulumi.set(__self__, "slug", slug)
+        pulumi.set(__self__, "suspended", suspended)
+        pulumi.set(__self__, "suspenders", suspenders)
+        pulumi.set(__self__, "updated_at", updated_at)
+        if branch is not None:
+            pulumi.set(__self__, "branch", branch)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
+        if image_path is not None:
+            pulumi.set(__self__, "image_path", image_path)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
+        if service_details is not None:
+            pulumi.set(__self__, "service_details", service_details)
+        if type is None:
+            type = 'cron_job'
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter(name="autoDeploy")
+    def auto_deploy(self) -> 'ServiceAutoDeploy':
+        return pulumi.get(self, "auto_deploy")
 
     @property
     @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
+    def created_at(self) -> str:
         return pulumi.get(self, "created_at")
 
     @property
-    @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[Sequence['outputs.EnvVarKeyValue']]:
-        return pulumi.get(self, "env_vars")
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional['ServiceNotifyOnFail']:
-        """
-        The notification setting for this service upon deployment failure.
-        """
+    def notify_on_fail(self) -> 'ServiceNotifyOnFail':
         return pulumi.get(self, "notify_on_fail")
 
     @property
-    @pulumi.getter(name="secretFiles")
-    def secret_files(self) -> Optional[Sequence['outputs.SecretFile']]:
-        return pulumi.get(self, "secret_files")
+    @pulumi.getter(name="ownerId")
+    def owner_id(self) -> str:
+        return pulumi.get(self, "owner_id")
 
     @property
-    @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional['outputs.CronJobServiceDetails']:
-        return pulumi.get(self, "service_details")
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> str:
+        return pulumi.get(self, "root_dir")
 
     @property
     @pulumi.getter
-    def slug(self) -> Optional[str]:
+    def slug(self) -> str:
         return pulumi.get(self, "slug")
 
     @property
     @pulumi.getter
-    def suspended(self) -> Optional['ServiceSuspended']:
+    def suspended(self) -> 'ServiceSuspended':
         return pulumi.get(self, "suspended")
 
     @property
     @pulumi.getter
-    def suspenders(self) -> Optional[Sequence[str]]:
+    def suspenders(self) -> Sequence['ServiceSuspendersItem']:
         return pulumi.get(self, "suspenders")
 
     @property
-    @pulumi.getter
-    def type(self) -> Optional[str]:
-        return pulumi.get(self, "type")
-
-    @property
     @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[str]:
+    def updated_at(self) -> str:
         return pulumi.get(self, "updated_at")
 
-
-@pulumi.output_type
-class CronJobServiceDetails(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "envSpecificDetails":
-            suggest = "env_specific_details"
-        elif key == "lastSuccessfulRunAt":
-            suggest = "last_successful_run_at"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in CronJobServiceDetails. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        CronJobServiceDetails.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        CronJobServiceDetails.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 env: 'CronJobServiceDetailsEnv',
-                 schedule: str,
-                 env_specific_details: Optional[Any] = None,
-                 last_successful_run_at: Optional[str] = None,
-                 plan: Optional['CronJobServiceDetailsPlan'] = None,
-                 region: Optional['CronJobServiceDetailsRegion'] = None):
-        pulumi.set(__self__, "env", env)
-        pulumi.set(__self__, "schedule", schedule)
-        if env_specific_details is not None:
-            pulumi.set(__self__, "env_specific_details", env_specific_details)
-        if last_successful_run_at is not None:
-            pulumi.set(__self__, "last_successful_run_at", last_successful_run_at)
-        if plan is None:
-            plan = 'starter'
-        if plan is not None:
-            pulumi.set(__self__, "plan", plan)
-        if region is None:
-            region = 'oregon'
-        if region is not None:
-            pulumi.set(__self__, "region", region)
-
     @property
     @pulumi.getter
-    def env(self) -> 'CronJobServiceDetailsEnv':
-        return pulumi.get(self, "env")
+    def branch(self) -> Optional[str]:
+        return pulumi.get(self, "branch")
 
     @property
-    @pulumi.getter
-    def schedule(self) -> str:
-        return pulumi.get(self, "schedule")
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional['outputs.BuildFilter']:
+        return pulumi.get(self, "build_filter")
 
     @property
-    @pulumi.getter(name="envSpecificDetails")
-    def env_specific_details(self) -> Optional[Any]:
-        return pulumi.get(self, "env_specific_details")
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> Optional[str]:
+        return pulumi.get(self, "image_path")
 
     @property
-    @pulumi.getter(name="lastSuccessfulRunAt")
-    def last_successful_run_at(self) -> Optional[str]:
-        return pulumi.get(self, "last_successful_run_at")
+    @pulumi.getter
+    def repo(self) -> Optional[str]:
+        return pulumi.get(self, "repo")
 
     @property
-    @pulumi.getter
-    def plan(self) -> Optional['CronJobServiceDetailsPlan']:
-        return pulumi.get(self, "plan")
+    @pulumi.getter(name="serviceDetails")
+    def service_details(self) -> Optional['outputs.CronJobDetailsOutput']:
+        return pulumi.get(self, "service_details")
 
     @property
     @pulumi.getter
-    def region(self) -> Optional['CronJobServiceDetailsRegion']:
-        return pulumi.get(self, "region")
+    def type(self) -> Optional[str]:
+        return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class CustomDomain(dict):
     def __init__(__self__, *,
+                 created_at: str,
                  domain_type: 'CustomDomainDomainType',
+                 id: str,
                  name: str,
+                 public_suffix: str,
                  redirect_for_name: str,
-                 server: 'outputs.CustomDomainServerProperties',
                  verification_status: 'CustomDomainVerificationStatus',
-                 created_at: Optional[str] = None,
-                 public_suffix: Optional[str] = None):
+                 server: Optional['outputs.CustomDomainServerProperties'] = None):
+        pulumi.set(__self__, "created_at", created_at)
         pulumi.set(__self__, "domain_type", domain_type)
+        pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "public_suffix", public_suffix)
         pulumi.set(__self__, "redirect_for_name", redirect_for_name)
-        pulumi.set(__self__, "server", server)
         pulumi.set(__self__, "verification_status", verification_status)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
-        if public_suffix is not None:
-            pulumi.set(__self__, "public_suffix", public_suffix)
+        if server is not None:
+            pulumi.set(__self__, "server", server)
+
+    @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> str:
+        return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter(name="domainType")
     def domain_type(self) -> 'CustomDomainDomainType':
         return pulumi.get(self, "domain_type")
 
     @property
     @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="publicSuffix")
+    def public_suffix(self) -> str:
+        return pulumi.get(self, "public_suffix")
+
+    @property
     @pulumi.getter(name="redirectForName")
     def redirect_for_name(self) -> str:
         return pulumi.get(self, "redirect_for_name")
 
     @property
-    @pulumi.getter
-    def server(self) -> 'outputs.CustomDomainServerProperties':
-        return pulumi.get(self, "server")
-
-    @property
     @pulumi.getter(name="verificationStatus")
     def verification_status(self) -> 'CustomDomainVerificationStatus':
         return pulumi.get(self, "verification_status")
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
-        return pulumi.get(self, "created_at")
-
-    @property
-    @pulumi.getter(name="publicSuffix")
-    def public_suffix(self) -> Optional[str]:
-        return pulumi.get(self, "public_suffix")
+    @pulumi.getter
+    def server(self) -> Optional['outputs.CustomDomainServerProperties']:
+        return pulumi.get(self, "server")
 
 
 @pulumi.output_type
 class CustomDomainServerProperties(dict):
     def __init__(__self__, *,
                  id: Optional[str] = None,
                  name: Optional[str] = None):
@@ -732,33 +784,160 @@
     def name(self) -> Optional[str]:
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
 class Deploy(dict):
     def __init__(__self__, *,
-                 clear_cache: Optional['DeployClearCache'] = None,
-                 commit: Optional['outputs.Commit'] = None):
-        if clear_cache is None:
-            clear_cache = 'do_not_clear'
-        if clear_cache is not None:
-            pulumi.set(__self__, "clear_cache", clear_cache)
+                 id: str,
+                 commit: Optional['outputs.DeployCommitProperties'] = None,
+                 created_at: Optional[str] = None,
+                 finished_at: Optional[str] = None,
+                 image: Optional['outputs.DeployImageProperties'] = None,
+                 status: Optional['DeployStatus'] = None,
+                 trigger: Optional['DeployTrigger'] = None,
+                 updated_at: Optional[str] = None):
+        """
+        :param 'DeployImageProperties' image: Image information used when creating the deploy. Not present for Git-backed deploys
+        """
+        pulumi.set(__self__, "id", id)
         if commit is not None:
             pulumi.set(__self__, "commit", commit)
+        if created_at is not None:
+            pulumi.set(__self__, "created_at", created_at)
+        if finished_at is not None:
+            pulumi.set(__self__, "finished_at", finished_at)
+        if image is not None:
+            pulumi.set(__self__, "image", image)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
+        if trigger is not None:
+            pulumi.set(__self__, "trigger", trigger)
+        if updated_at is not None:
+            pulumi.set(__self__, "updated_at", updated_at)
 
     @property
-    @pulumi.getter(name="clearCache")
-    def clear_cache(self) -> Optional['DeployClearCache']:
-        return pulumi.get(self, "clear_cache")
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def commit(self) -> Optional['outputs.Commit']:
+    def commit(self) -> Optional['outputs.DeployCommitProperties']:
         return pulumi.get(self, "commit")
 
+    @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> Optional[str]:
+        return pulumi.get(self, "created_at")
+
+    @property
+    @pulumi.getter(name="finishedAt")
+    def finished_at(self) -> Optional[str]:
+        return pulumi.get(self, "finished_at")
+
+    @property
+    @pulumi.getter
+    def image(self) -> Optional['outputs.DeployImageProperties']:
+        """
+        Image information used when creating the deploy. Not present for Git-backed deploys
+        """
+        return pulumi.get(self, "image")
+
+    @property
+    @pulumi.getter
+    def status(self) -> Optional['DeployStatus']:
+        return pulumi.get(self, "status")
+
+    @property
+    @pulumi.getter
+    def trigger(self) -> Optional['DeployTrigger']:
+        return pulumi.get(self, "trigger")
+
+    @property
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> Optional[str]:
+        return pulumi.get(self, "updated_at")
+
+
+@pulumi.output_type
+class DeployCommitProperties(dict):
+    def __init__(__self__, *,
+                 created_at: Optional[str] = None,
+                 id: Optional[str] = None,
+                 message: Optional[str] = None):
+        if created_at is not None:
+            pulumi.set(__self__, "created_at", created_at)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if message is not None:
+            pulumi.set(__self__, "message", message)
+
+    @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> Optional[str]:
+        return pulumi.get(self, "created_at")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def message(self) -> Optional[str]:
+        return pulumi.get(self, "message")
+
+
+@pulumi.output_type
+class DeployImageProperties(dict):
+    """
+    Image information used when creating the deploy. Not present for Git-backed deploys
+    """
+    def __init__(__self__, *,
+                 ref: Optional[str] = None,
+                 registry_credential: Optional[str] = None,
+                 sha: Optional[str] = None):
+        """
+        Image information used when creating the deploy. Not present for Git-backed deploys
+        :param str ref: Image reference used when creating the deploy
+        :param str registry_credential: Name of credential used to pull the image, if provided
+        :param str sha: SHA that the image reference was resolved to when creating the deploy
+        """
+        if ref is not None:
+            pulumi.set(__self__, "ref", ref)
+        if registry_credential is not None:
+            pulumi.set(__self__, "registry_credential", registry_credential)
+        if sha is not None:
+            pulumi.set(__self__, "sha", sha)
+
+    @property
+    @pulumi.getter
+    def ref(self) -> Optional[str]:
+        """
+        Image reference used when creating the deploy
+        """
+        return pulumi.get(self, "ref")
+
+    @property
+    @pulumi.getter(name="registryCredential")
+    def registry_credential(self) -> Optional[str]:
+        """
+        Name of credential used to pull the image, if provided
+        """
+        return pulumi.get(self, "registry_credential")
+
+    @property
+    @pulumi.getter
+    def sha(self) -> Optional[str]:
+        """
+        SHA that the image reference was resolved to when creating the deploy
+        """
+        return pulumi.get(self, "sha")
+
 
 @pulumi.output_type
 class Disk(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "mountPath":
@@ -774,51 +953,59 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         Disk.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
+                 id: str,
                  mount_path: str,
                  name: str,
-                 size_gb: Optional[float] = None):
+                 size_gb: int):
+        pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "mount_path", mount_path)
         pulumi.set(__self__, "name", name)
-        if size_gb is None:
-            size_gb = 1
-        if size_gb is not None:
-            pulumi.set(__self__, "size_gb", size_gb)
+        pulumi.set(__self__, "size_gb", size_gb)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="mountPath")
     def mount_path(self) -> str:
         return pulumi.get(self, "mount_path")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="sizeGB")
-    def size_gb(self) -> Optional[float]:
+    def size_gb(self) -> int:
         return pulumi.get(self, "size_gb")
 
 
 @pulumi.output_type
 class DockerDetails(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "dockerCommand":
             suggest = "docker_command"
         elif key == "dockerContext":
             suggest = "docker_context"
         elif key == "dockerfilePath":
             suggest = "dockerfile_path"
+        elif key == "preDeployCommand":
+            suggest = "pre_deploy_command"
+        elif key == "registryCredential":
+            suggest = "registry_credential"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in DockerDetails. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         DockerDetails.__key_warning(key)
         return super().__getitem__(key)
@@ -826,877 +1013,1012 @@
     def get(self, key: str, default = None) -> Any:
         DockerDetails.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  docker_command: str,
                  docker_context: str,
-                 dockerfile_path: Optional[str] = None):
+                 dockerfile_path: str,
+                 pre_deploy_command: Optional[str] = None,
+                 registry_credential: Optional['outputs.RegistryCredential'] = None):
         pulumi.set(__self__, "docker_command", docker_command)
         pulumi.set(__self__, "docker_context", docker_context)
-        if dockerfile_path is not None:
-            pulumi.set(__self__, "dockerfile_path", dockerfile_path)
+        pulumi.set(__self__, "dockerfile_path", dockerfile_path)
+        if pre_deploy_command is not None:
+            pulumi.set(__self__, "pre_deploy_command", pre_deploy_command)
+        if registry_credential is not None:
+            pulumi.set(__self__, "registry_credential", registry_credential)
 
     @property
     @pulumi.getter(name="dockerCommand")
     def docker_command(self) -> str:
         return pulumi.get(self, "docker_command")
 
     @property
     @pulumi.getter(name="dockerContext")
     def docker_context(self) -> str:
         return pulumi.get(self, "docker_context")
 
     @property
     @pulumi.getter(name="dockerfilePath")
-    def dockerfile_path(self) -> Optional[str]:
+    def dockerfile_path(self) -> str:
         return pulumi.get(self, "dockerfile_path")
 
+    @property
+    @pulumi.getter(name="preDeployCommand")
+    def pre_deploy_command(self) -> Optional[str]:
+        return pulumi.get(self, "pre_deploy_command")
+
+    @property
+    @pulumi.getter(name="registryCredential")
+    def registry_credential(self) -> Optional['outputs.RegistryCredential']:
+        return pulumi.get(self, "registry_credential")
+
 
 @pulumi.output_type
-class EnvVarKeyValue(dict):
+class EnvVar(dict):
+    def __init__(__self__, *,
+                 key: str,
+                 value: str):
+        pulumi.set(__self__, "key", key)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> str:
+        return pulumi.get(self, "key")
+
+    @property
+    @pulumi.getter
+    def value(self) -> str:
+        return pulumi.get(self, "value")
+
+
+@pulumi.output_type
+class EnvVarKeyGenerateValue(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "generateValue":
             suggest = "generate_value"
 
         if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in EnvVarKeyValue. Access the value via the '{suggest}' property getter instead.")
+            pulumi.log.warn(f"Key '{key}' not found in EnvVarKeyGenerateValue. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
-        EnvVarKeyValue.__key_warning(key)
+        EnvVarKeyGenerateValue.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
-        EnvVarKeyValue.__key_warning(key)
+        EnvVarKeyGenerateValue.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 key: str,
-                 generate_value: Optional['EnvVarKeyValueGenerateValue'] = None,
-                 value: Optional[str] = None):
+                 generate_value: bool,
+                 key: str):
+        pulumi.set(__self__, "generate_value", generate_value)
         pulumi.set(__self__, "key", key)
-        if generate_value is not None:
-            pulumi.set(__self__, "generate_value", generate_value)
-        if value is not None:
-            pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter(name="generateValue")
+    def generate_value(self) -> bool:
+        return pulumi.get(self, "generate_value")
 
     @property
     @pulumi.getter
     def key(self) -> str:
         return pulumi.get(self, "key")
 
+
+@pulumi.output_type
+class EnvVarKeyValue(dict):
+    def __init__(__self__, *,
+                 key: str,
+                 value: str):
+        pulumi.set(__self__, "key", key)
+        pulumi.set(__self__, "value", value)
+
     @property
-    @pulumi.getter(name="generateValue")
-    def generate_value(self) -> Optional['EnvVarKeyValueGenerateValue']:
-        return pulumi.get(self, "generate_value")
+    @pulumi.getter
+    def key(self) -> str:
+        return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
-    def value(self) -> Optional[str]:
+    def value(self) -> str:
         return pulumi.get(self, "value")
 
 
 @pulumi.output_type
+class EnvVarWithCursor(dict):
+    def __init__(__self__, *,
+                 cursor: str,
+                 env_var: 'outputs.EnvVar'):
+        pulumi.set(__self__, "cursor", cursor)
+        pulumi.set(__self__, "env_var", env_var)
+
+    @property
+    @pulumi.getter
+    def cursor(self) -> str:
+        return pulumi.get(self, "cursor")
+
+    @property
+    @pulumi.getter(name="envVar")
+    def env_var(self) -> 'outputs.EnvVar':
+        return pulumi.get(self, "env_var")
+
+
+@pulumi.output_type
 class GetBackgroundWorker(dict):
-    """
-    A background worker service
-    """
     def __init__(__self__, *,
+                 auto_deploy: 'ServiceAutoDeploy',
+                 created_at: str,
+                 id: str,
                  name: str,
+                 notify_on_fail: 'ServiceNotifyOnFail',
                  owner_id: str,
-                 repo: str,
-                 auto_deploy: Optional['ServiceAutoDeploy'] = None,
+                 root_dir: str,
+                 slug: str,
+                 suspended: 'ServiceSuspended',
+                 suspenders: Sequence['ServiceSuspendersItem'],
+                 updated_at: str,
                  branch: Optional[str] = None,
-                 created_at: Optional[str] = None,
-                 env_vars: Optional[Sequence['outputs.EnvVarKeyValue']] = None,
-                 notify_on_fail: Optional['ServiceNotifyOnFail'] = None,
-                 secret_files: Optional[Sequence['outputs.SecretFile']] = None,
-                 service_details: Optional['outputs.BackgroundWorkerServiceDetails'] = None,
-                 slug: Optional[str] = None,
-                 suspended: Optional['ServiceSuspended'] = None,
-                 suspenders: Optional[Sequence[str]] = None,
-                 type: Optional[str] = None,
-                 updated_at: Optional[str] = None):
-        """
-        A background worker service
-        :param str owner_id: The id of the owner (user/team).
-        :param str repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param 'ServiceAutoDeploy' auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param str branch: If left empty, this will fall back to the default branch of the repository.
-        :param 'ServiceNotifyOnFail' notify_on_fail: The notification setting for this service upon deployment failure.
-        """
+                 build_filter: Optional['outputs.BuildFilter'] = None,
+                 image_path: Optional[str] = None,
+                 repo: Optional[str] = None,
+                 service_details: Optional['outputs.BackgroundWorkerDetailsOutput'] = None,
+                 type: Optional[str] = None):
+        pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "created_at", created_at)
+        pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "notify_on_fail", notify_on_fail)
         pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
-        if auto_deploy is None:
-            auto_deploy = 'no'
-        if auto_deploy is not None:
-            pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "root_dir", root_dir)
+        pulumi.set(__self__, "slug", slug)
+        pulumi.set(__self__, "suspended", suspended)
+        pulumi.set(__self__, "suspenders", suspenders)
+        pulumi.set(__self__, "updated_at", updated_at)
         if branch is not None:
             pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
-        if env_vars is not None:
-            pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
-        if secret_files is not None:
-            pulumi.set(__self__, "secret_files", secret_files)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
+        if image_path is not None:
+            pulumi.set(__self__, "image_path", image_path)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
         if service_details is not None:
             pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
         if type is None:
             type = 'background_worker'
         if type is not None:
             pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
+
+    @property
+    @pulumi.getter(name="autoDeploy")
+    def auto_deploy(self) -> 'ServiceAutoDeploy':
+        return pulumi.get(self, "auto_deploy")
+
+    @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> str:
+        return pulumi.get(self, "created_at")
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="notifyOnFail")
+    def notify_on_fail(self) -> 'ServiceNotifyOnFail':
+        return pulumi.get(self, "notify_on_fail")
+
+    @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> str:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @property
-    @pulumi.getter
-    def repo(self) -> str:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
-        return pulumi.get(self, "repo")
-
-    @property
-    @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional['ServiceAutoDeploy']:
-        """
-        Whether to auto deploy the service or not upon git push.
-        """
-        return pulumi.get(self, "auto_deploy")
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> str:
+        return pulumi.get(self, "root_dir")
 
     @property
     @pulumi.getter
-    def branch(self) -> Optional[str]:
-        """
-        If left empty, this will fall back to the default branch of the repository.
-        """
-        return pulumi.get(self, "branch")
+    def slug(self) -> str:
+        return pulumi.get(self, "slug")
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
-        return pulumi.get(self, "created_at")
+    @pulumi.getter
+    def suspended(self) -> 'ServiceSuspended':
+        return pulumi.get(self, "suspended")
 
     @property
-    @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[Sequence['outputs.EnvVarKeyValue']]:
-        return pulumi.get(self, "env_vars")
+    @pulumi.getter
+    def suspenders(self) -> Sequence['ServiceSuspendersItem']:
+        return pulumi.get(self, "suspenders")
 
     @property
-    @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional['ServiceNotifyOnFail']:
-        """
-        The notification setting for this service upon deployment failure.
-        """
-        return pulumi.get(self, "notify_on_fail")
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> str:
+        return pulumi.get(self, "updated_at")
 
     @property
-    @pulumi.getter(name="secretFiles")
-    def secret_files(self) -> Optional[Sequence['outputs.SecretFile']]:
-        return pulumi.get(self, "secret_files")
+    @pulumi.getter
+    def branch(self) -> Optional[str]:
+        return pulumi.get(self, "branch")
 
     @property
-    @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional['outputs.BackgroundWorkerServiceDetails']:
-        return pulumi.get(self, "service_details")
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional['outputs.BuildFilter']:
+        return pulumi.get(self, "build_filter")
 
     @property
-    @pulumi.getter
-    def slug(self) -> Optional[str]:
-        return pulumi.get(self, "slug")
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> Optional[str]:
+        return pulumi.get(self, "image_path")
 
     @property
     @pulumi.getter
-    def suspended(self) -> Optional['ServiceSuspended']:
-        return pulumi.get(self, "suspended")
+    def repo(self) -> Optional[str]:
+        return pulumi.get(self, "repo")
 
     @property
-    @pulumi.getter
-    def suspenders(self) -> Optional[Sequence[str]]:
-        return pulumi.get(self, "suspenders")
+    @pulumi.getter(name="serviceDetails")
+    def service_details(self) -> Optional['outputs.BackgroundWorkerDetailsOutput']:
+        return pulumi.get(self, "service_details")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         return pulumi.get(self, "type")
 
-    @property
-    @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[str]:
-        return pulumi.get(self, "updated_at")
-
 
 @pulumi.output_type
 class GetCronJob(dict):
-    """
-    A cron job
-    """
     def __init__(__self__, *,
+                 auto_deploy: 'ServiceAutoDeploy',
+                 created_at: str,
+                 id: str,
                  name: str,
+                 notify_on_fail: 'ServiceNotifyOnFail',
                  owner_id: str,
-                 repo: str,
-                 auto_deploy: Optional['ServiceAutoDeploy'] = None,
+                 root_dir: str,
+                 slug: str,
+                 suspended: 'ServiceSuspended',
+                 suspenders: Sequence['ServiceSuspendersItem'],
+                 updated_at: str,
                  branch: Optional[str] = None,
-                 created_at: Optional[str] = None,
-                 env_vars: Optional[Sequence['outputs.EnvVarKeyValue']] = None,
-                 notify_on_fail: Optional['ServiceNotifyOnFail'] = None,
-                 secret_files: Optional[Sequence['outputs.SecretFile']] = None,
-                 service_details: Optional['outputs.CronJobServiceDetails'] = None,
-                 slug: Optional[str] = None,
-                 suspended: Optional['ServiceSuspended'] = None,
-                 suspenders: Optional[Sequence[str]] = None,
-                 type: Optional[str] = None,
-                 updated_at: Optional[str] = None):
-        """
-        A cron job
-        :param str owner_id: The id of the owner (user/team).
-        :param str repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param 'ServiceAutoDeploy' auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param str branch: If left empty, this will fall back to the default branch of the repository.
-        :param 'ServiceNotifyOnFail' notify_on_fail: The notification setting for this service upon deployment failure.
-        """
+                 build_filter: Optional['outputs.BuildFilter'] = None,
+                 image_path: Optional[str] = None,
+                 repo: Optional[str] = None,
+                 service_details: Optional['outputs.CronJobDetailsOutput'] = None,
+                 type: Optional[str] = None):
+        pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "created_at", created_at)
+        pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "notify_on_fail", notify_on_fail)
         pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
-        if auto_deploy is None:
-            auto_deploy = 'no'
-        if auto_deploy is not None:
-            pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "root_dir", root_dir)
+        pulumi.set(__self__, "slug", slug)
+        pulumi.set(__self__, "suspended", suspended)
+        pulumi.set(__self__, "suspenders", suspenders)
+        pulumi.set(__self__, "updated_at", updated_at)
         if branch is not None:
             pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
-        if env_vars is not None:
-            pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
-        if secret_files is not None:
-            pulumi.set(__self__, "secret_files", secret_files)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
+        if image_path is not None:
+            pulumi.set(__self__, "image_path", image_path)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
         if service_details is not None:
             pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
         if type is None:
             type = 'cron_job'
         if type is not None:
             pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
+
+    @property
+    @pulumi.getter(name="autoDeploy")
+    def auto_deploy(self) -> 'ServiceAutoDeploy':
+        return pulumi.get(self, "auto_deploy")
+
+    @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> str:
+        return pulumi.get(self, "created_at")
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="notifyOnFail")
+    def notify_on_fail(self) -> 'ServiceNotifyOnFail':
+        return pulumi.get(self, "notify_on_fail")
+
+    @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> str:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @property
-    @pulumi.getter
-    def repo(self) -> str:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
-        return pulumi.get(self, "repo")
-
-    @property
-    @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional['ServiceAutoDeploy']:
-        """
-        Whether to auto deploy the service or not upon git push.
-        """
-        return pulumi.get(self, "auto_deploy")
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> str:
+        return pulumi.get(self, "root_dir")
 
     @property
     @pulumi.getter
-    def branch(self) -> Optional[str]:
-        """
-        If left empty, this will fall back to the default branch of the repository.
-        """
-        return pulumi.get(self, "branch")
+    def slug(self) -> str:
+        return pulumi.get(self, "slug")
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
-        return pulumi.get(self, "created_at")
+    @pulumi.getter
+    def suspended(self) -> 'ServiceSuspended':
+        return pulumi.get(self, "suspended")
 
     @property
-    @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[Sequence['outputs.EnvVarKeyValue']]:
-        return pulumi.get(self, "env_vars")
+    @pulumi.getter
+    def suspenders(self) -> Sequence['ServiceSuspendersItem']:
+        return pulumi.get(self, "suspenders")
 
     @property
-    @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional['ServiceNotifyOnFail']:
-        """
-        The notification setting for this service upon deployment failure.
-        """
-        return pulumi.get(self, "notify_on_fail")
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> str:
+        return pulumi.get(self, "updated_at")
 
     @property
-    @pulumi.getter(name="secretFiles")
-    def secret_files(self) -> Optional[Sequence['outputs.SecretFile']]:
-        return pulumi.get(self, "secret_files")
+    @pulumi.getter
+    def branch(self) -> Optional[str]:
+        return pulumi.get(self, "branch")
 
     @property
-    @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional['outputs.CronJobServiceDetails']:
-        return pulumi.get(self, "service_details")
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional['outputs.BuildFilter']:
+        return pulumi.get(self, "build_filter")
 
     @property
-    @pulumi.getter
-    def slug(self) -> Optional[str]:
-        return pulumi.get(self, "slug")
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> Optional[str]:
+        return pulumi.get(self, "image_path")
 
     @property
     @pulumi.getter
-    def suspended(self) -> Optional['ServiceSuspended']:
-        return pulumi.get(self, "suspended")
+    def repo(self) -> Optional[str]:
+        return pulumi.get(self, "repo")
 
     @property
-    @pulumi.getter
-    def suspenders(self) -> Optional[Sequence[str]]:
-        return pulumi.get(self, "suspenders")
+    @pulumi.getter(name="serviceDetails")
+    def service_details(self) -> Optional['outputs.CronJobDetailsOutput']:
+        return pulumi.get(self, "service_details")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         return pulumi.get(self, "type")
 
-    @property
-    @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[str]:
-        return pulumi.get(self, "updated_at")
-
 
 @pulumi.output_type
 class GetPrivateService(dict):
-    """
-    A private service
-    """
     def __init__(__self__, *,
+                 auto_deploy: 'ServiceAutoDeploy',
+                 created_at: str,
+                 id: str,
                  name: str,
+                 notify_on_fail: 'ServiceNotifyOnFail',
                  owner_id: str,
-                 repo: str,
-                 auto_deploy: Optional['ServiceAutoDeploy'] = None,
+                 root_dir: str,
+                 slug: str,
+                 suspended: 'ServiceSuspended',
+                 suspenders: Sequence['ServiceSuspendersItem'],
+                 updated_at: str,
                  branch: Optional[str] = None,
-                 created_at: Optional[str] = None,
-                 env_vars: Optional[Sequence['outputs.EnvVarKeyValue']] = None,
-                 notify_on_fail: Optional['ServiceNotifyOnFail'] = None,
-                 secret_files: Optional[Sequence['outputs.SecretFile']] = None,
-                 service_details: Optional['outputs.PrivateServiceDetails'] = None,
-                 slug: Optional[str] = None,
-                 suspended: Optional['ServiceSuspended'] = None,
-                 suspenders: Optional[Sequence[str]] = None,
-                 type: Optional[str] = None,
-                 updated_at: Optional[str] = None):
-        """
-        A private service
-        :param str owner_id: The id of the owner (user/team).
-        :param str repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param 'ServiceAutoDeploy' auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param str branch: If left empty, this will fall back to the default branch of the repository.
-        :param 'ServiceNotifyOnFail' notify_on_fail: The notification setting for this service upon deployment failure.
-        """
+                 build_filter: Optional['outputs.BuildFilter'] = None,
+                 image_path: Optional[str] = None,
+                 repo: Optional[str] = None,
+                 service_details: Optional['outputs.PrivateServiceDetailsOutput'] = None,
+                 type: Optional[str] = None):
+        pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "created_at", created_at)
+        pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "notify_on_fail", notify_on_fail)
         pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
-        if auto_deploy is None:
-            auto_deploy = 'no'
-        if auto_deploy is not None:
-            pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "root_dir", root_dir)
+        pulumi.set(__self__, "slug", slug)
+        pulumi.set(__self__, "suspended", suspended)
+        pulumi.set(__self__, "suspenders", suspenders)
+        pulumi.set(__self__, "updated_at", updated_at)
         if branch is not None:
             pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
-        if env_vars is not None:
-            pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
-        if secret_files is not None:
-            pulumi.set(__self__, "secret_files", secret_files)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
+        if image_path is not None:
+            pulumi.set(__self__, "image_path", image_path)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
         if service_details is not None:
             pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
         if type is None:
             type = 'private_service'
         if type is not None:
             pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
+
+    @property
+    @pulumi.getter(name="autoDeploy")
+    def auto_deploy(self) -> 'ServiceAutoDeploy':
+        return pulumi.get(self, "auto_deploy")
+
+    @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> str:
+        return pulumi.get(self, "created_at")
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="notifyOnFail")
+    def notify_on_fail(self) -> 'ServiceNotifyOnFail':
+        return pulumi.get(self, "notify_on_fail")
+
+    @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> str:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @property
-    @pulumi.getter
-    def repo(self) -> str:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
-        return pulumi.get(self, "repo")
-
-    @property
-    @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional['ServiceAutoDeploy']:
-        """
-        Whether to auto deploy the service or not upon git push.
-        """
-        return pulumi.get(self, "auto_deploy")
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> str:
+        return pulumi.get(self, "root_dir")
 
     @property
     @pulumi.getter
-    def branch(self) -> Optional[str]:
-        """
-        If left empty, this will fall back to the default branch of the repository.
-        """
-        return pulumi.get(self, "branch")
+    def slug(self) -> str:
+        return pulumi.get(self, "slug")
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
-        return pulumi.get(self, "created_at")
+    @pulumi.getter
+    def suspended(self) -> 'ServiceSuspended':
+        return pulumi.get(self, "suspended")
 
     @property
-    @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[Sequence['outputs.EnvVarKeyValue']]:
-        return pulumi.get(self, "env_vars")
+    @pulumi.getter
+    def suspenders(self) -> Sequence['ServiceSuspendersItem']:
+        return pulumi.get(self, "suspenders")
 
     @property
-    @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional['ServiceNotifyOnFail']:
-        """
-        The notification setting for this service upon deployment failure.
-        """
-        return pulumi.get(self, "notify_on_fail")
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> str:
+        return pulumi.get(self, "updated_at")
 
     @property
-    @pulumi.getter(name="secretFiles")
-    def secret_files(self) -> Optional[Sequence['outputs.SecretFile']]:
-        return pulumi.get(self, "secret_files")
+    @pulumi.getter
+    def branch(self) -> Optional[str]:
+        return pulumi.get(self, "branch")
 
     @property
-    @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional['outputs.PrivateServiceDetails']:
-        return pulumi.get(self, "service_details")
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional['outputs.BuildFilter']:
+        return pulumi.get(self, "build_filter")
 
     @property
-    @pulumi.getter
-    def slug(self) -> Optional[str]:
-        return pulumi.get(self, "slug")
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> Optional[str]:
+        return pulumi.get(self, "image_path")
 
     @property
     @pulumi.getter
-    def suspended(self) -> Optional['ServiceSuspended']:
-        return pulumi.get(self, "suspended")
+    def repo(self) -> Optional[str]:
+        return pulumi.get(self, "repo")
 
     @property
-    @pulumi.getter
-    def suspenders(self) -> Optional[Sequence[str]]:
-        return pulumi.get(self, "suspenders")
+    @pulumi.getter(name="serviceDetails")
+    def service_details(self) -> Optional['outputs.PrivateServiceDetailsOutput']:
+        return pulumi.get(self, "service_details")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         return pulumi.get(self, "type")
 
-    @property
-    @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[str]:
-        return pulumi.get(self, "updated_at")
-
 
 @pulumi.output_type
 class GetStaticSite(dict):
-    """
-    A static website service
-    """
     def __init__(__self__, *,
+                 auto_deploy: 'ServiceAutoDeploy',
+                 created_at: str,
+                 id: str,
                  name: str,
+                 notify_on_fail: 'ServiceNotifyOnFail',
                  owner_id: str,
-                 repo: str,
-                 auto_deploy: Optional['ServiceAutoDeploy'] = None,
+                 root_dir: str,
+                 slug: str,
+                 suspended: 'ServiceSuspended',
+                 suspenders: Sequence['ServiceSuspendersItem'],
+                 updated_at: str,
                  branch: Optional[str] = None,
-                 created_at: Optional[str] = None,
-                 env_vars: Optional[Sequence['outputs.EnvVarKeyValue']] = None,
-                 notify_on_fail: Optional['ServiceNotifyOnFail'] = None,
-                 secret_files: Optional[Sequence['outputs.SecretFile']] = None,
-                 service_details: Optional['outputs.StaticSiteServiceDetails'] = None,
-                 slug: Optional[str] = None,
-                 suspended: Optional['ServiceSuspended'] = None,
-                 suspenders: Optional[Sequence[str]] = None,
-                 type: Optional[str] = None,
-                 updated_at: Optional[str] = None):
-        """
-        A static website service
-        :param str owner_id: The id of the owner (user/team).
-        :param str repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param 'ServiceAutoDeploy' auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param str branch: If left empty, this will fall back to the default branch of the repository.
-        :param 'ServiceNotifyOnFail' notify_on_fail: The notification setting for this service upon deployment failure.
-        """
+                 build_filter: Optional['outputs.BuildFilter'] = None,
+                 image_path: Optional[str] = None,
+                 repo: Optional[str] = None,
+                 service_details: Optional['outputs.StaticSiteDetailsOutput'] = None,
+                 type: Optional[str] = None):
+        pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "created_at", created_at)
+        pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "notify_on_fail", notify_on_fail)
         pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
-        if auto_deploy is None:
-            auto_deploy = 'no'
-        if auto_deploy is not None:
-            pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "root_dir", root_dir)
+        pulumi.set(__self__, "slug", slug)
+        pulumi.set(__self__, "suspended", suspended)
+        pulumi.set(__self__, "suspenders", suspenders)
+        pulumi.set(__self__, "updated_at", updated_at)
         if branch is not None:
             pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
-        if env_vars is not None:
-            pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
-        if secret_files is not None:
-            pulumi.set(__self__, "secret_files", secret_files)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
+        if image_path is not None:
+            pulumi.set(__self__, "image_path", image_path)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
         if service_details is not None:
             pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
         if type is None:
             type = 'static_site'
         if type is not None:
             pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
+
+    @property
+    @pulumi.getter(name="autoDeploy")
+    def auto_deploy(self) -> 'ServiceAutoDeploy':
+        return pulumi.get(self, "auto_deploy")
+
+    @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> str:
+        return pulumi.get(self, "created_at")
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="notifyOnFail")
+    def notify_on_fail(self) -> 'ServiceNotifyOnFail':
+        return pulumi.get(self, "notify_on_fail")
+
+    @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> str:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @property
-    @pulumi.getter
-    def repo(self) -> str:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
-        return pulumi.get(self, "repo")
-
-    @property
-    @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional['ServiceAutoDeploy']:
-        """
-        Whether to auto deploy the service or not upon git push.
-        """
-        return pulumi.get(self, "auto_deploy")
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> str:
+        return pulumi.get(self, "root_dir")
 
     @property
     @pulumi.getter
-    def branch(self) -> Optional[str]:
-        """
-        If left empty, this will fall back to the default branch of the repository.
-        """
-        return pulumi.get(self, "branch")
+    def slug(self) -> str:
+        return pulumi.get(self, "slug")
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
-        return pulumi.get(self, "created_at")
+    @pulumi.getter
+    def suspended(self) -> 'ServiceSuspended':
+        return pulumi.get(self, "suspended")
 
     @property
-    @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[Sequence['outputs.EnvVarKeyValue']]:
-        return pulumi.get(self, "env_vars")
+    @pulumi.getter
+    def suspenders(self) -> Sequence['ServiceSuspendersItem']:
+        return pulumi.get(self, "suspenders")
 
     @property
-    @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional['ServiceNotifyOnFail']:
-        """
-        The notification setting for this service upon deployment failure.
-        """
-        return pulumi.get(self, "notify_on_fail")
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> str:
+        return pulumi.get(self, "updated_at")
 
     @property
-    @pulumi.getter(name="secretFiles")
-    def secret_files(self) -> Optional[Sequence['outputs.SecretFile']]:
-        return pulumi.get(self, "secret_files")
+    @pulumi.getter
+    def branch(self) -> Optional[str]:
+        return pulumi.get(self, "branch")
 
     @property
-    @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional['outputs.StaticSiteServiceDetails']:
-        return pulumi.get(self, "service_details")
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional['outputs.BuildFilter']:
+        return pulumi.get(self, "build_filter")
 
     @property
-    @pulumi.getter
-    def slug(self) -> Optional[str]:
-        return pulumi.get(self, "slug")
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> Optional[str]:
+        return pulumi.get(self, "image_path")
 
     @property
     @pulumi.getter
-    def suspended(self) -> Optional['ServiceSuspended']:
-        return pulumi.get(self, "suspended")
+    def repo(self) -> Optional[str]:
+        return pulumi.get(self, "repo")
 
     @property
-    @pulumi.getter
-    def suspenders(self) -> Optional[Sequence[str]]:
-        return pulumi.get(self, "suspenders")
+    @pulumi.getter(name="serviceDetails")
+    def service_details(self) -> Optional['outputs.StaticSiteDetailsOutput']:
+        return pulumi.get(self, "service_details")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         return pulumi.get(self, "type")
 
-    @property
-    @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[str]:
-        return pulumi.get(self, "updated_at")
-
 
 @pulumi.output_type
 class GetWebService(dict):
-    """
-    A web service
-    """
     def __init__(__self__, *,
+                 auto_deploy: 'ServiceAutoDeploy',
+                 created_at: str,
+                 id: str,
                  name: str,
+                 notify_on_fail: 'ServiceNotifyOnFail',
                  owner_id: str,
-                 repo: str,
-                 auto_deploy: Optional['ServiceAutoDeploy'] = None,
+                 root_dir: str,
+                 slug: str,
+                 suspended: 'ServiceSuspended',
+                 suspenders: Sequence['ServiceSuspendersItem'],
+                 updated_at: str,
                  branch: Optional[str] = None,
-                 created_at: Optional[str] = None,
-                 env_vars: Optional[Sequence['outputs.EnvVarKeyValue']] = None,
-                 notify_on_fail: Optional['ServiceNotifyOnFail'] = None,
-                 secret_files: Optional[Sequence['outputs.SecretFile']] = None,
-                 service_details: Optional['outputs.WebServiceServiceDetails'] = None,
-                 slug: Optional[str] = None,
-                 suspended: Optional['ServiceSuspended'] = None,
-                 suspenders: Optional[Sequence[str]] = None,
-                 type: Optional[str] = None,
-                 updated_at: Optional[str] = None):
-        """
-        A web service
-        :param str owner_id: The id of the owner (user/team).
-        :param str repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param 'ServiceAutoDeploy' auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param str branch: If left empty, this will fall back to the default branch of the repository.
-        :param 'ServiceNotifyOnFail' notify_on_fail: The notification setting for this service upon deployment failure.
-        """
+                 build_filter: Optional['outputs.BuildFilter'] = None,
+                 image_path: Optional[str] = None,
+                 repo: Optional[str] = None,
+                 service_details: Optional['outputs.WebServiceDetailsOutput'] = None,
+                 type: Optional[str] = None):
+        pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "created_at", created_at)
+        pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "notify_on_fail", notify_on_fail)
         pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
-        if auto_deploy is None:
-            auto_deploy = 'no'
-        if auto_deploy is not None:
-            pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "root_dir", root_dir)
+        pulumi.set(__self__, "slug", slug)
+        pulumi.set(__self__, "suspended", suspended)
+        pulumi.set(__self__, "suspenders", suspenders)
+        pulumi.set(__self__, "updated_at", updated_at)
         if branch is not None:
             pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
-        if env_vars is not None:
-            pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
-        if secret_files is not None:
-            pulumi.set(__self__, "secret_files", secret_files)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
+        if image_path is not None:
+            pulumi.set(__self__, "image_path", image_path)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
         if service_details is not None:
             pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
         if type is None:
             type = 'web_service'
         if type is not None:
             pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
+
+    @property
+    @pulumi.getter(name="autoDeploy")
+    def auto_deploy(self) -> 'ServiceAutoDeploy':
+        return pulumi.get(self, "auto_deploy")
+
+    @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> str:
+        return pulumi.get(self, "created_at")
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="notifyOnFail")
+    def notify_on_fail(self) -> 'ServiceNotifyOnFail':
+        return pulumi.get(self, "notify_on_fail")
+
+    @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> str:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @property
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> str:
+        return pulumi.get(self, "root_dir")
+
+    @property
     @pulumi.getter
-    def repo(self) -> str:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
-        return pulumi.get(self, "repo")
+    def slug(self) -> str:
+        return pulumi.get(self, "slug")
 
     @property
-    @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional['ServiceAutoDeploy']:
-        """
-        Whether to auto deploy the service or not upon git push.
-        """
-        return pulumi.get(self, "auto_deploy")
+    @pulumi.getter
+    def suspended(self) -> 'ServiceSuspended':
+        return pulumi.get(self, "suspended")
 
     @property
     @pulumi.getter
-    def branch(self) -> Optional[str]:
-        """
-        If left empty, this will fall back to the default branch of the repository.
-        """
-        return pulumi.get(self, "branch")
+    def suspenders(self) -> Sequence['ServiceSuspendersItem']:
+        return pulumi.get(self, "suspenders")
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
-        return pulumi.get(self, "created_at")
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> str:
+        return pulumi.get(self, "updated_at")
 
     @property
-    @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[Sequence['outputs.EnvVarKeyValue']]:
-        return pulumi.get(self, "env_vars")
+    @pulumi.getter
+    def branch(self) -> Optional[str]:
+        return pulumi.get(self, "branch")
 
     @property
-    @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional['ServiceNotifyOnFail']:
-        """
-        The notification setting for this service upon deployment failure.
-        """
-        return pulumi.get(self, "notify_on_fail")
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional['outputs.BuildFilter']:
+        return pulumi.get(self, "build_filter")
 
     @property
-    @pulumi.getter(name="secretFiles")
-    def secret_files(self) -> Optional[Sequence['outputs.SecretFile']]:
-        return pulumi.get(self, "secret_files")
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> Optional[str]:
+        return pulumi.get(self, "image_path")
+
+    @property
+    @pulumi.getter
+    def repo(self) -> Optional[str]:
+        return pulumi.get(self, "repo")
 
     @property
     @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional['outputs.WebServiceServiceDetails']:
+    def service_details(self) -> Optional['outputs.WebServiceDetailsOutput']:
         return pulumi.get(self, "service_details")
 
     @property
     @pulumi.getter
-    def slug(self) -> Optional[str]:
-        return pulumi.get(self, "slug")
+    def type(self) -> Optional[str]:
+        return pulumi.get(self, "type")
+
+
+@pulumi.output_type
+class Header(dict):
+    def __init__(__self__, *,
+                 id: str,
+                 name: str,
+                 path: str,
+                 value: str):
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "path", path)
+        pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
-    def suspended(self) -> Optional['ServiceSuspended']:
-        return pulumi.get(self, "suspended")
+    def id(self) -> str:
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def suspenders(self) -> Optional[Sequence[str]]:
-        return pulumi.get(self, "suspenders")
+    def name(self) -> str:
+        return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def type(self) -> Optional[str]:
-        return pulumi.get(self, "type")
+    def path(self) -> str:
+        return pulumi.get(self, "path")
 
     @property
-    @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[str]:
-        return pulumi.get(self, "updated_at")
+    @pulumi.getter
+    def value(self) -> str:
+        return pulumi.get(self, "value")
+
+
+@pulumi.output_type
+class Image(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "imagePath":
+            suggest = "image_path"
+        elif key == "ownerId":
+            suggest = "owner_id"
+        elif key == "registryCredentialId":
+            suggest = "registry_credential_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in Image. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        Image.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        Image.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 image_path: str,
+                 owner_id: str,
+                 registry_credential_id: Optional[str] = None):
+        """
+        :param str image_path: Path to the image used for this server (e.g docker.io/library/nginx:latest).
+        :param str owner_id: The ID of the owner for this image. This should match the owner of the service as well as the owner of any specified registry credential.
+        :param str registry_credential_id: Optional reference to the registry credential passed to the image repository to retrieve this image.
+        """
+        pulumi.set(__self__, "image_path", image_path)
+        pulumi.set(__self__, "owner_id", owner_id)
+        if registry_credential_id is not None:
+            pulumi.set(__self__, "registry_credential_id", registry_credential_id)
+
+    @property
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> str:
+        """
+        Path to the image used for this server (e.g docker.io/library/nginx:latest).
+        """
+        return pulumi.get(self, "image_path")
+
+    @property
+    @pulumi.getter(name="ownerId")
+    def owner_id(self) -> str:
+        """
+        The ID of the owner for this image. This should match the owner of the service as well as the owner of any specified registry credential.
+        """
+        return pulumi.get(self, "owner_id")
+
+    @property
+    @pulumi.getter(name="registryCredentialId")
+    def registry_credential_id(self) -> Optional[str]:
+        """
+        Optional reference to the registry credential passed to the image repository to retrieve this image.
+        """
+        return pulumi.get(self, "registry_credential_id")
+
+
+@pulumi.output_type
+class ImageProperties(dict):
+    """
+    Image information used when creating the deploy. Not present for Git-backed deploys
+    """
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "registryCredential":
+            suggest = "registry_credential"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ImageProperties. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ImageProperties.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ImageProperties.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 ref: Optional[str] = None,
+                 registry_credential: Optional[str] = None,
+                 sha: Optional[str] = None):
+        """
+        Image information used when creating the deploy. Not present for Git-backed deploys
+        :param str ref: Image reference used when creating the deploy
+        :param str registry_credential: Name of credential used to pull the image, if provided
+        :param str sha: SHA that the image reference was resolved to when creating the deploy
+        """
+        if ref is not None:
+            pulumi.set(__self__, "ref", ref)
+        if registry_credential is not None:
+            pulumi.set(__self__, "registry_credential", registry_credential)
+        if sha is not None:
+            pulumi.set(__self__, "sha", sha)
+
+    @property
+    @pulumi.getter
+    def ref(self) -> Optional[str]:
+        """
+        Image reference used when creating the deploy
+        """
+        return pulumi.get(self, "ref")
+
+    @property
+    @pulumi.getter(name="registryCredential")
+    def registry_credential(self) -> Optional[str]:
+        """
+        Name of credential used to pull the image, if provided
+        """
+        return pulumi.get(self, "registry_credential")
+
+    @property
+    @pulumi.getter
+    def sha(self) -> Optional[str]:
+        """
+        SHA that the image reference was resolved to when creating the deploy
+        """
+        return pulumi.get(self, "sha")
 
 
 @pulumi.output_type
 class Job(dict):
     def __init__(__self__, *,
+                 created_at: str,
+                 id: str,
                  plan_id: str,
+                 service_id: str,
                  start_command: str,
-                 created_at: Optional[str] = None,
                  finished_at: Optional[str] = None,
                  started_at: Optional[str] = None,
                  status: Optional[str] = None):
+        pulumi.set(__self__, "created_at", created_at)
+        pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "plan_id", plan_id)
+        pulumi.set(__self__, "service_id", service_id)
         pulumi.set(__self__, "start_command", start_command)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
         if finished_at is not None:
             pulumi.set(__self__, "finished_at", finished_at)
         if started_at is not None:
             pulumi.set(__self__, "started_at", started_at)
         if status is not None:
             pulumi.set(__self__, "status", status)
 
     @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> str:
+        return pulumi.get(self, "created_at")
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
+
+    @property
     @pulumi.getter(name="planId")
     def plan_id(self) -> str:
         return pulumi.get(self, "plan_id")
 
     @property
+    @pulumi.getter(name="serviceId")
+    def service_id(self) -> str:
+        return pulumi.get(self, "service_id")
+
+    @property
     @pulumi.getter(name="startCommand")
     def start_command(self) -> str:
         return pulumi.get(self, "start_command")
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
-        return pulumi.get(self, "created_at")
-
-    @property
     @pulumi.getter(name="finishedAt")
     def finished_at(self) -> Optional[str]:
         return pulumi.get(self, "finished_at")
 
     @property
     @pulumi.getter(name="startedAt")
     def started_at(self) -> Optional[str]:
@@ -1705,15 +2027,15 @@
     @property
     @pulumi.getter
     def status(self) -> Optional[str]:
         return pulumi.get(self, "status")
 
 
 @pulumi.output_type
-class ListCustomDomainsResponse(dict):
+class ListCustomDomainsItemProperties(dict):
     def __init__(__self__, *,
                  cursor: Optional[str] = None,
                  custom_domain: Optional['outputs.CustomDomain'] = None):
         if cursor is not None:
             pulumi.set(__self__, "cursor", cursor)
         if custom_domain is not None:
             pulumi.set(__self__, "custom_domain", custom_domain)
@@ -1726,57 +2048,36 @@
     @property
     @pulumi.getter(name="customDomain")
     def custom_domain(self) -> Optional['outputs.CustomDomain']:
         return pulumi.get(self, "custom_domain")
 
 
 @pulumi.output_type
-class ListDeploysResponse(dict):
+class ListDeploysItemProperties(dict):
     def __init__(__self__, *,
                  cursor: Optional[str] = None,
-                 custom_domain: Optional['outputs.Deploy'] = None):
+                 deploy: Optional['outputs.Deploy'] = None):
         if cursor is not None:
             pulumi.set(__self__, "cursor", cursor)
-        if custom_domain is not None:
-            pulumi.set(__self__, "custom_domain", custom_domain)
+        if deploy is not None:
+            pulumi.set(__self__, "deploy", deploy)
 
     @property
     @pulumi.getter
     def cursor(self) -> Optional[str]:
         return pulumi.get(self, "cursor")
 
     @property
-    @pulumi.getter(name="customDomain")
-    def custom_domain(self) -> Optional['outputs.Deploy']:
-        return pulumi.get(self, "custom_domain")
-
-
-@pulumi.output_type
-class ListEnvVarsResponse(dict):
-    def __init__(__self__, *,
-                 cursor: Optional[str] = None,
-                 env_var: Optional['outputs.EnvVarKeyValue'] = None):
-        if cursor is not None:
-            pulumi.set(__self__, "cursor", cursor)
-        if env_var is not None:
-            pulumi.set(__self__, "env_var", env_var)
-
-    @property
     @pulumi.getter
-    def cursor(self) -> Optional[str]:
-        return pulumi.get(self, "cursor")
-
-    @property
-    @pulumi.getter(name="envVar")
-    def env_var(self) -> Optional['outputs.EnvVarKeyValue']:
-        return pulumi.get(self, "env_var")
+    def deploy(self) -> Optional['outputs.Deploy']:
+        return pulumi.get(self, "deploy")
 
 
 @pulumi.output_type
-class ListJobsResponse(dict):
+class ListJobItemProperties(dict):
     def __init__(__self__, *,
                  cursor: Optional[str] = None,
                  job: Optional['outputs.Job'] = None):
         if cursor is not None:
             pulumi.set(__self__, "cursor", cursor)
         if job is not None:
             pulumi.set(__self__, "job", job)
@@ -1789,1101 +2090,1160 @@
     @property
     @pulumi.getter
     def job(self) -> Optional['outputs.Job']:
         return pulumi.get(self, "job")
 
 
 @pulumi.output_type
-class ListServiceHeadersResponse(dict):
+class ListRetrieveHeadersItemProperties(dict):
     def __init__(__self__, *,
                  cursor: Optional[str] = None,
-                 header: Optional['outputs.ServiceHeader'] = None):
-        """
-        :param 'ServiceHeader' header: A service header object
-        """
+                 headers: Optional['outputs.Header'] = None):
         if cursor is not None:
             pulumi.set(__self__, "cursor", cursor)
-        if header is not None:
-            pulumi.set(__self__, "header", header)
+        if headers is not None:
+            pulumi.set(__self__, "headers", headers)
 
     @property
     @pulumi.getter
     def cursor(self) -> Optional[str]:
         return pulumi.get(self, "cursor")
 
     @property
     @pulumi.getter
-    def header(self) -> Optional['outputs.ServiceHeader']:
-        """
-        A service header object
-        """
-        return pulumi.get(self, "header")
+    def headers(self) -> Optional['outputs.Header']:
+        return pulumi.get(self, "headers")
 
 
 @pulumi.output_type
-class ListServiceResponse(dict):
+class ListRetrieveRoutesItemProperties(dict):
     def __init__(__self__, *,
                  cursor: Optional[str] = None,
-                 service: Optional[Any] = None):
+                 routes: Optional['outputs.Route'] = None):
         if cursor is not None:
             pulumi.set(__self__, "cursor", cursor)
-        if service is not None:
-            pulumi.set(__self__, "service", service)
+        if routes is not None:
+            pulumi.set(__self__, "routes", routes)
 
     @property
     @pulumi.getter
     def cursor(self) -> Optional[str]:
         return pulumi.get(self, "cursor")
 
     @property
     @pulumi.getter
-    def service(self) -> Optional[Any]:
-        return pulumi.get(self, "service")
+    def routes(self) -> Optional['outputs.Route']:
+        return pulumi.get(self, "routes")
 
 
 @pulumi.output_type
-class ListStaticSiteRoutesResponse(dict):
+class ListServicesResponse(dict):
     def __init__(__self__, *,
                  cursor: Optional[str] = None,
-                 route: Optional['outputs.StaticSiteRoute'] = None):
-        """
-        :param 'StaticSiteRoute' route: A route object for a static site
-        """
+                 service: Optional[Any] = None):
         if cursor is not None:
             pulumi.set(__self__, "cursor", cursor)
-        if route is not None:
-            pulumi.set(__self__, "route", route)
+        if service is not None:
+            pulumi.set(__self__, "service", service)
 
     @property
     @pulumi.getter
     def cursor(self) -> Optional[str]:
         return pulumi.get(self, "cursor")
 
     @property
     @pulumi.getter
-    def route(self) -> Optional['outputs.StaticSiteRoute']:
-        """
-        A route object for a static site
-        """
-        return pulumi.get(self, "route")
+    def service(self) -> Optional[Any]:
+        return pulumi.get(self, "service")
 
 
 @pulumi.output_type
 class NativeEnvironmentDetails(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "buildCommand":
             suggest = "build_command"
         elif key == "startCommand":
             suggest = "start_command"
+        elif key == "preDeployCommand":
+            suggest = "pre_deploy_command"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in NativeEnvironmentDetails. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         NativeEnvironmentDetails.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         NativeEnvironmentDetails.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  build_command: str,
-                 start_command: str):
+                 start_command: str,
+                 pre_deploy_command: Optional[str] = None):
         pulumi.set(__self__, "build_command", build_command)
         pulumi.set(__self__, "start_command", start_command)
+        if pre_deploy_command is not None:
+            pulumi.set(__self__, "pre_deploy_command", pre_deploy_command)
 
     @property
     @pulumi.getter(name="buildCommand")
     def build_command(self) -> str:
         return pulumi.get(self, "build_command")
 
     @property
     @pulumi.getter(name="startCommand")
     def start_command(self) -> str:
         return pulumi.get(self, "start_command")
 
+    @property
+    @pulumi.getter(name="preDeployCommand")
+    def pre_deploy_command(self) -> Optional[str]:
+        return pulumi.get(self, "pre_deploy_command")
+
 
 @pulumi.output_type
-class OpenPorts(dict):
+class PrivateServiceDetailsOutput(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "buildPlan":
+            suggest = "build_plan"
+        elif key == "envSpecificDetails":
+            suggest = "env_specific_details"
+        elif key == "numInstances":
+            suggest = "num_instances"
+        elif key == "openPorts":
+            suggest = "open_ports"
+        elif key == "pullRequestPreviewsEnabled":
+            suggest = "pull_request_previews_enabled"
+        elif key == "parentServer":
+            suggest = "parent_server"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in PrivateServiceDetailsOutput. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        PrivateServiceDetailsOutput.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        PrivateServiceDetailsOutput.__key_warning(key)
+        return super().get(key, default)
+
     def __init__(__self__, *,
-                 port: Optional[float] = None,
-                 protocol: Optional['OpenPortsProtocol'] = None):
-        if port is not None:
-            pulumi.set(__self__, "port", port)
-        if protocol is not None:
-            pulumi.set(__self__, "protocol", protocol)
+                 build_plan: str,
+                 env: 'PrivateServiceDetailsOutputEnv',
+                 env_specific_details: Any,
+                 num_instances: int,
+                 open_ports: Sequence['outputs.ServerPort'],
+                 plan: 'PrivateServiceDetailsOutputPlan',
+                 pull_request_previews_enabled: 'PrivateServiceDetailsOutputPullRequestPreviewsEnabled',
+                 region: 'PrivateServiceDetailsOutputRegion',
+                 url: str,
+                 autoscaling: Optional['outputs.AutoscalingConfig'] = None,
+                 disk: Optional['outputs.Disk'] = None,
+                 parent_server: Optional['outputs.Resource'] = None):
+        """
+        :param 'PrivateServiceDetailsOutputEnv' env: Environment (runtime)
+        :param int num_instances: For a *manually* scaled service, this is the number of instances the service is scaled to. DOES NOT indicate the number of running instances for an *autoscaled* service.
+        :param 'PrivateServiceDetailsOutputPlan' plan: The instance type to use for the preview instance. Note that base services with any paid instance type can't create preview instances with the `free` instance type.
+        """
+        pulumi.set(__self__, "build_plan", build_plan)
+        pulumi.set(__self__, "env", env)
+        pulumi.set(__self__, "env_specific_details", env_specific_details)
+        pulumi.set(__self__, "num_instances", num_instances)
+        pulumi.set(__self__, "open_ports", open_ports)
+        pulumi.set(__self__, "plan", plan)
+        pulumi.set(__self__, "pull_request_previews_enabled", pull_request_previews_enabled)
+        pulumi.set(__self__, "region", region)
+        pulumi.set(__self__, "url", url)
+        if autoscaling is not None:
+            pulumi.set(__self__, "autoscaling", autoscaling)
+        if disk is not None:
+            pulumi.set(__self__, "disk", disk)
+        if parent_server is not None:
+            pulumi.set(__self__, "parent_server", parent_server)
+
+    @property
+    @pulumi.getter(name="buildPlan")
+    def build_plan(self) -> str:
+        return pulumi.get(self, "build_plan")
 
     @property
     @pulumi.getter
-    def port(self) -> Optional[float]:
-        return pulumi.get(self, "port")
+    def env(self) -> 'PrivateServiceDetailsOutputEnv':
+        """
+        Environment (runtime)
+        """
+        return pulumi.get(self, "env")
+
+    @property
+    @pulumi.getter(name="envSpecificDetails")
+    def env_specific_details(self) -> Any:
+        return pulumi.get(self, "env_specific_details")
+
+    @property
+    @pulumi.getter(name="numInstances")
+    def num_instances(self) -> int:
+        """
+        For a *manually* scaled service, this is the number of instances the service is scaled to. DOES NOT indicate the number of running instances for an *autoscaled* service.
+        """
+        return pulumi.get(self, "num_instances")
+
+    @property
+    @pulumi.getter(name="openPorts")
+    def open_ports(self) -> Sequence['outputs.ServerPort']:
+        return pulumi.get(self, "open_ports")
 
     @property
     @pulumi.getter
-    def protocol(self) -> Optional['OpenPortsProtocol']:
-        return pulumi.get(self, "protocol")
+    def plan(self) -> 'PrivateServiceDetailsOutputPlan':
+        """
+        The instance type to use for the preview instance. Note that base services with any paid instance type can't create preview instances with the `free` instance type.
+        """
+        return pulumi.get(self, "plan")
+
+    @property
+    @pulumi.getter(name="pullRequestPreviewsEnabled")
+    def pull_request_previews_enabled(self) -> 'PrivateServiceDetailsOutputPullRequestPreviewsEnabled':
+        return pulumi.get(self, "pull_request_previews_enabled")
+
+    @property
+    @pulumi.getter
+    def region(self) -> 'PrivateServiceDetailsOutputRegion':
+        return pulumi.get(self, "region")
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        return pulumi.get(self, "url")
+
+    @property
+    @pulumi.getter
+    def autoscaling(self) -> Optional['outputs.AutoscalingConfig']:
+        return pulumi.get(self, "autoscaling")
+
+    @property
+    @pulumi.getter
+    def disk(self) -> Optional['outputs.Disk']:
+        return pulumi.get(self, "disk")
+
+    @property
+    @pulumi.getter(name="parentServer")
+    def parent_server(self) -> Optional['outputs.Resource']:
+        return pulumi.get(self, "parent_server")
 
 
 @pulumi.output_type
-class PrivateService(dict):
-    """
-    A private service
-    """
+class PrivateServiceOutput(dict):
     def __init__(__self__, *,
+                 auto_deploy: 'ServiceAutoDeploy',
+                 created_at: str,
+                 id: str,
                  name: str,
+                 notify_on_fail: 'ServiceNotifyOnFail',
                  owner_id: str,
-                 repo: str,
-                 auto_deploy: Optional['ServiceAutoDeploy'] = None,
+                 root_dir: str,
+                 slug: str,
+                 suspended: 'ServiceSuspended',
+                 suspenders: Sequence['ServiceSuspendersItem'],
+                 updated_at: str,
                  branch: Optional[str] = None,
-                 created_at: Optional[str] = None,
-                 env_vars: Optional[Sequence['outputs.EnvVarKeyValue']] = None,
-                 notify_on_fail: Optional['ServiceNotifyOnFail'] = None,
-                 secret_files: Optional[Sequence['outputs.SecretFile']] = None,
-                 service_details: Optional['outputs.PrivateServiceDetails'] = None,
-                 slug: Optional[str] = None,
-                 suspended: Optional['ServiceSuspended'] = None,
-                 suspenders: Optional[Sequence[str]] = None,
-                 type: Optional[str] = None,
-                 updated_at: Optional[str] = None):
-        """
-        A private service
-        :param str owner_id: The id of the owner (user/team).
-        :param str repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param 'ServiceAutoDeploy' auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param str branch: If left empty, this will fall back to the default branch of the repository.
-        :param 'ServiceNotifyOnFail' notify_on_fail: The notification setting for this service upon deployment failure.
-        """
+                 build_filter: Optional['outputs.BuildFilter'] = None,
+                 image_path: Optional[str] = None,
+                 repo: Optional[str] = None,
+                 service_details: Optional['outputs.PrivateServiceDetailsOutput'] = None,
+                 type: Optional[str] = None):
+        pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "created_at", created_at)
+        pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "notify_on_fail", notify_on_fail)
         pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
-        if auto_deploy is None:
-            auto_deploy = 'no'
-        if auto_deploy is not None:
-            pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "root_dir", root_dir)
+        pulumi.set(__self__, "slug", slug)
+        pulumi.set(__self__, "suspended", suspended)
+        pulumi.set(__self__, "suspenders", suspenders)
+        pulumi.set(__self__, "updated_at", updated_at)
         if branch is not None:
             pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
-        if env_vars is not None:
-            pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
-        if secret_files is not None:
-            pulumi.set(__self__, "secret_files", secret_files)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
+        if image_path is not None:
+            pulumi.set(__self__, "image_path", image_path)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
         if service_details is not None:
             pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
         if type is None:
             type = 'private_service'
         if type is not None:
             pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter(name="ownerId")
-    def owner_id(self) -> str:
-        """
-        The id of the owner (user/team).
-        """
-        return pulumi.get(self, "owner_id")
-
-    @property
-    @pulumi.getter
-    def repo(self) -> str:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
-        return pulumi.get(self, "repo")
 
     @property
     @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional['ServiceAutoDeploy']:
-        """
-        Whether to auto deploy the service or not upon git push.
-        """
+    def auto_deploy(self) -> 'ServiceAutoDeploy':
         return pulumi.get(self, "auto_deploy")
 
     @property
-    @pulumi.getter
-    def branch(self) -> Optional[str]:
-        """
-        If left empty, this will fall back to the default branch of the repository.
-        """
-        return pulumi.get(self, "branch")
-
-    @property
     @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
+    def created_at(self) -> str:
         return pulumi.get(self, "created_at")
 
     @property
-    @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[Sequence['outputs.EnvVarKeyValue']]:
-        return pulumi.get(self, "env_vars")
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional['ServiceNotifyOnFail']:
-        """
-        The notification setting for this service upon deployment failure.
-        """
+    def notify_on_fail(self) -> 'ServiceNotifyOnFail':
         return pulumi.get(self, "notify_on_fail")
 
     @property
-    @pulumi.getter(name="secretFiles")
-    def secret_files(self) -> Optional[Sequence['outputs.SecretFile']]:
-        return pulumi.get(self, "secret_files")
+    @pulumi.getter(name="ownerId")
+    def owner_id(self) -> str:
+        return pulumi.get(self, "owner_id")
 
     @property
-    @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional['outputs.PrivateServiceDetails']:
-        return pulumi.get(self, "service_details")
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> str:
+        return pulumi.get(self, "root_dir")
 
     @property
     @pulumi.getter
-    def slug(self) -> Optional[str]:
+    def slug(self) -> str:
         return pulumi.get(self, "slug")
 
     @property
     @pulumi.getter
-    def suspended(self) -> Optional['ServiceSuspended']:
+    def suspended(self) -> 'ServiceSuspended':
         return pulumi.get(self, "suspended")
 
     @property
     @pulumi.getter
-    def suspenders(self) -> Optional[Sequence[str]]:
+    def suspenders(self) -> Sequence['ServiceSuspendersItem']:
         return pulumi.get(self, "suspenders")
 
     @property
-    @pulumi.getter
-    def type(self) -> Optional[str]:
-        return pulumi.get(self, "type")
-
-    @property
     @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[str]:
+    def updated_at(self) -> str:
         return pulumi.get(self, "updated_at")
 
-
-@pulumi.output_type
-class PrivateServiceDetails(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "envSpecificDetails":
-            suggest = "env_specific_details"
-        elif key == "numInstances":
-            suggest = "num_instances"
-        elif key == "openPorts":
-            suggest = "open_ports"
-        elif key == "parentServer":
-            suggest = "parent_server"
-        elif key == "pullRequestPreviewsEnabled":
-            suggest = "pull_request_previews_enabled"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in PrivateServiceDetails. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        PrivateServiceDetails.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        PrivateServiceDetails.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 env: 'PrivateServiceDetailsEnv',
-                 disk: Optional['outputs.Disk'] = None,
-                 env_specific_details: Optional[Any] = None,
-                 num_instances: Optional[float] = None,
-                 open_ports: Optional[Sequence['outputs.OpenPorts']] = None,
-                 parent_server: Optional['outputs.PrivateServiceDetailsParentServerProperties'] = None,
-                 plan: Optional['PrivateServiceDetailsPlan'] = None,
-                 pull_request_previews_enabled: Optional['PrivateServiceDetailsPullRequestPreviewsEnabled'] = None,
-                 region: Optional['PrivateServiceDetailsRegion'] = None,
-                 url: Optional[str] = None):
-        pulumi.set(__self__, "env", env)
-        if disk is not None:
-            pulumi.set(__self__, "disk", disk)
-        if env_specific_details is not None:
-            pulumi.set(__self__, "env_specific_details", env_specific_details)
-        if num_instances is None:
-            num_instances = 1
-        if num_instances is not None:
-            pulumi.set(__self__, "num_instances", num_instances)
-        if open_ports is not None:
-            pulumi.set(__self__, "open_ports", open_ports)
-        if parent_server is not None:
-            pulumi.set(__self__, "parent_server", parent_server)
-        if plan is None:
-            plan = 'starter'
-        if plan is not None:
-            pulumi.set(__self__, "plan", plan)
-        if pull_request_previews_enabled is None:
-            pull_request_previews_enabled = 'no'
-        if pull_request_previews_enabled is not None:
-            pulumi.set(__self__, "pull_request_previews_enabled", pull_request_previews_enabled)
-        if region is None:
-            region = 'oregon'
-        if region is not None:
-            pulumi.set(__self__, "region", region)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
-
     @property
     @pulumi.getter
-    def env(self) -> 'PrivateServiceDetailsEnv':
-        return pulumi.get(self, "env")
+    def branch(self) -> Optional[str]:
+        return pulumi.get(self, "branch")
 
     @property
-    @pulumi.getter
-    def disk(self) -> Optional['outputs.Disk']:
-        return pulumi.get(self, "disk")
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional['outputs.BuildFilter']:
+        return pulumi.get(self, "build_filter")
 
     @property
-    @pulumi.getter(name="envSpecificDetails")
-    def env_specific_details(self) -> Optional[Any]:
-        return pulumi.get(self, "env_specific_details")
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> Optional[str]:
+        return pulumi.get(self, "image_path")
 
     @property
-    @pulumi.getter(name="numInstances")
-    def num_instances(self) -> Optional[float]:
-        return pulumi.get(self, "num_instances")
+    @pulumi.getter
+    def repo(self) -> Optional[str]:
+        return pulumi.get(self, "repo")
 
     @property
-    @pulumi.getter(name="openPorts")
-    def open_ports(self) -> Optional[Sequence['outputs.OpenPorts']]:
-        return pulumi.get(self, "open_ports")
+    @pulumi.getter(name="serviceDetails")
+    def service_details(self) -> Optional['outputs.PrivateServiceDetailsOutput']:
+        return pulumi.get(self, "service_details")
 
     @property
-    @pulumi.getter(name="parentServer")
-    def parent_server(self) -> Optional['outputs.PrivateServiceDetailsParentServerProperties']:
-        return pulumi.get(self, "parent_server")
+    @pulumi.getter
+    def type(self) -> Optional[str]:
+        return pulumi.get(self, "type")
+
+
+@pulumi.output_type
+class RegistryCredential(dict):
+    def __init__(__self__, *,
+                 id: str,
+                 name: str,
+                 registry: 'RegistryCredentialRegistry',
+                 username: str):
+        """
+        :param str id: Unique identifier for this credential
+        :param str name: Descriptive name for this credential
+        :param 'RegistryCredentialRegistry' registry: The registry to use this credential with
+        :param str username: The username associated with the credential
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "registry", registry)
+        pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
-    def plan(self) -> Optional['PrivateServiceDetailsPlan']:
-        return pulumi.get(self, "plan")
+    def id(self) -> str:
+        """
+        Unique identifier for this credential
+        """
+        return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="pullRequestPreviewsEnabled")
-    def pull_request_previews_enabled(self) -> Optional['PrivateServiceDetailsPullRequestPreviewsEnabled']:
-        return pulumi.get(self, "pull_request_previews_enabled")
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Descriptive name for this credential
+        """
+        return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def region(self) -> Optional['PrivateServiceDetailsRegion']:
-        return pulumi.get(self, "region")
+    def registry(self) -> 'RegistryCredentialRegistry':
+        """
+        The registry to use this credential with
+        """
+        return pulumi.get(self, "registry")
 
     @property
     @pulumi.getter
-    def url(self) -> Optional[str]:
-        return pulumi.get(self, "url")
+    def username(self) -> str:
+        """
+        The username associated with the credential
+        """
+        return pulumi.get(self, "username")
 
 
 @pulumi.output_type
-class PrivateServiceDetailsParentServerProperties(dict):
+class Resource(dict):
     def __init__(__self__, *,
-                 id: Optional[str] = None,
-                 name: Optional[str] = None):
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+                 id: str,
+                 name: str):
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
-    def id(self) -> Optional[str]:
+    def id(self) -> str:
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[str]:
+    def name(self) -> str:
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
-class SecretFile(dict):
+class Route(dict):
     def __init__(__self__, *,
-                 contents: str,
-                 name: str):
-        pulumi.set(__self__, "contents", contents)
-        pulumi.set(__self__, "name", name)
+                 destination: str,
+                 id: str,
+                 priority: int,
+                 source: str,
+                 type: 'RouteType'):
+        """
+        :param int priority: Redirect and Rewrite Rules are applied in priority order starting at 0
+        """
+        pulumi.set(__self__, "destination", destination)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "priority", priority)
+        pulumi.set(__self__, "source", source)
+        pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
-    def contents(self) -> str:
-        return pulumi.get(self, "contents")
+    def destination(self) -> str:
+        return pulumi.get(self, "destination")
 
     @property
     @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
+    def id(self) -> str:
+        return pulumi.get(self, "id")
 
-@pulumi.output_type
-class ServerProperties(dict):
-    def __init__(__self__, *,
-                 id: Optional[str] = None,
-                 name: Optional[str] = None):
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+    @property
+    @pulumi.getter
+    def priority(self) -> int:
+        """
+        Redirect and Rewrite Rules are applied in priority order starting at 0
+        """
+        return pulumi.get(self, "priority")
 
     @property
     @pulumi.getter
-    def id(self) -> Optional[str]:
-        return pulumi.get(self, "id")
+    def source(self) -> str:
+        return pulumi.get(self, "source")
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[str]:
-        return pulumi.get(self, "name")
+    def type(self) -> 'RouteType':
+        return pulumi.get(self, "type")
 
 
 @pulumi.output_type
-class ServiceHeader(dict):
-    """
-    A service header object
-    """
+class SecretFile(dict):
     def __init__(__self__, *,
-                 name: str,
-                 path: str,
-                 value: str):
-        """
-        A service header object
-        """
+                 id: str,
+                 name: str):
+        pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "path", path)
-        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
+
+@pulumi.output_type
+class ServerPort(dict):
+    def __init__(__self__, *,
+                 port: int,
+                 protocol: 'ServerPortProtocol'):
+        pulumi.set(__self__, "port", port)
+        pulumi.set(__self__, "protocol", protocol)
+
     @property
     @pulumi.getter
-    def path(self) -> str:
-        return pulumi.get(self, "path")
+    def port(self) -> int:
+        return pulumi.get(self, "port")
 
     @property
     @pulumi.getter
-    def value(self) -> str:
-        return pulumi.get(self, "value")
+    def protocol(self) -> 'ServerPortProtocol':
+        return pulumi.get(self, "protocol")
 
 
 @pulumi.output_type
-class StaticSite(dict):
-    """
-    A static website service
-    """
+class Service(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "autoDeploy":
+            suggest = "auto_deploy"
+        elif key == "createdAt":
+            suggest = "created_at"
+        elif key == "notifyOnFail":
+            suggest = "notify_on_fail"
+        elif key == "ownerId":
+            suggest = "owner_id"
+        elif key == "rootDir":
+            suggest = "root_dir"
+        elif key == "updatedAt":
+            suggest = "updated_at"
+        elif key == "buildFilter":
+            suggest = "build_filter"
+        elif key == "imagePath":
+            suggest = "image_path"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in Service. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        Service.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        Service.__key_warning(key)
+        return super().get(key, default)
+
     def __init__(__self__, *,
+                 auto_deploy: 'ServiceAutoDeploy',
+                 created_at: str,
+                 id: str,
                  name: str,
+                 notify_on_fail: 'ServiceNotifyOnFail',
                  owner_id: str,
-                 repo: str,
-                 auto_deploy: Optional['ServiceAutoDeploy'] = None,
+                 root_dir: str,
+                 slug: str,
+                 suspended: 'ServiceSuspended',
+                 suspenders: Sequence['ServiceSuspendersItem'],
+                 updated_at: str,
                  branch: Optional[str] = None,
-                 created_at: Optional[str] = None,
-                 env_vars: Optional[Sequence['outputs.EnvVarKeyValue']] = None,
-                 notify_on_fail: Optional['ServiceNotifyOnFail'] = None,
-                 secret_files: Optional[Sequence['outputs.SecretFile']] = None,
-                 service_details: Optional['outputs.StaticSiteServiceDetails'] = None,
-                 slug: Optional[str] = None,
-                 suspended: Optional['ServiceSuspended'] = None,
-                 suspenders: Optional[Sequence[str]] = None,
-                 type: Optional[str] = None,
-                 updated_at: Optional[str] = None):
-        """
-        A static website service
-        :param str owner_id: The id of the owner (user/team).
-        :param str repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param 'ServiceAutoDeploy' auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param str branch: If left empty, this will fall back to the default branch of the repository.
-        :param 'ServiceNotifyOnFail' notify_on_fail: The notification setting for this service upon deployment failure.
-        """
+                 build_filter: Optional['outputs.BuildFilter'] = None,
+                 image_path: Optional[str] = None,
+                 repo: Optional[str] = None):
+        pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "created_at", created_at)
+        pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "notify_on_fail", notify_on_fail)
         pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
-        if auto_deploy is None:
-            auto_deploy = 'no'
-        if auto_deploy is not None:
-            pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "root_dir", root_dir)
+        pulumi.set(__self__, "slug", slug)
+        pulumi.set(__self__, "suspended", suspended)
+        pulumi.set(__self__, "suspenders", suspenders)
+        pulumi.set(__self__, "updated_at", updated_at)
         if branch is not None:
             pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
-        if env_vars is not None:
-            pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
-        if secret_files is not None:
-            pulumi.set(__self__, "secret_files", secret_files)
-        if service_details is not None:
-            pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
-        if type is None:
-            type = 'static_site'
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter(name="ownerId")
-    def owner_id(self) -> str:
-        """
-        The id of the owner (user/team).
-        """
-        return pulumi.get(self, "owner_id")
-
-    @property
-    @pulumi.getter
-    def repo(self) -> str:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
-        return pulumi.get(self, "repo")
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
+        if image_path is not None:
+            pulumi.set(__self__, "image_path", image_path)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
 
     @property
     @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional['ServiceAutoDeploy']:
-        """
-        Whether to auto deploy the service or not upon git push.
-        """
+    def auto_deploy(self) -> 'ServiceAutoDeploy':
         return pulumi.get(self, "auto_deploy")
 
     @property
-    @pulumi.getter
-    def branch(self) -> Optional[str]:
-        """
-        If left empty, this will fall back to the default branch of the repository.
-        """
-        return pulumi.get(self, "branch")
-
-    @property
     @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
+    def created_at(self) -> str:
         return pulumi.get(self, "created_at")
 
     @property
-    @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[Sequence['outputs.EnvVarKeyValue']]:
-        return pulumi.get(self, "env_vars")
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional['ServiceNotifyOnFail']:
-        """
-        The notification setting for this service upon deployment failure.
-        """
+    def notify_on_fail(self) -> 'ServiceNotifyOnFail':
         return pulumi.get(self, "notify_on_fail")
 
     @property
-    @pulumi.getter(name="secretFiles")
-    def secret_files(self) -> Optional[Sequence['outputs.SecretFile']]:
-        return pulumi.get(self, "secret_files")
+    @pulumi.getter(name="ownerId")
+    def owner_id(self) -> str:
+        return pulumi.get(self, "owner_id")
 
     @property
-    @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional['outputs.StaticSiteServiceDetails']:
-        return pulumi.get(self, "service_details")
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> str:
+        return pulumi.get(self, "root_dir")
 
     @property
     @pulumi.getter
-    def slug(self) -> Optional[str]:
+    def slug(self) -> str:
         return pulumi.get(self, "slug")
 
     @property
     @pulumi.getter
-    def suspended(self) -> Optional['ServiceSuspended']:
+    def suspended(self) -> 'ServiceSuspended':
         return pulumi.get(self, "suspended")
 
     @property
     @pulumi.getter
-    def suspenders(self) -> Optional[Sequence[str]]:
+    def suspenders(self) -> Sequence['ServiceSuspendersItem']:
         return pulumi.get(self, "suspenders")
 
     @property
-    @pulumi.getter
-    def type(self) -> Optional[str]:
-        return pulumi.get(self, "type")
-
-    @property
     @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[str]:
+    def updated_at(self) -> str:
         return pulumi.get(self, "updated_at")
 
-
-@pulumi.output_type
-class StaticSiteRoute(dict):
-    """
-    A route object for a static site
-    """
-    def __init__(__self__, *,
-                 destination: str,
-                 source: str,
-                 type: 'StaticSiteRouteType'):
-        """
-        A route object for a static site
-        """
-        pulumi.set(__self__, "destination", destination)
-        pulumi.set(__self__, "source", source)
-        pulumi.set(__self__, "type", type)
-
     @property
     @pulumi.getter
-    def destination(self) -> str:
-        return pulumi.get(self, "destination")
+    def branch(self) -> Optional[str]:
+        return pulumi.get(self, "branch")
 
     @property
-    @pulumi.getter
-    def source(self) -> str:
-        return pulumi.get(self, "source")
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional['outputs.BuildFilter']:
+        return pulumi.get(self, "build_filter")
+
+    @property
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> Optional[str]:
+        return pulumi.get(self, "image_path")
 
     @property
     @pulumi.getter
-    def type(self) -> 'StaticSiteRouteType':
-        return pulumi.get(self, "type")
+    def repo(self) -> Optional[str]:
+        return pulumi.get(self, "repo")
 
 
 @pulumi.output_type
-class StaticSiteServiceDetails(dict):
+class StaticSiteDetailsOutput(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "buildCommand":
             suggest = "build_command"
-        elif key == "parentServer":
-            suggest = "parent_server"
+        elif key == "buildPlan":
+            suggest = "build_plan"
         elif key == "publishPath":
             suggest = "publish_path"
         elif key == "pullRequestPreviewsEnabled":
             suggest = "pull_request_previews_enabled"
+        elif key == "parentServer":
+            suggest = "parent_server"
 
         if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in StaticSiteServiceDetails. Access the value via the '{suggest}' property getter instead.")
+            pulumi.log.warn(f"Key '{key}' not found in StaticSiteDetailsOutput. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
-        StaticSiteServiceDetails.__key_warning(key)
+        StaticSiteDetailsOutput.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
-        StaticSiteServiceDetails.__key_warning(key)
+        StaticSiteDetailsOutput.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 build_command: Optional[str] = None,
-                 headers: Optional[Sequence['outputs.ServiceHeader']] = None,
-                 parent_server: Optional['outputs.StaticSiteServiceDetailsParentServerProperties'] = None,
-                 publish_path: Optional[str] = None,
-                 pull_request_previews_enabled: Optional['StaticSiteServiceDetailsPullRequestPreviewsEnabled'] = None,
-                 routes: Optional[Sequence['outputs.StaticSiteRoute']] = None,
-                 url: Optional[str] = None):
-        """
-        :param str url: The HTTPS service URL. A subdomain of onrender.com, by default.
-        """
-        if build_command is not None:
-            pulumi.set(__self__, "build_command", build_command)
-        if headers is not None:
-            pulumi.set(__self__, "headers", headers)
+                 build_command: str,
+                 build_plan: str,
+                 publish_path: str,
+                 pull_request_previews_enabled: 'StaticSiteDetailsOutputPullRequestPreviewsEnabled',
+                 url: str,
+                 parent_server: Optional['outputs.Resource'] = None):
+        pulumi.set(__self__, "build_command", build_command)
+        pulumi.set(__self__, "build_plan", build_plan)
+        pulumi.set(__self__, "publish_path", publish_path)
+        pulumi.set(__self__, "pull_request_previews_enabled", pull_request_previews_enabled)
+        pulumi.set(__self__, "url", url)
         if parent_server is not None:
             pulumi.set(__self__, "parent_server", parent_server)
-        if publish_path is None:
-            publish_path = 'public'
-        if publish_path is not None:
-            pulumi.set(__self__, "publish_path", publish_path)
-        if pull_request_previews_enabled is None:
-            pull_request_previews_enabled = 'no'
-        if pull_request_previews_enabled is not None:
-            pulumi.set(__self__, "pull_request_previews_enabled", pull_request_previews_enabled)
-        if routes is not None:
-            pulumi.set(__self__, "routes", routes)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter(name="buildCommand")
-    def build_command(self) -> Optional[str]:
+    def build_command(self) -> str:
         return pulumi.get(self, "build_command")
 
     @property
-    @pulumi.getter
-    def headers(self) -> Optional[Sequence['outputs.ServiceHeader']]:
-        return pulumi.get(self, "headers")
-
-    @property
-    @pulumi.getter(name="parentServer")
-    def parent_server(self) -> Optional['outputs.StaticSiteServiceDetailsParentServerProperties']:
-        return pulumi.get(self, "parent_server")
+    @pulumi.getter(name="buildPlan")
+    def build_plan(self) -> str:
+        return pulumi.get(self, "build_plan")
 
     @property
     @pulumi.getter(name="publishPath")
-    def publish_path(self) -> Optional[str]:
+    def publish_path(self) -> str:
         return pulumi.get(self, "publish_path")
 
     @property
     @pulumi.getter(name="pullRequestPreviewsEnabled")
-    def pull_request_previews_enabled(self) -> Optional['StaticSiteServiceDetailsPullRequestPreviewsEnabled']:
+    def pull_request_previews_enabled(self) -> 'StaticSiteDetailsOutputPullRequestPreviewsEnabled':
         return pulumi.get(self, "pull_request_previews_enabled")
 
     @property
     @pulumi.getter
-    def routes(self) -> Optional[Sequence['outputs.StaticSiteRoute']]:
-        return pulumi.get(self, "routes")
-
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[str]:
-        """
-        The HTTPS service URL. A subdomain of onrender.com, by default.
-        """
+    def url(self) -> str:
         return pulumi.get(self, "url")
 
-
-@pulumi.output_type
-class StaticSiteServiceDetailsParentServerProperties(dict):
-    def __init__(__self__, *,
-                 id: Optional[str] = None,
-                 name: Optional[str] = None):
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-
     @property
-    @pulumi.getter
-    def id(self) -> Optional[str]:
-        return pulumi.get(self, "id")
-
-    @property
-    @pulumi.getter
-    def name(self) -> Optional[str]:
-        return pulumi.get(self, "name")
+    @pulumi.getter(name="parentServer")
+    def parent_server(self) -> Optional['outputs.Resource']:
+        return pulumi.get(self, "parent_server")
 
 
 @pulumi.output_type
-class WebService(dict):
-    """
-    A web service
-    """
+class StaticSiteOutput(dict):
     def __init__(__self__, *,
+                 auto_deploy: 'ServiceAutoDeploy',
+                 created_at: str,
+                 id: str,
                  name: str,
+                 notify_on_fail: 'ServiceNotifyOnFail',
                  owner_id: str,
-                 repo: str,
-                 auto_deploy: Optional['ServiceAutoDeploy'] = None,
+                 root_dir: str,
+                 slug: str,
+                 suspended: 'ServiceSuspended',
+                 suspenders: Sequence['ServiceSuspendersItem'],
+                 updated_at: str,
                  branch: Optional[str] = None,
-                 created_at: Optional[str] = None,
-                 env_vars: Optional[Sequence['outputs.EnvVarKeyValue']] = None,
-                 notify_on_fail: Optional['ServiceNotifyOnFail'] = None,
-                 secret_files: Optional[Sequence['outputs.SecretFile']] = None,
-                 service_details: Optional['outputs.WebServiceServiceDetails'] = None,
-                 slug: Optional[str] = None,
-                 suspended: Optional['ServiceSuspended'] = None,
-                 suspenders: Optional[Sequence[str]] = None,
-                 type: Optional[str] = None,
-                 updated_at: Optional[str] = None):
-        """
-        A web service
-        :param str owner_id: The id of the owner (user/team).
-        :param str repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param 'ServiceAutoDeploy' auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param str branch: If left empty, this will fall back to the default branch of the repository.
-        :param 'ServiceNotifyOnFail' notify_on_fail: The notification setting for this service upon deployment failure.
-        """
+                 build_filter: Optional['outputs.BuildFilter'] = None,
+                 image_path: Optional[str] = None,
+                 repo: Optional[str] = None,
+                 service_details: Optional['outputs.StaticSiteDetailsOutput'] = None,
+                 type: Optional[str] = None):
+        pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "created_at", created_at)
+        pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "notify_on_fail", notify_on_fail)
         pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
-        if auto_deploy is None:
-            auto_deploy = 'no'
-        if auto_deploy is not None:
-            pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "root_dir", root_dir)
+        pulumi.set(__self__, "slug", slug)
+        pulumi.set(__self__, "suspended", suspended)
+        pulumi.set(__self__, "suspenders", suspenders)
+        pulumi.set(__self__, "updated_at", updated_at)
         if branch is not None:
             pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
-        if env_vars is not None:
-            pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
-        if secret_files is not None:
-            pulumi.set(__self__, "secret_files", secret_files)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
+        if image_path is not None:
+            pulumi.set(__self__, "image_path", image_path)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
         if service_details is not None:
             pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
         if type is None:
-            type = 'web_service'
+            type = 'static_site'
         if type is not None:
             pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
+
+    @property
+    @pulumi.getter(name="autoDeploy")
+    def auto_deploy(self) -> 'ServiceAutoDeploy':
+        return pulumi.get(self, "auto_deploy")
+
+    @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> str:
+        return pulumi.get(self, "created_at")
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="notifyOnFail")
+    def notify_on_fail(self) -> 'ServiceNotifyOnFail':
+        return pulumi.get(self, "notify_on_fail")
+
+    @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> str:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @property
-    @pulumi.getter
-    def repo(self) -> str:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
-        return pulumi.get(self, "repo")
-
-    @property
-    @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional['ServiceAutoDeploy']:
-        """
-        Whether to auto deploy the service or not upon git push.
-        """
-        return pulumi.get(self, "auto_deploy")
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> str:
+        return pulumi.get(self, "root_dir")
 
     @property
     @pulumi.getter
-    def branch(self) -> Optional[str]:
-        """
-        If left empty, this will fall back to the default branch of the repository.
-        """
-        return pulumi.get(self, "branch")
+    def slug(self) -> str:
+        return pulumi.get(self, "slug")
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
-        return pulumi.get(self, "created_at")
+    @pulumi.getter
+    def suspended(self) -> 'ServiceSuspended':
+        return pulumi.get(self, "suspended")
 
     @property
-    @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[Sequence['outputs.EnvVarKeyValue']]:
-        return pulumi.get(self, "env_vars")
+    @pulumi.getter
+    def suspenders(self) -> Sequence['ServiceSuspendersItem']:
+        return pulumi.get(self, "suspenders")
 
     @property
-    @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional['ServiceNotifyOnFail']:
-        """
-        The notification setting for this service upon deployment failure.
-        """
-        return pulumi.get(self, "notify_on_fail")
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> str:
+        return pulumi.get(self, "updated_at")
 
     @property
-    @pulumi.getter(name="secretFiles")
-    def secret_files(self) -> Optional[Sequence['outputs.SecretFile']]:
-        return pulumi.get(self, "secret_files")
+    @pulumi.getter
+    def branch(self) -> Optional[str]:
+        return pulumi.get(self, "branch")
 
     @property
-    @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional['outputs.WebServiceServiceDetails']:
-        return pulumi.get(self, "service_details")
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional['outputs.BuildFilter']:
+        return pulumi.get(self, "build_filter")
 
     @property
-    @pulumi.getter
-    def slug(self) -> Optional[str]:
-        return pulumi.get(self, "slug")
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> Optional[str]:
+        return pulumi.get(self, "image_path")
 
     @property
     @pulumi.getter
-    def suspended(self) -> Optional['ServiceSuspended']:
-        return pulumi.get(self, "suspended")
+    def repo(self) -> Optional[str]:
+        return pulumi.get(self, "repo")
 
     @property
-    @pulumi.getter
-    def suspenders(self) -> Optional[Sequence[str]]:
-        return pulumi.get(self, "suspenders")
+    @pulumi.getter(name="serviceDetails")
+    def service_details(self) -> Optional['outputs.StaticSiteDetailsOutput']:
+        return pulumi.get(self, "service_details")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         return pulumi.get(self, "type")
 
-    @property
-    @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[str]:
-        return pulumi.get(self, "updated_at")
-
 
 @pulumi.output_type
-class WebServiceServiceDetails(dict):
+class WebServiceDetailsOutput(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "envSpecificDetails":
+        if key == "buildPlan":
+            suggest = "build_plan"
+        elif key == "envSpecificDetails":
             suggest = "env_specific_details"
         elif key == "healthCheckPath":
             suggest = "health_check_path"
         elif key == "numInstances":
             suggest = "num_instances"
         elif key == "openPorts":
             suggest = "open_ports"
-        elif key == "parentServer":
-            suggest = "parent_server"
         elif key == "pullRequestPreviewsEnabled":
             suggest = "pull_request_previews_enabled"
+        elif key == "parentServer":
+            suggest = "parent_server"
 
         if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in WebServiceServiceDetails. Access the value via the '{suggest}' property getter instead.")
+            pulumi.log.warn(f"Key '{key}' not found in WebServiceDetailsOutput. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
-        WebServiceServiceDetails.__key_warning(key)
+        WebServiceDetailsOutput.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
-        WebServiceServiceDetails.__key_warning(key)
+        WebServiceDetailsOutput.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 env: 'WebServiceServiceDetailsEnv',
+                 build_plan: str,
+                 env: 'WebServiceDetailsOutputEnv',
+                 env_specific_details: Any,
+                 health_check_path: str,
+                 num_instances: int,
+                 open_ports: Sequence['outputs.ServerPort'],
+                 plan: 'WebServiceDetailsOutputPlan',
+                 pull_request_previews_enabled: 'WebServiceDetailsOutputPullRequestPreviewsEnabled',
+                 region: 'WebServiceDetailsOutputRegion',
+                 url: str,
+                 autoscaling: Optional['outputs.AutoscalingConfig'] = None,
                  disk: Optional['outputs.Disk'] = None,
-                 env_specific_details: Optional[Any] = None,
-                 health_check_path: Optional[str] = None,
-                 num_instances: Optional[float] = None,
-                 open_ports: Optional[Sequence['outputs.OpenPorts']] = None,
-                 parent_server: Optional['outputs.WebServiceServiceDetailsParentServerProperties'] = None,
-                 plan: Optional['WebServiceServiceDetailsPlan'] = None,
-                 pull_request_previews_enabled: Optional['WebServiceServiceDetailsPullRequestPreviewsEnabled'] = None,
-                 region: Optional['WebServiceServiceDetailsRegion'] = None,
-                 url: Optional[str] = None):
+                 parent_server: Optional['outputs.Resource'] = None):
+        """
+        :param 'WebServiceDetailsOutputEnv' env: Environment (runtime)
+        :param int num_instances: For a *manually* scaled service, this is the number of instances the service is scaled to. DOES NOT indicate the number of running instances for an *autoscaled* service.
+        :param 'WebServiceDetailsOutputPlan' plan: The instance type to use for the preview instance. Note that base services with any paid instance type can't create preview instances with the `free` instance type.
+        """
+        pulumi.set(__self__, "build_plan", build_plan)
         pulumi.set(__self__, "env", env)
+        pulumi.set(__self__, "env_specific_details", env_specific_details)
+        pulumi.set(__self__, "health_check_path", health_check_path)
+        pulumi.set(__self__, "num_instances", num_instances)
+        pulumi.set(__self__, "open_ports", open_ports)
+        pulumi.set(__self__, "plan", plan)
+        pulumi.set(__self__, "pull_request_previews_enabled", pull_request_previews_enabled)
+        pulumi.set(__self__, "region", region)
+        pulumi.set(__self__, "url", url)
+        if autoscaling is not None:
+            pulumi.set(__self__, "autoscaling", autoscaling)
         if disk is not None:
             pulumi.set(__self__, "disk", disk)
-        if env_specific_details is not None:
-            pulumi.set(__self__, "env_specific_details", env_specific_details)
-        if health_check_path is not None:
-            pulumi.set(__self__, "health_check_path", health_check_path)
-        if num_instances is None:
-            num_instances = 1
-        if num_instances is not None:
-            pulumi.set(__self__, "num_instances", num_instances)
-        if open_ports is not None:
-            pulumi.set(__self__, "open_ports", open_ports)
         if parent_server is not None:
             pulumi.set(__self__, "parent_server", parent_server)
-        if plan is None:
-            plan = 'starter'
-        if plan is not None:
-            pulumi.set(__self__, "plan", plan)
-        if pull_request_previews_enabled is None:
-            pull_request_previews_enabled = 'no'
-        if pull_request_previews_enabled is not None:
-            pulumi.set(__self__, "pull_request_previews_enabled", pull_request_previews_enabled)
-        if region is None:
-            region = 'oregon'
-        if region is not None:
-            pulumi.set(__self__, "region", region)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
 
     @property
-    @pulumi.getter
-    def env(self) -> 'WebServiceServiceDetailsEnv':
-        return pulumi.get(self, "env")
+    @pulumi.getter(name="buildPlan")
+    def build_plan(self) -> str:
+        return pulumi.get(self, "build_plan")
 
     @property
     @pulumi.getter
-    def disk(self) -> Optional['outputs.Disk']:
-        return pulumi.get(self, "disk")
+    def env(self) -> 'WebServiceDetailsOutputEnv':
+        """
+        Environment (runtime)
+        """
+        return pulumi.get(self, "env")
 
     @property
     @pulumi.getter(name="envSpecificDetails")
-    def env_specific_details(self) -> Optional[Any]:
+    def env_specific_details(self) -> Any:
         return pulumi.get(self, "env_specific_details")
 
     @property
     @pulumi.getter(name="healthCheckPath")
-    def health_check_path(self) -> Optional[str]:
+    def health_check_path(self) -> str:
         return pulumi.get(self, "health_check_path")
 
     @property
     @pulumi.getter(name="numInstances")
-    def num_instances(self) -> Optional[float]:
+    def num_instances(self) -> int:
+        """
+        For a *manually* scaled service, this is the number of instances the service is scaled to. DOES NOT indicate the number of running instances for an *autoscaled* service.
+        """
         return pulumi.get(self, "num_instances")
 
     @property
     @pulumi.getter(name="openPorts")
-    def open_ports(self) -> Optional[Sequence['outputs.OpenPorts']]:
+    def open_ports(self) -> Sequence['outputs.ServerPort']:
         return pulumi.get(self, "open_ports")
 
     @property
-    @pulumi.getter(name="parentServer")
-    def parent_server(self) -> Optional['outputs.WebServiceServiceDetailsParentServerProperties']:
-        return pulumi.get(self, "parent_server")
-
-    @property
     @pulumi.getter
-    def plan(self) -> Optional['WebServiceServiceDetailsPlan']:
+    def plan(self) -> 'WebServiceDetailsOutputPlan':
+        """
+        The instance type to use for the preview instance. Note that base services with any paid instance type can't create preview instances with the `free` instance type.
+        """
         return pulumi.get(self, "plan")
 
     @property
     @pulumi.getter(name="pullRequestPreviewsEnabled")
-    def pull_request_previews_enabled(self) -> Optional['WebServiceServiceDetailsPullRequestPreviewsEnabled']:
+    def pull_request_previews_enabled(self) -> 'WebServiceDetailsOutputPullRequestPreviewsEnabled':
         return pulumi.get(self, "pull_request_previews_enabled")
 
     @property
     @pulumi.getter
-    def region(self) -> Optional['WebServiceServiceDetailsRegion']:
+    def region(self) -> 'WebServiceDetailsOutputRegion':
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
-    def url(self) -> Optional[str]:
+    def url(self) -> str:
         return pulumi.get(self, "url")
 
+    @property
+    @pulumi.getter
+    def autoscaling(self) -> Optional['outputs.AutoscalingConfig']:
+        return pulumi.get(self, "autoscaling")
+
+    @property
+    @pulumi.getter
+    def disk(self) -> Optional['outputs.Disk']:
+        return pulumi.get(self, "disk")
+
+    @property
+    @pulumi.getter(name="parentServer")
+    def parent_server(self) -> Optional['outputs.Resource']:
+        return pulumi.get(self, "parent_server")
+
 
 @pulumi.output_type
-class WebServiceServiceDetailsParentServerProperties(dict):
+class WebServiceOutput(dict):
     def __init__(__self__, *,
-                 id: Optional[str] = None,
-                 name: Optional[str] = None):
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+                 auto_deploy: 'ServiceAutoDeploy',
+                 created_at: str,
+                 id: str,
+                 name: str,
+                 notify_on_fail: 'ServiceNotifyOnFail',
+                 owner_id: str,
+                 root_dir: str,
+                 slug: str,
+                 suspended: 'ServiceSuspended',
+                 suspenders: Sequence['ServiceSuspendersItem'],
+                 updated_at: str,
+                 branch: Optional[str] = None,
+                 build_filter: Optional['outputs.BuildFilter'] = None,
+                 image_path: Optional[str] = None,
+                 repo: Optional[str] = None,
+                 service_details: Optional['outputs.WebServiceDetailsOutput'] = None,
+                 type: Optional[str] = None):
+        pulumi.set(__self__, "auto_deploy", auto_deploy)
+        pulumi.set(__self__, "created_at", created_at)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "notify_on_fail", notify_on_fail)
+        pulumi.set(__self__, "owner_id", owner_id)
+        pulumi.set(__self__, "root_dir", root_dir)
+        pulumi.set(__self__, "slug", slug)
+        pulumi.set(__self__, "suspended", suspended)
+        pulumi.set(__self__, "suspenders", suspenders)
+        pulumi.set(__self__, "updated_at", updated_at)
+        if branch is not None:
+            pulumi.set(__self__, "branch", branch)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
+        if image_path is not None:
+            pulumi.set(__self__, "image_path", image_path)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
+        if service_details is not None:
+            pulumi.set(__self__, "service_details", service_details)
+        if type is None:
+            type = 'web_service'
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter(name="autoDeploy")
+    def auto_deploy(self) -> 'ServiceAutoDeploy':
+        return pulumi.get(self, "auto_deploy")
+
+    @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> str:
+        return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
-    def id(self) -> Optional[str]:
+    def id(self) -> str:
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[str]:
+    def name(self) -> str:
         return pulumi.get(self, "name")
 
+    @property
+    @pulumi.getter(name="notifyOnFail")
+    def notify_on_fail(self) -> 'ServiceNotifyOnFail':
+        return pulumi.get(self, "notify_on_fail")
+
+    @property
+    @pulumi.getter(name="ownerId")
+    def owner_id(self) -> str:
+        return pulumi.get(self, "owner_id")
+
+    @property
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> str:
+        return pulumi.get(self, "root_dir")
+
+    @property
+    @pulumi.getter
+    def slug(self) -> str:
+        return pulumi.get(self, "slug")
+
+    @property
+    @pulumi.getter
+    def suspended(self) -> 'ServiceSuspended':
+        return pulumi.get(self, "suspended")
+
+    @property
+    @pulumi.getter
+    def suspenders(self) -> Sequence['ServiceSuspendersItem']:
+        return pulumi.get(self, "suspenders")
+
+    @property
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> str:
+        return pulumi.get(self, "updated_at")
+
+    @property
+    @pulumi.getter
+    def branch(self) -> Optional[str]:
+        return pulumi.get(self, "branch")
+
+    @property
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional['outputs.BuildFilter']:
+        return pulumi.get(self, "build_filter")
+
+    @property
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> Optional[str]:
+        return pulumi.get(self, "image_path")
+
+    @property
+    @pulumi.getter
+    def repo(self) -> Optional[str]:
+        return pulumi.get(self, "repo")
+
+    @property
+    @pulumi.getter(name="serviceDetails")
+    def service_details(self) -> Optional['outputs.WebServiceDetailsOutput']:
+        return pulumi.get(self, "service_details")
+
+    @property
+    @pulumi.getter
+    def type(self) -> Optional[str]:
+        return pulumi.get(self, "type")
+
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/private_service.py` & `pulumi_render-0.2.0/pulumi_render/services/private_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,259 +15,209 @@
 __all__ = ['PrivateServiceArgs', 'PrivateService']
 
 @pulumi.input_type
 class PrivateServiceArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  owner_id: pulumi.Input[str],
-                 repo: pulumi.Input[str],
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
+                 build_filter: Optional[pulumi.Input['BuildFilterArgs']] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]] = None,
+                 image: Optional[pulumi.Input['ImageArgs']] = None,
+                 repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]] = None,
-                 service_details: Optional[pulumi.Input['PrivateServiceDetailsArgs']] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None):
+                 service_details: Optional[pulumi.Input['PrivateServiceDetailsCreateArgs']] = None,
+                 type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a PrivateService resource.
-        :param pulumi.Input[str] owner_id: The id of the owner (user/team).
+        :param pulumi.Input['ServiceCreateAutoDeploy'] auto_deploy: Defaults to "yes"
+        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository
         :param pulumi.Input[str] repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param pulumi.Input['ServiceAutoDeploy'] auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository.
-        :param pulumi.Input['ServiceNotifyOnFail'] notify_on_fail: The notification setting for this service upon deployment failure.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
         if auto_deploy is None:
-            auto_deploy = 'no'
+            auto_deploy = 'yes'
         if auto_deploy is not None:
             pulumi.set(__self__, "auto_deploy", auto_deploy)
         if branch is not None:
             pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
         if env_vars is not None:
             pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
+        if image is not None:
+            pulumi.set(__self__, "image", image)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
+        if root_dir is not None:
+            pulumi.set(__self__, "root_dir", root_dir)
         if secret_files is not None:
             pulumi.set(__self__, "secret_files", secret_files)
         if service_details is not None:
             pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
         if type is None:
             type = 'private_service'
         if type is not None:
             pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> pulumi.Input[str]:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @owner_id.setter
     def owner_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "owner_id", value)
 
     @property
-    @pulumi.getter
-    def repo(self) -> pulumi.Input[str]:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
-        return pulumi.get(self, "repo")
-
-    @repo.setter
-    def repo(self, value: pulumi.Input[str]):
-        pulumi.set(self, "repo", value)
-
-    @property
     @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional[pulumi.Input['ServiceAutoDeploy']]:
+    def auto_deploy(self) -> Optional[pulumi.Input['ServiceCreateAutoDeploy']]:
         """
-        Whether to auto deploy the service or not upon git push.
+        Defaults to "yes"
         """
         return pulumi.get(self, "auto_deploy")
 
     @auto_deploy.setter
-    def auto_deploy(self, value: Optional[pulumi.Input['ServiceAutoDeploy']]):
+    def auto_deploy(self, value: Optional[pulumi.Input['ServiceCreateAutoDeploy']]):
         pulumi.set(self, "auto_deploy", value)
 
     @property
     @pulumi.getter
     def branch(self) -> Optional[pulumi.Input[str]]:
         """
-        If left empty, this will fall back to the default branch of the repository.
+        If left empty, this will fall back to the default branch of the repository
         """
         return pulumi.get(self, "branch")
 
     @branch.setter
     def branch(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "branch", value)
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "created_at")
-
-    @created_at.setter
-    def created_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "created_at", value)
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional[pulumi.Input['BuildFilterArgs']]:
+        return pulumi.get(self, "build_filter")
+
+    @build_filter.setter
+    def build_filter(self, value: Optional[pulumi.Input['BuildFilterArgs']]):
+        pulumi.set(self, "build_filter", value)
 
     @property
     @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]]:
+    def env_vars(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]]:
         return pulumi.get(self, "env_vars")
 
     @env_vars.setter
-    def env_vars(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]]):
+    def env_vars(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]]):
         pulumi.set(self, "env_vars", value)
 
     @property
-    @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional[pulumi.Input['ServiceNotifyOnFail']]:
+    @pulumi.getter
+    def image(self) -> Optional[pulumi.Input['ImageArgs']]:
+        return pulumi.get(self, "image")
+
+    @image.setter
+    def image(self, value: Optional[pulumi.Input['ImageArgs']]):
+        pulumi.set(self, "image", value)
+
+    @property
+    @pulumi.getter
+    def repo(self) -> Optional[pulumi.Input[str]]:
         """
-        The notification setting for this service upon deployment failure.
+        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
         """
-        return pulumi.get(self, "notify_on_fail")
+        return pulumi.get(self, "repo")
 
-    @notify_on_fail.setter
-    def notify_on_fail(self, value: Optional[pulumi.Input['ServiceNotifyOnFail']]):
-        pulumi.set(self, "notify_on_fail", value)
+    @repo.setter
+    def repo(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "repo", value)
+
+    @property
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "root_dir")
+
+    @root_dir.setter
+    def root_dir(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "root_dir", value)
 
     @property
     @pulumi.getter(name="secretFiles")
     def secret_files(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]]:
         return pulumi.get(self, "secret_files")
 
     @secret_files.setter
     def secret_files(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]]):
         pulumi.set(self, "secret_files", value)
 
     @property
     @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional[pulumi.Input['PrivateServiceDetailsArgs']]:
+    def service_details(self) -> Optional[pulumi.Input['PrivateServiceDetailsCreateArgs']]:
         return pulumi.get(self, "service_details")
 
     @service_details.setter
-    def service_details(self, value: Optional[pulumi.Input['PrivateServiceDetailsArgs']]):
+    def service_details(self, value: Optional[pulumi.Input['PrivateServiceDetailsCreateArgs']]):
         pulumi.set(self, "service_details", value)
 
     @property
     @pulumi.getter
-    def slug(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "slug")
-
-    @slug.setter
-    def slug(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "slug", value)
-
-    @property
-    @pulumi.getter
-    def suspended(self) -> Optional[pulumi.Input['ServiceSuspended']]:
-        return pulumi.get(self, "suspended")
-
-    @suspended.setter
-    def suspended(self, value: Optional[pulumi.Input['ServiceSuspended']]):
-        pulumi.set(self, "suspended", value)
-
-    @property
-    @pulumi.getter
-    def suspenders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "suspenders")
-
-    @suspenders.setter
-    def suspenders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "suspenders", value)
-
-    @property
-    @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
-    @property
-    @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "updated_at")
-
-    @updated_at.setter
-    def updated_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "updated_at", value)
-
 
 class PrivateService(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvVarKeyValueArgs']]]]] = None,
+                 build_filter: Optional[pulumi.Input[pulumi.InputType['BuildFilterArgs']]] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union[pulumi.InputType['EnvVarKeyValueArgs'], pulumi.InputType['EnvVarKeyGenerateValueArgs']]]]]] = None,
+                 image: Optional[pulumi.Input[pulumi.InputType['ImageArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
                  owner_id: Optional[pulumi.Input[str]] = None,
                  repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretFileArgs']]]]] = None,
-                 service_details: Optional[pulumi.Input[pulumi.InputType['PrivateServiceDetailsArgs']]] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 service_details: Optional[pulumi.Input[pulumi.InputType['PrivateServiceDetailsCreateArgs']]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        A private service
-
+        Create a PrivateService resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input['ServiceAutoDeploy'] auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository.
-        :param pulumi.Input['ServiceNotifyOnFail'] notify_on_fail: The notification setting for this service upon deployment failure.
-        :param pulumi.Input[str] owner_id: The id of the owner (user/team).
+        :param pulumi.Input['ServiceCreateAutoDeploy'] auto_deploy: Defaults to "yes"
+        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository
         :param pulumi.Input[str] repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: PrivateServiceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        A private service
-
+        Create a PrivateService resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param PrivateServiceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(PrivateServiceArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -275,63 +225,62 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvVarKeyValueArgs']]]]] = None,
+                 build_filter: Optional[pulumi.Input[pulumi.InputType['BuildFilterArgs']]] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union[pulumi.InputType['EnvVarKeyValueArgs'], pulumi.InputType['EnvVarKeyGenerateValueArgs']]]]]] = None,
+                 image: Optional[pulumi.Input[pulumi.InputType['ImageArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
                  owner_id: Optional[pulumi.Input[str]] = None,
                  repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretFileArgs']]]]] = None,
-                 service_details: Optional[pulumi.Input[pulumi.InputType['PrivateServiceDetailsArgs']]] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 service_details: Optional[pulumi.Input[pulumi.InputType['PrivateServiceDetailsCreateArgs']]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PrivateServiceArgs.__new__(PrivateServiceArgs)
 
             if auto_deploy is None:
-                auto_deploy = 'no'
+                auto_deploy = 'yes'
             __props__.__dict__["auto_deploy"] = auto_deploy
             __props__.__dict__["branch"] = branch
-            __props__.__dict__["created_at"] = created_at
+            __props__.__dict__["build_filter"] = build_filter
             __props__.__dict__["env_vars"] = env_vars
+            __props__.__dict__["image"] = image
             if name is None and not opts.urn:
                 raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
-            __props__.__dict__["notify_on_fail"] = notify_on_fail
             if owner_id is None and not opts.urn:
                 raise TypeError("Missing required property 'owner_id'")
             __props__.__dict__["owner_id"] = owner_id
-            if repo is None and not opts.urn:
-                raise TypeError("Missing required property 'repo'")
             __props__.__dict__["repo"] = repo
+            __props__.__dict__["root_dir"] = root_dir
             __props__.__dict__["secret_files"] = secret_files
             __props__.__dict__["service_details"] = service_details
-            __props__.__dict__["slug"] = slug
-            __props__.__dict__["suspended"] = suspended
-            __props__.__dict__["suspenders"] = suspenders
             if type is None:
                 type = 'private_service'
             __props__.__dict__["type"] = type
-            __props__.__dict__["updated_at"] = updated_at
+            __props__.__dict__["created_at"] = None
+            __props__.__dict__["image_path"] = None
+            __props__.__dict__["notify_on_fail"] = None
+            __props__.__dict__["slug"] = None
+            __props__.__dict__["suspended"] = None
+            __props__.__dict__["suspenders"] = None
+            __props__.__dict__["updated_at"] = None
         super(PrivateService, __self__).__init__(
             'render:services:PrivateService',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -348,107 +297,116 @@
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = PrivateServiceArgs.__new__(PrivateServiceArgs)
 
         __props__.__dict__["auto_deploy"] = None
         __props__.__dict__["branch"] = None
+        __props__.__dict__["build_filter"] = None
         __props__.__dict__["created_at"] = None
         __props__.__dict__["env_vars"] = None
+        __props__.__dict__["image"] = None
+        __props__.__dict__["image_path"] = None
         __props__.__dict__["name"] = None
         __props__.__dict__["notify_on_fail"] = None
         __props__.__dict__["owner_id"] = None
         __props__.__dict__["repo"] = None
+        __props__.__dict__["root_dir"] = None
         __props__.__dict__["secret_files"] = None
         __props__.__dict__["service_details"] = None
         __props__.__dict__["slug"] = None
         __props__.__dict__["suspended"] = None
         __props__.__dict__["suspenders"] = None
         __props__.__dict__["type"] = None
         __props__.__dict__["updated_at"] = None
         return PrivateService(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="autoDeploy")
     def auto_deploy(self) -> pulumi.Output[Optional['ServiceAutoDeploy']]:
-        """
-        Whether to auto deploy the service or not upon git push.
-        """
         return pulumi.get(self, "auto_deploy")
 
     @property
     @pulumi.getter
     def branch(self) -> pulumi.Output[Optional[str]]:
-        """
-        If left empty, this will fall back to the default branch of the repository.
-        """
         return pulumi.get(self, "branch")
 
     @property
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> pulumi.Output[Optional['outputs.BuildFilter']]:
+        return pulumi.get(self, "build_filter")
+
+    @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter(name="envVars")
-    def env_vars(self) -> pulumi.Output[Optional[Sequence['outputs.EnvVarKeyValue']]]:
+    def env_vars(self) -> pulumi.Output[Optional[Sequence[Any]]]:
         return pulumi.get(self, "env_vars")
 
     @property
     @pulumi.getter
+    def image(self) -> pulumi.Output[Optional['outputs.Image']]:
+        return pulumi.get(self, "image")
+
+    @property
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "image_path")
+
+    @property
+    @pulumi.getter
     def name(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="notifyOnFail")
     def notify_on_fail(self) -> pulumi.Output[Optional['ServiceNotifyOnFail']]:
-        """
-        The notification setting for this service upon deployment failure.
-        """
         return pulumi.get(self, "notify_on_fail")
 
     @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> pulumi.Output[Optional[str]]:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @property
     @pulumi.getter
     def repo(self) -> pulumi.Output[Optional[str]]:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
         return pulumi.get(self, "repo")
 
     @property
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "root_dir")
+
+    @property
     @pulumi.getter(name="secretFiles")
     def secret_files(self) -> pulumi.Output[Optional[Sequence['outputs.SecretFile']]]:
         return pulumi.get(self, "secret_files")
 
     @property
     @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> pulumi.Output[Optional['outputs.PrivateServiceDetails']]:
+    def service_details(self) -> pulumi.Output[Optional['outputs.PrivateServiceDetailsOutput']]:
         return pulumi.get(self, "service_details")
 
     @property
     @pulumi.getter
     def slug(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "slug")
 
     @property
     @pulumi.getter
     def suspended(self) -> pulumi.Output[Optional['ServiceSuspended']]:
         return pulumi.get(self, "suspended")
 
     @property
     @pulumi.getter
-    def suspenders(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    def suspenders(self) -> pulumi.Output[Optional[Sequence['ServiceSuspendersItem']]]:
         return pulumi.get(self, "suspenders")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "type")
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/scale.py` & `pulumi_render-0.2.0/pulumi_render/services/scale_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,126 +5,126 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
-__all__ = ['ScaleArgs', 'Scale']
+__all__ = ['ScaleServiceArgs', 'ScaleService']
 
 @pulumi.input_type
-class ScaleArgs:
+class ScaleServiceArgs:
     def __init__(__self__, *,
-                 num_instances: pulumi.Input[float],
+                 num_instances: pulumi.Input[int],
                  service_id: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Scale resource.
-        :param pulumi.Input[str] service_id: (Required) The ID of the service
+        The set of arguments for constructing a ScaleService resource.
+        :param pulumi.Input[str] service_id: The ID of the service
         """
         pulumi.set(__self__, "num_instances", num_instances)
         if service_id is not None:
             pulumi.set(__self__, "service_id", service_id)
 
     @property
     @pulumi.getter(name="numInstances")
-    def num_instances(self) -> pulumi.Input[float]:
+    def num_instances(self) -> pulumi.Input[int]:
         return pulumi.get(self, "num_instances")
 
     @num_instances.setter
-    def num_instances(self, value: pulumi.Input[float]):
+    def num_instances(self, value: pulumi.Input[int]):
         pulumi.set(self, "num_instances", value)
 
     @property
     @pulumi.getter(name="serviceId")
     def service_id(self) -> Optional[pulumi.Input[str]]:
         """
-        (Required) The ID of the service
+        The ID of the service
         """
         return pulumi.get(self, "service_id")
 
     @service_id.setter
     def service_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_id", value)
 
 
-class Scale(pulumi.CustomResource):
+class ScaleService(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 num_instances: Optional[pulumi.Input[float]] = None,
+                 num_instances: Optional[pulumi.Input[int]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a Scale resource with the given unique name, props, and options.
+        Create a ScaleService resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] service_id: (Required) The ID of the service
+        :param pulumi.Input[str] service_id: The ID of the service
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ScaleArgs,
+                 args: ScaleServiceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Scale resource with the given unique name, props, and options.
+        Create a ScaleService resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param ScaleArgs args: The arguments to use to populate this resource's properties.
+        :param ScaleServiceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ScaleArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ScaleServiceArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 num_instances: Optional[pulumi.Input[float]] = None,
+                 num_instances: Optional[pulumi.Input[int]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ScaleArgs.__new__(ScaleArgs)
+            __props__ = ScaleServiceArgs.__new__(ScaleServiceArgs)
 
             if num_instances is None and not opts.urn:
                 raise TypeError("Missing required property 'num_instances'")
             __props__.__dict__["num_instances"] = num_instances
             __props__.__dict__["service_id"] = service_id
-        super(Scale, __self__).__init__(
-            'render:services:Scale',
+        super(ScaleService, __self__).__init__(
+            'render:services:ScaleService',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'Scale':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'ScaleService':
         """
-        Get an existing Scale resource's state with the given name, id, and optional extra
+        Get an existing ScaleService resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = ScaleArgs.__new__(ScaleArgs)
+        __props__ = ScaleServiceArgs.__new__(ScaleServiceArgs)
 
         __props__.__dict__["num_instances"] = None
-        return Scale(resource_name, opts=opts, __props__=__props__)
+        return ScaleService(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="numInstances")
-    def num_instances(self) -> pulumi.Output[float]:
+    def num_instances(self) -> pulumi.Output[int]:
         return pulumi.get(self, "num_instances")
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/static_site.py` & `pulumi_render-0.2.0/pulumi_render/services/static_site.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,261 +15,209 @@
 __all__ = ['StaticSiteArgs', 'StaticSite']
 
 @pulumi.input_type
 class StaticSiteArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  owner_id: pulumi.Input[str],
-                 repo: pulumi.Input[str],
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
+                 build_filter: Optional[pulumi.Input['BuildFilterArgs']] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]] = None,
+                 image: Optional[pulumi.Input['ImageArgs']] = None,
+                 repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]] = None,
-                 service_details: Optional[pulumi.Input['StaticSiteServiceDetailsArgs']] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None):
+                 service_details: Optional[pulumi.Input['StaticSiteDetailsCreateArgs']] = None,
+                 type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a StaticSite resource.
-        :param pulumi.Input[str] owner_id: The id of the owner (user/team).
+        :param pulumi.Input['ServiceCreateAutoDeploy'] auto_deploy: Defaults to "yes"
+        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository
         :param pulumi.Input[str] repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param pulumi.Input['ServiceAutoDeploy'] auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository.
-        :param pulumi.Input['ServiceNotifyOnFail'] notify_on_fail: The notification setting for this service upon deployment failure.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
         if auto_deploy is None:
-            auto_deploy = 'no'
+            auto_deploy = 'yes'
         if auto_deploy is not None:
             pulumi.set(__self__, "auto_deploy", auto_deploy)
         if branch is not None:
             pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
         if env_vars is not None:
             pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
+        if image is not None:
+            pulumi.set(__self__, "image", image)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
+        if root_dir is not None:
+            pulumi.set(__self__, "root_dir", root_dir)
         if secret_files is not None:
             pulumi.set(__self__, "secret_files", secret_files)
         if service_details is not None:
             pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
         if type is None:
             type = 'static_site'
         if type is not None:
             pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> pulumi.Input[str]:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @owner_id.setter
     def owner_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "owner_id", value)
 
     @property
-    @pulumi.getter
-    def repo(self) -> pulumi.Input[str]:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
-        return pulumi.get(self, "repo")
-
-    @repo.setter
-    def repo(self, value: pulumi.Input[str]):
-        pulumi.set(self, "repo", value)
-
-    @property
     @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional[pulumi.Input['ServiceAutoDeploy']]:
+    def auto_deploy(self) -> Optional[pulumi.Input['ServiceCreateAutoDeploy']]:
         """
-        Whether to auto deploy the service or not upon git push.
+        Defaults to "yes"
         """
         return pulumi.get(self, "auto_deploy")
 
     @auto_deploy.setter
-    def auto_deploy(self, value: Optional[pulumi.Input['ServiceAutoDeploy']]):
+    def auto_deploy(self, value: Optional[pulumi.Input['ServiceCreateAutoDeploy']]):
         pulumi.set(self, "auto_deploy", value)
 
     @property
     @pulumi.getter
     def branch(self) -> Optional[pulumi.Input[str]]:
         """
-        If left empty, this will fall back to the default branch of the repository.
+        If left empty, this will fall back to the default branch of the repository
         """
         return pulumi.get(self, "branch")
 
     @branch.setter
     def branch(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "branch", value)
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "created_at")
-
-    @created_at.setter
-    def created_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "created_at", value)
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional[pulumi.Input['BuildFilterArgs']]:
+        return pulumi.get(self, "build_filter")
+
+    @build_filter.setter
+    def build_filter(self, value: Optional[pulumi.Input['BuildFilterArgs']]):
+        pulumi.set(self, "build_filter", value)
 
     @property
     @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]]:
+    def env_vars(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]]:
         return pulumi.get(self, "env_vars")
 
     @env_vars.setter
-    def env_vars(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]]):
+    def env_vars(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]]):
         pulumi.set(self, "env_vars", value)
 
     @property
-    @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional[pulumi.Input['ServiceNotifyOnFail']]:
+    @pulumi.getter
+    def image(self) -> Optional[pulumi.Input['ImageArgs']]:
+        return pulumi.get(self, "image")
+
+    @image.setter
+    def image(self, value: Optional[pulumi.Input['ImageArgs']]):
+        pulumi.set(self, "image", value)
+
+    @property
+    @pulumi.getter
+    def repo(self) -> Optional[pulumi.Input[str]]:
         """
-        The notification setting for this service upon deployment failure.
+        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
         """
-        return pulumi.get(self, "notify_on_fail")
+        return pulumi.get(self, "repo")
 
-    @notify_on_fail.setter
-    def notify_on_fail(self, value: Optional[pulumi.Input['ServiceNotifyOnFail']]):
-        pulumi.set(self, "notify_on_fail", value)
+    @repo.setter
+    def repo(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "repo", value)
+
+    @property
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "root_dir")
+
+    @root_dir.setter
+    def root_dir(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "root_dir", value)
 
     @property
     @pulumi.getter(name="secretFiles")
     def secret_files(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]]:
         return pulumi.get(self, "secret_files")
 
     @secret_files.setter
     def secret_files(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]]):
         pulumi.set(self, "secret_files", value)
 
     @property
     @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional[pulumi.Input['StaticSiteServiceDetailsArgs']]:
+    def service_details(self) -> Optional[pulumi.Input['StaticSiteDetailsCreateArgs']]:
         return pulumi.get(self, "service_details")
 
     @service_details.setter
-    def service_details(self, value: Optional[pulumi.Input['StaticSiteServiceDetailsArgs']]):
+    def service_details(self, value: Optional[pulumi.Input['StaticSiteDetailsCreateArgs']]):
         pulumi.set(self, "service_details", value)
 
     @property
     @pulumi.getter
-    def slug(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "slug")
-
-    @slug.setter
-    def slug(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "slug", value)
-
-    @property
-    @pulumi.getter
-    def suspended(self) -> Optional[pulumi.Input['ServiceSuspended']]:
-        return pulumi.get(self, "suspended")
-
-    @suspended.setter
-    def suspended(self, value: Optional[pulumi.Input['ServiceSuspended']]):
-        pulumi.set(self, "suspended", value)
-
-    @property
-    @pulumi.getter
-    def suspenders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "suspenders")
-
-    @suspenders.setter
-    def suspenders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "suspenders", value)
-
-    @property
-    @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
-    @property
-    @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "updated_at")
-
-    @updated_at.setter
-    def updated_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "updated_at", value)
-
 
 class StaticSite(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvVarKeyValueArgs']]]]] = None,
+                 build_filter: Optional[pulumi.Input[pulumi.InputType['BuildFilterArgs']]] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union[pulumi.InputType['EnvVarKeyValueArgs'], pulumi.InputType['EnvVarKeyGenerateValueArgs']]]]]] = None,
+                 image: Optional[pulumi.Input[pulumi.InputType['ImageArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
                  owner_id: Optional[pulumi.Input[str]] = None,
                  repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretFileArgs']]]]] = None,
-                 service_details: Optional[pulumi.Input[pulumi.InputType['StaticSiteServiceDetailsArgs']]] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 service_details: Optional[pulumi.Input[pulumi.InputType['StaticSiteDetailsCreateArgs']]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        A static website service
-
         ## Example Usage
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input['ServiceAutoDeploy'] auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository.
-        :param pulumi.Input['ServiceNotifyOnFail'] notify_on_fail: The notification setting for this service upon deployment failure.
-        :param pulumi.Input[str] owner_id: The id of the owner (user/team).
+        :param pulumi.Input['ServiceCreateAutoDeploy'] auto_deploy: Defaults to "yes"
+        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository
         :param pulumi.Input[str] repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: StaticSiteArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        A static website service
-
         ## Example Usage
 
         :param str resource_name: The name of the resource.
         :param StaticSiteArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -279,63 +227,62 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvVarKeyValueArgs']]]]] = None,
+                 build_filter: Optional[pulumi.Input[pulumi.InputType['BuildFilterArgs']]] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union[pulumi.InputType['EnvVarKeyValueArgs'], pulumi.InputType['EnvVarKeyGenerateValueArgs']]]]]] = None,
+                 image: Optional[pulumi.Input[pulumi.InputType['ImageArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
                  owner_id: Optional[pulumi.Input[str]] = None,
                  repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretFileArgs']]]]] = None,
-                 service_details: Optional[pulumi.Input[pulumi.InputType['StaticSiteServiceDetailsArgs']]] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 service_details: Optional[pulumi.Input[pulumi.InputType['StaticSiteDetailsCreateArgs']]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = StaticSiteArgs.__new__(StaticSiteArgs)
 
             if auto_deploy is None:
-                auto_deploy = 'no'
+                auto_deploy = 'yes'
             __props__.__dict__["auto_deploy"] = auto_deploy
             __props__.__dict__["branch"] = branch
-            __props__.__dict__["created_at"] = created_at
+            __props__.__dict__["build_filter"] = build_filter
             __props__.__dict__["env_vars"] = env_vars
+            __props__.__dict__["image"] = image
             if name is None and not opts.urn:
                 raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
-            __props__.__dict__["notify_on_fail"] = notify_on_fail
             if owner_id is None and not opts.urn:
                 raise TypeError("Missing required property 'owner_id'")
             __props__.__dict__["owner_id"] = owner_id
-            if repo is None and not opts.urn:
-                raise TypeError("Missing required property 'repo'")
             __props__.__dict__["repo"] = repo
+            __props__.__dict__["root_dir"] = root_dir
             __props__.__dict__["secret_files"] = secret_files
             __props__.__dict__["service_details"] = service_details
-            __props__.__dict__["slug"] = slug
-            __props__.__dict__["suspended"] = suspended
-            __props__.__dict__["suspenders"] = suspenders
             if type is None:
                 type = 'static_site'
             __props__.__dict__["type"] = type
-            __props__.__dict__["updated_at"] = updated_at
+            __props__.__dict__["created_at"] = None
+            __props__.__dict__["image_path"] = None
+            __props__.__dict__["notify_on_fail"] = None
+            __props__.__dict__["slug"] = None
+            __props__.__dict__["suspended"] = None
+            __props__.__dict__["suspenders"] = None
+            __props__.__dict__["updated_at"] = None
         super(StaticSite, __self__).__init__(
             'render:services:StaticSite',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -352,107 +299,116 @@
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = StaticSiteArgs.__new__(StaticSiteArgs)
 
         __props__.__dict__["auto_deploy"] = None
         __props__.__dict__["branch"] = None
+        __props__.__dict__["build_filter"] = None
         __props__.__dict__["created_at"] = None
         __props__.__dict__["env_vars"] = None
+        __props__.__dict__["image"] = None
+        __props__.__dict__["image_path"] = None
         __props__.__dict__["name"] = None
         __props__.__dict__["notify_on_fail"] = None
         __props__.__dict__["owner_id"] = None
         __props__.__dict__["repo"] = None
+        __props__.__dict__["root_dir"] = None
         __props__.__dict__["secret_files"] = None
         __props__.__dict__["service_details"] = None
         __props__.__dict__["slug"] = None
         __props__.__dict__["suspended"] = None
         __props__.__dict__["suspenders"] = None
         __props__.__dict__["type"] = None
         __props__.__dict__["updated_at"] = None
         return StaticSite(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="autoDeploy")
     def auto_deploy(self) -> pulumi.Output[Optional['ServiceAutoDeploy']]:
-        """
-        Whether to auto deploy the service or not upon git push.
-        """
         return pulumi.get(self, "auto_deploy")
 
     @property
     @pulumi.getter
     def branch(self) -> pulumi.Output[Optional[str]]:
-        """
-        If left empty, this will fall back to the default branch of the repository.
-        """
         return pulumi.get(self, "branch")
 
     @property
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> pulumi.Output[Optional['outputs.BuildFilter']]:
+        return pulumi.get(self, "build_filter")
+
+    @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter(name="envVars")
-    def env_vars(self) -> pulumi.Output[Optional[Sequence['outputs.EnvVarKeyValue']]]:
+    def env_vars(self) -> pulumi.Output[Optional[Sequence[Any]]]:
         return pulumi.get(self, "env_vars")
 
     @property
     @pulumi.getter
+    def image(self) -> pulumi.Output[Optional['outputs.Image']]:
+        return pulumi.get(self, "image")
+
+    @property
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "image_path")
+
+    @property
+    @pulumi.getter
     def name(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="notifyOnFail")
     def notify_on_fail(self) -> pulumi.Output[Optional['ServiceNotifyOnFail']]:
-        """
-        The notification setting for this service upon deployment failure.
-        """
         return pulumi.get(self, "notify_on_fail")
 
     @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> pulumi.Output[Optional[str]]:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @property
     @pulumi.getter
     def repo(self) -> pulumi.Output[Optional[str]]:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
         return pulumi.get(self, "repo")
 
     @property
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "root_dir")
+
+    @property
     @pulumi.getter(name="secretFiles")
     def secret_files(self) -> pulumi.Output[Optional[Sequence['outputs.SecretFile']]]:
         return pulumi.get(self, "secret_files")
 
     @property
     @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> pulumi.Output[Optional['outputs.StaticSiteServiceDetails']]:
+    def service_details(self) -> pulumi.Output[Optional['outputs.StaticSiteDetailsOutput']]:
         return pulumi.get(self, "service_details")
 
     @property
     @pulumi.getter
     def slug(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "slug")
 
     @property
     @pulumi.getter
     def suspended(self) -> pulumi.Output[Optional['ServiceSuspended']]:
         return pulumi.get(self, "suspended")
 
     @property
     @pulumi.getter
-    def suspenders(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    def suspenders(self) -> pulumi.Output[Optional[Sequence['ServiceSuspendersItem']]]:
         return pulumi.get(self, "suspenders")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "type")
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/suspend.py` & `pulumi_render-0.2.0/pulumi_render/services/restart_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,68 +5,68 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
-__all__ = ['SuspendArgs', 'Suspend']
+__all__ = ['RestartServerArgs', 'RestartServer']
 
 @pulumi.input_type
-class SuspendArgs:
+class RestartServerArgs:
     def __init__(__self__, *,
                  service_id: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Suspend resource.
-        :param pulumi.Input[str] service_id: (Required) The ID of the service
+        The set of arguments for constructing a RestartServer resource.
+        :param pulumi.Input[str] service_id: The ID of the service
         """
         if service_id is not None:
             pulumi.set(__self__, "service_id", service_id)
 
     @property
     @pulumi.getter(name="serviceId")
     def service_id(self) -> Optional[pulumi.Input[str]]:
         """
-        (Required) The ID of the service
+        The ID of the service
         """
         return pulumi.get(self, "service_id")
 
     @service_id.setter
     def service_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_id", value)
 
 
-class Suspend(pulumi.CustomResource):
+class RestartServer(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a Suspend resource with the given unique name, props, and options.
+        Create a RestartServer resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] service_id: (Required) The ID of the service
+        :param pulumi.Input[str] service_id: The ID of the service
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[SuspendArgs] = None,
+                 args: Optional[RestartServerArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Suspend resource with the given unique name, props, and options.
+        Create a RestartServer resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param SuspendArgs args: The arguments to use to populate this resource's properties.
+        :param RestartServerArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(SuspendArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(RestartServerArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -75,34 +75,34 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = SuspendArgs.__new__(SuspendArgs)
+            __props__ = RestartServerArgs.__new__(RestartServerArgs)
 
             __props__.__dict__["service_id"] = service_id
-        super(Suspend, __self__).__init__(
-            'render:services:Suspend',
+        super(RestartServer, __self__).__init__(
+            'render:services:RestartServer',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'Suspend':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'RestartServer':
         """
-        Get an existing Suspend resource's state with the given name, id, and optional extra
+        Get an existing RestartServer resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = SuspendArgs.__new__(SuspendArgs)
+        __props__ = RestartServerArgs.__new__(RestartServerArgs)
 
-        return Suspend(resource_name, opts=opts, __props__=__props__)
+        return RestartServer(resource_name, opts=opts, __props__=__props__)
```

### Comparing `pulumi_render-0.1.1/pulumi_render/services/web_service.py` & `pulumi_render-0.2.0/pulumi_render/services/cron_job.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,447 +8,405 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._enums import *
 from ._inputs import *
 
-__all__ = ['WebServiceArgs', 'WebService']
+__all__ = ['CronJobArgs', 'CronJob']
 
 @pulumi.input_type
-class WebServiceArgs:
+class CronJobArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  owner_id: pulumi.Input[str],
-                 repo: pulumi.Input[str],
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
+                 build_filter: Optional[pulumi.Input['BuildFilterArgs']] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]] = None,
+                 image: Optional[pulumi.Input['ImageArgs']] = None,
+                 repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]] = None,
-                 service_details: Optional[pulumi.Input['WebServiceServiceDetailsArgs']] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None):
+                 service_details: Optional[pulumi.Input['CronJobDetailsCreateArgs']] = None,
+                 type: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a WebService resource.
-        :param pulumi.Input[str] owner_id: The id of the owner (user/team).
+        The set of arguments for constructing a CronJob resource.
+        :param pulumi.Input['ServiceCreateAutoDeploy'] auto_deploy: Defaults to "yes"
+        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository
         :param pulumi.Input[str] repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        :param pulumi.Input['ServiceAutoDeploy'] auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository.
-        :param pulumi.Input['ServiceNotifyOnFail'] notify_on_fail: The notification setting for this service upon deployment failure.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "owner_id", owner_id)
-        pulumi.set(__self__, "repo", repo)
         if auto_deploy is None:
-            auto_deploy = 'no'
+            auto_deploy = 'yes'
         if auto_deploy is not None:
             pulumi.set(__self__, "auto_deploy", auto_deploy)
         if branch is not None:
             pulumi.set(__self__, "branch", branch)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
+        if build_filter is not None:
+            pulumi.set(__self__, "build_filter", build_filter)
         if env_vars is not None:
             pulumi.set(__self__, "env_vars", env_vars)
-        if notify_on_fail is not None:
-            pulumi.set(__self__, "notify_on_fail", notify_on_fail)
+        if image is not None:
+            pulumi.set(__self__, "image", image)
+        if repo is not None:
+            pulumi.set(__self__, "repo", repo)
+        if root_dir is not None:
+            pulumi.set(__self__, "root_dir", root_dir)
         if secret_files is not None:
             pulumi.set(__self__, "secret_files", secret_files)
         if service_details is not None:
             pulumi.set(__self__, "service_details", service_details)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-        if suspended is not None:
-            pulumi.set(__self__, "suspended", suspended)
-        if suspenders is not None:
-            pulumi.set(__self__, "suspenders", suspenders)
         if type is None:
-            type = 'web_service'
+            type = 'cron_job'
         if type is not None:
             pulumi.set(__self__, "type", type)
-        if updated_at is not None:
-            pulumi.set(__self__, "updated_at", updated_at)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> pulumi.Input[str]:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @owner_id.setter
     def owner_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "owner_id", value)
 
     @property
-    @pulumi.getter
-    def repo(self) -> pulumi.Input[str]:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
-        return pulumi.get(self, "repo")
-
-    @repo.setter
-    def repo(self, value: pulumi.Input[str]):
-        pulumi.set(self, "repo", value)
-
-    @property
     @pulumi.getter(name="autoDeploy")
-    def auto_deploy(self) -> Optional[pulumi.Input['ServiceAutoDeploy']]:
+    def auto_deploy(self) -> Optional[pulumi.Input['ServiceCreateAutoDeploy']]:
         """
-        Whether to auto deploy the service or not upon git push.
+        Defaults to "yes"
         """
         return pulumi.get(self, "auto_deploy")
 
     @auto_deploy.setter
-    def auto_deploy(self, value: Optional[pulumi.Input['ServiceAutoDeploy']]):
+    def auto_deploy(self, value: Optional[pulumi.Input['ServiceCreateAutoDeploy']]):
         pulumi.set(self, "auto_deploy", value)
 
     @property
     @pulumi.getter
     def branch(self) -> Optional[pulumi.Input[str]]:
         """
-        If left empty, this will fall back to the default branch of the repository.
+        If left empty, this will fall back to the default branch of the repository
         """
         return pulumi.get(self, "branch")
 
     @branch.setter
     def branch(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "branch", value)
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "created_at")
-
-    @created_at.setter
-    def created_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "created_at", value)
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> Optional[pulumi.Input['BuildFilterArgs']]:
+        return pulumi.get(self, "build_filter")
+
+    @build_filter.setter
+    def build_filter(self, value: Optional[pulumi.Input['BuildFilterArgs']]):
+        pulumi.set(self, "build_filter", value)
 
     @property
     @pulumi.getter(name="envVars")
-    def env_vars(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]]:
+    def env_vars(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]]:
         return pulumi.get(self, "env_vars")
 
     @env_vars.setter
-    def env_vars(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]]):
+    def env_vars(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Union['EnvVarKeyValueArgs', 'EnvVarKeyGenerateValueArgs']]]]]):
         pulumi.set(self, "env_vars", value)
 
     @property
-    @pulumi.getter(name="notifyOnFail")
-    def notify_on_fail(self) -> Optional[pulumi.Input['ServiceNotifyOnFail']]:
+    @pulumi.getter
+    def image(self) -> Optional[pulumi.Input['ImageArgs']]:
+        return pulumi.get(self, "image")
+
+    @image.setter
+    def image(self, value: Optional[pulumi.Input['ImageArgs']]):
+        pulumi.set(self, "image", value)
+
+    @property
+    @pulumi.getter
+    def repo(self) -> Optional[pulumi.Input[str]]:
         """
-        The notification setting for this service upon deployment failure.
+        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
         """
-        return pulumi.get(self, "notify_on_fail")
+        return pulumi.get(self, "repo")
 
-    @notify_on_fail.setter
-    def notify_on_fail(self, value: Optional[pulumi.Input['ServiceNotifyOnFail']]):
-        pulumi.set(self, "notify_on_fail", value)
+    @repo.setter
+    def repo(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "repo", value)
+
+    @property
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "root_dir")
+
+    @root_dir.setter
+    def root_dir(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "root_dir", value)
 
     @property
     @pulumi.getter(name="secretFiles")
     def secret_files(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]]:
         return pulumi.get(self, "secret_files")
 
     @secret_files.setter
     def secret_files(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecretFileArgs']]]]):
         pulumi.set(self, "secret_files", value)
 
     @property
     @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> Optional[pulumi.Input['WebServiceServiceDetailsArgs']]:
+    def service_details(self) -> Optional[pulumi.Input['CronJobDetailsCreateArgs']]:
         return pulumi.get(self, "service_details")
 
     @service_details.setter
-    def service_details(self, value: Optional[pulumi.Input['WebServiceServiceDetailsArgs']]):
+    def service_details(self, value: Optional[pulumi.Input['CronJobDetailsCreateArgs']]):
         pulumi.set(self, "service_details", value)
 
     @property
     @pulumi.getter
-    def slug(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "slug")
-
-    @slug.setter
-    def slug(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "slug", value)
-
-    @property
-    @pulumi.getter
-    def suspended(self) -> Optional[pulumi.Input['ServiceSuspended']]:
-        return pulumi.get(self, "suspended")
-
-    @suspended.setter
-    def suspended(self, value: Optional[pulumi.Input['ServiceSuspended']]):
-        pulumi.set(self, "suspended", value)
-
-    @property
-    @pulumi.getter
-    def suspenders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "suspenders")
-
-    @suspenders.setter
-    def suspenders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "suspenders", value)
-
-    @property
-    @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
-    @property
-    @pulumi.getter(name="updatedAt")
-    def updated_at(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "updated_at")
-
-    @updated_at.setter
-    def updated_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "updated_at", value)
 
-
-class WebService(pulumi.CustomResource):
+class CronJob(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvVarKeyValueArgs']]]]] = None,
+                 build_filter: Optional[pulumi.Input[pulumi.InputType['BuildFilterArgs']]] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union[pulumi.InputType['EnvVarKeyValueArgs'], pulumi.InputType['EnvVarKeyGenerateValueArgs']]]]]] = None,
+                 image: Optional[pulumi.Input[pulumi.InputType['ImageArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
                  owner_id: Optional[pulumi.Input[str]] = None,
                  repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretFileArgs']]]]] = None,
-                 service_details: Optional[pulumi.Input[pulumi.InputType['WebServiceServiceDetailsArgs']]] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 service_details: Optional[pulumi.Input[pulumi.InputType['CronJobDetailsCreateArgs']]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        A web service
-
+        Create a CronJob resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input['ServiceAutoDeploy'] auto_deploy: Whether to auto deploy the service or not upon git push.
-        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository.
-        :param pulumi.Input['ServiceNotifyOnFail'] notify_on_fail: The notification setting for this service upon deployment failure.
-        :param pulumi.Input[str] owner_id: The id of the owner (user/team).
+        :param pulumi.Input['ServiceCreateAutoDeploy'] auto_deploy: Defaults to "yes"
+        :param pulumi.Input[str] branch: If left empty, this will fall back to the default branch of the repository
         :param pulumi.Input[str] repo: Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: WebServiceArgs,
+                 args: CronJobArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        A web service
-
+        Create a CronJob resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param WebServiceArgs args: The arguments to use to populate this resource's properties.
+        :param CronJobArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(WebServiceArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(CronJobArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 auto_deploy: Optional[pulumi.Input['ServiceAutoDeploy']] = None,
+                 auto_deploy: Optional[pulumi.Input['ServiceCreateAutoDeploy']] = None,
                  branch: Optional[pulumi.Input[str]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvVarKeyValueArgs']]]]] = None,
+                 build_filter: Optional[pulumi.Input[pulumi.InputType['BuildFilterArgs']]] = None,
+                 env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[Union[pulumi.InputType['EnvVarKeyValueArgs'], pulumi.InputType['EnvVarKeyGenerateValueArgs']]]]]] = None,
+                 image: Optional[pulumi.Input[pulumi.InputType['ImageArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 notify_on_fail: Optional[pulumi.Input['ServiceNotifyOnFail']] = None,
                  owner_id: Optional[pulumi.Input[str]] = None,
                  repo: Optional[pulumi.Input[str]] = None,
+                 root_dir: Optional[pulumi.Input[str]] = None,
                  secret_files: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretFileArgs']]]]] = None,
-                 service_details: Optional[pulumi.Input[pulumi.InputType['WebServiceServiceDetailsArgs']]] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
-                 suspended: Optional[pulumi.Input['ServiceSuspended']] = None,
-                 suspenders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 service_details: Optional[pulumi.Input[pulumi.InputType['CronJobDetailsCreateArgs']]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 updated_at: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = WebServiceArgs.__new__(WebServiceArgs)
+            __props__ = CronJobArgs.__new__(CronJobArgs)
 
             if auto_deploy is None:
-                auto_deploy = 'no'
+                auto_deploy = 'yes'
             __props__.__dict__["auto_deploy"] = auto_deploy
             __props__.__dict__["branch"] = branch
-            __props__.__dict__["created_at"] = created_at
+            __props__.__dict__["build_filter"] = build_filter
             __props__.__dict__["env_vars"] = env_vars
+            __props__.__dict__["image"] = image
             if name is None and not opts.urn:
                 raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
-            __props__.__dict__["notify_on_fail"] = notify_on_fail
             if owner_id is None and not opts.urn:
                 raise TypeError("Missing required property 'owner_id'")
             __props__.__dict__["owner_id"] = owner_id
-            if repo is None and not opts.urn:
-                raise TypeError("Missing required property 'repo'")
             __props__.__dict__["repo"] = repo
+            __props__.__dict__["root_dir"] = root_dir
             __props__.__dict__["secret_files"] = secret_files
             __props__.__dict__["service_details"] = service_details
-            __props__.__dict__["slug"] = slug
-            __props__.__dict__["suspended"] = suspended
-            __props__.__dict__["suspenders"] = suspenders
             if type is None:
-                type = 'web_service'
+                type = 'cron_job'
             __props__.__dict__["type"] = type
-            __props__.__dict__["updated_at"] = updated_at
-        super(WebService, __self__).__init__(
-            'render:services:WebService',
+            __props__.__dict__["created_at"] = None
+            __props__.__dict__["image_path"] = None
+            __props__.__dict__["notify_on_fail"] = None
+            __props__.__dict__["slug"] = None
+            __props__.__dict__["suspended"] = None
+            __props__.__dict__["suspenders"] = None
+            __props__.__dict__["updated_at"] = None
+        super(CronJob, __self__).__init__(
+            'render:services:CronJob',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'WebService':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'CronJob':
         """
-        Get an existing WebService resource's state with the given name, id, and optional extra
+        Get an existing CronJob resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = WebServiceArgs.__new__(WebServiceArgs)
+        __props__ = CronJobArgs.__new__(CronJobArgs)
 
         __props__.__dict__["auto_deploy"] = None
         __props__.__dict__["branch"] = None
+        __props__.__dict__["build_filter"] = None
         __props__.__dict__["created_at"] = None
         __props__.__dict__["env_vars"] = None
+        __props__.__dict__["image"] = None
+        __props__.__dict__["image_path"] = None
         __props__.__dict__["name"] = None
         __props__.__dict__["notify_on_fail"] = None
         __props__.__dict__["owner_id"] = None
         __props__.__dict__["repo"] = None
+        __props__.__dict__["root_dir"] = None
         __props__.__dict__["secret_files"] = None
         __props__.__dict__["service_details"] = None
         __props__.__dict__["slug"] = None
         __props__.__dict__["suspended"] = None
         __props__.__dict__["suspenders"] = None
         __props__.__dict__["type"] = None
         __props__.__dict__["updated_at"] = None
-        return WebService(resource_name, opts=opts, __props__=__props__)
+        return CronJob(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="autoDeploy")
     def auto_deploy(self) -> pulumi.Output[Optional['ServiceAutoDeploy']]:
-        """
-        Whether to auto deploy the service or not upon git push.
-        """
         return pulumi.get(self, "auto_deploy")
 
     @property
     @pulumi.getter
     def branch(self) -> pulumi.Output[Optional[str]]:
-        """
-        If left empty, this will fall back to the default branch of the repository.
-        """
         return pulumi.get(self, "branch")
 
     @property
+    @pulumi.getter(name="buildFilter")
+    def build_filter(self) -> pulumi.Output[Optional['outputs.BuildFilter']]:
+        return pulumi.get(self, "build_filter")
+
+    @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter(name="envVars")
-    def env_vars(self) -> pulumi.Output[Optional[Sequence['outputs.EnvVarKeyValue']]]:
+    def env_vars(self) -> pulumi.Output[Optional[Sequence[Any]]]:
         return pulumi.get(self, "env_vars")
 
     @property
     @pulumi.getter
+    def image(self) -> pulumi.Output[Optional['outputs.Image']]:
+        return pulumi.get(self, "image")
+
+    @property
+    @pulumi.getter(name="imagePath")
+    def image_path(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "image_path")
+
+    @property
+    @pulumi.getter
     def name(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="notifyOnFail")
     def notify_on_fail(self) -> pulumi.Output[Optional['ServiceNotifyOnFail']]:
-        """
-        The notification setting for this service upon deployment failure.
-        """
         return pulumi.get(self, "notify_on_fail")
 
     @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> pulumi.Output[Optional[str]]:
-        """
-        The id of the owner (user/team).
-        """
         return pulumi.get(self, "owner_id")
 
     @property
     @pulumi.getter
     def repo(self) -> pulumi.Output[Optional[str]]:
-        """
-        Do not include the branch in the repo string. You can instead supply a 'branch' parameter.
-        """
         return pulumi.get(self, "repo")
 
     @property
+    @pulumi.getter(name="rootDir")
+    def root_dir(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "root_dir")
+
+    @property
     @pulumi.getter(name="secretFiles")
     def secret_files(self) -> pulumi.Output[Optional[Sequence['outputs.SecretFile']]]:
         return pulumi.get(self, "secret_files")
 
     @property
     @pulumi.getter(name="serviceDetails")
-    def service_details(self) -> pulumi.Output[Optional['outputs.WebServiceServiceDetails']]:
+    def service_details(self) -> pulumi.Output[Optional['outputs.CronJobDetailsOutput']]:
         return pulumi.get(self, "service_details")
 
     @property
     @pulumi.getter
     def slug(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "slug")
 
     @property
     @pulumi.getter
     def suspended(self) -> pulumi.Output[Optional['ServiceSuspended']]:
         return pulumi.get(self, "suspended")
 
     @property
     @pulumi.getter
-    def suspenders(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    def suspenders(self) -> pulumi.Output[Optional[Sequence['ServiceSuspendersItem']]]:
         return pulumi.get(self, "suspenders")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "type")
```

### Comparing `pulumi_render-0.1.1/pulumi_render.egg-info/PKG-INFO` & `pulumi_render-0.2.0/pulumi_render.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_render
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Pulumi package for creating and managing Render resources.
 License: Apache-2.0
 Project-URL: Homepage, https://cloudysky.software
 Project-URL: Repository, https://github.com/cloudy-sky-software/pulumi-render
 Keywords: pulumi,render,category/cloud,kind/native
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_render-0.1.1/pulumi_render.egg-info/SOURCES.txt` & `pulumi_render-0.2.0/pulumi_render.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,42 +15,49 @@
 pulumi_render/config/vars.py
 pulumi_render/owners/__init__.py
 pulumi_render/owners/_enums.py
 pulumi_render/owners/get_owner.py
 pulumi_render/owners/list_owners.py
 pulumi_render/owners/outputs.py
 pulumi_render/registrycredentials/__init__.py
+pulumi_render/registrycredentials/_enums.py
 pulumi_render/registrycredentials/get_registry_credential.py
 pulumi_render/registrycredentials/list_registry_credentials.py
 pulumi_render/registrycredentials/outputs.py
 pulumi_render/registrycredentials/registry_credential.py
 pulumi_render/services/__init__.py
 pulumi_render/services/_enums.py
 pulumi_render/services/_inputs.py
-pulumi_render/services/auto_scaling.py
+pulumi_render/services/autoscale_service.py
 pulumi_render/services/background_worker.py
+pulumi_render/services/cancel_deploy.py
+pulumi_render/services/cancel_job.py
 pulumi_render/services/cron_job.py
-pulumi_render/services/custom_domains.py
-pulumi_render/services/deploys.py
-pulumi_render/services/env_vars.py
+pulumi_render/services/custom_domain.py
+pulumi_render/services/deploy.py
+pulumi_render/services/env_vars_for_service.py
 pulumi_render/services/get_background_worker.py
 pulumi_render/services/get_cron_job.py
 pulumi_render/services/get_custom_domain.py
 pulumi_render/services/get_deploy.py
 pulumi_render/services/get_job.py
 pulumi_render/services/get_private_service.py
 pulumi_render/services/get_static_site.py
 pulumi_render/services/get_web_service.py
-pulumi_render/services/jobs.py
+pulumi_render/services/job.py
 pulumi_render/services/list_custom_domains.py
 pulumi_render/services/list_deploys.py
-pulumi_render/services/list_env_vars.py
-pulumi_render/services/list_headers.py
-pulumi_render/services/list_jobs.py
-pulumi_render/services/list_routes.py
+pulumi_render/services/list_env_vars_for_service.py
+pulumi_render/services/list_job.py
+pulumi_render/services/list_retrieve_headers.py
+pulumi_render/services/list_retrieve_routes.py
 pulumi_render/services/list_services.py
 pulumi_render/services/outputs.py
+pulumi_render/services/preview_service.py
 pulumi_render/services/private_service.py
-pulumi_render/services/scale.py
+pulumi_render/services/refresh_custom_domain.py
+pulumi_render/services/restart_server.py
+pulumi_render/services/rollback_deploy.py
+pulumi_render/services/scale_service.py
 pulumi_render/services/static_site.py
-pulumi_render/services/suspend.py
+pulumi_render/services/suspend_service.py
 pulumi_render/services/web_service.py
```

### Comparing `pulumi_render-0.1.1/pyproject.toml` & `pulumi_render-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_render"
   description = "A Pulumi package for creating and managing Render resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "render", "category/cloud", "kind/native"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.1.1"
+  version = "0.2.0"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://cloudysky.software"
     Repository = "https://github.com/cloudy-sky-software/pulumi-render"
 
 [build-system]
```

