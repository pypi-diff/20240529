# Comparing `tmp/pulumi_nutanix-0.0.47.tar.gz` & `tmp/pulumi_nutanix-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_nutanix-0.0.47.tar", last modified: Thu Dec 14 11:27:57 2023, max compression
+gzip compressed data, was "pulumi_nutanix-0.0.48.tar", last modified: Wed May 29 08:28:28 2024, max compression
```

## Comparing `pulumi_nutanix-0.0.47.tar` & `pulumi_nutanix-0.0.48.tar`

### file list

```diff
@@ -1,102 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 11:27:57.000000 pulumi_nutanix-0.0.47/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-12-14 11:27:57.000000 pulumi_nutanix-0.0.47/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 11:27:57.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/
--rw-r--r--   0 runner    (1001) docker     (127)     7590 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   498567 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9301 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    28160 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/access_control_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12841 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/address_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/category_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12177 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/category_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 11:27:57.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    22943 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8348 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/foundation_central_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    43114 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/foundation_central_image_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    14714 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/foundation_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    82103 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/foundation_image_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14148 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/foundation_ipmi_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_access_control_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_access_control_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_address_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_address_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_assert_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_category_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    34769 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_floating_ips.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_central_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    13090 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_central_cluster_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_central_imaged_clusters_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    22245 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_central_imaged_node_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_central_imaged_nodes_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_central_list_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_discover_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_hypervisor_isos.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_nod_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_node_network_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    16969 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14290 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_karbon_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_karbon_cluster_kube_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6430 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_karbon_cluster_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_karbon_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_karbon_private_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_karbon_private_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    38427 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_network_security_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_pbr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_pbrs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21655 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    15807 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_protection_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_protection_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    21550 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_recovery_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_recovery_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_service_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_static_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    20343 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_subnets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13576 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    33844 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_vpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/get_vpcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42511 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    47543 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/karbon_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    19149 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/karbon_private_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)   106910 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/network_security_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)  1109696 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    33029 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/pbr.py
--rw-r--r--   0 runner    (1001) docker     (127)    59828 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    48029 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/protection_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    15072 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   111559 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/recovery_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    22461 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    13370 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/service_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18808 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/static_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    55759 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    29328 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/user.py
--rw-r--r--   0 runner    (1001) docker     (127)   125907 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    27266 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/pulumi_nutanix/vpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 11:27:57.000000 pulumi_nutanix-0.0.47/pulumi_nutanix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-12-14 11:27:57.000000 pulumi_nutanix-0.0.47/pulumi_nutanix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2023-12-14 11:27:57.000000 pulumi_nutanix-0.0.47/pulumi_nutanix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 11:27:57.000000 pulumi_nutanix-0.0.47/pulumi_nutanix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 11:27:57.000000 pulumi_nutanix-0.0.47/pulumi_nutanix.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-14 11:27:57.000000 pulumi_nutanix-0.0.47/pulumi_nutanix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-14 11:27:57.000000 pulumi_nutanix-0.0.47/pulumi_nutanix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 11:27:57.000000 pulumi_nutanix-0.0.47/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-12-14 11:27:56.000000 pulumi_nutanix-0.0.47/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:28:28.032052 pulumi_nutanix-0.0.48/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-29 08:28:28.032052 pulumi_nutanix-0.0.48/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:28:28.028052 pulumi_nutanix-0.0.48/pulumi_nutanix/
+-rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1544197 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28160 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/access_control_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/address_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/category_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/category_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:28:28.032052 pulumi_nutanix-0.0.48/pulumi_nutanix/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22943 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_central_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43114 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_central_image_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14716 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82103 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_image_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14148 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_ipmi_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_access_control_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_access_control_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_address_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_address_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_assert_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_category_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34769 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_floating_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_cluster_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_imaged_clusters_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22245 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_imaged_node_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_imaged_nodes_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_list_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_discover_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_hypervisor_isos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_node_network_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_nos_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16969 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14290 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_cluster_kube_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_cluster_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_private_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_private_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19472 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_clones.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15150 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21835 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_dbserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_dbservers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_maintenance_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_network_available_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_sla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_slas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24744 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_time_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_time_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_tms_capability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38429 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_network_security_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_pbr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_pbrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24933 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_protection_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_protection_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_recovery_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_recovery_plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_service_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_static_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20343 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13576 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33940 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/get_vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42511 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52706 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/karbon_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19115 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/karbon_private_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18915 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/karbon_worker_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_authorize_dbserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92262 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_clone_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47795 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98121 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46080 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_database_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47875 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_database_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57356 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_database_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60370 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_dbserver_vm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_linked_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13680 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_log_catchups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19404 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_maintenance_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34180 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28661 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90606 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_register_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56422 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_register_dbserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47875 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_scale_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29991 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_sla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31118 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_software_version_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18305 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_stretched_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22819 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/ndb_tms_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106914 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/network_security_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2714710 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30289 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/pbr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67188 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26646 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/protection_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17818 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18624 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/recovery_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22461 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/service_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18834 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/static_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60420 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29328 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21199 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128659 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27270 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix/vpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:28:28.032052 pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:28:28.032052 pulumi_nutanix-0.0.48/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-29 08:28:27.000000 pulumi_nutanix-0.0.48/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pulumi_nutanix-0.0.47/PKG-INFO` & `pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,67 @@
 Metadata-Version: 2.1
-Name: pulumi_nutanix
-Version: 0.0.47
+Name: pulumi-nutanix
+Version: 0.0.48
 Summary: A Pulumi package for creating and managing nutanix cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-nutanix
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-nutanix
-Description: # Nutanix Resource Provider
-        
-        The Nutanix Resource Provider lets you manage [Nutanix](http://example.com) resources.
-        
-        ## Installing
-        
-        This package is available for several languages/platforms:
-        
-        ### Node.js (JavaScript/TypeScript)
-        
-        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-        
-        ```bash
-        npm install @pierskarsenbarg/pulumi-nutanix
-        ```
-        
-        or `yarn`:
-        
-        ```bash
-        yarn add @pierskarsenbarg/pulumi-nutanix
-        ```
-        
-        ### Python
-        
-        To use from Python, install using `pip`:
-        
-        ```bash
-        pip install pulumi_nutanix
-        ```
-        
-        ### Go
-        
-        To use from Go, use `go get` to grab the latest version of the library:
-        
-        ```bash
-        go get github.com/pierskarsenbarg/pulumi-nutanix/sdk/go/...
-        ```
-        
-        ### .NET
-        
-        To use from .NET, install using `dotnet add package`:
-        
-        ```bash
-        dotnet add package PiersKarsenbarg.Nutanix
-        ```
-        
-        ## Configuration
-        
-        The following configuration points are available for the `nutanix` provider:
-        
-        - `nutanix:apiKey` (environment: `NUTANIX_API_KEY`) - the API key for `nutanix`
-        - `nutanix:region` (environment: `NUTANIX_REGION`) - the region in which to deploy resources
-        
-        ## Reference
-        
-        For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/foo/api-docs/).
-        
 Keywords: pulumi nutanix category/cloud
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+
+# Nutanix Resource Provider
+
+The Nutanix Resource Provider lets you manage [Nutanix](http://example.com) resources.
+
+## Installing
+
+This package is available for several languages/platforms:
+
+### Node.js (JavaScript/TypeScript)
+
+To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+
+```bash
+npm install @pierskarsenbarg/pulumi-nutanix
+```
+
+or `yarn`:
+
+```bash
+yarn add @pierskarsenbarg/pulumi-nutanix
+```
+
+### Python
+
+To use from Python, install using `pip`:
+
+```bash
+pip install pulumi_nutanix
+```
+
+### Go
+
+To use from Go, use `go get` to grab the latest version of the library:
+
+```bash
+go get github.com/pierskarsenbarg/pulumi-nutanix/sdk/go/...
+```
+
+### .NET
+
+To use from .NET, install using `dotnet add package`:
+
+```bash
+dotnet add package PiersKarsenbarg.Nutanix
+```
+
+## Configuration
+
+The following configuration points are available for the `nutanix` provider:
+
+- `nutanix:apiKey` (environment: `NUTANIX_API_KEY`) - the API key for `nutanix`
+- `nutanix:region` (environment: `NUTANIX_REGION`) - the region in which to deploy resources
+
+## Reference
+
+For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/foo/api-docs/).
```

### Comparing `pulumi_nutanix-0.0.47/README.md` & `pulumi_nutanix-0.0.48/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/_utilities.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 
 import asyncio
+import importlib.metadata
 import importlib.util
 import inspect
 import json
 import os
-import pkg_resources
 import sys
 import typing
 
 import pulumi
 import pulumi.runtime
 from pulumi.runtime.sync_await import _sync_await
 
@@ -68,15 +68,15 @@
     # pkg_resources uses setuptools to inspect the set of installed packages. We use it here to ask
     # for the currently installed version of the root package (i.e. us) and get its version.
 
     # Unfortunately, PEP440 and semver differ slightly in incompatible ways. The Pulumi engine expects
     # to receive a valid semver string when receiving requests from the language host, so it's our
     # responsibility as the library to convert our own PEP440 version into a valid semver string.
 
-    pep440_version_string = pkg_resources.require(root_package)[0].version
+    pep440_version_string = importlib.metadata.version(root_package)
     pep440_version = PEP440Version.parse(pep440_version_string)
     (major, minor, patch) = pep440_version.release
     prerelease = None
     if pep440_version.pre_tag == 'a':
         prerelease = f"alpha.{pep440_version.pre}"
     elif pep440_version.pre_tag == 'b':
         prerelease = f"beta.{pep440_version.pre}"
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/access_control_policy.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/access_control_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/address_group.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/address_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/category_key.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/category_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/category_value.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/category_value.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/config/vars.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/config/vars.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,14 +42,29 @@
     def insecure(self) -> Optional[bool]:
         """
         Explicitly allow the provider to perform "insecure" SSL requests. If omitted,default value is `false`
         """
         return __config__.get_bool('insecure')
 
     @property
+    def ndb_endpoint(self) -> Optional[str]:
+        """
+        endpoint for Era VM (era ip)
+        """
+        return __config__.get('ndbEndpoint')
+
+    @property
+    def ndb_password(self) -> Optional[str]:
+        return __config__.get('ndbPassword')
+
+    @property
+    def ndb_username(self) -> Optional[str]:
+        return __config__.get('ndbUsername')
+
+    @property
     def password(self) -> Optional[str]:
         """
         Password for provided user name.
         """
         return __config__.get('password')
 
     @property
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/floating_ip.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/floating_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/foundation_central_api_keys.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_central_api_keys.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,20 +13,24 @@
 
 @pulumi.input_type
 class FoundationCentralApiKeysArgs:
     def __init__(__self__, *,
                  alias: pulumi.Input[str]):
         """
         The set of arguments for constructing a FoundationCentralApiKeys resource.
+        :param pulumi.Input[str] alias: - (Required) Alias for the api key to be created.
         """
         pulumi.set(__self__, "alias", alias)
 
     @property
     @pulumi.getter
     def alias(self) -> pulumi.Input[str]:
+        """
+        - (Required) Alias for the api key to be created.
+        """
         return pulumi.get(self, "alias")
 
     @alias.setter
     def alias(self, value: pulumi.Input[str]):
         pulumi.set(self, "alias", value)
 
 
@@ -36,14 +40,19 @@
                  alias: Optional[pulumi.Input[str]] = None,
                  api_key: Optional[pulumi.Input[str]] = None,
                  created_timestamp: Optional[pulumi.Input[str]] = None,
                  current_time: Optional[pulumi.Input[str]] = None,
                  key_uuid: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering FoundationCentralApiKeys resources.
+        :param pulumi.Input[str] alias: - (Required) Alias for the api key to be created.
+        :param pulumi.Input[str] api_key: Api key in string format.
+        :param pulumi.Input[str] created_timestamp: Time when the api key was created.
+        :param pulumi.Input[str] current_time: Current time of Foundation Central.
+        :param pulumi.Input[str] key_uuid: UUID of the api key.
         """
         if alias is not None:
             pulumi.set(__self__, "alias", alias)
         if api_key is not None:
             pulumi.set(__self__, "api_key", api_key)
         if created_timestamp is not None:
             pulumi.set(__self__, "created_timestamp", created_timestamp)
@@ -51,50 +60,65 @@
             pulumi.set(__self__, "current_time", current_time)
         if key_uuid is not None:
             pulumi.set(__self__, "key_uuid", key_uuid)
 
     @property
     @pulumi.getter
     def alias(self) -> Optional[pulumi.Input[str]]:
+        """
+        - (Required) Alias for the api key to be created.
+        """
         return pulumi.get(self, "alias")
 
     @alias.setter
     def alias(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "alias", value)
 
     @property
     @pulumi.getter(name="apiKey")
     def api_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        Api key in string format.
+        """
         return pulumi.get(self, "api_key")
 
     @api_key.setter
     def api_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_key", value)
 
     @property
     @pulumi.getter(name="createdTimestamp")
     def created_timestamp(self) -> Optional[pulumi.Input[str]]:
+        """
+        Time when the api key was created.
+        """
         return pulumi.get(self, "created_timestamp")
 
     @created_timestamp.setter
     def created_timestamp(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_timestamp", value)
 
     @property
     @pulumi.getter(name="currentTime")
     def current_time(self) -> Optional[pulumi.Input[str]]:
+        """
+        Current time of Foundation Central.
+        """
         return pulumi.get(self, "current_time")
 
     @current_time.setter
     def current_time(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "current_time", value)
 
     @property
     @pulumi.getter(name="keyUuid")
     def key_uuid(self) -> Optional[pulumi.Input[str]]:
+        """
+        UUID of the api key.
+        """
         return pulumi.get(self, "key_uuid")
 
     @key_uuid.setter
     def key_uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_uuid", value)
 
 
@@ -102,26 +126,47 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  alias: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a FoundationCentralApiKeys resource with the given unique name, props, and options.
+        Provides a resource to create a new API key for nodes registration with Foundation Central.
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_nutanix as nutanix
+
+        new_api_key = nutanix.FoundationCentralApiKeys("newApiKey", alias="<NAME-FOR-API-KEY>")
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] alias: - (Required) Alias for the api key to be created.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: FoundationCentralApiKeysArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a FoundationCentralApiKeys resource with the given unique name, props, and options.
+        Provides a resource to create a new API key for nodes registration with Foundation Central.
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_nutanix as nutanix
+
+        new_api_key = nutanix.FoundationCentralApiKeys("newApiKey", alias="<NAME-FOR-API-KEY>")
+        ```
+
         :param str resource_name: The name of the resource.
         :param FoundationCentralApiKeysArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(FoundationCentralApiKeysArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -168,14 +213,19 @@
         """
         Get an existing FoundationCentralApiKeys resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] alias: - (Required) Alias for the api key to be created.
+        :param pulumi.Input[str] api_key: Api key in string format.
+        :param pulumi.Input[str] created_timestamp: Time when the api key was created.
+        :param pulumi.Input[str] current_time: Current time of Foundation Central.
+        :param pulumi.Input[str] key_uuid: UUID of the api key.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _FoundationCentralApiKeysState.__new__(_FoundationCentralApiKeysState)
 
         __props__.__dict__["alias"] = alias
         __props__.__dict__["api_key"] = api_key
@@ -183,29 +233,44 @@
         __props__.__dict__["current_time"] = current_time
         __props__.__dict__["key_uuid"] = key_uuid
         return FoundationCentralApiKeys(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def alias(self) -> pulumi.Output[str]:
+        """
+        - (Required) Alias for the api key to be created.
+        """
         return pulumi.get(self, "alias")
 
     @property
     @pulumi.getter(name="apiKey")
     def api_key(self) -> pulumi.Output[str]:
+        """
+        Api key in string format.
+        """
         return pulumi.get(self, "api_key")
 
     @property
     @pulumi.getter(name="createdTimestamp")
     def created_timestamp(self) -> pulumi.Output[str]:
+        """
+        Time when the api key was created.
+        """
         return pulumi.get(self, "created_timestamp")
 
     @property
     @pulumi.getter(name="currentTime")
     def current_time(self) -> pulumi.Output[str]:
+        """
+        Current time of Foundation Central.
+        """
         return pulumi.get(self, "current_time")
 
     @property
     @pulumi.getter(name="keyUuid")
     def key_uuid(self) -> pulumi.Output[str]:
+        """
+        UUID of the api key.
+        """
         return pulumi.get(self, "key_uuid")
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/foundation_central_image_cluster.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_central_image_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/foundation_image.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,14 +191,15 @@
             installer_type="nos",
             source="../../../files/nutanix_installer_x86_64.tar")
         hypervisor_image = nutanix.FoundationImage("hypervisor-image",
             filename="esx_image.iso",
             installer_type="esx",
             source="../../../files/VMware-Installer.x86_64.iso")
         ```
+
         ## lifecycle
 
         * `Update` : - Resource will trigger new resource create call for any kind of update in resource config and delete existing image from foundation vm.
 
         See detailed information in [Nutanix Foundation Image](https://www.nutanix.dev/api_references/foundation/#/b3A6MjIyMjM0MDQ-upload-hypervisor-or-aos-image-to-foundation).
 
         :param str resource_name: The name of the resource.
@@ -227,14 +228,15 @@
             installer_type="nos",
             source="../../../files/nutanix_installer_x86_64.tar")
         hypervisor_image = nutanix.FoundationImage("hypervisor-image",
             filename="esx_image.iso",
             installer_type="esx",
             source="../../../files/VMware-Installer.x86_64.iso")
         ```
+
         ## lifecycle
 
         * `Update` : - Resource will trigger new resource create call for any kind of update in resource config and delete existing image from foundation vm.
 
         See detailed information in [Nutanix Foundation Image](https://www.nutanix.dev/api_references/foundation/#/b3A6MjIyMjM0MDQ-upload-hypervisor-or-aos-image-to-foundation).
 
         :param str resource_name: The name of the resource.
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/foundation_image_nodes.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_image_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/foundation_ipmi_config.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/foundation_ipmi_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_access_control_policies.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_access_control_policies.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,21 +85,14 @@
 def get_access_control_policies(metadatas: Optional[Sequence[pulumi.InputType['GetAccessControlPoliciesMetadataArgs']]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAccessControlPoliciesResult:
     """
     Describes a list of access control policies.
 
     ## Example Usage
 
-    ```python
-    import pulumi
-    import pulumi_nutanix as nutanix
-
-    test = nutanix.get_access_control_policies()
-    ```
-
 
     :param Sequence[pulumi.InputType['GetAccessControlPoliciesMetadataArgs']] metadatas: - The Access Control Policy kind metadata.
     """
     __args__ = dict()
     __args__['metadatas'] = metadatas
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('nutanix:index/getAccessControlPolicies:getAccessControlPolicies', __args__, opts=opts, typ=GetAccessControlPoliciesResult).value
@@ -115,18 +108,11 @@
 def get_access_control_policies_output(metadatas: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetAccessControlPoliciesMetadataArgs']]]]] = None,
                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAccessControlPoliciesResult]:
     """
     Describes a list of access control policies.
 
     ## Example Usage
 
-    ```python
-    import pulumi
-    import pulumi_nutanix as nutanix
-
-    test = nutanix.get_access_control_policies()
-    ```
-
 
     :param Sequence[pulumi.InputType['GetAccessControlPoliciesMetadataArgs']] metadatas: - The Access Control Policy kind metadata.
     """
     ...
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_access_control_policy.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_access_control_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_address_group.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_address_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_address_groups.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_address_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_assert_helper.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_assert_helper.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_category_key.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_category_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_cluster.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_clusters.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_clusters.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 
     ```python
     import pulumi
     import pulumi_nutanix as nutanix
 
     clusters = nutanix.get_clusters()
     ```
+
     ## Reference
 
     The `project_reference`, `owner_reference`, `availability_zone_reference`, `cluster_reference`, attributes supports the following:
 
     * `kind`: - The kind name (Default value: project).
     * `name`: - the name.
     * `UUID`: - the UUID.
@@ -92,15 +93,15 @@
     ### Version
 
     The version attribute supports the following:
 
     * `product_name`: - Name of the producer/distribution of the image. For example windows or red hat.
     * `product_version`: - Version string for the disk image.
 
-    See detailed information in [Nutanix Image](https://nutanix.github.io/Automation/experimental/swagger-redoc-sandbox/#tag/clusters/paths/~1clusters~1multicluster_config/post).
+    See detailed information in [Nutanix Clusters](https://www.nutanix.dev/api_references/prism-central-v3/#/d93c30e04327e-get-a-list-of-existing-clusters).
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('nutanix:index/getClusters:getClusters', __args__, opts=opts, typ=GetClustersResult).value
 
     return AwaitableGetClustersResult(
         api_version=pulumi.get(__ret__, 'api_version'),
@@ -117,14 +118,15 @@
 
     ```python
     import pulumi
     import pulumi_nutanix as nutanix
 
     clusters = nutanix.get_clusters()
     ```
+
     ## Reference
 
     The `project_reference`, `owner_reference`, `availability_zone_reference`, `cluster_reference`, attributes supports the following:
 
     * `kind`: - The kind name (Default value: project).
     * `name`: - the name.
     * `UUID`: - the UUID.
@@ -132,10 +134,10 @@
     ### Version
 
     The version attribute supports the following:
 
     * `product_name`: - Name of the producer/distribution of the image. For example windows or red hat.
     * `product_version`: - Version string for the disk image.
 
-    See detailed information in [Nutanix Image](https://nutanix.github.io/Automation/experimental/swagger-redoc-sandbox/#tag/clusters/paths/~1clusters~1multicluster_config/post).
+    See detailed information in [Nutanix Clusters](https://www.nutanix.dev/api_references/prism-central-v3/#/d93c30e04327e-get-a-list-of-existing-clusters).
     """
     ...
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_floating_ip.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_floating_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_floating_ips.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_floating_ips.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_central_api_keys.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_api_keys.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,42 +40,57 @@
         if key_uuid and not isinstance(key_uuid, str):
             raise TypeError("Expected argument 'key_uuid' to be a str")
         pulumi.set(__self__, "key_uuid", key_uuid)
 
     @property
     @pulumi.getter
     def alias(self) -> str:
+        """
+        Alias of the api key.
+        """
         return pulumi.get(self, "alias")
 
     @property
     @pulumi.getter(name="apiKey")
     def api_key(self) -> str:
+        """
+        Api key in string format.
+        """
         return pulumi.get(self, "api_key")
 
     @property
     @pulumi.getter(name="createdTimestamp")
     def created_timestamp(self) -> str:
+        """
+        Time when the api key was created.
+        """
         return pulumi.get(self, "created_timestamp")
 
     @property
     @pulumi.getter(name="currentTime")
     def current_time(self) -> str:
+        """
+        Current time of Foundation Central.
+        """
         return pulumi.get(self, "current_time")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="keyUuid")
     def key_uuid(self) -> str:
+        """
+        UUID of the api key.
+        """
         return pulumi.get(self, "key_uuid")
 
 
 class AwaitableGetFoundationCentralApiKeysResult(GetFoundationCentralApiKeysResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -88,15 +103,27 @@
             id=self.id,
             key_uuid=self.key_uuid)
 
 
 def get_foundation_central_api_keys(key_uuid: Optional[str] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFoundationCentralApiKeysResult:
     """
-    Use this data source to access information about an existing resource.
+    Get an api key given its UUID.
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_nutanix as nutanix
+
+    api_keys_list = nutanix.get_foundation_central_api_keys(key_uuid="<KEY_UUID>")
+    ```
+
+
+    :param str key_uuid: UUID of the key which needs to be fetched.
     """
     __args__ = dict()
     __args__['keyUuid'] = key_uuid
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('nutanix:index/getFoundationCentralApiKeys:getFoundationCentralApiKeys', __args__, opts=opts, typ=GetFoundationCentralApiKeysResult).value
 
     return AwaitableGetFoundationCentralApiKeysResult(
@@ -108,10 +135,22 @@
         key_uuid=pulumi.get(__ret__, 'key_uuid'))
 
 
 @_utilities.lift_output_func(get_foundation_central_api_keys)
 def get_foundation_central_api_keys_output(key_uuid: Optional[pulumi.Input[str]] = None,
                                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFoundationCentralApiKeysResult]:
     """
-    Use this data source to access information about an existing resource.
+    Get an api key given its UUID.
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_nutanix as nutanix
+
+    api_keys_list = nutanix.get_foundation_central_api_keys(key_uuid="<KEY_UUID>")
+    ```
+
+
+    :param str key_uuid: UUID of the key which needs to be fetched.
     """
     ...
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_central_cluster_details.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_ndb_tms_capability.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,246 +5,234 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
-from ._inputs import *
 
 __all__ = [
-    'GetFoundationCentralClusterDetailsResult',
-    'AwaitableGetFoundationCentralClusterDetailsResult',
-    'get_foundation_central_cluster_details',
-    'get_foundation_central_cluster_details_output',
+    'GetNdbTmsCapabilityResult',
+    'AwaitableGetNdbTmsCapabilityResult',
+    'get_ndb_tms_capability',
+    'get_ndb_tms_capability_output',
 ]
 
 @pulumi.output_type
-class GetFoundationCentralClusterDetailsResult:
+class GetNdbTmsCapabilityResult:
     """
-    A collection of values returned by getFoundationCentralClusterDetails.
+    A collection of values returned by getNdbTmsCapability.
     """
-    def __init__(__self__, archived=None, cluster_external_ip=None, cluster_name=None, cluster_size=None, cluster_status=None, common_network_settings=None, created_timestamp=None, current_time=None, destroyed=None, foundation_init_configs=None, foundation_init_node_uuid=None, id=None, imaged_cluster_uuid=None, imaged_node_uuid_lists=None, redundancy_factor=None, storage_node_count=None, workflow_type=None):
-        if archived and not isinstance(archived, bool):
-            raise TypeError("Expected argument 'archived' to be a bool")
-        pulumi.set(__self__, "archived", archived)
-        if cluster_external_ip and not isinstance(cluster_external_ip, str):
-            raise TypeError("Expected argument 'cluster_external_ip' to be a str")
-        pulumi.set(__self__, "cluster_external_ip", cluster_external_ip)
-        if cluster_name and not isinstance(cluster_name, str):
-            raise TypeError("Expected argument 'cluster_name' to be a str")
-        pulumi.set(__self__, "cluster_name", cluster_name)
-        if cluster_size and not isinstance(cluster_size, int):
-            raise TypeError("Expected argument 'cluster_size' to be a int")
-        pulumi.set(__self__, "cluster_size", cluster_size)
-        if cluster_status and not isinstance(cluster_status, dict):
-            raise TypeError("Expected argument 'cluster_status' to be a dict")
-        pulumi.set(__self__, "cluster_status", cluster_status)
-        if common_network_settings and not isinstance(common_network_settings, dict):
-            raise TypeError("Expected argument 'common_network_settings' to be a dict")
-        pulumi.set(__self__, "common_network_settings", common_network_settings)
-        if created_timestamp and not isinstance(created_timestamp, str):
-            raise TypeError("Expected argument 'created_timestamp' to be a str")
-        pulumi.set(__self__, "created_timestamp", created_timestamp)
-        if current_time and not isinstance(current_time, str):
-            raise TypeError("Expected argument 'current_time' to be a str")
-        pulumi.set(__self__, "current_time", current_time)
-        if destroyed and not isinstance(destroyed, bool):
-            raise TypeError("Expected argument 'destroyed' to be a bool")
-        pulumi.set(__self__, "destroyed", destroyed)
-        if foundation_init_configs and not isinstance(foundation_init_configs, list):
-            raise TypeError("Expected argument 'foundation_init_configs' to be a list")
-        pulumi.set(__self__, "foundation_init_configs", foundation_init_configs)
-        if foundation_init_node_uuid and not isinstance(foundation_init_node_uuid, str):
-            raise TypeError("Expected argument 'foundation_init_node_uuid' to be a str")
-        pulumi.set(__self__, "foundation_init_node_uuid", foundation_init_node_uuid)
+    def __init__(__self__, capabilities=None, capability_reset_time=None, database_ids=None, heal_with_reset_capability=None, id=None, last_continuous_snapshot_time=None, last_continuous_snapshots=None, last_db_logs=None, log_catchup_start_time=None, log_time_info=None, nx_cluster_association_type=None, nx_cluster_id=None, output_time_zone=None, overall_continuous_range_end_time=None, sla_id=None, source=None, time_machine_id=None, type=None):
+        if capabilities and not isinstance(capabilities, list):
+            raise TypeError("Expected argument 'capabilities' to be a list")
+        pulumi.set(__self__, "capabilities", capabilities)
+        if capability_reset_time and not isinstance(capability_reset_time, str):
+            raise TypeError("Expected argument 'capability_reset_time' to be a str")
+        pulumi.set(__self__, "capability_reset_time", capability_reset_time)
+        if database_ids and not isinstance(database_ids, list):
+            raise TypeError("Expected argument 'database_ids' to be a list")
+        pulumi.set(__self__, "database_ids", database_ids)
+        if heal_with_reset_capability and not isinstance(heal_with_reset_capability, bool):
+            raise TypeError("Expected argument 'heal_with_reset_capability' to be a bool")
+        pulumi.set(__self__, "heal_with_reset_capability", heal_with_reset_capability)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if imaged_cluster_uuid and not isinstance(imaged_cluster_uuid, str):
-            raise TypeError("Expected argument 'imaged_cluster_uuid' to be a str")
-        pulumi.set(__self__, "imaged_cluster_uuid", imaged_cluster_uuid)
-        if imaged_node_uuid_lists and not isinstance(imaged_node_uuid_lists, list):
-            raise TypeError("Expected argument 'imaged_node_uuid_lists' to be a list")
-        pulumi.set(__self__, "imaged_node_uuid_lists", imaged_node_uuid_lists)
-        if redundancy_factor and not isinstance(redundancy_factor, int):
-            raise TypeError("Expected argument 'redundancy_factor' to be a int")
-        pulumi.set(__self__, "redundancy_factor", redundancy_factor)
-        if storage_node_count and not isinstance(storage_node_count, int):
-            raise TypeError("Expected argument 'storage_node_count' to be a int")
-        pulumi.set(__self__, "storage_node_count", storage_node_count)
-        if workflow_type and not isinstance(workflow_type, str):
-            raise TypeError("Expected argument 'workflow_type' to be a str")
-        pulumi.set(__self__, "workflow_type", workflow_type)
+        if last_continuous_snapshot_time and not isinstance(last_continuous_snapshot_time, str):
+            raise TypeError("Expected argument 'last_continuous_snapshot_time' to be a str")
+        pulumi.set(__self__, "last_continuous_snapshot_time", last_continuous_snapshot_time)
+        if last_continuous_snapshots and not isinstance(last_continuous_snapshots, list):
+            raise TypeError("Expected argument 'last_continuous_snapshots' to be a list")
+        pulumi.set(__self__, "last_continuous_snapshots", last_continuous_snapshots)
+        if last_db_logs and not isinstance(last_db_logs, list):
+            raise TypeError("Expected argument 'last_db_logs' to be a list")
+        pulumi.set(__self__, "last_db_logs", last_db_logs)
+        if log_catchup_start_time and not isinstance(log_catchup_start_time, str):
+            raise TypeError("Expected argument 'log_catchup_start_time' to be a str")
+        pulumi.set(__self__, "log_catchup_start_time", log_catchup_start_time)
+        if log_time_info and not isinstance(log_time_info, dict):
+            raise TypeError("Expected argument 'log_time_info' to be a dict")
+        pulumi.set(__self__, "log_time_info", log_time_info)
+        if nx_cluster_association_type and not isinstance(nx_cluster_association_type, str):
+            raise TypeError("Expected argument 'nx_cluster_association_type' to be a str")
+        pulumi.set(__self__, "nx_cluster_association_type", nx_cluster_association_type)
+        if nx_cluster_id and not isinstance(nx_cluster_id, str):
+            raise TypeError("Expected argument 'nx_cluster_id' to be a str")
+        pulumi.set(__self__, "nx_cluster_id", nx_cluster_id)
+        if output_time_zone and not isinstance(output_time_zone, str):
+            raise TypeError("Expected argument 'output_time_zone' to be a str")
+        pulumi.set(__self__, "output_time_zone", output_time_zone)
+        if overall_continuous_range_end_time and not isinstance(overall_continuous_range_end_time, str):
+            raise TypeError("Expected argument 'overall_continuous_range_end_time' to be a str")
+        pulumi.set(__self__, "overall_continuous_range_end_time", overall_continuous_range_end_time)
+        if sla_id and not isinstance(sla_id, str):
+            raise TypeError("Expected argument 'sla_id' to be a str")
+        pulumi.set(__self__, "sla_id", sla_id)
+        if source and not isinstance(source, bool):
+            raise TypeError("Expected argument 'source' to be a bool")
+        pulumi.set(__self__, "source", source)
+        if time_machine_id and not isinstance(time_machine_id, str):
+            raise TypeError("Expected argument 'time_machine_id' to be a str")
+        pulumi.set(__self__, "time_machine_id", time_machine_id)
+        if type and not isinstance(type, str):
+            raise TypeError("Expected argument 'type' to be a str")
+        pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
-    def archived(self) -> bool:
-        return pulumi.get(self, "archived")
+    def capabilities(self) -> Sequence['outputs.GetNdbTmsCapabilityCapabilityResult']:
+        return pulumi.get(self, "capabilities")
 
     @property
-    @pulumi.getter(name="clusterExternalIp")
-    def cluster_external_ip(self) -> str:
-        return pulumi.get(self, "cluster_external_ip")
+    @pulumi.getter(name="capabilityResetTime")
+    def capability_reset_time(self) -> str:
+        return pulumi.get(self, "capability_reset_time")
 
     @property
-    @pulumi.getter(name="clusterName")
-    def cluster_name(self) -> str:
-        return pulumi.get(self, "cluster_name")
+    @pulumi.getter(name="databaseIds")
+    def database_ids(self) -> Sequence[str]:
+        return pulumi.get(self, "database_ids")
 
     @property
-    @pulumi.getter(name="clusterSize")
-    def cluster_size(self) -> int:
-        return pulumi.get(self, "cluster_size")
+    @pulumi.getter(name="healWithResetCapability")
+    def heal_with_reset_capability(self) -> bool:
+        return pulumi.get(self, "heal_with_reset_capability")
 
     @property
-    @pulumi.getter(name="clusterStatus")
-    def cluster_status(self) -> 'outputs.GetFoundationCentralClusterDetailsClusterStatusResult':
-        return pulumi.get(self, "cluster_status")
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The provider-assigned unique ID for this managed resource.
+        """
+        return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="commonNetworkSettings")
-    def common_network_settings(self) -> 'outputs.GetFoundationCentralClusterDetailsCommonNetworkSettingsResult':
-        return pulumi.get(self, "common_network_settings")
+    @pulumi.getter(name="lastContinuousSnapshotTime")
+    def last_continuous_snapshot_time(self) -> str:
+        return pulumi.get(self, "last_continuous_snapshot_time")
 
     @property
-    @pulumi.getter(name="createdTimestamp")
-    def created_timestamp(self) -> str:
-        return pulumi.get(self, "created_timestamp")
+    @pulumi.getter(name="lastContinuousSnapshots")
+    def last_continuous_snapshots(self) -> Sequence['outputs.GetNdbTmsCapabilityLastContinuousSnapshotResult']:
+        return pulumi.get(self, "last_continuous_snapshots")
 
     @property
-    @pulumi.getter(name="currentTime")
-    def current_time(self) -> str:
-        return pulumi.get(self, "current_time")
+    @pulumi.getter(name="lastDbLogs")
+    def last_db_logs(self) -> Sequence['outputs.GetNdbTmsCapabilityLastDbLogResult']:
+        return pulumi.get(self, "last_db_logs")
 
     @property
-    @pulumi.getter
-    def destroyed(self) -> bool:
-        return pulumi.get(self, "destroyed")
+    @pulumi.getter(name="logCatchupStartTime")
+    def log_catchup_start_time(self) -> str:
+        return pulumi.get(self, "log_catchup_start_time")
 
     @property
-    @pulumi.getter(name="foundationInitConfigs")
-    def foundation_init_configs(self) -> Sequence['outputs.GetFoundationCentralClusterDetailsFoundationInitConfigResult']:
-        return pulumi.get(self, "foundation_init_configs")
+    @pulumi.getter(name="logTimeInfo")
+    def log_time_info(self) -> Mapping[str, str]:
+        return pulumi.get(self, "log_time_info")
 
     @property
-    @pulumi.getter(name="foundationInitNodeUuid")
-    def foundation_init_node_uuid(self) -> str:
-        return pulumi.get(self, "foundation_init_node_uuid")
+    @pulumi.getter(name="nxClusterAssociationType")
+    def nx_cluster_association_type(self) -> str:
+        return pulumi.get(self, "nx_cluster_association_type")
 
     @property
-    @pulumi.getter
-    def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
-        return pulumi.get(self, "id")
+    @pulumi.getter(name="nxClusterId")
+    def nx_cluster_id(self) -> str:
+        return pulumi.get(self, "nx_cluster_id")
 
     @property
-    @pulumi.getter(name="imagedClusterUuid")
-    def imaged_cluster_uuid(self) -> str:
-        return pulumi.get(self, "imaged_cluster_uuid")
+    @pulumi.getter(name="outputTimeZone")
+    def output_time_zone(self) -> str:
+        return pulumi.get(self, "output_time_zone")
 
     @property
-    @pulumi.getter(name="imagedNodeUuidLists")
-    def imaged_node_uuid_lists(self) -> Sequence[str]:
-        return pulumi.get(self, "imaged_node_uuid_lists")
+    @pulumi.getter(name="overallContinuousRangeEndTime")
+    def overall_continuous_range_end_time(self) -> str:
+        return pulumi.get(self, "overall_continuous_range_end_time")
 
     @property
-    @pulumi.getter(name="redundancyFactor")
-    def redundancy_factor(self) -> Optional[int]:
-        return pulumi.get(self, "redundancy_factor")
+    @pulumi.getter(name="slaId")
+    def sla_id(self) -> str:
+        return pulumi.get(self, "sla_id")
 
     @property
-    @pulumi.getter(name="storageNodeCount")
-    def storage_node_count(self) -> int:
-        return pulumi.get(self, "storage_node_count")
+    @pulumi.getter
+    def source(self) -> bool:
+        return pulumi.get(self, "source")
 
     @property
-    @pulumi.getter(name="workflowType")
-    def workflow_type(self) -> str:
-        return pulumi.get(self, "workflow_type")
+    @pulumi.getter(name="timeMachineId")
+    def time_machine_id(self) -> str:
+        return pulumi.get(self, "time_machine_id")
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        return pulumi.get(self, "type")
 
 
-class AwaitableGetFoundationCentralClusterDetailsResult(GetFoundationCentralClusterDetailsResult):
+class AwaitableGetNdbTmsCapabilityResult(GetNdbTmsCapabilityResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetFoundationCentralClusterDetailsResult(
-            archived=self.archived,
-            cluster_external_ip=self.cluster_external_ip,
-            cluster_name=self.cluster_name,
-            cluster_size=self.cluster_size,
-            cluster_status=self.cluster_status,
-            common_network_settings=self.common_network_settings,
-            created_timestamp=self.created_timestamp,
-            current_time=self.current_time,
-            destroyed=self.destroyed,
-            foundation_init_configs=self.foundation_init_configs,
-            foundation_init_node_uuid=self.foundation_init_node_uuid,
+        return GetNdbTmsCapabilityResult(
+            capabilities=self.capabilities,
+            capability_reset_time=self.capability_reset_time,
+            database_ids=self.database_ids,
+            heal_with_reset_capability=self.heal_with_reset_capability,
             id=self.id,
-            imaged_cluster_uuid=self.imaged_cluster_uuid,
-            imaged_node_uuid_lists=self.imaged_node_uuid_lists,
-            redundancy_factor=self.redundancy_factor,
-            storage_node_count=self.storage_node_count,
-            workflow_type=self.workflow_type)
-
-
-def get_foundation_central_cluster_details(cluster_external_ip: Optional[str] = None,
-                                           cluster_name: Optional[str] = None,
-                                           cluster_size: Optional[int] = None,
-                                           cluster_status: Optional[pulumi.InputType['GetFoundationCentralClusterDetailsClusterStatusArgs']] = None,
-                                           common_network_settings: Optional[pulumi.InputType['GetFoundationCentralClusterDetailsCommonNetworkSettingsArgs']] = None,
-                                           imaged_cluster_uuid: Optional[str] = None,
-                                           redundancy_factor: Optional[int] = None,
-                                           storage_node_count: Optional[int] = None,
-                                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFoundationCentralClusterDetailsResult:
+            last_continuous_snapshot_time=self.last_continuous_snapshot_time,
+            last_continuous_snapshots=self.last_continuous_snapshots,
+            last_db_logs=self.last_db_logs,
+            log_catchup_start_time=self.log_catchup_start_time,
+            log_time_info=self.log_time_info,
+            nx_cluster_association_type=self.nx_cluster_association_type,
+            nx_cluster_id=self.nx_cluster_id,
+            output_time_zone=self.output_time_zone,
+            overall_continuous_range_end_time=self.overall_continuous_range_end_time,
+            sla_id=self.sla_id,
+            source=self.source,
+            time_machine_id=self.time_machine_id,
+            type=self.type)
+
+
+def get_ndb_tms_capability(time_machine_id: Optional[str] = None,
+                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNdbTmsCapabilityResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
-    __args__['clusterExternalIp'] = cluster_external_ip
-    __args__['clusterName'] = cluster_name
-    __args__['clusterSize'] = cluster_size
-    __args__['clusterStatus'] = cluster_status
-    __args__['commonNetworkSettings'] = common_network_settings
-    __args__['imagedClusterUuid'] = imaged_cluster_uuid
-    __args__['redundancyFactor'] = redundancy_factor
-    __args__['storageNodeCount'] = storage_node_count
+    __args__['timeMachineId'] = time_machine_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('nutanix:index/getFoundationCentralClusterDetails:getFoundationCentralClusterDetails', __args__, opts=opts, typ=GetFoundationCentralClusterDetailsResult).value
+    __ret__ = pulumi.runtime.invoke('nutanix:index/getNdbTmsCapability:getNdbTmsCapability', __args__, opts=opts, typ=GetNdbTmsCapabilityResult).value
 
-    return AwaitableGetFoundationCentralClusterDetailsResult(
-        archived=pulumi.get(__ret__, 'archived'),
-        cluster_external_ip=pulumi.get(__ret__, 'cluster_external_ip'),
-        cluster_name=pulumi.get(__ret__, 'cluster_name'),
-        cluster_size=pulumi.get(__ret__, 'cluster_size'),
-        cluster_status=pulumi.get(__ret__, 'cluster_status'),
-        common_network_settings=pulumi.get(__ret__, 'common_network_settings'),
-        created_timestamp=pulumi.get(__ret__, 'created_timestamp'),
-        current_time=pulumi.get(__ret__, 'current_time'),
-        destroyed=pulumi.get(__ret__, 'destroyed'),
-        foundation_init_configs=pulumi.get(__ret__, 'foundation_init_configs'),
-        foundation_init_node_uuid=pulumi.get(__ret__, 'foundation_init_node_uuid'),
+    return AwaitableGetNdbTmsCapabilityResult(
+        capabilities=pulumi.get(__ret__, 'capabilities'),
+        capability_reset_time=pulumi.get(__ret__, 'capability_reset_time'),
+        database_ids=pulumi.get(__ret__, 'database_ids'),
+        heal_with_reset_capability=pulumi.get(__ret__, 'heal_with_reset_capability'),
         id=pulumi.get(__ret__, 'id'),
-        imaged_cluster_uuid=pulumi.get(__ret__, 'imaged_cluster_uuid'),
-        imaged_node_uuid_lists=pulumi.get(__ret__, 'imaged_node_uuid_lists'),
-        redundancy_factor=pulumi.get(__ret__, 'redundancy_factor'),
-        storage_node_count=pulumi.get(__ret__, 'storage_node_count'),
-        workflow_type=pulumi.get(__ret__, 'workflow_type'))
-
-
-@_utilities.lift_output_func(get_foundation_central_cluster_details)
-def get_foundation_central_cluster_details_output(cluster_external_ip: Optional[pulumi.Input[Optional[str]]] = None,
-                                                  cluster_name: Optional[pulumi.Input[Optional[str]]] = None,
-                                                  cluster_size: Optional[pulumi.Input[Optional[int]]] = None,
-                                                  cluster_status: Optional[pulumi.Input[Optional[pulumi.InputType['GetFoundationCentralClusterDetailsClusterStatusArgs']]]] = None,
-                                                  common_network_settings: Optional[pulumi.Input[Optional[pulumi.InputType['GetFoundationCentralClusterDetailsCommonNetworkSettingsArgs']]]] = None,
-                                                  imaged_cluster_uuid: Optional[pulumi.Input[str]] = None,
-                                                  redundancy_factor: Optional[pulumi.Input[Optional[int]]] = None,
-                                                  storage_node_count: Optional[pulumi.Input[Optional[int]]] = None,
-                                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFoundationCentralClusterDetailsResult]:
+        last_continuous_snapshot_time=pulumi.get(__ret__, 'last_continuous_snapshot_time'),
+        last_continuous_snapshots=pulumi.get(__ret__, 'last_continuous_snapshots'),
+        last_db_logs=pulumi.get(__ret__, 'last_db_logs'),
+        log_catchup_start_time=pulumi.get(__ret__, 'log_catchup_start_time'),
+        log_time_info=pulumi.get(__ret__, 'log_time_info'),
+        nx_cluster_association_type=pulumi.get(__ret__, 'nx_cluster_association_type'),
+        nx_cluster_id=pulumi.get(__ret__, 'nx_cluster_id'),
+        output_time_zone=pulumi.get(__ret__, 'output_time_zone'),
+        overall_continuous_range_end_time=pulumi.get(__ret__, 'overall_continuous_range_end_time'),
+        sla_id=pulumi.get(__ret__, 'sla_id'),
+        source=pulumi.get(__ret__, 'source'),
+        time_machine_id=pulumi.get(__ret__, 'time_machine_id'),
+        type=pulumi.get(__ret__, 'type'))
+
+
+@_utilities.lift_output_func(get_ndb_tms_capability)
+def get_ndb_tms_capability_output(time_machine_id: Optional[pulumi.Input[str]] = None,
+                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNdbTmsCapabilityResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_central_imaged_clusters_list.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_imaged_clusters_list.py`

 * *Files 19% similar despite different names*

```diff
@@ -60,24 +60,30 @@
     @pulumi.getter(name="imagedClusters")
     def imaged_clusters(self) -> Sequence['outputs.GetFoundationCentralImagedClustersListImagedClusterResult']:
         return pulumi.get(self, "imaged_clusters")
 
     @property
     @pulumi.getter
     def length(self) -> Optional[int]:
+        """
+        The number of records retrieved.
+        """
         return pulumi.get(self, "length")
 
     @property
     @pulumi.getter
     def metadatas(self) -> Sequence['outputs.GetFoundationCentralImagedClustersListMetadataResult']:
         return pulumi.get(self, "metadatas")
 
     @property
     @pulumi.getter
     def offset(self) -> Optional[int]:
+        """
+        Offset from the start of the object list.
+        """
         return pulumi.get(self, "offset")
 
 
 class AwaitableGetFoundationCentralImagedClustersListResult(GetFoundationCentralImagedClustersListResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -92,15 +98,28 @@
 
 
 def get_foundation_central_imaged_clusters_list(filters: Optional[pulumi.InputType['GetFoundationCentralImagedClustersListFiltersArgs']] = None,
                                                 length: Optional[int] = None,
                                                 offset: Optional[int] = None,
                                                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFoundationCentralImagedClustersListResult:
     """
-    Use this data source to access information about an existing resource.
+    List all the clusters created using Foundation Central.
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_nutanix as nutanix
+
+    imaged_clusters_list = nutanix.get_foundation_central_imaged_clusters_list()
+    ```
+
+
+    :param int length: The number of records retrieved.
+    :param int offset: Offset from the start of the object list.
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['length'] = length
     __args__['offset'] = offset
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('nutanix:index/getFoundationCentralImagedClustersList:getFoundationCentralImagedClustersList', __args__, opts=opts, typ=GetFoundationCentralImagedClustersListResult).value
@@ -116,10 +135,23 @@
 
 @_utilities.lift_output_func(get_foundation_central_imaged_clusters_list)
 def get_foundation_central_imaged_clusters_list_output(filters: Optional[pulumi.Input[Optional[pulumi.InputType['GetFoundationCentralImagedClustersListFiltersArgs']]]] = None,
                                                        length: Optional[pulumi.Input[Optional[int]]] = None,
                                                        offset: Optional[pulumi.Input[Optional[int]]] = None,
                                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFoundationCentralImagedClustersListResult]:
     """
-    Use this data source to access information about an existing resource.
+    List all the clusters created using Foundation Central.
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_nutanix as nutanix
+
+    imaged_clusters_list = nutanix.get_foundation_central_imaged_clusters_list()
+    ```
+
+
+    :param int length: The number of records retrieved.
+    :param int offset: Offset from the start of the object list.
     """
     ...
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_central_imaged_node_details.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_imaged_node_details.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_central_imaged_nodes_list.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_imaged_nodes_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,24 +60,33 @@
     @pulumi.getter(name="imagedNodes")
     def imaged_nodes(self) -> Sequence['outputs.GetFoundationCentralImagedNodesListImagedNodeResult']:
         return pulumi.get(self, "imaged_nodes")
 
     @property
     @pulumi.getter
     def length(self) -> Optional[int]:
+        """
+        The number of records retrieved.
+        """
         return pulumi.get(self, "length")
 
     @property
     @pulumi.getter
     def metadatas(self) -> Sequence['outputs.GetFoundationCentralImagedNodesListMetadataResult']:
+        """
+        List metadata output for all list apis.
+        """
         return pulumi.get(self, "metadatas")
 
     @property
     @pulumi.getter
     def offset(self) -> Optional[int]:
+        """
+        Offset from the start of the object list.
+        """
         return pulumi.get(self, "offset")
 
 
 class AwaitableGetFoundationCentralImagedNodesListResult(GetFoundationCentralImagedNodesListResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -92,15 +101,28 @@
 
 
 def get_foundation_central_imaged_nodes_list(filters: Optional[pulumi.InputType['GetFoundationCentralImagedNodesListFiltersArgs']] = None,
                                              length: Optional[int] = None,
                                              offset: Optional[int] = None,
                                              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFoundationCentralImagedNodesListResult:
     """
-    Use this data source to access information about an existing resource.
+    List all the nodes registered with Foundation Central
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_nutanix as nutanix
+
+    nodes_list = nutanix.get_foundation_central_imaged_nodes_list()
+    ```
+
+
+    :param int length: The number of records retrieved.
+    :param int offset: Offset from the start of the object list.
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['length'] = length
     __args__['offset'] = offset
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('nutanix:index/getFoundationCentralImagedNodesList:getFoundationCentralImagedNodesList', __args__, opts=opts, typ=GetFoundationCentralImagedNodesListResult).value
@@ -116,10 +138,23 @@
 
 @_utilities.lift_output_func(get_foundation_central_imaged_nodes_list)
 def get_foundation_central_imaged_nodes_list_output(filters: Optional[pulumi.Input[Optional[pulumi.InputType['GetFoundationCentralImagedNodesListFiltersArgs']]]] = None,
                                                     length: Optional[pulumi.Input[Optional[int]]] = None,
                                                     offset: Optional[pulumi.Input[Optional[int]]] = None,
                                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFoundationCentralImagedNodesListResult]:
     """
-    Use this data source to access information about an existing resource.
+    List all the nodes registered with Foundation Central
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_nutanix as nutanix
+
+    nodes_list = nutanix.get_foundation_central_imaged_nodes_list()
+    ```
+
+
+    :param int length: The number of records retrieved.
+    :param int offset: Offset from the start of the object list.
     """
     ...
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_central_list_api_keys.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_central_list_api_keys.py`

 * *Files 24% similar despite different names*

```diff
@@ -52,24 +52,33 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def length(self) -> Optional[int]:
+        """
+        The number of records retrieved.
+        """
         return pulumi.get(self, "length")
 
     @property
     @pulumi.getter
     def metadata(self) -> Optional['outputs.GetFoundationCentralListApiKeysMetadataResult']:
+        """
+        List metadata output for all list apis.
+        """
         return pulumi.get(self, "metadata")
 
     @property
     @pulumi.getter
     def offset(self) -> Optional[int]:
+        """
+        Offset from the start of the object list.
+        """
         return pulumi.get(self, "offset")
 
 
 class AwaitableGetFoundationCentralListApiKeysResult(GetFoundationCentralListApiKeysResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -83,15 +92,29 @@
 
 
 def get_foundation_central_list_api_keys(length: Optional[int] = None,
                                          metadata: Optional[pulumi.InputType['GetFoundationCentralListApiKeysMetadataArgs']] = None,
                                          offset: Optional[int] = None,
                                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFoundationCentralListApiKeysResult:
     """
-    Use this data source to access information about an existing resource.
+    List all the api keys created in Foundation Central.
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_nutanix as nutanix
+
+    api_keys_list = nutanix.get_foundation_central_list_api_keys()
+    ```
+
+
+    :param int length: The number of records retrieved.
+    :param pulumi.InputType['GetFoundationCentralListApiKeysMetadataArgs'] metadata: List metadata output for all list apis.
+    :param int offset: Offset from the start of the object list.
     """
     __args__ = dict()
     __args__['length'] = length
     __args__['metadata'] = metadata
     __args__['offset'] = offset
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('nutanix:index/getFoundationCentralListApiKeys:getFoundationCentralListApiKeys', __args__, opts=opts, typ=GetFoundationCentralListApiKeysResult).value
@@ -106,10 +129,24 @@
 
 @_utilities.lift_output_func(get_foundation_central_list_api_keys)
 def get_foundation_central_list_api_keys_output(length: Optional[pulumi.Input[Optional[int]]] = None,
                                                 metadata: Optional[pulumi.Input[Optional[pulumi.InputType['GetFoundationCentralListApiKeysMetadataArgs']]]] = None,
                                                 offset: Optional[pulumi.Input[Optional[int]]] = None,
                                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFoundationCentralListApiKeysResult]:
     """
-    Use this data source to access information about an existing resource.
+    List all the api keys created in Foundation Central.
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_nutanix as nutanix
+
+    api_keys_list = nutanix.get_foundation_central_list_api_keys()
+    ```
+
+
+    :param int length: The number of records retrieved.
+    :param pulumi.InputType['GetFoundationCentralListApiKeysMetadataArgs'] metadata: List metadata output for all list apis.
+    :param int offset: Offset from the start of the object list.
     """
     ...
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_discover_nodes.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_discover_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_hypervisor_isos.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_hypervisor_isos.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 
     ```python
     import pulumi
     import pulumi_nutanix as nutanix
 
     hypervisor_isos = nutanix.get_foundation_hypervisor_isos()
     ```
+
     ## Note
 
     * This data source only lists .iso files details.
 
     See detailed information in [Nutanix Foundation Hypervisor Isos](https://www.nutanix.dev/api_references/foundation/#/b3A6MjIyMjM0MDE-list-hypervisor-images-available-in-foundation).
     """
     __args__ = dict()
@@ -145,14 +146,15 @@
 
     ```python
     import pulumi
     import pulumi_nutanix as nutanix
 
     hypervisor_isos = nutanix.get_foundation_hypervisor_isos()
     ```
+
     ## Note
 
     * This data source only lists .iso files details.
 
     See detailed information in [Nutanix Foundation Hypervisor Isos](https://www.nutanix.dev/api_references/foundation/#/b3A6MjIyMjM0MDE-list-hypervisor-images-available-in-foundation).
     """
     ...
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_nod_packages.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_nos_packages.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetFoundationNodPackagesResult',
-    'AwaitableGetFoundationNodPackagesResult',
-    'get_foundation_nod_packages',
-    'get_foundation_nod_packages_output',
+    'GetFoundationNosPackagesResult',
+    'AwaitableGetFoundationNosPackagesResult',
+    'get_foundation_nos_packages',
+    'get_foundation_nos_packages_output',
 ]
 
 @pulumi.output_type
-class GetFoundationNodPackagesResult:
+class GetFoundationNosPackagesResult:
     """
-    A collection of values returned by getFoundationNodPackages.
+    A collection of values returned by getFoundationNosPackages.
     """
     def __init__(__self__, entities=None, id=None):
         if entities and not isinstance(entities, list):
             raise TypeError("Expected argument 'entities' to be a list")
         pulumi.set(__self__, "entities", entities)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
@@ -42,64 +42,66 @@
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
 
-class AwaitableGetFoundationNodPackagesResult(GetFoundationNodPackagesResult):
+class AwaitableGetFoundationNosPackagesResult(GetFoundationNosPackagesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetFoundationNodPackagesResult(
+        return GetFoundationNosPackagesResult(
             entities=self.entities,
             id=self.id)
 
 
-def get_foundation_nod_packages(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFoundationNodPackagesResult:
+def get_foundation_nos_packages(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFoundationNosPackagesResult:
     """
     Describes a list of nos (aos) packages present in foundation vm
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_nutanix as nutanix
 
-    nos_packages = nutanix.get_foundation_nod_packages()
+    nos_packages = nutanix.get_foundation_nos_packages()
     ```
+
     ## Note
 
     * This data source only lists .tar file names.
 
     See detailed information in [Nutanix Foundation Nos Packages](https://www.nutanix.dev/api_references/foundation/#/b3A6MjIyMjMzODg-get-list-of-aos-packages-available-in-foundation).
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('nutanix:index/getFoundationNodPackages:getFoundationNodPackages', __args__, opts=opts, typ=GetFoundationNodPackagesResult).value
+    __ret__ = pulumi.runtime.invoke('nutanix:index/getFoundationNosPackages:getFoundationNosPackages', __args__, opts=opts, typ=GetFoundationNosPackagesResult).value
 
-    return AwaitableGetFoundationNodPackagesResult(
+    return AwaitableGetFoundationNosPackagesResult(
         entities=pulumi.get(__ret__, 'entities'),
         id=pulumi.get(__ret__, 'id'))
 
 
-@_utilities.lift_output_func(get_foundation_nod_packages)
-def get_foundation_nod_packages_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFoundationNodPackagesResult]:
+@_utilities.lift_output_func(get_foundation_nos_packages)
+def get_foundation_nos_packages_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFoundationNosPackagesResult]:
     """
     Describes a list of nos (aos) packages present in foundation vm
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_nutanix as nutanix
 
-    nos_packages = nutanix.get_foundation_nod_packages()
+    nos_packages = nutanix.get_foundation_nos_packages()
     ```
+
     ## Note
 
     * This data source only lists .tar file names.
 
     See detailed information in [Nutanix Foundation Nos Packages](https://www.nutanix.dev/api_references/foundation/#/b3A6MjIyMjMzODg-get-list-of-aos-packages-available-in-foundation).
     """
     ...
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_foundation_node_network_details.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_foundation_node_network_details.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_host.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_hosts.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_image.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_karbon_cluster.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_karbon_cluster_kube_config.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_cluster_kube_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_karbon_cluster_ssh.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_cluster_ssh.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_karbon_clusters.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_clusters.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_karbon_private_registries.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_private_registries.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_karbon_private_registry.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_karbon_private_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_network_security_rule.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_network_security_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -516,14 +516,15 @@
                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNetworkSecurityRuleResult:
     """
     Describes a Network security rule
 
     > NOTE: The use of network_security_rule is only applicable in AHV clusters and requires Microsegmentation to be enabled. This feature is a function of the Flow product and requires a Flow license. For more information on Flow and Microsegmentation please visit https://www.nutanix.com/products/flow
 
     ## Example Usage
+
     ### Isolate Development VMs From Production VMs And Get Its Information)
 
     ```python
     import pulumi
     import pulumi_nutanix as nutanix
 
     isolation = nutanix.NetworkSecurityRule("isolation",
@@ -605,14 +606,15 @@
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNetworkSecurityRuleResult]:
     """
     Describes a Network security rule
 
     > NOTE: The use of network_security_rule is only applicable in AHV clusters and requires Microsegmentation to be enabled. This feature is a function of the Flow product and requires a Flow license. For more information on Flow and Microsegmentation please visit https://www.nutanix.com/products/flow
 
     ## Example Usage
+
     ### Isolate Development VMs From Production VMs And Get Its Information)
 
     ```python
     import pulumi
     import pulumi_nutanix as nutanix
 
     isolation = nutanix.NetworkSecurityRule("isolation",
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_pbr.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_pbr.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_pbrs.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_pbrs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_permission.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_permissions.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_project.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,24 +19,33 @@
 ]
 
 @pulumi.output_type
 class GetProjectResult:
     """
     A collection of values returned by getProject.
     """
-    def __init__(__self__, account_reference_lists=None, api_version=None, categories=None, default_subnet_reference=None, description=None, environment_reference_lists=None, external_network_lists=None, external_user_group_reference_lists=None, id=None, is_default=None, metadata=None, name=None, owner_reference=None, project_id=None, project_name=None, project_reference=None, resource_domains=None, state=None, subnet_reference_lists=None, user_reference_lists=None):
+    def __init__(__self__, account_reference_lists=None, acps=None, api_version=None, categories=None, cluster_reference_lists=None, default_environment_references=None, default_subnet_reference=None, description=None, environment_reference_lists=None, external_network_lists=None, external_user_group_reference_lists=None, id=None, is_default=None, metadata=None, name=None, owner_reference=None, project_id=None, project_name=None, project_reference=None, resource_domains=None, state=None, subnet_reference_lists=None, tunnel_reference_lists=None, user_reference_lists=None, vpc_reference_lists=None):
         if account_reference_lists and not isinstance(account_reference_lists, list):
             raise TypeError("Expected argument 'account_reference_lists' to be a list")
         pulumi.set(__self__, "account_reference_lists", account_reference_lists)
+        if acps and not isinstance(acps, list):
+            raise TypeError("Expected argument 'acps' to be a list")
+        pulumi.set(__self__, "acps", acps)
         if api_version and not isinstance(api_version, str):
             raise TypeError("Expected argument 'api_version' to be a str")
         pulumi.set(__self__, "api_version", api_version)
         if categories and not isinstance(categories, list):
             raise TypeError("Expected argument 'categories' to be a list")
         pulumi.set(__self__, "categories", categories)
+        if cluster_reference_lists and not isinstance(cluster_reference_lists, list):
+            raise TypeError("Expected argument 'cluster_reference_lists' to be a list")
+        pulumi.set(__self__, "cluster_reference_lists", cluster_reference_lists)
+        if default_environment_references and not isinstance(default_environment_references, list):
+            raise TypeError("Expected argument 'default_environment_references' to be a list")
+        pulumi.set(__self__, "default_environment_references", default_environment_references)
         if default_subnet_reference and not isinstance(default_subnet_reference, dict):
             raise TypeError("Expected argument 'default_subnet_reference' to be a dict")
         pulumi.set(__self__, "default_subnet_reference", default_subnet_reference)
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
         if environment_reference_lists and not isinstance(environment_reference_lists, list):
@@ -77,55 +86,85 @@
         pulumi.set(__self__, "resource_domains", resource_domains)
         if state and not isinstance(state, str):
             raise TypeError("Expected argument 'state' to be a str")
         pulumi.set(__self__, "state", state)
         if subnet_reference_lists and not isinstance(subnet_reference_lists, list):
             raise TypeError("Expected argument 'subnet_reference_lists' to be a list")
         pulumi.set(__self__, "subnet_reference_lists", subnet_reference_lists)
+        if tunnel_reference_lists and not isinstance(tunnel_reference_lists, list):
+            raise TypeError("Expected argument 'tunnel_reference_lists' to be a list")
+        pulumi.set(__self__, "tunnel_reference_lists", tunnel_reference_lists)
         if user_reference_lists and not isinstance(user_reference_lists, list):
             raise TypeError("Expected argument 'user_reference_lists' to be a list")
         pulumi.set(__self__, "user_reference_lists", user_reference_lists)
+        if vpc_reference_lists and not isinstance(vpc_reference_lists, list):
+            raise TypeError("Expected argument 'vpc_reference_lists' to be a list")
+        pulumi.set(__self__, "vpc_reference_lists", vpc_reference_lists)
 
     @property
     @pulumi.getter(name="accountReferenceLists")
     def account_reference_lists(self) -> Sequence['outputs.GetProjectAccountReferenceListResult']:
         """
         List of accounts associated with the project.
         * `account_reference_list.#.kind` - The kind name. Default value is `account`
         * `account_reference_list.#.uuid` - The UUID of an account.
         * `account_reference_list.#.name` - The name of an account.
         """
         return pulumi.get(self, "account_reference_lists")
 
     @property
+    @pulumi.getter
+    def acps(self) -> Sequence['outputs.GetProjectAcpResult']:
+        return pulumi.get(self, "acps")
+
+    @property
     @pulumi.getter(name="apiVersion")
     def api_version(self) -> str:
         return pulumi.get(self, "api_version")
 
     @property
     @pulumi.getter
     def categories(self) -> Sequence['outputs.GetProjectCategoryResult']:
+        """
+        - (Optional) The category values represented as a dictionary of key > list of values.
+        """
         return pulumi.get(self, "categories")
 
     @property
+    @pulumi.getter(name="clusterReferenceLists")
+    def cluster_reference_lists(self) -> Sequence['outputs.GetProjectClusterReferenceListResult']:
+        """
+        (Optional/Computed) List of clusters associated with the project..
+        * `cluster_reference_list.#.kind` - (Optional) The kind name. Default value is `cluster`
+        * `cluster_reference_list.#.uuid` - (Required) The UUID of a cluster
+        * `cluster_reference_list.#.name` - (Optional/Computed) The name of a cluster.
+        """
+        return pulumi.get(self, "cluster_reference_lists")
+
+    @property
+    @pulumi.getter(name="defaultEnvironmentReferences")
+    def default_environment_references(self) -> Sequence['outputs.GetProjectDefaultEnvironmentReferenceResult']:
+        """
+        (Optional/Computed) Reference to a environment.
+        """
+        return pulumi.get(self, "default_environment_references")
+
+    @property
     @pulumi.getter(name="defaultSubnetReference")
     def default_subnet_reference(self) -> Mapping[str, str]:
         """
         Reference to a subnet.
-        * `default_subnet_reference.kind` - The kind name. Default value is `subnet`
-        * `default_subnet_reference.uuid` - The UUID of a subnet.
-        * `default_subnet_reference.name` - The name of a subnet.
         """
         return pulumi.get(self, "default_subnet_reference")
 
     @property
     @pulumi.getter
     def description(self) -> str:
         """
-        A description for project.
+        Description of ACP
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="environmentReferenceLists")
     def environment_reference_lists(self) -> Sequence['outputs.GetProjectEnvironmentReferenceListResult']:
         """
@@ -204,19 +243,14 @@
         return pulumi.get(self, "project_reference")
 
     @property
     @pulumi.getter(name="resourceDomains")
     def resource_domains(self) -> Sequence['outputs.GetProjectResourceDomainResult']:
         """
         The status for a resource domain (limits and values)
-        * `resource_domain.resources` Array of the utilization/limit for resource types
-        * `resource_domain.resources.#.limit` The resource consumption limit (unspecified is unlimited)
-        * `resource_domain.resources.#.resource_type` The type of resource (for example storage, CPUs)
-        * `resource_domain.resources.#.units` - The units of the resource type
-        * `resource_domain.resources.#.value` - The amount of resource consumed
         """
         return pulumi.get(self, "resource_domains")
 
     @property
     @pulumi.getter
     def state(self) -> str:
         return pulumi.get(self, "state")
@@ -229,34 +263,56 @@
         * `subnet_reference_list.#.kind` - The kind name. Default value is `subnet`
         * `subnet_reference_list.#.uuid` - The UUID of a subnet
         * `subnet_reference_list.#.name` - The name of a subnet.
         """
         return pulumi.get(self, "subnet_reference_lists")
 
     @property
+    @pulumi.getter(name="tunnelReferenceLists")
+    def tunnel_reference_lists(self) -> Sequence['outputs.GetProjectTunnelReferenceListResult']:
+        """
+        (Optional/Computed) List of tunnels associated with the project.
+        * `tunnel_reference_list.#.kind` - (Optional) The kind name. Default value is `tunnel`
+        * `tunnel_reference_list.#.uuid` - (Required) The UUID of a tunnel
+        * `tunnel_reference_list.#.name` - (Optional/Computed) The name of a tunnel.
+        """
+        return pulumi.get(self, "tunnel_reference_lists")
+
+    @property
     @pulumi.getter(name="userReferenceLists")
     def user_reference_lists(self) -> Sequence['outputs.GetProjectUserReferenceListResult']:
         """
-        List of users in the project.
-        * `user_reference_list.#.kind` - The kind name. Default value is `user`
-        * `user_reference_list.#.uuid` - The UUID of a user
-        * `user_reference_list.#.name` - The name of a user.
+        List of Reference of users.
         """
         return pulumi.get(self, "user_reference_lists")
 
+    @property
+    @pulumi.getter(name="vpcReferenceLists")
+    def vpc_reference_lists(self) -> Sequence['outputs.GetProjectVpcReferenceListResult']:
+        """
+        (Optional/Computed) List of VPCs associated with the project..
+        * `vpc_reference_list.#.kind` - (Optional) The kind name. Default value is `vpc`
+        * `vpc_reference_list.#.uuid` - (Required) The UUID of a vpc
+        * `vpc_reference_list.#.name` - (Optional/Computed) The name of a vpc.
+        """
+        return pulumi.get(self, "vpc_reference_lists")
+
 
 class AwaitableGetProjectResult(GetProjectResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetProjectResult(
             account_reference_lists=self.account_reference_lists,
+            acps=self.acps,
             api_version=self.api_version,
             categories=self.categories,
+            cluster_reference_lists=self.cluster_reference_lists,
+            default_environment_references=self.default_environment_references,
             default_subnet_reference=self.default_subnet_reference,
             description=self.description,
             environment_reference_lists=self.environment_reference_lists,
             external_network_lists=self.external_network_lists,
             external_user_group_reference_lists=self.external_user_group_reference_lists,
             id=self.id,
             is_default=self.is_default,
@@ -265,15 +321,17 @@
             owner_reference=self.owner_reference,
             project_id=self.project_id,
             project_name=self.project_name,
             project_reference=self.project_reference,
             resource_domains=self.resource_domains,
             state=self.state,
             subnet_reference_lists=self.subnet_reference_lists,
-            user_reference_lists=self.user_reference_lists)
+            tunnel_reference_lists=self.tunnel_reference_lists,
+            user_reference_lists=self.user_reference_lists,
+            vpc_reference_lists=self.vpc_reference_lists)
 
 
 def get_project(categories: Optional[Sequence[pulumi.InputType['GetProjectCategoryArgs']]] = None,
                 external_user_group_reference_lists: Optional[Sequence[pulumi.InputType['GetProjectExternalUserGroupReferenceListArgs']]] = None,
                 project_id: Optional[str] = None,
                 project_name: Optional[str] = None,
                 subnet_reference_lists: Optional[Sequence[pulumi.InputType['GetProjectSubnetReferenceListArgs']]] = None,
@@ -325,42 +383,43 @@
             uuid=subnet.metadata["uuid"],
         ),
         api_version="3.1")
     test = nutanix.get_project_output(project_id=project_test.id)
     ```
 
 
+    :param Sequence[pulumi.InputType['GetProjectCategoryArgs']] categories: - (Optional) The category values represented as a dictionary of key > list of values.
     :param Sequence[pulumi.InputType['GetProjectExternalUserGroupReferenceListArgs']] external_user_group_reference_lists: List of directory service user groups. These groups are not managed by Nutanix.
            * `external_user_group_reference_list.#.kind` - The kind name. Default value is `user_group`
            * `external_user_group_reference_list.#.uuid` - The UUID of a user_group
            * `external_user_group_reference_list.#.name` - The name of a user_group
     :param str project_id: - (Required) The `id` of the project.
     :param Sequence[pulumi.InputType['GetProjectSubnetReferenceListArgs']] subnet_reference_lists: List of subnets for the project.
            * `subnet_reference_list.#.kind` - The kind name. Default value is `subnet`
            * `subnet_reference_list.#.uuid` - The UUID of a subnet
            * `subnet_reference_list.#.name` - The name of a subnet.
-    :param Sequence[pulumi.InputType['GetProjectUserReferenceListArgs']] user_reference_lists: List of users in the project.
-           * `user_reference_list.#.kind` - The kind name. Default value is `user`
-           * `user_reference_list.#.uuid` - The UUID of a user
-           * `user_reference_list.#.name` - The name of a user.
+    :param Sequence[pulumi.InputType['GetProjectUserReferenceListArgs']] user_reference_lists: List of Reference of users.
     """
     __args__ = dict()
     __args__['categories'] = categories
     __args__['externalUserGroupReferenceLists'] = external_user_group_reference_lists
     __args__['projectId'] = project_id
     __args__['projectName'] = project_name
     __args__['subnetReferenceLists'] = subnet_reference_lists
     __args__['userReferenceLists'] = user_reference_lists
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('nutanix:index/getProject:getProject', __args__, opts=opts, typ=GetProjectResult).value
 
     return AwaitableGetProjectResult(
         account_reference_lists=pulumi.get(__ret__, 'account_reference_lists'),
+        acps=pulumi.get(__ret__, 'acps'),
         api_version=pulumi.get(__ret__, 'api_version'),
         categories=pulumi.get(__ret__, 'categories'),
+        cluster_reference_lists=pulumi.get(__ret__, 'cluster_reference_lists'),
+        default_environment_references=pulumi.get(__ret__, 'default_environment_references'),
         default_subnet_reference=pulumi.get(__ret__, 'default_subnet_reference'),
         description=pulumi.get(__ret__, 'description'),
         environment_reference_lists=pulumi.get(__ret__, 'environment_reference_lists'),
         external_network_lists=pulumi.get(__ret__, 'external_network_lists'),
         external_user_group_reference_lists=pulumi.get(__ret__, 'external_user_group_reference_lists'),
         id=pulumi.get(__ret__, 'id'),
         is_default=pulumi.get(__ret__, 'is_default'),
@@ -369,15 +428,17 @@
         owner_reference=pulumi.get(__ret__, 'owner_reference'),
         project_id=pulumi.get(__ret__, 'project_id'),
         project_name=pulumi.get(__ret__, 'project_name'),
         project_reference=pulumi.get(__ret__, 'project_reference'),
         resource_domains=pulumi.get(__ret__, 'resource_domains'),
         state=pulumi.get(__ret__, 'state'),
         subnet_reference_lists=pulumi.get(__ret__, 'subnet_reference_lists'),
-        user_reference_lists=pulumi.get(__ret__, 'user_reference_lists'))
+        tunnel_reference_lists=pulumi.get(__ret__, 'tunnel_reference_lists'),
+        user_reference_lists=pulumi.get(__ret__, 'user_reference_lists'),
+        vpc_reference_lists=pulumi.get(__ret__, 'vpc_reference_lists'))
 
 
 @_utilities.lift_output_func(get_project)
 def get_project_output(categories: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetProjectCategoryArgs']]]]] = None,
                        external_user_group_reference_lists: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetProjectExternalUserGroupReferenceListArgs']]]]] = None,
                        project_id: Optional[pulumi.Input[Optional[str]]] = None,
                        project_name: Optional[pulumi.Input[Optional[str]]] = None,
@@ -430,22 +491,20 @@
             uuid=subnet.metadata["uuid"],
         ),
         api_version="3.1")
     test = nutanix.get_project_output(project_id=project_test.id)
     ```
 
 
+    :param Sequence[pulumi.InputType['GetProjectCategoryArgs']] categories: - (Optional) The category values represented as a dictionary of key > list of values.
     :param Sequence[pulumi.InputType['GetProjectExternalUserGroupReferenceListArgs']] external_user_group_reference_lists: List of directory service user groups. These groups are not managed by Nutanix.
            * `external_user_group_reference_list.#.kind` - The kind name. Default value is `user_group`
            * `external_user_group_reference_list.#.uuid` - The UUID of a user_group
            * `external_user_group_reference_list.#.name` - The name of a user_group
     :param str project_id: - (Required) The `id` of the project.
     :param Sequence[pulumi.InputType['GetProjectSubnetReferenceListArgs']] subnet_reference_lists: List of subnets for the project.
            * `subnet_reference_list.#.kind` - The kind name. Default value is `subnet`
            * `subnet_reference_list.#.uuid` - The UUID of a subnet
            * `subnet_reference_list.#.name` - The name of a subnet.
-    :param Sequence[pulumi.InputType['GetProjectUserReferenceListArgs']] user_reference_lists: List of users in the project.
-           * `user_reference_list.#.kind` - The kind name. Default value is `user`
-           * `user_reference_list.#.uuid` - The UUID of a user
-           * `user_reference_list.#.name` - The name of a user.
+    :param Sequence[pulumi.InputType['GetProjectUserReferenceListArgs']] user_reference_lists: List of Reference of users.
     """
     ...
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_projects.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_projects.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_protection_rule.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_protection_rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,41 +76,27 @@
         return pulumi.get(self, "api_version")
 
     @property
     @pulumi.getter(name="availabilityZoneConnectivityLists")
     def availability_zone_connectivity_lists(self) -> Sequence['outputs.GetProtectionRuleAvailabilityZoneConnectivityListResult']:
         """
         (Required) This encodes the datapipes between various availability zones and\\nthe backup policy of the pipes.
-        * `availability_zone_connectivity_list.destination_availability_zone_index` - (Optional/Computed) Index of the availability zone.
-        * `availability_zone_connectivity_list.source_availability_zone_index` - (Optional/Computed) Index of the availability zone.
-        * `availability_zone_connectivity_list.snapshot_schedule_list` - (Optional/Computed) Snapshot schedules for the pair of the availability zones.
-        * `availability_zone_connectivity_list.snapshot_schedule_list.#.recovery_point_objective_secs` - (Required) "A recovery point objective (RPO) is the maximum acceptable amount of data loss.
-        * `availability_zone_connectivity_list.snapshot_schedule_list.#.local_snapshot_retention_policy` - (Optional/Computed) This describes the snapshot retention policy for this availability zone.
-        * `availability_zone_connectivity_list.snapshot_schedule_list.#.local_snapshot_retention_policy.0.num_snapshots` - (Optional/Computed) Number of snapshots need to be retained.
-        * `availability_zone_connectivity_list.snapshot_schedule_list.#.local_snapshot_retention_policy.0.rollup_retention_policy_multiple` - (Optional/Computed) Multiplier to 'snapshot_interval_type'.
-        * `availability_zone_connectivity_list.snapshot_schedule_list.#.local_snapshot_retention_policy.0.rollup_retention_policy_snapshot_interval_type` - (Optional/Computed)
-        * `availability_zone_connectivity_list.snapshot_schedule_list.#.auto_suspend_timeout_secs` - (Optional/Computed) Auto suspend timeout in case of connection failure between the sites.
-        * `availability_zone_connectivity_list.snapshot_schedule_list.#.snapshot_type` - (Optional/Computed) Crash consistent or Application Consistent snapshot.
-        * `availability_zone_connectivity_list.snapshot_schedule_list.#.remote_snapshot_retention_policy` - (Optional/Computed) This describes the snapshot retention policy for this availability zone.
         """
         return pulumi.get(self, "availability_zone_connectivity_lists")
 
     @property
     @pulumi.getter
     def categories(self) -> Sequence['outputs.GetProtectionRuleCategoryResult']:
         return pulumi.get(self, "categories")
 
     @property
     @pulumi.getter(name="categoryFilters")
     def category_filters(self) -> Sequence['outputs.GetProtectionRuleCategoryFilterResult']:
         """
         (Optional/Computed)
-        * `category_filter.0.type` - (Optional/Computed) The type of the filter being used.
-        * `category_filter.0.kind_list` - (Optional/Computed) List of kinds associated with this filter.
-        * `category_filter.0.params` - (Optional/Computed) A list of category key and list of values.
         """
         return pulumi.get(self, "category_filters")
 
     @property
     @pulumi.getter
     def description(self) -> str:
         """
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_protection_rules.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_protection_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_recovery_plans.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_recovery_plans.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_role.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_roles.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_service_group.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_service_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_service_groups.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_service_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_static_routes.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_static_routes.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_subnet.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_subnets.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_subnets.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,17 @@
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_nutanix as nutanix
 
     subnets = nutanix.get_subnets()
+    test = nutanix.get_subnets(metadatas=[nutanix.GetSubnetsMetadataArgs(
+        filter="name==vlan0_test_2",
+    )])
     ```
 
 
     :param Sequence[pulumi.InputType['GetSubnetsMetadataArgs']] metadatas: The subnet kind metadata.
     """
     __args__ = dict()
     __args__['metadatas'] = metadatas
@@ -120,13 +123,16 @@
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_nutanix as nutanix
 
     subnets = nutanix.get_subnets()
+    test = nutanix.get_subnets(metadatas=[nutanix.GetSubnetsMetadataArgs(
+        filter="name==vlan0_test_2",
+    )])
     ```
 
 
     :param Sequence[pulumi.InputType['GetSubnetsMetadataArgs']] metadatas: The subnet kind metadata.
     """
     ...
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_user.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_user_group.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_user_groups.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_users.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_virtual_machine.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_virtual_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,14 +314,17 @@
         - VM guests may be customized at boot time using one of several different methods. Currently, cloud-init w/ ConfigDriveV2 (for Linux VMs) and Sysprep (for Windows VMs) are supported. Only ONE OF sysprep or cloud_init should be provided. Note that guest customization can currently only be set during VM creation. Attempting to change it after creation will result in an error. Additional properties can be specified. For example - in the context of VM template creation if \\"override_script\\" is set to \\"True\\" then the deployer can upload their own custom script.
         """
         return pulumi.get(self, "guest_customization_sysprep")
 
     @property
     @pulumi.getter(name="guestCustomizationSysprepCustomKeyValues")
     def guest_customization_sysprep_custom_key_values(self) -> Mapping[str, Any]:
+        """
+        - Generic key value pair used for custom attributes in sysprep.
+        """
         return pulumi.get(self, "guest_customization_sysprep_custom_key_values")
 
     @property
     @pulumi.getter(name="guestOsId")
     def guest_os_id(self) -> str:
         """
         - Guest OS Identifier. For ESX, refer to VMware documentation [link](https://www.vmware.com/support/developer/converter-sdk/conv43_apireference/vim.vm.GuestOsDescriptor.GuestOsIdentifier.html) for the list of guest OS identifiers.
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_vpc.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/get_vpcs.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/get_vpcs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/image.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/karbon_cluster.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/karbon_cluster.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,14 +55,17 @@
         if name is not None:
             pulumi.set(__self__, "name", name)
         if private_registries is not None:
             pulumi.set(__self__, "private_registries", private_registries)
         if single_master_config is not None:
             pulumi.set(__self__, "single_master_config", single_master_config)
         if wait_timeout_minutes is not None:
+            warnings.warn("""use timeouts instead""", DeprecationWarning)
+            pulumi.log.warn("""wait_timeout_minutes is deprecated: use timeouts instead""")
+        if wait_timeout_minutes is not None:
             pulumi.set(__self__, "wait_timeout_minutes", wait_timeout_minutes)
 
     @property
     @pulumi.getter(name="cniConfig")
     def cni_config(self) -> pulumi.Input['KarbonClusterCniConfigArgs']:
         """
         - (Required) K8s cluster networking configuration. The flannel or the calico configuration needs to be provided. **Note:** Updates to this attribute forces new resource creation.
@@ -192,14 +195,17 @@
 
     @property
     @pulumi.getter(name="waitTimeoutMinutes")
     def wait_timeout_minutes(self) -> Optional[pulumi.Input[int]]:
         """
         - (Optional) Maximum wait time for the Karbon cluster to provision.
         """
+        warnings.warn("""use timeouts instead""", DeprecationWarning)
+        pulumi.log.warn("""wait_timeout_minutes is deprecated: use timeouts instead""")
+
         return pulumi.get(self, "wait_timeout_minutes")
 
     @wait_timeout_minutes.setter
     def wait_timeout_minutes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "wait_timeout_minutes", value)
 
 
@@ -258,14 +264,17 @@
         if status is not None:
             pulumi.set(__self__, "status", status)
         if storage_class_config is not None:
             pulumi.set(__self__, "storage_class_config", storage_class_config)
         if version is not None:
             pulumi.set(__self__, "version", version)
         if wait_timeout_minutes is not None:
+            warnings.warn("""use timeouts instead""", DeprecationWarning)
+            pulumi.log.warn("""wait_timeout_minutes is deprecated: use timeouts instead""")
+        if wait_timeout_minutes is not None:
             pulumi.set(__self__, "wait_timeout_minutes", wait_timeout_minutes)
         if worker_node_pool is not None:
             pulumi.set(__self__, "worker_node_pool", worker_node_pool)
 
     @property
     @pulumi.getter(name="activePassiveConfig")
     def active_passive_config(self) -> Optional[pulumi.Input['KarbonClusterActivePassiveConfigArgs']]:
@@ -415,14 +424,17 @@
 
     @property
     @pulumi.getter(name="waitTimeoutMinutes")
     def wait_timeout_minutes(self) -> Optional[pulumi.Input[int]]:
         """
         - (Optional) Maximum wait time for the Karbon cluster to provision.
         """
+        warnings.warn("""use timeouts instead""", DeprecationWarning)
+        pulumi.log.warn("""wait_timeout_minutes is deprecated: use timeouts instead""")
+
         return pulumi.get(self, "wait_timeout_minutes")
 
     @wait_timeout_minutes.setter
     def wait_timeout_minutes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "wait_timeout_minutes", value)
 
     @property
@@ -506,14 +518,63 @@
                     prism_element_cluster_uuid="my_pe_cluster_uuid",
                 ),
                 node_os_version="ntnx-1.0",
                 num_instances=1,
             ))
         ```
 
+        ### resource to create karbon cluster with timeouts
+        ```python
+        import pulumi
+        import pulumi_nutanix as nutanix
+
+        example_cluster = nutanix.KarbonCluster("exampleCluster",
+            cni_config=nutanix.KarbonClusterCniConfigArgs(
+                node_cidr_mask_size=24,
+                pod_ipv4_cidr="172.20.0.0/16",
+                service_ipv4_cidr="172.19.0.0/16",
+            ),
+            etcd_node_pool=nutanix.KarbonClusterEtcdNodePoolArgs(
+                ahv_config=nutanix.KarbonClusterEtcdNodePoolAhvConfigArgs(
+                    network_uuid="my_subnet_id",
+                    prism_element_cluster_uuid="my_pe_cluster_uuid",
+                ),
+                node_os_version="ntnx-1.0",
+                num_instances=1,
+            ),
+            master_node_pool=nutanix.KarbonClusterMasterNodePoolArgs(
+                ahv_config=nutanix.KarbonClusterMasterNodePoolAhvConfigArgs(
+                    network_uuid="my_subnet_id",
+                    prism_element_cluster_uuid="my_pe_cluster_uuid",
+                ),
+                node_os_version="ntnx-1.0",
+                num_instances=1,
+            ),
+            storage_class_config=nutanix.KarbonClusterStorageClassConfigArgs(
+                reclaim_policy="Delete",
+                volumes_config=nutanix.KarbonClusterStorageClassConfigVolumesConfigArgs(
+                    file_system="ext4",
+                    flash_mode=False,
+                    password="my_pe_pw",
+                    prism_element_cluster_uuid="my_pe_cluster_uuid",
+                    storage_container="my_storage_container_name",
+                    username="my_pe_username",
+                ),
+            ),
+            version="1.18.15-1",
+            worker_node_pool=nutanix.KarbonClusterWorkerNodePoolArgs(
+                ahv_config=nutanix.KarbonClusterWorkerNodePoolAhvConfigArgs(
+                    network_uuid="my_subnet_id",
+                    prism_element_cluster_uuid="my_pe_cluster_uuid",
+                ),
+                node_os_version="ntnx-1.0",
+                num_instances=1,
+            ))
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['KarbonClusterActivePassiveConfigArgs']] active_passive_config: - (Optional) The active passive mode uses the Virtual Router Redundancy Protocol (VRRP) protocol to provide high availability of the master. **Note:** Updates to this attribute forces new resource creation.
         :param pulumi.Input[pulumi.InputType['KarbonClusterCniConfigArgs']] cni_config: - (Required) K8s cluster networking configuration. The flannel or the calico configuration needs to be provided. **Note:** Updates to this attribute forces new resource creation.
         :param pulumi.Input[pulumi.InputType['KarbonClusterEtcdNodePoolArgs']] etcd_node_pool: - (Required) Configuration of the node pools that the nodes in the etcd cluster belong to. The etcd nodes require a minimum of 8,192 MiB memory and 409,60 MiB disk space.
         :param pulumi.Input[pulumi.InputType['KarbonClusterExternalLbConfigArgs']] external_lb_config: - (Optional) The external load balancer configuration in the case of a multi-master-external-load-balancer type master deployment. **Note:** Updates to this attribute forces new resource creation.
         :param pulumi.Input[pulumi.InputType['KarbonClusterMasterNodePoolArgs']] master_node_pool: - (Required) Configuration of the master node pools.
@@ -583,14 +644,63 @@
                     prism_element_cluster_uuid="my_pe_cluster_uuid",
                 ),
                 node_os_version="ntnx-1.0",
                 num_instances=1,
             ))
         ```
 
+        ### resource to create karbon cluster with timeouts
+        ```python
+        import pulumi
+        import pulumi_nutanix as nutanix
+
+        example_cluster = nutanix.KarbonCluster("exampleCluster",
+            cni_config=nutanix.KarbonClusterCniConfigArgs(
+                node_cidr_mask_size=24,
+                pod_ipv4_cidr="172.20.0.0/16",
+                service_ipv4_cidr="172.19.0.0/16",
+            ),
+            etcd_node_pool=nutanix.KarbonClusterEtcdNodePoolArgs(
+                ahv_config=nutanix.KarbonClusterEtcdNodePoolAhvConfigArgs(
+                    network_uuid="my_subnet_id",
+                    prism_element_cluster_uuid="my_pe_cluster_uuid",
+                ),
+                node_os_version="ntnx-1.0",
+                num_instances=1,
+            ),
+            master_node_pool=nutanix.KarbonClusterMasterNodePoolArgs(
+                ahv_config=nutanix.KarbonClusterMasterNodePoolAhvConfigArgs(
+                    network_uuid="my_subnet_id",
+                    prism_element_cluster_uuid="my_pe_cluster_uuid",
+                ),
+                node_os_version="ntnx-1.0",
+                num_instances=1,
+            ),
+            storage_class_config=nutanix.KarbonClusterStorageClassConfigArgs(
+                reclaim_policy="Delete",
+                volumes_config=nutanix.KarbonClusterStorageClassConfigVolumesConfigArgs(
+                    file_system="ext4",
+                    flash_mode=False,
+                    password="my_pe_pw",
+                    prism_element_cluster_uuid="my_pe_cluster_uuid",
+                    storage_container="my_storage_container_name",
+                    username="my_pe_username",
+                ),
+            ),
+            version="1.18.15-1",
+            worker_node_pool=nutanix.KarbonClusterWorkerNodePoolArgs(
+                ahv_config=nutanix.KarbonClusterWorkerNodePoolAhvConfigArgs(
+                    network_uuid="my_subnet_id",
+                    prism_element_cluster_uuid="my_pe_cluster_uuid",
+                ),
+                node_os_version="ntnx-1.0",
+                num_instances=1,
+            ))
+        ```
+
         :param str resource_name: The name of the resource.
         :param KarbonClusterArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(KarbonClusterArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -812,14 +922,17 @@
 
     @property
     @pulumi.getter(name="waitTimeoutMinutes")
     def wait_timeout_minutes(self) -> pulumi.Output[Optional[int]]:
         """
         - (Optional) Maximum wait time for the Karbon cluster to provision.
         """
+        warnings.warn("""use timeouts instead""", DeprecationWarning)
+        pulumi.log.warn("""wait_timeout_minutes is deprecated: use timeouts instead""")
+
         return pulumi.get(self, "wait_timeout_minutes")
 
     @property
     @pulumi.getter(name="workerNodePool")
     def worker_node_pool(self) -> pulumi.Output['outputs.KarbonClusterWorkerNodePool']:
         return pulumi.get(self, "worker_node_pool")
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/karbon_private_registry.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/karbon_private_registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,54 +10,43 @@
 from . import _utilities
 
 __all__ = ['KarbonPrivateRegistryArgs', 'KarbonPrivateRegistry']
 
 @pulumi.input_type
 class KarbonPrivateRegistryArgs:
     def __init__(__self__, *,
-                 port: pulumi.Input[int],
                  url: pulumi.Input[str],
                  cert: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
+                 port: Optional[pulumi.Input[int]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a KarbonPrivateRegistry resource.
-        :param pulumi.Input[int] port: - (Optional) Port of the private registry.
         :param pulumi.Input[str] url: - (Optional) URL of the private registry. **Note:** Updates to this attribute forces new resource creation.
         :param pulumi.Input[str] cert: - (Optional) Certificate of the private registry in format of base64-encoded byte array. **Note:** Updates to this attribute forces new resource creation.
         :param pulumi.Input[str] name: - (Required) Name of the private registry configuration. **Note:** Updates to this attribute forces new resource creation.
         :param pulumi.Input[str] password: - (Optional) Password for authentication to the private registry. **Note:** Updates to this attribute forces new resource creation.
+        :param pulumi.Input[int] port: - (Optional) Port of the private registry.
         :param pulumi.Input[str] username: - (Optional) Username for authentication to the private registry. **Note:** Updates to this attribute forces new resource creation.
         """
-        pulumi.set(__self__, "port", port)
         pulumi.set(__self__, "url", url)
         if cert is not None:
             pulumi.set(__self__, "cert", cert)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if password is not None:
             pulumi.set(__self__, "password", password)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
-    def port(self) -> pulumi.Input[int]:
-        """
-        - (Optional) Port of the private registry.
-        """
-        return pulumi.get(self, "port")
-
-    @port.setter
-    def port(self, value: pulumi.Input[int]):
-        pulumi.set(self, "port", value)
-
-    @property
-    @pulumi.getter
     def url(self) -> pulumi.Input[str]:
         """
         - (Optional) URL of the private registry. **Note:** Updates to this attribute forces new resource creation.
         """
         return pulumi.get(self, "url")
 
     @url.setter
@@ -98,14 +87,26 @@
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
+    def port(self) -> Optional[pulumi.Input[int]]:
+        """
+        - (Optional) Port of the private registry.
+        """
+        return pulumi.get(self, "port")
+
+    @port.setter
+    def port(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port", value)
+
+    @property
+    @pulumi.getter
     def username(self) -> Optional[pulumi.Input[str]]:
         """
         - (Optional) Username for authentication to the private registry. **Note:** Updates to this attribute forces new resource creation.
         """
         return pulumi.get(self, "username")
 
     @username.setter
@@ -315,16 +316,14 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KarbonPrivateRegistryArgs.__new__(KarbonPrivateRegistryArgs)
 
             __props__.__dict__["cert"] = cert
             __props__.__dict__["name"] = name
             __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
-            if port is None and not opts.urn:
-                raise TypeError("Missing required property 'port'")
             __props__.__dict__["port"] = port
             if url is None and not opts.urn:
                 raise TypeError("Missing required property 'url'")
             __props__.__dict__["url"] = url
             __props__.__dict__["username"] = username
             __props__.__dict__["endpoint"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
@@ -404,15 +403,15 @@
         """
         - (Optional) Password for authentication to the private registry. **Note:** Updates to this attribute forces new resource creation.
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
-    def port(self) -> pulumi.Output[int]:
+    def port(self) -> pulumi.Output[Optional[int]]:
         """
         - (Optional) Port of the private registry.
         """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/network_security_rule.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/network_security_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1043,14 +1043,15 @@
                  __props__=None):
         """
         Provides a Nutanix network security rule resource to Create a network security rule.
 
         > NOTE: The use of network_security_rule is only applicable in AHV clusters and requires Microsegmentation to be enabled. This feature is a function of the Flow product and requires a Flow license. For more information on Flow and Microsegmentation please visit https://www.nutanix.com/products/flow
 
         ## Example Usage
+
         ### Isolation Rule Example
 
         ```python
         import pulumi
         import pulumi_nutanix as nutanix
 
         isolation = nutanix.NetworkSecurityRule("isolation",
@@ -1065,14 +1066,15 @@
             isolation_rule_second_entity_filter_kind_lists=["vm"],
             isolation_rule_second_entity_filter_params=[nutanix.NetworkSecurityRuleIsolationRuleSecondEntityFilterParamArgs(
                 name="Environment",
                 values=["Production"],
             )],
             isolation_rule_second_entity_filter_type="CATEGORIES_MATCH_ALL")
         ```
+
         ### Usage with service and address groups
         ```python
         import pulumi
         import pulumi_nutanix as nutanix
 
         service1 = nutanix.ServiceGroup("service1",
             description="test",
@@ -1168,14 +1170,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Nutanix network security rule resource to Create a network security rule.
 
         > NOTE: The use of network_security_rule is only applicable in AHV clusters and requires Microsegmentation to be enabled. This feature is a function of the Flow product and requires a Flow license. For more information on Flow and Microsegmentation please visit https://www.nutanix.com/products/flow
 
         ## Example Usage
+
         ### Isolation Rule Example
 
         ```python
         import pulumi
         import pulumi_nutanix as nutanix
 
         isolation = nutanix.NetworkSecurityRule("isolation",
@@ -1190,14 +1193,15 @@
             isolation_rule_second_entity_filter_kind_lists=["vm"],
             isolation_rule_second_entity_filter_params=[nutanix.NetworkSecurityRuleIsolationRuleSecondEntityFilterParamArgs(
                 name="Environment",
                 values=["Production"],
             )],
             isolation_rule_second_entity_filter_type="CATEGORIES_MATCH_ALL")
         ```
+
         ### Usage with service and address groups
         ```python
         import pulumi
         import pulumi_nutanix as nutanix
 
         service1 = nutanix.ServiceGroup("service1",
             description="test",
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/pbr.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/pbr.py`

 * *Files 3% similar despite different names*

```diff
@@ -418,14 +418,15 @@
                  vpc_name: Optional[pulumi.Input[str]] = None,
                  vpc_reference_uuid: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides Nutanix resource to create Policy Based Routing inside VPCs.
 
         ## Example Usage
+
         ### pbr creation with vpc name with any source or destination or protocol with permit action
 
         ```python
         import pulumi
         import pulumi_nutanix as nutanix
 
         pbr = nutanix.Pbr("pbr",
@@ -436,48 +437,14 @@
             priority=123,
             protocol_type="ALL",
             source=nutanix.PbrSourceArgs(
                 address_type="ALL",
             ),
             vpc_name="test123")
         ```
-        ## source
-
-        source address of an IP packet. This could be either an ip prefix or an address_type .
-
-        * `address` - (Optional) address type of source. Should be one of {INTERNET, ALL}.
-        * `subnet_ip` - (Optional) IP subnet provided as an address.
-        * `prefix_length` - (Optional) prefix length of provided subnet.
-
-        ## destination
-
-        destination address of an IP packet. This could be either an ip prefix or an address_type .
-
-        * `address` - (Optional) address type of source. Should be one of {INTERNET, ALL}.
-        * `subnet_ip` - (Optional) IP subnet provided as an address.
-        * `prefix_length` - (Optional) prefix length of provided subnet.
-
-        ## protocol_parameters
-
-        Routing policy IP protocol parameters
-
-        * `tcp` - (Optional) TCP parameters in routing policy
-        * `udp` - (Optional) UDP parameters in routing policy
-        * `icmp` - (Optional) ICMP parameters in routing policy.
-        * `protocol_number` - (Optional) Protocol number in routing policy
-
-        ## tcp, udp
-
-        * `source_port_range` - (Required) Range of TCP/UDP ports.
-        * `destination_port_range` - (Required) Range of TCP/UDP ports.
-
-        ## source_port_range, destination_port_range
-
-        * `start_port` - (Required) start port number
-        * `end_port` - (Required) end port number
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] action: Routing policy action. Must be one of {DENY, PERMIT, REROUTE} .
         :param pulumi.Input[str] api_version: The version of the API.
         :param pulumi.Input[bool] is_bidirectional: Additionally create Policy in reverse direction. Should be used with {TCP, UDP with start and end port ranges and ICMP with icmp code and type}. Supported with 2022.x.
         :param pulumi.Input[str] name: name of policy
@@ -493,14 +460,15 @@
                  resource_name: str,
                  args: PbrArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides Nutanix resource to create Policy Based Routing inside VPCs.
 
         ## Example Usage
+
         ### pbr creation with vpc name with any source or destination or protocol with permit action
 
         ```python
         import pulumi
         import pulumi_nutanix as nutanix
 
         pbr = nutanix.Pbr("pbr",
@@ -511,48 +479,14 @@
             priority=123,
             protocol_type="ALL",
             source=nutanix.PbrSourceArgs(
                 address_type="ALL",
             ),
             vpc_name="test123")
         ```
-        ## source
-
-        source address of an IP packet. This could be either an ip prefix or an address_type .
-
-        * `address` - (Optional) address type of source. Should be one of {INTERNET, ALL}.
-        * `subnet_ip` - (Optional) IP subnet provided as an address.
-        * `prefix_length` - (Optional) prefix length of provided subnet.
-
-        ## destination
-
-        destination address of an IP packet. This could be either an ip prefix or an address_type .
-
-        * `address` - (Optional) address type of source. Should be one of {INTERNET, ALL}.
-        * `subnet_ip` - (Optional) IP subnet provided as an address.
-        * `prefix_length` - (Optional) prefix length of provided subnet.
-
-        ## protocol_parameters
-
-        Routing policy IP protocol parameters
-
-        * `tcp` - (Optional) TCP parameters in routing policy
-        * `udp` - (Optional) UDP parameters in routing policy
-        * `icmp` - (Optional) ICMP parameters in routing policy.
-        * `protocol_number` - (Optional) Protocol number in routing policy
-
-        ## tcp, udp
-
-        * `source_port_range` - (Required) Range of TCP/UDP ports.
-        * `destination_port_range` - (Required) Range of TCP/UDP ports.
-
-        ## source_port_range, destination_port_range
-
-        * `start_port` - (Required) start port number
-        * `end_port` - (Required) end port number
 
         :param str resource_name: The name of the resource.
         :param PbrArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/project.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/project.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,69 +15,63 @@
 
 @pulumi.input_type
 class ProjectArgs:
     def __init__(__self__, *,
                  default_subnet_reference: pulumi.Input['ProjectDefaultSubnetReferenceArgs'],
                  description: pulumi.Input[str],
                  account_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectAccountReferenceListArgs']]]] = None,
+                 acps: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectAcpArgs']]]] = None,
                  api_version: Optional[pulumi.Input[str]] = None,
                  categories: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectCategoryArgs']]]] = None,
+                 cluster_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectClusterReferenceListArgs']]]] = None,
+                 cluster_uuid: Optional[pulumi.Input[str]] = None,
+                 default_environment_reference: Optional[pulumi.Input['ProjectDefaultEnvironmentReferenceArgs']] = None,
+                 enable_collab: Optional[pulumi.Input[bool]] = None,
                  environment_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentReferenceListArgs']]]] = None,
                  external_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectExternalNetworkListArgs']]]] = None,
                  external_user_group_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectExternalUserGroupReferenceListArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  owner_reference: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  project_reference: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  resource_domain: Optional[pulumi.Input['ProjectResourceDomainArgs']] = None,
                  subnet_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectSubnetReferenceListArgs']]]] = None,
-                 user_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserReferenceListArgs']]]] = None):
+                 tunnel_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTunnelReferenceListArgs']]]] = None,
+                 use_project_internal: Optional[pulumi.Input[bool]] = None,
+                 user_group_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserGroupListArgs']]]] = None,
+                 user_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserListArgs']]]] = None,
+                 user_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserReferenceListArgs']]]] = None,
+                 vpc_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectVpcReferenceListArgs']]]] = None):
         """
         The set of arguments for constructing a Project resource.
-        :param pulumi.Input['ProjectDefaultSubnetReferenceArgs'] default_subnet_reference: Reference to a subnet.
-               * `default_subnet_reference.kind` - (Optional) The kind name. Default value is `subnet`
-               * `default_subnet_reference.uuid` - (Required) The UUID of a subnet.
-               * `default_subnet_reference.name` - (Optional/Computed) The name of a subnet.
         :param pulumi.Input[str] description: A description for project.
-        :param pulumi.Input[Sequence[pulumi.Input['ProjectAccountReferenceListArgs']]] account_reference_lists: List of accounts associated with the project.
-               * `account_reference_list.#.kind` - (Optional) The kind name. Default value is `account`
-               * `account_reference_list.#.uuid` - (Required) The UUID of an account.
-               * `account_reference_list.#.name` - (Optional/Computed) The name of an account.
-        :param pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentReferenceListArgs']]] environment_reference_lists: List of environments associated with the project.
-               * `environment_reference_list.#.kind` - (Optional) The kind name. Default value is `environment`
-               * `environment_reference_list.#.uuid` - (Required) The UUID of an environment.
-               * `environment_reference_list.#.name` - (Optional/Computed) The name of an environment.
-        :param pulumi.Input[Sequence[pulumi.Input['ProjectExternalNetworkListArgs']]] external_network_lists: List of external networks associated with the project.
-               * `external_network_list.#.uuid` - (Required) The UUID of a network.
-               * `external_network_list.#.name` - (Optional/Computed) The name of a network.
-        :param pulumi.Input[Sequence[pulumi.Input['ProjectExternalUserGroupReferenceListArgs']]] external_user_group_reference_lists: List of directory service user groups. These groups are not managed by Nutanix.
-               * `external_user_group_reference_list.#.kind` - (Optional) The kind name. Default value is `user_group`
-               * `external_user_group_reference_list.#.uuid` - (Required) The UUID of a user_group
-               * `external_user_group_reference_list.#.name` - (Optional/Computed) The name of a user_group
+        :param pulumi.Input[Sequence[pulumi.Input['ProjectCategoryArgs']]] categories: - (Optional) The category values represented as a dictionary of key > list of values.
+        :param pulumi.Input[str] cluster_uuid: The UUID of cluster. (Required when using project_internal flag).
+        :param pulumi.Input[bool] enable_collab: flag to allow collaboration of projects. (Use with project_internal flag)
         :param pulumi.Input[str] name: The name for the project.
-        :param pulumi.Input['ProjectResourceDomainArgs'] resource_domain: The status for a resource domain (limits and values)
-               * `resource_domain.resources` - (Required) Array of the utilization/limit for resource types
-               * `resource_domain.resources.#.limit` - (Required) The resource consumption limit (unspecified is unlimited)
-               * `resource_domain.resources.#.resource_type` - (Required) The type of resource (for example storage, CPUs)
-        :param pulumi.Input[Sequence[pulumi.Input['ProjectSubnetReferenceListArgs']]] subnet_reference_lists: List of subnets for the project.
-               * `subnet_reference_list.#.kind` - (Optional) The kind name. Default value is `subnet`
-               * `subnet_reference_list.#.uuid` - (Required) The UUID of a subnet
-               * `subnet_reference_list.#.name` - (Optional/Computed) The name of a subnet.
-        :param pulumi.Input[Sequence[pulumi.Input['ProjectUserReferenceListArgs']]] user_reference_lists: List of users in the project.
-               * `user_reference_list.#.kind` - (Optional) The kind name. Default value is `user`
-               * `user_reference_list.#.uuid` - (Required) The UUID of a user
-               * `user_reference_list.#.name` - (Optional/Computed) The name of a user.
+        :param pulumi.Input[bool] use_project_internal: flag to use project internal for user role mapping
+        :param pulumi.Input[Sequence[pulumi.Input['ProjectUserReferenceListArgs']]] user_reference_lists: List of Reference of users.
         """
         pulumi.set(__self__, "default_subnet_reference", default_subnet_reference)
         pulumi.set(__self__, "description", description)
         if account_reference_lists is not None:
             pulumi.set(__self__, "account_reference_lists", account_reference_lists)
+        if acps is not None:
+            pulumi.set(__self__, "acps", acps)
         if api_version is not None:
             pulumi.set(__self__, "api_version", api_version)
         if categories is not None:
             pulumi.set(__self__, "categories", categories)
+        if cluster_reference_lists is not None:
+            pulumi.set(__self__, "cluster_reference_lists", cluster_reference_lists)
+        if cluster_uuid is not None:
+            pulumi.set(__self__, "cluster_uuid", cluster_uuid)
+        if default_environment_reference is not None:
+            pulumi.set(__self__, "default_environment_reference", default_environment_reference)
+        if enable_collab is not None:
+            pulumi.set(__self__, "enable_collab", enable_collab)
         if environment_reference_lists is not None:
             pulumi.set(__self__, "environment_reference_lists", environment_reference_lists)
         if external_network_lists is not None:
             pulumi.set(__self__, "external_network_lists", external_network_lists)
         if external_user_group_reference_lists is not None:
             pulumi.set(__self__, "external_user_group_reference_lists", external_user_group_reference_lists)
         if name is not None:
@@ -86,26 +80,30 @@
             pulumi.set(__self__, "owner_reference", owner_reference)
         if project_reference is not None:
             pulumi.set(__self__, "project_reference", project_reference)
         if resource_domain is not None:
             pulumi.set(__self__, "resource_domain", resource_domain)
         if subnet_reference_lists is not None:
             pulumi.set(__self__, "subnet_reference_lists", subnet_reference_lists)
+        if tunnel_reference_lists is not None:
+            pulumi.set(__self__, "tunnel_reference_lists", tunnel_reference_lists)
+        if use_project_internal is not None:
+            pulumi.set(__self__, "use_project_internal", use_project_internal)
+        if user_group_lists is not None:
+            pulumi.set(__self__, "user_group_lists", user_group_lists)
+        if user_lists is not None:
+            pulumi.set(__self__, "user_lists", user_lists)
         if user_reference_lists is not None:
             pulumi.set(__self__, "user_reference_lists", user_reference_lists)
+        if vpc_reference_lists is not None:
+            pulumi.set(__self__, "vpc_reference_lists", vpc_reference_lists)
 
     @property
     @pulumi.getter(name="defaultSubnetReference")
     def default_subnet_reference(self) -> pulumi.Input['ProjectDefaultSubnetReferenceArgs']:
-        """
-        Reference to a subnet.
-        * `default_subnet_reference.kind` - (Optional) The kind name. Default value is `subnet`
-        * `default_subnet_reference.uuid` - (Required) The UUID of a subnet.
-        * `default_subnet_reference.name` - (Optional/Computed) The name of a subnet.
-        """
         return pulumi.get(self, "default_subnet_reference")
 
     @default_subnet_reference.setter
     def default_subnet_reference(self, value: pulumi.Input['ProjectDefaultSubnetReferenceArgs']):
         pulumi.set(self, "default_subnet_reference", value)
 
     @property
@@ -119,82 +117,113 @@
     @description.setter
     def description(self, value: pulumi.Input[str]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="accountReferenceLists")
     def account_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectAccountReferenceListArgs']]]]:
-        """
-        List of accounts associated with the project.
-        * `account_reference_list.#.kind` - (Optional) The kind name. Default value is `account`
-        * `account_reference_list.#.uuid` - (Required) The UUID of an account.
-        * `account_reference_list.#.name` - (Optional/Computed) The name of an account.
-        """
         return pulumi.get(self, "account_reference_lists")
 
     @account_reference_lists.setter
     def account_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectAccountReferenceListArgs']]]]):
         pulumi.set(self, "account_reference_lists", value)
 
     @property
+    @pulumi.getter
+    def acps(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectAcpArgs']]]]:
+        return pulumi.get(self, "acps")
+
+    @acps.setter
+    def acps(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectAcpArgs']]]]):
+        pulumi.set(self, "acps", value)
+
+    @property
     @pulumi.getter(name="apiVersion")
     def api_version(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "api_version")
 
     @api_version.setter
     def api_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_version", value)
 
     @property
     @pulumi.getter
     def categories(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectCategoryArgs']]]]:
+        """
+        - (Optional) The category values represented as a dictionary of key > list of values.
+        """
         return pulumi.get(self, "categories")
 
     @categories.setter
     def categories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectCategoryArgs']]]]):
         pulumi.set(self, "categories", value)
 
     @property
-    @pulumi.getter(name="environmentReferenceLists")
-    def environment_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentReferenceListArgs']]]]:
+    @pulumi.getter(name="clusterReferenceLists")
+    def cluster_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectClusterReferenceListArgs']]]]:
+        return pulumi.get(self, "cluster_reference_lists")
+
+    @cluster_reference_lists.setter
+    def cluster_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectClusterReferenceListArgs']]]]):
+        pulumi.set(self, "cluster_reference_lists", value)
+
+    @property
+    @pulumi.getter(name="clusterUuid")
+    def cluster_uuid(self) -> Optional[pulumi.Input[str]]:
+        """
+        The UUID of cluster. (Required when using project_internal flag).
+        """
+        return pulumi.get(self, "cluster_uuid")
+
+    @cluster_uuid.setter
+    def cluster_uuid(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cluster_uuid", value)
+
+    @property
+    @pulumi.getter(name="defaultEnvironmentReference")
+    def default_environment_reference(self) -> Optional[pulumi.Input['ProjectDefaultEnvironmentReferenceArgs']]:
+        return pulumi.get(self, "default_environment_reference")
+
+    @default_environment_reference.setter
+    def default_environment_reference(self, value: Optional[pulumi.Input['ProjectDefaultEnvironmentReferenceArgs']]):
+        pulumi.set(self, "default_environment_reference", value)
+
+    @property
+    @pulumi.getter(name="enableCollab")
+    def enable_collab(self) -> Optional[pulumi.Input[bool]]:
         """
-        List of environments associated with the project.
-        * `environment_reference_list.#.kind` - (Optional) The kind name. Default value is `environment`
-        * `environment_reference_list.#.uuid` - (Required) The UUID of an environment.
-        * `environment_reference_list.#.name` - (Optional/Computed) The name of an environment.
+        flag to allow collaboration of projects. (Use with project_internal flag)
         """
+        return pulumi.get(self, "enable_collab")
+
+    @enable_collab.setter
+    def enable_collab(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_collab", value)
+
+    @property
+    @pulumi.getter(name="environmentReferenceLists")
+    def environment_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentReferenceListArgs']]]]:
         return pulumi.get(self, "environment_reference_lists")
 
     @environment_reference_lists.setter
     def environment_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentReferenceListArgs']]]]):
         pulumi.set(self, "environment_reference_lists", value)
 
     @property
     @pulumi.getter(name="externalNetworkLists")
     def external_network_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectExternalNetworkListArgs']]]]:
-        """
-        List of external networks associated with the project.
-        * `external_network_list.#.uuid` - (Required) The UUID of a network.
-        * `external_network_list.#.name` - (Optional/Computed) The name of a network.
-        """
         return pulumi.get(self, "external_network_lists")
 
     @external_network_lists.setter
     def external_network_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectExternalNetworkListArgs']]]]):
         pulumi.set(self, "external_network_lists", value)
 
     @property
     @pulumi.getter(name="externalUserGroupReferenceLists")
     def external_user_group_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectExternalUserGroupReferenceListArgs']]]]:
-        """
-        List of directory service user groups. These groups are not managed by Nutanix.
-        * `external_user_group_reference_list.#.kind` - (Optional) The kind name. Default value is `user_group`
-        * `external_user_group_reference_list.#.uuid` - (Required) The UUID of a user_group
-        * `external_user_group_reference_list.#.name` - (Optional/Computed) The name of a user_group
-        """
         return pulumi.get(self, "external_user_group_reference_lists")
 
     @external_user_group_reference_lists.setter
     def external_user_group_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectExternalUserGroupReferenceListArgs']]]]):
         pulumi.set(self, "external_user_group_reference_lists", value)
 
     @property
@@ -226,123 +255,150 @@
     @project_reference.setter
     def project_reference(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "project_reference", value)
 
     @property
     @pulumi.getter(name="resourceDomain")
     def resource_domain(self) -> Optional[pulumi.Input['ProjectResourceDomainArgs']]:
-        """
-        The status for a resource domain (limits and values)
-        * `resource_domain.resources` - (Required) Array of the utilization/limit for resource types
-        * `resource_domain.resources.#.limit` - (Required) The resource consumption limit (unspecified is unlimited)
-        * `resource_domain.resources.#.resource_type` - (Required) The type of resource (for example storage, CPUs)
-        """
         return pulumi.get(self, "resource_domain")
 
     @resource_domain.setter
     def resource_domain(self, value: Optional[pulumi.Input['ProjectResourceDomainArgs']]):
         pulumi.set(self, "resource_domain", value)
 
     @property
     @pulumi.getter(name="subnetReferenceLists")
     def subnet_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectSubnetReferenceListArgs']]]]:
-        """
-        List of subnets for the project.
-        * `subnet_reference_list.#.kind` - (Optional) The kind name. Default value is `subnet`
-        * `subnet_reference_list.#.uuid` - (Required) The UUID of a subnet
-        * `subnet_reference_list.#.name` - (Optional/Computed) The name of a subnet.
-        """
         return pulumi.get(self, "subnet_reference_lists")
 
     @subnet_reference_lists.setter
     def subnet_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectSubnetReferenceListArgs']]]]):
         pulumi.set(self, "subnet_reference_lists", value)
 
     @property
+    @pulumi.getter(name="tunnelReferenceLists")
+    def tunnel_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTunnelReferenceListArgs']]]]:
+        return pulumi.get(self, "tunnel_reference_lists")
+
+    @tunnel_reference_lists.setter
+    def tunnel_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTunnelReferenceListArgs']]]]):
+        pulumi.set(self, "tunnel_reference_lists", value)
+
+    @property
+    @pulumi.getter(name="useProjectInternal")
+    def use_project_internal(self) -> Optional[pulumi.Input[bool]]:
+        """
+        flag to use project internal for user role mapping
+        """
+        return pulumi.get(self, "use_project_internal")
+
+    @use_project_internal.setter
+    def use_project_internal(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "use_project_internal", value)
+
+    @property
+    @pulumi.getter(name="userGroupLists")
+    def user_group_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserGroupListArgs']]]]:
+        return pulumi.get(self, "user_group_lists")
+
+    @user_group_lists.setter
+    def user_group_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserGroupListArgs']]]]):
+        pulumi.set(self, "user_group_lists", value)
+
+    @property
+    @pulumi.getter(name="userLists")
+    def user_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserListArgs']]]]:
+        return pulumi.get(self, "user_lists")
+
+    @user_lists.setter
+    def user_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserListArgs']]]]):
+        pulumi.set(self, "user_lists", value)
+
+    @property
     @pulumi.getter(name="userReferenceLists")
     def user_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserReferenceListArgs']]]]:
         """
-        List of users in the project.
-        * `user_reference_list.#.kind` - (Optional) The kind name. Default value is `user`
-        * `user_reference_list.#.uuid` - (Required) The UUID of a user
-        * `user_reference_list.#.name` - (Optional/Computed) The name of a user.
+        List of Reference of users.
         """
         return pulumi.get(self, "user_reference_lists")
 
     @user_reference_lists.setter
     def user_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserReferenceListArgs']]]]):
         pulumi.set(self, "user_reference_lists", value)
 
+    @property
+    @pulumi.getter(name="vpcReferenceLists")
+    def vpc_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectVpcReferenceListArgs']]]]:
+        return pulumi.get(self, "vpc_reference_lists")
+
+    @vpc_reference_lists.setter
+    def vpc_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectVpcReferenceListArgs']]]]):
+        pulumi.set(self, "vpc_reference_lists", value)
+
 
 @pulumi.input_type
 class _ProjectState:
     def __init__(__self__, *,
                  account_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectAccountReferenceListArgs']]]] = None,
+                 acps: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectAcpArgs']]]] = None,
                  api_version: Optional[pulumi.Input[str]] = None,
                  categories: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectCategoryArgs']]]] = None,
+                 cluster_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectClusterReferenceListArgs']]]] = None,
+                 cluster_uuid: Optional[pulumi.Input[str]] = None,
+                 default_environment_reference: Optional[pulumi.Input['ProjectDefaultEnvironmentReferenceArgs']] = None,
                  default_subnet_reference: Optional[pulumi.Input['ProjectDefaultSubnetReferenceArgs']] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 enable_collab: Optional[pulumi.Input[bool]] = None,
                  environment_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentReferenceListArgs']]]] = None,
                  external_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectExternalNetworkListArgs']]]] = None,
                  external_user_group_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectExternalUserGroupReferenceListArgs']]]] = None,
                  is_default: Optional[pulumi.Input[bool]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  owner_reference: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  project_reference: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  resource_domain: Optional[pulumi.Input['ProjectResourceDomainArgs']] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  subnet_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectSubnetReferenceListArgs']]]] = None,
-                 user_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserReferenceListArgs']]]] = None):
+                 tunnel_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTunnelReferenceListArgs']]]] = None,
+                 use_project_internal: Optional[pulumi.Input[bool]] = None,
+                 user_group_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserGroupListArgs']]]] = None,
+                 user_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserListArgs']]]] = None,
+                 user_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserReferenceListArgs']]]] = None,
+                 vpc_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectVpcReferenceListArgs']]]] = None):
         """
         Input properties used for looking up and filtering Project resources.
-        :param pulumi.Input[Sequence[pulumi.Input['ProjectAccountReferenceListArgs']]] account_reference_lists: List of accounts associated with the project.
-               * `account_reference_list.#.kind` - (Optional) The kind name. Default value is `account`
-               * `account_reference_list.#.uuid` - (Required) The UUID of an account.
-               * `account_reference_list.#.name` - (Optional/Computed) The name of an account.
-        :param pulumi.Input['ProjectDefaultSubnetReferenceArgs'] default_subnet_reference: Reference to a subnet.
-               * `default_subnet_reference.kind` - (Optional) The kind name. Default value is `subnet`
-               * `default_subnet_reference.uuid` - (Required) The UUID of a subnet.
-               * `default_subnet_reference.name` - (Optional/Computed) The name of a subnet.
+        :param pulumi.Input[Sequence[pulumi.Input['ProjectCategoryArgs']]] categories: - (Optional) The category values represented as a dictionary of key > list of values.
+        :param pulumi.Input[str] cluster_uuid: The UUID of cluster. (Required when using project_internal flag).
         :param pulumi.Input[str] description: A description for project.
-        :param pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentReferenceListArgs']]] environment_reference_lists: List of environments associated with the project.
-               * `environment_reference_list.#.kind` - (Optional) The kind name. Default value is `environment`
-               * `environment_reference_list.#.uuid` - (Required) The UUID of an environment.
-               * `environment_reference_list.#.name` - (Optional/Computed) The name of an environment.
-        :param pulumi.Input[Sequence[pulumi.Input['ProjectExternalNetworkListArgs']]] external_network_lists: List of external networks associated with the project.
-               * `external_network_list.#.uuid` - (Required) The UUID of a network.
-               * `external_network_list.#.name` - (Optional/Computed) The name of a network.
-        :param pulumi.Input[Sequence[pulumi.Input['ProjectExternalUserGroupReferenceListArgs']]] external_user_group_reference_lists: List of directory service user groups. These groups are not managed by Nutanix.
-               * `external_user_group_reference_list.#.kind` - (Optional) The kind name. Default value is `user_group`
-               * `external_user_group_reference_list.#.uuid` - (Required) The UUID of a user_group
-               * `external_user_group_reference_list.#.name` - (Optional/Computed) The name of a user_group
+        :param pulumi.Input[bool] enable_collab: flag to allow collaboration of projects. (Use with project_internal flag)
         :param pulumi.Input[str] name: The name for the project.
-        :param pulumi.Input['ProjectResourceDomainArgs'] resource_domain: The status for a resource domain (limits and values)
-               * `resource_domain.resources` - (Required) Array of the utilization/limit for resource types
-               * `resource_domain.resources.#.limit` - (Required) The resource consumption limit (unspecified is unlimited)
-               * `resource_domain.resources.#.resource_type` - (Required) The type of resource (for example storage, CPUs)
-        :param pulumi.Input[Sequence[pulumi.Input['ProjectSubnetReferenceListArgs']]] subnet_reference_lists: List of subnets for the project.
-               * `subnet_reference_list.#.kind` - (Optional) The kind name. Default value is `subnet`
-               * `subnet_reference_list.#.uuid` - (Required) The UUID of a subnet
-               * `subnet_reference_list.#.name` - (Optional/Computed) The name of a subnet.
-        :param pulumi.Input[Sequence[pulumi.Input['ProjectUserReferenceListArgs']]] user_reference_lists: List of users in the project.
-               * `user_reference_list.#.kind` - (Optional) The kind name. Default value is `user`
-               * `user_reference_list.#.uuid` - (Required) The UUID of a user
-               * `user_reference_list.#.name` - (Optional/Computed) The name of a user.
+        :param pulumi.Input[bool] use_project_internal: flag to use project internal for user role mapping
+        :param pulumi.Input[Sequence[pulumi.Input['ProjectUserReferenceListArgs']]] user_reference_lists: List of Reference of users.
         """
         if account_reference_lists is not None:
             pulumi.set(__self__, "account_reference_lists", account_reference_lists)
+        if acps is not None:
+            pulumi.set(__self__, "acps", acps)
         if api_version is not None:
             pulumi.set(__self__, "api_version", api_version)
         if categories is not None:
             pulumi.set(__self__, "categories", categories)
+        if cluster_reference_lists is not None:
+            pulumi.set(__self__, "cluster_reference_lists", cluster_reference_lists)
+        if cluster_uuid is not None:
+            pulumi.set(__self__, "cluster_uuid", cluster_uuid)
+        if default_environment_reference is not None:
+            pulumi.set(__self__, "default_environment_reference", default_environment_reference)
         if default_subnet_reference is not None:
             pulumi.set(__self__, "default_subnet_reference", default_subnet_reference)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if enable_collab is not None:
+            pulumi.set(__self__, "enable_collab", enable_collab)
         if environment_reference_lists is not None:
             pulumi.set(__self__, "environment_reference_lists", environment_reference_lists)
         if external_network_lists is not None:
             pulumi.set(__self__, "external_network_lists", external_network_lists)
         if external_user_group_reference_lists is not None:
             pulumi.set(__self__, "external_user_group_reference_lists", external_user_group_reference_lists)
         if is_default is not None:
@@ -357,59 +413,99 @@
             pulumi.set(__self__, "project_reference", project_reference)
         if resource_domain is not None:
             pulumi.set(__self__, "resource_domain", resource_domain)
         if state is not None:
             pulumi.set(__self__, "state", state)
         if subnet_reference_lists is not None:
             pulumi.set(__self__, "subnet_reference_lists", subnet_reference_lists)
+        if tunnel_reference_lists is not None:
+            pulumi.set(__self__, "tunnel_reference_lists", tunnel_reference_lists)
+        if use_project_internal is not None:
+            pulumi.set(__self__, "use_project_internal", use_project_internal)
+        if user_group_lists is not None:
+            pulumi.set(__self__, "user_group_lists", user_group_lists)
+        if user_lists is not None:
+            pulumi.set(__self__, "user_lists", user_lists)
         if user_reference_lists is not None:
             pulumi.set(__self__, "user_reference_lists", user_reference_lists)
+        if vpc_reference_lists is not None:
+            pulumi.set(__self__, "vpc_reference_lists", vpc_reference_lists)
 
     @property
     @pulumi.getter(name="accountReferenceLists")
     def account_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectAccountReferenceListArgs']]]]:
-        """
-        List of accounts associated with the project.
-        * `account_reference_list.#.kind` - (Optional) The kind name. Default value is `account`
-        * `account_reference_list.#.uuid` - (Required) The UUID of an account.
-        * `account_reference_list.#.name` - (Optional/Computed) The name of an account.
-        """
         return pulumi.get(self, "account_reference_lists")
 
     @account_reference_lists.setter
     def account_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectAccountReferenceListArgs']]]]):
         pulumi.set(self, "account_reference_lists", value)
 
     @property
+    @pulumi.getter
+    def acps(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectAcpArgs']]]]:
+        return pulumi.get(self, "acps")
+
+    @acps.setter
+    def acps(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectAcpArgs']]]]):
+        pulumi.set(self, "acps", value)
+
+    @property
     @pulumi.getter(name="apiVersion")
     def api_version(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "api_version")
 
     @api_version.setter
     def api_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_version", value)
 
     @property
     @pulumi.getter
     def categories(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectCategoryArgs']]]]:
+        """
+        - (Optional) The category values represented as a dictionary of key > list of values.
+        """
         return pulumi.get(self, "categories")
 
     @categories.setter
     def categories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectCategoryArgs']]]]):
         pulumi.set(self, "categories", value)
 
     @property
-    @pulumi.getter(name="defaultSubnetReference")
-    def default_subnet_reference(self) -> Optional[pulumi.Input['ProjectDefaultSubnetReferenceArgs']]:
+    @pulumi.getter(name="clusterReferenceLists")
+    def cluster_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectClusterReferenceListArgs']]]]:
+        return pulumi.get(self, "cluster_reference_lists")
+
+    @cluster_reference_lists.setter
+    def cluster_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectClusterReferenceListArgs']]]]):
+        pulumi.set(self, "cluster_reference_lists", value)
+
+    @property
+    @pulumi.getter(name="clusterUuid")
+    def cluster_uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Reference to a subnet.
-        * `default_subnet_reference.kind` - (Optional) The kind name. Default value is `subnet`
-        * `default_subnet_reference.uuid` - (Required) The UUID of a subnet.
-        * `default_subnet_reference.name` - (Optional/Computed) The name of a subnet.
+        The UUID of cluster. (Required when using project_internal flag).
         """
+        return pulumi.get(self, "cluster_uuid")
+
+    @cluster_uuid.setter
+    def cluster_uuid(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cluster_uuid", value)
+
+    @property
+    @pulumi.getter(name="defaultEnvironmentReference")
+    def default_environment_reference(self) -> Optional[pulumi.Input['ProjectDefaultEnvironmentReferenceArgs']]:
+        return pulumi.get(self, "default_environment_reference")
+
+    @default_environment_reference.setter
+    def default_environment_reference(self, value: Optional[pulumi.Input['ProjectDefaultEnvironmentReferenceArgs']]):
+        pulumi.set(self, "default_environment_reference", value)
+
+    @property
+    @pulumi.getter(name="defaultSubnetReference")
+    def default_subnet_reference(self) -> Optional[pulumi.Input['ProjectDefaultSubnetReferenceArgs']]:
         return pulumi.get(self, "default_subnet_reference")
 
     @default_subnet_reference.setter
     def default_subnet_reference(self, value: Optional[pulumi.Input['ProjectDefaultSubnetReferenceArgs']]):
         pulumi.set(self, "default_subnet_reference", value)
 
     @property
@@ -421,51 +517,46 @@
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="environmentReferenceLists")
-    def environment_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentReferenceListArgs']]]]:
+    @pulumi.getter(name="enableCollab")
+    def enable_collab(self) -> Optional[pulumi.Input[bool]]:
         """
-        List of environments associated with the project.
-        * `environment_reference_list.#.kind` - (Optional) The kind name. Default value is `environment`
-        * `environment_reference_list.#.uuid` - (Required) The UUID of an environment.
-        * `environment_reference_list.#.name` - (Optional/Computed) The name of an environment.
+        flag to allow collaboration of projects. (Use with project_internal flag)
         """
+        return pulumi.get(self, "enable_collab")
+
+    @enable_collab.setter
+    def enable_collab(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_collab", value)
+
+    @property
+    @pulumi.getter(name="environmentReferenceLists")
+    def environment_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentReferenceListArgs']]]]:
         return pulumi.get(self, "environment_reference_lists")
 
     @environment_reference_lists.setter
     def environment_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectEnvironmentReferenceListArgs']]]]):
         pulumi.set(self, "environment_reference_lists", value)
 
     @property
     @pulumi.getter(name="externalNetworkLists")
     def external_network_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectExternalNetworkListArgs']]]]:
-        """
-        List of external networks associated with the project.
-        * `external_network_list.#.uuid` - (Required) The UUID of a network.
-        * `external_network_list.#.name` - (Optional/Computed) The name of a network.
-        """
         return pulumi.get(self, "external_network_lists")
 
     @external_network_lists.setter
     def external_network_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectExternalNetworkListArgs']]]]):
         pulumi.set(self, "external_network_lists", value)
 
     @property
     @pulumi.getter(name="externalUserGroupReferenceLists")
     def external_user_group_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectExternalUserGroupReferenceListArgs']]]]:
-        """
-        List of directory service user groups. These groups are not managed by Nutanix.
-        * `external_user_group_reference_list.#.kind` - (Optional) The kind name. Default value is `user_group`
-        * `external_user_group_reference_list.#.uuid` - (Required) The UUID of a user_group
-        * `external_user_group_reference_list.#.name` - (Optional/Computed) The name of a user_group
-        """
         return pulumi.get(self, "external_user_group_reference_lists")
 
     @external_user_group_reference_lists.setter
     def external_user_group_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectExternalUserGroupReferenceListArgs']]]]):
         pulumi.set(self, "external_user_group_reference_lists", value)
 
     @property
@@ -515,20 +606,14 @@
     @project_reference.setter
     def project_reference(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "project_reference", value)
 
     @property
     @pulumi.getter(name="resourceDomain")
     def resource_domain(self) -> Optional[pulumi.Input['ProjectResourceDomainArgs']]:
-        """
-        The status for a resource domain (limits and values)
-        * `resource_domain.resources` - (Required) Array of the utilization/limit for resource types
-        * `resource_domain.resources.#.limit` - (Required) The resource consumption limit (unspecified is unlimited)
-        * `resource_domain.resources.#.resource_type` - (Required) The type of resource (for example storage, CPUs)
-        """
         return pulumi.get(self, "resource_domain")
 
     @resource_domain.setter
     def resource_domain(self, value: Optional[pulumi.Input['ProjectResourceDomainArgs']]):
         pulumi.set(self, "resource_domain", value)
 
     @property
@@ -539,61 +624,110 @@
     @state.setter
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter(name="subnetReferenceLists")
     def subnet_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectSubnetReferenceListArgs']]]]:
-        """
-        List of subnets for the project.
-        * `subnet_reference_list.#.kind` - (Optional) The kind name. Default value is `subnet`
-        * `subnet_reference_list.#.uuid` - (Required) The UUID of a subnet
-        * `subnet_reference_list.#.name` - (Optional/Computed) The name of a subnet.
-        """
         return pulumi.get(self, "subnet_reference_lists")
 
     @subnet_reference_lists.setter
     def subnet_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectSubnetReferenceListArgs']]]]):
         pulumi.set(self, "subnet_reference_lists", value)
 
     @property
+    @pulumi.getter(name="tunnelReferenceLists")
+    def tunnel_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTunnelReferenceListArgs']]]]:
+        return pulumi.get(self, "tunnel_reference_lists")
+
+    @tunnel_reference_lists.setter
+    def tunnel_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTunnelReferenceListArgs']]]]):
+        pulumi.set(self, "tunnel_reference_lists", value)
+
+    @property
+    @pulumi.getter(name="useProjectInternal")
+    def use_project_internal(self) -> Optional[pulumi.Input[bool]]:
+        """
+        flag to use project internal for user role mapping
+        """
+        return pulumi.get(self, "use_project_internal")
+
+    @use_project_internal.setter
+    def use_project_internal(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "use_project_internal", value)
+
+    @property
+    @pulumi.getter(name="userGroupLists")
+    def user_group_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserGroupListArgs']]]]:
+        return pulumi.get(self, "user_group_lists")
+
+    @user_group_lists.setter
+    def user_group_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserGroupListArgs']]]]):
+        pulumi.set(self, "user_group_lists", value)
+
+    @property
+    @pulumi.getter(name="userLists")
+    def user_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserListArgs']]]]:
+        return pulumi.get(self, "user_lists")
+
+    @user_lists.setter
+    def user_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserListArgs']]]]):
+        pulumi.set(self, "user_lists", value)
+
+    @property
     @pulumi.getter(name="userReferenceLists")
     def user_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserReferenceListArgs']]]]:
         """
-        List of users in the project.
-        * `user_reference_list.#.kind` - (Optional) The kind name. Default value is `user`
-        * `user_reference_list.#.uuid` - (Required) The UUID of a user
-        * `user_reference_list.#.name` - (Optional/Computed) The name of a user.
+        List of Reference of users.
         """
         return pulumi.get(self, "user_reference_lists")
 
     @user_reference_lists.setter
     def user_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectUserReferenceListArgs']]]]):
         pulumi.set(self, "user_reference_lists", value)
 
+    @property
+    @pulumi.getter(name="vpcReferenceLists")
+    def vpc_reference_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectVpcReferenceListArgs']]]]:
+        return pulumi.get(self, "vpc_reference_lists")
+
+    @vpc_reference_lists.setter
+    def vpc_reference_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectVpcReferenceListArgs']]]]):
+        pulumi.set(self, "vpc_reference_lists", value)
+
 
 class Project(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  account_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectAccountReferenceListArgs']]]]] = None,
+                 acps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectAcpArgs']]]]] = None,
                  api_version: Optional[pulumi.Input[str]] = None,
                  categories: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectCategoryArgs']]]]] = None,
+                 cluster_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectClusterReferenceListArgs']]]]] = None,
+                 cluster_uuid: Optional[pulumi.Input[str]] = None,
+                 default_environment_reference: Optional[pulumi.Input[pulumi.InputType['ProjectDefaultEnvironmentReferenceArgs']]] = None,
                  default_subnet_reference: Optional[pulumi.Input[pulumi.InputType['ProjectDefaultSubnetReferenceArgs']]] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 enable_collab: Optional[pulumi.Input[bool]] = None,
                  environment_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectEnvironmentReferenceListArgs']]]]] = None,
                  external_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectExternalNetworkListArgs']]]]] = None,
                  external_user_group_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectExternalUserGroupReferenceListArgs']]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  owner_reference: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  project_reference: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  resource_domain: Optional[pulumi.Input[pulumi.InputType['ProjectResourceDomainArgs']]] = None,
                  subnet_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectSubnetReferenceListArgs']]]]] = None,
+                 tunnel_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTunnelReferenceListArgs']]]]] = None,
+                 use_project_internal: Optional[pulumi.Input[bool]] = None,
+                 user_group_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectUserGroupListArgs']]]]] = None,
+                 user_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectUserListArgs']]]]] = None,
                  user_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectUserReferenceListArgs']]]]] = None,
+                 vpc_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectVpcReferenceListArgs']]]]] = None,
                  __props__=None):
         """
         Provides a Nutanix Project resource to Create a Project.
 
         ## Example Usage
 
         ```python
@@ -617,15 +751,15 @@
                 "8.8.8.8",
                 "4.2.2.2",
             ],
             dhcp_domain_search_lists=[
                 "terraform.nutanix.com",
                 "terraform.unit.test.com",
             ])
-        project_test = nutanix.Project("projectTest",
+        project_test_project = nutanix.Project("projectTestProject",
             description="This is my project",
             categories=[nutanix.ProjectCategoryArgs(
                 name="Environment",
                 value="Staging",
             )],
             resource_domain=nutanix.ProjectResourceDomainArgs(
                 resources=[nutanix.ProjectResourceDomainResourceArgs(
@@ -633,51 +767,100 @@
                     resource_type="STORAGE",
                 )],
             ),
             default_subnet_reference=nutanix.ProjectDefaultSubnetReferenceArgs(
                 uuid=subnet.metadata["uuid"],
             ),
             api_version="3.1")
+        # set use_project_internal flag to create project with acps
+        project_test_index_project_project = nutanix.Project("projectTestIndex/projectProject",
+            description="This is my project",
+            cluster_uuid="<YOUR_CLUSTER_ID>",
+            use_project_internal=True,
+            default_subnet_reference=nutanix.ProjectDefaultSubnetReferenceArgs(
+                uuid=subnet.metadata["uuid"],
+            ),
+            user_reference_lists=[nutanix.ProjectUserReferenceListArgs(
+                name="{{user_name}}",
+                kind="user",
+                uuid="{{user_uuid}}",
+            )],
+            subnet_reference_lists=[nutanix.ProjectSubnetReferenceListArgs(
+                uuid=resource["nutanix_subnet"]["sub"]["id"],
+            )],
+            acps=[nutanix.ProjectAcpArgs(
+                name="{{acp_name}}",
+                role_reference=nutanix.ProjectAcpRoleReferenceArgs(
+                    kind="role",
+                    uuid="{{role_uuid}}",
+                    name="Developer",
+                ),
+                user_reference_lists=[nutanix.ProjectAcpUserReferenceListArgs(
+                    name="{{user_name}}",
+                    kind="user",
+                    uuid="{{user_uuid}}",
+                )],
+                description="{{description}}",
+            )],
+            api_version="3.1")
+        ## Create a project with user which not added in the PC
+        project_test_nutanix_index_project_project = nutanix.Project("projectTestNutanixIndex/projectProject",
+            description="This is my project",
+            cluster_uuid="<YOUR_CLUSTER_ID>",
+            use_project_internal=True,
+            default_subnet_reference=nutanix.ProjectDefaultSubnetReferenceArgs(
+                uuid=subnet.metadata["uuid"],
+            ),
+            user_reference_lists=[nutanix.ProjectUserReferenceListArgs(
+                name="{{user_name}}",
+                kind="user",
+                uuid="{{user_uuid}}",
+            )],
+            subnet_reference_lists=[nutanix.ProjectSubnetReferenceListArgs(
+                uuid=resource["nutanix_subnet"]["sub"]["id"],
+            )],
+            acps=[nutanix.ProjectAcpArgs(
+                name="{{acp_name}}",
+                role_reference=nutanix.ProjectAcpRoleReferenceArgs(
+                    kind="role",
+                    uuid="{{role_uuid}}",
+                    name="Developer",
+                ),
+                user_reference_lists=[nutanix.ProjectAcpUserReferenceListArgs(
+                    name="{{user_name}}",
+                    kind="user",
+                    uuid="{{user_uuid}}",
+                )],
+                description="{{description}}",
+            )],
+            user_lists=[nutanix.ProjectUserListArgs(
+                metadata={
+                    "kind": "user",
+                    "uuid": "{{ UUID of the USER }}",
+                },
+                directory_service_user=nutanix.ProjectUserListDirectoryServiceUserArgs(
+                    user_principal_name="{{ Name of user }}",
+                    directory_service_reference=nutanix.ProjectUserListDirectoryServiceUserDirectoryServiceReferenceArgs(
+                        uuid="{{ DIRECTORY SERVICE UUID }}",
+                        kind="directory_service",
+                    ),
+                ),
+            )],
+            api_version="3.1")
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectAccountReferenceListArgs']]]] account_reference_lists: List of accounts associated with the project.
-               * `account_reference_list.#.kind` - (Optional) The kind name. Default value is `account`
-               * `account_reference_list.#.uuid` - (Required) The UUID of an account.
-               * `account_reference_list.#.name` - (Optional/Computed) The name of an account.
-        :param pulumi.Input[pulumi.InputType['ProjectDefaultSubnetReferenceArgs']] default_subnet_reference: Reference to a subnet.
-               * `default_subnet_reference.kind` - (Optional) The kind name. Default value is `subnet`
-               * `default_subnet_reference.uuid` - (Required) The UUID of a subnet.
-               * `default_subnet_reference.name` - (Optional/Computed) The name of a subnet.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectCategoryArgs']]]] categories: - (Optional) The category values represented as a dictionary of key > list of values.
+        :param pulumi.Input[str] cluster_uuid: The UUID of cluster. (Required when using project_internal flag).
         :param pulumi.Input[str] description: A description for project.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectEnvironmentReferenceListArgs']]]] environment_reference_lists: List of environments associated with the project.
-               * `environment_reference_list.#.kind` - (Optional) The kind name. Default value is `environment`
-               * `environment_reference_list.#.uuid` - (Required) The UUID of an environment.
-               * `environment_reference_list.#.name` - (Optional/Computed) The name of an environment.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectExternalNetworkListArgs']]]] external_network_lists: List of external networks associated with the project.
-               * `external_network_list.#.uuid` - (Required) The UUID of a network.
-               * `external_network_list.#.name` - (Optional/Computed) The name of a network.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectExternalUserGroupReferenceListArgs']]]] external_user_group_reference_lists: List of directory service user groups. These groups are not managed by Nutanix.
-               * `external_user_group_reference_list.#.kind` - (Optional) The kind name. Default value is `user_group`
-               * `external_user_group_reference_list.#.uuid` - (Required) The UUID of a user_group
-               * `external_user_group_reference_list.#.name` - (Optional/Computed) The name of a user_group
+        :param pulumi.Input[bool] enable_collab: flag to allow collaboration of projects. (Use with project_internal flag)
         :param pulumi.Input[str] name: The name for the project.
-        :param pulumi.Input[pulumi.InputType['ProjectResourceDomainArgs']] resource_domain: The status for a resource domain (limits and values)
-               * `resource_domain.resources` - (Required) Array of the utilization/limit for resource types
-               * `resource_domain.resources.#.limit` - (Required) The resource consumption limit (unspecified is unlimited)
-               * `resource_domain.resources.#.resource_type` - (Required) The type of resource (for example storage, CPUs)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectSubnetReferenceListArgs']]]] subnet_reference_lists: List of subnets for the project.
-               * `subnet_reference_list.#.kind` - (Optional) The kind name. Default value is `subnet`
-               * `subnet_reference_list.#.uuid` - (Required) The UUID of a subnet
-               * `subnet_reference_list.#.name` - (Optional/Computed) The name of a subnet.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectUserReferenceListArgs']]]] user_reference_lists: List of users in the project.
-               * `user_reference_list.#.kind` - (Optional) The kind name. Default value is `user`
-               * `user_reference_list.#.uuid` - (Required) The UUID of a user
-               * `user_reference_list.#.name` - (Optional/Computed) The name of a user.
+        :param pulumi.Input[bool] use_project_internal: flag to use project internal for user role mapping
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectUserReferenceListArgs']]]] user_reference_lists: List of Reference of users.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProjectArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -707,15 +890,15 @@
                 "8.8.8.8",
                 "4.2.2.2",
             ],
             dhcp_domain_search_lists=[
                 "terraform.nutanix.com",
                 "terraform.unit.test.com",
             ])
-        project_test = nutanix.Project("projectTest",
+        project_test_project = nutanix.Project("projectTestProject",
             description="This is my project",
             categories=[nutanix.ProjectCategoryArgs(
                 name="Environment",
                 value="Staging",
             )],
             resource_domain=nutanix.ProjectResourceDomainArgs(
                 resources=[nutanix.ProjectResourceDomainResourceArgs(
@@ -723,14 +906,89 @@
                     resource_type="STORAGE",
                 )],
             ),
             default_subnet_reference=nutanix.ProjectDefaultSubnetReferenceArgs(
                 uuid=subnet.metadata["uuid"],
             ),
             api_version="3.1")
+        # set use_project_internal flag to create project with acps
+        project_test_index_project_project = nutanix.Project("projectTestIndex/projectProject",
+            description="This is my project",
+            cluster_uuid="<YOUR_CLUSTER_ID>",
+            use_project_internal=True,
+            default_subnet_reference=nutanix.ProjectDefaultSubnetReferenceArgs(
+                uuid=subnet.metadata["uuid"],
+            ),
+            user_reference_lists=[nutanix.ProjectUserReferenceListArgs(
+                name="{{user_name}}",
+                kind="user",
+                uuid="{{user_uuid}}",
+            )],
+            subnet_reference_lists=[nutanix.ProjectSubnetReferenceListArgs(
+                uuid=resource["nutanix_subnet"]["sub"]["id"],
+            )],
+            acps=[nutanix.ProjectAcpArgs(
+                name="{{acp_name}}",
+                role_reference=nutanix.ProjectAcpRoleReferenceArgs(
+                    kind="role",
+                    uuid="{{role_uuid}}",
+                    name="Developer",
+                ),
+                user_reference_lists=[nutanix.ProjectAcpUserReferenceListArgs(
+                    name="{{user_name}}",
+                    kind="user",
+                    uuid="{{user_uuid}}",
+                )],
+                description="{{description}}",
+            )],
+            api_version="3.1")
+        ## Create a project with user which not added in the PC
+        project_test_nutanix_index_project_project = nutanix.Project("projectTestNutanixIndex/projectProject",
+            description="This is my project",
+            cluster_uuid="<YOUR_CLUSTER_ID>",
+            use_project_internal=True,
+            default_subnet_reference=nutanix.ProjectDefaultSubnetReferenceArgs(
+                uuid=subnet.metadata["uuid"],
+            ),
+            user_reference_lists=[nutanix.ProjectUserReferenceListArgs(
+                name="{{user_name}}",
+                kind="user",
+                uuid="{{user_uuid}}",
+            )],
+            subnet_reference_lists=[nutanix.ProjectSubnetReferenceListArgs(
+                uuid=resource["nutanix_subnet"]["sub"]["id"],
+            )],
+            acps=[nutanix.ProjectAcpArgs(
+                name="{{acp_name}}",
+                role_reference=nutanix.ProjectAcpRoleReferenceArgs(
+                    kind="role",
+                    uuid="{{role_uuid}}",
+                    name="Developer",
+                ),
+                user_reference_lists=[nutanix.ProjectAcpUserReferenceListArgs(
+                    name="{{user_name}}",
+                    kind="user",
+                    uuid="{{user_uuid}}",
+                )],
+                description="{{description}}",
+            )],
+            user_lists=[nutanix.ProjectUserListArgs(
+                metadata={
+                    "kind": "user",
+                    "uuid": "{{ UUID of the USER }}",
+                },
+                directory_service_user=nutanix.ProjectUserListDirectoryServiceUserArgs(
+                    user_principal_name="{{ Name of user }}",
+                    directory_service_reference=nutanix.ProjectUserListDirectoryServiceUserDirectoryServiceReferenceArgs(
+                        uuid="{{ DIRECTORY SERVICE UUID }}",
+                        kind="directory_service",
+                    ),
+                ),
+            )],
+            api_version="3.1")
         ```
 
         :param str resource_name: The name of the resource.
         :param ProjectArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -741,218 +999,237 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  account_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectAccountReferenceListArgs']]]]] = None,
+                 acps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectAcpArgs']]]]] = None,
                  api_version: Optional[pulumi.Input[str]] = None,
                  categories: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectCategoryArgs']]]]] = None,
+                 cluster_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectClusterReferenceListArgs']]]]] = None,
+                 cluster_uuid: Optional[pulumi.Input[str]] = None,
+                 default_environment_reference: Optional[pulumi.Input[pulumi.InputType['ProjectDefaultEnvironmentReferenceArgs']]] = None,
                  default_subnet_reference: Optional[pulumi.Input[pulumi.InputType['ProjectDefaultSubnetReferenceArgs']]] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 enable_collab: Optional[pulumi.Input[bool]] = None,
                  environment_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectEnvironmentReferenceListArgs']]]]] = None,
                  external_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectExternalNetworkListArgs']]]]] = None,
                  external_user_group_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectExternalUserGroupReferenceListArgs']]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  owner_reference: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  project_reference: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  resource_domain: Optional[pulumi.Input[pulumi.InputType['ProjectResourceDomainArgs']]] = None,
                  subnet_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectSubnetReferenceListArgs']]]]] = None,
+                 tunnel_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTunnelReferenceListArgs']]]]] = None,
+                 use_project_internal: Optional[pulumi.Input[bool]] = None,
+                 user_group_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectUserGroupListArgs']]]]] = None,
+                 user_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectUserListArgs']]]]] = None,
                  user_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectUserReferenceListArgs']]]]] = None,
+                 vpc_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectVpcReferenceListArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProjectArgs.__new__(ProjectArgs)
 
             __props__.__dict__["account_reference_lists"] = account_reference_lists
+            __props__.__dict__["acps"] = acps
             __props__.__dict__["api_version"] = api_version
             __props__.__dict__["categories"] = categories
+            __props__.__dict__["cluster_reference_lists"] = cluster_reference_lists
+            __props__.__dict__["cluster_uuid"] = cluster_uuid
+            __props__.__dict__["default_environment_reference"] = default_environment_reference
             if default_subnet_reference is None and not opts.urn:
                 raise TypeError("Missing required property 'default_subnet_reference'")
             __props__.__dict__["default_subnet_reference"] = default_subnet_reference
             if description is None and not opts.urn:
                 raise TypeError("Missing required property 'description'")
             __props__.__dict__["description"] = description
+            __props__.__dict__["enable_collab"] = enable_collab
             __props__.__dict__["environment_reference_lists"] = environment_reference_lists
             __props__.__dict__["external_network_lists"] = external_network_lists
             __props__.__dict__["external_user_group_reference_lists"] = external_user_group_reference_lists
             __props__.__dict__["name"] = name
             __props__.__dict__["owner_reference"] = owner_reference
             __props__.__dict__["project_reference"] = project_reference
             __props__.__dict__["resource_domain"] = resource_domain
             __props__.__dict__["subnet_reference_lists"] = subnet_reference_lists
+            __props__.__dict__["tunnel_reference_lists"] = tunnel_reference_lists
+            __props__.__dict__["use_project_internal"] = use_project_internal
+            __props__.__dict__["user_group_lists"] = user_group_lists
+            __props__.__dict__["user_lists"] = user_lists
             __props__.__dict__["user_reference_lists"] = user_reference_lists
+            __props__.__dict__["vpc_reference_lists"] = vpc_reference_lists
             __props__.__dict__["is_default"] = None
             __props__.__dict__["metadata"] = None
             __props__.__dict__["state"] = None
         super(Project, __self__).__init__(
             'nutanix:index/project:Project',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             account_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectAccountReferenceListArgs']]]]] = None,
+            acps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectAcpArgs']]]]] = None,
             api_version: Optional[pulumi.Input[str]] = None,
             categories: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectCategoryArgs']]]]] = None,
+            cluster_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectClusterReferenceListArgs']]]]] = None,
+            cluster_uuid: Optional[pulumi.Input[str]] = None,
+            default_environment_reference: Optional[pulumi.Input[pulumi.InputType['ProjectDefaultEnvironmentReferenceArgs']]] = None,
             default_subnet_reference: Optional[pulumi.Input[pulumi.InputType['ProjectDefaultSubnetReferenceArgs']]] = None,
             description: Optional[pulumi.Input[str]] = None,
+            enable_collab: Optional[pulumi.Input[bool]] = None,
             environment_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectEnvironmentReferenceListArgs']]]]] = None,
             external_network_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectExternalNetworkListArgs']]]]] = None,
             external_user_group_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectExternalUserGroupReferenceListArgs']]]]] = None,
             is_default: Optional[pulumi.Input[bool]] = None,
             metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             owner_reference: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             project_reference: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             resource_domain: Optional[pulumi.Input[pulumi.InputType['ProjectResourceDomainArgs']]] = None,
             state: Optional[pulumi.Input[str]] = None,
             subnet_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectSubnetReferenceListArgs']]]]] = None,
-            user_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectUserReferenceListArgs']]]]] = None) -> 'Project':
+            tunnel_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTunnelReferenceListArgs']]]]] = None,
+            use_project_internal: Optional[pulumi.Input[bool]] = None,
+            user_group_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectUserGroupListArgs']]]]] = None,
+            user_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectUserListArgs']]]]] = None,
+            user_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectUserReferenceListArgs']]]]] = None,
+            vpc_reference_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectVpcReferenceListArgs']]]]] = None) -> 'Project':
         """
         Get an existing Project resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectAccountReferenceListArgs']]]] account_reference_lists: List of accounts associated with the project.
-               * `account_reference_list.#.kind` - (Optional) The kind name. Default value is `account`
-               * `account_reference_list.#.uuid` - (Required) The UUID of an account.
-               * `account_reference_list.#.name` - (Optional/Computed) The name of an account.
-        :param pulumi.Input[pulumi.InputType['ProjectDefaultSubnetReferenceArgs']] default_subnet_reference: Reference to a subnet.
-               * `default_subnet_reference.kind` - (Optional) The kind name. Default value is `subnet`
-               * `default_subnet_reference.uuid` - (Required) The UUID of a subnet.
-               * `default_subnet_reference.name` - (Optional/Computed) The name of a subnet.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectCategoryArgs']]]] categories: - (Optional) The category values represented as a dictionary of key > list of values.
+        :param pulumi.Input[str] cluster_uuid: The UUID of cluster. (Required when using project_internal flag).
         :param pulumi.Input[str] description: A description for project.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectEnvironmentReferenceListArgs']]]] environment_reference_lists: List of environments associated with the project.
-               * `environment_reference_list.#.kind` - (Optional) The kind name. Default value is `environment`
-               * `environment_reference_list.#.uuid` - (Required) The UUID of an environment.
-               * `environment_reference_list.#.name` - (Optional/Computed) The name of an environment.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectExternalNetworkListArgs']]]] external_network_lists: List of external networks associated with the project.
-               * `external_network_list.#.uuid` - (Required) The UUID of a network.
-               * `external_network_list.#.name` - (Optional/Computed) The name of a network.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectExternalUserGroupReferenceListArgs']]]] external_user_group_reference_lists: List of directory service user groups. These groups are not managed by Nutanix.
-               * `external_user_group_reference_list.#.kind` - (Optional) The kind name. Default value is `user_group`
-               * `external_user_group_reference_list.#.uuid` - (Required) The UUID of a user_group
-               * `external_user_group_reference_list.#.name` - (Optional/Computed) The name of a user_group
+        :param pulumi.Input[bool] enable_collab: flag to allow collaboration of projects. (Use with project_internal flag)
         :param pulumi.Input[str] name: The name for the project.
-        :param pulumi.Input[pulumi.InputType['ProjectResourceDomainArgs']] resource_domain: The status for a resource domain (limits and values)
-               * `resource_domain.resources` - (Required) Array of the utilization/limit for resource types
-               * `resource_domain.resources.#.limit` - (Required) The resource consumption limit (unspecified is unlimited)
-               * `resource_domain.resources.#.resource_type` - (Required) The type of resource (for example storage, CPUs)
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectSubnetReferenceListArgs']]]] subnet_reference_lists: List of subnets for the project.
-               * `subnet_reference_list.#.kind` - (Optional) The kind name. Default value is `subnet`
-               * `subnet_reference_list.#.uuid` - (Required) The UUID of a subnet
-               * `subnet_reference_list.#.name` - (Optional/Computed) The name of a subnet.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectUserReferenceListArgs']]]] user_reference_lists: List of users in the project.
-               * `user_reference_list.#.kind` - (Optional) The kind name. Default value is `user`
-               * `user_reference_list.#.uuid` - (Required) The UUID of a user
-               * `user_reference_list.#.name` - (Optional/Computed) The name of a user.
+        :param pulumi.Input[bool] use_project_internal: flag to use project internal for user role mapping
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectUserReferenceListArgs']]]] user_reference_lists: List of Reference of users.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ProjectState.__new__(_ProjectState)
 
         __props__.__dict__["account_reference_lists"] = account_reference_lists
+        __props__.__dict__["acps"] = acps
         __props__.__dict__["api_version"] = api_version
         __props__.__dict__["categories"] = categories
+        __props__.__dict__["cluster_reference_lists"] = cluster_reference_lists
+        __props__.__dict__["cluster_uuid"] = cluster_uuid
+        __props__.__dict__["default_environment_reference"] = default_environment_reference
         __props__.__dict__["default_subnet_reference"] = default_subnet_reference
         __props__.__dict__["description"] = description
+        __props__.__dict__["enable_collab"] = enable_collab
         __props__.__dict__["environment_reference_lists"] = environment_reference_lists
         __props__.__dict__["external_network_lists"] = external_network_lists
         __props__.__dict__["external_user_group_reference_lists"] = external_user_group_reference_lists
         __props__.__dict__["is_default"] = is_default
         __props__.__dict__["metadata"] = metadata
         __props__.__dict__["name"] = name
         __props__.__dict__["owner_reference"] = owner_reference
         __props__.__dict__["project_reference"] = project_reference
         __props__.__dict__["resource_domain"] = resource_domain
         __props__.__dict__["state"] = state
         __props__.__dict__["subnet_reference_lists"] = subnet_reference_lists
+        __props__.__dict__["tunnel_reference_lists"] = tunnel_reference_lists
+        __props__.__dict__["use_project_internal"] = use_project_internal
+        __props__.__dict__["user_group_lists"] = user_group_lists
+        __props__.__dict__["user_lists"] = user_lists
         __props__.__dict__["user_reference_lists"] = user_reference_lists
+        __props__.__dict__["vpc_reference_lists"] = vpc_reference_lists
         return Project(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="accountReferenceLists")
     def account_reference_lists(self) -> pulumi.Output[Sequence['outputs.ProjectAccountReferenceList']]:
-        """
-        List of accounts associated with the project.
-        * `account_reference_list.#.kind` - (Optional) The kind name. Default value is `account`
-        * `account_reference_list.#.uuid` - (Required) The UUID of an account.
-        * `account_reference_list.#.name` - (Optional/Computed) The name of an account.
-        """
         return pulumi.get(self, "account_reference_lists")
 
     @property
+    @pulumi.getter
+    def acps(self) -> pulumi.Output[Optional[Sequence['outputs.ProjectAcp']]]:
+        return pulumi.get(self, "acps")
+
+    @property
     @pulumi.getter(name="apiVersion")
     def api_version(self) -> pulumi.Output[str]:
         return pulumi.get(self, "api_version")
 
     @property
     @pulumi.getter
     def categories(self) -> pulumi.Output[Sequence['outputs.ProjectCategory']]:
+        """
+        - (Optional) The category values represented as a dictionary of key > list of values.
+        """
         return pulumi.get(self, "categories")
 
     @property
-    @pulumi.getter(name="defaultSubnetReference")
-    def default_subnet_reference(self) -> pulumi.Output['outputs.ProjectDefaultSubnetReference']:
+    @pulumi.getter(name="clusterReferenceLists")
+    def cluster_reference_lists(self) -> pulumi.Output[Sequence['outputs.ProjectClusterReferenceList']]:
+        return pulumi.get(self, "cluster_reference_lists")
+
+    @property
+    @pulumi.getter(name="clusterUuid")
+    def cluster_uuid(self) -> pulumi.Output[Optional[str]]:
         """
-        Reference to a subnet.
-        * `default_subnet_reference.kind` - (Optional) The kind name. Default value is `subnet`
-        * `default_subnet_reference.uuid` - (Required) The UUID of a subnet.
-        * `default_subnet_reference.name` - (Optional/Computed) The name of a subnet.
+        The UUID of cluster. (Required when using project_internal flag).
         """
+        return pulumi.get(self, "cluster_uuid")
+
+    @property
+    @pulumi.getter(name="defaultEnvironmentReference")
+    def default_environment_reference(self) -> pulumi.Output['outputs.ProjectDefaultEnvironmentReference']:
+        return pulumi.get(self, "default_environment_reference")
+
+    @property
+    @pulumi.getter(name="defaultSubnetReference")
+    def default_subnet_reference(self) -> pulumi.Output['outputs.ProjectDefaultSubnetReference']:
         return pulumi.get(self, "default_subnet_reference")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[str]:
         """
         A description for project.
         """
         return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="environmentReferenceLists")
-    def environment_reference_lists(self) -> pulumi.Output[Sequence['outputs.ProjectEnvironmentReferenceList']]:
+    @pulumi.getter(name="enableCollab")
+    def enable_collab(self) -> pulumi.Output[Optional[bool]]:
         """
-        List of environments associated with the project.
-        * `environment_reference_list.#.kind` - (Optional) The kind name. Default value is `environment`
-        * `environment_reference_list.#.uuid` - (Required) The UUID of an environment.
-        * `environment_reference_list.#.name` - (Optional/Computed) The name of an environment.
+        flag to allow collaboration of projects. (Use with project_internal flag)
         """
+        return pulumi.get(self, "enable_collab")
+
+    @property
+    @pulumi.getter(name="environmentReferenceLists")
+    def environment_reference_lists(self) -> pulumi.Output[Sequence['outputs.ProjectEnvironmentReferenceList']]:
         return pulumi.get(self, "environment_reference_lists")
 
     @property
     @pulumi.getter(name="externalNetworkLists")
     def external_network_lists(self) -> pulumi.Output[Sequence['outputs.ProjectExternalNetworkList']]:
-        """
-        List of external networks associated with the project.
-        * `external_network_list.#.uuid` - (Required) The UUID of a network.
-        * `external_network_list.#.name` - (Optional/Computed) The name of a network.
-        """
         return pulumi.get(self, "external_network_lists")
 
     @property
     @pulumi.getter(name="externalUserGroupReferenceLists")
     def external_user_group_reference_lists(self) -> pulumi.Output[Sequence['outputs.ProjectExternalUserGroupReferenceList']]:
-        """
-        List of directory service user groups. These groups are not managed by Nutanix.
-        * `external_user_group_reference_list.#.kind` - (Optional) The kind name. Default value is `user_group`
-        * `external_user_group_reference_list.#.uuid` - (Required) The UUID of a user_group
-        * `external_user_group_reference_list.#.name` - (Optional/Computed) The name of a user_group
-        """
         return pulumi.get(self, "external_user_group_reference_lists")
 
     @property
     @pulumi.getter(name="isDefault")
     def is_default(self) -> pulumi.Output[bool]:
         return pulumi.get(self, "is_default")
 
@@ -978,42 +1255,55 @@
     @pulumi.getter(name="projectReference")
     def project_reference(self) -> pulumi.Output[Mapping[str, str]]:
         return pulumi.get(self, "project_reference")
 
     @property
     @pulumi.getter(name="resourceDomain")
     def resource_domain(self) -> pulumi.Output[Optional['outputs.ProjectResourceDomain']]:
-        """
-        The status for a resource domain (limits and values)
-        * `resource_domain.resources` - (Required) Array of the utilization/limit for resource types
-        * `resource_domain.resources.#.limit` - (Required) The resource consumption limit (unspecified is unlimited)
-        * `resource_domain.resources.#.resource_type` - (Required) The type of resource (for example storage, CPUs)
-        """
         return pulumi.get(self, "resource_domain")
 
     @property
     @pulumi.getter
     def state(self) -> pulumi.Output[str]:
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter(name="subnetReferenceLists")
     def subnet_reference_lists(self) -> pulumi.Output[Sequence['outputs.ProjectSubnetReferenceList']]:
+        return pulumi.get(self, "subnet_reference_lists")
+
+    @property
+    @pulumi.getter(name="tunnelReferenceLists")
+    def tunnel_reference_lists(self) -> pulumi.Output[Sequence['outputs.ProjectTunnelReferenceList']]:
+        return pulumi.get(self, "tunnel_reference_lists")
+
+    @property
+    @pulumi.getter(name="useProjectInternal")
+    def use_project_internal(self) -> pulumi.Output[Optional[bool]]:
         """
-        List of subnets for the project.
-        * `subnet_reference_list.#.kind` - (Optional) The kind name. Default value is `subnet`
-        * `subnet_reference_list.#.uuid` - (Required) The UUID of a subnet
-        * `subnet_reference_list.#.name` - (Optional/Computed) The name of a subnet.
+        flag to use project internal for user role mapping
         """
-        return pulumi.get(self, "subnet_reference_lists")
+        return pulumi.get(self, "use_project_internal")
+
+    @property
+    @pulumi.getter(name="userGroupLists")
+    def user_group_lists(self) -> pulumi.Output[Optional[Sequence['outputs.ProjectUserGroupList']]]:
+        return pulumi.get(self, "user_group_lists")
+
+    @property
+    @pulumi.getter(name="userLists")
+    def user_lists(self) -> pulumi.Output[Optional[Sequence['outputs.ProjectUserList']]]:
+        return pulumi.get(self, "user_lists")
 
     @property
     @pulumi.getter(name="userReferenceLists")
     def user_reference_lists(self) -> pulumi.Output[Sequence['outputs.ProjectUserReferenceList']]:
         """
-        List of users in the project.
-        * `user_reference_list.#.kind` - (Optional) The kind name. Default value is `user`
-        * `user_reference_list.#.uuid` - (Required) The UUID of a user
-        * `user_reference_list.#.name` - (Optional/Computed) The name of a user.
+        List of Reference of users.
         """
         return pulumi.get(self, "user_reference_lists")
 
+    @property
+    @pulumi.getter(name="vpcReferenceLists")
+    def vpc_reference_lists(self) -> pulumi.Output[Sequence['outputs.ProjectVpcReferenceList']]:
+        return pulumi.get(self, "vpc_reference_lists")
+
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/provider.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,42 +14,52 @@
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  foundation_endpoint: Optional[pulumi.Input[str]] = None,
                  foundation_port: Optional[pulumi.Input[str]] = None,
                  insecure: Optional[pulumi.Input[bool]] = None,
+                 ndb_endpoint: Optional[pulumi.Input[str]] = None,
+                 ndb_password: Optional[pulumi.Input[str]] = None,
+                 ndb_username: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[str]] = None,
                  proxy_url: Optional[pulumi.Input[str]] = None,
                  session_auth: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  wait_timeout: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a Provider resource.
         :param pulumi.Input[str] endpoint: URL for Nutanix Prism (e.g IP or FQDN for cluster VIP note, this is never the data services VIP, and should not be an
                individual CVM address, as this would cause calls to fail during cluster lifecycle management operations, such as AOS
                upgrades.
         :param pulumi.Input[str] foundation_endpoint: endpoint for foundation VM (eg. Foundation VM IP)
         :param pulumi.Input[str] foundation_port: Port for foundation VM
         :param pulumi.Input[bool] insecure: Explicitly allow the provider to perform "insecure" SSL requests. If omitted,default value is `false`
+        :param pulumi.Input[str] ndb_endpoint: endpoint for Era VM (era ip)
         :param pulumi.Input[str] password: Password for provided user name.
         :param pulumi.Input[str] port: Port for Nutanix Prism.
         :param pulumi.Input[bool] session_auth: Use session authentification instead of basic auth for each request
         :param pulumi.Input[str] username: User name for Nutanix Prism. Could be local cluster auth (e.g. 'admin') or directory auth.
         :param pulumi.Input[int] wait_timeout: Set if you know that the creation o update of a resource may take long time (minutes)
         """
         if endpoint is not None:
             pulumi.set(__self__, "endpoint", endpoint)
         if foundation_endpoint is not None:
             pulumi.set(__self__, "foundation_endpoint", foundation_endpoint)
         if foundation_port is not None:
             pulumi.set(__self__, "foundation_port", foundation_port)
         if insecure is not None:
             pulumi.set(__self__, "insecure", insecure)
+        if ndb_endpoint is not None:
+            pulumi.set(__self__, "ndb_endpoint", ndb_endpoint)
+        if ndb_password is not None:
+            pulumi.set(__self__, "ndb_password", ndb_password)
+        if ndb_username is not None:
+            pulumi.set(__self__, "ndb_username", ndb_username)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if proxy_url is not None:
             pulumi.set(__self__, "proxy_url", proxy_url)
         if session_auth is not None:
@@ -106,14 +116,44 @@
         return pulumi.get(self, "insecure")
 
     @insecure.setter
     def insecure(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "insecure", value)
 
     @property
+    @pulumi.getter(name="ndbEndpoint")
+    def ndb_endpoint(self) -> Optional[pulumi.Input[str]]:
+        """
+        endpoint for Era VM (era ip)
+        """
+        return pulumi.get(self, "ndb_endpoint")
+
+    @ndb_endpoint.setter
+    def ndb_endpoint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ndb_endpoint", value)
+
+    @property
+    @pulumi.getter(name="ndbPassword")
+    def ndb_password(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "ndb_password")
+
+    @ndb_password.setter
+    def ndb_password(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ndb_password", value)
+
+    @property
+    @pulumi.getter(name="ndbUsername")
+    def ndb_username(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "ndb_username")
+
+    @ndb_username.setter
+    def ndb_username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ndb_username", value)
+
+    @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
         Password for provided user name.
         """
         return pulumi.get(self, "password")
 
@@ -184,14 +224,17 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  foundation_endpoint: Optional[pulumi.Input[str]] = None,
                  foundation_port: Optional[pulumi.Input[str]] = None,
                  insecure: Optional[pulumi.Input[bool]] = None,
+                 ndb_endpoint: Optional[pulumi.Input[str]] = None,
+                 ndb_password: Optional[pulumi.Input[str]] = None,
+                 ndb_username: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[str]] = None,
                  proxy_url: Optional[pulumi.Input[str]] = None,
                  session_auth: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  wait_timeout: Optional[pulumi.Input[int]] = None,
                  __props__=None):
@@ -205,14 +248,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] endpoint: URL for Nutanix Prism (e.g IP or FQDN for cluster VIP note, this is never the data services VIP, and should not be an
                individual CVM address, as this would cause calls to fail during cluster lifecycle management operations, such as AOS
                upgrades.
         :param pulumi.Input[str] foundation_endpoint: endpoint for foundation VM (eg. Foundation VM IP)
         :param pulumi.Input[str] foundation_port: Port for foundation VM
         :param pulumi.Input[bool] insecure: Explicitly allow the provider to perform "insecure" SSL requests. If omitted,default value is `false`
+        :param pulumi.Input[str] ndb_endpoint: endpoint for Era VM (era ip)
         :param pulumi.Input[str] password: Password for provided user name.
         :param pulumi.Input[str] port: Port for Nutanix Prism.
         :param pulumi.Input[bool] session_auth: Use session authentification instead of basic auth for each request
         :param pulumi.Input[str] username: User name for Nutanix Prism. Could be local cluster auth (e.g. 'admin') or directory auth.
         :param pulumi.Input[int] wait_timeout: Set if you know that the creation o update of a resource may take long time (minutes)
         """
         ...
@@ -242,14 +286,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  foundation_endpoint: Optional[pulumi.Input[str]] = None,
                  foundation_port: Optional[pulumi.Input[str]] = None,
                  insecure: Optional[pulumi.Input[bool]] = None,
+                 ndb_endpoint: Optional[pulumi.Input[str]] = None,
+                 ndb_password: Optional[pulumi.Input[str]] = None,
+                 ndb_username: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[str]] = None,
                  proxy_url: Optional[pulumi.Input[str]] = None,
                  session_auth: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  wait_timeout: Optional[pulumi.Input[int]] = None,
                  __props__=None):
@@ -261,14 +308,17 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
             __props__.__dict__["endpoint"] = endpoint
             __props__.__dict__["foundation_endpoint"] = foundation_endpoint
             __props__.__dict__["foundation_port"] = foundation_port
             __props__.__dict__["insecure"] = pulumi.Output.from_input(insecure).apply(pulumi.runtime.to_json) if insecure is not None else None
+            __props__.__dict__["ndb_endpoint"] = ndb_endpoint
+            __props__.__dict__["ndb_password"] = ndb_password
+            __props__.__dict__["ndb_username"] = ndb_username
             __props__.__dict__["password"] = password
             __props__.__dict__["port"] = port
             __props__.__dict__["proxy_url"] = proxy_url
             __props__.__dict__["session_auth"] = pulumi.Output.from_input(session_auth).apply(pulumi.runtime.to_json) if session_auth is not None else None
             __props__.__dict__["username"] = username
             __props__.__dict__["wait_timeout"] = pulumi.Output.from_input(wait_timeout).apply(pulumi.runtime.to_json) if wait_timeout is not None else None
         super(Provider, __self__).__init__(
@@ -300,14 +350,32 @@
     def foundation_port(self) -> pulumi.Output[Optional[str]]:
         """
         Port for foundation VM
         """
         return pulumi.get(self, "foundation_port")
 
     @property
+    @pulumi.getter(name="ndbEndpoint")
+    def ndb_endpoint(self) -> pulumi.Output[Optional[str]]:
+        """
+        endpoint for Era VM (era ip)
+        """
+        return pulumi.get(self, "ndb_endpoint")
+
+    @property
+    @pulumi.getter(name="ndbPassword")
+    def ndb_password(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "ndb_password")
+
+    @property
+    @pulumi.getter(name="ndbUsername")
+    def ndb_username(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "ndb_username")
+
+    @property
     @pulumi.getter
     def password(self) -> pulumi.Output[Optional[str]]:
         """
         Password for provided user name.
         """
         return pulumi.get(self, "password")
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/role.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/service_group.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/service_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/static_routes.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/static_routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
                  api_version: Optional[pulumi.Input[str]] = None,
                  default_route_nexthops: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['StaticRoutesDefaultRouteNexthopArgs']]]]] = None,
                  static_routes_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['StaticRoutesStaticRoutesListArgs']]]]] = None,
                  vpc_name: Optional[pulumi.Input[str]] = None,
                  vpc_uuid: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Provides Nutanix resource to create Floating IPs.
+        Provides Nutanix resource to create Static Routes within VPCs.
 
         ## create one static route for vpc uuid with external subnet
 
         ```python
         import pulumi
         import pulumi_nutanix as nutanix
 
@@ -263,15 +263,15 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[StaticRoutesArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Provides Nutanix resource to create Floating IPs.
+        Provides Nutanix resource to create Static Routes within VPCs.
 
         ## create one static route for vpc uuid with external subnet
 
         ```python
         import pulumi
         import pulumi_nutanix as nutanix
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/subnet.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/subnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,31 +37,36 @@
                  project_reference: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  subnet_ip: Optional[pulumi.Input[str]] = None,
                  vlan_id: Optional[pulumi.Input[int]] = None,
                  vpc_reference_uuid: Optional[pulumi.Input[str]] = None,
                  vswitch_name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Subnet resource.
-        :param pulumi.Input[str] subnet_type: - (Optional).
+        :param pulumi.Input[str] subnet_type: - (Optional). Valid Types are ["VLAN", "OVERLAY"]
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] availability_zone_reference: - (Optional) The reference to a availability_zone.
         :param pulumi.Input[Sequence[pulumi.Input['SubnetCategoryArgs']]] categories: - (Optional) The categories of the resource.
         :param pulumi.Input[str] cluster_uuid: - (Required) The UUID of the cluster.
         :param pulumi.Input[str] default_gateway_ip: - (Optional) Default gateway IP address.
         :param pulumi.Input[str] description: - (Optional) A description for subnet.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] dhcp_domain_search_lists: - (Optional).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dhcp_domain_name_server_lists: - (Optional). List of Domain Name Server addresses .
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dhcp_domain_search_lists: - (Optional).The DNS domain search list .
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] dhcp_options: - (Optional) Spec for defining DHCP options.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] dhcp_server_address: - (Optional) Host address.
         :param pulumi.Input[int] dhcp_server_address_port: - (Optional) Port Number.
+        :param pulumi.Input[bool] enable_nat: - (Optional) Whether NAT should be performed for VPCs attaching to the subnet. This field is supported only for external subnets. NAT is enabled by default on external subnets.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_config_pool_list_ranges: -(Optional) Range of IPs.
+        :param pulumi.Input[bool] is_external: - (Optional) Whether the subnet is external subnet or not.
         :param pulumi.Input[str] name: - (Optional) Subnet name (Readonly).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] network_function_chain_reference: - (Optional) The reference to a network_function_chain.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] owner_reference: - (Optional) The reference to a user.
         :param pulumi.Input[int] prefix_length: - (Optional).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] project_reference: - (Optional) The reference to a project.
         :param pulumi.Input[str] subnet_ip: - (Optional) Subnet IP address.
-        :param pulumi.Input[int] vlan_id: - (Optional).
+        :param pulumi.Input[int] vlan_id: - (Optional). For VLAN subnet.
+        :param pulumi.Input[str] vpc_reference_uuid: VPC reference uuid
         :param pulumi.Input[str] vswitch_name: - (Optional).
         """
         pulumi.set(__self__, "subnet_type", subnet_type)
         if availability_zone_reference is not None:
             pulumi.set(__self__, "availability_zone_reference", availability_zone_reference)
         if categories is not None:
             pulumi.set(__self__, "categories", categories)
@@ -106,15 +111,15 @@
         if vswitch_name is not None:
             pulumi.set(__self__, "vswitch_name", vswitch_name)
 
     @property
     @pulumi.getter(name="subnetType")
     def subnet_type(self) -> pulumi.Input[str]:
         """
-        - (Optional).
+        - (Optional). Valid Types are ["VLAN", "OVERLAY"]
         """
         return pulumi.get(self, "subnet_type")
 
     @subnet_type.setter
     def subnet_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "subnet_type", value)
 
@@ -177,25 +182,28 @@
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="dhcpDomainNameServerLists")
     def dhcp_domain_name_server_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        - (Optional). List of Domain Name Server addresses .
+        """
         return pulumi.get(self, "dhcp_domain_name_server_lists")
 
     @dhcp_domain_name_server_lists.setter
     def dhcp_domain_name_server_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "dhcp_domain_name_server_lists", value)
 
     @property
     @pulumi.getter(name="dhcpDomainSearchLists")
     def dhcp_domain_search_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        - (Optional).
+        - (Optional).The DNS domain search list .
         """
         return pulumi.get(self, "dhcp_domain_search_lists")
 
     @dhcp_domain_search_lists.setter
     def dhcp_domain_search_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "dhcp_domain_search_lists", value)
 
@@ -234,32 +242,41 @@
     @dhcp_server_address_port.setter
     def dhcp_server_address_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "dhcp_server_address_port", value)
 
     @property
     @pulumi.getter(name="enableNat")
     def enable_nat(self) -> Optional[pulumi.Input[bool]]:
+        """
+        - (Optional) Whether NAT should be performed for VPCs attaching to the subnet. This field is supported only for external subnets. NAT is enabled by default on external subnets.
+        """
         return pulumi.get(self, "enable_nat")
 
     @enable_nat.setter
     def enable_nat(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_nat", value)
 
     @property
     @pulumi.getter(name="ipConfigPoolListRanges")
     def ip_config_pool_list_ranges(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        -(Optional) Range of IPs.
+        """
         return pulumi.get(self, "ip_config_pool_list_ranges")
 
     @ip_config_pool_list_ranges.setter
     def ip_config_pool_list_ranges(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "ip_config_pool_list_ranges", value)
 
     @property
     @pulumi.getter(name="isExternal")
     def is_external(self) -> Optional[pulumi.Input[bool]]:
+        """
+        - (Optional) Whether the subnet is external subnet or not.
+        """
         return pulumi.get(self, "is_external")
 
     @is_external.setter
     def is_external(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_external", value)
 
     @property
@@ -334,25 +351,28 @@
     def subnet_ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subnet_ip", value)
 
     @property
     @pulumi.getter(name="vlanId")
     def vlan_id(self) -> Optional[pulumi.Input[int]]:
         """
-        - (Optional).
+        - (Optional). For VLAN subnet.
         """
         return pulumi.get(self, "vlan_id")
 
     @vlan_id.setter
     def vlan_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "vlan_id", value)
 
     @property
     @pulumi.getter(name="vpcReferenceUuid")
     def vpc_reference_uuid(self) -> Optional[pulumi.Input[str]]:
+        """
+        VPC reference uuid
+        """
         return pulumi.get(self, "vpc_reference_uuid")
 
     @vpc_reference_uuid.setter
     def vpc_reference_uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vpc_reference_uuid", value)
 
     @property
@@ -402,28 +422,33 @@
         Input properties used for looking up and filtering Subnet resources.
         :param pulumi.Input[str] api_version: The version of the API.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] availability_zone_reference: - (Optional) The reference to a availability_zone.
         :param pulumi.Input[Sequence[pulumi.Input['SubnetCategoryArgs']]] categories: - (Optional) The categories of the resource.
         :param pulumi.Input[str] cluster_uuid: - (Required) The UUID of the cluster.
         :param pulumi.Input[str] default_gateway_ip: - (Optional) Default gateway IP address.
         :param pulumi.Input[str] description: - (Optional) A description for subnet.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] dhcp_domain_search_lists: - (Optional).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dhcp_domain_name_server_lists: - (Optional). List of Domain Name Server addresses .
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dhcp_domain_search_lists: - (Optional).The DNS domain search list .
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] dhcp_options: - (Optional) Spec for defining DHCP options.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] dhcp_server_address: - (Optional) Host address.
         :param pulumi.Input[int] dhcp_server_address_port: - (Optional) Port Number.
+        :param pulumi.Input[bool] enable_nat: - (Optional) Whether NAT should be performed for VPCs attaching to the subnet. This field is supported only for external subnets. NAT is enabled by default on external subnets.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_config_pool_list_ranges: -(Optional) Range of IPs.
+        :param pulumi.Input[bool] is_external: - (Optional) Whether the subnet is external subnet or not.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: - (Required) The subnet kind metadata.
         :param pulumi.Input[str] name: - (Optional) Subnet name (Readonly).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] network_function_chain_reference: - (Optional) The reference to a network_function_chain.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] owner_reference: - (Optional) The reference to a user.
         :param pulumi.Input[int] prefix_length: - (Optional).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] project_reference: - (Optional) The reference to a project.
         :param pulumi.Input[str] state: - The state of the subnet.
         :param pulumi.Input[str] subnet_ip: - (Optional) Subnet IP address.
-        :param pulumi.Input[str] subnet_type: - (Optional).
-        :param pulumi.Input[int] vlan_id: - (Optional).
+        :param pulumi.Input[str] subnet_type: - (Optional). Valid Types are ["VLAN", "OVERLAY"]
+        :param pulumi.Input[int] vlan_id: - (Optional). For VLAN subnet.
+        :param pulumi.Input[str] vpc_reference_uuid: VPC reference uuid
         :param pulumi.Input[str] vswitch_name: - (Optional).
         """
         if api_version is not None:
             pulumi.set(__self__, "api_version", api_version)
         if availability_zone_reference is not None:
             pulumi.set(__self__, "availability_zone_reference", availability_zone_reference)
         if categories is not None:
@@ -557,25 +582,28 @@
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="dhcpDomainNameServerLists")
     def dhcp_domain_name_server_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        - (Optional). List of Domain Name Server addresses .
+        """
         return pulumi.get(self, "dhcp_domain_name_server_lists")
 
     @dhcp_domain_name_server_lists.setter
     def dhcp_domain_name_server_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "dhcp_domain_name_server_lists", value)
 
     @property
     @pulumi.getter(name="dhcpDomainSearchLists")
     def dhcp_domain_search_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        - (Optional).
+        - (Optional).The DNS domain search list .
         """
         return pulumi.get(self, "dhcp_domain_search_lists")
 
     @dhcp_domain_search_lists.setter
     def dhcp_domain_search_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "dhcp_domain_search_lists", value)
 
@@ -614,32 +642,41 @@
     @dhcp_server_address_port.setter
     def dhcp_server_address_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "dhcp_server_address_port", value)
 
     @property
     @pulumi.getter(name="enableNat")
     def enable_nat(self) -> Optional[pulumi.Input[bool]]:
+        """
+        - (Optional) Whether NAT should be performed for VPCs attaching to the subnet. This field is supported only for external subnets. NAT is enabled by default on external subnets.
+        """
         return pulumi.get(self, "enable_nat")
 
     @enable_nat.setter
     def enable_nat(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_nat", value)
 
     @property
     @pulumi.getter(name="ipConfigPoolListRanges")
     def ip_config_pool_list_ranges(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        -(Optional) Range of IPs.
+        """
         return pulumi.get(self, "ip_config_pool_list_ranges")
 
     @ip_config_pool_list_ranges.setter
     def ip_config_pool_list_ranges(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "ip_config_pool_list_ranges", value)
 
     @property
     @pulumi.getter(name="isExternal")
     def is_external(self) -> Optional[pulumi.Input[bool]]:
+        """
+        - (Optional) Whether the subnet is external subnet or not.
+        """
         return pulumi.get(self, "is_external")
 
     @is_external.setter
     def is_external(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_external", value)
 
     @property
@@ -738,37 +775,40 @@
     def subnet_ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subnet_ip", value)
 
     @property
     @pulumi.getter(name="subnetType")
     def subnet_type(self) -> Optional[pulumi.Input[str]]:
         """
-        - (Optional).
+        - (Optional). Valid Types are ["VLAN", "OVERLAY"]
         """
         return pulumi.get(self, "subnet_type")
 
     @subnet_type.setter
     def subnet_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subnet_type", value)
 
     @property
     @pulumi.getter(name="vlanId")
     def vlan_id(self) -> Optional[pulumi.Input[int]]:
         """
-        - (Optional).
+        - (Optional). For VLAN subnet.
         """
         return pulumi.get(self, "vlan_id")
 
     @vlan_id.setter
     def vlan_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "vlan_id", value)
 
     @property
     @pulumi.getter(name="vpcReferenceUuid")
     def vpc_reference_uuid(self) -> Optional[pulumi.Input[str]]:
+        """
+        VPC reference uuid
+        """
         return pulumi.get(self, "vpc_reference_uuid")
 
     @vpc_reference_uuid.setter
     def vpc_reference_uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vpc_reference_uuid", value)
 
     @property
@@ -819,26 +859,31 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] availability_zone_reference: - (Optional) The reference to a availability_zone.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SubnetCategoryArgs']]]] categories: - (Optional) The categories of the resource.
         :param pulumi.Input[str] cluster_uuid: - (Required) The UUID of the cluster.
         :param pulumi.Input[str] default_gateway_ip: - (Optional) Default gateway IP address.
         :param pulumi.Input[str] description: - (Optional) A description for subnet.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] dhcp_domain_search_lists: - (Optional).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dhcp_domain_name_server_lists: - (Optional). List of Domain Name Server addresses .
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dhcp_domain_search_lists: - (Optional).The DNS domain search list .
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] dhcp_options: - (Optional) Spec for defining DHCP options.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] dhcp_server_address: - (Optional) Host address.
         :param pulumi.Input[int] dhcp_server_address_port: - (Optional) Port Number.
+        :param pulumi.Input[bool] enable_nat: - (Optional) Whether NAT should be performed for VPCs attaching to the subnet. This field is supported only for external subnets. NAT is enabled by default on external subnets.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_config_pool_list_ranges: -(Optional) Range of IPs.
+        :param pulumi.Input[bool] is_external: - (Optional) Whether the subnet is external subnet or not.
         :param pulumi.Input[str] name: - (Optional) Subnet name (Readonly).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] network_function_chain_reference: - (Optional) The reference to a network_function_chain.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] owner_reference: - (Optional) The reference to a user.
         :param pulumi.Input[int] prefix_length: - (Optional).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] project_reference: - (Optional) The reference to a project.
         :param pulumi.Input[str] subnet_ip: - (Optional) Subnet IP address.
-        :param pulumi.Input[str] subnet_type: - (Optional).
-        :param pulumi.Input[int] vlan_id: - (Optional).
+        :param pulumi.Input[str] subnet_type: - (Optional). Valid Types are ["VLAN", "OVERLAY"]
+        :param pulumi.Input[int] vlan_id: - (Optional). For VLAN subnet.
+        :param pulumi.Input[str] vpc_reference_uuid: VPC reference uuid
         :param pulumi.Input[str] vswitch_name: - (Optional).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SubnetArgs,
@@ -968,28 +1013,33 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] api_version: The version of the API.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] availability_zone_reference: - (Optional) The reference to a availability_zone.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SubnetCategoryArgs']]]] categories: - (Optional) The categories of the resource.
         :param pulumi.Input[str] cluster_uuid: - (Required) The UUID of the cluster.
         :param pulumi.Input[str] default_gateway_ip: - (Optional) Default gateway IP address.
         :param pulumi.Input[str] description: - (Optional) A description for subnet.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] dhcp_domain_search_lists: - (Optional).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dhcp_domain_name_server_lists: - (Optional). List of Domain Name Server addresses .
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dhcp_domain_search_lists: - (Optional).The DNS domain search list .
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] dhcp_options: - (Optional) Spec for defining DHCP options.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] dhcp_server_address: - (Optional) Host address.
         :param pulumi.Input[int] dhcp_server_address_port: - (Optional) Port Number.
+        :param pulumi.Input[bool] enable_nat: - (Optional) Whether NAT should be performed for VPCs attaching to the subnet. This field is supported only for external subnets. NAT is enabled by default on external subnets.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_config_pool_list_ranges: -(Optional) Range of IPs.
+        :param pulumi.Input[bool] is_external: - (Optional) Whether the subnet is external subnet or not.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: - (Required) The subnet kind metadata.
         :param pulumi.Input[str] name: - (Optional) Subnet name (Readonly).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] network_function_chain_reference: - (Optional) The reference to a network_function_chain.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] owner_reference: - (Optional) The reference to a user.
         :param pulumi.Input[int] prefix_length: - (Optional).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] project_reference: - (Optional) The reference to a project.
         :param pulumi.Input[str] state: - The state of the subnet.
         :param pulumi.Input[str] subnet_ip: - (Optional) Subnet IP address.
-        :param pulumi.Input[str] subnet_type: - (Optional).
-        :param pulumi.Input[int] vlan_id: - (Optional).
+        :param pulumi.Input[str] subnet_type: - (Optional). Valid Types are ["VLAN", "OVERLAY"]
+        :param pulumi.Input[int] vlan_id: - (Optional). For VLAN subnet.
+        :param pulumi.Input[str] vpc_reference_uuid: VPC reference uuid
         :param pulumi.Input[str] vswitch_name: - (Optional).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SubnetState.__new__(_SubnetState)
 
         __props__.__dict__["api_version"] = api_version
@@ -1073,21 +1123,24 @@
         - (Optional) A description for subnet.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="dhcpDomainNameServerLists")
     def dhcp_domain_name_server_lists(self) -> pulumi.Output[Sequence[str]]:
+        """
+        - (Optional). List of Domain Name Server addresses .
+        """
         return pulumi.get(self, "dhcp_domain_name_server_lists")
 
     @property
     @pulumi.getter(name="dhcpDomainSearchLists")
     def dhcp_domain_search_lists(self) -> pulumi.Output[Sequence[str]]:
         """
-        - (Optional).
+        - (Optional).The DNS domain search list .
         """
         return pulumi.get(self, "dhcp_domain_search_lists")
 
     @property
     @pulumi.getter(name="dhcpOptions")
     def dhcp_options(self) -> pulumi.Output[Mapping[str, str]]:
         """
@@ -1110,24 +1163,33 @@
         - (Optional) Port Number.
         """
         return pulumi.get(self, "dhcp_server_address_port")
 
     @property
     @pulumi.getter(name="enableNat")
     def enable_nat(self) -> pulumi.Output[bool]:
+        """
+        - (Optional) Whether NAT should be performed for VPCs attaching to the subnet. This field is supported only for external subnets. NAT is enabled by default on external subnets.
+        """
         return pulumi.get(self, "enable_nat")
 
     @property
     @pulumi.getter(name="ipConfigPoolListRanges")
     def ip_config_pool_list_ranges(self) -> pulumi.Output[Sequence[str]]:
+        """
+        -(Optional) Range of IPs.
+        """
         return pulumi.get(self, "ip_config_pool_list_ranges")
 
     @property
     @pulumi.getter(name="isExternal")
     def is_external(self) -> pulumi.Output[bool]:
+        """
+        - (Optional) Whether the subnet is external subnet or not.
+        """
         return pulumi.get(self, "is_external")
 
     @property
     @pulumi.getter
     def metadata(self) -> pulumi.Output[Mapping[str, str]]:
         """
         - (Required) The subnet kind metadata.
@@ -1190,29 +1252,32 @@
         """
         return pulumi.get(self, "subnet_ip")
 
     @property
     @pulumi.getter(name="subnetType")
     def subnet_type(self) -> pulumi.Output[str]:
         """
-        - (Optional).
+        - (Optional). Valid Types are ["VLAN", "OVERLAY"]
         """
         return pulumi.get(self, "subnet_type")
 
     @property
     @pulumi.getter(name="vlanId")
     def vlan_id(self) -> pulumi.Output[int]:
         """
-        - (Optional).
+        - (Optional). For VLAN subnet.
         """
         return pulumi.get(self, "vlan_id")
 
     @property
     @pulumi.getter(name="vpcReferenceUuid")
     def vpc_reference_uuid(self) -> pulumi.Output[str]:
+        """
+        VPC reference uuid
+        """
         return pulumi.get(self, "vpc_reference_uuid")
 
     @property
     @pulumi.getter(name="vswitchName")
     def vswitch_name(self) -> pulumi.Output[str]:
         """
         - (Optional).
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/user.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/virtual_machine.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/virtual_machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,28 +71,30 @@
         :param pulumi.Input[bool] enable_script_exec: - (Optional) Extra configs related to power state transition. Indicates whether to execute set script before ngt shutdown/reboot.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineGpuListArgs']]] gpu_lists: - (Optional) GPUs attached to the VM.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] guest_customization_cloud_init_custom_key_values: - (Optional) Generic key value pair used for custom attributes in cloud init.
         :param pulumi.Input[str] guest_customization_cloud_init_meta_data: The contents of the meta_data configuration for cloud-init. This can be formatted as YAML or JSON. The value must be base64 encoded.
         :param pulumi.Input[str] guest_customization_cloud_init_user_data: - (Optional) The contents of the user_data configuration for cloud-init. This can be formatted as YAML, JSON, or could be a shell script. The value must be base64 encoded.
         :param pulumi.Input[bool] guest_customization_is_overridable: - (Optional) Flag to allow override of customization by deployer.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] guest_customization_sysprep: - (Optional) VM guests may be customized at boot time using one of several different methods. Currently, cloud-init w/ ConfigDriveV2 (for Linux VMs) and Sysprep (for Windows VMs) are supported. Only ONE OF sysprep or cloud_init should be provided. Note that guest customization can currently only be set during VM creation. Attempting to change it after creation will result in an error. Additional properties can be specified. For example - in the context of VM template creation if \\"override_script\\" is set to \\"True\\" then the deployer can upload their own custom script.
+        :param pulumi.Input[Mapping[str, Any]] guest_customization_sysprep_custom_key_values: - (Optional) Generic key value pair used for custom attributes in sysprep.
         :param pulumi.Input[str] guest_os_id: - (Optional) Guest OS Identifier. For ESX, refer to VMware documentation [link](https://www.vmware.com/support/developer/converter-sdk/conv43_apireference/vim.vm.GuestOsDescriptor.GuestOsIdentifier.html) for the list of guest OS identifiers.
         :param pulumi.Input[str] hardware_clock_timezone: - (Optional) VM's hardware clock timezone in IANA TZDB format (America/Los_Angeles).
         :param pulumi.Input[bool] is_vcpu_hard_pinned: - (Optional) Add true to enable CPU pinning.
         :param pulumi.Input[str] machine_type: - Machine type for the VM. Machine type Q35 is required for secure boot and does not support IDE disks.
-        :param pulumi.Input[int] memory_size_mib: - (Optional) Memory size in MiB.
+        :param pulumi.Input[int] memory_size_mib: - (Optional) Memory size in MiB. On updating memory to powered ON VMs should only be done in 1GB increments.
         :param pulumi.Input[str] name: - (Required) The name for the vm.
         :param pulumi.Input[Mapping[str, Any]] ngt_credentials: - (Ooptional) Credentials to login server.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ngt_enabled_capability_lists: Application names that are enabled.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineNicListArgs']]] nic_lists: - (Optional) Spec NICs attached to the VM.
         :param pulumi.Input[int] num_sockets: - (Optional) Number of vCPU sockets.
         :param pulumi.Input[int] num_vcpus_per_socket: - (Optional) Number of vCPUs per socket.
         :param pulumi.Input[int] num_vnuma_nodes: - (Optional) Number of vNUMA nodes. 0 means vNUMA is disabled.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] nutanix_guest_tools: - (Optional) Information regarding Nutanix Guest Tools.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] owner_reference: - (Optional) The reference to a user.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parent_reference: - (Optional) Reference to an entity that the VM cloned from.
         :param pulumi.Input[str] power_state_mechanism: - (Optional) Indicates the mechanism guiding the VM power state transition. Currently used for the transition to \\"OFF\\" state. Power state mechanism (ACPI/GUEST/HARD).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] project_reference: - (Optional) The reference to a project.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineSerialPortListArgs']]] serial_port_lists: - (Optional) Serial Ports configured on the VM.
         :param pulumi.Input[bool] should_fail_on_script_failure: - (Optional)  Extra configs related to power state transition. Indicates whether to abort ngt shutdown/reboot if script fails.
         :param pulumi.Input[bool] use_hot_add: - (Optional) Use Hot Add when modifying VM resources. Passing value false will result in VM reboots. Default value is `true`.
         :param pulumi.Input[bool] vga_console_enabled: - (Optional) Indicates whether VGA console should be enabled or not.
         """
@@ -388,14 +390,17 @@
     @guest_customization_sysprep.setter
     def guest_customization_sysprep(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "guest_customization_sysprep", value)
 
     @property
     @pulumi.getter(name="guestCustomizationSysprepCustomKeyValues")
     def guest_customization_sysprep_custom_key_values(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+        """
+        - (Optional) Generic key value pair used for custom attributes in sysprep.
+        """
         return pulumi.get(self, "guest_customization_sysprep_custom_key_values")
 
     @guest_customization_sysprep_custom_key_values.setter
     def guest_customization_sysprep_custom_key_values(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "guest_customization_sysprep_custom_key_values", value)
 
     @property
@@ -446,15 +451,15 @@
     def machine_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "machine_type", value)
 
     @property
     @pulumi.getter(name="memorySizeMib")
     def memory_size_mib(self) -> Optional[pulumi.Input[int]]:
         """
-        - (Optional) Memory size in MiB.
+        - (Optional) Memory size in MiB. On updating memory to powered ON VMs should only be done in 1GB increments.
         """
         return pulumi.get(self, "memory_size_mib")
 
     @memory_size_mib.setter
     def memory_size_mib(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "memory_size_mib", value)
 
@@ -565,14 +570,17 @@
     @owner_reference.setter
     def owner_reference(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "owner_reference", value)
 
     @property
     @pulumi.getter(name="parentReference")
     def parent_reference(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        - (Optional) Reference to an entity that the VM cloned from.
+        """
         return pulumi.get(self, "parent_reference")
 
     @parent_reference.setter
     def parent_reference(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "parent_reference", value)
 
     @property
@@ -716,38 +724,40 @@
         :param pulumi.Input[bool] enable_script_exec: - (Optional) Extra configs related to power state transition. Indicates whether to execute set script before ngt shutdown/reboot.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineGpuListArgs']]] gpu_lists: - (Optional) GPUs attached to the VM.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] guest_customization_cloud_init_custom_key_values: - (Optional) Generic key value pair used for custom attributes in cloud init.
         :param pulumi.Input[str] guest_customization_cloud_init_meta_data: The contents of the meta_data configuration for cloud-init. This can be formatted as YAML or JSON. The value must be base64 encoded.
         :param pulumi.Input[str] guest_customization_cloud_init_user_data: - (Optional) The contents of the user_data configuration for cloud-init. This can be formatted as YAML, JSON, or could be a shell script. The value must be base64 encoded.
         :param pulumi.Input[bool] guest_customization_is_overridable: - (Optional) Flag to allow override of customization by deployer.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] guest_customization_sysprep: - (Optional) VM guests may be customized at boot time using one of several different methods. Currently, cloud-init w/ ConfigDriveV2 (for Linux VMs) and Sysprep (for Windows VMs) are supported. Only ONE OF sysprep or cloud_init should be provided. Note that guest customization can currently only be set during VM creation. Attempting to change it after creation will result in an error. Additional properties can be specified. For example - in the context of VM template creation if \\"override_script\\" is set to \\"True\\" then the deployer can upload their own custom script.
+        :param pulumi.Input[Mapping[str, Any]] guest_customization_sysprep_custom_key_values: - (Optional) Generic key value pair used for custom attributes in sysprep.
         :param pulumi.Input[str] guest_os_id: - (Optional) Guest OS Identifier. For ESX, refer to VMware documentation [link](https://www.vmware.com/support/developer/converter-sdk/conv43_apireference/vim.vm.GuestOsDescriptor.GuestOsIdentifier.html) for the list of guest OS identifiers.
         :param pulumi.Input[str] hardware_clock_timezone: - (Optional) VM's hardware clock timezone in IANA TZDB format (America/Los_Angeles).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] host_reference: - Reference to a host.
         :param pulumi.Input[str] hypervisor_type: - The hypervisor type for the hypervisor the VM is hosted on.
         :param pulumi.Input[bool] is_vcpu_hard_pinned: - (Optional) Add true to enable CPU pinning.
         :param pulumi.Input[str] machine_type: - Machine type for the VM. Machine type Q35 is required for secure boot and does not support IDE disks.
-        :param pulumi.Input[int] memory_size_mib: - (Optional) Memory size in MiB.
+        :param pulumi.Input[int] memory_size_mib: - (Optional) Memory size in MiB. On updating memory to powered ON VMs should only be done in 1GB increments.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: - The vm kind metadata.
         :param pulumi.Input[str] name: - (Required) The name for the vm.
         :param pulumi.Input[Mapping[str, Any]] ngt_credentials: - (Ooptional) Credentials to login server.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ngt_enabled_capability_lists: Application names that are enabled.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineNicListStatusArgs']]] nic_list_statuses: - Status NICs attached to the VM.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineNicListArgs']]] nic_lists: - (Optional) Spec NICs attached to the VM.
         :param pulumi.Input[int] num_sockets: - (Optional) Number of vCPU sockets.
         :param pulumi.Input[int] num_vcpus_per_socket: - (Optional) Number of vCPUs per socket.
         :param pulumi.Input[int] num_vnuma_nodes: - (Optional) Number of vNUMA nodes. 0 means vNUMA is disabled.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] nutanix_guest_tools: - (Optional) Information regarding Nutanix Guest Tools.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] owner_reference: - (Optional) The reference to a user.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parent_reference: - (Optional) Reference to an entity that the VM cloned from.
         :param pulumi.Input[str] power_state: - (Optional) The current or desired power state of the VM. (Options : ON , OFF)
         :param pulumi.Input[str] power_state_mechanism: - (Optional) Indicates the mechanism guiding the VM power state transition. Currently used for the transition to \\"OFF\\" state. Power state mechanism (ACPI/GUEST/HARD).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] project_reference: - (Optional) The reference to a project.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineSerialPortListArgs']]] serial_port_lists: - (Optional) Serial Ports configured on the VM.
         :param pulumi.Input[bool] should_fail_on_script_failure: - (Optional)  Extra configs related to power state transition. Indicates whether to abort ngt shutdown/reboot if script fails.
-        :param pulumi.Input[str] state: - (Optional) Nutanix Guest Tools is enabled or not.
+        :param pulumi.Input[str] state: - The state of the vm.
         :param pulumi.Input[bool] use_hot_add: - (Optional) Use Hot Add when modifying VM resources. Passing value false will result in VM reboots. Default value is `true`.
         :param pulumi.Input[bool] vga_console_enabled: - (Optional) Indicates whether VGA console should be enabled or not.
         """
         if api_version is not None:
             pulumi.set(__self__, "api_version", api_version)
         if availability_zone_reference is not None:
             pulumi.set(__self__, "availability_zone_reference", availability_zone_reference)
@@ -1080,14 +1090,17 @@
     @guest_customization_sysprep.setter
     def guest_customization_sysprep(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "guest_customization_sysprep", value)
 
     @property
     @pulumi.getter(name="guestCustomizationSysprepCustomKeyValues")
     def guest_customization_sysprep_custom_key_values(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+        """
+        - (Optional) Generic key value pair used for custom attributes in sysprep.
+        """
         return pulumi.get(self, "guest_customization_sysprep_custom_key_values")
 
     @guest_customization_sysprep_custom_key_values.setter
     def guest_customization_sysprep_custom_key_values(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "guest_customization_sysprep_custom_key_values", value)
 
     @property
@@ -1162,15 +1175,15 @@
     def machine_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "machine_type", value)
 
     @property
     @pulumi.getter(name="memorySizeMib")
     def memory_size_mib(self) -> Optional[pulumi.Input[int]]:
         """
-        - (Optional) Memory size in MiB.
+        - (Optional) Memory size in MiB. On updating memory to powered ON VMs should only be done in 1GB increments.
         """
         return pulumi.get(self, "memory_size_mib")
 
     @memory_size_mib.setter
     def memory_size_mib(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "memory_size_mib", value)
 
@@ -1305,14 +1318,17 @@
     @owner_reference.setter
     def owner_reference(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "owner_reference", value)
 
     @property
     @pulumi.getter(name="parentReference")
     def parent_reference(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        - (Optional) Reference to an entity that the VM cloned from.
+        """
         return pulumi.get(self, "parent_reference")
 
     @parent_reference.setter
     def parent_reference(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "parent_reference", value)
 
     @property
@@ -1375,15 +1391,15 @@
     def should_fail_on_script_failure(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "should_fail_on_script_failure", value)
 
     @property
     @pulumi.getter
     def state(self) -> Optional[pulumi.Input[str]]:
         """
-        - (Optional) Nutanix Guest Tools is enabled or not.
+        - The state of the vm.
         """
         return pulumi.get(self, "state")
 
     @state.setter
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
@@ -1474,14 +1490,15 @@
                 name="Environment",
                 value="Staging",
             )],
             num_vcpus_per_socket=1,
             num_sockets=1,
             memory_size_mib=2048)
         ```
+
         ### With Storage Config
         ```python
         import pulumi
         import pulumi_nutanix as nutanix
 
         clusters = nutanix.get_clusters()
         vm = nutanix.VirtualMachine("vm",
@@ -1497,14 +1514,26 @@
                         kind="storage_container",
                         uuid="2bbe67bc-fd14-4637-8de1-6379257f4219",
                     )],
                 ),
             )])
         ```
 
+        ## Import
+
+        Nutanix Virtual machines can be imported using the `UUID` eg,
+
+        `
+
+        ```sh
+        $ pulumi import nutanix:index/virtualMachine:VirtualMachine vm01 0F75E6A7-55FB-44D9-A50D-14AD72E2CF7C
+        ```
+
+        `
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] availability_zone_reference: - (Optional) The reference to a availability_zone.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] boot_device_disk_address: - (Optional) Address of disk to boot from.
         :param pulumi.Input[str] boot_device_mac_address: - (Optional) MAC address of nic to boot from.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] boot_device_order_lists: - (Optional) Indicates the order of device types in which VM should try to boot from. If boot device order is not provided the system will decide appropriate boot device order.
         :param pulumi.Input[str] boot_type: - (Optional) Indicates whether the VM should use Secure boot, UEFI boot or Legacy boot.If UEFI or; Secure boot is enabled then other legacy boot options (like boot_device and; boot_device_order_list) are ignored. Secure boot depends on UEFI boot, i.e. enabling; Secure boot means that UEFI boot is also enabled. The possible value are: UEFI", "LEGACY", "SECURE_BOOT".
@@ -1516,28 +1545,30 @@
         :param pulumi.Input[bool] enable_script_exec: - (Optional) Extra configs related to power state transition. Indicates whether to execute set script before ngt shutdown/reboot.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineGpuListArgs']]]] gpu_lists: - (Optional) GPUs attached to the VM.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] guest_customization_cloud_init_custom_key_values: - (Optional) Generic key value pair used for custom attributes in cloud init.
         :param pulumi.Input[str] guest_customization_cloud_init_meta_data: The contents of the meta_data configuration for cloud-init. This can be formatted as YAML or JSON. The value must be base64 encoded.
         :param pulumi.Input[str] guest_customization_cloud_init_user_data: - (Optional) The contents of the user_data configuration for cloud-init. This can be formatted as YAML, JSON, or could be a shell script. The value must be base64 encoded.
         :param pulumi.Input[bool] guest_customization_is_overridable: - (Optional) Flag to allow override of customization by deployer.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] guest_customization_sysprep: - (Optional) VM guests may be customized at boot time using one of several different methods. Currently, cloud-init w/ ConfigDriveV2 (for Linux VMs) and Sysprep (for Windows VMs) are supported. Only ONE OF sysprep or cloud_init should be provided. Note that guest customization can currently only be set during VM creation. Attempting to change it after creation will result in an error. Additional properties can be specified. For example - in the context of VM template creation if \\"override_script\\" is set to \\"True\\" then the deployer can upload their own custom script.
+        :param pulumi.Input[Mapping[str, Any]] guest_customization_sysprep_custom_key_values: - (Optional) Generic key value pair used for custom attributes in sysprep.
         :param pulumi.Input[str] guest_os_id: - (Optional) Guest OS Identifier. For ESX, refer to VMware documentation [link](https://www.vmware.com/support/developer/converter-sdk/conv43_apireference/vim.vm.GuestOsDescriptor.GuestOsIdentifier.html) for the list of guest OS identifiers.
         :param pulumi.Input[str] hardware_clock_timezone: - (Optional) VM's hardware clock timezone in IANA TZDB format (America/Los_Angeles).
         :param pulumi.Input[bool] is_vcpu_hard_pinned: - (Optional) Add true to enable CPU pinning.
         :param pulumi.Input[str] machine_type: - Machine type for the VM. Machine type Q35 is required for secure boot and does not support IDE disks.
-        :param pulumi.Input[int] memory_size_mib: - (Optional) Memory size in MiB.
+        :param pulumi.Input[int] memory_size_mib: - (Optional) Memory size in MiB. On updating memory to powered ON VMs should only be done in 1GB increments.
         :param pulumi.Input[str] name: - (Required) The name for the vm.
         :param pulumi.Input[Mapping[str, Any]] ngt_credentials: - (Ooptional) Credentials to login server.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ngt_enabled_capability_lists: Application names that are enabled.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNicListArgs']]]] nic_lists: - (Optional) Spec NICs attached to the VM.
         :param pulumi.Input[int] num_sockets: - (Optional) Number of vCPU sockets.
         :param pulumi.Input[int] num_vcpus_per_socket: - (Optional) Number of vCPUs per socket.
         :param pulumi.Input[int] num_vnuma_nodes: - (Optional) Number of vNUMA nodes. 0 means vNUMA is disabled.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] nutanix_guest_tools: - (Optional) Information regarding Nutanix Guest Tools.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] owner_reference: - (Optional) The reference to a user.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parent_reference: - (Optional) Reference to an entity that the VM cloned from.
         :param pulumi.Input[str] power_state_mechanism: - (Optional) Indicates the mechanism guiding the VM power state transition. Currently used for the transition to \\"OFF\\" state. Power state mechanism (ACPI/GUEST/HARD).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] project_reference: - (Optional) The reference to a project.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineSerialPortListArgs']]]] serial_port_lists: - (Optional) Serial Ports configured on the VM.
         :param pulumi.Input[bool] should_fail_on_script_failure: - (Optional)  Extra configs related to power state transition. Indicates whether to abort ngt shutdown/reboot if script fails.
         :param pulumi.Input[bool] use_hot_add: - (Optional) Use Hot Add when modifying VM resources. Passing value false will result in VM reboots. Default value is `true`.
         :param pulumi.Input[bool] vga_console_enabled: - (Optional) Indicates whether VGA console should be enabled or not.
         """
@@ -1563,14 +1594,15 @@
                 name="Environment",
                 value="Staging",
             )],
             num_vcpus_per_socket=1,
             num_sockets=1,
             memory_size_mib=2048)
         ```
+
         ### With Storage Config
         ```python
         import pulumi
         import pulumi_nutanix as nutanix
 
         clusters = nutanix.get_clusters()
         vm = nutanix.VirtualMachine("vm",
@@ -1586,14 +1618,26 @@
                         kind="storage_container",
                         uuid="2bbe67bc-fd14-4637-8de1-6379257f4219",
                     )],
                 ),
             )])
         ```
 
+        ## Import
+
+        Nutanix Virtual machines can be imported using the `UUID` eg,
+
+        `
+
+        ```sh
+        $ pulumi import nutanix:index/virtualMachine:VirtualMachine vm01 0F75E6A7-55FB-44D9-A50D-14AD72E2CF7C
+        ```
+
+        `
+
         :param str resource_name: The name of the resource.
         :param VirtualMachineArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(VirtualMachineArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -1784,38 +1828,40 @@
         :param pulumi.Input[bool] enable_script_exec: - (Optional) Extra configs related to power state transition. Indicates whether to execute set script before ngt shutdown/reboot.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineGpuListArgs']]]] gpu_lists: - (Optional) GPUs attached to the VM.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] guest_customization_cloud_init_custom_key_values: - (Optional) Generic key value pair used for custom attributes in cloud init.
         :param pulumi.Input[str] guest_customization_cloud_init_meta_data: The contents of the meta_data configuration for cloud-init. This can be formatted as YAML or JSON. The value must be base64 encoded.
         :param pulumi.Input[str] guest_customization_cloud_init_user_data: - (Optional) The contents of the user_data configuration for cloud-init. This can be formatted as YAML, JSON, or could be a shell script. The value must be base64 encoded.
         :param pulumi.Input[bool] guest_customization_is_overridable: - (Optional) Flag to allow override of customization by deployer.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] guest_customization_sysprep: - (Optional) VM guests may be customized at boot time using one of several different methods. Currently, cloud-init w/ ConfigDriveV2 (for Linux VMs) and Sysprep (for Windows VMs) are supported. Only ONE OF sysprep or cloud_init should be provided. Note that guest customization can currently only be set during VM creation. Attempting to change it after creation will result in an error. Additional properties can be specified. For example - in the context of VM template creation if \\"override_script\\" is set to \\"True\\" then the deployer can upload their own custom script.
+        :param pulumi.Input[Mapping[str, Any]] guest_customization_sysprep_custom_key_values: - (Optional) Generic key value pair used for custom attributes in sysprep.
         :param pulumi.Input[str] guest_os_id: - (Optional) Guest OS Identifier. For ESX, refer to VMware documentation [link](https://www.vmware.com/support/developer/converter-sdk/conv43_apireference/vim.vm.GuestOsDescriptor.GuestOsIdentifier.html) for the list of guest OS identifiers.
         :param pulumi.Input[str] hardware_clock_timezone: - (Optional) VM's hardware clock timezone in IANA TZDB format (America/Los_Angeles).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] host_reference: - Reference to a host.
         :param pulumi.Input[str] hypervisor_type: - The hypervisor type for the hypervisor the VM is hosted on.
         :param pulumi.Input[bool] is_vcpu_hard_pinned: - (Optional) Add true to enable CPU pinning.
         :param pulumi.Input[str] machine_type: - Machine type for the VM. Machine type Q35 is required for secure boot and does not support IDE disks.
-        :param pulumi.Input[int] memory_size_mib: - (Optional) Memory size in MiB.
+        :param pulumi.Input[int] memory_size_mib: - (Optional) Memory size in MiB. On updating memory to powered ON VMs should only be done in 1GB increments.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] metadata: - The vm kind metadata.
         :param pulumi.Input[str] name: - (Required) The name for the vm.
         :param pulumi.Input[Mapping[str, Any]] ngt_credentials: - (Ooptional) Credentials to login server.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ngt_enabled_capability_lists: Application names that are enabled.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNicListStatusArgs']]]] nic_list_statuses: - Status NICs attached to the VM.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNicListArgs']]]] nic_lists: - (Optional) Spec NICs attached to the VM.
         :param pulumi.Input[int] num_sockets: - (Optional) Number of vCPU sockets.
         :param pulumi.Input[int] num_vcpus_per_socket: - (Optional) Number of vCPUs per socket.
         :param pulumi.Input[int] num_vnuma_nodes: - (Optional) Number of vNUMA nodes. 0 means vNUMA is disabled.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] nutanix_guest_tools: - (Optional) Information regarding Nutanix Guest Tools.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] owner_reference: - (Optional) The reference to a user.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parent_reference: - (Optional) Reference to an entity that the VM cloned from.
         :param pulumi.Input[str] power_state: - (Optional) The current or desired power state of the VM. (Options : ON , OFF)
         :param pulumi.Input[str] power_state_mechanism: - (Optional) Indicates the mechanism guiding the VM power state transition. Currently used for the transition to \\"OFF\\" state. Power state mechanism (ACPI/GUEST/HARD).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] project_reference: - (Optional) The reference to a project.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineSerialPortListArgs']]]] serial_port_lists: - (Optional) Serial Ports configured on the VM.
         :param pulumi.Input[bool] should_fail_on_script_failure: - (Optional)  Extra configs related to power state transition. Indicates whether to abort ngt shutdown/reboot if script fails.
-        :param pulumi.Input[str] state: - (Optional) Nutanix Guest Tools is enabled or not.
+        :param pulumi.Input[str] state: - The state of the vm.
         :param pulumi.Input[bool] use_hot_add: - (Optional) Use Hot Add when modifying VM resources. Passing value false will result in VM reboots. Default value is `true`.
         :param pulumi.Input[bool] vga_console_enabled: - (Optional) Indicates whether VGA console should be enabled or not.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _VirtualMachineState.__new__(_VirtualMachineState)
 
@@ -2025,14 +2071,17 @@
         - (Optional) VM guests may be customized at boot time using one of several different methods. Currently, cloud-init w/ ConfigDriveV2 (for Linux VMs) and Sysprep (for Windows VMs) are supported. Only ONE OF sysprep or cloud_init should be provided. Note that guest customization can currently only be set during VM creation. Attempting to change it after creation will result in an error. Additional properties can be specified. For example - in the context of VM template creation if \\"override_script\\" is set to \\"True\\" then the deployer can upload their own custom script.
         """
         return pulumi.get(self, "guest_customization_sysprep")
 
     @property
     @pulumi.getter(name="guestCustomizationSysprepCustomKeyValues")
     def guest_customization_sysprep_custom_key_values(self) -> pulumi.Output[Mapping[str, Any]]:
+        """
+        - (Optional) Generic key value pair used for custom attributes in sysprep.
+        """
         return pulumi.get(self, "guest_customization_sysprep_custom_key_values")
 
     @property
     @pulumi.getter(name="guestOsId")
     def guest_os_id(self) -> pulumi.Output[str]:
         """
         - (Optional) Guest OS Identifier. For ESX, refer to VMware documentation [link](https://www.vmware.com/support/developer/converter-sdk/conv43_apireference/vim.vm.GuestOsDescriptor.GuestOsIdentifier.html) for the list of guest OS identifiers.
@@ -2079,15 +2128,15 @@
         """
         return pulumi.get(self, "machine_type")
 
     @property
     @pulumi.getter(name="memorySizeMib")
     def memory_size_mib(self) -> pulumi.Output[int]:
         """
-        - (Optional) Memory size in MiB.
+        - (Optional) Memory size in MiB. On updating memory to powered ON VMs should only be done in 1GB increments.
         """
         return pulumi.get(self, "memory_size_mib")
 
     @property
     @pulumi.getter
     def metadata(self) -> pulumi.Output[Mapping[str, str]]:
         """
@@ -2174,14 +2223,17 @@
         - (Optional) The reference to a user.
         """
         return pulumi.get(self, "owner_reference")
 
     @property
     @pulumi.getter(name="parentReference")
     def parent_reference(self) -> pulumi.Output[Mapping[str, str]]:
+        """
+        - (Optional) Reference to an entity that the VM cloned from.
+        """
         return pulumi.get(self, "parent_reference")
 
     @property
     @pulumi.getter(name="powerState")
     def power_state(self) -> pulumi.Output[str]:
         """
         - (Optional) The current or desired power state of the VM. (Options : ON , OFF)
@@ -2220,15 +2272,15 @@
         """
         return pulumi.get(self, "should_fail_on_script_failure")
 
     @property
     @pulumi.getter
     def state(self) -> pulumi.Output[str]:
         """
-        - (Optional) Nutanix Guest Tools is enabled or not.
+        - The state of the vm.
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter(name="useHotAdd")
     def use_hot_add(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix/vpc.py` & `pulumi_nutanix-0.0.48/pulumi_nutanix/vpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,15 @@
                  externally_routable_prefix_lists: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VpcExternallyRoutablePrefixListArgs']]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides Nutanix resource to create VPC.
 
         ## Example Usage
+
         ### vpc creation with external subnet name
 
         ```python
         import pulumi
         import pulumi_nutanix as nutanix
 
         vpc = nutanix.Vpc("vpc",
@@ -289,14 +290,15 @@
                 "test-ext2",
             ],
             externally_routable_prefix_lists=[nutanix.VpcExternallyRoutablePrefixListArgs(
                 ip="192.43.0.0",
                 prefix_length=16,
             )])
         ```
+
         ### vpc creation with external subnet uuid
 
         ```python
         import pulumi
         import pulumi_nutanix as nutanix
 
         vpc = nutanix.Vpc("vpc",
@@ -331,14 +333,15 @@
                  resource_name: str,
                  args: Optional[VpcArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides Nutanix resource to create VPC.
 
         ## Example Usage
+
         ### vpc creation with external subnet name
 
         ```python
         import pulumi
         import pulumi_nutanix as nutanix
 
         vpc = nutanix.Vpc("vpc",
@@ -355,14 +358,15 @@
                 "test-ext2",
             ],
             externally_routable_prefix_lists=[nutanix.VpcExternallyRoutablePrefixListArgs(
                 ip="192.43.0.0",
                 prefix_length=16,
             )])
         ```
+
         ### vpc creation with external subnet uuid
 
         ```python
         import pulumi
         import pulumi_nutanix as nutanix
 
         vpc = nutanix.Vpc("vpc",
```

### Comparing `pulumi_nutanix-0.0.47/pulumi_nutanix.egg-info/SOURCES.txt` & `pulumi_nutanix-0.0.48/pulumi_nutanix.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -27,25 +27,49 @@
 pulumi_nutanix/get_foundation_central_cluster_details.py
 pulumi_nutanix/get_foundation_central_imaged_clusters_list.py
 pulumi_nutanix/get_foundation_central_imaged_node_details.py
 pulumi_nutanix/get_foundation_central_imaged_nodes_list.py
 pulumi_nutanix/get_foundation_central_list_api_keys.py
 pulumi_nutanix/get_foundation_discover_nodes.py
 pulumi_nutanix/get_foundation_hypervisor_isos.py
-pulumi_nutanix/get_foundation_nod_packages.py
 pulumi_nutanix/get_foundation_node_network_details.py
+pulumi_nutanix/get_foundation_nos_packages.py
 pulumi_nutanix/get_host.py
 pulumi_nutanix/get_hosts.py
 pulumi_nutanix/get_image.py
 pulumi_nutanix/get_karbon_cluster.py
 pulumi_nutanix/get_karbon_cluster_kube_config.py
 pulumi_nutanix/get_karbon_cluster_ssh.py
 pulumi_nutanix/get_karbon_clusters.py
 pulumi_nutanix/get_karbon_private_registries.py
 pulumi_nutanix/get_karbon_private_registry.py
+pulumi_nutanix/get_ndb_clone.py
+pulumi_nutanix/get_ndb_clones.py
+pulumi_nutanix/get_ndb_cluster.py
+pulumi_nutanix/get_ndb_clusters.py
+pulumi_nutanix/get_ndb_database.py
+pulumi_nutanix/get_ndb_databases.py
+pulumi_nutanix/get_ndb_dbserver.py
+pulumi_nutanix/get_ndb_dbservers.py
+pulumi_nutanix/get_ndb_maintenance_window.py
+pulumi_nutanix/get_ndb_maintenance_windows.py
+pulumi_nutanix/get_ndb_network.py
+pulumi_nutanix/get_ndb_network_available_ips.py
+pulumi_nutanix/get_ndb_networks.py
+pulumi_nutanix/get_ndb_profile.py
+pulumi_nutanix/get_ndb_profiles.py
+pulumi_nutanix/get_ndb_sla.py
+pulumi_nutanix/get_ndb_slas.py
+pulumi_nutanix/get_ndb_snapshot.py
+pulumi_nutanix/get_ndb_snapshots.py
+pulumi_nutanix/get_ndb_tag.py
+pulumi_nutanix/get_ndb_tags.py
+pulumi_nutanix/get_ndb_time_machine.py
+pulumi_nutanix/get_ndb_time_machines.py
+pulumi_nutanix/get_ndb_tms_capability.py
 pulumi_nutanix/get_network_security_rule.py
 pulumi_nutanix/get_pbr.py
 pulumi_nutanix/get_pbrs.py
 pulumi_nutanix/get_permission.py
 pulumi_nutanix/get_permissions.py
 pulumi_nutanix/get_project.py
 pulumi_nutanix/get_projects.py
@@ -66,28 +90,53 @@
 pulumi_nutanix/get_users.py
 pulumi_nutanix/get_virtual_machine.py
 pulumi_nutanix/get_vpc.py
 pulumi_nutanix/get_vpcs.py
 pulumi_nutanix/image.py
 pulumi_nutanix/karbon_cluster.py
 pulumi_nutanix/karbon_private_registry.py
+pulumi_nutanix/karbon_worker_nodepool.py
+pulumi_nutanix/ndb_authorize_dbserver.py
+pulumi_nutanix/ndb_clone.py
+pulumi_nutanix/ndb_clone_refresh.py
+pulumi_nutanix/ndb_cluster.py
+pulumi_nutanix/ndb_database.py
+pulumi_nutanix/ndb_database_restore.py
+pulumi_nutanix/ndb_database_scale.py
+pulumi_nutanix/ndb_database_snapshot.py
+pulumi_nutanix/ndb_dbserver_vm.py
+pulumi_nutanix/ndb_linked_databases.py
+pulumi_nutanix/ndb_log_catchups.py
+pulumi_nutanix/ndb_maintenance_task.py
+pulumi_nutanix/ndb_maintenance_window.py
+pulumi_nutanix/ndb_network.py
+pulumi_nutanix/ndb_profile.py
+pulumi_nutanix/ndb_register_database.py
+pulumi_nutanix/ndb_register_dbserver.py
+pulumi_nutanix/ndb_scale_database.py
+pulumi_nutanix/ndb_sla.py
+pulumi_nutanix/ndb_software_version_profile.py
+pulumi_nutanix/ndb_stretched_vlan.py
+pulumi_nutanix/ndb_tag.py
+pulumi_nutanix/ndb_tms_cluster.py
 pulumi_nutanix/network_security_rule.py
 pulumi_nutanix/outputs.py
 pulumi_nutanix/pbr.py
 pulumi_nutanix/project.py
 pulumi_nutanix/protection_rule.py
 pulumi_nutanix/provider.py
 pulumi_nutanix/pulumi-plugin.json
 pulumi_nutanix/py.typed
 pulumi_nutanix/recovery_plan.py
 pulumi_nutanix/role.py
 pulumi_nutanix/service_group.py
 pulumi_nutanix/static_routes.py
 pulumi_nutanix/subnet.py
 pulumi_nutanix/user.py
+pulumi_nutanix/user_groups.py
 pulumi_nutanix/virtual_machine.py
 pulumi_nutanix/vpc.py
 pulumi_nutanix.egg-info/PKG-INFO
 pulumi_nutanix.egg-info/SOURCES.txt
 pulumi_nutanix.egg-info/dependency_links.txt
 pulumi_nutanix.egg-info/not-zip-safe
 pulumi_nutanix.egg-info/requires.txt
```

### Comparing `pulumi_nutanix-0.0.47/setup.py` & `pulumi_nutanix-0.0.48/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.47"
+VERSION = "0.0.48"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "nutanix Pulumi Package - Development Version"
 
 
 setup(name='pulumi_nutanix',
-      python_requires='>=3.7',
+      python_requires='>=3.8',
       version=VERSION,
       description="A Pulumi package for creating and managing nutanix cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       keywords='pulumi nutanix category/cloud',
       url='https://github.com/pierskarsenbarg/pulumi-nutanix',
       project_urls={
```

