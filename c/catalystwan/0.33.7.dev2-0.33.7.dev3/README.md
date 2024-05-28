# Comparing `tmp/catalystwan-0.33.7.dev2.tar.gz` & `tmp/catalystwan-0.33.7.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystwan-0.33.7.dev2.tar", max compression
+gzip compressed data, was "catalystwan-0.33.7.dev3.tar", max compression
```

## Comparing `catalystwan-0.33.7.dev2.tar` & `catalystwan-0.33.7.dev3.tar`

### file list

```diff
@@ -1,569 +1,569 @@
--rw-r--r--   0        0        0    11375 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/LICENSE
--rw-r--r--   0        0        0    13533 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/README.md
--rw-r--r--   0        0        0     2558 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/__init__.py
--rw-r--r--   0        0        0     1532 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/abstractions.py
--rw-r--r--   0        0        0        0 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/__init__.py
--rw-r--r--   0        0        0     6689 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/admin_tech_api.py
--rw-r--r--   0        0        0    14935 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/administration.py
--rw-r--r--   0        0        0     6314 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/alarms_api.py
--rw-r--r--   0        0        0     3293 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/api_container.py
--rw-r--r--   0        0        0    11636 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/basic_api.py
--rw-r--r--   0        0        0      386 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/__init__.py
--rw-r--r--   0        0        0     2017 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/builder_factory.py
--rw-r--r--   0        0        0     2679 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/cli.py
--rw-r--r--   0        0        0     2696 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/other.py
--rw-r--r--   0        0        0     3889 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/report.py
--rw-r--r--   0        0        0     8611 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/service.py
--rw-r--r--   0        0        0     2768 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/system.py
--rw-r--r--   0        0        0     8776 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/transport.py
--rw-r--r--   0        0        0     2053 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/config_device_inventory_api.py
--rw-r--r--   0        0        0     4760 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/config_group_api.py
--rw-r--r--   0        0        0     6672 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/configuration_groups/parcel.py
--rw-r--r--   0        0        0     7315 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/dashboard_api.py
--rw-r--r--   0        0        0     7360 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/device_action_api.py
--rw-r--r--   0        0        0    55556 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/feature_profile_api.py
--rw-r--r--   0        0        0     1919 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/logs_api.py
--rw-r--r--   0        0        0     2449 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/monitoring_status_api.py
--rw-r--r--   0        0        0     6036 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/mtt_aaa_api.py
--rw-r--r--   0        0        0     4394 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/omp_api.py
--rw-r--r--   0        0        0     5691 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/packet_capture_api.py
--rw-r--r--   0        0        0     1654 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/parcel_api.py
--rw-r--r--   0        0        0     5600 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/partition_manager_api.py
--rw-r--r--   0        0        0    36861 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/policy_api.py
--rw-r--r--   0        0        0     2284 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/resource_pool_api.py
--rw-r--r--   0        0        0    11320 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/software_action_api.py
--rw-r--r--   0        0        0     5473 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/speedtest_api.py
--rw-r--r--   0        0        0     7149 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/task_status_api.py
--rw-r--r--   0        0        0    30133 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/template_api.py
--rw-r--r--   0        0        0     3540 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/README.md
--rw-r--r--   0        0        0      251 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/bool_str.py
--rw-r--r--   0        0        0     7481 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/cli_template.py
--rw-r--r--   0        0        0     3425 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/device_template/device_template.py
--rw-r--r--   0        0        0      571 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/device_template/device_template_payload.json.j2
--rw-r--r--   0        0        0      137 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/device_variable.py
--rw-r--r--   0        0        0     5029 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/feature_template.py
--rw-r--r--   0        0        0     6576 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/feature_template_field.py
--rw-r--r--   0        0        0      661 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/feature_template_payload.py
--rw-r--r--   0        0        0     3244 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_aaa_model.py
--rw-r--r--   0        0        0      667 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_banner_model.py
--rw-r--r--   0        0        0     2180 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_bfd_model.py
--rw-r--r--   0        0        0    12522 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_bgp_model.py
--rw-r--r--   0        0        0     3436 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_logging_model.py
--rw-r--r--   0        0        0     1584 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_ntp_model.py
--rw-r--r--   0        0        0     3835 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_omp_model.py
--rw-r--r--   0        0        0     6749 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_ospf.py
--rw-r--r--   0        0        0    13901 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_ospfv3.py
--rw-r--r--   0        0        0     9589 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
--rw-r--r--   0        0        0     2581 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_snmp_model.py
--rw-r--r--   0        0        0     8986 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_system.py
--rw-r--r--   0        0        0    21665 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_vpn_interface_model.py
--rw-r--r--   0        0        0    15836 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_vpn_model.py
--rw-r--r--   0        0        0      472 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cli_template.py
--rw-r--r--   0        0        0     1835 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/omp_vsmart_model.py
--rw-r--r--   0        0        0      806 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/security_vsmart_model.py
--rw-r--r--   0        0        0     1882 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/supported.py
--rw-r--r--   0        0        0     2624 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/system_vsmart_model.py
--rw-r--r--   0        0        0     2261 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/aaa_model.py
--rw-r--r--   0        0        0    11178 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
--rw-r--r--   0        0        0     1041 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
--rw-r--r--   0        0        0     4264 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
--rw-r--r--   0        0        0     3735 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
--rw-r--r--   0        0        0     1999 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
--rw-r--r--   0        0        0     2558 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
--rw-r--r--   0        0        0     4547 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
--rw-r--r--   0        0        0     1843 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
--rw-r--r--   0        0        0     2247 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
--rw-r--r--   0        0        0     2098 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
--rw-r--r--   0        0        0      683 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
--rw-r--r--   0        0        0     7113 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/tenant/tenant.json.j2
--rw-r--r--   0        0        0     1460 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/tenant/tenant_model.py
--rw-r--r--   0        0        0     5013 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/tenant_backup_restore_api.py
--rw-r--r--   0        0        0     4406 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/tenant_management_api.py
--rw-r--r--   0        0        0     5090 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/tenant_migration_api.py
--rw-r--r--   0        0        0    13729 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/versions_utils.py
--rw-r--r--   0        0        0    21802 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/dataclasses.py
--rw-r--r--   0        0        0    25624 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/__init__.py
--rw-r--r--   0        0        0    11938 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/administration_user_and_group.py
--rw-r--r--   0        0        0     6731 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/certificate_management_device.py
--rw-r--r--   0        0        0     1476 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/certificate_management_vmanage.py
--rw-r--r--   0        0        0     4035 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/client.py
--rw-r--r--   0        0        0     2722 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/cluster_management.py
--rw-r--r--   0        0        0      983 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/device/software_update.py
--rw-r--r--   0        0        0     9447 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/disaster_recovery.py
--rw-r--r--   0        0        0     3876 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/application_priority.py
--rw-r--r--   0        0        0     2406 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/cli.py
--rw-r--r--   0        0        0     3557 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/dns_security.py
--rw-r--r--   0        0        0     3735 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/embedded_security.py
--rw-r--r--   0        0        0     2600 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py
--rw-r--r--   0        0        0     4419 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
--rw-r--r--   0        0        0     3585 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py
--rw-r--r--   0        0        0     3315 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/sig_security.py
--rw-r--r--   0        0        0    10040 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
--rw-r--r--   0        0        0     3679 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/topology.py
--rw-r--r--   0        0        0     7276 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
--rw-r--r--   0        0        0      442 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/network_hierarchy.py
--rw-r--r--   0        0        0     1361 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/abstractions.py
--rw-r--r--   0        0        0     1969 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
--rw-r--r--   0        0        0     2024 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
--rw-r--r--   0        0        0     2046 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/aip.py
--rw-r--r--   0        0        0     2046 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/amp.py
--rw-r--r--   0        0        0     1756 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/cflowd.py
--rw-r--r--   0        0        0     2025 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/control.py
--rw-r--r--   0        0        0     2170 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/device_access.py
--rw-r--r--   0        0        0     2239 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
--rw-r--r--   0        0        0     1853 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/dns_security.py
--rw-r--r--   0        0        0     2099 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
--rw-r--r--   0        0        0     1995 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/intrusion_prevention.py
--rw-r--r--   0        0        0     1954 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/mesh.py
--rw-r--r--   0        0        0     1991 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/qos_map.py
--rw-r--r--   0        0        0     2065 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/rewrite.py
--rw-r--r--   0        0        0     1798 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/route_policy.py
--rw-r--r--   0        0        0     1967 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/rule_set.py
--rw-r--r--   0        0        0     2092 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/security_group.py
--rw-r--r--   0        0        0     1879 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/ssl_decryption.py
--rw-r--r--   0        0        0     1985 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/ssl_decryption_utd_profile.py
--rw-r--r--   0        0        0     2029 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
--rw-r--r--   0        0        0     1869 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/url_filtering.py
--rw-r--r--   0        0        0     2184 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
--rw-r--r--   0        0        0     2111 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
--rw-r--r--   0        0        0     1740 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/app.py
--rw-r--r--   0        0        0     1900 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/app_probe.py
--rw-r--r--   0        0        0     1793 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/as_path.py
--rw-r--r--   0        0        0     1813 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/class_map.py
--rw-r--r--   0        0        0     1772 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/color.py
--rw-r--r--   0        0        0     1854 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/community.py
--rw-r--r--   0        0        0     1971 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
--rw-r--r--   0        0        0     1873 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/data_prefix.py
--rw-r--r--   0        0        0     2023 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/expanded_community.py
--rw-r--r--   0        0        0     1978 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/extended_community.py
--rw-r--r--   0        0        0     1752 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/fqdn.py
--rw-r--r--   0        0        0     1893 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/geo_location.py
--rw-r--r--   0        0        0     1930 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/ips_signature.py
--rw-r--r--   0        0        0     1873 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
--rw-r--r--   0        0        0     1833 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/local_app.py
--rw-r--r--   0        0        0     1893 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/local_domain.py
--rw-r--r--   0        0        0     1792 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/mirror.py
--rw-r--r--   0        0        0     1817 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/policer.py
--rw-r--r--   0        0        0     1752 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/port.py
--rw-r--r--   0        0        0     2065 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
--rw-r--r--   0        0        0     1852 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/prefix.py
--rw-r--r--   0        0        0     1930 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/protocol_name.py
--rw-r--r--   0        0        0     1683 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/region.py
--rw-r--r--   0        0        0     1892 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/site.py
--rw-r--r--   0        0        0     1782 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/sla.py
--rw-r--r--   0        0        0     1940 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py
--rw-r--r--   0        0        0     1752 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/tloc.py
--rw-r--r--   0        0        0     1872 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/trunkgroup.py
--rw-r--r--   0        0        0     1930 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/umbrella_data.py
--rw-r--r--   0        0        0     1863 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
--rw-r--r--   0        0        0     1863 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/url_block_list.py
--rw-r--r--   0        0        0     1734 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/vpn.py
--rw-r--r--   0        0        0     1752 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/zone.py
--rw-r--r--   0        0        0     1726 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/security_template.py
--rw-r--r--   0        0        0     1738 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/vedge_template.py
--rw-r--r--   0        0        0     2974 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/vsmart_template.py
--rw-r--r--   0        0        0     8865 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/software_actions.py
--rw-r--r--   0        0        0      784 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/topology_group.py
--rw-r--r--   0        0        0     6820 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_dashboard_status.py
--rw-r--r--   0        0        0    10675 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_device_actions.py
--rw-r--r--   0        0        0    13973 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_device_inventory.py
--rw-r--r--   0        0        0      881 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_device_template.py
--rw-r--r--   0        0        0     5287 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_feature_profile.py
--rw-r--r--   0        0        0     6387 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_group.py
--rw-r--r--   0        0        0    27565 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_settings.py
--rw-r--r--   0        0        0    15076 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/endpoints_container.py
--rw-r--r--   0        0        0      760 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/misc.py
--rw-r--r--   0        0        0     8272 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/monitoring/device_details.py
--rw-r--r--   0        0        0      347 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/monitoring/server_info.py
--rw-r--r--   0        0        0     1929 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/monitoring/status.py
--rw-r--r--   0        0        0     1446 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/real_time_monitoring/reboot_history.py
--rw-r--r--   0        0        0     1419 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/sdavc_cloud_connector.py
--rw-r--r--   0        0        0     1047 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/tenant_backup_restore.py
--rw-r--r--   0        0        0     7648 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/tenant_management.py
--rw-r--r--   0        0        0     3649 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/tenant_migration.py
--rw-r--r--   0        0        0     3661 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
--rw-r--r--   0        0        0     6246 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/exceptions.py
--rw-r--r--   0        0        0     1340 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/base.py
--rw-r--r--   0        0        0    16862 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_application_priority.py
--rw-r--r--   0        0        0     2364 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_cli.py
--rw-r--r--   0        0        0     4587 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_dns_security.py
--rw-r--r--   0        0        0     2459 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_extended_community.py
--rw-r--r--   0        0        0     1834 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_other.py
--rw-r--r--   0        0        0    30868 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_service.py
--rw-r--r--   0        0        0    14507 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_sig_security.py
--rw-r--r--   0        0        0    12728 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_system.py
--rw-r--r--   0        0        0    63086 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_transport.py
--rw-r--r--   0        0        0     4124 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/topology/test_topology.py
--rw-r--r--   0        0        0      683 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/profile_builder/base.py
--rw-r--r--   0        0        0     3861 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/profile_builder/test_pb_service.py
--rw-r--r--   0        0        0     2647 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/profile_builder/test_pb_transport.py
--rw-r--r--   0        0        0     1078 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/test_config_migration.py
--rw-r--r--   0        0        0     3803 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/test_data/__init__.py
--rw-r--r--   0        0        0     1902 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/test_find_template_values.py
--rw-r--r--   0        0        0      676 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/logging.conf
--rw-r--r--   0        0        0    16233 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/common.py
--rw-r--r--   0        0        0      194 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/common.py
--rw-r--r--   0        0        0    20593 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/config_migration.py
--rw-r--r--   0        0        0       89 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/docs/README.md
--rw-r--r--   0        0        0   142336 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/docs/diagram.png
--rw-r--r--   0        0        0    10043 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/README.md
--rw-r--r--   0        0        0      663 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/builder.py
--rw-r--r--   0        0        0    28615 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/common.py
--rw-r--r--   0        0        0     5933 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/parcel.py
--rw-r--r--   0        0        0      324 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/acl/__init__.py
--rw-r--r--   0        0        0    12853 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/acl/ipv4acl.py
--rw-r--r--   0        0        0    12379 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/acl/ipv6acl.py
--rw-r--r--   0        0        0     4708 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/application_priority/__init__.py
--rw-r--r--   0        0        0     1385 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/application_priority/policy_settings.py
--rw-r--r--   0        0        0     1572 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/application_priority/qos_policy.py
--rw-r--r--   0        0        0    29351 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/application_priority/traffic_policy.py
--rw-r--r--   0        0        0      292 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/cli/__init__.py
--rw-r--r--   0        0        0      480 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/cli/config.py
--rw-r--r--   0        0        0      275 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/dns_security/__init__.py
--rw-r--r--   0        0        0     2787 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/dns_security/dns.py
--rw-r--r--   0        0        0      507 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/__init__.py
--rw-r--r--   0        0        0    16716 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/ngfirewall.py
--rw-r--r--   0        0        0     4146 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/policy.py
--rw-r--r--   0        0        0      420 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/__init__.py
--rw-r--r--   0        0        0     4750 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py
--rw-r--r--   0        0        0     3950 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py
--rw-r--r--   0        0        0     5327 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
--rw-r--r--   0        0        0     1426 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
--rw-r--r--   0        0        0     1203 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
--rw-r--r--   0        0        0      825 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py
--rw-r--r--   0        0        0      653 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
--rw-r--r--   0        0        0     1244 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
--rw-r--r--   0        0        0      981 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
--rw-r--r--   0        0        0     1305 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/extended_community.py
--rw-r--r--   0        0        0      807 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
--rw-r--r--   0        0        0     1152 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
--rw-r--r--   0        0        0     1706 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
--rw-r--r--   0        0        0     1096 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py
--rw-r--r--   0        0        0     1332 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py
--rw-r--r--   0        0        0     3106 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
--rw-r--r--   0        0        0     1106 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
--rw-r--r--   0        0        0     5255 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
--rw-r--r--   0        0        0     1215 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
--rw-r--r--   0        0        0     1641 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
--rw-r--r--   0        0        0     1485 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/aip.py
--rw-r--r--   0        0        0     1898 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/amp.py
--rw-r--r--   0        0        0     1277 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
--rw-r--r--   0        0        0      871 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
--rw-r--r--   0        0        0      830 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
--rw-r--r--   0        0        0     1288 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
--rw-r--r--   0        0        0     1398 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/intrusion_prevention.py
--rw-r--r--   0        0        0     1604 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
--rw-r--r--   0        0        0      907 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
--rw-r--r--   0        0        0      799 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
--rw-r--r--   0        0        0     1408 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
--rw-r--r--   0        0        0     3388 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption.py
--rw-r--r--   0        0        0     3935 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption_profile.py
--rw-r--r--   0        0        0     1079 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
--rw-r--r--   0        0        0     3679 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url_filtering.py
--rw-r--r--   0        0        0     1461 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
--rw-r--r--   0        0        0      667 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/__init__.py
--rw-r--r--   0        0        0    25515 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/bgp.py
--rw-r--r--   0        0        0     7425 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/ospf.py
--rw-r--r--   0        0        0    12993 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/ospfv3.py
--rw-r--r--   0        0        0     2066 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/__init__.py
--rw-r--r--   0        0        0    10235 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
--rw-r--r--   0        0        0    14485 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
--rw-r--r--   0        0        0     5289 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
--rw-r--r--   0        0        0     4001 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
--rw-r--r--   0        0        0     1349 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
--rw-r--r--   0        0        0    12626 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
--rw-r--r--   0        0        0     6938 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
--rw-r--r--   0        0        0     6350 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
--rw-r--r--   0        0        0     5347 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/multilink.py
--rw-r--r--   0        0        0     8633 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
--rw-r--r--   0        0        0    23869 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
--rw-r--r--   0        0        0    10821 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
--rw-r--r--   0        0        0     3291 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
--rw-r--r--   0        0        0     9187 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
--rw-r--r--   0        0        0     6966 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
--rw-r--r--   0        0        0     5161 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
--rw-r--r--   0        0        0     3705 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
--rw-r--r--   0        0        0     5706 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
--rw-r--r--   0        0        0      297 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/sig_security/__init__.py
--rw-r--r--   0        0        0    16817 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/sig_security/sig_security.py
--rw-r--r--   0        0        0     1287 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py
--rw-r--r--   0        0        0    15436 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
--rw-r--r--   0        0        0      977 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py
--rw-r--r--   0        0        0    10457 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py
--rw-r--r--   0        0        0     2623 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py
--rw-r--r--   0        0        0     6844 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/device_access.py
--rw-r--r--   0        0        0     6847 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/device_access_ipv6.py
--rw-r--r--   0        0        0     6396 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py
--rw-r--r--   0        0        0     6355 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py
--rw-r--r--   0        0        0     2935 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py
--rw-r--r--   0        0        0     3932 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py
--rw-r--r--   0        0        0     5166 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py
--rw-r--r--   0        0        0     6653 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/security.py
--rw-r--r--   0        0        0     6841 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py
--rw-r--r--   0        0        0      726 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/__init__.py
--rw-r--r--   0        0        0    12828 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/custom_control.py
--rw-r--r--   0        0        0     2162 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/hubspoke.py
--rw-r--r--   0        0        0      799 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/mesh.py
--rw-r--r--   0        0        0     2671 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/__init__.py
--rw-r--r--   0        0        0     2298 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
--rw-r--r--   0        0        0     2754 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_profile.py
--rw-r--r--   0        0        0     1579 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/gps.py
--rw-r--r--   0        0        0     5633 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/management/ethernet.py
--rw-r--r--   0        0        0     4400 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/t1e1controller.py
--rw-r--r--   0        0        0    10979 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/vpn.py
--rw-r--r--   0        0        0     9090 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/cellular.py
--rw-r--r--   0        0        0    13993 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ethernet.py
--rw-r--r--   0        0        0     2169 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/gre.py
--rw-r--r--   0        0        0     5137 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ipsec.py
--rw-r--r--   0        0        0    11421 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/multilink.py
--rw-r--r--   0        0        0    16558 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/protocol_over.py
--rw-r--r--   0        0        0     8889 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/t1e1serial.py
--rw-r--r--   0        0        0     2788 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/network_hierarchy.py
--rw-r--r--   0        0        0      157 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/profile_type.py
--rw-r--r--   0        0        0     1073 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/topology_group.py
--rw-r--r--   0        0        0     1041 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/device_inventory.py
--rw-r--r--   0        0        0      341 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/feature_profile_parcel.py
--rw-r--r--   0        0        0      785 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/misc/application_protocols.py
--rw-r--r--   0        0        0      405 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/monitoring/server_info.py
--rw-r--r--   0        0        0    10542 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/__init__.py
--rw-r--r--   0        0        0     8738 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/centralized.py
--rw-r--r--   0        0        0     5789 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/access_control_list.py
--rw-r--r--   0        0        0     5991 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/access_control_list_ipv6.py
--rw-r--r--   0        0        0     2204 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/aip.py
--rw-r--r--   0        0        0     2598 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/amp.py
--rw-r--r--   0        0        0     3159 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/cflowd.py
--rw-r--r--   0        0        0    12158 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/control.py
--rw-r--r--   0        0        0     4134 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/device_access.py
--rw-r--r--   0        0        0     4250 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/device_access_ipv6.py
--rw-r--r--   0        0        0     4585 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/dns_security.py
--rw-r--r--   0        0        0     3251 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/hub_and_spoke.py
--rw-r--r--   0        0        0     2139 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/intrusion_prevention.py
--rw-r--r--   0        0        0     1403 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/mesh.py
--rw-r--r--   0        0        0     3520 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/qos_map.py
--rw-r--r--   0        0        0     1410 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/rewrite.py
--rw-r--r--   0        0        0     6150 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/route_policy.py
--rw-r--r--   0        0        0    12381 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/rule_set.py
--rw-r--r--   0        0        0     3147 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/security_group.py
--rw-r--r--   0        0        0     7992 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/ssl_decryption.py
--rw-r--r--   0        0        0     3539 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/ssl_decryption_utd_profile.py
--rw-r--r--   0        0        0    14018 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/traffic_data.py
--rw-r--r--   0        0        0     2684 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/url_filtering.py
--rw-r--r--   0        0        0     1329 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/vpn_membership.py
--rw-r--r--   0        0        0    10584 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/zone_based_firewall.py
--rw-r--r--   0        0        0     1331 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/app.py
--rw-r--r--   0        0        0     1295 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/app_probe.py
--rw-r--r--   0        0        0      651 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/as_path.py
--rw-r--r--   0        0        0      789 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/class_map.py
--rw-r--r--   0        0        0      661 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/color.py
--rw-r--r--   0        0        0     2634 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/communities.py
--rw-r--r--   0        0        0      918 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/data_ipv6_prefix.py
--rw-r--r--   0        0        0      860 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/data_prefix.py
--rw-r--r--   0        0        0      495 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/fqdn.py
--rw-r--r--   0        0        0     1055 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/geo_location.py
--rw-r--r--   0        0        0      817 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/ips_signature.py
--rw-r--r--   0        0        0     1111 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/ipv6_prefix.py
--rw-r--r--   0        0        0      990 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/local_app.py
--rw-r--r--   0        0        0      923 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/local_domain.py
--rw-r--r--   0        0        0      714 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/mirror.py
--rw-r--r--   0        0        0     1127 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/policer.py
--rw-r--r--   0        0        0      771 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/port.py
--rw-r--r--   0        0        0     3196 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/preferred_color_group.py
--rw-r--r--   0        0        0     1055 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/prefix.py
--rw-r--r--   0        0        0      723 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/protocol_name.py
--rw-r--r--   0        0        0     1325 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/region.py
--rw-r--r--   0        0        0      942 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/site.py
--rw-r--r--   0        0        0     6864 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/sla.py
--rw-r--r--   0        0        0      970 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/threat_grid_api_key.py
--rw-r--r--   0        0        0      960 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/tloc.py
--rw-r--r--   0        0        0     2111 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/trunkgroup.py
--rw-r--r--   0        0        0      824 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/umbrella_data.py
--rw-r--r--   0        0        0      856 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/url.py
--rw-r--r--   0        0        0     1071 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/vpn.py
--rw-r--r--   0        0        0     1405 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/zone.py
--rw-r--r--   0        0        0     6204 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/localized.py
--rw-r--r--   0        0        0     3752 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/policy.py
--rw-r--r--   0        0        0    37132 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/policy_definition.py
--rw-r--r--   0        0        0     1557 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/policy_list.py
--rw-r--r--   0        0        0     9385 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/security.py
--rw-r--r--   0        0        0     2437 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/templates.py
--rw-r--r--   0        0        0     5239 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/tenant.py
--rw-r--r--   0        0        0     9717 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/response.py
--rw-r--r--   0        0        0    19497 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/session.py
--rw-r--r--   0        0        0        0 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/__init__.py
--rw-r--r--   0        0        0     1236 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_converter_chooser.py
--rw-r--r--   0        0        0      629 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/__init__.py
--rw-r--r--   0        0        0     1710 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/dhcp.py
--rw-r--r--   0        0        0    16810 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/interface.py
--rw-r--r--   0        0        0    11799 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/ospfv3.py
--rw-r--r--   0        0        0     3185 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/vpn.py
--rw-r--r--   0        0        0     3583 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_device_template_with_info.py
--rw-r--r--   0        0        0     6139 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_merge_parcels.py
--rw-r--r--   0        0        0     4782 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_normalizer.py
--rw-r--r--   0        0        0    21196 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_transform.py
--rw-r--r--   0        0        0        0 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/models/__init__.py
--rw-r--r--   0        0        0      401 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
--rw-r--r--   0        0        0      513 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/banner_1.json
--rw-r--r--   0        0        0      116 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/alias.json
--rw-r--r--   0        0        0      114 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/basic.json
--rw-r--r--   0        0        0      109 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/basic_no_value.json
--rw-r--r--   0        0        0      848 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/children.json
--rw-r--r--   0        0        0     2348 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/children_nested.json
--rw-r--r--   0        0        0     2348 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      274 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/data_path.json
--rw-r--r--   0        0        0     2973 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/cisco_bfd.json
--rw-r--r--   0        0        0    11100 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/complex_aaa.json
--rw-r--r--   0        0        0    41165 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
--rw-r--r--   0        0        0     5219 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/default_cisco_system.json
--rw-r--r--   0        0        0     5505 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/iuo.json
--rw-r--r--   0        0        0      249 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/omp_1.json
--rw-r--r--   0        0        0      875 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/omp_2.json
--rw-r--r--   0        0        0     1682 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/omp_3.json
--rw-r--r--   0        0        0      662 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/__init__.py
--rw-r--r--   0        0        0     2828 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_aaa.py
--rw-r--r--   0        0        0      303 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_banner.py
--rw-r--r--   0        0        0      587 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_bfd.py
--rw-r--r--   0        0        0      344 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_system.py
--rw-r--r--   0        0        0     8078 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_vpn.py
--rw-r--r--   0        0        0     1091 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/omp_vsmart.py
--rw-r--r--   0        0        0      605 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/alias.json
--rw-r--r--   0        0        0      574 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/basic.json
--rw-r--r--   0        0        0     1810 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/children.json
--rw-r--r--   0        0        0     4005 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/children_nested.json
--rw-r--r--   0        0        0     4005 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      731 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/data_path.json
--rw-r--r--   0        0        0    43436 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cedge_aaa.json
--rw-r--r--   0        0        0     1200 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_banner.json
--rw-r--r--   0        0        0     9495 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_bfd.json
--rw-r--r--   0        0        0    99045 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_system.json
--rw-r--r--   0        0        0    87854 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_vpn.json
--rw-r--r--   0        0        0     5939 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/omp-vsmart.json
--rw-r--r--   0        0        0     1381 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_chose_model.py
--rw-r--r--   0        0        0     2598 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_deserialize_model.py
--rw-r--r--   0        0        0     6762 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_find_template_values_2.py
--rw-r--r--   0        0        0     4598 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_generate_payload.py
--rw-r--r--   0        0        0     1755 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_serialize_model.py
--rw-r--r--   0        0        0     8145 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_admin_tech_api.py
--rw-r--r--   0        0        0    17792 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_administration.py
--rw-r--r--   0        0        0    11116 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_alarms_api.py
--rw-r--r--   0        0        0     8322 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_cli_template.py
--rw-r--r--   0        0        0     5494 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_creation_tools.py
--rw-r--r--   0        0        0     3981 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_device_action_api.py
--rw-r--r--   0        0        0    28159 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_devices_api.py
--rw-r--r--   0        0        0    34991 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_endpoints.py
--rw-r--r--   0        0        0     1897 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_extended_community_converter.py
--rw-r--r--   0        0        0    10767 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_feature_profile_api.py
--rw-r--r--   0        0        0      894 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_feature_template_field.py
--rw-r--r--   0        0        0     1545 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_logs_api.py
--rw-r--r--   0        0        0     1007 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_mirror_converter.py
--rw-r--r--   0        0        0     1899 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_models_common.py
--rw-r--r--   0        0        0     1809 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_monitoring_server_info.py
--rw-r--r--   0        0        0     5489 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_monitoring_status_api.py
--rw-r--r--   0        0        0    11026 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_mtt_aaa_api.py
--rw-r--r--   0        0        0    10026 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_normalize_to_model_definition.py
--rw-r--r--   0        0        0    16472 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_omp_api.py
--rw-r--r--   0        0        0     5223 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_packet_capture.py
--rw-r--r--   0        0        0     5727 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_partition_manager_api.py
--rw-r--r--   0        0        0     7926 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_response.py
--rw-r--r--   0        0        0     6724 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_session.py
--rw-r--r--   0        0        0     7117 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_software_action_api.py
--rw-r--r--   0        0        0     6071 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_speed_test_api.py
--rw-r--r--   0        0        0    14926 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_task_status_api.py
--rw-r--r--   0        0        0    15055 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_templates.py
--rw-r--r--   0        0        0     3705 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_tenant_backup_restore_api.py
--rw-r--r--   0        0        0     6114 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_tenant_management_api.py
--rw-r--r--   0        0        0     4506 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_tenant_migration_api.py
--rw-r--r--   0        0        0    12377 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_typed_list.py
--rw-r--r--   0        0        0     2968 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_version.py
--rw-r--r--   0        0        0    10377 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_version_utils.py
--rw-r--r--   0        0        0     3343 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_vmanage_auth.py
--rw-r--r--   0        0        0     9379 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/typed_list.py
--rw-r--r--   0        0        0        0 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/__init__.py
--rw-r--r--   0        0        0      266 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/alarm_status.py
--rw-r--r--   0        0        0      253 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/certificate_status.py
--rw-r--r--   0        0        0      279 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/colors.py
--rw-r--r--   0        0        0      239 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/exceptions.py
--rw-r--r--   0        0        0      320 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/__init__.py
--rw-r--r--   0        0        0     3433 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/aaa.py
--rw-r--r--   0        0        0     5810 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/appqoe.py
--rw-r--r--   0        0        0      784 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/banner.py
--rw-r--r--   0        0        0      268 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/base.py
--rw-r--r--   0        0        0     3283 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/basic.py
--rw-r--r--   0        0        0      898 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/bfd.py
--rw-r--r--   0        0        0     9266 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/bgp.py
--rw-r--r--   0        0        0     1765 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cellular_controller.py
--rw-r--r--   0        0        0     3269 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cellular_profile.py
--rw-r--r--   0        0        0      756 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cli.py
--rw-r--r--   0        0        0     1932 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cloud_credentials.py
--rw-r--r--   0        0        0     4566 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/dhcp.py
--rw-r--r--   0        0        0     5349 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/eigrp.py
--rw-r--r--   0        0        0     6334 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ethernet.py
--rw-r--r--   0        0        0      578 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/global_.py
--rw-r--r--   0        0        0     1573 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/gps.py
--rw-r--r--   0        0        0      331 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/helpers.py
--rw-r--r--   0        0        0    13128 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/ethernet.py
--rw-r--r--   0        0        0     5619 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/gre.py
--rw-r--r--   0        0        0     5959 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/ipsec.py
--rw-r--r--   0        0        0     9349 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/multilink.py
--rw-r--r--   0        0        0     7411 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/svi.py
--rw-r--r--   0        0        0     1963 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/logging_.py
--rw-r--r--   0        0        0     4855 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/model_definition_normalizer.py
--rw-r--r--   0        0        0    13085 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/multicast.py
--rw-r--r--   0        0        0     5470 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/normalizer.py
--rw-r--r--   0        0        0     2295 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ntp.py
--rw-r--r--   0        0        0     1475 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/omp.py
--rw-r--r--   0        0        0     5684 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ospf.py
--rw-r--r--   0        0        0    11458 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ospfv3.py
--rw-r--r--   0        0        0     6251 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/parcel_factory.py
--rw-r--r--   0        0        0     1568 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/security.py
--rw-r--r--   0        0        0    10159 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/sig.py
--rw-r--r--   0        0        0     2240 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/snmp.py
--rw-r--r--   0        0        0     9032 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/switchport.py
--rw-r--r--   0        0        0     2776 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py
--rw-r--r--   0        0        0     2250 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ucse.py
--rw-r--r--   0        0        0    31317 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/vpn.py
--rw-r--r--   0        0        0     5742 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/cellular.py
--rw-r--r--   0        0        0    13497 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/ethernet.py
--rw-r--r--   0        0        0     4844 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/gre.py
--rw-r--r--   0        0        0     6866 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/ipsec.py
--rw-r--r--   0        0        0    14360 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/multilink.py
--rw-r--r--   0        0        0    18190 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/protocol_over.py
--rw-r--r--   0        0        0     5344 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/t1e1serial.py
--rw-r--r--   0        0        0     8057 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wireless_lan.py
--rw-r--r--   0        0        0     7722 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/policy/policy_definitions.py
--rw-r--r--   0        0        0    14226 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/policy/policy_lists.py
--rw-r--r--   0        0        0      165 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/utils.py
--rw-r--r--   0        0        0    12777 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/creators/config_pusher.py
--rw-r--r--   0        0        0     8511 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/creators/strategy/parcels.py
--rw-r--r--   0        0        0     1760 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/factories/feature_profile_api.py
--rw-r--r--   0        0        0     1257 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/factories/parcel_pusher.py
--rw-r--r--   0        0        0     3464 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/reverters/config_reverter.py
--rw-r--r--   0        0        0        0 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/steps/__init__.py
--rw-r--r--   0        0        0     3767 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/steps/constants.py
--rw-r--r--   0        0        0     9821 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/steps/transform.py
--rw-r--r--   0        0        0      154 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_status.py
--rw-r--r--   0        0        0     4778 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/creation_tools.py
--rw-r--r--   0        0        0     7281 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/dashboard.py
--rw-r--r--   0        0        0     2863 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/device_model.py
--rw-r--r--   0        0        0     2110 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/dict.py
--rw-r--r--   0        0        0      953 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/feature_template/choose_model.py
--rw-r--r--   0        0        0     4882 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/feature_template/find_template_values.py
--rw-r--r--   0        0        0     1173 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/model.py
--rw-r--r--   0        0        0      584 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/operation_status.py
--rw-r--r--   0        0        0      196 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/personality.py
--rw-r--r--   0        0        0      360 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/pydantic_field.py
--rw-r--r--   0        0        0      172 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/reachability.py
--rw-r--r--   0        0        0      407 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/session_type.py
--rw-r--r--   0        0        0      149 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/template_type.py
--rw-r--r--   0        0        0     9825 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/timezone.py
--rw-r--r--   0        0        0      449 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/type_check.py
--rw-r--r--   0        0        0     3930 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/upgrades_helper.py
--rw-r--r--   0        0        0      159 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/validate_status.py
--rw-r--r--   0        0        0     3032 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/version.py
--rw-r--r--   0        0        0     5415 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/vmanage_auth.py
--rw-r--r--   0        0        0    20653 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/workflows/config_migration.py
--rw-r--r--   0        0        0     9946 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/workflows/tenant_migration.py
--rw-r--r--   0        0        0      866 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/pyproject.toml
--rw-r--r--   0        0        0    18941 1970-01-01 00:00:00.000000 catalystwan-0.33.7.dev2/setup.py
--rw-r--r--   0        0        0    14665 1970-01-01 00:00:00.000000 catalystwan-0.33.7.dev2/PKG-INFO
+-rw-r--r--   0        0        0    11375 2024-05-28 12:42:55.737484 catalystwan-0.33.7.dev3/LICENSE
+-rw-r--r--   0        0        0    13533 2024-05-28 12:42:55.737484 catalystwan-0.33.7.dev3/README.md
+-rw-r--r--   0        0        0     2558 2024-05-28 12:42:55.737484 catalystwan-0.33.7.dev3/catalystwan/__init__.py
+-rw-r--r--   0        0        0     1532 2024-05-28 12:42:55.737484 catalystwan-0.33.7.dev3/catalystwan/abstractions.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/__init__.py
+-rw-r--r--   0        0        0     6689 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/admin_tech_api.py
+-rw-r--r--   0        0        0    14935 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/administration.py
+-rw-r--r--   0        0        0     6314 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/alarms_api.py
+-rw-r--r--   0        0        0     3293 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/api_container.py
+-rw-r--r--   0        0        0    11636 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/basic_api.py
+-rw-r--r--   0        0        0      386 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/builders/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/__init__.py
+-rw-r--r--   0        0        0     2017 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/builder_factory.py
+-rw-r--r--   0        0        0     2679 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/cli.py
+-rw-r--r--   0        0        0     2696 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/other.py
+-rw-r--r--   0        0        0     3889 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/report.py
+-rw-r--r--   0        0        0     8611 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/service.py
+-rw-r--r--   0        0        0     2768 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/system.py
+-rw-r--r--   0        0        0     8776 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/transport.py
+-rw-r--r--   0        0        0     2053 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/config_device_inventory_api.py
+-rw-r--r--   0        0        0     4760 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/config_group_api.py
+-rw-r--r--   0        0        0     6672 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/configuration_groups/parcel.py
+-rw-r--r--   0        0        0     7315 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/dashboard_api.py
+-rw-r--r--   0        0        0     7360 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/device_action_api.py
+-rw-r--r--   0        0        0    55821 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/feature_profile_api.py
+-rw-r--r--   0        0        0     1919 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/logs_api.py
+-rw-r--r--   0        0        0     2449 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/monitoring_status_api.py
+-rw-r--r--   0        0        0     6036 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/mtt_aaa_api.py
+-rw-r--r--   0        0        0     4394 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/omp_api.py
+-rw-r--r--   0        0        0     5691 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/packet_capture_api.py
+-rw-r--r--   0        0        0     1654 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/parcel_api.py
+-rw-r--r--   0        0        0     5600 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/partition_manager_api.py
+-rw-r--r--   0        0        0    36861 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/policy_api.py
+-rw-r--r--   0        0        0     2284 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/resource_pool_api.py
+-rw-r--r--   0        0        0    11320 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/software_action_api.py
+-rw-r--r--   0        0        0     5473 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/speedtest_api.py
+-rw-r--r--   0        0        0     7149 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/task_status_api.py
+-rw-r--r--   0        0        0    30133 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/template_api.py
+-rw-r--r--   0        0        0     3540 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/README.md
+-rw-r--r--   0        0        0      251 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/bool_str.py
+-rw-r--r--   0        0        0     7481 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/cli_template.py
+-rw-r--r--   0        0        0     3425 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/device_template/device_template.py
+-rw-r--r--   0        0        0      571 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/device_template/device_template_payload.json.j2
+-rw-r--r--   0        0        0      137 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/device_variable.py
+-rw-r--r--   0        0        0     5029 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/feature_template.py
+-rw-r--r--   0        0        0     6576 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/feature_template_field.py
+-rw-r--r--   0        0        0      661 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/feature_template_payload.py
+-rw-r--r--   0        0        0     3244 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_aaa_model.py
+-rw-r--r--   0        0        0      667 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_banner_model.py
+-rw-r--r--   0        0        0     2180 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_bfd_model.py
+-rw-r--r--   0        0        0    12522 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_bgp_model.py
+-rw-r--r--   0        0        0     3436 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_logging_model.py
+-rw-r--r--   0        0        0     1584 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_ntp_model.py
+-rw-r--r--   0        0        0     3835 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_omp_model.py
+-rw-r--r--   0        0        0     6749 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_ospf.py
+-rw-r--r--   0        0        0    13901 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_ospfv3.py
+-rw-r--r--   0        0        0     9589 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
+-rw-r--r--   0        0        0     2581 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_snmp_model.py
+-rw-r--r--   0        0        0     8986 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_system.py
+-rw-r--r--   0        0        0    21665 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_vpn_interface_model.py
+-rw-r--r--   0        0        0    15836 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_vpn_model.py
+-rw-r--r--   0        0        0      472 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cli_template.py
+-rw-r--r--   0        0        0     1835 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/omp_vsmart_model.py
+-rw-r--r--   0        0        0      806 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/security_vsmart_model.py
+-rw-r--r--   0        0        0     1882 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/supported.py
+-rw-r--r--   0        0        0     2624 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/models/system_vsmart_model.py
+-rw-r--r--   0        0        0     2261 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/aaa/aaa_model.py
+-rw-r--r--   0        0        0    11178 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
+-rw-r--r--   0        0        0     1041 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
+-rw-r--r--   0        0        0     4264 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
+-rw-r--r--   0        0        0     3735 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
+-rw-r--r--   0        0        0     1999 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
+-rw-r--r--   0        0        0     2558 2024-05-28 12:42:55.741484 catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
+-rw-r--r--   0        0        0     4547 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
+-rw-r--r--   0        0        0     1843 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
+-rw-r--r--   0        0        0     2247 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
+-rw-r--r--   0        0        0     2098 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
+-rw-r--r--   0        0        0      683 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
+-rw-r--r--   0        0        0     7113 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/tenant/tenant.json.j2
+-rw-r--r--   0        0        0     1460 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/tenant/tenant_model.py
+-rw-r--r--   0        0        0     5013 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/api/tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     4406 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/api/tenant_management_api.py
+-rw-r--r--   0        0        0     5090 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/api/tenant_migration_api.py
+-rw-r--r--   0        0        0    13729 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/api/versions_utils.py
+-rw-r--r--   0        0        0    21802 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/dataclasses.py
+-rw-r--r--   0        0        0    25624 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/__init__.py
+-rw-r--r--   0        0        0    11938 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/administration_user_and_group.py
+-rw-r--r--   0        0        0     6731 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/certificate_management_device.py
+-rw-r--r--   0        0        0     1476 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/certificate_management_vmanage.py
+-rw-r--r--   0        0        0     4035 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/client.py
+-rw-r--r--   0        0        0     2722 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/cluster_management.py
+-rw-r--r--   0        0        0      983 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/device/software_update.py
+-rw-r--r--   0        0        0     9447 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/disaster_recovery.py
+-rw-r--r--   0        0        0     3873 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/application_priority.py
+-rw-r--r--   0        0        0     2404 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/cli.py
+-rw-r--r--   0        0        0     3554 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/dns_security.py
+-rw-r--r--   0        0        0     3732 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/embedded_security.py
+-rw-r--r--   0        0        0     2598 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py
+-rw-r--r--   0        0        0     4927 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
+-rw-r--r--   0        0        0     3583 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py
+-rw-r--r--   0        0        0     3315 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/sig_security.py
+-rw-r--r--   0        0        0    10038 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
+-rw-r--r--   0        0        0     3676 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/topology.py
+-rw-r--r--   0        0        0     7258 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
+-rw-r--r--   0        0        0      442 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/network_hierarchy.py
+-rw-r--r--   0        0        0     1361 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/abstractions.py
+-rw-r--r--   0        0        0     1969 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
+-rw-r--r--   0        0        0     2024 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
+-rw-r--r--   0        0        0     2046 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/aip.py
+-rw-r--r--   0        0        0     2046 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/amp.py
+-rw-r--r--   0        0        0     1756 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/cflowd.py
+-rw-r--r--   0        0        0     2025 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/control.py
+-rw-r--r--   0        0        0     2170 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/device_access.py
+-rw-r--r--   0        0        0     2239 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
+-rw-r--r--   0        0        0     1853 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/dns_security.py
+-rw-r--r--   0        0        0     2099 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
+-rw-r--r--   0        0        0     1995 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/intrusion_prevention.py
+-rw-r--r--   0        0        0     1954 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/mesh.py
+-rw-r--r--   0        0        0     1991 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/qos_map.py
+-rw-r--r--   0        0        0     2065 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/rewrite.py
+-rw-r--r--   0        0        0     1798 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/route_policy.py
+-rw-r--r--   0        0        0     1967 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/rule_set.py
+-rw-r--r--   0        0        0     2092 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/security_group.py
+-rw-r--r--   0        0        0     1879 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/ssl_decryption.py
+-rw-r--r--   0        0        0     1985 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/ssl_decryption_utd_profile.py
+-rw-r--r--   0        0        0     2029 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
+-rw-r--r--   0        0        0     1869 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/url_filtering.py
+-rw-r--r--   0        0        0     2184 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
+-rw-r--r--   0        0        0     2111 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
+-rw-r--r--   0        0        0     1740 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/app.py
+-rw-r--r--   0        0        0     1900 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/app_probe.py
+-rw-r--r--   0        0        0     1793 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/as_path.py
+-rw-r--r--   0        0        0     1813 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/class_map.py
+-rw-r--r--   0        0        0     1772 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/color.py
+-rw-r--r--   0        0        0     1854 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/community.py
+-rw-r--r--   0        0        0     1971 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
+-rw-r--r--   0        0        0     1873 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/data_prefix.py
+-rw-r--r--   0        0        0     2023 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/expanded_community.py
+-rw-r--r--   0        0        0     1978 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/extended_community.py
+-rw-r--r--   0        0        0     1752 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/fqdn.py
+-rw-r--r--   0        0        0     1893 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/geo_location.py
+-rw-r--r--   0        0        0     1930 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/ips_signature.py
+-rw-r--r--   0        0        0     1873 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
+-rw-r--r--   0        0        0     1833 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/local_app.py
+-rw-r--r--   0        0        0     1893 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/local_domain.py
+-rw-r--r--   0        0        0     1792 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/mirror.py
+-rw-r--r--   0        0        0     1817 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/policer.py
+-rw-r--r--   0        0        0     1752 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/port.py
+-rw-r--r--   0        0        0     2065 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
+-rw-r--r--   0        0        0     1852 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/prefix.py
+-rw-r--r--   0        0        0     1930 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/protocol_name.py
+-rw-r--r--   0        0        0     1683 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/region.py
+-rw-r--r--   0        0        0     1892 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/site.py
+-rw-r--r--   0        0        0     1782 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/sla.py
+-rw-r--r--   0        0        0     1940 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py
+-rw-r--r--   0        0        0     1752 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/tloc.py
+-rw-r--r--   0        0        0     1872 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/trunkgroup.py
+-rw-r--r--   0        0        0     1930 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/umbrella_data.py
+-rw-r--r--   0        0        0     1863 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
+-rw-r--r--   0        0        0     1863 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/url_block_list.py
+-rw-r--r--   0        0        0     1734 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/vpn.py
+-rw-r--r--   0        0        0     1752 2024-05-28 12:42:55.745484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/zone.py
+-rw-r--r--   0        0        0     1726 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/security_template.py
+-rw-r--r--   0        0        0     1738 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/vedge_template.py
+-rw-r--r--   0        0        0     2974 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/vsmart_template.py
+-rw-r--r--   0        0        0     8865 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/software_actions.py
+-rw-r--r--   0        0        0      784 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/topology_group.py
+-rw-r--r--   0        0        0     6820 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration_dashboard_status.py
+-rw-r--r--   0        0        0    10675 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration_device_actions.py
+-rw-r--r--   0        0        0    13973 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration_device_inventory.py
+-rw-r--r--   0        0        0      881 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration_device_template.py
+-rw-r--r--   0        0        0     5287 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration_feature_profile.py
+-rw-r--r--   0        0        0     6387 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration_group.py
+-rw-r--r--   0        0        0    27565 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration_settings.py
+-rw-r--r--   0        0        0    15076 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/endpoints_container.py
+-rw-r--r--   0        0        0      760 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/misc.py
+-rw-r--r--   0        0        0     8272 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/monitoring/device_details.py
+-rw-r--r--   0        0        0      347 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/monitoring/server_info.py
+-rw-r--r--   0        0        0     1929 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/monitoring/status.py
+-rw-r--r--   0        0        0     1446 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/real_time_monitoring/reboot_history.py
+-rw-r--r--   0        0        0     1419 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/sdavc_cloud_connector.py
+-rw-r--r--   0        0        0     1047 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/tenant_backup_restore.py
+-rw-r--r--   0        0        0     7648 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/tenant_management.py
+-rw-r--r--   0        0        0     3649 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/tenant_migration.py
+-rw-r--r--   0        0        0     3661 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
+-rw-r--r--   0        0        0     6246 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/exceptions.py
+-rw-r--r--   0        0        0     1340 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/base.py
+-rw-r--r--   0        0        0    16862 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_application_priority.py
+-rw-r--r--   0        0        0     2364 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_cli.py
+-rw-r--r--   0        0        0     4587 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_dns_security.py
+-rw-r--r--   0        0        0     2459 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_extended_community.py
+-rw-r--r--   0        0        0     1834 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_other.py
+-rw-r--r--   0        0        0    30868 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_service.py
+-rw-r--r--   0        0        0    14507 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_sig_security.py
+-rw-r--r--   0        0        0    12728 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_system.py
+-rw-r--r--   0        0        0    63086 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_transport.py
+-rw-r--r--   0        0        0     4124 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/topology/test_topology.py
+-rw-r--r--   0        0        0      683 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/profile_builder/base.py
+-rw-r--r--   0        0        0     3861 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/profile_builder/test_pb_service.py
+-rw-r--r--   0        0        0     2647 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/profile_builder/test_pb_transport.py
+-rw-r--r--   0        0        0     1078 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/test_config_migration.py
+-rw-r--r--   0        0        0     3803 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/test_data/__init__.py
+-rw-r--r--   0        0        0     1902 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/integration_tests/test_find_template_values.py
+-rw-r--r--   0        0        0      676 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/logging.conf
+-rw-r--r--   0        0        0    16233 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/models/common.py
+-rw-r--r--   0        0        0      194 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/common.py
+-rw-r--r--   0        0        0    20541 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/config_migration.py
+-rw-r--r--   0        0        0       89 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/docs/README.md
+-rw-r--r--   0        0        0   142336 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/docs/diagram.png
+-rw-r--r--   0        0        0    10043 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/README.md
+-rw-r--r--   0        0        0      663 2024-05-28 12:42:55.749484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/builder.py
+-rw-r--r--   0        0        0    28613 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/common.py
+-rw-r--r--   0        0        0     5933 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/parcel.py
+-rw-r--r--   0        0        0      324 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/acl/__init__.py
+-rw-r--r--   0        0        0    12853 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/acl/ipv4acl.py
+-rw-r--r--   0        0        0    12379 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/acl/ipv6acl.py
+-rw-r--r--   0        0        0     4708 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/application_priority/__init__.py
+-rw-r--r--   0        0        0     1385 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/application_priority/policy_settings.py
+-rw-r--r--   0        0        0     1572 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/application_priority/qos_policy.py
+-rw-r--r--   0        0        0    29351 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/application_priority/traffic_policy.py
+-rw-r--r--   0        0        0      292 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/cli/__init__.py
+-rw-r--r--   0        0        0      480 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/cli/config.py
+-rw-r--r--   0        0        0      275 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/dns_security/__init__.py
+-rw-r--r--   0        0        0     2787 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/dns_security/dns.py
+-rw-r--r--   0        0        0      507 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/__init__.py
+-rw-r--r--   0        0        0    16716 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/ngfirewall.py
+-rw-r--r--   0        0        0     4146 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/policy.py
+-rw-r--r--   0        0        0      420 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/other/__init__.py
+-rw-r--r--   0        0        0     4750 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py
+-rw-r--r--   0        0        0     3950 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py
+-rw-r--r--   0        0        0     5327 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
+-rw-r--r--   0        0        0     1426 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
+-rw-r--r--   0        0        0     1203 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
+-rw-r--r--   0        0        0      825 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py
+-rw-r--r--   0        0        0      653 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
+-rw-r--r--   0        0        0     1244 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
+-rw-r--r--   0        0        0      981 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
+-rw-r--r--   0        0        0     1305 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/extended_community.py
+-rw-r--r--   0        0        0      807 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
+-rw-r--r--   0        0        0     1152 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
+-rw-r--r--   0        0        0     1706 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
+-rw-r--r--   0        0        0     1096 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py
+-rw-r--r--   0        0        0     1332 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py
+-rw-r--r--   0        0        0     3106 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
+-rw-r--r--   0        0        0     1106 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
+-rw-r--r--   0        0        0     5255 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
+-rw-r--r--   0        0        0     1215 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
+-rw-r--r--   0        0        0     1641 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
+-rw-r--r--   0        0        0     1485 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/aip.py
+-rw-r--r--   0        0        0     1898 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/amp.py
+-rw-r--r--   0        0        0     1277 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
+-rw-r--r--   0        0        0      871 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
+-rw-r--r--   0        0        0      830 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
+-rw-r--r--   0        0        0     1288 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
+-rw-r--r--   0        0        0     1398 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/intrusion_prevention.py
+-rw-r--r--   0        0        0     1604 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
+-rw-r--r--   0        0        0      907 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
+-rw-r--r--   0        0        0      799 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
+-rw-r--r--   0        0        0     1408 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
+-rw-r--r--   0        0        0     3388 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption.py
+-rw-r--r--   0        0        0     3935 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption_profile.py
+-rw-r--r--   0        0        0     1079 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
+-rw-r--r--   0        0        0     3679 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url_filtering.py
+-rw-r--r--   0        0        0     1461 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
+-rw-r--r--   0        0        0      667 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/routing/__init__.py
+-rw-r--r--   0        0        0    25515 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/routing/bgp.py
+-rw-r--r--   0        0        0     7425 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/routing/ospf.py
+-rw-r--r--   0        0        0    12993 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/routing/ospfv3.py
+-rw-r--r--   0        0        0     2066 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/__init__.py
+-rw-r--r--   0        0        0    10235 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
+-rw-r--r--   0        0        0    14485 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
+-rw-r--r--   0        0        0     5289 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
+-rw-r--r--   0        0        0     4001 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
+-rw-r--r--   0        0        0     1349 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
+-rw-r--r--   0        0        0    12626 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
+-rw-r--r--   0        0        0     6938 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
+-rw-r--r--   0        0        0     6350 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
+-rw-r--r--   0        0        0     5347 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/lan/multilink.py
+-rw-r--r--   0        0        0     8633 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
+-rw-r--r--   0        0        0    23869 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
+-rw-r--r--   0        0        0    10821 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
+-rw-r--r--   0        0        0     3291 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
+-rw-r--r--   0        0        0     9187 2024-05-28 12:42:55.753484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
+-rw-r--r--   0        0        0     6966 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
+-rw-r--r--   0        0        0     5161 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
+-rw-r--r--   0        0        0     3705 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
+-rw-r--r--   0        0        0     5706 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
+-rw-r--r--   0        0        0      297 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/sig_security/__init__.py
+-rw-r--r--   0        0        0    16817 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/sig_security/sig_security.py
+-rw-r--r--   0        0        0     1287 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py
+-rw-r--r--   0        0        0    15436 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
+-rw-r--r--   0        0        0      977 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py
+-rw-r--r--   0        0        0    10457 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py
+-rw-r--r--   0        0        0     2623 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py
+-rw-r--r--   0        0        0     6844 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/device_access.py
+-rw-r--r--   0        0        0     6847 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/device_access_ipv6.py
+-rw-r--r--   0        0        0     6396 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py
+-rw-r--r--   0        0        0     6355 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py
+-rw-r--r--   0        0        0     2935 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py
+-rw-r--r--   0        0        0     3932 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py
+-rw-r--r--   0        0        0     5166 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py
+-rw-r--r--   0        0        0     6653 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/security.py
+-rw-r--r--   0        0        0     6841 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py
+-rw-r--r--   0        0        0      726 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/topology/__init__.py
+-rw-r--r--   0        0        0    12828 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/topology/custom_control.py
+-rw-r--r--   0        0        0     2162 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/topology/hubspoke.py
+-rw-r--r--   0        0        0      799 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/topology/mesh.py
+-rw-r--r--   0        0        0     2671 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/__init__.py
+-rw-r--r--   0        0        0     2298 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
+-rw-r--r--   0        0        0     2754 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_profile.py
+-rw-r--r--   0        0        0     1579 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/gps.py
+-rw-r--r--   0        0        0     5633 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/management/ethernet.py
+-rw-r--r--   0        0        0     4400 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/t1e1controller.py
+-rw-r--r--   0        0        0    10979 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/vpn.py
+-rw-r--r--   0        0        0     9090 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/cellular.py
+-rw-r--r--   0        0        0    13993 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ethernet.py
+-rw-r--r--   0        0        0     2169 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/gre.py
+-rw-r--r--   0        0        0     5137 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ipsec.py
+-rw-r--r--   0        0        0    11421 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/multilink.py
+-rw-r--r--   0        0        0    16558 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/protocol_over.py
+-rw-r--r--   0        0        0     8889 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/t1e1serial.py
+-rw-r--r--   0        0        0     2788 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/network_hierarchy.py
+-rw-r--r--   0        0        0      157 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/profile_type.py
+-rw-r--r--   0        0        0     1073 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/configuration/topology_group.py
+-rw-r--r--   0        0        0     1041 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/device_inventory.py
+-rw-r--r--   0        0        0      341 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/feature_profile_parcel.py
+-rw-r--r--   0        0        0      785 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/misc/application_protocols.py
+-rw-r--r--   0        0        0      405 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/monitoring/server_info.py
+-rw-r--r--   0        0        0    10542 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/__init__.py
+-rw-r--r--   0        0        0     8738 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/centralized.py
+-rw-r--r--   0        0        0     5789 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/access_control_list.py
+-rw-r--r--   0        0        0     5991 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/access_control_list_ipv6.py
+-rw-r--r--   0        0        0     2204 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/aip.py
+-rw-r--r--   0        0        0     2598 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/amp.py
+-rw-r--r--   0        0        0     3159 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/cflowd.py
+-rw-r--r--   0        0        0    12158 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/control.py
+-rw-r--r--   0        0        0     4134 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/device_access.py
+-rw-r--r--   0        0        0     4250 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/device_access_ipv6.py
+-rw-r--r--   0        0        0     4585 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/dns_security.py
+-rw-r--r--   0        0        0     3251 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/hub_and_spoke.py
+-rw-r--r--   0        0        0     2139 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/intrusion_prevention.py
+-rw-r--r--   0        0        0     1403 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/mesh.py
+-rw-r--r--   0        0        0     3520 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/qos_map.py
+-rw-r--r--   0        0        0     1410 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/rewrite.py
+-rw-r--r--   0        0        0     6150 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/route_policy.py
+-rw-r--r--   0        0        0    12381 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/rule_set.py
+-rw-r--r--   0        0        0     3147 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/security_group.py
+-rw-r--r--   0        0        0     7992 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/ssl_decryption.py
+-rw-r--r--   0        0        0     3539 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/ssl_decryption_utd_profile.py
+-rw-r--r--   0        0        0    14018 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/traffic_data.py
+-rw-r--r--   0        0        0     2684 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/url_filtering.py
+-rw-r--r--   0        0        0     1329 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/vpn_membership.py
+-rw-r--r--   0        0        0    10584 2024-05-28 12:42:55.757484 catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/zone_based_firewall.py
+-rw-r--r--   0        0        0     1331 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/app.py
+-rw-r--r--   0        0        0     1295 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/app_probe.py
+-rw-r--r--   0        0        0      651 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/as_path.py
+-rw-r--r--   0        0        0      789 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/class_map.py
+-rw-r--r--   0        0        0      661 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/color.py
+-rw-r--r--   0        0        0     2634 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/communities.py
+-rw-r--r--   0        0        0      918 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/data_ipv6_prefix.py
+-rw-r--r--   0        0        0      860 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/data_prefix.py
+-rw-r--r--   0        0        0      495 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/fqdn.py
+-rw-r--r--   0        0        0     1055 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/geo_location.py
+-rw-r--r--   0        0        0      817 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/ips_signature.py
+-rw-r--r--   0        0        0     1111 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/ipv6_prefix.py
+-rw-r--r--   0        0        0      990 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/local_app.py
+-rw-r--r--   0        0        0      923 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/local_domain.py
+-rw-r--r--   0        0        0      714 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/mirror.py
+-rw-r--r--   0        0        0     1127 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/policer.py
+-rw-r--r--   0        0        0      771 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/port.py
+-rw-r--r--   0        0        0     3196 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/preferred_color_group.py
+-rw-r--r--   0        0        0     1055 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/prefix.py
+-rw-r--r--   0        0        0      723 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/protocol_name.py
+-rw-r--r--   0        0        0     1325 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/region.py
+-rw-r--r--   0        0        0      942 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/site.py
+-rw-r--r--   0        0        0     6864 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/sla.py
+-rw-r--r--   0        0        0      970 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/threat_grid_api_key.py
+-rw-r--r--   0        0        0      960 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/tloc.py
+-rw-r--r--   0        0        0     2111 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/trunkgroup.py
+-rw-r--r--   0        0        0      824 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/umbrella_data.py
+-rw-r--r--   0        0        0      856 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/url.py
+-rw-r--r--   0        0        0     1071 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/vpn.py
+-rw-r--r--   0        0        0     1405 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/list/zone.py
+-rw-r--r--   0        0        0     6204 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/localized.py
+-rw-r--r--   0        0        0     3752 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/policy.py
+-rw-r--r--   0        0        0    37132 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/policy_definition.py
+-rw-r--r--   0        0        0     1557 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/policy_list.py
+-rw-r--r--   0        0        0     9385 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/policy/security.py
+-rw-r--r--   0        0        0     2437 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/templates.py
+-rw-r--r--   0        0        0     5239 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/models/tenant.py
+-rw-r--r--   0        0        0     9717 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/response.py
+-rw-r--r--   0        0        0    19497 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/session.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/__init__.py
+-rw-r--r--   0        0        0     1236 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_converter_chooser.py
+-rw-r--r--   0        0        0      629 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_data/feature_templates/__init__.py
+-rw-r--r--   0        0        0     1710 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_data/feature_templates/dhcp.py
+-rw-r--r--   0        0        0    16810 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_data/feature_templates/interface.py
+-rw-r--r--   0        0        0    11799 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_data/feature_templates/ospfv3.py
+-rw-r--r--   0        0        0     3185 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_data/feature_templates/vpn.py
+-rw-r--r--   0        0        0     3583 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_device_template_with_info.py
+-rw-r--r--   0        0        0     6139 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_merge_parcels.py
+-rw-r--r--   0        0        0     4782 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_normalizer.py
+-rw-r--r--   0        0        0    21196 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_transform.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/models/__init__.py
+-rw-r--r--   0        0        0      401 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
+-rw-r--r--   0        0        0      513 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/banner_1.json
+-rw-r--r--   0        0        0      116 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/basic/alias.json
+-rw-r--r--   0        0        0      114 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/basic/basic.json
+-rw-r--r--   0        0        0      109 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/basic/basic_no_value.json
+-rw-r--r--   0        0        0      848 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/basic/children.json
+-rw-r--r--   0        0        0     2348 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/basic/children_nested.json
+-rw-r--r--   0        0        0     2348 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      274 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/basic/data_path.json
+-rw-r--r--   0        0        0     2973 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/cisco_bfd.json
+-rw-r--r--   0        0        0    11100 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/complex_aaa.json
+-rw-r--r--   0        0        0    41165 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
+-rw-r--r--   0        0        0     5219 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/default_cisco_system.json
+-rw-r--r--   0        0        0     5505 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/iuo.json
+-rw-r--r--   0        0        0      249 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/omp_1.json
+-rw-r--r--   0        0        0      875 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/omp_2.json
+-rw-r--r--   0        0        0     1682 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/omp_3.json
+-rw-r--r--   0        0        0      662 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/models/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/models/cisco_aaa.py
+-rw-r--r--   0        0        0      303 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/models/cisco_banner.py
+-rw-r--r--   0        0        0      587 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/models/cisco_bfd.py
+-rw-r--r--   0        0        0      344 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/models/cisco_system.py
+-rw-r--r--   0        0        0     8078 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/models/cisco_vpn.py
+-rw-r--r--   0        0        0     1091 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/models/omp_vsmart.py
+-rw-r--r--   0        0        0      605 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/basic/alias.json
+-rw-r--r--   0        0        0      574 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/basic/basic.json
+-rw-r--r--   0        0        0     1810 2024-05-28 12:42:55.761484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/basic/children.json
+-rw-r--r--   0        0        0     4005 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/basic/children_nested.json
+-rw-r--r--   0        0        0     4005 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      731 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/basic/data_path.json
+-rw-r--r--   0        0        0    43436 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/cedge_aaa.json
+-rw-r--r--   0        0        0     1200 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/cisco_banner.json
+-rw-r--r--   0        0        0     9495 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/cisco_bfd.json
+-rw-r--r--   0        0        0    99045 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/cisco_system.json
+-rw-r--r--   0        0        0    87854 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/cisco_vpn.json
+-rw-r--r--   0        0        0     5939 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/omp-vsmart.json
+-rw-r--r--   0        0        0     1381 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/test_chose_model.py
+-rw-r--r--   0        0        0     2598 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/test_deserialize_model.py
+-rw-r--r--   0        0        0     6762 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/test_find_template_values_2.py
+-rw-r--r--   0        0        0     4598 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/test_generate_payload.py
+-rw-r--r--   0        0        0     1755 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/templates/test_serialize_model.py
+-rw-r--r--   0        0        0     8145 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_admin_tech_api.py
+-rw-r--r--   0        0        0    17792 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_administration.py
+-rw-r--r--   0        0        0    11116 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_alarms_api.py
+-rw-r--r--   0        0        0     8322 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_cli_template.py
+-rw-r--r--   0        0        0     5494 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_creation_tools.py
+-rw-r--r--   0        0        0     3981 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_device_action_api.py
+-rw-r--r--   0        0        0    28159 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_devices_api.py
+-rw-r--r--   0        0        0    34991 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_endpoints.py
+-rw-r--r--   0        0        0     1897 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_extended_community_converter.py
+-rw-r--r--   0        0        0    10767 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_feature_profile_api.py
+-rw-r--r--   0        0        0      894 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_feature_template_field.py
+-rw-r--r--   0        0        0     1545 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_logs_api.py
+-rw-r--r--   0        0        0     1007 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_mirror_converter.py
+-rw-r--r--   0        0        0     1899 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_models_common.py
+-rw-r--r--   0        0        0     1809 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_monitoring_server_info.py
+-rw-r--r--   0        0        0     5489 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_monitoring_status_api.py
+-rw-r--r--   0        0        0    11026 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_mtt_aaa_api.py
+-rw-r--r--   0        0        0    10026 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_normalize_to_model_definition.py
+-rw-r--r--   0        0        0    16472 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_omp_api.py
+-rw-r--r--   0        0        0     5223 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_packet_capture.py
+-rw-r--r--   0        0        0     5727 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_partition_manager_api.py
+-rw-r--r--   0        0        0     7926 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_response.py
+-rw-r--r--   0        0        0     6724 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_session.py
+-rw-r--r--   0        0        0     7117 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_software_action_api.py
+-rw-r--r--   0        0        0     6071 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_speed_test_api.py
+-rw-r--r--   0        0        0    14926 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_task_status_api.py
+-rw-r--r--   0        0        0    15055 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_templates.py
+-rw-r--r--   0        0        0     3705 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     6114 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_tenant_management_api.py
+-rw-r--r--   0        0        0     4506 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_tenant_migration_api.py
+-rw-r--r--   0        0        0    12377 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_typed_list.py
+-rw-r--r--   0        0        0     2968 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_version.py
+-rw-r--r--   0        0        0    10377 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_version_utils.py
+-rw-r--r--   0        0        0     3343 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/tests/test_vmanage_auth.py
+-rw-r--r--   0        0        0     9379 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/typed_list.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/__init__.py
+-rw-r--r--   0        0        0      266 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/alarm_status.py
+-rw-r--r--   0        0        0      253 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/certificate_status.py
+-rw-r--r--   0        0        0      279 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/colors.py
+-rw-r--r--   0        0        0      239 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/exceptions.py
+-rw-r--r--   0        0        0      320 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/__init__.py
+-rw-r--r--   0        0        0     3433 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/aaa.py
+-rw-r--r--   0        0        0     5810 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/appqoe.py
+-rw-r--r--   0        0        0      784 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/banner.py
+-rw-r--r--   0        0        0      268 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/base.py
+-rw-r--r--   0        0        0     3283 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/basic.py
+-rw-r--r--   0        0        0      898 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/bfd.py
+-rw-r--r--   0        0        0     9266 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/bgp.py
+-rw-r--r--   0        0        0     1765 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/cellular_controller.py
+-rw-r--r--   0        0        0     3269 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/cellular_profile.py
+-rw-r--r--   0        0        0      756 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/cli.py
+-rw-r--r--   0        0        0     1932 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/cloud_credentials.py
+-rw-r--r--   0        0        0     4566 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/dhcp.py
+-rw-r--r--   0        0        0     5349 2024-05-28 12:42:55.765484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/eigrp.py
+-rw-r--r--   0        0        0     6334 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/ethernet.py
+-rw-r--r--   0        0        0      578 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/global_.py
+-rw-r--r--   0        0        0     1573 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/gps.py
+-rw-r--r--   0        0        0      331 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/helpers.py
+-rw-r--r--   0        0        0    13128 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/lan/ethernet.py
+-rw-r--r--   0        0        0     5619 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/lan/gre.py
+-rw-r--r--   0        0        0     5959 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/lan/ipsec.py
+-rw-r--r--   0        0        0     9349 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/lan/multilink.py
+-rw-r--r--   0        0        0     7411 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/lan/svi.py
+-rw-r--r--   0        0        0     1963 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/logging_.py
+-rw-r--r--   0        0        0     4855 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/model_definition_normalizer.py
+-rw-r--r--   0        0        0    13085 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/multicast.py
+-rw-r--r--   0        0        0     5470 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/normalizer.py
+-rw-r--r--   0        0        0     2295 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/ntp.py
+-rw-r--r--   0        0        0     1475 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/omp.py
+-rw-r--r--   0        0        0     5684 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/ospf.py
+-rw-r--r--   0        0        0    11458 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/ospfv3.py
+-rw-r--r--   0        0        0     6251 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/parcel_factory.py
+-rw-r--r--   0        0        0     1568 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/security.py
+-rw-r--r--   0        0        0    10159 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/sig.py
+-rw-r--r--   0        0        0     2240 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/snmp.py
+-rw-r--r--   0        0        0     9032 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/switchport.py
+-rw-r--r--   0        0        0     2776 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py
+-rw-r--r--   0        0        0     2250 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/ucse.py
+-rw-r--r--   0        0        0    31317 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/vpn.py
+-rw-r--r--   0        0        0     5742 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wan/cellular.py
+-rw-r--r--   0        0        0    13497 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wan/ethernet.py
+-rw-r--r--   0        0        0     4844 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wan/gre.py
+-rw-r--r--   0        0        0     6866 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wan/ipsec.py
+-rw-r--r--   0        0        0    14360 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wan/multilink.py
+-rw-r--r--   0        0        0    18190 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wan/protocol_over.py
+-rw-r--r--   0        0        0     5344 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wan/t1e1serial.py
+-rw-r--r--   0        0        0     8057 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wireless_lan.py
+-rw-r--r--   0        0        0     7722 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/policy/policy_definitions.py
+-rw-r--r--   0        0        0    14226 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/policy/policy_lists.py
+-rw-r--r--   0        0        0      165 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/utils.py
+-rw-r--r--   0        0        0    13019 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/creators/config_pusher.py
+-rw-r--r--   0        0        0     8511 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/creators/strategy/parcels.py
+-rw-r--r--   0        0        0     1760 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/factories/feature_profile_api.py
+-rw-r--r--   0        0        0     1257 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/factories/parcel_pusher.py
+-rw-r--r--   0        0        0     3464 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/reverters/config_reverter.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/steps/__init__.py
+-rw-r--r--   0        0        0     3767 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/steps/constants.py
+-rw-r--r--   0        0        0     9821 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/steps/transform.py
+-rw-r--r--   0        0        0      154 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/config_status.py
+-rw-r--r--   0        0        0     4778 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/creation_tools.py
+-rw-r--r--   0        0        0     7281 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/dashboard.py
+-rw-r--r--   0        0        0     2863 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/device_model.py
+-rw-r--r--   0        0        0     2110 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/dict.py
+-rw-r--r--   0        0        0      953 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/feature_template/choose_model.py
+-rw-r--r--   0        0        0     4882 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/feature_template/find_template_values.py
+-rw-r--r--   0        0        0     1173 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/model.py
+-rw-r--r--   0        0        0      584 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/operation_status.py
+-rw-r--r--   0        0        0      196 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/personality.py
+-rw-r--r--   0        0        0      360 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/pydantic_field.py
+-rw-r--r--   0        0        0      172 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/reachability.py
+-rw-r--r--   0        0        0      407 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/session_type.py
+-rw-r--r--   0        0        0      149 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/template_type.py
+-rw-r--r--   0        0        0     9825 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/timezone.py
+-rw-r--r--   0        0        0      449 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/type_check.py
+-rw-r--r--   0        0        0     3930 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/upgrades_helper.py
+-rw-r--r--   0        0        0      159 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/utils/validate_status.py
+-rw-r--r--   0        0        0     3032 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/version.py
+-rw-r--r--   0        0        0     5415 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/vmanage_auth.py
+-rw-r--r--   0        0        0    20612 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/workflows/config_migration.py
+-rw-r--r--   0        0        0     9946 2024-05-28 12:42:55.769484 catalystwan-0.33.7.dev3/catalystwan/workflows/tenant_migration.py
+-rw-r--r--   0        0        0      866 2024-05-28 12:42:55.773484 catalystwan-0.33.7.dev3/pyproject.toml
+-rw-r--r--   0        0        0    18941 1970-01-01 00:00:00.000000 catalystwan-0.33.7.dev3/setup.py
+-rw-r--r--   0        0        0    14665 1970-01-01 00:00:00.000000 catalystwan-0.33.7.dev3/PKG-INFO
```

### Comparing `catalystwan-0.33.7.dev2/LICENSE` & `catalystwan-0.33.7.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/README.md` & `catalystwan-0.33.7.dev3/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/__init__.py` & `catalystwan-0.33.7.dev3/catalystwan/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/abstractions.py` & `catalystwan-0.33.7.dev3/catalystwan/abstractions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/admin_tech_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/administration.py` & `catalystwan-0.33.7.dev3/catalystwan/api/administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/alarms_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/api_container.py` & `catalystwan-0.33.7.dev3/catalystwan/api/api_container.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/basic_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/basic_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/builder_factory.py` & `catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/builder_factory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/cli.py` & `catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/cli.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/other.py` & `catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/other.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/report.py` & `catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/report.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/service.py` & `catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/service.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/system.py` & `catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/transport.py` & `catalystwan-0.33.7.dev3/catalystwan/api/builders/feature_profiles/transport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/config_device_inventory_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/config_device_inventory_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/config_group_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/config_group_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/configuration_groups/parcel.py` & `catalystwan-0.33.7.dev3/catalystwan/api/configuration_groups/parcel.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/dashboard_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/dashboard_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/device_action_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/feature_profile_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/feature_profile_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 from catalystwan.endpoints.configuration.feature_profile.sdwan.embedded_security import EmbeddedSecurityFeatureProfile
 from catalystwan.endpoints.configuration.feature_profile.sdwan.policy_object import PolicyObjectFeatureProfile
 from catalystwan.endpoints.configuration_feature_profile import SDRoutingConfigurationFeatureProfile
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileInfo,
-    GetFeatureProfilesPayload,
+    GetFeatureProfilesParams,
     GetReferenceCountFeatureProfilesPayload,
 )
 from catalystwan.models.configuration.feature_profile.parcel import (
     Parcel,
     ParcelAssociationPayload,
     ParcelCreationResponse,
 )
@@ -212,15 +212,15 @@
 
     def get_profiles(
         self, limit: Optional[int] = None, offset: Optional[int] = None
     ) -> DataSequence[FeatureProfileInfo]:
         """
         Get all Transport Feature Profiles
         """
-        payload = GetFeatureProfilesPayload(limit=limit if limit else None, offset=offset if offset else None)
+        payload = GetFeatureProfilesParams(limit=limit if limit else None, offset=offset if offset else None)
 
         return self.endpoint.get_transport_feature_profiles(payload)
 
     def create_profile(self, name: str, description: str) -> FeatureProfileCreationResponse:
         """
         Create Transport Feature Profile
         """
@@ -318,15 +318,15 @@
 
     def get_profiles(
         self, limit: Optional[int] = None, offset: Optional[int] = None
     ) -> DataSequence[FeatureProfileInfo]:
         """
         Get all Other Feature Profiles
         """
-        payload = GetFeatureProfilesPayload(limit=limit if limit else None, offset=offset if offset else None)
+        payload = GetFeatureProfilesParams(limit=limit if limit else None, offset=offset if offset else None)
 
         return self.endpoint.get_sdwan_other_feature_profiles(payload)
 
     def create_profile(self, name: str, description: str) -> FeatureProfileCreationResponse:
         """
         Create Other Feature Profile
         """
@@ -385,15 +385,15 @@
 
     def get_profiles(
         self, limit: Optional[int] = None, offset: Optional[int] = None
     ) -> DataSequence[FeatureProfileInfo]:
         """
         Get all Service Feature Profiles
         """
-        payload = GetFeatureProfilesPayload(limit=limit if limit else None, offset=offset if offset else None)
+        payload = GetFeatureProfilesParams(limit=limit if limit else None, offset=offset if offset else None)
 
         return self.endpoint.get_sdwan_service_feature_profiles(payload)
 
     def create_profile(self, name: str, description: str) -> FeatureProfileCreationResponse:
         """
         Create Service Feature Profile
         """
@@ -441,15 +441,15 @@
 
     def get_profiles(
         self, limit: Optional[int] = None, offset: Optional[int] = None
     ) -> DataSequence[FeatureProfileInfo]:
         """
         Get all System Feature Profiles
         """
-        payload = GetFeatureProfilesPayload(limit=limit if limit else None, offset=offset if offset else None)
+        payload = GetFeatureProfilesParams(limit=limit if limit else None, offset=offset if offset else None)
 
         return self.endpoint.get_sdwan_system_feature_profiles(payload)
 
     def create_profile(self, name: str, description: str) -> FeatureProfileCreationResponse:
         """
         Create System Feature Profile
         """
@@ -809,14 +809,20 @@
     def __init__(self, session: ManagerSession):
         self.session = session
         self.endpoint = PolicyObjectFeatureProfile(session)
 
     def get_profiles(self) -> DataSequence[FeatureProfileInfo]:
         return self.endpoint.get_profiles()
 
+    def create_profile(self, profile: FeatureProfileCreationPayload) -> FeatureProfileCreationResponse:
+        return self.endpoint.create_profile()
+
+    def delete_profile(self, profile_id: UUID) -> None:
+        return self.endpoint.delete_profile(profile_id=profile_id)
+
     @overload
     def get(
         self, profile_id: UUID, parcel_type: Type[AdvancedInspectionProfileParcel]
     ) -> DataSequence[Parcel[AdvancedInspectionProfileParcel]]:
         ...
 
     @overload
@@ -1198,15 +1204,15 @@
 
     def get_profiles(
         self, limit: Optional[int] = None, offset: Optional[int] = None
     ) -> DataSequence[FeatureProfileInfo]:
         """
         Get all Embedded Security Feature Profiles
         """
-        payload = GetFeatureProfilesPayload(limit=limit if limit else None, offset=offset if offset else None)
+        payload = GetFeatureProfilesParams(limit=limit if limit else None, offset=offset if offset else None)
 
         return self.endpoint.get_embedded_security_feature_profiles(payload)
 
     def create_profile(self, name: str, description: str) -> FeatureProfileCreationResponse:
         """
         Create Embedded Security Feature Profile
         """
@@ -1308,15 +1314,15 @@
 
     def get_profiles(
         self, limit: Optional[int] = None, offset: Optional[int] = None
     ) -> DataSequence[FeatureProfileInfo]:
         """
         Get all CLI Feature Profiles
         """
-        payload = GetFeatureProfilesPayload(limit=limit if limit else None, offset=offset if offset else None)
+        payload = GetFeatureProfilesParams(limit=limit if limit else None, offset=offset if offset else None)
 
         return self.endpoint.get_profiles(payload)
 
     def create_profile(self, name: str, description: str = "") -> FeatureProfileCreationResponse:
         """
         Create CLI Feature Profile
         """
@@ -1369,15 +1375,15 @@
 
     def get_profiles(
         self, limit: Optional[int] = None, offset: Optional[int] = None
     ) -> DataSequence[FeatureProfileInfo]:
         """
         Get all DNS Security Feature Profiles
         """
-        payload = GetFeatureProfilesPayload(limit=limit if limit else None, offset=offset if offset else None)
+        payload = GetFeatureProfilesParams(limit=limit if limit else None, offset=offset if offset else None)
 
         return self.endpoint.get_dns_security_feature_profiles(payload)
 
     def create_profile(self, name: str, description: str) -> FeatureProfileCreationResponse:
         """
         Create DNS Security Feature Profile
         """
@@ -1482,15 +1488,15 @@
 
     def get_profiles(
         self, limit: Optional[int] = None, offset: Optional[int] = None
     ) -> DataSequence[FeatureProfileInfo]:
         """
         Get all Application Priority Feature Profiles
         """
-        payload = GetFeatureProfilesPayload(limit=limit if limit else None, offset=offset if offset else None)
+        payload = GetFeatureProfilesParams(limit=limit if limit else None, offset=offset if offset else None)
 
         return self.endpoint.get_application_priority_feature_profiles(payload)
 
     def create_profile(self, name: str, description: str) -> FeatureProfileCreationResponse:
         """
         Create Application Priority Feature Profile
         """
@@ -1609,15 +1615,15 @@
 
     def get_profiles(
         self, limit: Optional[int] = None, offset: Optional[int] = None
     ) -> DataSequence[FeatureProfileInfo]:
         """
         Get all Topology Feature Profiles
         """
-        payload = GetFeatureProfilesPayload(limit=limit, offset=offset)
+        payload = GetFeatureProfilesParams(limit=limit, offset=offset)
         return self.endpoint.get_topology_feature_profiles(payload)
 
     def create_profile(self, name: str, description: str) -> FeatureProfileCreationResponse:
         """
         Create Topology Feature Profile
         """
         payload = FeatureProfileCreationPayload(name=name, description=description)
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/logs_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/monitoring_status_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/mtt_aaa_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/omp_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/packet_capture_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/packet_capture_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/parcel_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/parcel_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/partition_manager_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/policy_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/policy_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/resource_pool_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/resource_pool_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/software_action_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/speedtest_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/speedtest_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/task_status_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/template_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/template_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/README.md` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/cli_template.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/device_template/device_template.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/device_template/device_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/device_template/device_template_payload.json.j2` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/device_template/device_template_payload.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/feature_template.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/feature_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/feature_template_field.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/feature_template_payload.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/feature_template_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_aaa_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_banner_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_banner_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_bfd_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_bfd_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_bgp_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_bgp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_logging_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_logging_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_ntp_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_ntp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_omp_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_omp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_ospf.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_ospfv3.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_secure_internet_gateway.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_secure_internet_gateway.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_snmp_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_snmp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_system.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_vpn_interface_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_vpn_interface_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_vpn_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/omp_vsmart_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/omp_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/security_vsmart_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/security_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/supported.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/supported.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/system_vsmart_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/models/system_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/aaa_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/aaa/aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/user.json.j2` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/aaa/feature/user.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/tenant/tenant.json.j2` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/tenant/tenant.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/tenant/tenant_model.py` & `catalystwan-0.33.7.dev3/catalystwan/api/templates/payloads/tenant/tenant_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/tenant_backup_restore_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/tenant_management_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/tenant_migration_api.py` & `catalystwan-0.33.7.dev3/catalystwan/api/tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/api/versions_utils.py` & `catalystwan-0.33.7.dev3/catalystwan/api/versions_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/dataclasses.py` & `catalystwan-0.33.7.dev3/catalystwan/dataclasses.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/__init__.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/administration_user_and_group.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/administration_user_and_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/certificate_management_device.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/certificate_management_device.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/certificate_management_vmanage.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/certificate_management_vmanage.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/client.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/client.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/cluster_management.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/cluster_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/device/software_update.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/device/software_update.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/disaster_recovery.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/disaster_recovery.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/application_priority.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/application_priority.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileDetail,
     FeatureProfileEditPayload,
     FeatureProfileInfo,
-    GetFeatureProfilesPayload,
+    GetFeatureProfilesParams,
 )
 from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelCreationResponse
 from catalystwan.models.configuration.feature_profile.sdwan.application_priority import AnyApplicationPriorityParcel
 from catalystwan.typed_list import DataSequence
 
 
 class ApplicationPriorityFeatureProfile(APIEndpoints):
@@ -24,22 +24,22 @@
         self, payload: FeatureProfileCreationPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/application-priority")
     def get_application_priority_feature_profiles(
-        self, params: GetFeatureProfilesPayload
+        self, params: GetFeatureProfilesParams
     ) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/application-priority/{profile_id}")
     def get_application_priority_feature_profile(
-        self, profile_id: str, params: GetFeatureProfilesPayload
+        self, profile_id: str, params: GetFeatureProfilesParams
     ) -> FeatureProfileDetail:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sdwan/application-priority/{profile_id}")
     def edit_application_priority_feature_profile(
         self, profile_id: str, payload: FeatureProfileEditPayload
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/cli.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileInfo,
-    GetFeatureProfilesPayload,
+    GetFeatureProfilesParams,
 )
 from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelId
 from catalystwan.models.configuration.feature_profile.sdwan.cli import ConfigParcel
 from catalystwan.typed_list import DataSequence
 
 
 class CliFeatureProfile(APIEndpoints):
     # @versions(supported_versions=(">=20.9"), raises=False)
     @get("/v1/feature-profile/sdwan/cli")
-    def get_profiles(self, payload: Optional[GetFeatureProfilesPayload]) -> DataSequence[FeatureProfileInfo]:
+    def get_profiles(self, payload: Optional[GetFeatureProfilesParams]) -> DataSequence[FeatureProfileInfo]:
         ...
 
     # @versions(supported_versions=(">=20.9"), raises=False)
     @post("/v1/feature-profile/sdwan/cli")
     def create_profile(self, payload: FeatureProfileCreationPayload) -> FeatureProfileCreationResponse:
         ...
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/dns_security.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/dns_security.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileDetail,
     FeatureProfileEditPayload,
     FeatureProfileInfo,
-    GetFeatureProfilesPayload,
+    GetFeatureProfilesParams,
 )
 from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelCreationResponse
 from catalystwan.models.configuration.feature_profile.sdwan.dns_security import AnyDnsSecurityParcel
 from catalystwan.typed_list import DataSequence
 
 
 class DnsSecurityFeatureProfile(APIEndpoints):
@@ -23,21 +23,21 @@
     def create_dns_security_feature_profile(
         self, payload: FeatureProfileCreationPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/dns-security")
-    def get_dns_security_feature_profiles(self, params: GetFeatureProfilesPayload) -> DataSequence[FeatureProfileInfo]:
+    def get_dns_security_feature_profiles(self, params: GetFeatureProfilesParams) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/dns-security/{profile_id}")
     def get_dns_security_feature_profile(
-        self, profile_id: str, params: GetFeatureProfilesPayload
+        self, profile_id: str, params: GetFeatureProfilesParams
     ) -> FeatureProfileDetail:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sdwan/dns-security/{profile_id}")
     def edit_dns_security_feature_profile(
         self, profile_id: str, payload: FeatureProfileEditPayload
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/embedded_security.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/embedded_security.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileDetail,
     FeatureProfileEditPayload,
     FeatureProfileInfo,
-    GetFeatureProfilesPayload,
+    GetFeatureProfilesParams,
 )
 from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelCreationResponse
 from catalystwan.models.configuration.feature_profile.sdwan.embedded_security import (
     AnyEmbeddedSecurityParcel,
     PolicyParcel,
 )
 from catalystwan.typed_list import DataSequence
@@ -27,22 +27,22 @@
         self, payload: FeatureProfileCreationPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/embedded-security")
     def get_embedded_security_feature_profiles(
-        self, params: GetFeatureProfilesPayload
+        self, params: GetFeatureProfilesParams
     ) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/embedded-security/{profile_id}")
     def get_embedded_security_feature_profile(
-        self, profile_id: str, params: GetFeatureProfilesPayload
+        self, profile_id: str, params: GetFeatureProfilesParams
     ) -> FeatureProfileDetail:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sdwan/embedded-security/{profile_id}")
     def edit_embedded_security_feature_profile(
         self, profile_id: str, payload: FeatureProfileEditPayload
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 from catalystwan.api.configuration_groups.parcel import _ParcelBase
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileInfo,
-    GetFeatureProfilesPayload,
+    GetFeatureProfilesParams,
 )
 from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelId
 from catalystwan.typed_list import DataSequence
 
 
 class OtherFeatureProfile(APIEndpoints):
     @versions(supported_versions=(">=20.9"), raises=False)
     @get("/v1/feature-profile/sdwan/other")
     def get_sdwan_other_feature_profiles(
-        self, payload: Optional[GetFeatureProfilesPayload]
+        self, payload: Optional[GetFeatureProfilesParams]
     ) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @post("/v1/feature-profile/sdwan/other")
     def create_sdwan_other_feature_profile(
         self, payload: FeatureProfileCreationPayload
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
-from catalystwan.models.configuration.feature_profile.common import FeatureProfileInfo, GetFeatureProfilesPayload
+from catalystwan.models.configuration.feature_profile.common import (
+    FeatureProfileCreationPayload,
+    FeatureProfileCreationResponse,
+    FeatureProfileInfo,
+    GetFeatureProfilesParams,
+)
 from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelCreationResponse
 from catalystwan.models.configuration.feature_profile.sdwan.policy_object import AnyPolicyObjectParcel
 from catalystwan.typed_list import DataSequence
 
 
 class PolicyObjectFeatureProfile(APIEndpoints):
     @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/policy-object")
     def get_profiles(
-        self, params: GetFeatureProfilesPayload = GetFeatureProfilesPayload()
+        self, params: GetFeatureProfilesParams = GetFeatureProfilesParams()
     ) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
+    @post("/v1/feature-profile/sdwan/policy-object")
+    def create_profile(self, payload: FeatureProfileCreationPayload) -> FeatureProfileCreationResponse:
+        ...
+
+    @versions(supported_versions=(">=20.12"), raises=False)
+    @delete("/v1/feature-profile/sdwan/policy-object/{profile_id}")
+    def delete_profile(self, profile_id: UUID) -> None:
+        ...
+
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/policy-object/{profile_id}/{policy_object_list_type}")
     def create(
         self, profile_id: UUID, policy_object_list_type: str, payload: AnyPolicyObjectParcel
     ) -> ParcelCreationResponse:
         ...
 
     # @versions(supported_versions=(">=20.12"), raises=False)
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, versions
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileInfo,
-    GetFeatureProfilesPayload,
+    GetFeatureProfilesParams,
 )
 from catalystwan.models.configuration.feature_profile.parcel import ParcelAssociationPayload, ParcelCreationResponse
 from catalystwan.models.configuration.feature_profile.sdwan.service import (
     AnyLanVpnInterfaceParcel,
     AnyTopLevelServiceParcel,
 )
 from catalystwan.typed_list import DataSequence
 
 
 class ServiceFeatureProfile(APIEndpoints):
     @versions(supported_versions=(">=20.9"), raises=False)
     @get("/v1/feature-profile/sdwan/service")
     def get_sdwan_service_feature_profiles(
-        self, payload: Optional[GetFeatureProfilesPayload]
+        self, payload: Optional[GetFeatureProfilesParams]
     ) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @post("/v1/feature-profile/sdwan/service")
     def create_sdwan_service_feature_profile(
         self, payload: FeatureProfileCreationPayload
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/sig_security.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/sig_security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from catalystwan.api.configuration_groups.parcel import _ParcelBase
 from catalystwan.endpoints import JSON, APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileInfo,
-    GetFeatureProfilesPayload,
+    GetFeatureProfilesParams,
     SchemaTypeQuery,
 )
 from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelId
 from catalystwan.models.configuration.feature_profile.sdwan.system import AnySystemParcel
 from catalystwan.models.configuration.feature_profile.sdwan.system.aaa import AAAParcel
 from catalystwan.models.configuration.feature_profile.sdwan.system.banner import BannerParcel
 from catalystwan.models.configuration.feature_profile.sdwan.system.basic import BasicParcel
@@ -34,15 +34,15 @@
     @get("/v1/feature-profile/sdwan/system/{parcel_type}/schema", resp_json_key="request")
     def get_schema(self, parcel_type: str, params: SchemaTypeQuery) -> JSON:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @get("/v1/feature-profile/sdwan/system")
     def get_sdwan_system_feature_profiles(
-        self, payload: Optional[GetFeatureProfilesPayload]
+        self, payload: Optional[GetFeatureProfilesParams]
     ) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @post("/v1/feature-profile/sdwan/system")
     def create_sdwan_system_feature_profile(
         self, payload: FeatureProfileCreationPayload
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/topology.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/topology.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from catalystwan.endpoints import JSON, APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileDetail,
     FeatureProfileEditPayload,
     FeatureProfileInfo,
-    GetFeatureProfilesPayload,
+    GetFeatureProfilesParams,
     SchemaTypeQuery,
 )
 from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelCreationResponse
 from catalystwan.models.configuration.feature_profile.sdwan.topology import AnyTopologyParcel
 from catalystwan.typed_list import DataSequence
 
 
@@ -23,20 +23,20 @@
     @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/topology")
     def create_topology_feature_profile(self, payload: FeatureProfileCreationPayload) -> FeatureProfileCreationResponse:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/topology")
-    def get_topology_feature_profiles(self, params: GetFeatureProfilesPayload) -> DataSequence[FeatureProfileInfo]:
+    def get_topology_feature_profiles(self, params: GetFeatureProfilesParams) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/topology/{profile_id}")
-    def get_topology_feature_profile(self, profile_id: str, params: GetFeatureProfilesPayload) -> FeatureProfileDetail:
+    def get_topology_feature_profile(self, profile_id: str, params: GetFeatureProfilesParams) -> FeatureProfileDetail:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sdwan/topology/{profile_id}")
     def edit_topology_feature_profile(
         self, profile_id: str, payload: FeatureProfileEditPayload
     ) -> FeatureProfileCreationResponse:
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from catalystwan.endpoints import JSON, APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileDetail,
     FeatureProfileEditPayload,
     FeatureProfileInfo,
-    GetFeatureProfilesPayload,
+    GetFeatureProfilesParams,
     SchemaTypeQuery,
 )
 from catalystwan.models.configuration.feature_profile.parcel import (
     Parcel,
     ParcelAssociationPayload,
     ParcelCreationResponse,
     ParcelId,
@@ -35,22 +35,20 @@
     def create_transport_feature_profile(
         self, payload: FeatureProfileCreationPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/transport")
-    def get_transport_feature_profiles(self, params: GetFeatureProfilesPayload) -> DataSequence[FeatureProfileInfo]:
+    def get_transport_feature_profiles(self, params: GetFeatureProfilesParams) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/transport/{profile_id}")
-    def get_transport_feature_profile(
-        self, profile_id: UUID, params: GetFeatureProfilesPayload
-    ) -> FeatureProfileDetail:
+    def get_transport_feature_profile(self, profile_id: UUID, params: GetFeatureProfilesParams) -> FeatureProfileDetail:
         ...
 
     @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sdwan/transport/{profile_id}")
     def edit_transport_feature_profile(
         self, profile_id: UUID, payload: FeatureProfileEditPayload
     ) -> FeatureProfileCreationResponse:
@@ -121,15 +119,15 @@
     @delete("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn/{parcel_id}")
     def delete_management_vpn_parcel(self, profile_id: UUID, parcel_id: str) -> None:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @get("/v1/feature-profile/sdwan/transport")
     def get_sdwan_transport_feature_profiles(
-        self, payload: Optional[GetFeatureProfilesPayload]
+        self, payload: Optional[GetFeatureProfilesParams]
     ) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @get("/v1/feature-profile/sdwan/transport/cellular-controller/schema", resp_json_key="request")
     def get_sdwan_transport_cellular_controller_parcel_schema(self, params: SchemaTypeQuery) -> JSON:
         ...
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/abstractions.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/abstractions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/access_control_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/aip.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/aip.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/amp.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/amp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/cflowd.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/cflowd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/control.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/control.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/device_access.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/device_access.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/dns_security.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/dns_security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/intrusion_prevention.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/intrusion_prevention.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/mesh.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/mesh.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/qos_map.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/qos_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/rewrite.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/rewrite.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/route_policy.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/route_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/rule_set.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/rule_set.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/security_group.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/security_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/ssl_decryption.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/ssl_decryption.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/ssl_decryption_utd_profile.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/ssl_decryption_utd_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/traffic_data.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/traffic_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/url_filtering.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/url_filtering.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/app.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/app_probe.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/as_path.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/as_path.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/class_map.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/class_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/color.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/community.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/data_prefix.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/expanded_community.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/expanded_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/extended_community.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/extended_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/fqdn.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/fqdn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/geo_location.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/geo_location.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/ips_signature.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/local_app.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/local_app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/local_domain.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/mirror.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/mirror.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/policer.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/policer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/port.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/prefix.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/protocol_name.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/protocol_name.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/region.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/region.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/site.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/site.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/sla.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/sla.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/tloc.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/tloc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/trunkgroup.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/trunkgroup.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/umbrella_data.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/umbrella_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/url_allow_list.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/url_allow_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/url_block_list.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/url_block_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/vpn.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/zone.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/list/zone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/security_template.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/security_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/vedge_template.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/vedge_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/vsmart_template.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/policy/vsmart_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/software_actions.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/software_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/topology_group.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration/topology_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_dashboard_status.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration_dashboard_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_device_actions.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration_device_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_device_inventory.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration_device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_device_template.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration_device_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_feature_profile.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration_feature_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_group.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_settings.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/configuration_settings.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/endpoints_container.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/endpoints_container.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/misc.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/misc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/monitoring/device_details.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/monitoring/device_details.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/monitoring/status.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/monitoring/status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/real_time_monitoring/reboot_history.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/real_time_monitoring/reboot_history.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/sdavc_cloud_connector.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/sdavc_cloud_connector.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/tenant_backup_restore.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/tenant_backup_restore.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/tenant_management.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/tenant_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/tenant_migration.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py` & `catalystwan-0.33.7.dev3/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/exceptions.py` & `catalystwan-0.33.7.dev3/catalystwan/exceptions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/base.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/base.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_application_priority.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_application_priority.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_cli.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_cli.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_dns_security.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_dns_security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_extended_community.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_extended_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_other.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_other.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_service.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_service.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_sig_security.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_sig_security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_system.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_transport.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/test_transport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/topology/test_topology.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/feature_profile/sdwan/topology/test_topology.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/profile_builder/base.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/profile_builder/base.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/profile_builder/test_pb_service.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/profile_builder/test_pb_service.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/profile_builder/test_pb_transport.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/profile_builder/test_pb_transport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/test_config_migration.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/test_config_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/test_data/__init__.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/test_data/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/integration_tests/test_find_template_values.py` & `catalystwan-0.33.7.dev3/catalystwan/integration_tests/test_find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/logging.conf` & `catalystwan-0.33.7.dev3/catalystwan/logging.conf`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/common.py` & `catalystwan-0.33.7.dev3/catalystwan/models/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/config_migration.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/config_migration.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,14 @@
     sites_by_list_id: Dict[UUID, List[str]] = field(default_factory=dict)
     lan_vpns_by_list_id: Dict[UUID, List[str]] = field(default_factory=dict)
 
     @staticmethod
     def from_configs(
         network_hierarchy: List[NodeInfo],
         transformed_parcels: List[TransformedParcel],
-        policy_list_infos: List[AnyPolicyListInfo],
     ) -> "PolicyConvertContext":
         context = PolicyConvertContext()
         for node in network_hierarchy:
             if node.data.hierarchy_id is not None:
                 if node.data.label == "SITE" and node.data.hierarchy_id.site_id is not None:
                     context.site_map[node.name] = node.data.hierarchy_id.site_id
                 if node.data.label == "REGION" and node.data.hierarchy_id.region_id is not None:
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/docs/diagram.png` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/docs/diagram.png`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/README.md` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/builder.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/builder.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/common.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,20 +108,20 @@
 
 class SchemaTypeQuery(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
 
     schema_type: SchemaType = Field(alias="schemaType")
 
 
-class GetFeatureProfilesPayload(BaseModel):
+class GetFeatureProfilesParams(BaseModel):
     limit: Optional[int] = None
     offset: Optional[int] = None
 
 
-class GetReferenceCountFeatureProfilesPayload(GetFeatureProfilesPayload):
+class GetReferenceCountFeatureProfilesPayload(GetFeatureProfilesParams):
     model_config = ConfigDict(populate_by_name=True)
 
     reference_count: Optional[bool] = Field(serialization_alias="referenceCount", validation_alias="referenceCount")
 
 
 class DNSIPv4(BaseModel):
     model_config = ConfigDict(
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/parcel.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/parcel.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/acl/ipv4acl.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/acl/ipv4acl.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/acl/ipv6acl.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/acl/ipv6acl.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/application_priority/__init__.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/application_priority/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/application_priority/policy_settings.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/application_priority/policy_settings.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/application_priority/qos_policy.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/application_priority/qos_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/application_priority/traffic_policy.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/application_priority/traffic_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/dns_security/dns.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/dns_security/dns.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/ngfirewall.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/ngfirewall.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/policy.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/extended_community.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/extended_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/aip.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/aip.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/amp.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/amp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/intrusion_prevention.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/intrusion_prevention.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption_profile.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url_filtering.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url_filtering.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/__init__.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/bgp.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/routing/bgp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/ospf.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/routing/ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/ospfv3.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/routing/ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/__init__.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/multilink.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/lan/multilink.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/sig_security/sig_security.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/sig_security/sig_security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/device_access.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/device_access.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/device_access_ipv6.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/device_access_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/security.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/__init__.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/topology/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/custom_control.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/topology/custom_control.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/hubspoke.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/topology/hubspoke.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/mesh.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/topology/mesh.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/__init__.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_profile.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/gps.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/gps.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/management/ethernet.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/management/ethernet.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/t1e1controller.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/t1e1controller.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/vpn.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/cellular.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/cellular.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ethernet.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ethernet.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/gre.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/gre.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ipsec.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ipsec.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/multilink.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/multilink.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/protocol_over.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/protocol_over.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/t1e1serial.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/t1e1serial.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/network_hierarchy.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/network_hierarchy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/configuration/topology_group.py` & `catalystwan-0.33.7.dev3/catalystwan/models/configuration/topology_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/device_inventory.py` & `catalystwan-0.33.7.dev3/catalystwan/models/device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/misc/application_protocols.py` & `catalystwan-0.33.7.dev3/catalystwan/models/misc/application_protocols.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/__init__.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/centralized.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/centralized.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/access_control_list.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/access_control_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/access_control_list_ipv6.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/access_control_list_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/aip.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/aip.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/amp.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/amp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/cflowd.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/cflowd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/control.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/control.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/device_access.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/device_access.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/device_access_ipv6.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/device_access_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/dns_security.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/dns_security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/hub_and_spoke.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/hub_and_spoke.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/intrusion_prevention.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/intrusion_prevention.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/mesh.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/mesh.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/qos_map.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/qos_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/rewrite.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/rewrite.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/route_policy.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/route_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/rule_set.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/rule_set.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/security_group.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/security_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/ssl_decryption.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/ssl_decryption.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/ssl_decryption_utd_profile.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/ssl_decryption_utd_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/traffic_data.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/traffic_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/url_filtering.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/url_filtering.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/vpn_membership.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/vpn_membership.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/zone_based_firewall.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/definition/zone_based_firewall.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/app.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/app_probe.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/as_path.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/as_path.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/class_map.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/class_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/color.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/communities.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/communities.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/data_ipv6_prefix.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/data_ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/data_prefix.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/geo_location.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/geo_location.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/ips_signature.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/ipv6_prefix.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/local_app.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/local_app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/local_domain.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/mirror.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/mirror.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/policer.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/policer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/port.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/preferred_color_group.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/preferred_color_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/prefix.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/protocol_name.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/protocol_name.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/region.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/region.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/site.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/site.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/sla.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/sla.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/threat_grid_api_key.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/threat_grid_api_key.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/tloc.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/tloc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/trunkgroup.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/trunkgroup.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/umbrella_data.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/umbrella_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/url.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/url.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/vpn.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/zone.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/list/zone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/localized.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/localized.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/policy.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/policy_definition.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/policy_definition.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/policy_list.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/policy_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/policy/security.py` & `catalystwan-0.33.7.dev3/catalystwan/models/policy/security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/templates.py` & `catalystwan-0.33.7.dev3/catalystwan/models/templates.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/models/tenant.py` & `catalystwan-0.33.7.dev3/catalystwan/models/tenant.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/response.py` & `catalystwan-0.33.7.dev3/catalystwan/response.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/session.py` & `catalystwan-0.33.7.dev3/catalystwan/session.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_converter_chooser.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_converter_chooser.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/__init__.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_data/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/dhcp.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_data/feature_templates/dhcp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/interface.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_data/feature_templates/interface.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/ospfv3.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_data/feature_templates/ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/vpn.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_data/feature_templates/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_device_template_with_info.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_device_template_with_info.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_merge_parcels.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_merge_parcels.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_normalizer.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_transform.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/config_migration/test_transform.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/banner_1.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/banner_1.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/children.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/children_nested.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/cisco_bfd.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/complex_aaa.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/complex_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/complex_cisco_vpn.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/complex_cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/default_cisco_system.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/default_cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/iuo.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/iuo.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/omp_2.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/omp_2.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/omp_3.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/definitions/omp_3.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/__init__.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/models/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_aaa.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/models/cisco_aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_bfd.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/models/cisco_bfd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_vpn.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/models/cisco_vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/omp_vsmart.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/models/omp_vsmart.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/alias.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/basic/alias.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/basic.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/basic/basic.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/children.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/children_nested.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/data_path.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/basic/data_path.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cedge_aaa.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/cedge_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_banner.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/cisco_banner.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_bfd.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_system.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_vpn.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/omp-vsmart.json` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/schemas/omp-vsmart.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_chose_model.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/test_chose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_deserialize_model.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/test_deserialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_find_template_values_2.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/test_find_template_values_2.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_generate_payload.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/test_generate_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_serialize_model.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/templates/test_serialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_admin_tech_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_administration.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_alarms_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_cli_template.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_creation_tools.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_device_action_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_devices_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_devices_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_endpoints.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_extended_community_converter.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_extended_community_converter.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_feature_profile_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_feature_profile_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_feature_template_field.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_logs_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_mirror_converter.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_mirror_converter.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_models_common.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_models_common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_monitoring_server_info.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_monitoring_server_info.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_monitoring_status_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_mtt_aaa_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_normalize_to_model_definition.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_normalize_to_model_definition.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_omp_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_packet_capture.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_packet_capture.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_partition_manager_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_response.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_session.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_software_action_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_speed_test_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_speed_test_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_task_status_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_templates.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_tenant_backup_restore_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_tenant_management_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_tenant_migration_api.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_typed_list.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_version.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_version_utils.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/tests/test_vmanage_auth.py` & `catalystwan-0.33.7.dev3/catalystwan/tests/test_vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/typed_list.py` & `catalystwan-0.33.7.dev3/catalystwan/typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/aaa.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/appqoe.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/appqoe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/banner.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/banner.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/basic.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/basic.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/bfd.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/bfd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/bgp.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/bgp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cellular_controller.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/cellular_controller.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cellular_profile.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/cellular_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cli.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/cli.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cloud_credentials.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/cloud_credentials.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/dhcp.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/dhcp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/eigrp.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/eigrp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ethernet.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/ethernet.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/global_.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/global_.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/gps.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/gps.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/ethernet.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/lan/ethernet.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/gre.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/lan/gre.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/ipsec.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/lan/ipsec.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/multilink.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/lan/multilink.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/svi.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/lan/svi.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/logging_.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/logging_.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/model_definition_normalizer.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/model_definition_normalizer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/multicast.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/multicast.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/normalizer.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/normalizer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ntp.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/ntp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/omp.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/omp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ospf.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ospfv3.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/parcel_factory.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/parcel_factory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/security.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/sig.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/sig.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/snmp.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/snmp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/switchport.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/switchport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ucse.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/ucse.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/vpn.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/cellular.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wan/cellular.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/ethernet.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wan/ethernet.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/gre.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wan/gre.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/ipsec.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wan/ipsec.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/multilink.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wan/multilink.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/protocol_over.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wan/protocol_over.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/t1e1serial.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wan/t1e1serial.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wireless_lan.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/feature_template/wireless_lan.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/policy/policy_definitions.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/policy/policy_definitions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/policy/policy_lists.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/converters/policy/policy_lists.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/creators/config_pusher.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/creators/config_pusher.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from catalystwan.exceptions import ManagerHTTPError
 from catalystwan.models.configuration.config_migration import (
     TransformedFeatureProfile,
     TransformedParcel,
     UX2Config,
     UX2ConfigPushResult,
 )
-from catalystwan.models.configuration.feature_profile.common import ProfileType
+from catalystwan.models.configuration.feature_profile.common import FeatureProfileCreationPayload, ProfileType
 from catalystwan.models.configuration.feature_profile.parcel import AnyParcel, Parcel, list_types
 from catalystwan.models.configuration.feature_profile.sdwan.policy_object import AnyPolicyObjectParcel
 from catalystwan.models.configuration.feature_profile.sdwan.topology.custom_control import CustomControlParcel
 from catalystwan.models.configuration.feature_profile.sdwan.topology.hubspoke import HubSpokeParcel
 from catalystwan.models.configuration.feature_profile.sdwan.topology.mesh import MeshParcel
 from catalystwan.session import ManagerSession
 from catalystwan.typed_list import DataSequence
@@ -50,15 +50,15 @@
             feature_profile_map={item.header.origin: item for item in ux2_config.feature_profiles},
             parcel_map={item.header.origin: item for item in ux2_config.profile_parcels},
         )
 
     def push(self) -> UX2ConfigPushResult:
         self._create_cloud_credentials()
         self._create_config_groups()
-        dpop = self._get_default_policy_object_profile()
+        dpop = self._get_or_create_default_policy_object_profile()
         self._insert_groups_of_interest_in_default_policy_object_profile(dpop)
         self._create_topology_groups(dpop)  # needs to be executed after vpn parcels and groups of interests are created
         self._push_result.report.set_failed_push_parcels_flat_list()
         logger.debug(f"Configuration push completed. Rollback configuration {self._push_result}")
         return self._push_result
 
     def _create_cloud_credentials(self):
@@ -98,17 +98,22 @@
                 self._push_result.rollback.add_config_group(cg_id)
                 self._push_result.report.add_report(
                     name=transformed_config_group.config_group.name,
                     uuid=cg_id,
                     feature_profiles=created_profiles,
                 )
 
-    def _get_default_policy_object_profile(self) -> UUID:
+    def _get_or_create_default_policy_object_profile(self) -> UUID:
         api = self._session.api.sdwan_feature_profiles.policy_object
-        profile_id = api.get_profiles().find(solution="sdwan", created_by="system").profile_id
+        profiles = api.get_profiles()
+        if len(profiles) >= 1:
+            return profiles[0].profile_id
+        profile_id = api.create_profile(
+            FeatureProfileCreationPayload(name="Policy_Profile_Global", description="Policy_Profile_Global_description")
+        ).id
         return profile_id
 
     def _insert_groups_of_interest_in_default_policy_object_profile(self, profile_id: UUID):
         # TODO: fix typing issues in this method, probably we need literal containig AnyPolicyObjectType type_
         def cast_(parcel: AnyParcel) -> AnyPolicyObjectParcel:
             return parcel  # type: ignore
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/creators/strategy/parcels.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/creators/strategy/parcels.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/factories/feature_profile_api.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/factories/feature_profile_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/factories/parcel_pusher.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/factories/parcel_pusher.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/reverters/config_reverter.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/reverters/config_reverter.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/steps/constants.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/steps/constants.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/steps/transform.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/config_migration/steps/transform.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/creation_tools.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/dashboard.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/device_model.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/device_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/dict.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/dict.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/feature_template/choose_model.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/feature_template/choose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/feature_template/find_template_values.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/feature_template/find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/model.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/operation_status.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/operation_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/timezone.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/utils/upgrades_helper.py` & `catalystwan-0.33.7.dev3/catalystwan/utils/upgrades_helper.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/version.py` & `catalystwan-0.33.7.dev3/catalystwan/version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/vmanage_auth.py` & `catalystwan-0.33.7.dev3/catalystwan/vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/catalystwan/workflows/config_migration.py` & `catalystwan-0.33.7.dev3/catalystwan/workflows/config_migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,17 +388,15 @@
             cloud_credential_templates.append(ft)
 
     # Add Cloud Credentials to UX2
     if cloud_credential_templates:
         ux2.cloud_credentials = create_cloud_credentials_from_templates(cloud_credential_templates)
 
     # Prepare Context for Policy Conversion (VPN Parcels must be already transformed)
-    policy_context = PolicyConvertContext.from_configs(
-        ux1.network_hierarchy, ux2.profile_parcels, ux1.policies.policy_lists
-    )
+    policy_context = PolicyConvertContext.from_configs(ux1.network_hierarchy, ux2.profile_parcels)
 
     # Policy Lists
     for policy_list in ux1.policies.policy_lists:
         try:
             pl_parcel = convert_policy_list(policy_list, policy_context)
             if pl_parcel is not None:
                 header = TransformHeader(
```

### Comparing `catalystwan-0.33.7.dev2/catalystwan/workflows/tenant_migration.py` & `catalystwan-0.33.7.dev3/catalystwan/workflows/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev2/pyproject.toml` & `catalystwan-0.33.7.dev3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "catalystwan"
-version = "0.33.7dev2"
+version = "0.33.7dev3"
 description = "Cisco Catalyst WAN SDK for Python"
 authors = ["kagorski <kagorski@cisco.com>"]
 readme = "README.md"
 repository = "https://github.com/cisco-open/cisco-catalyst-wan-sdk"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
```

### Comparing `catalystwan-0.33.7.dev2/setup.py` & `catalystwan-0.33.7.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
  'requests-toolbelt>=1.0.0,<2.0.0',
  'requests>=2.27.1,<3.0.0',
  'tenacity>=8.1.0,<9.0.0',
  'typing-extensions>=4.6.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'catalystwan',
-    'version': '0.33.7.dev2',
+    'version': '0.33.7.dev3',
     'description': 'Cisco Catalyst WAN SDK for Python',
     'long_description': '<p align="center">\n  <a href="#"><img src="docs/images/catalystwan.svg" alt="Cisco Catalyst WAN SDK Logo" style="height:150px" />\n</p>\n\n[![Python-Supported](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)](https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating simple and parallel automatic requests via official SD-WAN Manager API. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any SD-WAN Manager.\n\n## Important Notice: Early Beta Release\n\nWelcome to the Cisco Catalyst WAN SDK!\n\nWe are thrilled to announce that Cisco Catalyst WAN SDK is now available in early beta. This is an exciting step forward in enabling developers to harness the full potential of Cisco\'s networking solutions.  Please be aware that, as an early beta release, this version of the SDK is still undergoing development and testing. As such, it is provided "as is" and support to address any issues are limited and best effort.\n\n## Not recommend to use in production environments.\nWe encourage developers to explore and test the SDK\'s capabilities, but please exercise caution when using it in production environments.  We are dedicated to improving the Cisco Catalyst WAN SDK and we value your input. Your feedback is crucial to us-it will guide us in refining and enhancing the SDK to better meet your needs.\nTo report any issues, share your insights, or suggest improvements, please visit our Issues page on GitHub or reach out to us through the provided communication channels.\n\nThank you for being a part of our development journey!\n\n## Installation\n```console\npip install catalystwan\n```\n\n## Manager Session\nIn order to execute SDK APIs **ManagerSession** needs to be created. The fastest way to get started is to use `create_manager_session()` method which configures session, performs authentication for given credentials and returns **ManagerSession** instance in operational state. **ManagerSession** provides a collection of supported APIs in `api` instance variable.\nPlease check example below:\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    devices = session.api.devices.get()\n    print(devices)\n```\n**ManagerSession** extends [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) so all functionality from [requests](https://requests.readthedocs.io/en/latest/) library is avaiable to user, it also implements python [contextmanager](https://docs.python.org/3.8/library/contextlib.html#contextlib.contextmanager) and automatically frees server resources on exit.\n\n<details>\n    <summary> <b>Configure Manager Session before using</b> <i>(click to expand)</i></summary>\n\nIt is possible to configure **ManagerSession** prior sending any request.\n\n```python\nfrom catalystwan.session import ManagerSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\n# configure session using constructor - nothing will be sent to target server yet\nsession = ManagerSession(url=url, username=username, password=password)\n# login and send requests\nsession.login()\nsession.get("/dataservice/device")\nsession.close()\n```\nWhen interacting with the SDWAN Manager API without using a context manager, it\'s important \nto manually execute the `close()` method to release the user session resource.\nEnsure that the `close()` method is called after you have finished using the session to maintain optimal resource management and avoid potential errors.\n\n</details>\n\n<details>\n    <summary> <b>Login as Tenant</b> <i>(click to expand)</i></summary>\n\nTenant domain needs to be provided in url together with Tenant credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "tenant.example.com"\nusername = "tenant_user"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    print(session.session_type)\n```\n\n</details>\n\n<details>\n    <summary> <b>Login as Provider-as-Tenant</b> <i>(click to expand)</i></summary>\n\nTenant `subdomain` needs to be provided as additional argument together with Provider credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "provider"\npassword = "password123"\nsubdomain = "tenant.example.com"\n\nwith create_manager_session(url=url, username=username, password=password, subdomain=subdomain) as session:\n    print(session.session_type)\n```\n\n</details>\n\n\n\n## API usage examples\nAll examples below assumes `session` variable contains logged-in [Manager Session](#Manager-Session) instance.\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\ncontrollers = session.endpoints.configuration_device_inventory.get_device_details(\'controllers\')\nvsmarts = controllers.filter(personality=Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices=vsmarts, image=image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\nTo get all alarms:\n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter(viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn = 24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get all critical alarms from past `n` hours:\n\n```python\nn = 48\ncritical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)\n```\n\n</details>\n\n<details>\n    <summary> <b>Users</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all users\nsession.api.users.get()\n\n# Create user\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nsession.api.users.create(new_user)\n\n# Update user data\nnew_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")\nsession.api.users.update(new_user_update)\n\n# Update user password\nsession.api.users.update_password("new_user", "n3W-P4s$w0rd")\n\n# Reset user\nsession.api.users.reset("new_user")\n\n# Delete user\nsession.api.users.delete("new_user")\n\n# Get current user authentication type and role\nsession.api.users.get_auth_type()\nsession.api.users.get_role()\n```\n\n</details>\n\n<details>\n    <summary> <b>User Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all user groups\nsession.api.user_groups.get()\n\n# Create user group\ngroup = UserGroup("new_user_group", [])\ngroup.enable_read({"Audit Log", "Alarms"})\ngroup.enable_read_and_write({"Device Inventory"})\nsession.api.user_groups.create(group)\n\n# Update user group\ngroup.disable({"Alarms"})\nsession.api.user_groups.update(group)\n\n# Delete user group\nsession.api.user_groups.delete(group.group_name)\n```\n\n</details>\n\n</details>\n\n<details>\n    <summary> <b>Sessions</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all active sessions\nactive_sessions = session.api.sessions.get()\n\n# Invalidate sessions for given user\nnew_user_sessions = active_sessions.filter(raw_username="new_user")\nsession.api.sessions.invalidate(new_user_sessions)\n```\n\n</details>\n\n<details>\n    <summary> <b>Resource Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# get resource groups\nsession.api.resource_groups.get()\n\n# create resource group\nnew_resource_group = ResourceGroup(\n    name="new_resource_group",\n    desc="Custom Resource Group #1",\n    siteIds=[]\n)\nsession.api.resource_groups.create(new_resource_group)\n\n# update resource group\nresource_group = session.api.resource_groups.get().filter(name="new_resource_group").single_or_default()\nupdated_resource_group = ResourceGroupUpdateRequest(\n    id=resource_group.id,\n    name=resource_group.name,\n    desc="Custom Resource Group #1 with updated description and site ids",\n    siteIds=[200]\n)\n\n# switch to resource group view\nsession.api.resource_groups.switch("new_resource_group")\n\n# delete resource group\nsession.api.resource_groups.delete(resource_group.id)\n```\n\n</details>\n\n<details>\n    <summary> <b>Tenant management</b> <i>(click to expand)</i></summary>\n\n```python\napi = session.api.tenant_management\n# create tenants\ntenants = [\n    Tenant(\n        name="tenant1",\n        org_name="CiscoDevNet",\n        subdomain="alpha.bravo.net",\n        desc="This is tenant for unit tests",\n        edge_connector_enable=True,\n        edge_connector_system_ip="172.16.255.81",\n        edge_connector_tunnel_interface_name="GigabitEthernet1",\n        wan_edge_forecast=1,\n    )\n]\ncreate_task = api.create(tenants)\ncreate_task.wait_for_completed()\n# list all tenants\ntenants_data = api.get_all()\n# pick tenant from list by name\ntenant = tenants_data.filter(name="tenant1").single_or_default()\n# get selected tenant id\ntenant_id = tenant.tenant_id\n# get vsession id of selected tenant\nvsessionid = api.vsession_id(tenant_id)\n# delete tenant by ids\ndelete_task = api.delete([tenant_id])\ndelete_task.wait_for_completed()\n# others\napi.get_hosting_capacity_on_vsmarts()\napi.get_statuses()\napi.get_vsmart_mapping()\n```\n</details>\n\n<details>\n    <summary> <b>Tenant migration</b> <i>(click to expand)</i></summary>\n\n```python\nfrom pathlib import Path\nfrom catalystwan.session import create_manager_session\nfrom catalystwan.models.tenant import TenantExport\nfrom catalystwan.workflows.tenant_migration import migration_workflow\n\ntenant = TenantExport(\n    name="mango",\n    desc="Mango tenant description",\n    org_name="Provider Org-Mango Inc",\n    subdomain="mango.fruits.com",\n    wan_edge_forecast=100,\n    migration_key="MangoTenantMigrationKey",   # only for SDWAN Manager >= 20.13\n    is_destination_overlay_mt=True,            # only for SDWAN Manager >= 20.13\n)\n\nwith create_manager_session(url="10.0.1.15", username="st-admin", password="") as origin_session, \\\n     create_manager_session(url="10.9.0.16", username="mt-provider-admin", password="") as target_session:\n    migration_workflow(\n        origin_session=origin_session,\n        target_session=target_session,\n        workdir=Path("workdir"),\n        tenant=tenant,\n        validator="10.9.12.26"\n    )\n```\n\n`migration_workflow` performs multi-step migration procedure according to [Migrate Single-Tenant Cisco SD-WAN Overlay to Multitenant Cisco SD-WAN Deployment](https://www.cisco.com/c/en/us/td/docs/routers/sdwan/configuration/system-interface/vedge-20-x/systems-interfaces-book/sdwan-multitenancy.html#concept_sjj_jmm_z4b)\n\n\nSince 20.13 also MT to ST is supported (just provide suitable origin/target sessions, and `is_destination_overlay_mt` parameter)\n\n\nEach step of the `migration_workflow` procedure can be executed independently using api methods: `export_tenant`, `download`, `import_tenant`, `store_token`, `migrate_network`\n\n```python\norigin_api = origin_session.api.tenant_migration_api\ntarget_api = target_session.api.tenant_migration_api\ntenant_file = Path("~/tenant.tar.gz")\ntoken_file = Path("~/tenant-token.txt")\n# export\nexport_task = origin_api.export_tenant(tenant=tenant)\nremote_filename = export_task.wait_for_file()\n# download\norigin_api.download(export_path, remote_filename)\n# import\nimport_task = target_api.import_tenant(export_path, tenant.migration_key)\nimport_task.wait_for_completed()\n# get token\nmigration_id = import_task.import_info.migration_token_query_params.migration_id\ntarget_api.store_token(migration_id, token_path)\n# migrate network\nmigrate_task = origin_api.migrate_network(token_path)\nmigrate_task.wait_for_completed()\n```\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n    session.api.users.delete("bogus-user-name")\nexcept ManagerHTTPError as error:\n    # Process an error.\n    print(error.response.status_code)\n    print(error.info.code)\n    print(error.info.message)\n    print(error.info.details)\n\n```\n\n## [Supported API endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md)\n\n\n## [Contributing, bug reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on catalystwan@cisco.com.\n',
     'author': 'kagorski',
     'author_email': 'kagorski@cisco.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cisco-open/cisco-catalyst-wan-sdk',
```

### Comparing `catalystwan-0.33.7.dev2/PKG-INFO` & `catalystwan-0.33.7.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystwan
-Version: 0.33.7.dev2
+Version: 0.33.7.dev3
 Summary: Cisco Catalyst WAN SDK for Python
 Home-page: https://github.com/cisco-open/cisco-catalyst-wan-sdk
 Author: kagorski
 Author-email: kagorski@cisco.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: catalystwan Version: 0.33.7.dev2 Summary: Cisco
+Metadata-Version: 2.1 Name: catalystwan Version: 0.33.7.dev3 Summary: Cisco
 Catalyst WAN SDK for Python Home-page: https://github.com/cisco-open/cisco-
 catalyst-wan-sdk Author: kagorski Author-email: kagorski@cisco.com Requires-
 Python: >=3.8.0,<4.0.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Jinja2
 (>=3.1.2,<4.0.0) Requires-Dist: attrs (>=21.4.0,<22.0.0) Requires-Dist:
```

