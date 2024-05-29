# Comparing `tmp/pulumi_signalfx-7.2.0a1716512682.tar.gz` & `tmp/pulumi_signalfx-7.2.0a1716963243.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_signalfx-7.2.0a1716512682.tar", last modified: Fri May 24 01:09:41 2024, max compression
+gzip compressed data, was "pulumi_signalfx-7.2.0a1716963243.tar", last modified: Wed May 29 06:22:31 2024, max compression
```

## Comparing `pulumi_signalfx-7.2.0a1716512682.tar` & `pulumi_signalfx-7.2.0a1716963243.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:41.178842 pulumi_signalfx-7.2.0a1716512682/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-24 01:09:41.178842 pulumi_signalfx-7.2.0a1716512682/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:41.170842 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   169197 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    18519 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/alert_muting_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:41.174842 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/aws/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/aws/external_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    78469 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/aws/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/aws/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/aws/token_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:41.174842 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/azure/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    51988 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/azure/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/azure/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:41.174842 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    61667 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    32113 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/dashboard_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/data_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    56014 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    17564 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/event_feed_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:41.174842 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/gcp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34395 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/gcp/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/gcp/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/get_dimension_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    40028 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/heatmap_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:41.174842 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/jira/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31138 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/jira/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    59930 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/list_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:41.174842 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/log/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/log/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/log/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20439 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/log/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    26019 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/log/view.py
--rw-r--r--   0 runner    (1001) docker     (127)    18836 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/metric_ruleset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:41.174842 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/opsgenie/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/opsgenie/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    21592 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/org_token.py
--rw-r--r--   0 runner    (1001) docker     (127)   153891 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:41.178842 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/pagerduty/get_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/pagerduty/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:41.178842 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/servicenow/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/servicenow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26431 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/servicenow/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    39002 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/single_value_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:41.178842 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/slack/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/slack/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    16847 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/slo.py
--rw-r--r--   0 runner    (1001) docker     (127)    30799 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/table_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    26819 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/team.py
--rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/text_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    77114 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/time_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:41.178842 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/victorops/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/victorops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/victorops/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/webhook_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:09:41.178842 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-24 01:09:41.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-24 01:09:41.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:09:41.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 01:09:41.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 01:09:41.000000 pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-24 01:09:34.000000 pulumi_signalfx-7.2.0a1716512682/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 01:09:41.178842 pulumi_signalfx-7.2.0a1716512682/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.698932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   169197 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18519 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/alert_muting_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.702932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/external_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78469 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/token_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.702932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51988 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.702932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61667 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32113 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/dashboard_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/data_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56014 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17564 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/event_feed_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.702932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34395 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/get_dimension_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40028 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/heatmap_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31138 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/jira/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59930 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/list_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20439 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26019 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18836 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/metric_ruleset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/opsgenie/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21592 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/org_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)   153891 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/pagerduty/get_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/pagerduty/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/servicenow/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/servicenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26431 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/servicenow/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39002 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/single_value_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/slack/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16847 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/slo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30799 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/table_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26819 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/text_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77114 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/time_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/victorops/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/victorops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/victorops/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/webhook_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-29 06:22:31.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-29 06:22:31.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:22:31.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 06:22:31.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 06:22:31.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/setup.cfg
```

### Comparing `pulumi_signalfx-7.2.0a1716512682/PKG-INFO` & `pulumi_signalfx-7.2.0a1716963243/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_signalfx
-Version: 7.2.0a1716512682
+Version: 7.2.0a1716963243
 Summary: A Pulumi package for creating and managing SignalFx resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi,signalfx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_signalfx-7.2.0a1716512682/README.md` & `pulumi_signalfx-7.2.0a1716963243/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/__init__.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/_inputs.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/_utilities.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/alert_muting_rule.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/alert_muting_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/aws/_inputs.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/aws/external_integration.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/external_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/aws/integration.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/aws/outputs.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/aws/token_integration.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/token_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/azure/_inputs.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/azure/integration.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/azure/outputs.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/config/__init__.pyi` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/config/vars.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/dashboard.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/dashboard_group.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/dashboard_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/data_link.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/data_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/detector.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/detector.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/event_feed_chart.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/event_feed_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/gcp/_inputs.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/gcp/integration.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/gcp/outputs.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/get_dimension_values.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/get_dimension_values.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/heatmap_chart.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/heatmap_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/jira/integration.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/jira/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/list_chart.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/list_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/log/_inputs.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/log/outputs.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/log/timeline.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/timeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/log/view.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/view.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/metric_ruleset.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/metric_ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/opsgenie/integration.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/opsgenie/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/org_token.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/org_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/outputs.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/pagerduty/get_integration.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/pagerduty/get_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/pagerduty/integration.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/pagerduty/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/provider.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/servicenow/integration.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/servicenow/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/single_value_chart.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/single_value_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/slack/integration.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/slack/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/slo.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/slo.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/table_chart.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/table_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/team.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/text_chart.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/text_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/time_chart.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/time_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/victorops/integration.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/victorops/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx/webhook_integration.py` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/webhook_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx.egg-info/PKG-INFO` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_signalfx
-Version: 7.2.0a1716512682
+Version: 7.2.0a1716963243
 Summary: A Pulumi package for creating and managing SignalFx resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi,signalfx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_signalfx-7.2.0a1716512682/pulumi_signalfx.egg-info/SOURCES.txt` & `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716512682/pyproject.toml` & `pulumi_signalfx-7.2.0a1716963243/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_signalfx"
   description = "A Pulumi package for creating and managing SignalFx resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "signalfx"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "7.2.0a1716512682"
+  version = "7.2.0a1716963243"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-signalfx"
 
 [build-system]
```

