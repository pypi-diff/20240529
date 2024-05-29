# Comparing `tmp/cdktf-cdktf-provider-launchdarkly-4.1.3.tar.gz` & `tmp/cdktf-cdktf-provider-launchdarkly-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-launchdarkly-4.1.3.tar", last modified: Fri May 17 03:42:09 2024, max compression
+gzip compressed data, was "cdktf-cdktf-provider-launchdarkly-4.1.4.tar", last modified: Wed May 29 03:41:44 2024, max compression
```

## Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3.tar` & `cdktf-cdktf-provider-launchdarkly-4.1.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-05-17 03:41:55.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.899542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.903542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   448270 2024-05-17 03:41:55.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/_jsii/provider-launchdarkly@4.1.3.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/access_token/
--rw-r--r--   0 runner    (1001) docker     (127)    88303 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/access_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/audit_log_subscription/
--rw-r--r--   0 runner    (1001) docker     (127)    59429 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/audit_log_subscription/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/custom_role/
--rw-r--r--   0 runner    (1001) docker     (127)    72794 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/custom_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_audit_log_subscription/
--rw-r--r--   0 runner    (1001) docker     (127)    32783 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_audit_log_subscription/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_environment/
--rw-r--r--   0 runner    (1001) docker     (127)    38854 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag/
--rw-r--r--   0 runner    (1001) docker     (127)    69707 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag_environment/
--rw-r--r--   0 runner    (1001) docker     (127)    84010 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag_environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_flag_trigger/
--rw-r--r--   0 runner    (1001) docker     (127)    40739 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_flag_trigger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_metric/
--rw-r--r--   0 runner    (1001) docker     (127)    74608 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_project/
--rw-r--r--   0 runner    (1001) docker     (127)    40324 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_relay_proxy_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)    29401 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_relay_proxy_configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_segment/
--rw-r--r--   0 runner    (1001) docker     (127)    65041 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_segment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team/
--rw-r--r--   0 runner    (1001) docker     (127)    38022 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_member/
--rw-r--r--   0 runner    (1001) docker     (127)    21195 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_members/
--rw-r--r--   0 runner    (1001) docker     (127)    34055 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_members/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_webhook/
--rw-r--r--   0 runner    (1001) docker     (127)    33699 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_webhook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/destination/
--rw-r--r--   0 runner    (1001) docker     (127)    36010 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/destination/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/environment/
--rw-r--r--   0 runner    (1001) docker     (127)    86011 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/feature_flag/
--rw-r--r--   0 runner    (1001) docker     (127)   121531 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/feature_flag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/feature_flag_environment/
--rw-r--r--   0 runner    (1001) docker     (127)   159503 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/feature_flag_environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/flag_trigger/
--rw-r--r--   0 runner    (1001) docker     (127)    38676 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/flag_trigger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/metric/
--rw-r--r--   0 runner    (1001) docker     (127)    74544 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/project/
--rw-r--r--   0 runner    (1001) docker     (127)   121571 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/provider/
--rw-r--r--   0 runner    (1001) docker     (127)    20356 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/relay_proxy_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)    47019 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/relay_proxy_configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/segment/
--rw-r--r--   0 runner    (1001) docker     (127)   128901 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/segment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/team/
--rw-r--r--   0 runner    (1001) docker     (127)    32524 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/team/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/team_member/
--rw-r--r--   0 runner    (1001) docker     (127)    30569 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/team_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/team_role_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)    20256 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/team_role_mapping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.911542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/webhook/
--rw-r--r--   0 runner    (1001) docker     (127)    55575 2024-05-17 03:41:56.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/webhook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:42:09.907542 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-17 03:42:09.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-17 03:42:09.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:42:09.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-17 03:42:09.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-17 03:42:09.000000 cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.227773 cdktf-cdktf-provider-launchdarkly-4.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-29 03:41:44.227773 cdktf-cdktf-provider-launchdarkly-4.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 03:41:44.227773 cdktf-cdktf-provider-launchdarkly-4.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.215773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.219773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.219773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   448298 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/_jsii/provider-launchdarkly@4.1.4.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.219773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/access_token/
+-rw-r--r--   0 runner    (1001) docker     (127)    88303 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/access_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.219773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/audit_log_subscription/
+-rw-r--r--   0 runner    (1001) docker     (127)    59429 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/audit_log_subscription/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/custom_role/
+-rw-r--r--   0 runner    (1001) docker     (127)    72794 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/custom_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_audit_log_subscription/
+-rw-r--r--   0 runner    (1001) docker     (127)    32783 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_audit_log_subscription/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_environment/
+-rw-r--r--   0 runner    (1001) docker     (127)    38854 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag/
+-rw-r--r--   0 runner    (1001) docker     (127)    69707 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag_environment/
+-rw-r--r--   0 runner    (1001) docker     (127)    84010 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag_environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_flag_trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)    40739 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_flag_trigger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_metric/
+-rw-r--r--   0 runner    (1001) docker     (127)    74608 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_project/
+-rw-r--r--   0 runner    (1001) docker     (127)    40324 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_relay_proxy_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)    29401 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_relay_proxy_configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_segment/
+-rw-r--r--   0 runner    (1001) docker     (127)    65041 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_segment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team/
+-rw-r--r--   0 runner    (1001) docker     (127)    38022 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_member/
+-rw-r--r--   0 runner    (1001) docker     (127)    21195 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_members/
+-rw-r--r--   0 runner    (1001) docker     (127)    34055 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_members/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_webhook/
+-rw-r--r--   0 runner    (1001) docker     (127)    33699 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_webhook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/destination/
+-rw-r--r--   0 runner    (1001) docker     (127)    36010 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/destination/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)    86011 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/feature_flag/
+-rw-r--r--   0 runner    (1001) docker     (127)   121531 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/feature_flag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/feature_flag_environment/
+-rw-r--r--   0 runner    (1001) docker     (127)   159503 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/feature_flag_environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.223773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/flag_trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)    38676 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/flag_trigger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.227773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)    74544 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.227773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/project/
+-rw-r--r--   0 runner    (1001) docker     (127)   121571 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.227773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)    20356 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.227773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/relay_proxy_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)    47019 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/relay_proxy_configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.227773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)   128901 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/segment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.227773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/team/
+-rw-r--r--   0 runner    (1001) docker     (127)    32524 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/team/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.227773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/team_member/
+-rw-r--r--   0 runner    (1001) docker     (127)    30569 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/team_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.227773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/team_role_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)    20256 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/team_role_mapping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.227773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/webhook/
+-rw-r--r--   0 runner    (1001) docker     (127)    55575 2024-05-29 03:41:33.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/webhook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:41:44.219773 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-29 03:41:44.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-29 03:41:44.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:41:44.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-29 03:41:44.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-29 03:41:44.000000 cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/LICENSE` & `cdktf-cdktf-provider-launchdarkly-4.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/PKG-INFO` & `cdktf-cdktf-provider-launchdarkly-4.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-launchdarkly
-Version: 4.1.3
+Version: 4.1.4
 Summary: Prebuilt launchdarkly Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-launchdarkly.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-launchdarkly.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -17,17 +17,17 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CDKTF prebuilt bindings for launchdarkly/launchdarkly provider version 2.18.3
+# CDKTF prebuilt bindings for launchdarkly/launchdarkly provider version 2.18.4
 
-This repo builds and publishes the [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-launchdarkly](https://www.npmjs.com/package/@cdktf/provider-launchdarkly).
 
@@ -81,15 +81,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform launchdarkly provider version 1:1. In fact, it always tracks `latest` of `~> 2.13` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3)
+* [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/README.md` & `cdktf-cdktf-provider-launchdarkly-4.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# CDKTF prebuilt bindings for launchdarkly/launchdarkly provider version 2.18.3
+# CDKTF prebuilt bindings for launchdarkly/launchdarkly provider version 2.18.4
 
-This repo builds and publishes the [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-launchdarkly](https://www.npmjs.com/package/@cdktf/provider-launchdarkly).
 
@@ -58,15 +58,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform launchdarkly provider version 1:1. In fact, it always tracks `latest` of `~> 2.13` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3)
+* [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/setup.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-launchdarkly",
-    "version": "4.1.3",
+    "version": "4.1.4",
     "description": "Prebuilt launchdarkly Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-launchdarkly.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -52,15 +52,15 @@
         "cdktf_cdktf_provider_launchdarkly.team",
         "cdktf_cdktf_provider_launchdarkly.team_member",
         "cdktf_cdktf_provider_launchdarkly.team_role_mapping",
         "cdktf_cdktf_provider_launchdarkly.webhook"
     ],
     "package_data": {
         "cdktf_cdktf_provider_launchdarkly._jsii": [
-            "provider-launchdarkly@4.1.3.jsii.tgz"
+            "provider-launchdarkly@4.1.4.jsii.tgz"
         ],
         "cdktf_cdktf_provider_launchdarkly": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# CDKTF prebuilt bindings for launchdarkly/launchdarkly provider version 2.18.3
+# CDKTF prebuilt bindings for launchdarkly/launchdarkly provider version 2.18.4
 
-This repo builds and publishes the [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-launchdarkly](https://www.npmjs.com/package/@cdktf/provider-launchdarkly).
 
@@ -59,15 +59,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform launchdarkly provider version 1:1. In fact, it always tracks `latest` of `~> 2.13` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3)
+* [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/access_token/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/access_token/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_access_token`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_access_token`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token).
+Refer to the Terraform Registry for docs: [`launchdarkly_access_token`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class AccessToken(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.accessToken.AccessToken",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token launchdarkly_access_token}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token launchdarkly_access_token}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         custom_roles: typing.Optional[typing.Sequence[builtins.str]] = None,
@@ -49,27 +49,27 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token launchdarkly_access_token} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token launchdarkly_access_token} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param custom_roles: A list of custom role IDs to use as access limits for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#custom_roles AccessToken#custom_roles}
-        :param default_api_version: The default API version for this token. Defaults to the latest API version. A change in this field will force the destruction of the existing token in state and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#default_api_version AccessToken#default_api_version}
-        :param expire: An expiration time for the current token secret, expressed as a Unix epoch time. Replace the computed token secret with a new value. The expired secret will no longer be able to authorize usage of the LaunchDarkly API. This field argument is **deprecated**. Please update your config to remove ``expire`` to maintain compatibility with future versions Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#expire AccessToken#expire}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#id AccessToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param inline_roles: inline_roles block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#inline_roles AccessToken#inline_roles}
-        :param name: A human-friendly name for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#name AccessToken#name}
-        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#policy_statements AccessToken#policy_statements}
-        :param role: A built-in LaunchDarkly role. Can be ``reader``, ``writer``, or ``admin``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#role AccessToken#role}
-        :param service_token: Whether the token will be a `service token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#service-tokens>`_. A change in this field will force the destruction of the existing token and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#service_token AccessToken#service_token}
+        :param custom_roles: A list of custom role IDs to use as access limits for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#custom_roles AccessToken#custom_roles}
+        :param default_api_version: The default API version for this token. Defaults to the latest API version. A change in this field will force the destruction of the existing token in state and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#default_api_version AccessToken#default_api_version}
+        :param expire: An expiration time for the current token secret, expressed as a Unix epoch time. Replace the computed token secret with a new value. The expired secret will no longer be able to authorize usage of the LaunchDarkly API. This field argument is **deprecated**. Please update your config to remove ``expire`` to maintain compatibility with future versions Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#expire AccessToken#expire}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#id AccessToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param inline_roles: inline_roles block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#inline_roles AccessToken#inline_roles}
+        :param name: A human-friendly name for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#name AccessToken#name}
+        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#policy_statements AccessToken#policy_statements}
+        :param role: A built-in LaunchDarkly role. Can be ``reader``, ``writer``, or ``admin``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#role AccessToken#role}
+        :param service_token: Whether the token will be a `service token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#service-tokens>`_. A change in this field will force the destruction of the existing token and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#service_token AccessToken#service_token}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -108,15 +108,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a AccessToken resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the AccessToken to import.
-        :param import_from_id: The id of the existing AccessToken that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing AccessToken that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the AccessToken to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ff521033794a17762ec24876587ce0a56fb17a09b59cfe53ad9f3f40bbb6cb20)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -399,23 +399,23 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param custom_roles: A list of custom role IDs to use as access limits for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#custom_roles AccessToken#custom_roles}
-        :param default_api_version: The default API version for this token. Defaults to the latest API version. A change in this field will force the destruction of the existing token in state and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#default_api_version AccessToken#default_api_version}
-        :param expire: An expiration time for the current token secret, expressed as a Unix epoch time. Replace the computed token secret with a new value. The expired secret will no longer be able to authorize usage of the LaunchDarkly API. This field argument is **deprecated**. Please update your config to remove ``expire`` to maintain compatibility with future versions Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#expire AccessToken#expire}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#id AccessToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param inline_roles: inline_roles block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#inline_roles AccessToken#inline_roles}
-        :param name: A human-friendly name for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#name AccessToken#name}
-        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#policy_statements AccessToken#policy_statements}
-        :param role: A built-in LaunchDarkly role. Can be ``reader``, ``writer``, or ``admin``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#role AccessToken#role}
-        :param service_token: Whether the token will be a `service token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#service-tokens>`_. A change in this field will force the destruction of the existing token and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#service_token AccessToken#service_token}
+        :param custom_roles: A list of custom role IDs to use as access limits for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#custom_roles AccessToken#custom_roles}
+        :param default_api_version: The default API version for this token. Defaults to the latest API version. A change in this field will force the destruction of the existing token in state and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#default_api_version AccessToken#default_api_version}
+        :param expire: An expiration time for the current token secret, expressed as a Unix epoch time. Replace the computed token secret with a new value. The expired secret will no longer be able to authorize usage of the LaunchDarkly API. This field argument is **deprecated**. Please update your config to remove ``expire`` to maintain compatibility with future versions Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#expire AccessToken#expire}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#id AccessToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param inline_roles: inline_roles block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#inline_roles AccessToken#inline_roles}
+        :param name: A human-friendly name for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#name AccessToken#name}
+        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#policy_statements AccessToken#policy_statements}
+        :param role: A built-in LaunchDarkly role. Can be ``reader``, ``writer``, or ``admin``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#role AccessToken#role}
+        :param service_token: Whether the token will be a `service token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#service-tokens>`_. A change in this field will force the destruction of the existing token and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#service_token AccessToken#service_token}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2057e14f74a5d72eae1bfd306b184f12411fbbd7712def89d264547c92f1ea09)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -531,98 +531,98 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def custom_roles(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of custom role IDs to use as access limits for the access token.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#custom_roles AccessToken#custom_roles}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#custom_roles AccessToken#custom_roles}
         '''
         result = self._values.get("custom_roles")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def default_api_version(self) -> typing.Optional[jsii.Number]:
         '''The default API version for this token.
 
         Defaults to the latest API version. A change in this field will force the destruction of the existing token in state and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#default_api_version AccessToken#default_api_version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#default_api_version AccessToken#default_api_version}
         '''
         result = self._values.get("default_api_version")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def expire(self) -> typing.Optional[jsii.Number]:
         '''An expiration time for the current token secret, expressed as a Unix epoch time.
 
         Replace the computed token secret with a new value. The expired secret will no longer be able to authorize usage of the LaunchDarkly API. This field argument is **deprecated**. Please update your config to remove ``expire`` to maintain compatibility with future versions
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#expire AccessToken#expire}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#expire AccessToken#expire}
         '''
         result = self._values.get("expire")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#id AccessToken#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#id AccessToken#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def inline_roles(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AccessTokenInlineRoles"]]]:
         '''inline_roles block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#inline_roles AccessToken#inline_roles}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#inline_roles AccessToken#inline_roles}
         '''
         result = self._values.get("inline_roles")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AccessTokenInlineRoles"]]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''A human-friendly name for the access token.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#name AccessToken#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#name AccessToken#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def policy_statements(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AccessTokenPolicyStatements"]]]:
         '''policy_statements block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#policy_statements AccessToken#policy_statements}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#policy_statements AccessToken#policy_statements}
         '''
         result = self._values.get("policy_statements")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AccessTokenPolicyStatements"]]], result)
 
     @builtins.property
     def role(self) -> typing.Optional[builtins.str]:
         '''A built-in LaunchDarkly role. Can be ``reader``, ``writer``, or ``admin``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#role AccessToken#role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#role AccessToken#role}
         '''
         result = self._values.get("role")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def service_token(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the token will be a `service token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#service-tokens>`_. A change in this field will force the destruction of the existing token and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#service_token AccessToken#service_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#service_token AccessToken#service_token}
         '''
         result = self._values.get("service_token")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -653,19 +653,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Either ``allow`` or ``deny``. This argument defines whether the statement allows or denies access to the named resources and actions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#effect AccessToken#effect}
-        :param actions: The list of action specifiers defining the actions to which the statement applies. Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#actions AccessToken#actions}
-        :param not_actions: The list of action specifiers defining the actions to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#not_actions AccessToken#not_actions}
-        :param not_resources: The list of resource specifiers defining the resources to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#not_resources AccessToken#not_resources}
-        :param resources: The list of resource specifiers defining the resources to which the statement applies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#resources AccessToken#resources}
+        :param effect: Either ``allow`` or ``deny``. This argument defines whether the statement allows or denies access to the named resources and actions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#effect AccessToken#effect}
+        :param actions: The list of action specifiers defining the actions to which the statement applies. Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#actions AccessToken#actions}
+        :param not_actions: The list of action specifiers defining the actions to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#not_actions AccessToken#not_actions}
+        :param not_resources: The list of resource specifiers defining the resources to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#not_resources AccessToken#not_resources}
+        :param resources: The list of resource specifiers defining the resources to which the statement applies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#resources AccessToken#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6bf777dc854b3453cf4763366a000825853d9755645cbb159247ac5859373423)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -684,54 +684,54 @@
 
     @builtins.property
     def effect(self) -> builtins.str:
         '''Either ``allow`` or ``deny``.
 
         This argument defines whether the statement allows or denies access to the named resources and actions.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#effect AccessToken#effect}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#effect AccessToken#effect}
         '''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of action specifiers defining the actions to which the statement applies.
 
         Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#actions AccessToken#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#actions AccessToken#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of action specifiers defining the actions to which the statement does not apply.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#not_actions AccessToken#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#not_actions AccessToken#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of resource specifiers defining the resources to which the statement does not apply.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#not_resources AccessToken#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#not_resources AccessToken#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of resource specifiers defining the resources to which the statement applies.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#resources AccessToken#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#resources AccessToken#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -997,19 +997,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Either ``allow`` or ``deny``. This argument defines whether the statement allows or denies access to the named resources and actions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#effect AccessToken#effect}
-        :param actions: The list of action specifiers defining the actions to which the statement applies. Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#actions AccessToken#actions}
-        :param not_actions: The list of action specifiers defining the actions to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#not_actions AccessToken#not_actions}
-        :param not_resources: The list of resource specifiers defining the resources to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#not_resources AccessToken#not_resources}
-        :param resources: The list of resource specifiers defining the resources to which the statement applies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#resources AccessToken#resources}
+        :param effect: Either ``allow`` or ``deny``. This argument defines whether the statement allows or denies access to the named resources and actions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#effect AccessToken#effect}
+        :param actions: The list of action specifiers defining the actions to which the statement applies. Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#actions AccessToken#actions}
+        :param not_actions: The list of action specifiers defining the actions to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#not_actions AccessToken#not_actions}
+        :param not_resources: The list of resource specifiers defining the resources to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#not_resources AccessToken#not_resources}
+        :param resources: The list of resource specifiers defining the resources to which the statement applies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#resources AccessToken#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__69536178ec1dc81c007afab784c9a2f1c87f74bac4ab24e4995657c04b64bc4a)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -1028,54 +1028,54 @@
 
     @builtins.property
     def effect(self) -> builtins.str:
         '''Either ``allow`` or ``deny``.
 
         This argument defines whether the statement allows or denies access to the named resources and actions.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#effect AccessToken#effect}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#effect AccessToken#effect}
         '''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of action specifiers defining the actions to which the statement applies.
 
         Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#actions AccessToken#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#actions AccessToken#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of action specifiers defining the actions to which the statement does not apply.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#not_actions AccessToken#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#not_actions AccessToken#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of resource specifiers defining the resources to which the statement does not apply.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#not_resources AccessToken#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#not_resources AccessToken#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of resource specifiers defining the resources to which the statement applies.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/access_token#resources AccessToken#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/access_token#resources AccessToken#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/audit_log_subscription/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/audit_log_subscription/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_audit_log_subscription`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_audit_log_subscription`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription).
+Refer to the Terraform Registry for docs: [`launchdarkly_audit_log_subscription`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class AuditLogSubscription(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.auditLogSubscription.AuditLogSubscription",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription launchdarkly_audit_log_subscription}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription launchdarkly_audit_log_subscription}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         config: typing.Mapping[builtins.str, builtins.str],
@@ -47,25 +47,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription launchdarkly_audit_log_subscription} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription launchdarkly_audit_log_subscription} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param config: The set of configuration fields corresponding to the value defined for ``integration_key``. Refer to the ``formVariables`` field in the corresponding ``integrations/<integration_key>/manifest.json`` file in `this repo <https://github.com/launchdarkly/integration-framework/tree/master/integrations>`_ for a full list of fields for the integration you wish to configure. **IMPORTANT**: Please note that Terraform will only accept these in snake case, regardless of the case shown in the manifest. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#config AuditLogSubscription#config}
-        :param integration_key: The integration key. Supported integration keys are ``chronosphere``, ``cloudtrail``, ``datadog``, ``dynatrace``, ``elastic``, ``grafana``, ``honeycomb``, ``logdna``, ``msteams``, ``new-relic-apm``, ``signalfx``, ``slack``, and ``splunk``. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#integration_key AuditLogSubscription#integration_key}
-        :param name: A human-friendly name for your audit log subscription viewable from within the LaunchDarkly Integrations page. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#name AuditLogSubscription#name}
-        :param on: Whether or not you want your subscription enabled, i.e. to actively send events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#on AuditLogSubscription#on}
-        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#statements AuditLogSubscription#statements}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#id AuditLogSubscription#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#tags AuditLogSubscription#tags}
+        :param config: The set of configuration fields corresponding to the value defined for ``integration_key``. Refer to the ``formVariables`` field in the corresponding ``integrations/<integration_key>/manifest.json`` file in `this repo <https://github.com/launchdarkly/integration-framework/tree/master/integrations>`_ for a full list of fields for the integration you wish to configure. **IMPORTANT**: Please note that Terraform will only accept these in snake case, regardless of the case shown in the manifest. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#config AuditLogSubscription#config}
+        :param integration_key: The integration key. Supported integration keys are ``chronosphere``, ``cloudtrail``, ``datadog``, ``dynatrace``, ``elastic``, ``grafana``, ``honeycomb``, ``logdna``, ``msteams``, ``new-relic-apm``, ``signalfx``, ``slack``, and ``splunk``. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#integration_key AuditLogSubscription#integration_key}
+        :param name: A human-friendly name for your audit log subscription viewable from within the LaunchDarkly Integrations page. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#name AuditLogSubscription#name}
+        :param on: Whether or not you want your subscription enabled, i.e. to actively send events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#on AuditLogSubscription#on}
+        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#statements AuditLogSubscription#statements}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#id AuditLogSubscription#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#tags AuditLogSubscription#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -102,15 +102,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a AuditLogSubscription resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the AuditLogSubscription to import.
-        :param import_from_id: The id of the existing AuditLogSubscription that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing AuditLogSubscription that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the AuditLogSubscription to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__13e2178d972de561c6e0e19d7a939e5e9ec8becbe13a692471ade66625a0cdd0)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -316,21 +316,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param config: The set of configuration fields corresponding to the value defined for ``integration_key``. Refer to the ``formVariables`` field in the corresponding ``integrations/<integration_key>/manifest.json`` file in `this repo <https://github.com/launchdarkly/integration-framework/tree/master/integrations>`_ for a full list of fields for the integration you wish to configure. **IMPORTANT**: Please note that Terraform will only accept these in snake case, regardless of the case shown in the manifest. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#config AuditLogSubscription#config}
-        :param integration_key: The integration key. Supported integration keys are ``chronosphere``, ``cloudtrail``, ``datadog``, ``dynatrace``, ``elastic``, ``grafana``, ``honeycomb``, ``logdna``, ``msteams``, ``new-relic-apm``, ``signalfx``, ``slack``, and ``splunk``. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#integration_key AuditLogSubscription#integration_key}
-        :param name: A human-friendly name for your audit log subscription viewable from within the LaunchDarkly Integrations page. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#name AuditLogSubscription#name}
-        :param on: Whether or not you want your subscription enabled, i.e. to actively send events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#on AuditLogSubscription#on}
-        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#statements AuditLogSubscription#statements}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#id AuditLogSubscription#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#tags AuditLogSubscription#tags}
+        :param config: The set of configuration fields corresponding to the value defined for ``integration_key``. Refer to the ``formVariables`` field in the corresponding ``integrations/<integration_key>/manifest.json`` file in `this repo <https://github.com/launchdarkly/integration-framework/tree/master/integrations>`_ for a full list of fields for the integration you wish to configure. **IMPORTANT**: Please note that Terraform will only accept these in snake case, regardless of the case shown in the manifest. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#config AuditLogSubscription#config}
+        :param integration_key: The integration key. Supported integration keys are ``chronosphere``, ``cloudtrail``, ``datadog``, ``dynatrace``, ``elastic``, ``grafana``, ``honeycomb``, ``logdna``, ``msteams``, ``new-relic-apm``, ``signalfx``, ``slack``, and ``splunk``. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#integration_key AuditLogSubscription#integration_key}
+        :param name: A human-friendly name for your audit log subscription viewable from within the LaunchDarkly Integrations page. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#name AuditLogSubscription#name}
+        :param on: Whether or not you want your subscription enabled, i.e. to actively send events. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#on AuditLogSubscription#on}
+        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#statements AuditLogSubscription#statements}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#id AuditLogSubscription#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#tags AuditLogSubscription#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ef1e41a2cdac9756b56ce790ba595e5e76b13fcfd9f0a7f2d71efe562ae45ed6)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -438,79 +438,79 @@
 
     @builtins.property
     def config(self) -> typing.Mapping[builtins.str, builtins.str]:
         '''The set of configuration fields corresponding to the value defined for ``integration_key``.
 
         Refer to the ``formVariables`` field in the corresponding ``integrations/<integration_key>/manifest.json`` file in `this repo <https://github.com/launchdarkly/integration-framework/tree/master/integrations>`_ for a full list of fields for the integration you wish to configure. **IMPORTANT**: Please note that Terraform will only accept these in snake case, regardless of the case shown in the manifest.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#config AuditLogSubscription#config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#config AuditLogSubscription#config}
         '''
         result = self._values.get("config")
         assert result is not None, "Required property 'config' is missing"
         return typing.cast(typing.Mapping[builtins.str, builtins.str], result)
 
     @builtins.property
     def integration_key(self) -> builtins.str:
         '''The integration key.
 
         Supported integration keys are ``chronosphere``, ``cloudtrail``, ``datadog``, ``dynatrace``, ``elastic``, ``grafana``, ``honeycomb``, ``logdna``, ``msteams``, ``new-relic-apm``, ``signalfx``, ``slack``, and ``splunk``. A change in this field will force the destruction of the existing resource and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#integration_key AuditLogSubscription#integration_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#integration_key AuditLogSubscription#integration_key}
         '''
         result = self._values.get("integration_key")
         assert result is not None, "Required property 'integration_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''A human-friendly name for your audit log subscription viewable from within the LaunchDarkly Integrations page.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#name AuditLogSubscription#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#name AuditLogSubscription#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def on(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
         '''Whether or not you want your subscription enabled, i.e. to actively send events.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#on AuditLogSubscription#on}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#on AuditLogSubscription#on}
         '''
         result = self._values.get("on")
         assert result is not None, "Required property 'on' is missing"
         return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], result)
 
     @builtins.property
     def statements(
         self,
     ) -> typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AuditLogSubscriptionStatements"]]:
         '''statements block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#statements AuditLogSubscription#statements}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#statements AuditLogSubscription#statements}
         '''
         result = self._values.get("statements")
         assert result is not None, "Required property 'statements' is missing"
         return typing.cast(typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AuditLogSubscriptionStatements"]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#id AuditLogSubscription#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#id AuditLogSubscription#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#tags AuditLogSubscription#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#tags AuditLogSubscription#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -541,19 +541,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Either ``allow`` or ``deny``. This argument defines whether the statement allows or denies access to the named resources and actions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#effect AuditLogSubscription#effect}
-        :param actions: The list of action specifiers defining the actions to which the statement applies. Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#actions AuditLogSubscription#actions}
-        :param not_actions: The list of action specifiers defining the actions to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#not_actions AuditLogSubscription#not_actions}
-        :param not_resources: The list of resource specifiers defining the resources to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#not_resources AuditLogSubscription#not_resources}
-        :param resources: The list of resource specifiers defining the resources to which the statement applies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#resources AuditLogSubscription#resources}
+        :param effect: Either ``allow`` or ``deny``. This argument defines whether the statement allows or denies access to the named resources and actions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#effect AuditLogSubscription#effect}
+        :param actions: The list of action specifiers defining the actions to which the statement applies. Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#actions AuditLogSubscription#actions}
+        :param not_actions: The list of action specifiers defining the actions to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#not_actions AuditLogSubscription#not_actions}
+        :param not_resources: The list of resource specifiers defining the resources to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#not_resources AuditLogSubscription#not_resources}
+        :param resources: The list of resource specifiers defining the resources to which the statement applies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#resources AuditLogSubscription#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7eafab4833c3c1fd2c0d9c87f5e7f4b213057774377a08fc698b07c04d741b68)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -572,54 +572,54 @@
 
     @builtins.property
     def effect(self) -> builtins.str:
         '''Either ``allow`` or ``deny``.
 
         This argument defines whether the statement allows or denies access to the named resources and actions.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#effect AuditLogSubscription#effect}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#effect AuditLogSubscription#effect}
         '''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of action specifiers defining the actions to which the statement applies.
 
         Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#actions AuditLogSubscription#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#actions AuditLogSubscription#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of action specifiers defining the actions to which the statement does not apply.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#not_actions AuditLogSubscription#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#not_actions AuditLogSubscription#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of resource specifiers defining the resources to which the statement does not apply.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#not_resources AuditLogSubscription#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#not_resources AuditLogSubscription#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of resource specifiers defining the resources to which the statement applies.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/audit_log_subscription#resources AuditLogSubscription#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/audit_log_subscription#resources AuditLogSubscription#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/custom_role/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/custom_role/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_custom_role`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_custom_role`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role).
+Refer to the Terraform Registry for docs: [`launchdarkly_custom_role`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class CustomRole(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.customRole.CustomRole",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role launchdarkly_custom_role}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role launchdarkly_custom_role}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -47,25 +47,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role launchdarkly_custom_role} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role launchdarkly_custom_role} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: A unique key that will be used to reference the custom role in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#key CustomRole#key}
-        :param name: A name for the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#name CustomRole#name}
-        :param base_permissions: The base permission level - either reader or no_access. Defaults to reader. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#base_permissions CustomRole#base_permissions}
-        :param description: Description of the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#description CustomRole#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#id CustomRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#policy CustomRole#policy}
-        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#policy_statements CustomRole#policy_statements}
+        :param key: A unique key that will be used to reference the custom role in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#key CustomRole#key}
+        :param name: A name for the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#name CustomRole#name}
+        :param base_permissions: The base permission level - either reader or no_access. Defaults to reader. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#base_permissions CustomRole#base_permissions}
+        :param description: Description of the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#description CustomRole#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#id CustomRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#policy CustomRole#policy}
+        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#policy_statements CustomRole#policy_statements}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -102,15 +102,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a CustomRole resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the CustomRole to import.
-        :param import_from_id: The id of the existing CustomRole that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing CustomRole that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the CustomRole to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8197891f321e1cf62014e941a69d69a9676a0036c2e565fb4af261d0a17a1b60)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -329,21 +329,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: A unique key that will be used to reference the custom role in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#key CustomRole#key}
-        :param name: A name for the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#name CustomRole#name}
-        :param base_permissions: The base permission level - either reader or no_access. Defaults to reader. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#base_permissions CustomRole#base_permissions}
-        :param description: Description of the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#description CustomRole#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#id CustomRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#policy CustomRole#policy}
-        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#policy_statements CustomRole#policy_statements}
+        :param key: A unique key that will be used to reference the custom role in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#key CustomRole#key}
+        :param name: A name for the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#name CustomRole#name}
+        :param base_permissions: The base permission level - either reader or no_access. Defaults to reader. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#base_permissions CustomRole#base_permissions}
+        :param description: Description of the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#description CustomRole#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#id CustomRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#policy CustomRole#policy}
+        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#policy_statements CustomRole#policy_statements}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__07c8f74a83c7759d8c01598cfa8dc958eb71b3c4c22021be7d2d89ce6c766d90)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -452,76 +452,76 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''A unique key that will be used to reference the custom role in your code.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#key CustomRole#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#key CustomRole#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''A name for the custom role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#name CustomRole#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#name CustomRole#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def base_permissions(self) -> typing.Optional[builtins.str]:
         '''The base permission level - either reader or no_access. Defaults to reader.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#base_permissions CustomRole#base_permissions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#base_permissions CustomRole#base_permissions}
         '''
         result = self._values.get("base_permissions")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Description of the custom role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#description CustomRole#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#description CustomRole#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#id CustomRole#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#id CustomRole#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def policy(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["CustomRolePolicy"]]]:
         '''policy block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#policy CustomRole#policy}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#policy CustomRole#policy}
         '''
         result = self._values.get("policy")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["CustomRolePolicy"]]], result)
 
     @builtins.property
     def policy_statements(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["CustomRolePolicyStatements"]]]:
         '''policy_statements block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#policy_statements CustomRole#policy_statements}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#policy_statements CustomRole#policy_statements}
         '''
         result = self._values.get("policy_statements")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["CustomRolePolicyStatements"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -544,46 +544,46 @@
         self,
         *,
         actions: typing.Sequence[builtins.str],
         effect: builtins.str,
         resources: typing.Sequence[builtins.str],
     ) -> None:
         '''
-        :param actions: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#actions CustomRole#actions}.
-        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#effect CustomRole#effect}.
-        :param resources: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#resources CustomRole#resources}.
+        :param actions: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#actions CustomRole#actions}.
+        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#effect CustomRole#effect}.
+        :param resources: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#resources CustomRole#resources}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e0fff094e247e8f703f81b4e9562b0b46c16f58d75ce567d9573162aae6ea0e0)
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument resources", value=resources, expected_type=type_hints["resources"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "actions": actions,
             "effect": effect,
             "resources": resources,
         }
 
     @builtins.property
     def actions(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#actions CustomRole#actions}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#actions CustomRole#actions}.'''
         result = self._values.get("actions")
         assert result is not None, "Required property 'actions' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def effect(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#effect CustomRole#effect}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#effect CustomRole#effect}.'''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def resources(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#resources CustomRole#resources}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#resources CustomRole#resources}.'''
         result = self._values.get("resources")
         assert result is not None, "Required property 'resources' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -799,19 +799,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Either ``allow`` or ``deny``. This argument defines whether the statement allows or denies access to the named resources and actions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#effect CustomRole#effect}
-        :param actions: The list of action specifiers defining the actions to which the statement applies. Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#actions CustomRole#actions}
-        :param not_actions: The list of action specifiers defining the actions to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#not_actions CustomRole#not_actions}
-        :param not_resources: The list of resource specifiers defining the resources to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#not_resources CustomRole#not_resources}
-        :param resources: The list of resource specifiers defining the resources to which the statement applies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#resources CustomRole#resources}
+        :param effect: Either ``allow`` or ``deny``. This argument defines whether the statement allows or denies access to the named resources and actions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#effect CustomRole#effect}
+        :param actions: The list of action specifiers defining the actions to which the statement applies. Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#actions CustomRole#actions}
+        :param not_actions: The list of action specifiers defining the actions to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#not_actions CustomRole#not_actions}
+        :param not_resources: The list of resource specifiers defining the resources to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#not_resources CustomRole#not_resources}
+        :param resources: The list of resource specifiers defining the resources to which the statement applies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#resources CustomRole#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7176f75a37625f31b0c968054092a5d514a83466831576d24355e3e80666e824)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -830,54 +830,54 @@
 
     @builtins.property
     def effect(self) -> builtins.str:
         '''Either ``allow`` or ``deny``.
 
         This argument defines whether the statement allows or denies access to the named resources and actions.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#effect CustomRole#effect}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#effect CustomRole#effect}
         '''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of action specifiers defining the actions to which the statement applies.
 
         Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#actions CustomRole#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#actions CustomRole#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of action specifiers defining the actions to which the statement does not apply.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#not_actions CustomRole#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#not_actions CustomRole#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of resource specifiers defining the resources to which the statement does not apply.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#not_resources CustomRole#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#not_resources CustomRole#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of resource specifiers defining the resources to which the statement applies.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/custom_role#resources CustomRole#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/custom_role#resources CustomRole#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_audit_log_subscription/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_audit_log_subscription/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_audit_log_subscription`
 
-Refer to the Terraform Registry for docs: [`data_launchdarkly_audit_log_subscription`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/audit_log_subscription).
+Refer to the Terraform Registry for docs: [`data_launchdarkly_audit_log_subscription`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/audit_log_subscription).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class DataLaunchdarklyAuditLogSubscription(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyAuditLogSubscription.DataLaunchdarklyAuditLogSubscription",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/audit_log_subscription launchdarkly_audit_log_subscription}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/audit_log_subscription launchdarkly_audit_log_subscription}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: builtins.str,
@@ -42,20 +42,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/audit_log_subscription launchdarkly_audit_log_subscription} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/audit_log_subscription launchdarkly_audit_log_subscription} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: The audit log subscription ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/audit_log_subscription#id DataLaunchdarklyAuditLogSubscription#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param integration_key: The integration key. Supported integration keys are ``chronosphere``, ``cloudtrail``, ``datadog``, ``dynatrace``, ``elastic``, ``grafana``, ``honeycomb``, ``logdna``, ``msteams``, ``new-relic-apm``, ``signalfx``, ``slack``, and ``splunk``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/audit_log_subscription#integration_key DataLaunchdarklyAuditLogSubscription#integration_key}
+        :param id: The audit log subscription ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/audit_log_subscription#id DataLaunchdarklyAuditLogSubscription#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param integration_key: The integration key. Supported integration keys are ``chronosphere``, ``cloudtrail``, ``datadog``, ``dynatrace``, ``elastic``, ``grafana``, ``honeycomb``, ``logdna``, ``msteams``, ``new-relic-apm``, ``signalfx``, ``slack``, and ``splunk``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/audit_log_subscription#integration_key DataLaunchdarklyAuditLogSubscription#integration_key}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -87,15 +87,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataLaunchdarklyAuditLogSubscription resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataLaunchdarklyAuditLogSubscription to import.
-        :param import_from_id: The id of the existing DataLaunchdarklyAuditLogSubscription that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/audit_log_subscription#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataLaunchdarklyAuditLogSubscription that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/audit_log_subscription#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataLaunchdarklyAuditLogSubscription to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a7422ab4782073ac74b7fb6b09b4cc092fa0bdb526d4fddb249164ba1205d125)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -210,16 +210,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: The audit log subscription ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/audit_log_subscription#id DataLaunchdarklyAuditLogSubscription#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param integration_key: The integration key. Supported integration keys are ``chronosphere``, ``cloudtrail``, ``datadog``, ``dynatrace``, ``elastic``, ``grafana``, ``honeycomb``, ``logdna``, ``msteams``, ``new-relic-apm``, ``signalfx``, ``slack``, and ``splunk``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/audit_log_subscription#integration_key DataLaunchdarklyAuditLogSubscription#integration_key}
+        :param id: The audit log subscription ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/audit_log_subscription#id DataLaunchdarklyAuditLogSubscription#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param integration_key: The integration key. Supported integration keys are ``chronosphere``, ``cloudtrail``, ``datadog``, ``dynatrace``, ``elastic``, ``grafana``, ``honeycomb``, ``logdna``, ``msteams``, ``new-relic-apm``, ``signalfx``, ``slack``, and ``splunk``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/audit_log_subscription#integration_key DataLaunchdarklyAuditLogSubscription#integration_key}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__10868b98900046cc2261e2c194d4755bb088a829c32d6db63109a63b17d26f89)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -313,30 +313,30 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> builtins.str:
         '''The audit log subscription ID.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/audit_log_subscription#id DataLaunchdarklyAuditLogSubscription#id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/audit_log_subscription#id DataLaunchdarklyAuditLogSubscription#id}
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         assert result is not None, "Required property 'id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def integration_key(self) -> builtins.str:
         '''The integration key.
 
         Supported integration keys are ``chronosphere``, ``cloudtrail``, ``datadog``, ``dynatrace``, ``elastic``, ``grafana``, ``honeycomb``, ``logdna``, ``msteams``, ``new-relic-apm``, ``signalfx``, ``slack``, and ``splunk``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/audit_log_subscription#integration_key DataLaunchdarklyAuditLogSubscription#integration_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/audit_log_subscription#integration_key DataLaunchdarklyAuditLogSubscription#integration_key}
         '''
         result = self._values.get("integration_key")
         assert result is not None, "Required property 'integration_key' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_environment/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_environment/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_environment`
 
-Refer to the Terraform Registry for docs: [`data_launchdarkly_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment).
+Refer to the Terraform Registry for docs: [`data_launchdarkly_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class DataLaunchdarklyEnvironment(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyEnvironment.DataLaunchdarklyEnvironment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment launchdarkly_environment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment launchdarkly_environment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -44,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment launchdarkly_environment} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment launchdarkly_environment} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: The project-unique key for the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment#key DataLaunchdarklyEnvironment#key}
-        :param project_key: The environment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment#project_key DataLaunchdarklyEnvironment#project_key}
-        :param critical: Denotes whether the environment is critical. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment#critical DataLaunchdarklyEnvironment#critical}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment#id DataLaunchdarklyEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param key: The project-unique key for the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment#key DataLaunchdarklyEnvironment#key}
+        :param project_key: The environment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment#project_key DataLaunchdarklyEnvironment#project_key}
+        :param critical: Denotes whether the environment is critical. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment#critical DataLaunchdarklyEnvironment#critical}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment#id DataLaunchdarklyEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -93,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataLaunchdarklyEnvironment resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataLaunchdarklyEnvironment to import.
-        :param import_from_id: The id of the existing DataLaunchdarklyEnvironment that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataLaunchdarklyEnvironment that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataLaunchdarklyEnvironment to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d90bd23e68d84d5f1fedacb8ecd70cea35f1c3f6d069ab9212006ca07ddf1c4e)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -476,18 +476,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: The project-unique key for the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment#key DataLaunchdarklyEnvironment#key}
-        :param project_key: The environment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment#project_key DataLaunchdarklyEnvironment#project_key}
-        :param critical: Denotes whether the environment is critical. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment#critical DataLaunchdarklyEnvironment#critical}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment#id DataLaunchdarklyEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param key: The project-unique key for the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment#key DataLaunchdarklyEnvironment#key}
+        :param project_key: The environment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment#project_key DataLaunchdarklyEnvironment#project_key}
+        :param critical: Denotes whether the environment is critical. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment#critical DataLaunchdarklyEnvironment#critical}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment#id DataLaunchdarklyEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4ee324addf376c393e15f834298d163e79f6d102ae082c6a94d0c21841045aae)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -587,44 +587,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The project-unique key for the environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment#key DataLaunchdarklyEnvironment#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment#key DataLaunchdarklyEnvironment#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The environment's project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment#project_key DataLaunchdarklyEnvironment#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment#project_key DataLaunchdarklyEnvironment#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def critical(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Denotes whether the environment is critical.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment#critical DataLaunchdarklyEnvironment#critical}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment#critical DataLaunchdarklyEnvironment#critical}
         '''
         result = self._values.get("critical")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/environment#id DataLaunchdarklyEnvironment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/environment#id DataLaunchdarklyEnvironment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_feature_flag`
 
-Refer to the Terraform Registry for docs: [`data_launchdarkly_feature_flag`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag).
+Refer to the Terraform Registry for docs: [`data_launchdarkly_feature_flag`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class DataLaunchdarklyFeatureFlag(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyFeatureFlag.DataLaunchdarklyFeatureFlag",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag launchdarkly_feature_flag}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag launchdarkly_feature_flag}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -45,23 +45,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag launchdarkly_feature_flag} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag launchdarkly_feature_flag} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: The unique feature flag key that references the flag in your application code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}
-        :param project_key: The feature flag's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#project_key DataLaunchdarklyFeatureFlag#project_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#id DataLaunchdarklyFeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param maintainer_id: The feature flag maintainer's 24 character alphanumeric team member ID. ``maintainer_team_key`` cannot be set if ``maintainer_id`` is set. If neither is set, it will automatically be or stay set to the member ID associated with the API key used by your LaunchDarkly Terraform provider or the most recently-set maintainer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#maintainer_id DataLaunchdarklyFeatureFlag#maintainer_id}
-        :param maintainer_team_key: The key of the associated team that maintains this feature flag. ``maintainer_id`` cannot be set if ``maintainer_team_key`` is set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#maintainer_team_key DataLaunchdarklyFeatureFlag#maintainer_team_key}
+        :param key: The unique feature flag key that references the flag in your application code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}
+        :param project_key: The feature flag's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#project_key DataLaunchdarklyFeatureFlag#project_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#id DataLaunchdarklyFeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param maintainer_id: The feature flag maintainer's 24 character alphanumeric team member ID. ``maintainer_team_key`` cannot be set if ``maintainer_id`` is set. If neither is set, it will automatically be or stay set to the member ID associated with the API key used by your LaunchDarkly Terraform provider or the most recently-set maintainer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#maintainer_id DataLaunchdarklyFeatureFlag#maintainer_id}
+        :param maintainer_team_key: The key of the associated team that maintains this feature flag. ``maintainer_id`` cannot be set if ``maintainer_team_key`` is set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#maintainer_team_key DataLaunchdarklyFeatureFlag#maintainer_team_key}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -96,15 +96,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataLaunchdarklyFeatureFlag resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataLaunchdarklyFeatureFlag to import.
-        :param import_from_id: The id of the existing DataLaunchdarklyFeatureFlag that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataLaunchdarklyFeatureFlag that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataLaunchdarklyFeatureFlag to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cf79ead42c7cfc000b3592742ddc7ed149b6ee1e6db9a469423a7abd9df1a410)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -469,19 +469,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: The unique feature flag key that references the flag in your application code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}
-        :param project_key: The feature flag's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#project_key DataLaunchdarklyFeatureFlag#project_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#id DataLaunchdarklyFeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param maintainer_id: The feature flag maintainer's 24 character alphanumeric team member ID. ``maintainer_team_key`` cannot be set if ``maintainer_id`` is set. If neither is set, it will automatically be or stay set to the member ID associated with the API key used by your LaunchDarkly Terraform provider or the most recently-set maintainer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#maintainer_id DataLaunchdarklyFeatureFlag#maintainer_id}
-        :param maintainer_team_key: The key of the associated team that maintains this feature flag. ``maintainer_id`` cannot be set if ``maintainer_team_key`` is set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#maintainer_team_key DataLaunchdarklyFeatureFlag#maintainer_team_key}
+        :param key: The unique feature flag key that references the flag in your application code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}
+        :param project_key: The feature flag's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#project_key DataLaunchdarklyFeatureFlag#project_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#id DataLaunchdarklyFeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param maintainer_id: The feature flag maintainer's 24 character alphanumeric team member ID. ``maintainer_team_key`` cannot be set if ``maintainer_id`` is set. If neither is set, it will automatically be or stay set to the member ID associated with the API key used by your LaunchDarkly Terraform provider or the most recently-set maintainer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#maintainer_id DataLaunchdarklyFeatureFlag#maintainer_id}
+        :param maintainer_team_key: The key of the associated team that maintains this feature flag. ``maintainer_id`` cannot be set if ``maintainer_team_key`` is set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#maintainer_team_key DataLaunchdarklyFeatureFlag#maintainer_team_key}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__530b455bc63811ba078aa401a86b5e682619333c87f8c2405c03d404a47fc2b1)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -584,56 +584,56 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The unique feature flag key that references the flag in your application code.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The feature flag's project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#project_key DataLaunchdarklyFeatureFlag#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#project_key DataLaunchdarklyFeatureFlag#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#id DataLaunchdarklyFeatureFlag#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#id DataLaunchdarklyFeatureFlag#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def maintainer_id(self) -> typing.Optional[builtins.str]:
         '''The feature flag maintainer's 24 character alphanumeric team member ID.
 
         ``maintainer_team_key`` cannot be set if ``maintainer_id`` is set. If neither is set, it will automatically be or stay set to the member ID associated with the API key used by your LaunchDarkly Terraform provider or the most recently-set maintainer.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#maintainer_id DataLaunchdarklyFeatureFlag#maintainer_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#maintainer_id DataLaunchdarklyFeatureFlag#maintainer_id}
         '''
         result = self._values.get("maintainer_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def maintainer_team_key(self) -> typing.Optional[builtins.str]:
         '''The key of the associated team that maintains this feature flag. ``maintainer_id`` cannot be set if ``maintainer_team_key`` is set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag#maintainer_team_key DataLaunchdarklyFeatureFlag#maintainer_team_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag#maintainer_team_key DataLaunchdarklyFeatureFlag#maintainer_team_key}
         '''
         result = self._values.get("maintainer_team_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag_environment/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag_environment/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_feature_flag_environment`
 
-Refer to the Terraform Registry for docs: [`data_launchdarkly_feature_flag_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag_environment).
+Refer to the Terraform Registry for docs: [`data_launchdarkly_feature_flag_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag_environment).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class DataLaunchdarklyFeatureFlagEnvironment(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyFeatureFlagEnvironment.DataLaunchdarklyFeatureFlagEnvironment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag_environment launchdarkly_feature_flag_environment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag_environment launchdarkly_feature_flag_environment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         env_key: builtins.str,
@@ -43,21 +43,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag_environment launchdarkly_feature_flag_environment} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag_environment launchdarkly_feature_flag_environment} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param env_key: The environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag_environment#env_key DataLaunchdarklyFeatureFlagEnvironment#env_key}
-        :param flag_id: The feature flag's unique ``id`` in the format ``project_key/flag_key``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag_environment#flag_id DataLaunchdarklyFeatureFlagEnvironment#flag_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag_environment#id DataLaunchdarklyFeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param env_key: The environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag_environment#env_key DataLaunchdarklyFeatureFlagEnvironment#env_key}
+        :param flag_id: The feature flag's unique ``id`` in the format ``project_key/flag_key``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag_environment#flag_id DataLaunchdarklyFeatureFlagEnvironment#flag_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag_environment#id DataLaunchdarklyFeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +90,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataLaunchdarklyFeatureFlagEnvironment resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataLaunchdarklyFeatureFlagEnvironment to import.
-        :param import_from_id: The id of the existing DataLaunchdarklyFeatureFlagEnvironment that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag_environment#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataLaunchdarklyFeatureFlagEnvironment that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag_environment#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataLaunchdarklyFeatureFlagEnvironment to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bcbdece8673f98de26c21b45f8218ee2d6ccc672cdae393049585cfb49b3c54f)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -255,17 +255,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param env_key: The environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag_environment#env_key DataLaunchdarklyFeatureFlagEnvironment#env_key}
-        :param flag_id: The feature flag's unique ``id`` in the format ``project_key/flag_key``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag_environment#flag_id DataLaunchdarklyFeatureFlagEnvironment#flag_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag_environment#id DataLaunchdarklyFeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param env_key: The environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag_environment#env_key DataLaunchdarklyFeatureFlagEnvironment#env_key}
+        :param flag_id: The feature flag's unique ``id`` in the format ``project_key/flag_key``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag_environment#flag_id DataLaunchdarklyFeatureFlagEnvironment#flag_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag_environment#id DataLaunchdarklyFeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3887b8a55bec50ce0052798f0dc17b208c0f50312a4ba4a1a14d0afb5a2ac31c)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -362,33 +362,33 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def env_key(self) -> builtins.str:
         '''The environment key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag_environment#env_key DataLaunchdarklyFeatureFlagEnvironment#env_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag_environment#env_key DataLaunchdarklyFeatureFlagEnvironment#env_key}
         '''
         result = self._values.get("env_key")
         assert result is not None, "Required property 'env_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def flag_id(self) -> builtins.str:
         '''The feature flag's unique ``id`` in the format ``project_key/flag_key``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag_environment#flag_id DataLaunchdarklyFeatureFlagEnvironment#flag_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag_environment#flag_id DataLaunchdarklyFeatureFlagEnvironment#flag_id}
         '''
         result = self._values.get("flag_id")
         assert result is not None, "Required property 'flag_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/feature_flag_environment#id DataLaunchdarklyFeatureFlagEnvironment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/feature_flag_environment#id DataLaunchdarklyFeatureFlagEnvironment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_flag_trigger/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_flag_trigger/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_flag_trigger`
 
-Refer to the Terraform Registry for docs: [`data_launchdarkly_flag_trigger`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger).
+Refer to the Terraform Registry for docs: [`data_launchdarkly_flag_trigger`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class DataLaunchdarklyFlagTrigger(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyFlagTrigger.DataLaunchdarklyFlagTrigger",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger launchdarkly_flag_trigger}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger launchdarkly_flag_trigger}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         env_key: builtins.str,
@@ -47,25 +47,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger launchdarkly_flag_trigger} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger launchdarkly_flag_trigger} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#env_key DataLaunchdarklyFlagTrigger#env_key}
-        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#flag_key DataLaunchdarklyFlagTrigger#flag_key}
-        :param id: The flag trigger resource ID. This can be found on your trigger URL - please see docs for more info Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#id DataLaunchdarklyFlagTrigger#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#project_key DataLaunchdarklyFlagTrigger#project_key}
-        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#enabled DataLaunchdarklyFlagTrigger#enabled}
-        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#instructions DataLaunchdarklyFlagTrigger#instructions}
-        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#integration_key DataLaunchdarklyFlagTrigger#integration_key}
+        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#env_key DataLaunchdarklyFlagTrigger#env_key}
+        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#flag_key DataLaunchdarklyFlagTrigger#flag_key}
+        :param id: The flag trigger resource ID. This can be found on your trigger URL - please see docs for more info Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#id DataLaunchdarklyFlagTrigger#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#project_key DataLaunchdarklyFlagTrigger#project_key}
+        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#enabled DataLaunchdarklyFlagTrigger#enabled}
+        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#instructions DataLaunchdarklyFlagTrigger#instructions}
+        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#integration_key DataLaunchdarklyFlagTrigger#integration_key}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -102,29 +102,29 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataLaunchdarklyFlagTrigger resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataLaunchdarklyFlagTrigger to import.
-        :param import_from_id: The id of the existing DataLaunchdarklyFlagTrigger that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataLaunchdarklyFlagTrigger that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataLaunchdarklyFlagTrigger to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8cde40aaecd304dc8c96e04d9a05fb2d3e4c0b94e399cb2720bf628c7b0882e7)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
         return typing.cast(_cdktf_9a9027ec.ImportableResource, jsii.sinvoke(cls, "generateConfigForImport", [scope, import_to_id, import_from_id, provider]))
 
     @jsii.member(jsii_name="putInstructions")
     def put_instructions(self, *, kind: builtins.str) -> None:
         '''
-        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#kind DataLaunchdarklyFlagTrigger#kind}
+        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#kind DataLaunchdarklyFlagTrigger#kind}
         '''
         value = DataLaunchdarklyFlagTriggerInstructions(kind=kind)
 
         return typing.cast(None, jsii.invoke(self, "putInstructions", [value]))
 
     @jsii.member(jsii_name="resetEnabled")
     def reset_enabled(self) -> None:
@@ -324,21 +324,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#env_key DataLaunchdarklyFlagTrigger#env_key}
-        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#flag_key DataLaunchdarklyFlagTrigger#flag_key}
-        :param id: The flag trigger resource ID. This can be found on your trigger URL - please see docs for more info Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#id DataLaunchdarklyFlagTrigger#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#project_key DataLaunchdarklyFlagTrigger#project_key}
-        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#enabled DataLaunchdarklyFlagTrigger#enabled}
-        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#instructions DataLaunchdarklyFlagTrigger#instructions}
-        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#integration_key DataLaunchdarklyFlagTrigger#integration_key}
+        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#env_key DataLaunchdarklyFlagTrigger#env_key}
+        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#flag_key DataLaunchdarklyFlagTrigger#flag_key}
+        :param id: The flag trigger resource ID. This can be found on your trigger URL - please see docs for more info Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#id DataLaunchdarklyFlagTrigger#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#project_key DataLaunchdarklyFlagTrigger#project_key}
+        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#enabled DataLaunchdarklyFlagTrigger#enabled}
+        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#instructions DataLaunchdarklyFlagTrigger#instructions}
+        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#integration_key DataLaunchdarklyFlagTrigger#integration_key}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(instructions, dict):
             instructions = DataLaunchdarklyFlagTriggerInstructions(**instructions)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5035f89f2d6f39b0055a9fa8c745d6fd8d07edb45d3058407584bfb25fc0ac54)
@@ -447,84 +447,84 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def env_key(self) -> builtins.str:
         '''The LaunchDarkly environment key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#env_key DataLaunchdarklyFlagTrigger#env_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#env_key DataLaunchdarklyFlagTrigger#env_key}
         '''
         result = self._values.get("env_key")
         assert result is not None, "Required property 'env_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def flag_key(self) -> builtins.str:
         '''The key of the feature flag the trigger acts upon.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#flag_key DataLaunchdarklyFlagTrigger#flag_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#flag_key DataLaunchdarklyFlagTrigger#flag_key}
         '''
         result = self._values.get("flag_key")
         assert result is not None, "Required property 'flag_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> builtins.str:
         '''The flag trigger resource ID.
 
         This can be found on your trigger URL - please see docs for more info
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#id DataLaunchdarklyFlagTrigger#id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#id DataLaunchdarklyFlagTrigger#id}
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         assert result is not None, "Required property 'id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The LaunchDarkly project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#project_key DataLaunchdarklyFlagTrigger#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#project_key DataLaunchdarklyFlagTrigger#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the trigger is currently active or not. This property defaults to true upon creation.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#enabled DataLaunchdarklyFlagTrigger#enabled}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#enabled DataLaunchdarklyFlagTrigger#enabled}
         '''
         result = self._values.get("enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def instructions(
         self,
     ) -> typing.Optional["DataLaunchdarklyFlagTriggerInstructions"]:
         '''instructions block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#instructions DataLaunchdarklyFlagTrigger#instructions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#instructions DataLaunchdarklyFlagTrigger#instructions}
         '''
         result = self._values.get("instructions")
         return typing.cast(typing.Optional["DataLaunchdarklyFlagTriggerInstructions"], result)
 
     @builtins.property
     def integration_key(self) -> typing.Optional[builtins.str]:
         '''The unique identifier of the integration you intend to set your trigger up with.
 
         "generic-trigger" should be used for integrations not explicitly supported.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#integration_key DataLaunchdarklyFlagTrigger#integration_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#integration_key DataLaunchdarklyFlagTrigger#integration_key}
         '''
         result = self._values.get("integration_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -541,28 +541,28 @@
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyFlagTrigger.DataLaunchdarklyFlagTriggerInstructions",
     jsii_struct_bases=[],
     name_mapping={"kind": "kind"},
 )
 class DataLaunchdarklyFlagTriggerInstructions:
     def __init__(self, *, kind: builtins.str) -> None:
         '''
-        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#kind DataLaunchdarklyFlagTrigger#kind}
+        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#kind DataLaunchdarklyFlagTrigger#kind}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__427f08c549989595caa6db049131fa89e8c1d630b31e68b677cbd3f1109dce0d)
             check_type(argname="argument kind", value=kind, expected_type=type_hints["kind"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "kind": kind,
         }
 
     @builtins.property
     def kind(self) -> builtins.str:
         '''The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff".
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/flag_trigger#kind DataLaunchdarklyFlagTrigger#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/flag_trigger#kind DataLaunchdarklyFlagTrigger#kind}
         '''
         result = self._values.get("kind")
         assert result is not None, "Required property 'kind' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_metric/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_metric/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_metric`
 
-Refer to the Terraform Registry for docs: [`data_launchdarkly_metric`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric).
+Refer to the Terraform Registry for docs: [`data_launchdarkly_metric`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class DataLaunchdarklyMetric(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyMetric.DataLaunchdarklyMetric",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric launchdarkly_metric}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric launchdarkly_metric}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -55,33 +55,33 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric launchdarkly_metric} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric launchdarkly_metric} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#key DataLaunchdarklyMetric#key}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#project_key DataLaunchdarklyMetric#project_key}
-        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#description DataLaunchdarklyMetric#description}
-        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#event_key DataLaunchdarklyMetric#event_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#id DataLaunchdarklyMetric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#is_active DataLaunchdarklyMetric#is_active}
-        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#is_numeric DataLaunchdarklyMetric#is_numeric}
-        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
-        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#maintainer_id DataLaunchdarklyMetric#maintainer_id}
-        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#name DataLaunchdarklyMetric#name}
-        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#randomization_units DataLaunchdarklyMetric#randomization_units}
-        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#selector DataLaunchdarklyMetric#selector}
-        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#success_criteria DataLaunchdarklyMetric#success_criteria}
-        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#unit DataLaunchdarklyMetric#unit}
-        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#urls DataLaunchdarklyMetric#urls}
+        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#key DataLaunchdarklyMetric#key}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#project_key DataLaunchdarklyMetric#project_key}
+        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#description DataLaunchdarklyMetric#description}
+        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#event_key DataLaunchdarklyMetric#event_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#id DataLaunchdarklyMetric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#is_active DataLaunchdarklyMetric#is_active}
+        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#is_numeric DataLaunchdarklyMetric#is_numeric}
+        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
+        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#maintainer_id DataLaunchdarklyMetric#maintainer_id}
+        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#name DataLaunchdarklyMetric#name}
+        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#randomization_units DataLaunchdarklyMetric#randomization_units}
+        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#selector DataLaunchdarklyMetric#selector}
+        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#success_criteria DataLaunchdarklyMetric#success_criteria}
+        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#unit DataLaunchdarklyMetric#unit}
+        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#urls DataLaunchdarklyMetric#urls}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -126,15 +126,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataLaunchdarklyMetric resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataLaunchdarklyMetric to import.
-        :param import_from_id: The id of the existing DataLaunchdarklyMetric that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataLaunchdarklyMetric that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataLaunchdarklyMetric to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b658093c5ff8c90baca64fe00d4ab21afde9de87023ffc429da18df2c113f5b7)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -544,29 +544,29 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#key DataLaunchdarklyMetric#key}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#project_key DataLaunchdarklyMetric#project_key}
-        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#description DataLaunchdarklyMetric#description}
-        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#event_key DataLaunchdarklyMetric#event_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#id DataLaunchdarklyMetric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#is_active DataLaunchdarklyMetric#is_active}
-        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#is_numeric DataLaunchdarklyMetric#is_numeric}
-        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
-        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#maintainer_id DataLaunchdarklyMetric#maintainer_id}
-        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#name DataLaunchdarklyMetric#name}
-        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#randomization_units DataLaunchdarklyMetric#randomization_units}
-        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#selector DataLaunchdarklyMetric#selector}
-        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#success_criteria DataLaunchdarklyMetric#success_criteria}
-        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#unit DataLaunchdarklyMetric#unit}
-        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#urls DataLaunchdarklyMetric#urls}
+        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#key DataLaunchdarklyMetric#key}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#project_key DataLaunchdarklyMetric#project_key}
+        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#description DataLaunchdarklyMetric#description}
+        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#event_key DataLaunchdarklyMetric#event_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#id DataLaunchdarklyMetric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#is_active DataLaunchdarklyMetric#is_active}
+        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#is_numeric DataLaunchdarklyMetric#is_numeric}
+        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
+        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#maintainer_id DataLaunchdarklyMetric#maintainer_id}
+        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#name DataLaunchdarklyMetric#name}
+        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#randomization_units DataLaunchdarklyMetric#randomization_units}
+        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#selector DataLaunchdarklyMetric#selector}
+        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#success_criteria DataLaunchdarklyMetric#success_criteria}
+        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#unit DataLaunchdarklyMetric#unit}
+        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#urls DataLaunchdarklyMetric#urls}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c4e7dd175594ceed19a99d810c24f0f6258ee9cd02779a36f8dc3326a139dca9)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -699,152 +699,152 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''A unique key that will be used to reference the metric in your code.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#key DataLaunchdarklyMetric#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#key DataLaunchdarklyMetric#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The LaunchDarkly project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#project_key DataLaunchdarklyMetric#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#project_key DataLaunchdarklyMetric#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''A short description of what the metric will be used for.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#description DataLaunchdarklyMetric#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#description DataLaunchdarklyMetric#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def event_key(self) -> typing.Optional[builtins.str]:
         '''The event key for your metric (if custom metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#event_key DataLaunchdarklyMetric#event_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#event_key DataLaunchdarklyMetric#event_key}
         '''
         result = self._values.get("event_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#id DataLaunchdarklyMetric#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#id DataLaunchdarklyMetric#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def is_active(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the metric is active.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#is_active DataLaunchdarklyMetric#is_active}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#is_active DataLaunchdarklyMetric#is_active}
         '''
         result = self._values.get("is_active")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def is_numeric(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the metric is numeric.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#is_numeric DataLaunchdarklyMetric#is_numeric}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#is_numeric DataLaunchdarklyMetric#is_numeric}
         '''
         result = self._values.get("is_numeric")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def kind(self) -> typing.Optional[builtins.str]:
         '''The metric type -available choices are 'pageview', 'click', and 'custom'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
         '''
         result = self._values.get("kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def maintainer_id(self) -> typing.Optional[builtins.str]:
         '''The LaunchDarkly ID of the user who will maintain the metric.
 
         If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#maintainer_id DataLaunchdarklyMetric#maintainer_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#maintainer_id DataLaunchdarklyMetric#maintainer_id}
         '''
         result = self._values.get("maintainer_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''A human-readable name for your metric.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#name DataLaunchdarklyMetric#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#name DataLaunchdarklyMetric#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def randomization_units(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A set of one or more context kinds that this metric can measure events from.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#randomization_units DataLaunchdarklyMetric#randomization_units}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#randomization_units DataLaunchdarklyMetric#randomization_units}
         '''
         result = self._values.get("randomization_units")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def selector(self) -> typing.Optional[builtins.str]:
         '''The CSS selector for your metric (if click metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#selector DataLaunchdarklyMetric#selector}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#selector DataLaunchdarklyMetric#selector}
         '''
         result = self._values.get("selector")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def success_criteria(self) -> typing.Optional[builtins.str]:
         '''The success criteria for your metric (if numeric metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#success_criteria DataLaunchdarklyMetric#success_criteria}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#success_criteria DataLaunchdarklyMetric#success_criteria}
         '''
         result = self._values.get("success_criteria")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def unit(self) -> typing.Optional[builtins.str]:
         '''The unit for your metric (if numeric metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#unit DataLaunchdarklyMetric#unit}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#unit DataLaunchdarklyMetric#unit}
         '''
         result = self._values.get("unit")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def urls(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyMetricUrls"]]]:
         '''urls block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#urls DataLaunchdarklyMetric#urls}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#urls DataLaunchdarklyMetric#urls}
         '''
         result = self._values.get("urls")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyMetricUrls"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -873,18 +873,18 @@
         *,
         kind: builtins.str,
         pattern: typing.Optional[builtins.str] = None,
         substring: typing.Optional[builtins.str] = None,
         url: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param kind: The url type - available choices are 'exact', 'canonical', 'substring' and 'regex'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
-        :param pattern: The URL-matching regex. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#pattern DataLaunchdarklyMetric#pattern}
-        :param substring: The URL substring. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#substring DataLaunchdarklyMetric#substring}
-        :param url: The exact or canonical URL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#url DataLaunchdarklyMetric#url}
+        :param kind: The url type - available choices are 'exact', 'canonical', 'substring' and 'regex'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
+        :param pattern: The URL-matching regex. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#pattern DataLaunchdarklyMetric#pattern}
+        :param substring: The URL substring. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#substring DataLaunchdarklyMetric#substring}
+        :param url: The exact or canonical URL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#url DataLaunchdarklyMetric#url}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c17be6f52ff7b594d336bd7722da74adc4c2ebbae3659610d20c305cddd8aa1e)
             check_type(argname="argument kind", value=kind, expected_type=type_hints["kind"])
             check_type(argname="argument pattern", value=pattern, expected_type=type_hints["pattern"])
             check_type(argname="argument substring", value=substring, expected_type=type_hints["substring"])
             check_type(argname="argument url", value=url, expected_type=type_hints["url"])
@@ -898,43 +898,43 @@
         if url is not None:
             self._values["url"] = url
 
     @builtins.property
     def kind(self) -> builtins.str:
         '''The url type - available choices are 'exact', 'canonical', 'substring' and 'regex'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
         '''
         result = self._values.get("kind")
         assert result is not None, "Required property 'kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def pattern(self) -> typing.Optional[builtins.str]:
         '''The URL-matching regex.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#pattern DataLaunchdarklyMetric#pattern}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#pattern DataLaunchdarklyMetric#pattern}
         '''
         result = self._values.get("pattern")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def substring(self) -> typing.Optional[builtins.str]:
         '''The URL substring.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#substring DataLaunchdarklyMetric#substring}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#substring DataLaunchdarklyMetric#substring}
         '''
         result = self._values.get("substring")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def url(self) -> typing.Optional[builtins.str]:
         '''The exact or canonical URL.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/metric#url DataLaunchdarklyMetric#url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/metric#url DataLaunchdarklyMetric#url}
         '''
         result = self._values.get("url")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_project/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_project/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_project`
 
-Refer to the Terraform Registry for docs: [`data_launchdarkly_project`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/project).
+Refer to the Terraform Registry for docs: [`data_launchdarkly_project`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/project).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class DataLaunchdarklyProject(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyProject.DataLaunchdarklyProject",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/project launchdarkly_project}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/project launchdarkly_project}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -42,20 +42,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/project launchdarkly_project} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/project launchdarkly_project} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/project#key DataLaunchdarklyProject#key}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/project#id DataLaunchdarklyProject#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/project#key DataLaunchdarklyProject#key}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/project#id DataLaunchdarklyProject#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -87,15 +87,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataLaunchdarklyProject resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataLaunchdarklyProject to import.
-        :param import_from_id: The id of the existing DataLaunchdarklyProject that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/project#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataLaunchdarklyProject that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/project#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataLaunchdarklyProject to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__af431f0bfcd1a6e1460605dd9f80e8a250526b181238ac0c1077066ceec5324e)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -362,16 +362,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/project#key DataLaunchdarklyProject#key}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/project#id DataLaunchdarklyProject#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/project#key DataLaunchdarklyProject#key}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/project#id DataLaunchdarklyProject#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f677daac99e59cdf82ec5988e548c38ce1342b3e3d28a5ff2fd218aba3a04e0d)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -464,22 +464,22 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/project#key DataLaunchdarklyProject#key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/project#key DataLaunchdarklyProject#key}.'''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/project#id DataLaunchdarklyProject#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/project#id DataLaunchdarklyProject#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_relay_proxy_configuration/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_relay_proxy_configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_relay_proxy_configuration`
 
-Refer to the Terraform Registry for docs: [`data_launchdarkly_relay_proxy_configuration`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/relay_proxy_configuration).
+Refer to the Terraform Registry for docs: [`data_launchdarkly_relay_proxy_configuration`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/relay_proxy_configuration).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class DataLaunchdarklyRelayProxyConfiguration(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyRelayProxyConfiguration.DataLaunchdarklyRelayProxyConfiguration",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/relay_proxy_configuration launchdarkly_relay_proxy_configuration}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/relay_proxy_configuration launchdarkly_relay_proxy_configuration}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: builtins.str,
@@ -41,19 +41,19 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/relay_proxy_configuration launchdarkly_relay_proxy_configuration} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/relay_proxy_configuration launchdarkly_relay_proxy_configuration} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: The Relay Proxy configuration's unique 24 character ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/relay_proxy_configuration#id DataLaunchdarklyRelayProxyConfiguration#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The Relay Proxy configuration's unique 24 character ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/relay_proxy_configuration#id DataLaunchdarklyRelayProxyConfiguration#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -84,15 +84,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataLaunchdarklyRelayProxyConfiguration resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataLaunchdarklyRelayProxyConfiguration to import.
-        :param import_from_id: The id of the existing DataLaunchdarklyRelayProxyConfiguration that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/relay_proxy_configuration#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataLaunchdarklyRelayProxyConfiguration that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/relay_proxy_configuration#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataLaunchdarklyRelayProxyConfiguration to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0e9c57356dd4459122b96d2b82d3b1347a50cc512cb407e03c95f08e5cbc3c23)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -178,15 +178,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: The Relay Proxy configuration's unique 24 character ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/relay_proxy_configuration#id DataLaunchdarklyRelayProxyConfiguration#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The Relay Proxy configuration's unique 24 character ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/relay_proxy_configuration#id DataLaunchdarklyRelayProxyConfiguration#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1583f398ed928478045304696977a511501bb413634c7326cb91b8d838efddcb)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -278,15 +278,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> builtins.str:
         '''The Relay Proxy configuration's unique 24 character ID.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/relay_proxy_configuration#id DataLaunchdarklyRelayProxyConfiguration#id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/relay_proxy_configuration#id DataLaunchdarklyRelayProxyConfiguration#id}
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         assert result is not None, "Required property 'id' is missing"
         return typing.cast(builtins.str, result)
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_segment/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_segment/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_segment`
 
-Refer to the Terraform Registry for docs: [`data_launchdarkly_segment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment).
+Refer to the Terraform Registry for docs: [`data_launchdarkly_segment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class DataLaunchdarklySegment(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklySegment.DataLaunchdarklySegment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment launchdarkly_segment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment launchdarkly_segment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         env_key: builtins.str,
@@ -44,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment launchdarkly_segment} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment launchdarkly_segment} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param env_key: The segment's environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment#env_key DataLaunchdarklySegment#env_key}
-        :param key: The unique key that references the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment#key DataLaunchdarklySegment#key}
-        :param project_key: The segment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment#project_key DataLaunchdarklySegment#project_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment#id DataLaunchdarklySegment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param env_key: The segment's environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment#env_key DataLaunchdarklySegment#env_key}
+        :param key: The unique key that references the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment#key DataLaunchdarklySegment#key}
+        :param project_key: The segment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment#project_key DataLaunchdarklySegment#project_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment#id DataLaunchdarklySegment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -93,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataLaunchdarklySegment resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataLaunchdarklySegment to import.
-        :param import_from_id: The id of the existing DataLaunchdarklySegment that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataLaunchdarklySegment that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataLaunchdarklySegment to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e9a08e7c408f4b275be742f1b1e8671ae447a72a7327b4eb14a57a27cccd9901)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -286,18 +286,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param env_key: The segment's environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment#env_key DataLaunchdarklySegment#env_key}
-        :param key: The unique key that references the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment#key DataLaunchdarklySegment#key}
-        :param project_key: The segment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment#project_key DataLaunchdarklySegment#project_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment#id DataLaunchdarklySegment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param env_key: The segment's environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment#env_key DataLaunchdarklySegment#env_key}
+        :param key: The unique key that references the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment#key DataLaunchdarklySegment#key}
+        :param project_key: The segment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment#project_key DataLaunchdarklySegment#project_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment#id DataLaunchdarklySegment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4968e8cf106963aaca9d99652b60495322567d70543e75826303606d06a6f0ab)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -396,43 +396,43 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def env_key(self) -> builtins.str:
         '''The segment's environment key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment#env_key DataLaunchdarklySegment#env_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment#env_key DataLaunchdarklySegment#env_key}
         '''
         result = self._values.get("env_key")
         assert result is not None, "Required property 'env_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The unique key that references the segment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment#key DataLaunchdarklySegment#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment#key DataLaunchdarklySegment#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The segment's project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment#project_key DataLaunchdarklySegment#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment#project_key DataLaunchdarklySegment#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/segment#id DataLaunchdarklySegment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/segment#id DataLaunchdarklySegment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_team`
 
-Refer to the Terraform Registry for docs: [`data_launchdarkly_team`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team).
+Refer to the Terraform Registry for docs: [`data_launchdarkly_team`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class DataLaunchdarklyTeam(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyTeam.DataLaunchdarklyTeam",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team launchdarkly_team}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team launchdarkly_team}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -45,23 +45,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team launchdarkly_team} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team launchdarkly_team} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#key DataLaunchdarklyTeam#key}
-        :param custom_role_keys: A list of keys for custom roles the team has. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#custom_role_keys DataLaunchdarklyTeam#custom_role_keys}
-        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#description DataLaunchdarklyTeam#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#id DataLaunchdarklyTeam#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#name DataLaunchdarklyTeam#name}
+        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#key DataLaunchdarklyTeam#key}
+        :param custom_role_keys: A list of keys for custom roles the team has. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#custom_role_keys DataLaunchdarklyTeam#custom_role_keys}
+        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#description DataLaunchdarklyTeam#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#id DataLaunchdarklyTeam#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#name DataLaunchdarklyTeam#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -96,15 +96,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataLaunchdarklyTeam resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataLaunchdarklyTeam to import.
-        :param import_from_id: The id of the existing DataLaunchdarklyTeam that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataLaunchdarklyTeam that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataLaunchdarklyTeam to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b67b4ae76ef6f587f8285f8a251cb987601d2e1cd03459b6409252e903d95b14)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -275,19 +275,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#key DataLaunchdarklyTeam#key}
-        :param custom_role_keys: A list of keys for custom roles the team has. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#custom_role_keys DataLaunchdarklyTeam#custom_role_keys}
-        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#description DataLaunchdarklyTeam#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#id DataLaunchdarklyTeam#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#name DataLaunchdarklyTeam#name}
+        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#key DataLaunchdarklyTeam#key}
+        :param custom_role_keys: A list of keys for custom roles the team has. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#custom_role_keys DataLaunchdarklyTeam#custom_role_keys}
+        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#description DataLaunchdarklyTeam#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#id DataLaunchdarklyTeam#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#name DataLaunchdarklyTeam#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7badedbfe7425728bb984aea443d446b602f67e9c6bef983bb86976600624516)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -391,53 +391,53 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The team's unique key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#key DataLaunchdarklyTeam#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#key DataLaunchdarklyTeam#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def custom_role_keys(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of keys for custom roles the team has.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#custom_role_keys DataLaunchdarklyTeam#custom_role_keys}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#custom_role_keys DataLaunchdarklyTeam#custom_role_keys}
         '''
         result = self._values.get("custom_role_keys")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The team's description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#description DataLaunchdarklyTeam#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#description DataLaunchdarklyTeam#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#id DataLaunchdarklyTeam#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#id DataLaunchdarklyTeam#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The team's human-readable name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team#name DataLaunchdarklyTeam#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team#name DataLaunchdarklyTeam#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_member/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_member/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_team_member`
 
-Refer to the Terraform Registry for docs: [`data_launchdarkly_team_member`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_member).
+Refer to the Terraform Registry for docs: [`data_launchdarkly_team_member`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_member).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class DataLaunchdarklyTeamMember(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyTeamMember.DataLaunchdarklyTeamMember",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_member launchdarkly_team_member}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_member launchdarkly_team_member}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         email: builtins.str,
@@ -42,20 +42,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_member launchdarkly_team_member} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_member launchdarkly_team_member} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_member#email DataLaunchdarklyTeamMember#email}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_member#id DataLaunchdarklyTeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_member#email DataLaunchdarklyTeamMember#email}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_member#id DataLaunchdarklyTeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -87,15 +87,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataLaunchdarklyTeamMember resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataLaunchdarklyTeamMember to import.
-        :param import_from_id: The id of the existing DataLaunchdarklyTeamMember that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_member#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataLaunchdarklyTeamMember that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_member#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataLaunchdarklyTeamMember to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f8fd7a14404bc47fd617308961b46bd1e5045670ebad699722c5b927007f8510)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -207,16 +207,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_member#email DataLaunchdarklyTeamMember#email}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_member#id DataLaunchdarklyTeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_member#email DataLaunchdarklyTeamMember#email}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_member#id DataLaunchdarklyTeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7a6edd1e638b44c7b98e955269c9bca5af17547ada027c5912fee47e117b60da)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -309,22 +309,22 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def email(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_member#email DataLaunchdarklyTeamMember#email}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_member#email DataLaunchdarklyTeamMember#email}.'''
         result = self._values.get("email")
         assert result is not None, "Required property 'email' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_member#id DataLaunchdarklyTeamMember#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_member#id DataLaunchdarklyTeamMember#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_members/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_members/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_team_members`
 
-Refer to the Terraform Registry for docs: [`data_launchdarkly_team_members`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_members).
+Refer to the Terraform Registry for docs: [`data_launchdarkly_team_members`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_members).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class DataLaunchdarklyTeamMembers(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyTeamMembers.DataLaunchdarklyTeamMembers",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_members launchdarkly_team_members}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_members launchdarkly_team_members}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         emails: typing.Sequence[builtins.str],
@@ -43,21 +43,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_members launchdarkly_team_members} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_members launchdarkly_team_members} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param emails: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_members#emails DataLaunchdarklyTeamMembers#emails}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_members#id DataLaunchdarklyTeamMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ignore_missing: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_members#ignore_missing DataLaunchdarklyTeamMembers#ignore_missing}.
+        :param emails: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_members#emails DataLaunchdarklyTeamMembers#emails}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_members#id DataLaunchdarklyTeamMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param ignore_missing: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_members#ignore_missing DataLaunchdarklyTeamMembers#ignore_missing}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +90,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataLaunchdarklyTeamMembers resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataLaunchdarklyTeamMembers to import.
-        :param import_from_id: The id of the existing DataLaunchdarklyTeamMembers that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_members#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataLaunchdarklyTeamMembers that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_members#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataLaunchdarklyTeamMembers to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__138ac06dc97a89d0bd62d7cdedea843371476f1f187b14dbf6800c71a608d44e)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -225,17 +225,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param emails: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_members#emails DataLaunchdarklyTeamMembers#emails}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_members#id DataLaunchdarklyTeamMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ignore_missing: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_members#ignore_missing DataLaunchdarklyTeamMembers#ignore_missing}.
+        :param emails: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_members#emails DataLaunchdarklyTeamMembers#emails}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_members#id DataLaunchdarklyTeamMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param ignore_missing: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_members#ignore_missing DataLaunchdarklyTeamMembers#ignore_missing}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c3f21dd6b852fbc99de16a75ccb5b53977e93aeed01a891b5de7ba8d9a5ab7f5)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -331,34 +331,34 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def emails(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_members#emails DataLaunchdarklyTeamMembers#emails}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_members#emails DataLaunchdarklyTeamMembers#emails}.'''
         result = self._values.get("emails")
         assert result is not None, "Required property 'emails' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_members#id DataLaunchdarklyTeamMembers#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_members#id DataLaunchdarklyTeamMembers#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ignore_missing(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/team_members#ignore_missing DataLaunchdarklyTeamMembers#ignore_missing}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/team_members#ignore_missing DataLaunchdarklyTeamMembers#ignore_missing}.'''
         result = self._values.get("ignore_missing")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_webhook/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_webhook/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_webhook`
 
-Refer to the Terraform Registry for docs: [`data_launchdarkly_webhook`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/webhook).
+Refer to the Terraform Registry for docs: [`data_launchdarkly_webhook`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/webhook).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class DataLaunchdarklyWebhook(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyWebhook.DataLaunchdarklyWebhook",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/webhook launchdarkly_webhook}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/webhook launchdarkly_webhook}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: builtins.str,
@@ -43,21 +43,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/webhook launchdarkly_webhook} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/webhook launchdarkly_webhook} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: The ID of the webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/webhook#id DataLaunchdarklyWebhook#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/webhook#name DataLaunchdarklyWebhook#name}
-        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/webhook#secret DataLaunchdarklyWebhook#secret}
+        :param id: The ID of the webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/webhook#id DataLaunchdarklyWebhook#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/webhook#name DataLaunchdarklyWebhook#name}
+        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/webhook#secret DataLaunchdarklyWebhook#secret}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +90,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataLaunchdarklyWebhook resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataLaunchdarklyWebhook to import.
-        :param import_from_id: The id of the existing DataLaunchdarklyWebhook that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/webhook#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataLaunchdarklyWebhook that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/webhook#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataLaunchdarklyWebhook to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cc7fc7e8c9f4c4bcb4c8679efa6f0530d7348842e06cfa553b9c7c2fb033f980)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -233,17 +233,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: The ID of the webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/webhook#id DataLaunchdarklyWebhook#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/webhook#name DataLaunchdarklyWebhook#name}
-        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/webhook#secret DataLaunchdarklyWebhook#secret}
+        :param id: The ID of the webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/webhook#id DataLaunchdarklyWebhook#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/webhook#name DataLaunchdarklyWebhook#name}
+        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/webhook#secret DataLaunchdarklyWebhook#secret}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bb8e55aee311f83a83024803098694418c396805f00a0f1c480e08c2c444b0fd)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -341,37 +341,37 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> builtins.str:
         '''The ID of the webhook.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/webhook#id DataLaunchdarklyWebhook#id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/webhook#id DataLaunchdarklyWebhook#id}
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         assert result is not None, "Required property 'id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''A human-readable name for your webhook.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/webhook#name DataLaunchdarklyWebhook#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/webhook#name DataLaunchdarklyWebhook#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def secret(self) -> typing.Optional[builtins.str]:
         '''If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/data-sources/webhook#secret DataLaunchdarklyWebhook#secret}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/data-sources/webhook#secret DataLaunchdarklyWebhook#secret}
         '''
         result = self._values.get("secret")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/destination/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/destination/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_destination`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_destination`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination).
+Refer to the Terraform Registry for docs: [`launchdarkly_destination`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class Destination(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.destination.Destination",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination launchdarkly_destination}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination launchdarkly_destination}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         config: typing.Mapping[builtins.str, builtins.str],
@@ -48,26 +48,26 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination launchdarkly_destination} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination launchdarkly_destination} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param config: The destination-specific configuration. To learn more, read `Destination-Specific Configs <#destination-specific-configs>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#config Destination#config}
-        :param env_key: The environment key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#env_key Destination#env_key}
-        :param kind: The data export destination type. Available choices are ``kinesis``, ``google-pubsub``, ``mparticle``, ``azure-event-hubs``, and ``segment``. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#kind Destination#kind}
-        :param name: A human-readable name for your data export destination. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#name Destination#name}
-        :param project_key: The LaunchDarkly project key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#project_key Destination#project_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#id Destination#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param on: Whether the data export destination is on or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#on Destination#on}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#tags Destination#tags}
+        :param config: The destination-specific configuration. To learn more, read `Destination-Specific Configs <#destination-specific-configs>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#config Destination#config}
+        :param env_key: The environment key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#env_key Destination#env_key}
+        :param kind: The data export destination type. Available choices are ``kinesis``, ``google-pubsub``, ``mparticle``, ``azure-event-hubs``, and ``segment``. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#kind Destination#kind}
+        :param name: A human-readable name for your data export destination. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#name Destination#name}
+        :param project_key: The LaunchDarkly project key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#project_key Destination#project_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#id Destination#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param on: Whether the data export destination is on or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#on Destination#on}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#tags Destination#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -105,15 +105,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Destination resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Destination to import.
-        :param import_from_id: The id of the existing Destination that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Destination that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Destination to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__93b5d67333ceb9ebf407cfb4de25c1a88c0375538c41e7b48e7157625f42d50b)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -334,22 +334,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param config: The destination-specific configuration. To learn more, read `Destination-Specific Configs <#destination-specific-configs>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#config Destination#config}
-        :param env_key: The environment key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#env_key Destination#env_key}
-        :param kind: The data export destination type. Available choices are ``kinesis``, ``google-pubsub``, ``mparticle``, ``azure-event-hubs``, and ``segment``. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#kind Destination#kind}
-        :param name: A human-readable name for your data export destination. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#name Destination#name}
-        :param project_key: The LaunchDarkly project key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#project_key Destination#project_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#id Destination#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param on: Whether the data export destination is on or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#on Destination#on}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#tags Destination#tags}
+        :param config: The destination-specific configuration. To learn more, read `Destination-Specific Configs <#destination-specific-configs>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#config Destination#config}
+        :param env_key: The environment key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#env_key Destination#env_key}
+        :param kind: The data export destination type. Available choices are ``kinesis``, ``google-pubsub``, ``mparticle``, ``azure-event-hubs``, and ``segment``. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#kind Destination#kind}
+        :param name: A human-readable name for your data export destination. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#name Destination#name}
+        :param project_key: The LaunchDarkly project key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#project_key Destination#project_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#id Destination#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param on: Whether the data export destination is on or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#on Destination#on}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#tags Destination#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__466ca569c4ac44df79406165ee289e41c545d765b1fe3b6a01178b89a9ec74e8)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -458,92 +458,92 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def config(self) -> typing.Mapping[builtins.str, builtins.str]:
         '''The destination-specific configuration. To learn more, read `Destination-Specific Configs <#destination-specific-configs>`_.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#config Destination#config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#config Destination#config}
         '''
         result = self._values.get("config")
         assert result is not None, "Required property 'config' is missing"
         return typing.cast(typing.Mapping[builtins.str, builtins.str], result)
 
     @builtins.property
     def env_key(self) -> builtins.str:
         '''The environment key.
 
         A change in this field will force the destruction of the existing resource and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#env_key Destination#env_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#env_key Destination#env_key}
         '''
         result = self._values.get("env_key")
         assert result is not None, "Required property 'env_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def kind(self) -> builtins.str:
         '''The data export destination type.
 
         Available choices are ``kinesis``, ``google-pubsub``, ``mparticle``, ``azure-event-hubs``, and ``segment``. A change in this field will force the destruction of the existing resource and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#kind Destination#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#kind Destination#kind}
         '''
         result = self._values.get("kind")
         assert result is not None, "Required property 'kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''A human-readable name for your data export destination.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#name Destination#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#name Destination#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The LaunchDarkly project key.
 
         A change in this field will force the destruction of the existing resource and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#project_key Destination#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#project_key Destination#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#id Destination#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#id Destination#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def on(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the data export destination is on or not.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#on Destination#on}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#on Destination#on}
         '''
         result = self._values.get("on")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/destination#tags Destination#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/destination#tags Destination#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/environment/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/environment/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_environment`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment).
+Refer to the Terraform Registry for docs: [`launchdarkly_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class Environment(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.environment.Environment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment launchdarkly_environment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment launchdarkly_environment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         color: builtins.str,
@@ -53,31 +53,31 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment launchdarkly_environment} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment launchdarkly_environment} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param color: The color swatch as an RGB hex value with no leading ``#``. For example: ``000000``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#color Environment#color}
-        :param key: The project-unique key for the environment. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#key Environment#key}
-        :param name: The name of the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#name Environment#name}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#project_key Environment#project_key}
-        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#approval_settings Environment#approval_settings}
-        :param confirm_changes: Set to ``true`` if this environment requires confirmation for flag and segment changes. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#confirm_changes Environment#confirm_changes}
-        :param critical: Denotes whether the environment is critical. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#critical Environment#critical}
-        :param default_track_events: Set to ``true`` to enable data export for every flag created in this environment after you configure this argument. This field will default to ``false`` when not set. To learn more, read `Data Export <https://docs.launchdarkly.com/home/data-export>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#default_track_events Environment#default_track_events}
-        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK. This field will default to ``0`` when not set. To learn more, read `TTL settings <https://docs.launchdarkly.com/home/organize/environments#ttl-settings>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#default_ttl Environment#default_ttl}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#id Environment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param require_comments: Set to ``true`` if this environment requires comments for flag and segment changes. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#require_comments Environment#require_comments}
-        :param secure_mode: Set to ``true`` to ensure a user of the client-side SDK cannot impersonate another user. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#secure_mode Environment#secure_mode}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#tags Environment#tags}
+        :param color: The color swatch as an RGB hex value with no leading ``#``. For example: ``000000``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#color Environment#color}
+        :param key: The project-unique key for the environment. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#key Environment#key}
+        :param name: The name of the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#name Environment#name}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#project_key Environment#project_key}
+        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#approval_settings Environment#approval_settings}
+        :param confirm_changes: Set to ``true`` if this environment requires confirmation for flag and segment changes. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#confirm_changes Environment#confirm_changes}
+        :param critical: Denotes whether the environment is critical. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#critical Environment#critical}
+        :param default_track_events: Set to ``true`` to enable data export for every flag created in this environment after you configure this argument. This field will default to ``false`` when not set. To learn more, read `Data Export <https://docs.launchdarkly.com/home/data-export>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#default_track_events Environment#default_track_events}
+        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK. This field will default to ``0`` when not set. To learn more, read `TTL settings <https://docs.launchdarkly.com/home/organize/environments#ttl-settings>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#default_ttl Environment#default_ttl}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#id Environment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param require_comments: Set to ``true`` if this environment requires comments for flag and segment changes. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#require_comments Environment#require_comments}
+        :param secure_mode: Set to ``true`` to ensure a user of the client-side SDK cannot impersonate another user. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#secure_mode Environment#secure_mode}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#tags Environment#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -120,15 +120,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Environment resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Environment to import.
-        :param import_from_id: The id of the existing Environment that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Environment that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Environment to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7b366076fd47c0cd625bd77bfbcfcdd389034a6098566ad233d2747c4b0c7341)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -482,21 +482,21 @@
         min_num_approvals: typing.Optional[jsii.Number] = None,
         required: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         required_approval_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
         service_config: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         service_kind: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param can_apply_declined_changes: Set to ``true`` if changes can be applied as long as the ``min_num_approvals`` is met, regardless of whether any reviewers have declined a request. Defaults to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#can_apply_declined_changes Environment#can_apply_declined_changes}
-        :param can_review_own_request: Set to ``true`` if requesters can approve or decline their own request. They may always comment. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#can_review_own_request Environment#can_review_own_request}
-        :param min_num_approvals: The number of approvals required before an approval request can be applied. This number must be between 1 and 5. Defaults to 1. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#min_num_approvals Environment#min_num_approvals}
-        :param required: Set to ``true`` for changes to flags in this environment to require approval. You may only set ``required`` to true if ``required_approval_tags`` is not set and vice versa. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#required Environment#required}
-        :param required_approval_tags: An array of tags used to specify which flags with those tags require approval. You may only set ``required_approval_tags`` if ``required`` is not set to ``true`` and vice versa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#required_approval_tags Environment#required_approval_tags}
-        :param service_config: The configuration for the service associated with this approval. This is specific to each approval service. For a ``service_kind`` of ``servicenow``, the following fields apply:: - `template` (String) The sys_id of the Standard Change Request Template in ServiceNow that LaunchDarkly will use when creating the change request. - `detail_column` (String) The name of the ServiceNow Change Request column LaunchDarkly uses to populate detailed approval request information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#service_config Environment#service_config}
-        :param service_kind: The kind of service associated with this approval. This determines which platform is used for requesting approval. Valid values are ``servicenow``, ``launchdarkly``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#service_kind Environment#service_kind}
+        :param can_apply_declined_changes: Set to ``true`` if changes can be applied as long as the ``min_num_approvals`` is met, regardless of whether any reviewers have declined a request. Defaults to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#can_apply_declined_changes Environment#can_apply_declined_changes}
+        :param can_review_own_request: Set to ``true`` if requesters can approve or decline their own request. They may always comment. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#can_review_own_request Environment#can_review_own_request}
+        :param min_num_approvals: The number of approvals required before an approval request can be applied. This number must be between 1 and 5. Defaults to 1. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#min_num_approvals Environment#min_num_approvals}
+        :param required: Set to ``true`` for changes to flags in this environment to require approval. You may only set ``required`` to true if ``required_approval_tags`` is not set and vice versa. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#required Environment#required}
+        :param required_approval_tags: An array of tags used to specify which flags with those tags require approval. You may only set ``required_approval_tags`` if ``required`` is not set to ``true`` and vice versa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#required_approval_tags Environment#required_approval_tags}
+        :param service_config: The configuration for the service associated with this approval. This is specific to each approval service. For a ``service_kind`` of ``servicenow``, the following fields apply:: - `template` (String) The sys_id of the Standard Change Request Template in ServiceNow that LaunchDarkly will use when creating the change request. - `detail_column` (String) The name of the ServiceNow Change Request column LaunchDarkly uses to populate detailed approval request information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#service_config Environment#service_config}
+        :param service_kind: The kind of service associated with this approval. This determines which platform is used for requesting approval. Valid values are ``servicenow``, ``launchdarkly``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#service_kind Environment#service_kind}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fde5aff1deb87cd21c5ca5b96f9ed75728472d55dc6c7e315edff7452e2f09dd)
             check_type(argname="argument can_apply_declined_changes", value=can_apply_declined_changes, expected_type=type_hints["can_apply_declined_changes"])
             check_type(argname="argument can_review_own_request", value=can_review_own_request, expected_type=type_hints["can_review_own_request"])
             check_type(argname="argument min_num_approvals", value=min_num_approvals, expected_type=type_hints["min_num_approvals"])
             check_type(argname="argument required", value=required, expected_type=type_hints["required"])
@@ -523,61 +523,61 @@
     def can_apply_declined_changes(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set to ``true`` if changes can be applied as long as the ``min_num_approvals`` is met, regardless of whether any reviewers have declined a request.
 
         Defaults to ``true``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#can_apply_declined_changes Environment#can_apply_declined_changes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#can_apply_declined_changes Environment#can_apply_declined_changes}
         '''
         result = self._values.get("can_apply_declined_changes")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def can_review_own_request(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set to ``true`` if requesters can approve or decline their own request. They may always comment. Defaults to ``false``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#can_review_own_request Environment#can_review_own_request}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#can_review_own_request Environment#can_review_own_request}
         '''
         result = self._values.get("can_review_own_request")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def min_num_approvals(self) -> typing.Optional[jsii.Number]:
         '''The number of approvals required before an approval request can be applied.
 
         This number must be between 1 and 5. Defaults to 1.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#min_num_approvals Environment#min_num_approvals}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#min_num_approvals Environment#min_num_approvals}
         '''
         result = self._values.get("min_num_approvals")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def required(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set to ``true`` for changes to flags in this environment to require approval.
 
         You may only set ``required`` to true if ``required_approval_tags`` is not set and vice versa. Defaults to ``false``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#required Environment#required}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#required Environment#required}
         '''
         result = self._values.get("required")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def required_approval_tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''An array of tags used to specify which flags with those tags require approval.
 
         You may only set ``required_approval_tags`` if ``required`` is not set to ``true`` and vice versa.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#required_approval_tags Environment#required_approval_tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#required_approval_tags Environment#required_approval_tags}
         '''
         result = self._values.get("required_approval_tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def service_config(
         self,
@@ -585,26 +585,26 @@
         '''The configuration for the service associated with this approval.
 
         This is specific to each approval service. For a ``service_kind`` of ``servicenow``, the following fields apply::
 
             - `template` (String) The sys_id of the Standard Change Request Template in ServiceNow that LaunchDarkly will use when creating the change request.
             - `detail_column` (String) The name of the ServiceNow Change Request column LaunchDarkly uses to populate detailed approval request information.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#service_config Environment#service_config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#service_config Environment#service_config}
         '''
         result = self._values.get("service_config")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def service_kind(self) -> typing.Optional[builtins.str]:
         '''The kind of service associated with this approval.
 
         This determines which platform is used for requesting approval. Valid values are ``servicenow``, ``launchdarkly``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#service_kind Environment#service_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#service_kind Environment#service_kind}
         '''
         result = self._values.get("service_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -976,27 +976,27 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param color: The color swatch as an RGB hex value with no leading ``#``. For example: ``000000``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#color Environment#color}
-        :param key: The project-unique key for the environment. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#key Environment#key}
-        :param name: The name of the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#name Environment#name}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#project_key Environment#project_key}
-        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#approval_settings Environment#approval_settings}
-        :param confirm_changes: Set to ``true`` if this environment requires confirmation for flag and segment changes. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#confirm_changes Environment#confirm_changes}
-        :param critical: Denotes whether the environment is critical. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#critical Environment#critical}
-        :param default_track_events: Set to ``true`` to enable data export for every flag created in this environment after you configure this argument. This field will default to ``false`` when not set. To learn more, read `Data Export <https://docs.launchdarkly.com/home/data-export>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#default_track_events Environment#default_track_events}
-        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK. This field will default to ``0`` when not set. To learn more, read `TTL settings <https://docs.launchdarkly.com/home/organize/environments#ttl-settings>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#default_ttl Environment#default_ttl}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#id Environment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param require_comments: Set to ``true`` if this environment requires comments for flag and segment changes. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#require_comments Environment#require_comments}
-        :param secure_mode: Set to ``true`` to ensure a user of the client-side SDK cannot impersonate another user. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#secure_mode Environment#secure_mode}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#tags Environment#tags}
+        :param color: The color swatch as an RGB hex value with no leading ``#``. For example: ``000000``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#color Environment#color}
+        :param key: The project-unique key for the environment. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#key Environment#key}
+        :param name: The name of the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#name Environment#name}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#project_key Environment#project_key}
+        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#approval_settings Environment#approval_settings}
+        :param confirm_changes: Set to ``true`` if this environment requires confirmation for flag and segment changes. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#confirm_changes Environment#confirm_changes}
+        :param critical: Denotes whether the environment is critical. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#critical Environment#critical}
+        :param default_track_events: Set to ``true`` to enable data export for every flag created in this environment after you configure this argument. This field will default to ``false`` when not set. To learn more, read `Data Export <https://docs.launchdarkly.com/home/data-export>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#default_track_events Environment#default_track_events}
+        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK. This field will default to ``0`` when not set. To learn more, read `TTL settings <https://docs.launchdarkly.com/home/organize/environments#ttl-settings>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#default_ttl Environment#default_ttl}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#id Environment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param require_comments: Set to ``true`` if this environment requires comments for flag and segment changes. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#require_comments Environment#require_comments}
+        :param secure_mode: Set to ``true`` to ensure a user of the client-side SDK cannot impersonate another user. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#secure_mode Environment#secure_mode}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#tags Environment#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6e0608c2d3a8c4886786970a153e9cd6eadb59d4a6053f51e829a03f3de98831)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -1121,114 +1121,114 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def color(self) -> builtins.str:
         '''The color swatch as an RGB hex value with no leading ``#``. For example: ``000000``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#color Environment#color}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#color Environment#color}
         '''
         result = self._values.get("color")
         assert result is not None, "Required property 'color' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The project-unique key for the environment.
 
         A change in this field will force the destruction of the existing resource and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#key Environment#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#key Environment#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#name Environment#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#name Environment#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The LaunchDarkly project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#project_key Environment#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#project_key Environment#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def approval_settings(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[EnvironmentApprovalSettings]]]:
         '''approval_settings block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#approval_settings Environment#approval_settings}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#approval_settings Environment#approval_settings}
         '''
         result = self._values.get("approval_settings")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[EnvironmentApprovalSettings]]], result)
 
     @builtins.property
     def confirm_changes(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set to ``true`` if this environment requires confirmation for flag and segment changes.
 
         This field will default to ``false`` when not set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#confirm_changes Environment#confirm_changes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#confirm_changes Environment#confirm_changes}
         '''
         result = self._values.get("confirm_changes")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def critical(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Denotes whether the environment is critical.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#critical Environment#critical}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#critical Environment#critical}
         '''
         result = self._values.get("critical")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def default_track_events(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set to ``true`` to enable data export for every flag created in this environment after you configure this argument.
 
         This field will default to ``false`` when not set. To learn more, read `Data Export <https://docs.launchdarkly.com/home/data-export>`_.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#default_track_events Environment#default_track_events}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#default_track_events Environment#default_track_events}
         '''
         result = self._values.get("default_track_events")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def default_ttl(self) -> typing.Optional[jsii.Number]:
         '''The TTL for the environment.
 
         This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK. This field will default to ``0`` when not set. To learn more, read `TTL settings <https://docs.launchdarkly.com/home/organize/environments#ttl-settings>`_.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#default_ttl Environment#default_ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#default_ttl Environment#default_ttl}
         '''
         result = self._values.get("default_ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#id Environment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#id Environment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -1236,37 +1236,37 @@
     def require_comments(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set to ``true`` if this environment requires comments for flag and segment changes.
 
         This field will default to ``false`` when not set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#require_comments Environment#require_comments}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#require_comments Environment#require_comments}
         '''
         result = self._values.get("require_comments")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def secure_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set to ``true`` to ensure a user of the client-side SDK cannot impersonate another user.
 
         This field will default to ``false`` when not set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#secure_mode Environment#secure_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#secure_mode Environment#secure_mode}
         '''
         result = self._values.get("secure_mode")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/environment#tags Environment#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/environment#tags Environment#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/feature_flag/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/feature_flag/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_feature_flag`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_feature_flag`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag).
+Refer to the Terraform Registry for docs: [`launchdarkly_feature_flag`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class FeatureFlag(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.featureFlag.FeatureFlag",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag launchdarkly_feature_flag}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag launchdarkly_feature_flag}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -56,34 +56,34 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag launchdarkly_feature_flag} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag launchdarkly_feature_flag} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: The unique feature flag key that references the flag in your application code. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#key FeatureFlag#key}
-        :param name: The human-readable name of the feature flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#name FeatureFlag#name}
-        :param project_key: The feature flag's project key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#project_key FeatureFlag#project_key}
-        :param variation_type: The feature flag's variation type: ``boolean``, ``string``, ``number`` or ``json``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#variation_type FeatureFlag#variation_type}
-        :param archived: Specifies whether the flag is archived or not. Note that you cannot create a new flag that is archived, but can update a flag to be archived. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#archived FeatureFlag#archived}
-        :param client_side_availability: client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#client_side_availability FeatureFlag#client_side_availability}
-        :param custom_properties: custom_properties block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#custom_properties FeatureFlag#custom_properties}
-        :param defaults: defaults block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#defaults FeatureFlag#defaults}
-        :param description: The feature flag's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#description FeatureFlag#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#id FeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param include_in_snippet: Specifies whether this flag should be made available to the client-side JavaScript SDK using the client-side Id. This value gets its default from your project configuration if not set. ``include_in_snippet`` is now deprecated. Please migrate to ``client_side_availability.using_environment_id`` to maintain future compatibility. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#include_in_snippet FeatureFlag#include_in_snippet}
-        :param maintainer_id: The feature flag maintainer's 24 character alphanumeric team member ID. ``maintainer_team_key`` cannot be set if ``maintainer_id`` is set. If neither is set, it will automatically be or stay set to the member ID associated with the API key used by your LaunchDarkly Terraform provider or the most recently-set maintainer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#maintainer_id FeatureFlag#maintainer_id}
-        :param maintainer_team_key: The key of the associated team that maintains this feature flag. ``maintainer_id`` cannot be set if ``maintainer_team_key`` is set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#maintainer_team_key FeatureFlag#maintainer_team_key}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#tags FeatureFlag#tags}
-        :param temporary: Specifies whether the flag is a temporary flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#temporary FeatureFlag#temporary}
-        :param variations: variations block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#variations FeatureFlag#variations}
+        :param key: The unique feature flag key that references the flag in your application code. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#key FeatureFlag#key}
+        :param name: The human-readable name of the feature flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#name FeatureFlag#name}
+        :param project_key: The feature flag's project key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#project_key FeatureFlag#project_key}
+        :param variation_type: The feature flag's variation type: ``boolean``, ``string``, ``number`` or ``json``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#variation_type FeatureFlag#variation_type}
+        :param archived: Specifies whether the flag is archived or not. Note that you cannot create a new flag that is archived, but can update a flag to be archived. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#archived FeatureFlag#archived}
+        :param client_side_availability: client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#client_side_availability FeatureFlag#client_side_availability}
+        :param custom_properties: custom_properties block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#custom_properties FeatureFlag#custom_properties}
+        :param defaults: defaults block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#defaults FeatureFlag#defaults}
+        :param description: The feature flag's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#description FeatureFlag#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#id FeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param include_in_snippet: Specifies whether this flag should be made available to the client-side JavaScript SDK using the client-side Id. This value gets its default from your project configuration if not set. ``include_in_snippet`` is now deprecated. Please migrate to ``client_side_availability.using_environment_id`` to maintain future compatibility. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#include_in_snippet FeatureFlag#include_in_snippet}
+        :param maintainer_id: The feature flag maintainer's 24 character alphanumeric team member ID. ``maintainer_team_key`` cannot be set if ``maintainer_id`` is set. If neither is set, it will automatically be or stay set to the member ID associated with the API key used by your LaunchDarkly Terraform provider or the most recently-set maintainer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#maintainer_id FeatureFlag#maintainer_id}
+        :param maintainer_team_key: The key of the associated team that maintains this feature flag. ``maintainer_id`` cannot be set if ``maintainer_team_key`` is set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#maintainer_team_key FeatureFlag#maintainer_team_key}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#tags FeatureFlag#tags}
+        :param temporary: Specifies whether the flag is a temporary flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#temporary FeatureFlag#temporary}
+        :param variations: variations block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#variations FeatureFlag#variations}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -129,15 +129,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a FeatureFlag resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the FeatureFlag to import.
-        :param import_from_id: The id of the existing FeatureFlag that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing FeatureFlag that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the FeatureFlag to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5075f99da43d9aef24ceec35d6ff3e03dab34b8317782168617947b4b1b142d1)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -174,16 +174,16 @@
     def put_defaults(
         self,
         *,
         off_variation: jsii.Number,
         on_variation: jsii.Number,
     ) -> None:
         '''
-        :param off_variation: The index of the variation the flag will default to in all new environments when off. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#off_variation FeatureFlag#off_variation}
-        :param on_variation: The index of the variation the flag will default to in all new environments when on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#on_variation FeatureFlag#on_variation}
+        :param off_variation: The index of the variation the flag will default to in all new environments when off. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#off_variation FeatureFlag#off_variation}
+        :param on_variation: The index of the variation the flag will default to in all new environments when on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#on_variation FeatureFlag#on_variation}
         '''
         value = FeatureFlagDefaults(
             off_variation=off_variation, on_variation=on_variation
         )
 
         return typing.cast(None, jsii.invoke(self, "putDefaults", [value]))
 
@@ -541,16 +541,16 @@
     def __init__(
         self,
         *,
         using_environment_id: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         using_mobile_key: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     ) -> None:
         '''
-        :param using_environment_id: Whether this flag is available to SDKs using the client-side ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#using_environment_id FeatureFlag#using_environment_id}
-        :param using_mobile_key: Whether this flag is available to SDKs using a mobile key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#using_mobile_key FeatureFlag#using_mobile_key}
+        :param using_environment_id: Whether this flag is available to SDKs using the client-side ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#using_environment_id FeatureFlag#using_environment_id}
+        :param using_mobile_key: Whether this flag is available to SDKs using a mobile key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#using_mobile_key FeatureFlag#using_mobile_key}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__07f14cdaea6f10e022a6d396c287ff71ccbe0531800c60eed40fcce76ed2098e)
             check_type(argname="argument using_environment_id", value=using_environment_id, expected_type=type_hints["using_environment_id"])
             check_type(argname="argument using_mobile_key", value=using_mobile_key, expected_type=type_hints["using_mobile_key"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if using_environment_id is not None:
@@ -560,26 +560,26 @@
 
     @builtins.property
     def using_environment_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether this flag is available to SDKs using the client-side ID.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#using_environment_id FeatureFlag#using_environment_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#using_environment_id FeatureFlag#using_environment_id}
         '''
         result = self._values.get("using_environment_id")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def using_mobile_key(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether this flag is available to SDKs using a mobile key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#using_mobile_key FeatureFlag#using_mobile_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#using_mobile_key FeatureFlag#using_mobile_key}
         '''
         result = self._values.get("using_mobile_key")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -846,30 +846,30 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: The unique feature flag key that references the flag in your application code. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#key FeatureFlag#key}
-        :param name: The human-readable name of the feature flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#name FeatureFlag#name}
-        :param project_key: The feature flag's project key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#project_key FeatureFlag#project_key}
-        :param variation_type: The feature flag's variation type: ``boolean``, ``string``, ``number`` or ``json``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#variation_type FeatureFlag#variation_type}
-        :param archived: Specifies whether the flag is archived or not. Note that you cannot create a new flag that is archived, but can update a flag to be archived. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#archived FeatureFlag#archived}
-        :param client_side_availability: client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#client_side_availability FeatureFlag#client_side_availability}
-        :param custom_properties: custom_properties block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#custom_properties FeatureFlag#custom_properties}
-        :param defaults: defaults block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#defaults FeatureFlag#defaults}
-        :param description: The feature flag's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#description FeatureFlag#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#id FeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param include_in_snippet: Specifies whether this flag should be made available to the client-side JavaScript SDK using the client-side Id. This value gets its default from your project configuration if not set. ``include_in_snippet`` is now deprecated. Please migrate to ``client_side_availability.using_environment_id`` to maintain future compatibility. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#include_in_snippet FeatureFlag#include_in_snippet}
-        :param maintainer_id: The feature flag maintainer's 24 character alphanumeric team member ID. ``maintainer_team_key`` cannot be set if ``maintainer_id`` is set. If neither is set, it will automatically be or stay set to the member ID associated with the API key used by your LaunchDarkly Terraform provider or the most recently-set maintainer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#maintainer_id FeatureFlag#maintainer_id}
-        :param maintainer_team_key: The key of the associated team that maintains this feature flag. ``maintainer_id`` cannot be set if ``maintainer_team_key`` is set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#maintainer_team_key FeatureFlag#maintainer_team_key}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#tags FeatureFlag#tags}
-        :param temporary: Specifies whether the flag is a temporary flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#temporary FeatureFlag#temporary}
-        :param variations: variations block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#variations FeatureFlag#variations}
+        :param key: The unique feature flag key that references the flag in your application code. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#key FeatureFlag#key}
+        :param name: The human-readable name of the feature flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#name FeatureFlag#name}
+        :param project_key: The feature flag's project key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#project_key FeatureFlag#project_key}
+        :param variation_type: The feature flag's variation type: ``boolean``, ``string``, ``number`` or ``json``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#variation_type FeatureFlag#variation_type}
+        :param archived: Specifies whether the flag is archived or not. Note that you cannot create a new flag that is archived, but can update a flag to be archived. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#archived FeatureFlag#archived}
+        :param client_side_availability: client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#client_side_availability FeatureFlag#client_side_availability}
+        :param custom_properties: custom_properties block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#custom_properties FeatureFlag#custom_properties}
+        :param defaults: defaults block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#defaults FeatureFlag#defaults}
+        :param description: The feature flag's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#description FeatureFlag#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#id FeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param include_in_snippet: Specifies whether this flag should be made available to the client-side JavaScript SDK using the client-side Id. This value gets its default from your project configuration if not set. ``include_in_snippet`` is now deprecated. Please migrate to ``client_side_availability.using_environment_id`` to maintain future compatibility. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#include_in_snippet FeatureFlag#include_in_snippet}
+        :param maintainer_id: The feature flag maintainer's 24 character alphanumeric team member ID. ``maintainer_team_key`` cannot be set if ``maintainer_id`` is set. If neither is set, it will automatically be or stay set to the member ID associated with the API key used by your LaunchDarkly Terraform provider or the most recently-set maintainer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#maintainer_id FeatureFlag#maintainer_id}
+        :param maintainer_team_key: The key of the associated team that maintains this feature flag. ``maintainer_id`` cannot be set if ``maintainer_team_key`` is set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#maintainer_team_key FeatureFlag#maintainer_team_key}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#tags FeatureFlag#tags}
+        :param temporary: Specifies whether the flag is a temporary flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#temporary FeatureFlag#temporary}
+        :param variations: variations block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#variations FeatureFlag#variations}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(defaults, dict):
             defaults = FeatureFlagDefaults(**defaults)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a2b024440d957862712c9755f97389f4b688ffe513bf440a776f2367528a7e9f)
@@ -1007,108 +1007,108 @@
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The unique feature flag key that references the flag in your application code.
 
         A change in this field will force the destruction of the existing resource and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#key FeatureFlag#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#key FeatureFlag#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The human-readable name of the feature flag.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#name FeatureFlag#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#name FeatureFlag#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The feature flag's project key.
 
         A change in this field will force the destruction of the existing resource and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#project_key FeatureFlag#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#project_key FeatureFlag#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def variation_type(self) -> builtins.str:
         '''The feature flag's variation type: ``boolean``, ``string``, ``number`` or ``json``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#variation_type FeatureFlag#variation_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#variation_type FeatureFlag#variation_type}
         '''
         result = self._values.get("variation_type")
         assert result is not None, "Required property 'variation_type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def archived(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Specifies whether the flag is archived or not.
 
         Note that you cannot create a new flag that is archived, but can update a flag to be archived.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#archived FeatureFlag#archived}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#archived FeatureFlag#archived}
         '''
         result = self._values.get("archived")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def client_side_availability(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[FeatureFlagClientSideAvailability]]]:
         '''client_side_availability block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#client_side_availability FeatureFlag#client_side_availability}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#client_side_availability FeatureFlag#client_side_availability}
         '''
         result = self._values.get("client_side_availability")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[FeatureFlagClientSideAvailability]]], result)
 
     @builtins.property
     def custom_properties(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagCustomProperties"]]]:
         '''custom_properties block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#custom_properties FeatureFlag#custom_properties}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#custom_properties FeatureFlag#custom_properties}
         '''
         result = self._values.get("custom_properties")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagCustomProperties"]]], result)
 
     @builtins.property
     def defaults(self) -> typing.Optional["FeatureFlagDefaults"]:
         '''defaults block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#defaults FeatureFlag#defaults}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#defaults FeatureFlag#defaults}
         '''
         result = self._values.get("defaults")
         return typing.cast(typing.Optional["FeatureFlagDefaults"], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The feature flag's description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#description FeatureFlag#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#description FeatureFlag#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#id FeatureFlag#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#id FeatureFlag#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -1116,66 +1116,66 @@
     def include_in_snippet(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Specifies whether this flag should be made available to the client-side JavaScript SDK using the client-side Id.
 
         This value gets its default from your project configuration if not set. ``include_in_snippet`` is now deprecated. Please migrate to ``client_side_availability.using_environment_id`` to maintain future compatibility.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#include_in_snippet FeatureFlag#include_in_snippet}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#include_in_snippet FeatureFlag#include_in_snippet}
         '''
         result = self._values.get("include_in_snippet")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def maintainer_id(self) -> typing.Optional[builtins.str]:
         '''The feature flag maintainer's 24 character alphanumeric team member ID.
 
         ``maintainer_team_key`` cannot be set if ``maintainer_id`` is set. If neither is set, it will automatically be or stay set to the member ID associated with the API key used by your LaunchDarkly Terraform provider or the most recently-set maintainer.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#maintainer_id FeatureFlag#maintainer_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#maintainer_id FeatureFlag#maintainer_id}
         '''
         result = self._values.get("maintainer_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def maintainer_team_key(self) -> typing.Optional[builtins.str]:
         '''The key of the associated team that maintains this feature flag. ``maintainer_id`` cannot be set if ``maintainer_team_key`` is set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#maintainer_team_key FeatureFlag#maintainer_team_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#maintainer_team_key FeatureFlag#maintainer_team_key}
         '''
         result = self._values.get("maintainer_team_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#tags FeatureFlag#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#tags FeatureFlag#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def temporary(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Specifies whether the flag is a temporary flag.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#temporary FeatureFlag#temporary}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#temporary FeatureFlag#temporary}
         '''
         result = self._values.get("temporary")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def variations(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagVariations"]]]:
         '''variations block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#variations FeatureFlag#variations}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#variations FeatureFlag#variations}
         '''
         result = self._values.get("variations")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagVariations"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1198,17 +1198,17 @@
         self,
         *,
         key: builtins.str,
         name: builtins.str,
         value: typing.Sequence[builtins.str],
     ) -> None:
         '''
-        :param key: The unique custom property key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#key FeatureFlag#key}
-        :param name: The name of the custom property. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#name FeatureFlag#name}
-        :param value: The list of custom property value strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#value FeatureFlag#value}
+        :param key: The unique custom property key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#key FeatureFlag#key}
+        :param name: The name of the custom property. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#name FeatureFlag#name}
+        :param value: The list of custom property value strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#value FeatureFlag#value}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c7766b6ff19cff676147d8e598ddf37d57f59672f44b15e80616fff490f0023e)
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -1217,35 +1217,35 @@
             "value": value,
         }
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The unique custom property key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#key FeatureFlag#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#key FeatureFlag#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the custom property.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#name FeatureFlag#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#name FeatureFlag#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def value(self) -> typing.List[builtins.str]:
         '''The list of custom property value strings.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#value FeatureFlag#value}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#value FeatureFlag#value}
         '''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1453,41 +1453,41 @@
     def __init__(
         self,
         *,
         off_variation: jsii.Number,
         on_variation: jsii.Number,
     ) -> None:
         '''
-        :param off_variation: The index of the variation the flag will default to in all new environments when off. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#off_variation FeatureFlag#off_variation}
-        :param on_variation: The index of the variation the flag will default to in all new environments when on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#on_variation FeatureFlag#on_variation}
+        :param off_variation: The index of the variation the flag will default to in all new environments when off. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#off_variation FeatureFlag#off_variation}
+        :param on_variation: The index of the variation the flag will default to in all new environments when on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#on_variation FeatureFlag#on_variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2c66a4687bbd5a78f091fc125765bf2a56a6b71c8a235252b256684c9a8aa2f1)
             check_type(argname="argument off_variation", value=off_variation, expected_type=type_hints["off_variation"])
             check_type(argname="argument on_variation", value=on_variation, expected_type=type_hints["on_variation"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "off_variation": off_variation,
             "on_variation": on_variation,
         }
 
     @builtins.property
     def off_variation(self) -> jsii.Number:
         '''The index of the variation the flag will default to in all new environments when off.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#off_variation FeatureFlag#off_variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#off_variation FeatureFlag#off_variation}
         '''
         result = self._values.get("off_variation")
         assert result is not None, "Required property 'off_variation' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def on_variation(self) -> jsii.Number:
         '''The index of the variation the flag will default to in all new environments when on.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#on_variation FeatureFlag#on_variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#on_variation FeatureFlag#on_variation}
         '''
         result = self._values.get("on_variation")
         assert result is not None, "Required property 'on_variation' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1578,17 +1578,17 @@
         self,
         *,
         value: builtins.str,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param value: The variation value. The value's type must correspond to the ``variation_type`` argument. For example: ``variation_type = "boolean"`` accepts only ``true`` or ``false``. The ``number`` variation type accepts both floats and ints, but please note that any trailing zeroes on floats will be trimmed (i.e. ``1.1`` and ``1.100`` will both be converted to ``1.1``). If you wish to define an empty string variation, you must still define the value field on the variations block like so:: variations { value = "" } Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#value FeatureFlag#value}
-        :param description: The variation's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#description FeatureFlag#description}
-        :param name: The name of the variation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#name FeatureFlag#name}
+        :param value: The variation value. The value's type must correspond to the ``variation_type`` argument. For example: ``variation_type = "boolean"`` accepts only ``true`` or ``false``. The ``number`` variation type accepts both floats and ints, but please note that any trailing zeroes on floats will be trimmed (i.e. ``1.1`` and ``1.100`` will both be converted to ``1.1``). If you wish to define an empty string variation, you must still define the value field on the variations block like so:: variations { value = "" } Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#value FeatureFlag#value}
+        :param description: The variation's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#description FeatureFlag#description}
+        :param name: The name of the variation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#name FeatureFlag#name}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__190f28e6db25553ffb3b995e566038ac05cac527b1eb46d2227cd70af5c912fa)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -1607,34 +1607,34 @@
 
         If you wish to define an empty string variation, you must still define the value field on the variations block like so::
 
            variations {
              value = ""
            }
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#value FeatureFlag#value}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#value FeatureFlag#value}
         '''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The variation's description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#description FeatureFlag#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#description FeatureFlag#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The name of the variation.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag#name FeatureFlag#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag#name FeatureFlag#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/feature_flag_environment/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/feature_flag_environment/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_feature_flag_environment`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_feature_flag_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment).
+Refer to the Terraform Registry for docs: [`launchdarkly_feature_flag_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class FeatureFlagEnvironment(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.featureFlagEnvironment.FeatureFlagEnvironment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment launchdarkly_feature_flag_environment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment launchdarkly_feature_flag_environment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         env_key: builtins.str,
@@ -51,29 +51,29 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment launchdarkly_feature_flag_environment} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment launchdarkly_feature_flag_environment} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param env_key: The environment key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#env_key FeatureFlagEnvironment#env_key}
-        :param fallthrough: fallthrough block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#fallthrough FeatureFlagEnvironment#fallthrough}
-        :param flag_id: The feature flag's unique ``id`` in the format ``project_key/flag_key``. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#flag_id FeatureFlagEnvironment#flag_id}
-        :param off_variation: The index of the variation to serve if targeting is disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#off_variation FeatureFlagEnvironment#off_variation}
-        :param context_targets: context_targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#context_targets FeatureFlagEnvironment#context_targets}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#id FeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param on: Whether targeting is enabled. Defaults to ``false`` if not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#on FeatureFlagEnvironment#on}
-        :param prerequisites: prerequisites block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#prerequisites FeatureFlagEnvironment#prerequisites}
-        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#rules FeatureFlagEnvironment#rules}
-        :param targets: targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#targets FeatureFlagEnvironment#targets}
-        :param track_events: Whether to send event data back to LaunchDarkly. Defaults to ``false`` if not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#track_events FeatureFlagEnvironment#track_events}
+        :param env_key: The environment key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#env_key FeatureFlagEnvironment#env_key}
+        :param fallthrough: fallthrough block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#fallthrough FeatureFlagEnvironment#fallthrough}
+        :param flag_id: The feature flag's unique ``id`` in the format ``project_key/flag_key``. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#flag_id FeatureFlagEnvironment#flag_id}
+        :param off_variation: The index of the variation to serve if targeting is disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#off_variation FeatureFlagEnvironment#off_variation}
+        :param context_targets: context_targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#context_targets FeatureFlagEnvironment#context_targets}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#id FeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param on: Whether targeting is enabled. Defaults to ``false`` if not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#on FeatureFlagEnvironment#on}
+        :param prerequisites: prerequisites block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#prerequisites FeatureFlagEnvironment#prerequisites}
+        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#rules FeatureFlagEnvironment#rules}
+        :param targets: targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#targets FeatureFlagEnvironment#targets}
+        :param track_events: Whether to send event data back to LaunchDarkly. Defaults to ``false`` if not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#track_events FeatureFlagEnvironment#track_events}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -114,15 +114,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a FeatureFlagEnvironment resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the FeatureFlagEnvironment to import.
-        :param import_from_id: The id of the existing FeatureFlagEnvironment that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing FeatureFlagEnvironment that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the FeatureFlagEnvironment to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f298d44f2c9d889c80ebdfd75b63176802aab1902827bcbd69fc9cc192e5c4fd)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -148,18 +148,18 @@
         *,
         bucket_by: typing.Optional[builtins.str] = None,
         context_kind: typing.Optional[builtins.str] = None,
         rollout_weights: typing.Optional[typing.Sequence[jsii.Number]] = None,
         variation: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
-        :param context_kind: The context kind associated with the specified rollout. This argument is only valid if rollout_weights is also specified. If omitted, defaults to ``user``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
-        :param rollout_weights: List of integer percentage rollout weights (in thousandths of a percent) to apply to each variation if the rule clauses evaluates to ``true``. The sum of the ``rollout_weights`` must equal 100000 and the number of rollout weights specified in the array must match the number of flag variations. You must specify either ``variation`` or ``rollout_weights``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}
-        :param variation: The default integer variation index to serve if no ``prerequisites``, ``target``, or ``rules`` apply. You must specify either ``variation`` or ``rollout_weights``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
+        :param context_kind: The context kind associated with the specified rollout. This argument is only valid if rollout_weights is also specified. If omitted, defaults to ``user``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
+        :param rollout_weights: List of integer percentage rollout weights (in thousandths of a percent) to apply to each variation if the rule clauses evaluates to ``true``. The sum of the ``rollout_weights`` must equal 100000 and the number of rollout weights specified in the array must match the number of flag variations. You must specify either ``variation`` or ``rollout_weights``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}
+        :param variation: The default integer variation index to serve if no ``prerequisites``, ``target``, or ``rules`` apply. You must specify either ``variation`` or ``rollout_weights``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         value = FeatureFlagEnvironmentFallthrough(
             bucket_by=bucket_by,
             context_kind=context_kind,
             rollout_weights=rollout_weights,
             variation=variation,
         )
@@ -468,25 +468,25 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param env_key: The environment key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#env_key FeatureFlagEnvironment#env_key}
-        :param fallthrough: fallthrough block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#fallthrough FeatureFlagEnvironment#fallthrough}
-        :param flag_id: The feature flag's unique ``id`` in the format ``project_key/flag_key``. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#flag_id FeatureFlagEnvironment#flag_id}
-        :param off_variation: The index of the variation to serve if targeting is disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#off_variation FeatureFlagEnvironment#off_variation}
-        :param context_targets: context_targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#context_targets FeatureFlagEnvironment#context_targets}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#id FeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param on: Whether targeting is enabled. Defaults to ``false`` if not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#on FeatureFlagEnvironment#on}
-        :param prerequisites: prerequisites block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#prerequisites FeatureFlagEnvironment#prerequisites}
-        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#rules FeatureFlagEnvironment#rules}
-        :param targets: targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#targets FeatureFlagEnvironment#targets}
-        :param track_events: Whether to send event data back to LaunchDarkly. Defaults to ``false`` if not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#track_events FeatureFlagEnvironment#track_events}
+        :param env_key: The environment key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#env_key FeatureFlagEnvironment#env_key}
+        :param fallthrough: fallthrough block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#fallthrough FeatureFlagEnvironment#fallthrough}
+        :param flag_id: The feature flag's unique ``id`` in the format ``project_key/flag_key``. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#flag_id FeatureFlagEnvironment#flag_id}
+        :param off_variation: The index of the variation to serve if targeting is disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#off_variation FeatureFlagEnvironment#off_variation}
+        :param context_targets: context_targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#context_targets FeatureFlagEnvironment#context_targets}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#id FeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param on: Whether targeting is enabled. Defaults to ``false`` if not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#on FeatureFlagEnvironment#on}
+        :param prerequisites: prerequisites block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#prerequisites FeatureFlagEnvironment#prerequisites}
+        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#rules FeatureFlagEnvironment#rules}
+        :param targets: targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#targets FeatureFlagEnvironment#targets}
+        :param track_events: Whether to send event data back to LaunchDarkly. Defaults to ``false`` if not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#track_events FeatureFlagEnvironment#track_events}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(fallthrough, dict):
             fallthrough = FeatureFlagEnvironmentFallthrough(**fallthrough)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7906af57752c788e0f057973f44c65cc16cb2d8bdf337d01f76caefb9503b806)
@@ -609,124 +609,124 @@
 
     @builtins.property
     def env_key(self) -> builtins.str:
         '''The environment key.
 
         A change in this field will force the destruction of the existing resource and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#env_key FeatureFlagEnvironment#env_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#env_key FeatureFlagEnvironment#env_key}
         '''
         result = self._values.get("env_key")
         assert result is not None, "Required property 'env_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def fallthrough(self) -> "FeatureFlagEnvironmentFallthrough":
         '''fallthrough block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#fallthrough FeatureFlagEnvironment#fallthrough}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#fallthrough FeatureFlagEnvironment#fallthrough}
         '''
         result = self._values.get("fallthrough")
         assert result is not None, "Required property 'fallthrough' is missing"
         return typing.cast("FeatureFlagEnvironmentFallthrough", result)
 
     @builtins.property
     def flag_id(self) -> builtins.str:
         '''The feature flag's unique ``id`` in the format ``project_key/flag_key``.
 
         A change in this field will force the destruction of the existing resource and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#flag_id FeatureFlagEnvironment#flag_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#flag_id FeatureFlagEnvironment#flag_id}
         '''
         result = self._values.get("flag_id")
         assert result is not None, "Required property 'flag_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def off_variation(self) -> jsii.Number:
         '''The index of the variation to serve if targeting is disabled.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#off_variation FeatureFlagEnvironment#off_variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#off_variation FeatureFlagEnvironment#off_variation}
         '''
         result = self._values.get("off_variation")
         assert result is not None, "Required property 'off_variation' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def context_targets(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentContextTargets"]]]:
         '''context_targets block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#context_targets FeatureFlagEnvironment#context_targets}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#context_targets FeatureFlagEnvironment#context_targets}
         '''
         result = self._values.get("context_targets")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentContextTargets"]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#id FeatureFlagEnvironment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#id FeatureFlagEnvironment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def on(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether targeting is enabled. Defaults to ``false`` if not set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#on FeatureFlagEnvironment#on}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#on FeatureFlagEnvironment#on}
         '''
         result = self._values.get("on")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def prerequisites(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentPrerequisites"]]]:
         '''prerequisites block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#prerequisites FeatureFlagEnvironment#prerequisites}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#prerequisites FeatureFlagEnvironment#prerequisites}
         '''
         result = self._values.get("prerequisites")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentPrerequisites"]]], result)
 
     @builtins.property
     def rules(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentRules"]]]:
         '''rules block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#rules FeatureFlagEnvironment#rules}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#rules FeatureFlagEnvironment#rules}
         '''
         result = self._values.get("rules")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentRules"]]], result)
 
     @builtins.property
     def targets(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentTargets"]]]:
         '''targets block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#targets FeatureFlagEnvironment#targets}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#targets FeatureFlagEnvironment#targets}
         '''
         result = self._values.get("targets")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentTargets"]]], result)
 
     @builtins.property
     def track_events(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether to send event data back to LaunchDarkly. Defaults to ``false`` if not set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#track_events FeatureFlagEnvironment#track_events}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#track_events FeatureFlagEnvironment#track_events}
         '''
         result = self._values.get("track_events")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -753,17 +753,17 @@
         self,
         *,
         context_kind: builtins.str,
         values: typing.Sequence[builtins.str],
         variation: jsii.Number,
     ) -> None:
         '''
-        :param context_kind: The context kind on which the flag should target in this environment. User (``user``) targets should be specified as ``targets`` attribute blocks. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
-        :param values: List of ``user`` strings to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
-        :param variation: The index of the variation to serve if a user target value is matched. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        :param context_kind: The context kind on which the flag should target in this environment. User (``user``) targets should be specified as ``targets`` attribute blocks. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
+        :param values: List of ``user`` strings to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
+        :param variation: The index of the variation to serve if a user target value is matched. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__34b5642f26bcae6d4dc7221ef36abd376437c6e3e3763e1e7abb20f783bf5eba)
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
             check_type(argname="argument variation", value=variation, expected_type=type_hints["variation"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -774,35 +774,35 @@
 
     @builtins.property
     def context_kind(self) -> builtins.str:
         '''The context kind on which the flag should target in this environment.
 
         User (``user``) targets should be specified as ``targets`` attribute blocks.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
         '''
         result = self._values.get("context_kind")
         assert result is not None, "Required property 'context_kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''List of ``user`` strings to target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def variation(self) -> jsii.Number:
         '''The index of the variation to serve if a user target value is matched.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         assert result is not None, "Required property 'variation' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1020,18 +1020,18 @@
         *,
         bucket_by: typing.Optional[builtins.str] = None,
         context_kind: typing.Optional[builtins.str] = None,
         rollout_weights: typing.Optional[typing.Sequence[jsii.Number]] = None,
         variation: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
-        :param context_kind: The context kind associated with the specified rollout. This argument is only valid if rollout_weights is also specified. If omitted, defaults to ``user``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
-        :param rollout_weights: List of integer percentage rollout weights (in thousandths of a percent) to apply to each variation if the rule clauses evaluates to ``true``. The sum of the ``rollout_weights`` must equal 100000 and the number of rollout weights specified in the array must match the number of flag variations. You must specify either ``variation`` or ``rollout_weights``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}
-        :param variation: The default integer variation index to serve if no ``prerequisites``, ``target``, or ``rules`` apply. You must specify either ``variation`` or ``rollout_weights``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
+        :param context_kind: The context kind associated with the specified rollout. This argument is only valid if rollout_weights is also specified. If omitted, defaults to ``user``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
+        :param rollout_weights: List of integer percentage rollout weights (in thousandths of a percent) to apply to each variation if the rule clauses evaluates to ``true``. The sum of the ``rollout_weights`` must equal 100000 and the number of rollout weights specified in the array must match the number of flag variations. You must specify either ``variation`` or ``rollout_weights``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}
+        :param variation: The default integer variation index to serve if no ``prerequisites``, ``target``, or ``rules`` apply. You must specify either ``variation`` or ``rollout_weights``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__daf881e63563456bfb70bbbeb289ea98f58d399b5ee497dbb67f9a344a45c1c2)
             check_type(argname="argument bucket_by", value=bucket_by, expected_type=type_hints["bucket_by"])
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
             check_type(argname="argument rollout_weights", value=rollout_weights, expected_type=type_hints["rollout_weights"])
             check_type(argname="argument variation", value=variation, expected_type=type_hints["variation"])
@@ -1045,48 +1045,48 @@
         if variation is not None:
             self._values["variation"] = variation
 
     @builtins.property
     def bucket_by(self) -> typing.Optional[builtins.str]:
         '''Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
         '''
         result = self._values.get("bucket_by")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def context_kind(self) -> typing.Optional[builtins.str]:
         '''The context kind associated with the specified rollout.
 
         This argument is only valid if rollout_weights is also specified. If omitted, defaults to ``user``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
         '''
         result = self._values.get("context_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def rollout_weights(self) -> typing.Optional[typing.List[jsii.Number]]:
         '''List of integer percentage rollout weights (in thousandths of a percent) to apply to each variation if the rule clauses evaluates to ``true``.
 
         The sum of the ``rollout_weights`` must equal 100000 and the number of rollout weights specified in the array must match the number of flag variations. You must specify either ``variation`` or ``rollout_weights``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}
         '''
         result = self._values.get("rollout_weights")
         return typing.cast(typing.Optional[typing.List[jsii.Number]], result)
 
     @builtins.property
     def variation(self) -> typing.Optional[jsii.Number]:
         '''The default integer variation index to serve if no ``prerequisites``, ``target``, or ``rules`` apply.
 
         You must specify either ``variation`` or ``rollout_weights``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1223,41 +1223,41 @@
     jsii_type="@cdktf/provider-launchdarkly.featureFlagEnvironment.FeatureFlagEnvironmentPrerequisites",
     jsii_struct_bases=[],
     name_mapping={"flag_key": "flagKey", "variation": "variation"},
 )
 class FeatureFlagEnvironmentPrerequisites:
     def __init__(self, *, flag_key: builtins.str, variation: jsii.Number) -> None:
         '''
-        :param flag_key: The prerequisite feature flag's ``key``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#flag_key FeatureFlagEnvironment#flag_key}
-        :param variation: The index of the prerequisite feature flag's variation to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        :param flag_key: The prerequisite feature flag's ``key``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#flag_key FeatureFlagEnvironment#flag_key}
+        :param variation: The index of the prerequisite feature flag's variation to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__63941fb4c9cc7227c52d5626c12b2db316dd5ebb1ca55a101e171dbb2a76bc08)
             check_type(argname="argument flag_key", value=flag_key, expected_type=type_hints["flag_key"])
             check_type(argname="argument variation", value=variation, expected_type=type_hints["variation"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "flag_key": flag_key,
             "variation": variation,
         }
 
     @builtins.property
     def flag_key(self) -> builtins.str:
         '''The prerequisite feature flag's ``key``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#flag_key FeatureFlagEnvironment#flag_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#flag_key FeatureFlagEnvironment#flag_key}
         '''
         result = self._values.get("flag_key")
         assert result is not None, "Required property 'flag_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def variation(self) -> jsii.Number:
         '''The index of the prerequisite feature flag's variation to target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         assert result is not None, "Required property 'variation' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1460,19 +1460,19 @@
         bucket_by: typing.Optional[builtins.str] = None,
         clauses: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["FeatureFlagEnvironmentRulesClauses", typing.Dict[builtins.str, typing.Any]]]]] = None,
         description: typing.Optional[builtins.str] = None,
         rollout_weights: typing.Optional[typing.Sequence[jsii.Number]] = None,
         variation: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if ``rollout_weights`` is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
-        :param clauses: clauses block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#clauses FeatureFlagEnvironment#clauses}
-        :param description: A human-readable description of the targeting rule. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#description FeatureFlagEnvironment#description}
-        :param rollout_weights: List of integer percentage rollout weights (in thousandths of a percent) to apply to each variation if the rule clauses evaluates to ``true``. The sum of the ``rollout_weights`` must equal 100000 and the number of rollout weights specified in the array must match the number of flag variations. You must specify either ``variation`` or ``rollout_weights``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}
-        :param variation: The integer variation index to serve if the rule clauses evaluate to ``true``. You must specify either ``variation`` or ``rollout_weights`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if ``rollout_weights`` is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
+        :param clauses: clauses block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#clauses FeatureFlagEnvironment#clauses}
+        :param description: A human-readable description of the targeting rule. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#description FeatureFlagEnvironment#description}
+        :param rollout_weights: List of integer percentage rollout weights (in thousandths of a percent) to apply to each variation if the rule clauses evaluates to ``true``. The sum of the ``rollout_weights`` must equal 100000 and the number of rollout weights specified in the array must match the number of flag variations. You must specify either ``variation`` or ``rollout_weights``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}
+        :param variation: The integer variation index to serve if the rule clauses evaluate to ``true``. You must specify either ``variation`` or ``rollout_weights`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__79fd8592ed8cb3c1d7ae89faf7fa874caef359c1bef31b4e19682af92accaf76)
             check_type(argname="argument bucket_by", value=bucket_by, expected_type=type_hints["bucket_by"])
             check_type(argname="argument clauses", value=clauses, expected_type=type_hints["clauses"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument rollout_weights", value=rollout_weights, expected_type=type_hints["rollout_weights"])
@@ -1489,57 +1489,57 @@
         if variation is not None:
             self._values["variation"] = variation
 
     @builtins.property
     def bucket_by(self) -> typing.Optional[builtins.str]:
         '''Group percentage rollout by a custom attribute. This argument is only valid if ``rollout_weights`` is also specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
         '''
         result = self._values.get("bucket_by")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def clauses(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentRulesClauses"]]]:
         '''clauses block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#clauses FeatureFlagEnvironment#clauses}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#clauses FeatureFlagEnvironment#clauses}
         '''
         result = self._values.get("clauses")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentRulesClauses"]]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''A human-readable description of the targeting rule.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#description FeatureFlagEnvironment#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#description FeatureFlagEnvironment#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def rollout_weights(self) -> typing.Optional[typing.List[jsii.Number]]:
         '''List of integer percentage rollout weights (in thousandths of a percent) to apply to each variation if the rule clauses evaluates to ``true``.
 
         The sum of the ``rollout_weights`` must equal 100000 and the number of rollout weights specified in the array must match the number of flag variations. You must specify either ``variation`` or ``rollout_weights``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}
         '''
         result = self._values.get("rollout_weights")
         return typing.cast(typing.Optional[typing.List[jsii.Number]], result)
 
     @builtins.property
     def variation(self) -> typing.Optional[jsii.Number]:
         '''The integer variation index to serve if the rule clauses evaluate to ``true``.
 
         You must specify either ``variation`` or ``rollout_weights``
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1572,20 +1572,20 @@
         op: builtins.str,
         values: typing.Sequence[builtins.str],
         context_kind: typing.Optional[builtins.str] = None,
         negate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         value_type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param attribute: The user attribute to operate on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#attribute FeatureFlagEnvironment#attribute}
-        :param op: The operator associated with the rule clause. Available options are ``in``, ``endsWith``, ``startsWith``, ``matches``, ``contains``, ``lessThan``, ``lessThanOrEqual``, ``greaterThanOrEqual``, ``before``, ``after``, ``segmentMatch``, ``semVerEqual``, ``semVerLessThan``, and ``semVerGreaterThan``. Read LaunchDarkly's `Operators <https://docs.launchdarkly.com/sdk/concepts/flag-evaluation-rules#operators>`_ documentation for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#op FeatureFlagEnvironment#op}
-        :param values: The list of values associated with the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
-        :param context_kind: The context kind associated with this rule clause. This argument is only valid if ``rollout_weights`` is also specified. If omitted, defaults to ``user``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
-        :param negate: Whether to negate the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#negate FeatureFlagEnvironment#negate}
-        :param value_type: The type for each of the clause's values. Available types are ``boolean``, ``string``, and ``number``. If omitted, ``value_type`` defaults to ``string``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#value_type FeatureFlagEnvironment#value_type}
+        :param attribute: The user attribute to operate on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#attribute FeatureFlagEnvironment#attribute}
+        :param op: The operator associated with the rule clause. Available options are ``in``, ``endsWith``, ``startsWith``, ``matches``, ``contains``, ``lessThan``, ``lessThanOrEqual``, ``greaterThanOrEqual``, ``before``, ``after``, ``segmentMatch``, ``semVerEqual``, ``semVerLessThan``, and ``semVerGreaterThan``. Read LaunchDarkly's `Operators <https://docs.launchdarkly.com/sdk/concepts/flag-evaluation-rules#operators>`_ documentation for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#op FeatureFlagEnvironment#op}
+        :param values: The list of values associated with the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
+        :param context_kind: The context kind associated with this rule clause. This argument is only valid if ``rollout_weights`` is also specified. If omitted, defaults to ``user``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
+        :param negate: Whether to negate the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#negate FeatureFlagEnvironment#negate}
+        :param value_type: The type for each of the clause's values. Available types are ``boolean``, ``string``, and ``number``. If omitted, ``value_type`` defaults to ``string``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#value_type FeatureFlagEnvironment#value_type}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c3764dc1ebdf1737e8cb1806314d82ed5209be7d9cb0f28615542c981b19fcf3)
             check_type(argname="argument attribute", value=attribute, expected_type=type_hints["attribute"])
             check_type(argname="argument op", value=op, expected_type=type_hints["op"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
@@ -1603,71 +1603,71 @@
         if value_type is not None:
             self._values["value_type"] = value_type
 
     @builtins.property
     def attribute(self) -> builtins.str:
         '''The user attribute to operate on.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#attribute FeatureFlagEnvironment#attribute}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#attribute FeatureFlagEnvironment#attribute}
         '''
         result = self._values.get("attribute")
         assert result is not None, "Required property 'attribute' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def op(self) -> builtins.str:
         '''The operator associated with the rule clause.
 
         Available options are ``in``, ``endsWith``, ``startsWith``, ``matches``, ``contains``, ``lessThan``, ``lessThanOrEqual``, ``greaterThanOrEqual``, ``before``, ``after``, ``segmentMatch``, ``semVerEqual``, ``semVerLessThan``, and ``semVerGreaterThan``. Read LaunchDarkly's `Operators <https://docs.launchdarkly.com/sdk/concepts/flag-evaluation-rules#operators>`_ documentation for more information.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#op FeatureFlagEnvironment#op}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#op FeatureFlagEnvironment#op}
         '''
         result = self._values.get("op")
         assert result is not None, "Required property 'op' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''The list of values associated with the rule clause.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def context_kind(self) -> typing.Optional[builtins.str]:
         '''The context kind associated with this rule clause.
 
         This argument is only valid if ``rollout_weights`` is also specified. If omitted, defaults to ``user``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
         '''
         result = self._values.get("context_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def negate(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether to negate the rule clause.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#negate FeatureFlagEnvironment#negate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#negate FeatureFlagEnvironment#negate}
         '''
         result = self._values.get("negate")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def value_type(self) -> typing.Optional[builtins.str]:
         '''The type for each of the clause's values.
 
         Available types are ``boolean``, ``string``, and ``number``. If omitted, ``value_type`` defaults to ``string``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#value_type FeatureFlagEnvironment#value_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#value_type FeatureFlagEnvironment#value_type}
         '''
         result = self._values.get("value_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -2192,41 +2192,41 @@
     def __init__(
         self,
         *,
         values: typing.Sequence[builtins.str],
         variation: jsii.Number,
     ) -> None:
         '''
-        :param values: List of ``user`` strings to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
-        :param variation: The index of the variation to serve if a user target value is matched. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        :param values: List of ``user`` strings to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
+        :param variation: The index of the variation to serve if a user target value is matched. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c72fbcaf4343839fe9804c08d329a29b09af1ba31b7c68d3c1dd452b24ef3b9e)
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
             check_type(argname="argument variation", value=variation, expected_type=type_hints["variation"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "values": values,
             "variation": variation,
         }
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''List of ``user`` strings to target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def variation(self) -> jsii.Number:
         '''The index of the variation to serve if a user target value is matched.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         assert result is not None, "Required property 'variation' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/flag_trigger/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/flag_trigger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_flag_trigger`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_flag_trigger`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger).
+Refer to the Terraform Registry for docs: [`launchdarkly_flag_trigger`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class FlagTrigger(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.flagTrigger.FlagTrigger",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger launchdarkly_flag_trigger}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger launchdarkly_flag_trigger}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         enabled: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
@@ -47,25 +47,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger launchdarkly_flag_trigger} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger launchdarkly_flag_trigger} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#enabled FlagTrigger#enabled}
-        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#env_key FlagTrigger#env_key}
-        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#flag_key FlagTrigger#flag_key}
-        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#instructions FlagTrigger#instructions}
-        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#integration_key FlagTrigger#integration_key}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#project_key FlagTrigger#project_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#id FlagTrigger#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#enabled FlagTrigger#enabled}
+        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#env_key FlagTrigger#env_key}
+        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#flag_key FlagTrigger#flag_key}
+        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#instructions FlagTrigger#instructions}
+        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#integration_key FlagTrigger#integration_key}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#project_key FlagTrigger#project_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#id FlagTrigger#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -102,29 +102,29 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a FlagTrigger resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the FlagTrigger to import.
-        :param import_from_id: The id of the existing FlagTrigger that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing FlagTrigger that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the FlagTrigger to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e26684a362951051d5a8ca49a14182eba17d58c0c3a327f3afbea365cfe9a207)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
         return typing.cast(_cdktf_9a9027ec.ImportableResource, jsii.sinvoke(cls, "generateConfigForImport", [scope, import_to_id, import_from_id, provider]))
 
     @jsii.member(jsii_name="putInstructions")
     def put_instructions(self, *, kind: builtins.str) -> None:
         '''
-        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#kind FlagTrigger#kind}
+        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#kind FlagTrigger#kind}
         '''
         value = FlagTriggerInstructions(kind=kind)
 
         return typing.cast(None, jsii.invoke(self, "putInstructions", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -314,21 +314,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#enabled FlagTrigger#enabled}
-        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#env_key FlagTrigger#env_key}
-        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#flag_key FlagTrigger#flag_key}
-        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#instructions FlagTrigger#instructions}
-        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#integration_key FlagTrigger#integration_key}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#project_key FlagTrigger#project_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#id FlagTrigger#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#enabled FlagTrigger#enabled}
+        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#env_key FlagTrigger#env_key}
+        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#flag_key FlagTrigger#flag_key}
+        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#instructions FlagTrigger#instructions}
+        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#integration_key FlagTrigger#integration_key}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#project_key FlagTrigger#project_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#id FlagTrigger#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(instructions, dict):
             instructions = FlagTriggerInstructions(**instructions)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9f039e9efaf534fc0f33df3e00c8730b5e945d57b2562f833b651905cca539a0)
@@ -435,75 +435,75 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def enabled(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
         '''Whether the trigger is currently active or not. This property defaults to true upon creation.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#enabled FlagTrigger#enabled}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#enabled FlagTrigger#enabled}
         '''
         result = self._values.get("enabled")
         assert result is not None, "Required property 'enabled' is missing"
         return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], result)
 
     @builtins.property
     def env_key(self) -> builtins.str:
         '''The LaunchDarkly environment key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#env_key FlagTrigger#env_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#env_key FlagTrigger#env_key}
         '''
         result = self._values.get("env_key")
         assert result is not None, "Required property 'env_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def flag_key(self) -> builtins.str:
         '''The key of the feature flag the trigger acts upon.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#flag_key FlagTrigger#flag_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#flag_key FlagTrigger#flag_key}
         '''
         result = self._values.get("flag_key")
         assert result is not None, "Required property 'flag_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def instructions(self) -> "FlagTriggerInstructions":
         '''instructions block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#instructions FlagTrigger#instructions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#instructions FlagTrigger#instructions}
         '''
         result = self._values.get("instructions")
         assert result is not None, "Required property 'instructions' is missing"
         return typing.cast("FlagTriggerInstructions", result)
 
     @builtins.property
     def integration_key(self) -> builtins.str:
         '''The unique identifier of the integration you intend to set your trigger up with.
 
         "generic-trigger" should be used for integrations not explicitly supported.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#integration_key FlagTrigger#integration_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#integration_key FlagTrigger#integration_key}
         '''
         result = self._values.get("integration_key")
         assert result is not None, "Required property 'integration_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The LaunchDarkly project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#project_key FlagTrigger#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#project_key FlagTrigger#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#id FlagTrigger#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#id FlagTrigger#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -523,28 +523,28 @@
     jsii_type="@cdktf/provider-launchdarkly.flagTrigger.FlagTriggerInstructions",
     jsii_struct_bases=[],
     name_mapping={"kind": "kind"},
 )
 class FlagTriggerInstructions:
     def __init__(self, *, kind: builtins.str) -> None:
         '''
-        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#kind FlagTrigger#kind}
+        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#kind FlagTrigger#kind}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ba70d50fd1e0e0d95e46d625c8ddbc57458fddb83adaef40237b6c7c0673be92)
             check_type(argname="argument kind", value=kind, expected_type=type_hints["kind"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "kind": kind,
         }
 
     @builtins.property
     def kind(self) -> builtins.str:
         '''The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff".
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/flag_trigger#kind FlagTrigger#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/flag_trigger#kind FlagTrigger#kind}
         '''
         result = self._values.get("kind")
         assert result is not None, "Required property 'kind' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/metric/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/metric/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_metric`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_metric`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric).
+Refer to the Terraform Registry for docs: [`launchdarkly_metric`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class Metric(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.metric.Metric",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric launchdarkly_metric}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric launchdarkly_metric}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -56,34 +56,34 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric launchdarkly_metric} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric launchdarkly_metric} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#key Metric#key}
-        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#kind Metric#kind}
-        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#name Metric#name}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#project_key Metric#project_key}
-        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#description Metric#description}
-        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#event_key Metric#event_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#id Metric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#is_active Metric#is_active}
-        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#is_numeric Metric#is_numeric}
-        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#maintainer_id Metric#maintainer_id}
-        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#randomization_units Metric#randomization_units}
-        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#selector Metric#selector}
-        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#success_criteria Metric#success_criteria}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#tags Metric#tags}
-        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#unit Metric#unit}
-        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#urls Metric#urls}
+        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#key Metric#key}
+        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#kind Metric#kind}
+        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#name Metric#name}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#project_key Metric#project_key}
+        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#description Metric#description}
+        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#event_key Metric#event_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#id Metric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#is_active Metric#is_active}
+        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#is_numeric Metric#is_numeric}
+        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#maintainer_id Metric#maintainer_id}
+        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#randomization_units Metric#randomization_units}
+        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#selector Metric#selector}
+        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#success_criteria Metric#success_criteria}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#tags Metric#tags}
+        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#unit Metric#unit}
+        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#urls Metric#urls}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -129,15 +129,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Metric resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Metric to import.
-        :param import_from_id: The id of the existing Metric that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Metric that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Metric to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a7a238e8c4f1e0a87d2ca34026e7028f96b8e9e355bbdb808c9343d34164c6bb)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -557,30 +557,30 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#key Metric#key}
-        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#kind Metric#kind}
-        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#name Metric#name}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#project_key Metric#project_key}
-        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#description Metric#description}
-        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#event_key Metric#event_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#id Metric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#is_active Metric#is_active}
-        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#is_numeric Metric#is_numeric}
-        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#maintainer_id Metric#maintainer_id}
-        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#randomization_units Metric#randomization_units}
-        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#selector Metric#selector}
-        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#success_criteria Metric#success_criteria}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#tags Metric#tags}
-        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#unit Metric#unit}
-        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#urls Metric#urls}
+        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#key Metric#key}
+        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#kind Metric#kind}
+        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#name Metric#name}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#project_key Metric#project_key}
+        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#description Metric#description}
+        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#event_key Metric#event_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#id Metric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#is_active Metric#is_active}
+        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#is_numeric Metric#is_numeric}
+        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#maintainer_id Metric#maintainer_id}
+        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#randomization_units Metric#randomization_units}
+        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#selector Metric#selector}
+        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#success_criteria Metric#success_criteria}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#tags Metric#tags}
+        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#unit Metric#unit}
+        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#urls Metric#urls}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__aa7cac13f5219f12a99cd83049cfcaff852eed75dcf965f55118e2d716bd2eda)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -714,163 +714,163 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''A unique key that will be used to reference the metric in your code.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#key Metric#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#key Metric#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def kind(self) -> builtins.str:
         '''The metric type -available choices are 'pageview', 'click', and 'custom'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#kind Metric#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#kind Metric#kind}
         '''
         result = self._values.get("kind")
         assert result is not None, "Required property 'kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''A human-readable name for your metric.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#name Metric#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#name Metric#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The LaunchDarkly project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#project_key Metric#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#project_key Metric#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''A short description of what the metric will be used for.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#description Metric#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#description Metric#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def event_key(self) -> typing.Optional[builtins.str]:
         '''The event key for your metric (if custom metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#event_key Metric#event_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#event_key Metric#event_key}
         '''
         result = self._values.get("event_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#id Metric#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#id Metric#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def is_active(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the metric is active.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#is_active Metric#is_active}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#is_active Metric#is_active}
         '''
         result = self._values.get("is_active")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def is_numeric(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the metric is numeric.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#is_numeric Metric#is_numeric}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#is_numeric Metric#is_numeric}
         '''
         result = self._values.get("is_numeric")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def maintainer_id(self) -> typing.Optional[builtins.str]:
         '''The LaunchDarkly ID of the user who will maintain the metric.
 
         If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#maintainer_id Metric#maintainer_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#maintainer_id Metric#maintainer_id}
         '''
         result = self._values.get("maintainer_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def randomization_units(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A set of one or more context kinds that this metric can measure events from.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#randomization_units Metric#randomization_units}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#randomization_units Metric#randomization_units}
         '''
         result = self._values.get("randomization_units")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def selector(self) -> typing.Optional[builtins.str]:
         '''The CSS selector for your metric (if click metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#selector Metric#selector}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#selector Metric#selector}
         '''
         result = self._values.get("selector")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def success_criteria(self) -> typing.Optional[builtins.str]:
         '''The success criteria for your metric (if numeric metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#success_criteria Metric#success_criteria}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#success_criteria Metric#success_criteria}
         '''
         result = self._values.get("success_criteria")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#tags Metric#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#tags Metric#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def unit(self) -> typing.Optional[builtins.str]:
         '''The unit for your metric (if numeric metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#unit Metric#unit}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#unit Metric#unit}
         '''
         result = self._values.get("unit")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def urls(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["MetricUrls"]]]:
         '''urls block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#urls Metric#urls}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#urls Metric#urls}
         '''
         result = self._values.get("urls")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["MetricUrls"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -899,18 +899,18 @@
         *,
         kind: builtins.str,
         pattern: typing.Optional[builtins.str] = None,
         substring: typing.Optional[builtins.str] = None,
         url: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param kind: The url type - available choices are 'exact', 'canonical', 'substring' and 'regex'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#kind Metric#kind}
-        :param pattern: The URL-matching regex. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#pattern Metric#pattern}
-        :param substring: The URL substring. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#substring Metric#substring}
-        :param url: The exact or canonical URL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#url Metric#url}
+        :param kind: The url type - available choices are 'exact', 'canonical', 'substring' and 'regex'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#kind Metric#kind}
+        :param pattern: The URL-matching regex. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#pattern Metric#pattern}
+        :param substring: The URL substring. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#substring Metric#substring}
+        :param url: The exact or canonical URL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#url Metric#url}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__941ff69f5b9f18fc592a8e5b1561eb5a1ba864e6cf32bab45cb6df1623b19842)
             check_type(argname="argument kind", value=kind, expected_type=type_hints["kind"])
             check_type(argname="argument pattern", value=pattern, expected_type=type_hints["pattern"])
             check_type(argname="argument substring", value=substring, expected_type=type_hints["substring"])
             check_type(argname="argument url", value=url, expected_type=type_hints["url"])
@@ -924,43 +924,43 @@
         if url is not None:
             self._values["url"] = url
 
     @builtins.property
     def kind(self) -> builtins.str:
         '''The url type - available choices are 'exact', 'canonical', 'substring' and 'regex'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#kind Metric#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#kind Metric#kind}
         '''
         result = self._values.get("kind")
         assert result is not None, "Required property 'kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def pattern(self) -> typing.Optional[builtins.str]:
         '''The URL-matching regex.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#pattern Metric#pattern}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#pattern Metric#pattern}
         '''
         result = self._values.get("pattern")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def substring(self) -> typing.Optional[builtins.str]:
         '''The URL substring.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#substring Metric#substring}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#substring Metric#substring}
         '''
         result = self._values.get("substring")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def url(self) -> typing.Optional[builtins.str]:
         '''The exact or canonical URL.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/metric#url Metric#url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/metric#url Metric#url}
         '''
         result = self._values.get("url")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/project/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/project/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_project`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_project`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project).
+Refer to the Terraform Registry for docs: [`launchdarkly_project`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class Project(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.project.Project",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project launchdarkly_project}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project launchdarkly_project}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         environments: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ProjectEnvironments", typing.Dict[builtins.str, typing.Any]]]],
@@ -47,25 +47,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project launchdarkly_project} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project launchdarkly_project} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param environments: environments block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#environments Project#environments}
-        :param key: The project's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#key Project#key}
-        :param name: A human-readable name for your project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#name Project#name}
-        :param default_client_side_availability: default_client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#default_client_side_availability Project#default_client_side_availability}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#id Project#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param include_in_snippet: Whether feature flags created under the project should be available to client-side SDKs by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#include_in_snippet Project#include_in_snippet}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#tags Project#tags}
+        :param environments: environments block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#environments Project#environments}
+        :param key: The project's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#key Project#key}
+        :param name: A human-readable name for your project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#name Project#name}
+        :param default_client_side_availability: default_client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#default_client_side_availability Project#default_client_side_availability}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#id Project#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param include_in_snippet: Whether feature flags created under the project should be available to client-side SDKs by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#include_in_snippet Project#include_in_snippet}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#tags Project#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -102,15 +102,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Project resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Project to import.
-        :param import_from_id: The id of the existing Project that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Project that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Project to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bc132d41eed83f0e924ddfad27e2a768c892ddfa36e53b80e5e93f85c5e26180)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -334,21 +334,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param environments: environments block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#environments Project#environments}
-        :param key: The project's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#key Project#key}
-        :param name: A human-readable name for your project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#name Project#name}
-        :param default_client_side_availability: default_client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#default_client_side_availability Project#default_client_side_availability}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#id Project#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param include_in_snippet: Whether feature flags created under the project should be available to client-side SDKs by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#include_in_snippet Project#include_in_snippet}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#tags Project#tags}
+        :param environments: environments block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#environments Project#environments}
+        :param key: The project's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#key Project#key}
+        :param name: A human-readable name for your project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#name Project#name}
+        :param default_client_side_availability: default_client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#default_client_side_availability Project#default_client_side_availability}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#id Project#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param include_in_snippet: Whether feature flags created under the project should be available to client-side SDKs by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#include_in_snippet Project#include_in_snippet}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#tags Project#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8ae07973b215950e642bea0cd54fd02ef332024a996adeefa1d83b0c07431b53)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -458,77 +458,77 @@
 
     @builtins.property
     def environments(
         self,
     ) -> typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ProjectEnvironments"]]:
         '''environments block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#environments Project#environments}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#environments Project#environments}
         '''
         result = self._values.get("environments")
         assert result is not None, "Required property 'environments' is missing"
         return typing.cast(typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ProjectEnvironments"]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The project's unique key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#key Project#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#key Project#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''A human-readable name for your project.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#name Project#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#name Project#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def default_client_side_availability(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ProjectDefaultClientSideAvailability"]]]:
         '''default_client_side_availability block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#default_client_side_availability Project#default_client_side_availability}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#default_client_side_availability Project#default_client_side_availability}
         '''
         result = self._values.get("default_client_side_availability")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ProjectDefaultClientSideAvailability"]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#id Project#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#id Project#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def include_in_snippet(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether feature flags created under the project should be available to client-side SDKs by default.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#include_in_snippet Project#include_in_snippet}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#include_in_snippet Project#include_in_snippet}
         '''
         result = self._values.get("include_in_snippet")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#tags Project#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#tags Project#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -553,40 +553,40 @@
     def __init__(
         self,
         *,
         using_environment_id: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
         using_mobile_key: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
     ) -> None:
         '''
-        :param using_environment_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#using_environment_id Project#using_environment_id}.
-        :param using_mobile_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#using_mobile_key Project#using_mobile_key}.
+        :param using_environment_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#using_environment_id Project#using_environment_id}.
+        :param using_mobile_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#using_mobile_key Project#using_mobile_key}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c7874d920a1b7a98a3f26d393bb93580676cb36ccecceef747b568340945c93c)
             check_type(argname="argument using_environment_id", value=using_environment_id, expected_type=type_hints["using_environment_id"])
             check_type(argname="argument using_mobile_key", value=using_mobile_key, expected_type=type_hints["using_mobile_key"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "using_environment_id": using_environment_id,
             "using_mobile_key": using_mobile_key,
         }
 
     @builtins.property
     def using_environment_id(
         self,
     ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#using_environment_id Project#using_environment_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#using_environment_id Project#using_environment_id}.'''
         result = self._values.get("using_environment_id")
         assert result is not None, "Required property 'using_environment_id' is missing"
         return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], result)
 
     @builtins.property
     def using_mobile_key(
         self,
     ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#using_mobile_key Project#using_mobile_key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#using_mobile_key Project#using_mobile_key}.'''
         result = self._values.get("using_mobile_key")
         assert result is not None, "Required property 'using_mobile_key' is missing"
         return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -814,25 +814,25 @@
         default_track_events: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         default_ttl: typing.Optional[jsii.Number] = None,
         require_comments: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         secure_mode: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         tags: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param color: The color swatch as an RGB hex value with no leading ``#``. For example: ``000000``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#color Project#color}
-        :param key: The project-unique key for the environment. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#key Project#key}
-        :param name: The name of the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#name Project#name}
-        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#approval_settings Project#approval_settings}
-        :param confirm_changes: Set to ``true`` if this environment requires confirmation for flag and segment changes. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#confirm_changes Project#confirm_changes}
-        :param critical: Denotes whether the environment is critical. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#critical Project#critical}
-        :param default_track_events: Set to ``true`` to enable data export for every flag created in this environment after you configure this argument. This field will default to ``false`` when not set. To learn more, read `Data Export <https://docs.launchdarkly.com/home/data-export>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#default_track_events Project#default_track_events}
-        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK. This field will default to ``0`` when not set. To learn more, read `TTL settings <https://docs.launchdarkly.com/home/organize/environments#ttl-settings>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#default_ttl Project#default_ttl}
-        :param require_comments: Set to ``true`` if this environment requires comments for flag and segment changes. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#require_comments Project#require_comments}
-        :param secure_mode: Set to ``true`` to ensure a user of the client-side SDK cannot impersonate another user. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#secure_mode Project#secure_mode}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#tags Project#tags}
+        :param color: The color swatch as an RGB hex value with no leading ``#``. For example: ``000000``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#color Project#color}
+        :param key: The project-unique key for the environment. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#key Project#key}
+        :param name: The name of the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#name Project#name}
+        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#approval_settings Project#approval_settings}
+        :param confirm_changes: Set to ``true`` if this environment requires confirmation for flag and segment changes. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#confirm_changes Project#confirm_changes}
+        :param critical: Denotes whether the environment is critical. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#critical Project#critical}
+        :param default_track_events: Set to ``true`` to enable data export for every flag created in this environment after you configure this argument. This field will default to ``false`` when not set. To learn more, read `Data Export <https://docs.launchdarkly.com/home/data-export>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#default_track_events Project#default_track_events}
+        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK. This field will default to ``0`` when not set. To learn more, read `TTL settings <https://docs.launchdarkly.com/home/organize/environments#ttl-settings>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#default_ttl Project#default_ttl}
+        :param require_comments: Set to ``true`` if this environment requires comments for flag and segment changes. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#require_comments Project#require_comments}
+        :param secure_mode: Set to ``true`` to ensure a user of the client-side SDK cannot impersonate another user. This field will default to ``false`` when not set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#secure_mode Project#secure_mode}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#tags Project#tags}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ac2ed1b079b68cb919a5a6db7a4c230b9465cd2b936b69294e4e02637b01c6c4)
             check_type(argname="argument color", value=color, expected_type=type_hints["color"])
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument approval_settings", value=approval_settings, expected_type=type_hints["approval_settings"])
@@ -865,132 +865,132 @@
         if tags is not None:
             self._values["tags"] = tags
 
     @builtins.property
     def color(self) -> builtins.str:
         '''The color swatch as an RGB hex value with no leading ``#``. For example: ``000000``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#color Project#color}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#color Project#color}
         '''
         result = self._values.get("color")
         assert result is not None, "Required property 'color' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The project-unique key for the environment.
 
         A change in this field will force the destruction of the existing resource and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#key Project#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#key Project#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#name Project#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#name Project#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def approval_settings(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ProjectEnvironmentsApprovalSettings"]]]:
         '''approval_settings block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#approval_settings Project#approval_settings}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#approval_settings Project#approval_settings}
         '''
         result = self._values.get("approval_settings")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ProjectEnvironmentsApprovalSettings"]]], result)
 
     @builtins.property
     def confirm_changes(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set to ``true`` if this environment requires confirmation for flag and segment changes.
 
         This field will default to ``false`` when not set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#confirm_changes Project#confirm_changes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#confirm_changes Project#confirm_changes}
         '''
         result = self._values.get("confirm_changes")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def critical(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Denotes whether the environment is critical.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#critical Project#critical}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#critical Project#critical}
         '''
         result = self._values.get("critical")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def default_track_events(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set to ``true`` to enable data export for every flag created in this environment after you configure this argument.
 
         This field will default to ``false`` when not set. To learn more, read `Data Export <https://docs.launchdarkly.com/home/data-export>`_.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#default_track_events Project#default_track_events}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#default_track_events Project#default_track_events}
         '''
         result = self._values.get("default_track_events")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def default_ttl(self) -> typing.Optional[jsii.Number]:
         '''The TTL for the environment.
 
         This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK. This field will default to ``0`` when not set. To learn more, read `TTL settings <https://docs.launchdarkly.com/home/organize/environments#ttl-settings>`_.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#default_ttl Project#default_ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#default_ttl Project#default_ttl}
         '''
         result = self._values.get("default_ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def require_comments(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set to ``true`` if this environment requires comments for flag and segment changes.
 
         This field will default to ``false`` when not set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#require_comments Project#require_comments}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#require_comments Project#require_comments}
         '''
         result = self._values.get("require_comments")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def secure_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set to ``true`` to ensure a user of the client-side SDK cannot impersonate another user.
 
         This field will default to ``false`` when not set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#secure_mode Project#secure_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#secure_mode Project#secure_mode}
         '''
         result = self._values.get("secure_mode")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#tags Project#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#tags Project#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1025,21 +1025,21 @@
         min_num_approvals: typing.Optional[jsii.Number] = None,
         required: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         required_approval_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
         service_config: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         service_kind: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param can_apply_declined_changes: Set to ``true`` if changes can be applied as long as the ``min_num_approvals`` is met, regardless of whether any reviewers have declined a request. Defaults to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#can_apply_declined_changes Project#can_apply_declined_changes}
-        :param can_review_own_request: Set to ``true`` if requesters can approve or decline their own request. They may always comment. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#can_review_own_request Project#can_review_own_request}
-        :param min_num_approvals: The number of approvals required before an approval request can be applied. This number must be between 1 and 5. Defaults to 1. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#min_num_approvals Project#min_num_approvals}
-        :param required: Set to ``true`` for changes to flags in this environment to require approval. You may only set ``required`` to true if ``required_approval_tags`` is not set and vice versa. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#required Project#required}
-        :param required_approval_tags: An array of tags used to specify which flags with those tags require approval. You may only set ``required_approval_tags`` if ``required`` is not set to ``true`` and vice versa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#required_approval_tags Project#required_approval_tags}
-        :param service_config: The configuration for the service associated with this approval. This is specific to each approval service. For a ``service_kind`` of ``servicenow``, the following fields apply:: - `template` (String) The sys_id of the Standard Change Request Template in ServiceNow that LaunchDarkly will use when creating the change request. - `detail_column` (String) The name of the ServiceNow Change Request column LaunchDarkly uses to populate detailed approval request information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#service_config Project#service_config}
-        :param service_kind: The kind of service associated with this approval. This determines which platform is used for requesting approval. Valid values are ``servicenow``, ``launchdarkly``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#service_kind Project#service_kind}
+        :param can_apply_declined_changes: Set to ``true`` if changes can be applied as long as the ``min_num_approvals`` is met, regardless of whether any reviewers have declined a request. Defaults to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#can_apply_declined_changes Project#can_apply_declined_changes}
+        :param can_review_own_request: Set to ``true`` if requesters can approve or decline their own request. They may always comment. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#can_review_own_request Project#can_review_own_request}
+        :param min_num_approvals: The number of approvals required before an approval request can be applied. This number must be between 1 and 5. Defaults to 1. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#min_num_approvals Project#min_num_approvals}
+        :param required: Set to ``true`` for changes to flags in this environment to require approval. You may only set ``required`` to true if ``required_approval_tags`` is not set and vice versa. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#required Project#required}
+        :param required_approval_tags: An array of tags used to specify which flags with those tags require approval. You may only set ``required_approval_tags`` if ``required`` is not set to ``true`` and vice versa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#required_approval_tags Project#required_approval_tags}
+        :param service_config: The configuration for the service associated with this approval. This is specific to each approval service. For a ``service_kind`` of ``servicenow``, the following fields apply:: - `template` (String) The sys_id of the Standard Change Request Template in ServiceNow that LaunchDarkly will use when creating the change request. - `detail_column` (String) The name of the ServiceNow Change Request column LaunchDarkly uses to populate detailed approval request information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#service_config Project#service_config}
+        :param service_kind: The kind of service associated with this approval. This determines which platform is used for requesting approval. Valid values are ``servicenow``, ``launchdarkly``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#service_kind Project#service_kind}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7e0da4efd35c7e9a11f3765c4e842e83118be30fc18f2d3a933612b6d1f5eebf)
             check_type(argname="argument can_apply_declined_changes", value=can_apply_declined_changes, expected_type=type_hints["can_apply_declined_changes"])
             check_type(argname="argument can_review_own_request", value=can_review_own_request, expected_type=type_hints["can_review_own_request"])
             check_type(argname="argument min_num_approvals", value=min_num_approvals, expected_type=type_hints["min_num_approvals"])
             check_type(argname="argument required", value=required, expected_type=type_hints["required"])
@@ -1066,61 +1066,61 @@
     def can_apply_declined_changes(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set to ``true`` if changes can be applied as long as the ``min_num_approvals`` is met, regardless of whether any reviewers have declined a request.
 
         Defaults to ``true``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#can_apply_declined_changes Project#can_apply_declined_changes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#can_apply_declined_changes Project#can_apply_declined_changes}
         '''
         result = self._values.get("can_apply_declined_changes")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def can_review_own_request(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set to ``true`` if requesters can approve or decline their own request. They may always comment. Defaults to ``false``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#can_review_own_request Project#can_review_own_request}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#can_review_own_request Project#can_review_own_request}
         '''
         result = self._values.get("can_review_own_request")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def min_num_approvals(self) -> typing.Optional[jsii.Number]:
         '''The number of approvals required before an approval request can be applied.
 
         This number must be between 1 and 5. Defaults to 1.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#min_num_approvals Project#min_num_approvals}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#min_num_approvals Project#min_num_approvals}
         '''
         result = self._values.get("min_num_approvals")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def required(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Set to ``true`` for changes to flags in this environment to require approval.
 
         You may only set ``required`` to true if ``required_approval_tags`` is not set and vice versa. Defaults to ``false``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#required Project#required}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#required Project#required}
         '''
         result = self._values.get("required")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def required_approval_tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''An array of tags used to specify which flags with those tags require approval.
 
         You may only set ``required_approval_tags`` if ``required`` is not set to ``true`` and vice versa.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#required_approval_tags Project#required_approval_tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#required_approval_tags Project#required_approval_tags}
         '''
         result = self._values.get("required_approval_tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def service_config(
         self,
@@ -1128,26 +1128,26 @@
         '''The configuration for the service associated with this approval.
 
         This is specific to each approval service. For a ``service_kind`` of ``servicenow``, the following fields apply::
 
             - `template` (String) The sys_id of the Standard Change Request Template in ServiceNow that LaunchDarkly will use when creating the change request.
             - `detail_column` (String) The name of the ServiceNow Change Request column LaunchDarkly uses to populate detailed approval request information.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#service_config Project#service_config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#service_config Project#service_config}
         '''
         result = self._values.get("service_config")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def service_kind(self) -> typing.Optional[builtins.str]:
         '''The kind of service associated with this approval.
 
         This determines which platform is used for requesting approval. Valid values are ``servicenow``, ``launchdarkly``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/project#service_kind Project#service_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/project#service_kind Project#service_kind}
         '''
         result = self._values.get("service_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/provider/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/provider/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registry for docs: [`launchdarkly`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs).
+Refer to the Terraform Registry for docs: [`launchdarkly`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,36 +25,36 @@
 
 
 class LaunchdarklyProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.provider.LaunchdarklyProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs launchdarkly}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs launchdarkly}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         access_token: typing.Optional[builtins.str] = None,
         alias: typing.Optional[builtins.str] = None,
         api_host: typing.Optional[builtins.str] = None,
         http_timeout: typing.Optional[jsii.Number] = None,
         oauth_token: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs launchdarkly} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs launchdarkly} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param access_token: The `personal access token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#personal-tokens>`_ or `service token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#service-tokens>`_ used to authenticate with LaunchDarkly. You can also set this with the ``LAUNCHDARKLY_ACCESS_TOKEN`` environment variable. You must provide either ``access_token`` or ``oauth_token``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#access_token LaunchdarklyProvider#access_token}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#alias LaunchdarklyProvider#alias}
-        :param api_host: The LaunchDarkly host address. If this argument is not specified, the default host address is ``https://app.launchdarkly.com``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#api_host LaunchdarklyProvider#api_host}
-        :param http_timeout: The HTTP timeout (in seconds) when making API calls to LaunchDarkly. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#http_timeout LaunchdarklyProvider#http_timeout}
-        :param oauth_token: An OAuth V2 token you use to authenticate with LaunchDarkly. You can also set this with the ``LAUNCHDARKLY_OAUTH_TOKEN`` environment variable. You must provide either ``access_token`` or ``oauth_token``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#oauth_token LaunchdarklyProvider#oauth_token}
+        :param access_token: The `personal access token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#personal-tokens>`_ or `service token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#service-tokens>`_ used to authenticate with LaunchDarkly. You can also set this with the ``LAUNCHDARKLY_ACCESS_TOKEN`` environment variable. You must provide either ``access_token`` or ``oauth_token``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#access_token LaunchdarklyProvider#access_token}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#alias LaunchdarklyProvider#alias}
+        :param api_host: The LaunchDarkly host address. If this argument is not specified, the default host address is ``https://app.launchdarkly.com``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#api_host LaunchdarklyProvider#api_host}
+        :param http_timeout: The HTTP timeout (in seconds) when making API calls to LaunchDarkly. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#http_timeout LaunchdarklyProvider#http_timeout}
+        :param oauth_token: An OAuth V2 token you use to authenticate with LaunchDarkly. You can also set this with the ``LAUNCHDARKLY_OAUTH_TOKEN`` environment variable. You must provide either ``access_token`` or ``oauth_token``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#oauth_token LaunchdarklyProvider#oauth_token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__361329afd854bf518b4157de0781ee1d4b0e0a1ed34515261d7ac92f9008aa00)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = LaunchdarklyProviderConfig(
             access_token=access_token,
@@ -75,15 +75,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a LaunchdarklyProvider resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the LaunchdarklyProvider to import.
-        :param import_from_id: The id of the existing LaunchdarklyProvider that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing LaunchdarklyProvider that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the LaunchdarklyProvider to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e1bee4a71cff4d658c825fa50540dc4ceb86ff1f462f93cf56cf87d7178a1afa)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -227,19 +227,19 @@
         access_token: typing.Optional[builtins.str] = None,
         alias: typing.Optional[builtins.str] = None,
         api_host: typing.Optional[builtins.str] = None,
         http_timeout: typing.Optional[jsii.Number] = None,
         oauth_token: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param access_token: The `personal access token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#personal-tokens>`_ or `service token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#service-tokens>`_ used to authenticate with LaunchDarkly. You can also set this with the ``LAUNCHDARKLY_ACCESS_TOKEN`` environment variable. You must provide either ``access_token`` or ``oauth_token``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#access_token LaunchdarklyProvider#access_token}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#alias LaunchdarklyProvider#alias}
-        :param api_host: The LaunchDarkly host address. If this argument is not specified, the default host address is ``https://app.launchdarkly.com``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#api_host LaunchdarklyProvider#api_host}
-        :param http_timeout: The HTTP timeout (in seconds) when making API calls to LaunchDarkly. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#http_timeout LaunchdarklyProvider#http_timeout}
-        :param oauth_token: An OAuth V2 token you use to authenticate with LaunchDarkly. You can also set this with the ``LAUNCHDARKLY_OAUTH_TOKEN`` environment variable. You must provide either ``access_token`` or ``oauth_token``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#oauth_token LaunchdarklyProvider#oauth_token}
+        :param access_token: The `personal access token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#personal-tokens>`_ or `service token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#service-tokens>`_ used to authenticate with LaunchDarkly. You can also set this with the ``LAUNCHDARKLY_ACCESS_TOKEN`` environment variable. You must provide either ``access_token`` or ``oauth_token``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#access_token LaunchdarklyProvider#access_token}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#alias LaunchdarklyProvider#alias}
+        :param api_host: The LaunchDarkly host address. If this argument is not specified, the default host address is ``https://app.launchdarkly.com``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#api_host LaunchdarklyProvider#api_host}
+        :param http_timeout: The HTTP timeout (in seconds) when making API calls to LaunchDarkly. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#http_timeout LaunchdarklyProvider#http_timeout}
+        :param oauth_token: An OAuth V2 token you use to authenticate with LaunchDarkly. You can also set this with the ``LAUNCHDARKLY_OAUTH_TOKEN`` environment variable. You must provide either ``access_token`` or ``oauth_token``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#oauth_token LaunchdarklyProvider#oauth_token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__63a271634d8257ba9984a180dcb9f63b6327bde59eac52f68c8ec5802d84c5e8)
             check_type(argname="argument access_token", value=access_token, expected_type=type_hints["access_token"])
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument api_host", value=api_host, expected_type=type_hints["api_host"])
             check_type(argname="argument http_timeout", value=http_timeout, expected_type=type_hints["http_timeout"])
@@ -256,53 +256,53 @@
         if oauth_token is not None:
             self._values["oauth_token"] = oauth_token
 
     @builtins.property
     def access_token(self) -> typing.Optional[builtins.str]:
         '''The `personal access token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#personal-tokens>`_ or `service token <https://docs.launchdarkly.com/home/account-security/api-access-tokens#service-tokens>`_ used to authenticate with LaunchDarkly. You can also set this with the ``LAUNCHDARKLY_ACCESS_TOKEN`` environment variable. You must provide either ``access_token`` or ``oauth_token``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#access_token LaunchdarklyProvider#access_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#access_token LaunchdarklyProvider#access_token}
         '''
         result = self._values.get("access_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#alias LaunchdarklyProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#alias LaunchdarklyProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def api_host(self) -> typing.Optional[builtins.str]:
         '''The LaunchDarkly host address. If this argument is not specified, the default host address is ``https://app.launchdarkly.com``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#api_host LaunchdarklyProvider#api_host}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#api_host LaunchdarklyProvider#api_host}
         '''
         result = self._values.get("api_host")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def http_timeout(self) -> typing.Optional[jsii.Number]:
         '''The HTTP timeout (in seconds) when making API calls to LaunchDarkly.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#http_timeout LaunchdarklyProvider#http_timeout}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#http_timeout LaunchdarklyProvider#http_timeout}
         '''
         result = self._values.get("http_timeout")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def oauth_token(self) -> typing.Optional[builtins.str]:
         '''An OAuth V2 token you use to authenticate with LaunchDarkly.
 
         You can also set this with the ``LAUNCHDARKLY_OAUTH_TOKEN`` environment variable. You must provide either ``access_token`` or ``oauth_token``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs#oauth_token LaunchdarklyProvider#oauth_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs#oauth_token LaunchdarklyProvider#oauth_token}
         '''
         result = self._values.get("oauth_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/relay_proxy_configuration/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/relay_proxy_configuration/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_relay_proxy_configuration`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_relay_proxy_configuration`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration).
+Refer to the Terraform Registry for docs: [`launchdarkly_relay_proxy_configuration`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class RelayProxyConfiguration(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.relayProxyConfiguration.RelayProxyConfiguration",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration launchdarkly_relay_proxy_configuration}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration launchdarkly_relay_proxy_configuration}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -43,21 +43,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration launchdarkly_relay_proxy_configuration} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration launchdarkly_relay_proxy_configuration} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: A human-friendly name for the Relay Proxy configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#name RelayProxyConfiguration#name}
-        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#policy RelayProxyConfiguration#policy}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#id RelayProxyConfiguration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: A human-friendly name for the Relay Proxy configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#name RelayProxyConfiguration#name}
+        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#policy RelayProxyConfiguration#policy}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#id RelayProxyConfiguration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +90,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a RelayProxyConfiguration resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the RelayProxyConfiguration to import.
-        :param import_from_id: The id of the existing RelayProxyConfiguration that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing RelayProxyConfiguration that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the RelayProxyConfiguration to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0c9500a482f54cfdad52b37020668dc0bd224da1fb9650bc8325b2d71e168420)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -227,17 +227,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: A human-friendly name for the Relay Proxy configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#name RelayProxyConfiguration#name}
-        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#policy RelayProxyConfiguration#policy}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#id RelayProxyConfiguration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: A human-friendly name for the Relay Proxy configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#name RelayProxyConfiguration#name}
+        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#policy RelayProxyConfiguration#policy}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#id RelayProxyConfiguration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0a19f1f503f6b1f5ddbf46ca888b21aec2f7acd97e05b698fbf9dbe43f51df88)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -334,35 +334,35 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''A human-friendly name for the Relay Proxy configuration.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#name RelayProxyConfiguration#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#name RelayProxyConfiguration#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def policy(
         self,
     ) -> typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["RelayProxyConfigurationPolicy"]]:
         '''policy block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#policy RelayProxyConfiguration#policy}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#policy RelayProxyConfiguration#policy}
         '''
         result = self._values.get("policy")
         assert result is not None, "Required property 'policy' is missing"
         return typing.cast(typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["RelayProxyConfigurationPolicy"]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#id RelayProxyConfiguration#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#id RelayProxyConfiguration#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -396,19 +396,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Either ``allow`` or ``deny``. This argument defines whether the statement allows or denies access to the named resources and actions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#effect RelayProxyConfiguration#effect}
-        :param actions: The list of action specifiers defining the actions to which the statement applies. Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#actions RelayProxyConfiguration#actions}
-        :param not_actions: The list of action specifiers defining the actions to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#not_actions RelayProxyConfiguration#not_actions}
-        :param not_resources: The list of resource specifiers defining the resources to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#not_resources RelayProxyConfiguration#not_resources}
-        :param resources: The list of resource specifiers defining the resources to which the statement applies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#resources RelayProxyConfiguration#resources}
+        :param effect: Either ``allow`` or ``deny``. This argument defines whether the statement allows or denies access to the named resources and actions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#effect RelayProxyConfiguration#effect}
+        :param actions: The list of action specifiers defining the actions to which the statement applies. Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#actions RelayProxyConfiguration#actions}
+        :param not_actions: The list of action specifiers defining the actions to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#not_actions RelayProxyConfiguration#not_actions}
+        :param not_resources: The list of resource specifiers defining the resources to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#not_resources RelayProxyConfiguration#not_resources}
+        :param resources: The list of resource specifiers defining the resources to which the statement applies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#resources RelayProxyConfiguration#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ce59738af437ef56ab261cdc60e9461286fbfe18e1bf4f4ae1d8288dcf85c147)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -427,54 +427,54 @@
 
     @builtins.property
     def effect(self) -> builtins.str:
         '''Either ``allow`` or ``deny``.
 
         This argument defines whether the statement allows or denies access to the named resources and actions.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#effect RelayProxyConfiguration#effect}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#effect RelayProxyConfiguration#effect}
         '''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of action specifiers defining the actions to which the statement applies.
 
         Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#actions RelayProxyConfiguration#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#actions RelayProxyConfiguration#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of action specifiers defining the actions to which the statement does not apply.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#not_actions RelayProxyConfiguration#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#not_actions RelayProxyConfiguration#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of resource specifiers defining the resources to which the statement does not apply.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#not_resources RelayProxyConfiguration#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#not_resources RelayProxyConfiguration#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of resource specifiers defining the resources to which the statement applies.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/relay_proxy_configuration#resources RelayProxyConfiguration#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/relay_proxy_configuration#resources RelayProxyConfiguration#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/segment/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/segment/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_segment`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_segment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment).
+Refer to the Terraform Registry for docs: [`launchdarkly_segment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class Segment(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.segment.Segment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment launchdarkly_segment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment launchdarkly_segment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         env_key: builtins.str,
@@ -54,32 +54,32 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment launchdarkly_segment} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment launchdarkly_segment} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param env_key: The segment's environment key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#env_key Segment#env_key}
-        :param key: The unique key that references the segment. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#key Segment#key}
-        :param name: The human-friendly name for the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#name Segment#name}
-        :param project_key: The segment's project key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#project_key Segment#project_key}
-        :param description: The description of the segment's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#description Segment#description}
-        :param excluded: List of user keys excluded from the segment. To target on other context kinds, use the excluded_contexts block attribute. This attribute is not valid when ``unbounded`` is set to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#excluded Segment#excluded}
-        :param excluded_contexts: excluded_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#excluded_contexts Segment#excluded_contexts}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#id Segment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param included: List of user keys included in the segment. To target on other context kinds, use the included_contexts block attribute. This attribute is not valid when ``unbounded`` is set to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#included Segment#included}
-        :param included_contexts: included_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#included_contexts Segment#included_contexts}
-        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#rules Segment#rules}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#tags Segment#tags}
-        :param unbounded: Whether to create a standard segment (``false``) or a Big Segment (``true``). Standard segments include rule-based and smaller list-based segments. Big Segments include larger list-based segments and synced segments. Only use a Big Segment if you need to add more than 15,000 individual targets. It is not possible to manage the list of targeted contexts for Big Segments with Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#unbounded Segment#unbounded}
-        :param unbounded_context_kind: For Big Segments, the targeted context kind. If this attribute is not specified it will default to ``user``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#unbounded_context_kind Segment#unbounded_context_kind}
+        :param env_key: The segment's environment key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#env_key Segment#env_key}
+        :param key: The unique key that references the segment. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#key Segment#key}
+        :param name: The human-friendly name for the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#name Segment#name}
+        :param project_key: The segment's project key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#project_key Segment#project_key}
+        :param description: The description of the segment's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#description Segment#description}
+        :param excluded: List of user keys excluded from the segment. To target on other context kinds, use the excluded_contexts block attribute. This attribute is not valid when ``unbounded`` is set to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#excluded Segment#excluded}
+        :param excluded_contexts: excluded_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#excluded_contexts Segment#excluded_contexts}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#id Segment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param included: List of user keys included in the segment. To target on other context kinds, use the included_contexts block attribute. This attribute is not valid when ``unbounded`` is set to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#included Segment#included}
+        :param included_contexts: included_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#included_contexts Segment#included_contexts}
+        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#rules Segment#rules}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#tags Segment#tags}
+        :param unbounded: Whether to create a standard segment (``false``) or a Big Segment (``true``). Standard segments include rule-based and smaller list-based segments. Big Segments include larger list-based segments and synced segments. Only use a Big Segment if you need to add more than 15,000 individual targets. It is not possible to manage the list of targeted contexts for Big Segments with Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#unbounded Segment#unbounded}
+        :param unbounded_context_kind: For Big Segments, the targeted context kind. If this attribute is not specified it will default to ``user``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#unbounded_context_kind Segment#unbounded_context_kind}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -123,15 +123,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Segment resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Segment to import.
-        :param import_from_id: The id of the existing Segment that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Segment that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Segment to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d563361b02e46803ed18c62be8732cd1f4164094a27ac1ef01893574d839b092)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -521,28 +521,28 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param env_key: The segment's environment key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#env_key Segment#env_key}
-        :param key: The unique key that references the segment. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#key Segment#key}
-        :param name: The human-friendly name for the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#name Segment#name}
-        :param project_key: The segment's project key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#project_key Segment#project_key}
-        :param description: The description of the segment's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#description Segment#description}
-        :param excluded: List of user keys excluded from the segment. To target on other context kinds, use the excluded_contexts block attribute. This attribute is not valid when ``unbounded`` is set to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#excluded Segment#excluded}
-        :param excluded_contexts: excluded_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#excluded_contexts Segment#excluded_contexts}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#id Segment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param included: List of user keys included in the segment. To target on other context kinds, use the included_contexts block attribute. This attribute is not valid when ``unbounded`` is set to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#included Segment#included}
-        :param included_contexts: included_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#included_contexts Segment#included_contexts}
-        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#rules Segment#rules}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#tags Segment#tags}
-        :param unbounded: Whether to create a standard segment (``false``) or a Big Segment (``true``). Standard segments include rule-based and smaller list-based segments. Big Segments include larger list-based segments and synced segments. Only use a Big Segment if you need to add more than 15,000 individual targets. It is not possible to manage the list of targeted contexts for Big Segments with Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#unbounded Segment#unbounded}
-        :param unbounded_context_kind: For Big Segments, the targeted context kind. If this attribute is not specified it will default to ``user``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#unbounded_context_kind Segment#unbounded_context_kind}
+        :param env_key: The segment's environment key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#env_key Segment#env_key}
+        :param key: The unique key that references the segment. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#key Segment#key}
+        :param name: The human-friendly name for the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#name Segment#name}
+        :param project_key: The segment's project key. A change in this field will force the destruction of the existing resource and the creation of a new one. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#project_key Segment#project_key}
+        :param description: The description of the segment's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#description Segment#description}
+        :param excluded: List of user keys excluded from the segment. To target on other context kinds, use the excluded_contexts block attribute. This attribute is not valid when ``unbounded`` is set to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#excluded Segment#excluded}
+        :param excluded_contexts: excluded_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#excluded_contexts Segment#excluded_contexts}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#id Segment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param included: List of user keys included in the segment. To target on other context kinds, use the included_contexts block attribute. This attribute is not valid when ``unbounded`` is set to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#included Segment#included}
+        :param included_contexts: included_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#included_contexts Segment#included_contexts}
+        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#rules Segment#rules}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#tags Segment#tags}
+        :param unbounded: Whether to create a standard segment (``false``) or a Big Segment (``true``). Standard segments include rule-based and smaller list-based segments. Big Segments include larger list-based segments and synced segments. Only use a Big Segment if you need to add more than 15,000 individual targets. It is not possible to manage the list of targeted contexts for Big Segments with Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#unbounded Segment#unbounded}
+        :param unbounded_context_kind: For Big Segments, the targeted context kind. If this attribute is not specified it will default to ``user``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#unbounded_context_kind Segment#unbounded_context_kind}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ed6a1b3a85766111d2daacda6a12b49796357a0f41632344015ce3d5effeb417)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -672,155 +672,155 @@
 
     @builtins.property
     def env_key(self) -> builtins.str:
         '''The segment's environment key.
 
         A change in this field will force the destruction of the existing resource and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#env_key Segment#env_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#env_key Segment#env_key}
         '''
         result = self._values.get("env_key")
         assert result is not None, "Required property 'env_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The unique key that references the segment.
 
         A change in this field will force the destruction of the existing resource and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#key Segment#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#key Segment#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The human-friendly name for the segment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#name Segment#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#name Segment#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The segment's project key.
 
         A change in this field will force the destruction of the existing resource and the creation of a new one.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#project_key Segment#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#project_key Segment#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The description of the segment's purpose.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#description Segment#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#description Segment#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def excluded(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of user keys excluded from the segment.
 
         To target on other context kinds, use the excluded_contexts block attribute. This attribute is not valid when ``unbounded`` is set to ``true``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#excluded Segment#excluded}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#excluded Segment#excluded}
         '''
         result = self._values.get("excluded")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def excluded_contexts(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentExcludedContexts"]]]:
         '''excluded_contexts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#excluded_contexts Segment#excluded_contexts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#excluded_contexts Segment#excluded_contexts}
         '''
         result = self._values.get("excluded_contexts")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentExcludedContexts"]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#id Segment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#id Segment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def included(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of user keys included in the segment.
 
         To target on other context kinds, use the included_contexts block attribute. This attribute is not valid when ``unbounded`` is set to ``true``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#included Segment#included}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#included Segment#included}
         '''
         result = self._values.get("included")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def included_contexts(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentIncludedContexts"]]]:
         '''included_contexts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#included_contexts Segment#included_contexts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#included_contexts Segment#included_contexts}
         '''
         result = self._values.get("included_contexts")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentIncludedContexts"]]], result)
 
     @builtins.property
     def rules(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentRules"]]]:
         '''rules block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#rules Segment#rules}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#rules Segment#rules}
         '''
         result = self._values.get("rules")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentRules"]]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#tags Segment#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#tags Segment#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def unbounded(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether to create a standard segment (``false``) or a Big Segment (``true``).
 
         Standard segments include rule-based and smaller list-based segments. Big Segments include larger list-based segments and synced segments. Only use a Big Segment if you need to add more than 15,000 individual targets. It is not possible to manage the list of targeted contexts for Big Segments with Terraform.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#unbounded Segment#unbounded}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#unbounded Segment#unbounded}
         '''
         result = self._values.get("unbounded")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def unbounded_context_kind(self) -> typing.Optional[builtins.str]:
         '''For Big Segments, the targeted context kind. If this attribute is not specified it will default to ``user``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#unbounded_context_kind Segment#unbounded_context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#unbounded_context_kind Segment#unbounded_context_kind}
         '''
         result = self._values.get("unbounded_context_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -842,41 +842,41 @@
     def __init__(
         self,
         *,
         context_kind: builtins.str,
         values: typing.Sequence[builtins.str],
     ) -> None:
         '''
-        :param context_kind: The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#context_kind Segment#context_kind}
-        :param values: List of target object keys included in or excluded from the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#values Segment#values}
+        :param context_kind: The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#context_kind Segment#context_kind}
+        :param values: List of target object keys included in or excluded from the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#values Segment#values}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__28d6778735b2a7d16c2528dd49eb754dcee6d745bbd461138a998db1616f9b68)
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "context_kind": context_kind,
             "values": values,
         }
 
     @builtins.property
     def context_kind(self) -> builtins.str:
         '''The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#context_kind Segment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#context_kind Segment#context_kind}
         '''
         result = self._values.get("context_kind")
         assert result is not None, "Required property 'context_kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''List of target object keys included in or excluded from the segment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#values Segment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#values Segment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1067,41 +1067,41 @@
     def __init__(
         self,
         *,
         context_kind: builtins.str,
         values: typing.Sequence[builtins.str],
     ) -> None:
         '''
-        :param context_kind: The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#context_kind Segment#context_kind}
-        :param values: List of target object keys included in or excluded from the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#values Segment#values}
+        :param context_kind: The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#context_kind Segment#context_kind}
+        :param values: List of target object keys included in or excluded from the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#values Segment#values}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e25981c1c68a641a81bb8e7eb2bb2fd8444e6a3614ea2665574f3e24bb8f63f3)
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "context_kind": context_kind,
             "values": values,
         }
 
     @builtins.property
     def context_kind(self) -> builtins.str:
         '''The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#context_kind Segment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#context_kind Segment#context_kind}
         '''
         result = self._values.get("context_kind")
         assert result is not None, "Required property 'context_kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''List of target object keys included in or excluded from the segment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#values Segment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#values Segment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1299,18 +1299,18 @@
         *,
         bucket_by: typing.Optional[builtins.str] = None,
         clauses: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["SegmentRulesClauses", typing.Dict[builtins.str, typing.Any]]]]] = None,
         rollout_context_kind: typing.Optional[builtins.str] = None,
         weight: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param bucket_by: The attribute by which to group users together. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#bucket_by Segment#bucket_by}
-        :param clauses: clauses block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#clauses Segment#clauses}
-        :param rollout_context_kind: The context kind associated with this segment rule. This argument is only valid if weight is also specified. If omitted, defaults to 'user' Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#rollout_context_kind Segment#rollout_context_kind}
-        :param weight: The integer weight of the rule (between 1 and 100000). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#weight Segment#weight}
+        :param bucket_by: The attribute by which to group users together. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#bucket_by Segment#bucket_by}
+        :param clauses: clauses block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#clauses Segment#clauses}
+        :param rollout_context_kind: The context kind associated with this segment rule. This argument is only valid if weight is also specified. If omitted, defaults to 'user' Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#rollout_context_kind Segment#rollout_context_kind}
+        :param weight: The integer weight of the rule (between 1 and 100000). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#weight Segment#weight}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0e16d3fe1514553328b2d7b966d78da4ae66991478e0688d26bf0bfb77386c3a)
             check_type(argname="argument bucket_by", value=bucket_by, expected_type=type_hints["bucket_by"])
             check_type(argname="argument clauses", value=clauses, expected_type=type_hints["clauses"])
             check_type(argname="argument rollout_context_kind", value=rollout_context_kind, expected_type=type_hints["rollout_context_kind"])
             check_type(argname="argument weight", value=weight, expected_type=type_hints["weight"])
@@ -1324,46 +1324,46 @@
         if weight is not None:
             self._values["weight"] = weight
 
     @builtins.property
     def bucket_by(self) -> typing.Optional[builtins.str]:
         '''The attribute by which to group users together.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#bucket_by Segment#bucket_by}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#bucket_by Segment#bucket_by}
         '''
         result = self._values.get("bucket_by")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def clauses(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentRulesClauses"]]]:
         '''clauses block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#clauses Segment#clauses}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#clauses Segment#clauses}
         '''
         result = self._values.get("clauses")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentRulesClauses"]]], result)
 
     @builtins.property
     def rollout_context_kind(self) -> typing.Optional[builtins.str]:
         '''The context kind associated with this segment rule.
 
         This argument is only valid if weight is also specified. If omitted, defaults to 'user'
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#rollout_context_kind Segment#rollout_context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#rollout_context_kind Segment#rollout_context_kind}
         '''
         result = self._values.get("rollout_context_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def weight(self) -> typing.Optional[jsii.Number]:
         '''The integer weight of the rule (between 1 and 100000).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#weight Segment#weight}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#weight Segment#weight}
         '''
         result = self._values.get("weight")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1396,20 +1396,20 @@
         op: builtins.str,
         values: typing.Sequence[builtins.str],
         context_kind: typing.Optional[builtins.str] = None,
         negate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         value_type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param attribute: The user attribute to operate on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#attribute Segment#attribute}
-        :param op: The operator associated with the rule clause. Available options are ``in``, ``endsWith``, ``startsWith``, ``matches``, ``contains``, ``lessThan``, ``lessThanOrEqual``, ``greaterThanOrEqual``, ``before``, ``after``, ``segmentMatch``, ``semVerEqual``, ``semVerLessThan``, and ``semVerGreaterThan``. Read LaunchDarkly's `Operators <https://docs.launchdarkly.com/sdk/concepts/flag-evaluation-rules#operators>`_ documentation for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#op Segment#op}
-        :param values: The list of values associated with the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#values Segment#values}
-        :param context_kind: The context kind associated with this rule clause. This argument is only valid if ``rollout_weights`` is also specified. If omitted, defaults to ``user``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#context_kind Segment#context_kind}
-        :param negate: Whether to negate the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#negate Segment#negate}
-        :param value_type: The type for each of the clause's values. Available types are ``boolean``, ``string``, and ``number``. If omitted, ``value_type`` defaults to ``string``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#value_type Segment#value_type}
+        :param attribute: The user attribute to operate on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#attribute Segment#attribute}
+        :param op: The operator associated with the rule clause. Available options are ``in``, ``endsWith``, ``startsWith``, ``matches``, ``contains``, ``lessThan``, ``lessThanOrEqual``, ``greaterThanOrEqual``, ``before``, ``after``, ``segmentMatch``, ``semVerEqual``, ``semVerLessThan``, and ``semVerGreaterThan``. Read LaunchDarkly's `Operators <https://docs.launchdarkly.com/sdk/concepts/flag-evaluation-rules#operators>`_ documentation for more information. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#op Segment#op}
+        :param values: The list of values associated with the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#values Segment#values}
+        :param context_kind: The context kind associated with this rule clause. This argument is only valid if ``rollout_weights`` is also specified. If omitted, defaults to ``user``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#context_kind Segment#context_kind}
+        :param negate: Whether to negate the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#negate Segment#negate}
+        :param value_type: The type for each of the clause's values. Available types are ``boolean``, ``string``, and ``number``. If omitted, ``value_type`` defaults to ``string``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#value_type Segment#value_type}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7311c90332c47a9e3d1696d4575bebbeef73a3698887bf8aaab7fd21a18d62c3)
             check_type(argname="argument attribute", value=attribute, expected_type=type_hints["attribute"])
             check_type(argname="argument op", value=op, expected_type=type_hints["op"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
@@ -1427,71 +1427,71 @@
         if value_type is not None:
             self._values["value_type"] = value_type
 
     @builtins.property
     def attribute(self) -> builtins.str:
         '''The user attribute to operate on.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#attribute Segment#attribute}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#attribute Segment#attribute}
         '''
         result = self._values.get("attribute")
         assert result is not None, "Required property 'attribute' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def op(self) -> builtins.str:
         '''The operator associated with the rule clause.
 
         Available options are ``in``, ``endsWith``, ``startsWith``, ``matches``, ``contains``, ``lessThan``, ``lessThanOrEqual``, ``greaterThanOrEqual``, ``before``, ``after``, ``segmentMatch``, ``semVerEqual``, ``semVerLessThan``, and ``semVerGreaterThan``. Read LaunchDarkly's `Operators <https://docs.launchdarkly.com/sdk/concepts/flag-evaluation-rules#operators>`_ documentation for more information.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#op Segment#op}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#op Segment#op}
         '''
         result = self._values.get("op")
         assert result is not None, "Required property 'op' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''The list of values associated with the rule clause.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#values Segment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#values Segment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def context_kind(self) -> typing.Optional[builtins.str]:
         '''The context kind associated with this rule clause.
 
         This argument is only valid if ``rollout_weights`` is also specified. If omitted, defaults to ``user``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#context_kind Segment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#context_kind Segment#context_kind}
         '''
         result = self._values.get("context_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def negate(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether to negate the rule clause.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#negate Segment#negate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#negate Segment#negate}
         '''
         result = self._values.get("negate")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def value_type(self) -> typing.Optional[builtins.str]:
         '''The type for each of the clause's values.
 
         Available types are ``boolean``, ``string``, and ``number``. If omitted, ``value_type`` defaults to ``string``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/segment#value_type Segment#value_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/segment#value_type Segment#value_type}
         '''
         result = self._values.get("value_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/team/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/team/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_team`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_team`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team).
+Refer to the Terraform Registry for docs: [`launchdarkly_team`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class Team(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.team.Team",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team launchdarkly_team}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team launchdarkly_team}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -47,25 +47,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team launchdarkly_team} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team launchdarkly_team} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#key Team#key}
-        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#name Team#name}
-        :param custom_role_keys: A list of custom role keys for the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#custom_role_keys Team#custom_role_keys}
-        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#description Team#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#id Team#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param maintainers: A list of team maintainer IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#maintainers Team#maintainers}
-        :param member_ids: A list of team member IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#member_ids Team#member_ids}
+        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#key Team#key}
+        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#name Team#name}
+        :param custom_role_keys: A list of custom role keys for the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#custom_role_keys Team#custom_role_keys}
+        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#description Team#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#id Team#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param maintainers: A list of team maintainer IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#maintainers Team#maintainers}
+        :param member_ids: A list of team member IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#member_ids Team#member_ids}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -102,15 +102,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Team resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Team to import.
-        :param import_from_id: The id of the existing Team that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Team that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Team to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ca63e6ad3deeb7951c2c7332134ca7449c0e8cbb6ce1fd7b84416dcda3029380)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -313,21 +313,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#key Team#key}
-        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#name Team#name}
-        :param custom_role_keys: A list of custom role keys for the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#custom_role_keys Team#custom_role_keys}
-        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#description Team#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#id Team#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param maintainers: A list of team maintainer IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#maintainers Team#maintainers}
-        :param member_ids: A list of team member IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#member_ids Team#member_ids}
+        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#key Team#key}
+        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#name Team#name}
+        :param custom_role_keys: A list of custom role keys for the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#custom_role_keys Team#custom_role_keys}
+        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#description Team#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#id Team#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param maintainers: A list of team maintainer IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#maintainers Team#maintainers}
+        :param member_ids: A list of team member IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#member_ids Team#member_ids}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9af27aa374696620d0758031d237c56fb5f86bc739a7a6c4ad6d9fb431f22917)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -436,72 +436,72 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The team's unique key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#key Team#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#key Team#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The team's human-readable name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#name Team#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#name Team#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def custom_role_keys(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of custom role keys for the team.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#custom_role_keys Team#custom_role_keys}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#custom_role_keys Team#custom_role_keys}
         '''
         result = self._values.get("custom_role_keys")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The team's description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#description Team#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#description Team#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#id Team#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#id Team#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def maintainers(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of team maintainer IDs as strings.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#maintainers Team#maintainers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#maintainers Team#maintainers}
         '''
         result = self._values.get("maintainers")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def member_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of team member IDs as strings.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team#member_ids Team#member_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team#member_ids Team#member_ids}
         '''
         result = self._values.get("member_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/team_member/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/team_member/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_team_member`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_team_member`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member).
+Refer to the Terraform Registry for docs: [`launchdarkly_team_member`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class TeamMember(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.teamMember.TeamMember",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member launchdarkly_team_member}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member launchdarkly_team_member}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         email: builtins.str,
@@ -46,24 +46,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member launchdarkly_team_member} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member launchdarkly_team_member} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param email: The team member's email address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#email TeamMember#email}
-        :param custom_roles: IDs or keys of custom roles. Team members must have either a role or custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#custom_roles TeamMember#custom_roles}
-        :param first_name: The team member's first name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#first_name TeamMember#first_name}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#id TeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param last_name: The team member's last name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#last_name TeamMember#last_name}
-        :param role: The team member's role. This must be reader, writer, admin, or no_access. Team members must have either a role or custom role Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#role TeamMember#role}
+        :param email: The team member's email address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#email TeamMember#email}
+        :param custom_roles: IDs or keys of custom roles. Team members must have either a role or custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#custom_roles TeamMember#custom_roles}
+        :param first_name: The team member's first name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#first_name TeamMember#first_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#id TeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param last_name: The team member's last name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#last_name TeamMember#last_name}
+        :param role: The team member's role. This must be reader, writer, admin, or no_access. Team members must have either a role or custom role Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#role TeamMember#role}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -99,15 +99,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a TeamMember resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the TeamMember to import.
-        :param import_from_id: The id of the existing TeamMember that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing TeamMember that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the TeamMember to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3c628c312b4fef6a73adc4bcb1f9b8d1934ff95344a0dfa1f0b04b6b56f8d6c1)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -291,20 +291,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param email: The team member's email address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#email TeamMember#email}
-        :param custom_roles: IDs or keys of custom roles. Team members must have either a role or custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#custom_roles TeamMember#custom_roles}
-        :param first_name: The team member's first name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#first_name TeamMember#first_name}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#id TeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param last_name: The team member's last name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#last_name TeamMember#last_name}
-        :param role: The team member's role. This must be reader, writer, admin, or no_access. Team members must have either a role or custom role Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#role TeamMember#role}
+        :param email: The team member's email address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#email TeamMember#email}
+        :param custom_roles: IDs or keys of custom roles. Team members must have either a role or custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#custom_roles TeamMember#custom_roles}
+        :param first_name: The team member's first name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#first_name TeamMember#first_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#id TeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param last_name: The team member's last name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#last_name TeamMember#last_name}
+        :param role: The team member's role. This must be reader, writer, admin, or no_access. Team members must have either a role or custom role Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#role TeamMember#role}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b534a86927249425d58d28a1f89f74621ad1937c60a2bb4e04e33f522e9edb38)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -411,64 +411,64 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def email(self) -> builtins.str:
         '''The team member's email address.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#email TeamMember#email}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#email TeamMember#email}
         '''
         result = self._values.get("email")
         assert result is not None, "Required property 'email' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def custom_roles(self) -> typing.Optional[typing.List[builtins.str]]:
         '''IDs or keys of custom roles. Team members must have either a role or custom role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#custom_roles TeamMember#custom_roles}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#custom_roles TeamMember#custom_roles}
         '''
         result = self._values.get("custom_roles")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def first_name(self) -> typing.Optional[builtins.str]:
         '''The team member's first name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#first_name TeamMember#first_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#first_name TeamMember#first_name}
         '''
         result = self._values.get("first_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#id TeamMember#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#id TeamMember#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def last_name(self) -> typing.Optional[builtins.str]:
         '''The team member's last name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#last_name TeamMember#last_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#last_name TeamMember#last_name}
         '''
         result = self._values.get("last_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def role(self) -> typing.Optional[builtins.str]:
         '''The team member's role.
 
         This must be reader, writer, admin, or no_access. Team members must have either a role or custom role
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_member#role TeamMember#role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_member#role TeamMember#role}
         '''
         result = self._values.get("role")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/team_role_mapping/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/team_role_mapping/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_team_role_mapping`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_team_role_mapping`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_role_mapping).
+Refer to the Terraform Registry for docs: [`launchdarkly_team_role_mapping`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_role_mapping).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class TeamRoleMapping(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.teamRoleMapping.TeamRoleMapping",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_role_mapping launchdarkly_team_role_mapping}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_role_mapping launchdarkly_team_role_mapping}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         custom_role_keys: typing.Sequence[builtins.str],
@@ -42,20 +42,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_role_mapping launchdarkly_team_role_mapping} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_role_mapping launchdarkly_team_role_mapping} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param custom_role_keys: A set of custom role keys to assign to the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_role_mapping#custom_role_keys TeamRoleMapping#custom_role_keys}
-        :param team_key: The LaunchDarkly team key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_role_mapping#team_key TeamRoleMapping#team_key}
+        :param custom_role_keys: A set of custom role keys to assign to the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_role_mapping#custom_role_keys TeamRoleMapping#custom_role_keys}
+        :param team_key: The LaunchDarkly team key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_role_mapping#team_key TeamRoleMapping#team_key}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -87,15 +87,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a TeamRoleMapping resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the TeamRoleMapping to import.
-        :param import_from_id: The id of the existing TeamRoleMapping that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_role_mapping#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing TeamRoleMapping that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_role_mapping#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the TeamRoleMapping to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__02be9f8444894cd9e40117ba98ea040cf04cb92857308b98cbd675d3dae19a49)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -188,16 +188,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param custom_role_keys: A set of custom role keys to assign to the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_role_mapping#custom_role_keys TeamRoleMapping#custom_role_keys}
-        :param team_key: The LaunchDarkly team key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_role_mapping#team_key TeamRoleMapping#team_key}
+        :param custom_role_keys: A set of custom role keys to assign to the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_role_mapping#custom_role_keys TeamRoleMapping#custom_role_keys}
+        :param team_key: The LaunchDarkly team key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_role_mapping#team_key TeamRoleMapping#team_key}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9147ec9b8844034fd9f3d58395a40af6381c81e08480e78ab70f8cc136547ea3)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -291,25 +291,25 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def custom_role_keys(self) -> typing.List[builtins.str]:
         '''A set of custom role keys to assign to the team.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_role_mapping#custom_role_keys TeamRoleMapping#custom_role_keys}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_role_mapping#custom_role_keys TeamRoleMapping#custom_role_keys}
         '''
         result = self._values.get("custom_role_keys")
         assert result is not None, "Required property 'custom_role_keys' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def team_key(self) -> builtins.str:
         '''The LaunchDarkly team key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/team_role_mapping#team_key TeamRoleMapping#team_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/team_role_mapping#team_key TeamRoleMapping#team_key}
         '''
         result = self._values.get("team_key")
         assert result is not None, "Required property 'team_key' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly/webhook/__init__.py` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly/webhook/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_webhook`
 
-Refer to the Terraform Registry for docs: [`launchdarkly_webhook`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook).
+Refer to the Terraform Registry for docs: [`launchdarkly_webhook`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook).
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
@@ -25,15 +25,15 @@
 
 
 class Webhook(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.webhook.Webhook",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook launchdarkly_webhook}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook launchdarkly_webhook}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         url: builtins.str,
@@ -47,25 +47,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook launchdarkly_webhook} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook launchdarkly_webhook} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param url: The URL of the remote webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#url Webhook#url}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#id Webhook#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#name Webhook#name}
-        :param on: Whether this webhook is enabled or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#on Webhook#on}
-        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#secret Webhook#secret}
-        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#statements Webhook#statements}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#tags Webhook#tags}
+        :param url: The URL of the remote webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#url Webhook#url}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#id Webhook#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#name Webhook#name}
+        :param on: Whether this webhook is enabled or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#on Webhook#on}
+        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#secret Webhook#secret}
+        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#statements Webhook#statements}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#tags Webhook#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -102,15 +102,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Webhook resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Webhook to import.
-        :param import_from_id: The id of the existing Webhook that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Webhook that should be imported. Refer to the {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Webhook to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__706c0e12271d5b9a086a1449ba0299090be0dd04ea2245945d92dc3a110fb7a7)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -330,21 +330,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param url: The URL of the remote webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#url Webhook#url}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#id Webhook#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#name Webhook#name}
-        :param on: Whether this webhook is enabled or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#on Webhook#on}
-        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#secret Webhook#secret}
-        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#statements Webhook#statements}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#tags Webhook#tags}
+        :param url: The URL of the remote webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#url Webhook#url}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#id Webhook#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#name Webhook#name}
+        :param on: Whether this webhook is enabled or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#on Webhook#on}
+        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#secret Webhook#secret}
+        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#statements Webhook#statements}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#tags Webhook#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5c9e9a4f0e4faed0d39cbe1a077065dc1cbc3b6ddcf7bbe8cfa422156560bb7a)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -454,75 +454,75 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def url(self) -> builtins.str:
         '''The URL of the remote webhook.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#url Webhook#url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#url Webhook#url}
         '''
         result = self._values.get("url")
         assert result is not None, "Required property 'url' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#id Webhook#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#id Webhook#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''A human-readable name for your webhook.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#name Webhook#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#name Webhook#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def on(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether this webhook is enabled or not.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#on Webhook#on}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#on Webhook#on}
         '''
         result = self._values.get("on")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def secret(self) -> typing.Optional[builtins.str]:
         '''If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#secret Webhook#secret}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#secret Webhook#secret}
         '''
         result = self._values.get("secret")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def statements(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["WebhookStatements"]]]:
         '''statements block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#statements Webhook#statements}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#statements Webhook#statements}
         '''
         result = self._values.get("statements")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["WebhookStatements"]]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#tags Webhook#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#tags Webhook#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -553,19 +553,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Either ``allow`` or ``deny``. This argument defines whether the statement allows or denies access to the named resources and actions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#effect Webhook#effect}
-        :param actions: The list of action specifiers defining the actions to which the statement applies. Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#actions Webhook#actions}
-        :param not_actions: The list of action specifiers defining the actions to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#not_actions Webhook#not_actions}
-        :param not_resources: The list of resource specifiers defining the resources to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#not_resources Webhook#not_resources}
-        :param resources: The list of resource specifiers defining the resources to which the statement applies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#resources Webhook#resources}
+        :param effect: Either ``allow`` or ``deny``. This argument defines whether the statement allows or denies access to the named resources and actions. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#effect Webhook#effect}
+        :param actions: The list of action specifiers defining the actions to which the statement applies. Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#actions Webhook#actions}
+        :param not_actions: The list of action specifiers defining the actions to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#not_actions Webhook#not_actions}
+        :param not_resources: The list of resource specifiers defining the resources to which the statement does not apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#not_resources Webhook#not_resources}
+        :param resources: The list of resource specifiers defining the resources to which the statement applies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#resources Webhook#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0e3266808ccabb579be833fba2bff85febd8cdca8c3a5bab6b83eef5b88c78d8)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -584,54 +584,54 @@
 
     @builtins.property
     def effect(self) -> builtins.str:
         '''Either ``allow`` or ``deny``.
 
         This argument defines whether the statement allows or denies access to the named resources and actions.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#effect Webhook#effect}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#effect Webhook#effect}
         '''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of action specifiers defining the actions to which the statement applies.
 
         Either ``actions`` or ``not_actions`` must be specified. For a list of available actions read `Actions reference <https://docs.launchdarkly.com/home/account-security/custom-roles/actions#actions-reference>`_.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#actions Webhook#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#actions Webhook#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of action specifiers defining the actions to which the statement does not apply.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#not_actions Webhook#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#not_actions Webhook#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of resource specifiers defining the resources to which the statement does not apply.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#not_resources Webhook#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#not_resources Webhook#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of resource specifiers defining the resources to which the statement applies.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs/resources/webhook#resources Webhook#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs/resources/webhook#resources Webhook#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly.egg-info/PKG-INFO` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-launchdarkly
-Version: 4.1.3
+Version: 4.1.4
 Summary: Prebuilt launchdarkly Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-launchdarkly.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-launchdarkly.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -17,17 +17,17 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CDKTF prebuilt bindings for launchdarkly/launchdarkly provider version 2.18.3
+# CDKTF prebuilt bindings for launchdarkly/launchdarkly provider version 2.18.4
 
-This repo builds and publishes the [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-launchdarkly](https://www.npmjs.com/package/@cdktf/provider-launchdarkly).
 
@@ -81,15 +81,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform launchdarkly provider version 1:1. In fact, it always tracks `latest` of `~> 2.13` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.3)
+* [Terraform launchdarkly provider](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.18.4)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-launchdarkly-4.1.3/src/cdktf_cdktf_provider_launchdarkly.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-launchdarkly-4.1.4/src/cdktf_cdktf_provider_launchdarkly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_launchdarkly/py.typed
 src/cdktf_cdktf_provider_launchdarkly.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_launchdarkly.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_launchdarkly.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_launchdarkly.egg-info/requires.txt
 src/cdktf_cdktf_provider_launchdarkly.egg-info/top_level.txt
 src/cdktf_cdktf_provider_launchdarkly/_jsii/__init__.py
-src/cdktf_cdktf_provider_launchdarkly/_jsii/provider-launchdarkly@4.1.3.jsii.tgz
+src/cdktf_cdktf_provider_launchdarkly/_jsii/provider-launchdarkly@4.1.4.jsii.tgz
 src/cdktf_cdktf_provider_launchdarkly/access_token/__init__.py
 src/cdktf_cdktf_provider_launchdarkly/audit_log_subscription/__init__.py
 src/cdktf_cdktf_provider_launchdarkly/custom_role/__init__.py
 src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_audit_log_subscription/__init__.py
 src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_environment/__init__.py
 src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag/__init__.py
 src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag_environment/__init__.py
```

