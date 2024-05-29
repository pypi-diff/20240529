# Comparing `tmp/pulumi_sdwan-0.1.0a1716879684.tar.gz` & `tmp/pulumi_sdwan-0.1.0a1716883043.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_sdwan-0.1.0a1716879684.tar", last modified: Tue May 28 07:05:47 2024, max compression
+gzip compressed data, was "pulumi_sdwan-0.1.0a1716883043.tar", last modified: Tue May 28 08:00:10 2024, max compression
```

## Comparing `pulumi_sdwan-0.1.0a1716879684.tar` & `pulumi_sdwan-0.1.0a1716883043.tar`

### file list

```diff
@@ -1,294 +1,294 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:05:47.944932 pulumi_sdwan-0.1.0a1716879684/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-28 07:05:47.944932 pulumi_sdwan-0.1.0a1716879684/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:05:47.944932 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/
--rw-r--r--   0 runner    (1001) docker     (127)    44014 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1816905 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/activate_centralized_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    30793 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/advanced_inspection_profile_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    32911 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/advanced_malware_protection_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/allow_url_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/app_probe_class_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    12869 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/application_aware_routing_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/application_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/application_priority_feature_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    18992 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/application_priority_qos_policy_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/as_path_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8641 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/attach_feature_device_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/block_url_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    85236 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cedge_aaa_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   113060 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cedge_global_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    16913 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cedge_igmp_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    27529 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cedge_multicast_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    65661 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cedge_pim_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    46241 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cellular_cedge_profile_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    40154 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cellular_controller_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    62854 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cellular_profile_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/centralized_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    26555 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cflowd_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    22036 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_banner_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    30412 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_bfd_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    98513 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_bgp_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    54618 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_dhcp_server_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    35856 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_logging_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    36934 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_ntp_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    80185 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_omp_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    89950 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_ospf_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   194604 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_ospfv3_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    29470 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_secure_internet_gateway_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    47597 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_security_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    65606 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_sig_credentials_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    38477 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_snmp_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   232163 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_system_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    17746 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_thousandeyes_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    88191 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_trustsec_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    96935 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_vpn_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   513921 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_vpn_interface_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    77665 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_vpn_interface_gre_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   141327 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_vpn_interface_ipsec_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    55695 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_wireless_lan_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/class_map_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    13849 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cli_config_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    15324 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cli_device_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cli_feature_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cli_template_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9888 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/color_list_policy_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:05:47.944932 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    18675 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/configuration_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/configuration_group_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/configuration_group_device_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/configuration_group_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/custom_control_topology_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/data_fqdn_prefix_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    10304 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/data_ipv4_prefix_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/data_ipv6_prefix_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    33977 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/dns_security_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/domain_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    52201 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/eigrp_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/expanded_community_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    10456 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/extended_community_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    24657 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/feature_device_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/geo_location_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_advanced_inspection_profile_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_advanced_malware_protection_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_allow_url_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_app_probe_class_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_application_aware_routing_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_application_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_application_priority_feature_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_application_priority_qos_policy_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_as_path_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_block_url_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    24834 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cedge_aaa_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    32116 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cedge_global_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cedge_igmp_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cedge_multicast_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    18972 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cedge_pim_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cellular_cedge_profile_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cellular_controller_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    19127 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cellular_profile_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_centralized_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cflowd_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_banner_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_bfd_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    27303 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_bgp_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    16189 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_dhcp_server_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_logging_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_ntp_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    23164 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_omp_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    26037 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_ospf_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    55961 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_ospfv3_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_secure_internet_gateway_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    14105 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_security_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    20567 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_sig_credentials_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    11133 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_snmp_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    47301 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_system_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_thousandeyes_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    25663 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_trustsec_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    24735 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_vpn_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   143580 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_vpn_interface_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    23074 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_vpn_interface_gre_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    39416 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_vpn_interface_ipsec_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15728 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_wireless_lan_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_class_map_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cli_config_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cli_device_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cli_feature_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cli_template_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_color_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_configuration_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_configuration_group_device_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_configuration_group_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_custom_control_topology_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_data_fqdn_prefix_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_data_ipv4_prefix_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_data_ipv6_prefix_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    10802 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_dns_security_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_domain_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_eigrp_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_expanded_community_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_extended_community_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_feature_device_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_geo_location_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_gps_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_hub_and_spoke_topology_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_intrusion_prevention_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_ips_signature_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_ipv4_acl_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_ipv4_device_acl_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_ipv4_prefix_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_ipv6_acl_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_ipv6_device_acl_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_ipv6_prefix_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_local_application_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_localized_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_mesh_topology_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_mirror_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_object_group_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_policer_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_port_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_preferred_color_group_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_protocol_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_qos_map_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_region_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_rewrite_rule_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_route_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_rule_set_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_security_app_hosting_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_security_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_service_feature_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    58754 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_service_lan_vpn_interface_ethernet_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    29738 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_service_lan_vpn_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    17338 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_service_tracker_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_site_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_sla_class_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_standard_community_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_switchport_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_aaa_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_banner_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    42894 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_basic_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_bfd_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_feature_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_flexible_port_speed_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    32106 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_global_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_logging_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_mrf_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_ntp_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    42501 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_omp_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_performance_monitoring_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    37773 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_remote_access_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12673 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_security_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_snmp_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_tloc_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_tls_ssl_decryption_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    10603 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_tls_ssl_profile_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_traffic_data_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_transport_feature_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_transport_ipv6_tracker_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    35450 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_transport_management_vpn_interface_ethernet_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_transport_management_vpn_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    38737 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_transport_routing_bgp_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)   133799 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_transport_wan_vpn_interface_ethernet_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    15881 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_transport_wan_vpn_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11079 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_url_filtering_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vedge_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)   109443 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_cellular_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   118658 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_dsl_ipoe_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   110453 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_dsl_pppoa_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   117158 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_dsl_pppoe_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   116373 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_ethernet_pppoe_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   100746 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_multilink_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    27775 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_svi_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    89903 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_t1_e1_serial_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_membership_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_zone_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    39041 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/gps_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    16437 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/hub_and_spoke_topology_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    24962 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/intrusion_prevention_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/ips_signature_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    14507 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/ipv4_acl_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14749 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/ipv4_device_acl_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    10218 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/ipv4_prefix_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    14507 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/ipv6_acl_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14749 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/ipv6_device_acl_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/ipv6_prefix_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    10414 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/local_application_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    36302 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/localized_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    16008 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/mesh_topology_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11160 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/mirror_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    36119 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/object_group_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)  2702398 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/policer_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/port_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    23173 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/preferred_color_group_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/protocol_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/qos_map_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/region_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/rewrite_rule_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/route_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11221 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/rule_set_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/security_app_hosting_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    36588 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/security_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/service_feature_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)   209066 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/service_lan_vpn_interface_ethernet_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)   108249 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/service_lan_vpn_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    56467 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/service_tracker_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/site_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    29000 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/sla_class_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/standard_community_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    30741 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/switchport_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    47282 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_aaa_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    17728 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_banner_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)   212718 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_basic_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    25739 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_bfd_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_feature_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    17900 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_flexible_port_speed_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)   110811 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_global_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    33070 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_logging_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    27278 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_mrf_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    33906 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_ntp_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)   145714 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_omp_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    28150 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_performance_monitoring_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)   121745 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_remote_access_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    40023 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_security_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    36694 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_snmp_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/tloc_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    50541 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/tls_ssl_decryption_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    34035 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/tls_ssl_profile_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14639 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/traffic_data_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/transport_feature_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    49582 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/transport_ipv6_tracker_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)   120607 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/transport_management_vpn_interface_ethernet_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    44506 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/transport_management_vpn_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)   137806 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/transport_routing_bgp_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)   470349 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/transport_wan_vpn_interface_ethernet_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    50441 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/transport_wan_vpn_profile_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    37387 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/url_filtering_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)   383029 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_cellular_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   413280 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_dsl_ipoe_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   386431 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_dsl_pppoa_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   408281 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_dsl_pppoe_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   404832 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_ethernet_pppoe_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   351150 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_multilink_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   101455 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_svi_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)   313094 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_t1_e1_serial_feature_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_list_policy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    12255 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_membership_policy_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/zone_list_policy_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:05:47.944932 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-28 07:05:47.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13966 2024-05-28 07:05:47.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 07:05:47.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 07:05:47.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 07:05:47.000000 pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-28 07:05:41.000000 pulumi_sdwan-0.1.0a1716879684/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 07:05:47.944932 pulumi_sdwan-0.1.0a1716879684/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:00:10.838577 pulumi_sdwan-0.1.0a1716883043/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-28 08:00:10.838577 pulumi_sdwan-0.1.0a1716883043/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:00:10.838577 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/
+-rw-r--r--   0 runner    (1001) docker     (127)    44014 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1816905 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/activate_centralized_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30793 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/advanced_inspection_profile_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32911 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/advanced_malware_protection_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/allow_url_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/app_probe_class_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12869 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/application_aware_routing_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/application_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/application_priority_feature_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18992 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/application_priority_qos_policy_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/as_path_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8641 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/attach_feature_device_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/block_url_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85236 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cedge_aaa_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113060 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cedge_global_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16913 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cedge_igmp_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27529 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cedge_multicast_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65661 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cedge_pim_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46241 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cellular_cedge_profile_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40154 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cellular_controller_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62854 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cellular_profile_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/centralized_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26555 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cflowd_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22036 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_banner_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30412 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_bfd_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98513 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_bgp_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54618 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_dhcp_server_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35856 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_logging_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36934 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_ntp_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80185 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_omp_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89950 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_ospf_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   194604 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_ospfv3_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29470 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_secure_internet_gateway_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47597 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_security_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65606 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_sig_credentials_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38477 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_snmp_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   232163 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_system_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17746 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_thousandeyes_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88191 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_trustsec_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96935 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_vpn_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   513921 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_vpn_interface_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77665 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_vpn_interface_gre_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   141327 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_vpn_interface_ipsec_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55695 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_wireless_lan_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/class_map_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13849 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cli_config_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15324 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cli_device_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cli_feature_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cli_template_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9888 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/color_list_policy_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:00:10.838577 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18675 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/configuration_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/configuration_group_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/configuration_group_device_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/configuration_group_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/custom_control_topology_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/data_fqdn_prefix_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10304 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/data_ipv4_prefix_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/data_ipv6_prefix_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33977 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/dns_security_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/domain_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52201 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/eigrp_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/expanded_community_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10456 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/extended_community_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24657 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/feature_device_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/geo_location_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_advanced_inspection_profile_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_advanced_malware_protection_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_allow_url_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_app_probe_class_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_application_aware_routing_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_application_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_application_priority_feature_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_application_priority_qos_policy_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_as_path_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_block_url_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24834 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cedge_aaa_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32116 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cedge_global_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cedge_igmp_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cedge_multicast_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18972 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cedge_pim_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cellular_cedge_profile_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cellular_controller_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19127 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cellular_profile_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_centralized_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cflowd_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_banner_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_bfd_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27303 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_bgp_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16189 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_dhcp_server_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_logging_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_ntp_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23164 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_omp_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26037 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_ospf_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55961 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_ospfv3_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_secure_internet_gateway_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14105 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_security_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20567 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_sig_credentials_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11133 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_snmp_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47301 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_system_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_thousandeyes_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25663 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_trustsec_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24735 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_vpn_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   143580 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_vpn_interface_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23074 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_vpn_interface_gre_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39416 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_vpn_interface_ipsec_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15728 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_wireless_lan_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_class_map_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cli_config_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cli_device_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cli_feature_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cli_template_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_color_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_configuration_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_configuration_group_device_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_configuration_group_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_custom_control_topology_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_data_fqdn_prefix_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_data_ipv4_prefix_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_data_ipv6_prefix_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10802 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_dns_security_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_domain_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_eigrp_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_expanded_community_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_extended_community_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_feature_device_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_geo_location_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_gps_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_hub_and_spoke_topology_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_intrusion_prevention_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_ips_signature_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_ipv4_acl_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_ipv4_device_acl_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_ipv4_prefix_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_ipv6_acl_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_ipv6_device_acl_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_ipv6_prefix_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_local_application_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_localized_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_mesh_topology_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_mirror_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_object_group_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_policer_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_port_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_preferred_color_group_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_protocol_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_qos_map_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_region_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_rewrite_rule_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_route_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_rule_set_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_security_app_hosting_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_security_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_service_feature_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58754 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_service_lan_vpn_interface_ethernet_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29738 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_service_lan_vpn_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17338 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_service_tracker_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_site_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_sla_class_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_standard_community_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_switchport_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_aaa_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_banner_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42894 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_basic_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_bfd_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_feature_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_flexible_port_speed_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32106 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_global_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_logging_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_mrf_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_ntp_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42501 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_omp_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_performance_monitoring_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37773 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_remote_access_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12673 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_security_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_snmp_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_tloc_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_tls_ssl_decryption_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10603 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_tls_ssl_profile_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_traffic_data_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_transport_feature_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_transport_ipv6_tracker_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35450 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_transport_management_vpn_interface_ethernet_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_transport_management_vpn_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38737 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_transport_routing_bgp_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)   133799 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_transport_wan_vpn_interface_ethernet_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15881 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_transport_wan_vpn_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11079 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_url_filtering_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vedge_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109443 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_cellular_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118658 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_dsl_ipoe_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110453 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_dsl_pppoa_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117158 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_dsl_pppoe_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116373 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_ethernet_pppoe_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100746 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_multilink_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27775 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_svi_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89903 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_t1_e1_serial_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_membership_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_zone_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39041 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/gps_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16437 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/hub_and_spoke_topology_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24962 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/intrusion_prevention_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/ips_signature_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14507 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/ipv4_acl_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14749 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/ipv4_device_acl_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10218 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/ipv4_prefix_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14507 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/ipv6_acl_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14749 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/ipv6_device_acl_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/ipv6_prefix_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10414 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/local_application_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36302 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/localized_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16008 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/mesh_topology_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11160 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/mirror_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36119 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/object_group_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2702398 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/policer_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/port_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23173 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/preferred_color_group_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/protocol_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/qos_map_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/region_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/rewrite_rule_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/route_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11221 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/rule_set_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/security_app_hosting_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36588 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/security_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/service_feature_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)   209066 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/service_lan_vpn_interface_ethernet_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108249 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/service_lan_vpn_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56467 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/service_tracker_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/site_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29000 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/sla_class_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/standard_community_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30741 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/switchport_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47282 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_aaa_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17728 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_banner_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)   212718 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_basic_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25739 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_bfd_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_feature_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17900 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_flexible_port_speed_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110811 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_global_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33070 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_logging_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27278 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_mrf_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33906 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_ntp_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145714 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_omp_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28150 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_performance_monitoring_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121745 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_remote_access_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40023 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_security_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36694 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_snmp_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/tloc_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50541 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/tls_ssl_decryption_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34035 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/tls_ssl_profile_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14639 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/traffic_data_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/transport_feature_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49582 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/transport_ipv6_tracker_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120607 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/transport_management_vpn_interface_ethernet_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44506 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/transport_management_vpn_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137806 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/transport_routing_bgp_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)   470349 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/transport_wan_vpn_interface_ethernet_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50441 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/transport_wan_vpn_profile_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37387 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/url_filtering_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)   383029 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_cellular_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   413280 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_dsl_ipoe_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   386431 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_dsl_pppoa_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   408281 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_dsl_pppoe_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   404832 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_ethernet_pppoe_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   351150 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_multilink_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101455 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_svi_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)   313094 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_t1_e1_serial_feature_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_list_policy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12255 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_membership_policy_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/zone_list_policy_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:00:10.838577 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-28 08:00:10.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13966 2024-05-28 08:00:10.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:00:10.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 08:00:10.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 08:00:10.000000 pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-28 08:00:04.000000 pulumi_sdwan-0.1.0a1716883043/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:00:10.838577 pulumi_sdwan-0.1.0a1716883043/setup.cfg
```

### Comparing `pulumi_sdwan-0.1.0a1716879684/PKG-INFO` & `pulumi_sdwan-0.1.0a1716883043/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_sdwan
-Version: 0.1.0a1716879684
+Version: 0.1.0a1716883043
 Summary: A Pulumi package for managing resources on Cisco Catalyst SD-WAN.
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pulumi/pulumi-sdwan
 Project-URL: Repository, https://github.com/pulumi/pulumi-sdwan
 Keywords: pulumi,sdwan,category/network
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_sdwan-0.1.0a1716879684/README.md` & `pulumi_sdwan-0.1.0a1716883043/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/__init__.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/_inputs.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/_utilities.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/activate_centralized_policy.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/activate_centralized_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/advanced_inspection_profile_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/advanced_inspection_profile_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/advanced_malware_protection_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/advanced_malware_protection_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/allow_url_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/allow_url_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/app_probe_class_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/app_probe_class_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/application_aware_routing_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/application_aware_routing_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/application_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/application_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/application_priority_feature_profile.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/application_priority_feature_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/application_priority_qos_policy_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/application_priority_qos_policy_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/as_path_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/as_path_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/attach_feature_device_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/attach_feature_device_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/block_url_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/block_url_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cedge_aaa_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cedge_aaa_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cedge_global_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cedge_global_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cedge_igmp_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cedge_igmp_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cedge_multicast_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cedge_multicast_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cedge_pim_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cedge_pim_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cellular_cedge_profile_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cellular_cedge_profile_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cellular_controller_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cellular_controller_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cellular_profile_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cellular_profile_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/centralized_policy.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/centralized_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cflowd_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cflowd_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_banner_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_banner_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_bfd_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_bfd_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_bgp_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_bgp_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_dhcp_server_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_dhcp_server_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_logging_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_logging_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_ntp_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_ntp_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_omp_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_omp_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_ospf_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_ospf_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_ospfv3_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_ospfv3_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_secure_internet_gateway_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_secure_internet_gateway_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_security_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_security_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_sig_credentials_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_sig_credentials_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_snmp_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_snmp_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_system_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_system_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_thousandeyes_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_thousandeyes_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_trustsec_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_trustsec_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_vpn_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_vpn_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_vpn_interface_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_vpn_interface_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_vpn_interface_gre_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_vpn_interface_gre_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_vpn_interface_ipsec_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_vpn_interface_ipsec_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cisco_wireless_lan_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cisco_wireless_lan_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/class_map_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/class_map_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cli_config_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cli_config_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cli_device_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cli_device_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cli_feature_profile.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cli_feature_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/cli_template_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/cli_template_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/color_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/color_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/config/__init__.pyi` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/config/vars.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/configuration_group.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/configuration_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/configuration_group_deploy.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/configuration_group_deploy.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/configuration_group_device_variables.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/configuration_group_device_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/configuration_group_devices.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/configuration_group_devices.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/custom_control_topology_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/custom_control_topology_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/data_fqdn_prefix_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/data_fqdn_prefix_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/data_ipv4_prefix_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/data_ipv4_prefix_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/data_ipv6_prefix_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/data_ipv6_prefix_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/dns_security_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/dns_security_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/domain_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/domain_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/eigrp_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/eigrp_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/expanded_community_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/expanded_community_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/extended_community_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/extended_community_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/feature_device_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/feature_device_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/geo_location_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/geo_location_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_advanced_inspection_profile_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_advanced_inspection_profile_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_advanced_malware_protection_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_advanced_malware_protection_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_allow_url_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_allow_url_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_app_probe_class_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_app_probe_class_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_application_aware_routing_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_application_aware_routing_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_application_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_application_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_application_priority_feature_profile.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_application_priority_feature_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_application_priority_qos_policy_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_application_priority_qos_policy_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_as_path_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_as_path_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_block_url_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_block_url_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cedge_aaa_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cedge_aaa_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cedge_global_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cedge_global_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cedge_igmp_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cedge_igmp_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cedge_multicast_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cedge_multicast_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cedge_pim_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cedge_pim_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cellular_cedge_profile_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cellular_cedge_profile_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cellular_controller_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cellular_controller_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cellular_profile_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cellular_profile_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_centralized_policy.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_centralized_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cflowd_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cflowd_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_banner_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_banner_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_bfd_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_bfd_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_bgp_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_bgp_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_dhcp_server_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_dhcp_server_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_logging_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_logging_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_ntp_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_ntp_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_omp_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_omp_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_ospf_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_ospf_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_ospfv3_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_ospfv3_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_secure_internet_gateway_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_secure_internet_gateway_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_security_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_security_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_sig_credentials_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_sig_credentials_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_snmp_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_snmp_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_system_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_system_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_thousandeyes_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_thousandeyes_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_trustsec_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_trustsec_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_vpn_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_vpn_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_vpn_interface_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_vpn_interface_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_vpn_interface_gre_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_vpn_interface_gre_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_vpn_interface_ipsec_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_vpn_interface_ipsec_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cisco_wireless_lan_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cisco_wireless_lan_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_class_map_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_class_map_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cli_config_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cli_config_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cli_device_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cli_device_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cli_feature_profile.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cli_feature_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_cli_template_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_cli_template_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_color_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_color_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_configuration_group.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_configuration_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_configuration_group_device_variables.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_configuration_group_device_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_configuration_group_devices.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_configuration_group_devices.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_custom_control_topology_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_custom_control_topology_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_data_fqdn_prefix_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_data_fqdn_prefix_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_data_ipv4_prefix_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_data_ipv4_prefix_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_data_ipv6_prefix_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_data_ipv6_prefix_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_device.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_dns_security_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_dns_security_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_domain_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_domain_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_eigrp_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_eigrp_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_expanded_community_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_expanded_community_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_extended_community_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_extended_community_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_feature_device_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_feature_device_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_geo_location_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_geo_location_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_gps_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_gps_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_hub_and_spoke_topology_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_hub_and_spoke_topology_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_intrusion_prevention_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_intrusion_prevention_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_ips_signature_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_ips_signature_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_ipv4_acl_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_ipv4_acl_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_ipv4_device_acl_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_ipv4_device_acl_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_ipv4_prefix_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_ipv4_prefix_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_ipv6_acl_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_ipv6_acl_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_ipv6_device_acl_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_ipv6_device_acl_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_ipv6_prefix_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_ipv6_prefix_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_local_application_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_local_application_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_localized_policy.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_localized_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_mesh_topology_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_mesh_topology_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_mirror_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_mirror_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_object_group_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_object_group_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_policer_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_policer_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_port_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_port_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_preferred_color_group_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_preferred_color_group_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_protocol_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_protocol_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_qos_map_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_qos_map_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_region_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_region_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_rewrite_rule_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_rewrite_rule_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_route_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_route_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_rule_set_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_rule_set_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_security_app_hosting_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_security_app_hosting_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_security_policy.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_service_feature_profile.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_service_feature_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_service_lan_vpn_interface_ethernet_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_service_lan_vpn_interface_ethernet_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_service_lan_vpn_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_service_lan_vpn_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_service_tracker_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_service_tracker_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_site_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_site_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_sla_class_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_sla_class_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_standard_community_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_standard_community_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_switchport_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_switchport_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_aaa_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_aaa_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_banner_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_banner_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_basic_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_basic_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_bfd_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_bfd_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_feature_profile.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_feature_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_flexible_port_speed_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_flexible_port_speed_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_global_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_global_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_logging_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_logging_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_mrf_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_mrf_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_ntp_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_ntp_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_omp_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_omp_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_performance_monitoring_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_performance_monitoring_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_remote_access_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_remote_access_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_security_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_security_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_system_snmp_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_system_snmp_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_tloc_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_tloc_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_tls_ssl_decryption_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_tls_ssl_decryption_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_tls_ssl_profile_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_tls_ssl_profile_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_traffic_data_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_traffic_data_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_transport_feature_profile.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_transport_feature_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_transport_ipv6_tracker_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_transport_ipv6_tracker_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_transport_management_vpn_interface_ethernet_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_transport_management_vpn_interface_ethernet_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_transport_management_vpn_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_transport_management_vpn_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_transport_routing_bgp_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_transport_routing_bgp_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_transport_wan_vpn_interface_ethernet_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_transport_wan_vpn_interface_ethernet_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_transport_wan_vpn_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_transport_wan_vpn_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_url_filtering_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_url_filtering_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vedge_inventory.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vedge_inventory.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_cellular_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_cellular_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_dsl_ipoe_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_dsl_ipoe_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_dsl_pppoa_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_dsl_pppoa_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_dsl_pppoe_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_dsl_pppoe_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_ethernet_pppoe_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_ethernet_pppoe_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_multilink_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_multilink_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_svi_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_svi_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_interface_t1_e1_serial_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_interface_t1_e1_serial_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_vpn_membership_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_vpn_membership_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/get_zone_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/get_zone_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/gps_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/gps_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/hub_and_spoke_topology_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/hub_and_spoke_topology_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/intrusion_prevention_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/intrusion_prevention_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/ips_signature_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/ips_signature_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/ipv4_acl_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/ipv4_acl_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/ipv4_device_acl_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/ipv4_device_acl_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/ipv4_prefix_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/ipv4_prefix_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/ipv6_acl_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/ipv6_acl_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/ipv6_device_acl_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/ipv6_device_acl_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/ipv6_prefix_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/ipv6_prefix_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/local_application_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/local_application_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/localized_policy.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/localized_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/mesh_topology_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/mesh_topology_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/mirror_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/mirror_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/object_group_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/object_group_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/outputs.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/policer_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/policer_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/port_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/port_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/preferred_color_group_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/preferred_color_group_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/protocol_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/protocol_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/provider.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/qos_map_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/qos_map_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/region_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/region_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/rewrite_rule_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/rewrite_rule_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/route_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/route_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/rule_set_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/rule_set_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/security_app_hosting_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/security_app_hosting_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/security_policy.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/service_feature_profile.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/service_feature_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/service_lan_vpn_interface_ethernet_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/service_lan_vpn_interface_ethernet_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/service_lan_vpn_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/service_lan_vpn_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/service_tracker_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/service_tracker_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/site_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/site_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/sla_class_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/sla_class_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/standard_community_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/standard_community_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/switchport_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/switchport_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_aaa_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_aaa_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_banner_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_banner_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_basic_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_basic_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_bfd_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_bfd_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_feature_profile.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_feature_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_flexible_port_speed_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_flexible_port_speed_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_global_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_global_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_logging_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_logging_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_mrf_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_mrf_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_ntp_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_ntp_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_omp_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_omp_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_performance_monitoring_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_performance_monitoring_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_remote_access_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_remote_access_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_security_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_security_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/system_snmp_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/system_snmp_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/tloc_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/tloc_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/tls_ssl_decryption_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/tls_ssl_decryption_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/tls_ssl_profile_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/tls_ssl_profile_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/traffic_data_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/traffic_data_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/transport_feature_profile.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/transport_feature_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/transport_ipv6_tracker_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/transport_ipv6_tracker_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/transport_management_vpn_interface_ethernet_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/transport_management_vpn_interface_ethernet_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/transport_management_vpn_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/transport_management_vpn_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/transport_routing_bgp_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/transport_routing_bgp_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/transport_wan_vpn_interface_ethernet_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/transport_wan_vpn_interface_ethernet_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/transport_wan_vpn_profile_parcel.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/transport_wan_vpn_profile_parcel.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/url_filtering_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/url_filtering_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_cellular_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_cellular_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_dsl_ipoe_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_dsl_ipoe_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_dsl_pppoa_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_dsl_pppoa_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_dsl_pppoe_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_dsl_pppoe_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_ethernet_pppoe_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_ethernet_pppoe_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_multilink_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_multilink_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_svi_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_svi_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_interface_t1_e1_serial_feature_template.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_interface_t1_e1_serial_feature_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/vpn_membership_policy_definition.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/vpn_membership_policy_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan/zone_list_policy_object.py` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan/zone_list_policy_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan.egg-info/PKG-INFO` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_sdwan
-Version: 0.1.0a1716879684
+Version: 0.1.0a1716883043
 Summary: A Pulumi package for managing resources on Cisco Catalyst SD-WAN.
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pulumi/pulumi-sdwan
 Project-URL: Repository, https://github.com/pulumi/pulumi-sdwan
 Keywords: pulumi,sdwan,category/network
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_sdwan-0.1.0a1716879684/pulumi_sdwan.egg-info/SOURCES.txt` & `pulumi_sdwan-0.1.0a1716883043/pulumi_sdwan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_sdwan-0.1.0a1716879684/pyproject.toml` & `pulumi_sdwan-0.1.0a1716883043/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_sdwan"
   description = "A Pulumi package for managing resources on Cisco Catalyst SD-WAN."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "sdwan", "category/network"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.1.0a1716879684"
+  version = "0.1.0a1716883043"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://github.com/pulumi/pulumi-sdwan"
     Repository = "https://github.com/pulumi/pulumi-sdwan"
 
 [build-system]
```

