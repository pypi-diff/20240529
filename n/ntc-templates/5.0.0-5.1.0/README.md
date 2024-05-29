# Comparing `tmp/ntc_templates-5.0.0.tar.gz` & `tmp/ntc_templates-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntc_templates-5.0.0.tar", max compression
+gzip compressed data, was "ntc_templates-5.1.0.tar", max compression
```

## Comparing `ntc_templates-5.0.0.tar` & `ntc_templates-5.1.0.tar`

### file list

```diff
@@ -1,694 +1,694 @@
--rw-r--r--   0        0        0      601 2024-04-08 14:14:45.223636 ntc_templates-5.0.0/LICENSE
--rw-r--r--   0        0        0     2842 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/README.md
--rw-r--r--   0        0        0      260 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/__init__.py
--rw-r--r--   0        0        0     2292 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/parse.py
--rw-r--r--   0        0        0      728 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_aos_show_vlan.textfsm
--rw-r--r--   0        0        0      170 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_oam_mac-ping.textfsm
--rw-r--r--   0        0        0      371 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_lag.textfsm
--rw-r--r--   0        0        0      641 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_port.textfsm
--rw-r--r--   0        0        0      475 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_bgp_routes_vpn-ipv4.textfsm
--rw-r--r--   0        0        0      526 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_bgp_summary_family.textfsm
--rw-r--r--   0        0        0      668 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_interface.textfsm
--rw-r--r--   0        0        0      318 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_isis_adjacency.textfsm
--rw-r--r--   0        0        0      336 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_isis_interface.textfsm
--rw-r--r--   0        0        0      619 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_ldp_interface.textfsm
--rw-r--r--   0        0        0      608 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_mpls_interface.textfsm
--rw-r--r--   0        0        0      512 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_mpls_lsp.textfsm
--rw-r--r--   0        0        0      547 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_ospf_interface.textfsm
--rw-r--r--   0        0        0      425 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_pim_interface.textfsm
--rw-r--r--   0        0        0      649 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_rsvp_interface.textfsm
--rw-r--r--   0        0        0      544 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_service_id_base.textfsm
--rw-r--r--   0        0        0      665 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_service_sap-using.textfsm
--rw-r--r--   0        0        0      598 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_service_sdp-using.textfsm
--rw-r--r--   0        0        0      642 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_service_sdp.textfsm
--rw-r--r--   0        0        0      522 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_system_cpu.textfsm
--rw-r--r--   0        0        0      355 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_arp.textfsm
--rw-r--r--   0        0        0      184 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_etherchannel_summary.textfsm
--rw-r--r--   0        0        0     1647 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_interface.textfsm
--rw-r--r--   0        0        0     1824 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_interface_switchport.textfsm
--rw-r--r--   0        0        0      883 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_ip_route.textfsm
--rw-r--r--   0        0        0     1582 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      222 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_mac_address-table.textfsm
--rw-r--r--   0        0        0      706 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_static-channel-group.textfsm
--rw-r--r--   0        0        0      831 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_system.textfsm
--rw-r--r--   0        0        0     1243 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_vlan_all.textfsm
--rw-r--r--   0        0        0      371 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_bash_df_-h.textfsm
--rw-r--r--   0        0        0      430 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_dir_flash.textfsm
--rw-r--r--   0        0        0      121 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_boot-config.textfsm
--rw-r--r--   0        0        0      226 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_clock.textfsm
--rw-r--r--   0        0        0      524 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_environment_cooling.textfsm
--rw-r--r--   0        0        0      525 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_environment_temperature.textfsm
--rw-r--r--   0        0        0      107 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_hostname.textfsm
--rw-r--r--   0        0        0      897 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_interfaces.textfsm
--rw-r--r--   0        0        0      443 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_interfaces_description.textfsm
--rw-r--r--   0        0        0      408 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_interfaces_status.textfsm
--rw-r--r--   0        0        0      313 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver.textfsm
--rw-r--r--   0        0        0      757 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver_detail.textfsm
--rw-r--r--   0        0        0      671 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_inventory.textfsm
--rw-r--r--   0        0        0      517 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_access-lists.textfsm
--rw-r--r--   0        0        0      246 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_arp.textfsm
--rw-r--r--   0        0        0      664 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_bgp.textfsm
--rw-r--r--   0        0        0     2146 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_bgp_detail.textfsm
--rw-r--r--   0        0        0     1815 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0      246 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_helper-address.textfsm
--rw-r--r--   0        0        0      185 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0      736 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_ospf_database.textfsm
--rw-r--r--   0        0        0      434 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_ospf_interface_brief.textfsm
--rw-r--r--   0        0        0      471 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_ospf_neighbor.textfsm
--rw-r--r--   0        0        0      734 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_ospf_summary.textfsm
--rw-r--r--   0        0        0     1062 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_route.textfsm
--rw-r--r--   0        0        0     1101 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ipv6_bgp_summary.textfsm
--rw-r--r--   0        0        0      358 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_isis_neighbors.textfsm
--rw-r--r--   0        0        0      190 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      627 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     1677 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_mac_address-table.textfsm
--rw-r--r--   0        0        0      257 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_mac_security_interface.textfsm
--rw-r--r--   0        0        0      303 2024-04-08 14:14:45.227635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_mac_security_mka_counters.textfsm
--rw-r--r--   0        0        0     1431 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_mac_security_participants_detail.textfsm
--rw-r--r--   0        0        0      279 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_mlag.textfsm
--rw-r--r--   0        0        0      716 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_module.textfsm
--rw-r--r--   0        0        0      564 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_pim_ipv4_interface.textfsm
--rw-r--r--   0        0        0      430 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_pim_ipv4_neighbor.textfsm
--rw-r--r--   0        0        0     1368 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_port-channel_summary.textfsm
--rw-r--r--   0        0        0     5405 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_processes_top_once.textfsm
--rw-r--r--   0        0        0      573 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_reload_cause.textfsm
--rw-r--r--   0        0        0      275 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_snmp_community.textfsm
--rw-r--r--   0        0        0      424 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_version.textfsm
--rw-r--r--   0        0        0     6202 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_vlan.textfsm
--rw-r--r--   0        0        0     4153 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_vrf.textfsm
--rw-r--r--   0        0        0      701 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_aaa_authentication_port-access_interface_all_client-status.textfsm
--rw-r--r--   0        0        0      344 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_arp_all-vrfs.textfsm
--rw-r--r--   0        0        0      604 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_bfd_all-vrfs.textfsm
--rw-r--r--   0        0        0      531 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_bgp_all-vrfs_all_summary.textfsm
--rw-r--r--   0        0        0      531 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_bgp_all_all-vrfs_summary.textfsm
--rw-r--r--   0        0        0     4832 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_interface.textfsm
--rw-r--r--   0        0        0     4773 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_interface_dom_detail.textfsm
--rw-r--r--   0        0        0      420 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_ip_route_all-vrfs.textfsm
--rw-r--r--   0        0        0      997 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_lldp_neighbors-info_detail.textfsm
--rw-r--r--   0        0        0      262 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_mac-address-table.textfsm
--rw-r--r--   0        0        0      380 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_ntp_associations.textfsm
--rw-r--r--   0        0        0      956 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_system.textfsm
--rw-r--r--   0        0        0     1150 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_vlan.textfsm
--rw-r--r--   0        0        0      678 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_vsf_detail.textfsm
--rw-r--r--   0        0        0      917 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_os_show_ap_bss-table_details.textfsm
--rw-r--r--   0        0        0      768 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_os_show_ap_database.textfsm
--rw-r--r--   0        0        0     1044 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_os_show_ap_database_long.textfsm
--rw-r--r--   0        0        0      977 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_os_show_ap_radio-database.textfsm
--rw-r--r--   0        0        0      757 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_os_show_arp.textfsm
--rw-r--r--   0        0        0      200 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_os_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0      314 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/aruba_os_show_ipv6_interface_brief.textfsm
--rw-r--r--   0        0        0      119 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/avaya_ers_show_interface_name.textfsm
--rw-r--r--   0        0        0      702 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/avaya_ers_show_logging_config.textfsm
--rw-r--r--   0        0        0      187 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/avaya_ers_show_mac-address-table.textfsm
--rw-r--r--   0        0        0      878 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/avaya_ers_show_mlt.textfsm
--rw-r--r--   0        0        0      607 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/avaya_ers_show_mlt_all-members.textfsm
--rw-r--r--   0        0        0     1825 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/avaya_ers_show_sys-info.textfsm
--rw-r--r--   0        0        0      495 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/avaya_ers_show_vlan.textfsm
--rw-r--r--   0        0        0      367 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/avaya_vsp_show_software.textfsm
--rw-r--r--   0        0        0      583 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/broadcom_icos_show_isdp_neighbors.textfsm
--rw-r--r--   0        0        0      631 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/broadcom_icos_show_lldp_remote-device_all.textfsm
--rw-r--r--   0        0        0      480 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/broadcom_icos_show_mac-addr-table.textfsm
--rw-r--r--   0        0        0     1513 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/broadcom_icos_show_version.textfsm
--rw-r--r--   0        0        0      382 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/broadcom_icos_show_vlan_brief.textfsm
--rw-r--r--   0        0        0      358 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_arp.textfsm
--rw-r--r--   0        0        0     5683 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_interfaces.textfsm
--rw-r--r--   0        0        0      695 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_interfaces_brief.textfsm
--rw-r--r--   0        0        0      367 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_lag_brief.textfsm
--rw-r--r--   0        0        0      416 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      906 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      384 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_mac-address.textfsm
--rw-r--r--   0        0        0     1120 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_metro.textfsm
--rw-r--r--   0        0        0      301 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_monitor.textfsm
--rw-r--r--   0        0        0     2278 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_running-config_vlan.textfsm
--rw-r--r--   0        0        0      851 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_span.textfsm
--rw-r--r--   0        0        0      351 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_topo.textfsm
--rw-r--r--   0        0        0     2990 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_trunk.textfsm
--rw-r--r--   0        0        0     1629 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_version.textfsm
--rw-r--r--   0        0        0     6614 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_interfaces.textfsm
--rw-r--r--   0        0        0      430 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_interfaces_brief.textfsm
--rw-r--r--   0        0        0      367 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_lag_brief.textfsm
--rw-r--r--   0        0        0      906 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     1071 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_metro.textfsm
--rw-r--r--   0        0        0      311 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_monitor_actual.textfsm
--rw-r--r--   0        0        0     1624 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_running-config_interface.textfsm
--rw-r--r--   0        0        0     2277 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_running-config_vlan.textfsm
--rw-r--r--   0        0        0      739 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_span.textfsm
--rw-r--r--   0        0        0      591 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_topo.textfsm
--rw-r--r--   0        0        0      167 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/checkpoint_gaia_fw_stat.textfsm
--rw-r--r--   0        0        0      192 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/checkpoint_gaia_show_arp_dynamic_all.textfsm
--rw-r--r--   0        0        0      398 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/checkpoint_gaia_show_asset_all.textfsm
--rw-r--r--   0        0        0      189 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/checkpoint_gaia_show_dns.textfsm
--rw-r--r--   0        0        0       71 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/checkpoint_gaia_show_domainname.textfsm
--rw-r--r--   0        0        0      849 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/checkpoint_gaia_show_interfaces_all.textfsm
--rw-r--r--   0        0        0      509 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/checkpoint_gaia_show_ipv6_route.textfsm
--rw-r--r--   0        0        0      159 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/checkpoint_gaia_show_lom.textfsm
--rw-r--r--   0        0        0      208 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/checkpoint_gaia_show_ntp_servers.textfsm
--rw-r--r--   0        0        0      550 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/checkpoint_gaia_show_route.textfsm
--rw-r--r--   0        0        0      236 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/checkpoint_gaia_show_version_all.textfsm
--rw-r--r--   0        0        0      115 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/checkpoint_gaia_show_virtual-system_all.textfsm
--rw-r--r--   0        0        0      419 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/ciena_saos_chassis_show_temperature.textfsm
--rw-r--r--   0        0        0     1010 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/ciena_saos_port_show.textfsm
--rw-r--r--   0        0        0      945 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/ciena_saos_rstp_show.textfsm
--rw-r--r--   0        0        0      623 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/ciena_saos_software_show.textfsm
--rw-r--r--   0        0        0      289 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/ciena_saos_ssh_server_show_key.textfsm
--rw-r--r--   0        0        0      556 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/ciena_saos_traffic-profiling_standard-profile_show.textfsm
--rw-r--r--   0        0        0      646 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/ciena_saos_vlan_show.textfsm
--rw-r--r--   0        0        0      714 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_apic_fabric_show_vlan_extended.textfsm
--rw-r--r--   0        0        0      695 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_dir.textfsm
--rw-r--r--   0        0        0      737 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_ping.textfsm
--rw-r--r--   0        0        0     6125 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_access-list.textfsm
--rw-r--r--   0        0        0      347 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_arp.textfsm
--rw-r--r--   0        0        0     9761 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_asp_drop.textfsm
--rw-r--r--   0        0        0      829 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_asp_table_vpn-context_detail.textfsm
--rw-r--r--   0        0        0     1377 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_bgp_summary.textfsm
--rw-r--r--   0        0        0      917 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_cpu_usage_detailed.textfsm
--rw-r--r--   0        0        0      438 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_crypto_ikev1_sa_detail.textfsm
--rw-r--r--   0        0        0     6136 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_crypto_ipsec_sa.textfsm
--rw-r--r--   0        0        0     3036 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_failover.textfsm
--rw-r--r--   0        0        0     4419 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_interface.textfsm
--rw-r--r--   0        0        0     7392 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_interface_detail.textfsm
--rw-r--r--   0        0        0      286 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_interface_ip_brief.textfsm
--rw-r--r--   0        0        0      320 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_inventory.textfsm
--rw-r--r--   0        0        0     6025 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_license_all.textfsm
--rw-r--r--   0        0        0     2352 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_logging.textfsm
--rw-r--r--   0        0        0      381 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_module.textfsm
--rw-r--r--   0        0        0      540 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_module_details.textfsm
--rw-r--r--   0        0        0      372 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_module_status.textfsm
--rw-r--r--   0        0        0      105 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_name.textfsm
--rw-r--r--   0        0        0     1624 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_nat.textfsm
--rw-r--r--   0        0        0      581 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_object-group_network.textfsm
--rw-r--r--   0        0        0      421 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_ospf_interface_brief.textfsm
--rw-r--r--   0        0        0      380 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_ospf_neighbor.textfsm
--rw-r--r--   0        0        0     1346 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_port-channel_summary.textfsm
--rw-r--r--   0        0        0      425 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_resource_usage.textfsm
--rw-r--r--   0        0        0     1793 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_route.textfsm
--rw-r--r--   0        0        0     2300 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_running-config_all_crypto_map.textfsm
--rw-r--r--   0        0        0      437 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_ikev1.textfsm
--rw-r--r--   0        0        0     1212 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_map.textfsm
--rw-r--r--   0        0        0     1726 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_running-config_ipsec.textfsm
--rw-r--r--   0        0        0      512 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_running-config_object_network.textfsm
--rw-r--r--   0        0        0     4906 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_running-config_tunnel-group.textfsm
--rw-r--r--   0        0        0     2556 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_version.textfsm
--rw-r--r--   0        0        0     1625 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb.textfsm
--rw-r--r--   0        0        0     1828 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_anyconnect.textfsm
--rw-r--r--   0        0        0     7479 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_detail_l2l.textfsm
--rw-r--r--   0        0        0     1126 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_xlate.textfsm
--rw-r--r--   0        0        0     1886 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ftd_show_vpn-sessiondb_anyconnect.textfsm
--rw-r--r--   0        0        0      481 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_dir.textfsm
--rw-r--r--   0        0        0      935 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_ping.textfsm
--rw-r--r--   0        0        0     1971 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_access-list.textfsm
--rw-r--r--   0        0        0      432 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_access-session.textfsm
--rw-r--r--   0        0        0      953 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_adjacency.textfsm
--rw-r--r--   0        0        0      355 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_alert_counters.textfsm
--rw-r--r--   0        0        0      310 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_aliases.textfsm
--rw-r--r--   0        0        0      402 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ap_cdp_neighbors.textfsm
--rw-r--r--   0        0        0      555 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ap_summary.textfsm
--rw-r--r--   0        0        0      615 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_archive.textfsm
--rw-r--r--   0        0        0      419 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_authentication_sessions.textfsm
--rw-r--r--   0        0        0     2737 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_authentication_sessions_method_details.textfsm
--rw-r--r--   0        0        0     2508 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_bfd_neighbors_details.textfsm
--rw-r--r--   0        0        0     1704 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_boot.textfsm
--rw-r--r--   0        0        0      264 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_capability_feature_routing.textfsm
--rw-r--r--   0        0        0      538 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors.textfsm
--rw-r--r--   0        0        0      937 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      317 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_clock.textfsm
--rw-r--r--   0        0        0     2327 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_controller_t1.textfsm
--rw-r--r--   0        0        0     6120 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_crypto_ipsec_sa_detail.textfsm
--rw-r--r--   0        0        0     2174 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_crypto_pki_certificates.textfsm
--rw-r--r--   0        0        0     1432 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_crypto_session_detail.textfsm
--rw-r--r--   0        0        0     1047 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_dhcp_lease.textfsm
--rw-r--r--   0        0        0      491 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_dmvpn.textfsm
--rw-r--r--   0        0        0     1367 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_dot1x_all.textfsm
--rw-r--r--   0        0        0      413 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_environment_power_all.textfsm
--rw-r--r--   0        0        0     1603 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_environment_temperature.textfsm
--rw-r--r--   0        0        0     1326 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_etherchannel_summary.textfsm
--rw-r--r--   0        0        0      224 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_file_systems.textfsm
--rw-r--r--   0        0        0      454 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_hosts_summary.textfsm
--rw-r--r--   0        0        0     1226 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_interface_link.textfsm
--rw-r--r--   0        0        0      320 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_interface_transceiver.textfsm
--rw-r--r--   0        0        0     2778 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_interfaces.textfsm
--rw-r--r--   0        0        0      423 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_interfaces_description.textfsm
--rw-r--r--   0        0        0      934 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_interfaces_status.textfsm
--rw-r--r--   0        0        0     1511 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_interfaces_switchport.textfsm
--rw-r--r--   0        0        0      570 2024-04-08 14:14:45.231635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_inventory.textfsm
--rw-r--r--   0        0        0     2587 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_access-lists.textfsm
--rw-r--r--   0        0        0      558 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_arp.textfsm
--rw-r--r--   0        0        0     2029 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_bgp.textfsm
--rw-r--r--   0        0        0     1706 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors.textfsm
--rw-r--r--   0        0        0     2011 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors_advertised-routes.textfsm
--rw-r--r--   0        0        0      884 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0     1761 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_bgp_vpnv4_all_neighbors.textfsm
--rw-r--r--   0        0        0     1286 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_cef.textfsm
--rw-r--r--   0        0        0     3323 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_cef_detail.textfsm
--rw-r--r--   0        0        0      740 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_device_tracking_all.textfsm
--rw-r--r--   0        0        0     2669 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_interfaces_detail.textfsm
--rw-r--r--   0        0        0      779 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_neighbors.textfsm
--rw-r--r--   0        0        0     2642 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_topology.textfsm
--rwxr-xr-x   0        0        0      459 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_flow_toptalkers.textfsm
--rw-r--r--   0        0        0     4260 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_http_server_status.textfsm
--rw-r--r--   0        0        0     1963 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_interface.textfsm
--rw-r--r--   0        0        0      306 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0     1378 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_mroute.textfsm
--rw-r--r--   0        0        0      645 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_nat_translations.textfsm
--rw-r--r--   0        0        0      776 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database.textfsm
--rw-r--r--   0        0        0     1362 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_network.textfsm
--rw-r--r--   0        0        0     1807 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_router.textfsm
--rw-r--r--   0        0        0      426 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_ospf_interface_brief.textfsm
--rw-r--r--   0        0        0      389 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_ospf_neighbor.textfsm
--rw-r--r--   0        0        0      436 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_prefix-list.textfsm
--rw-r--r--   0        0        0     2562 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_route.textfsm
--rw-r--r--   0        0        0     1389 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_route_summary.textfsm
--rw-r--r--   0        0        0      593 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_source_binding.textfsm
--rw-r--r--   0        0        0      474 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_vrf_interfaces.textfsm
--rw-r--r--   0        0        0      917 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ipv6_access-lists.textfsm
--rw-r--r--   0        0        0      426 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ipv6_interface_brief.textfsm
--rw-r--r--   0        0        0      387 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ipv6_neighbors.textfsm
--rw-r--r--   0        0        0      523 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ipv6_route.textfsm
--rw-r--r--   0        0        0      956 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_isdn_status.textfsm
--rw-r--r--   0        0        0      412 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_isis_neighbors.textfsm
--rw-r--r--   0        0        0      547 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_license.textfsm
--rw-r--r--   0        0        0      479 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0     2769 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     5837 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_logging.textfsm
--rw-r--r--   0        0        0     4137 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_mac-address-table.textfsm
--rw-r--r--   0        0        0     1088 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_module.textfsm
--rw-r--r--   0        0        0      585 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_module_online_diag.textfsm
--rw-r--r--   0        0        0     1138 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_module_status.textfsm
--rw-r--r--   0        0        0      760 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_module_submodule.textfsm
--rw-r--r--   0        0        0      350 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_mpls_interfaces.textfsm
--rw-r--r--   0        0        0      391 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_nve_peers.textfsm
--rw-r--r--   0        0        0      346 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_nve_vni.textfsm
--rw-r--r--   0        0        0     1215 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_object-group.textfsm
--rw-r--r--   0        0        0     1072 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_platform_diag.textfsm
--rw-r--r--   0        0        0      974 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_port-security_interface_interface.textfsm
--rw-r--r--   0        0        0      922 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_power_available.textfsm
--rw-r--r--   0        0        0      684 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_power_status.textfsm
--rw-r--r--   0        0        0      314 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_power_supplies.textfsm
--rw-r--r--   0        0        0      344 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_processes_cpu.textfsm
--rw-r--r--   0        0        0      640 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_processes_memory_sorted.textfsm
--rw-r--r--   0        0        0     3950 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_redundancy.textfsm
--rw-r--r--   0        0        0      312 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_rep_topology.textfsm
--rw-r--r--   0        0        0      784 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_route-map.textfsm
--rw-r--r--   0        0        0     3318 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_running-config_partition_access-list.textfsm
--rw-r--r--   0        0        0     1034 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_running-config_partition_route-map.textfsm
--rw-r--r--   0        0        0      359 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_snmp_community.textfsm
--rw-r--r--   0        0        0      802 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_snmp_group.textfsm
--rw-r--r--   0        0        0      668 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_snmp_user.textfsm
--rw-r--r--   0        0        0      413 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_spanning-tree.textfsm
--rw-r--r--   0        0        0     2018 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_standby.textfsm
--rw-r--r--   0        0        0      660 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_standby_brief.textfsm
--rw-r--r--   0        0        0      581 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_switch_detail.textfsm
--rw-r--r--   0        0        0      357 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_switch_detail_stack_ports.textfsm
--rw-r--r--   0        0        0     1009 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_tacacs.textfsm
--rw-r--r--   0        0        0     1759 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_version.textfsm
--rw-r--r--   0        0        0     6342 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_vlan.textfsm
--rw-r--r--   0        0        0     1374 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_vlans.textfsm
--rw-r--r--   0        0        0      684 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_vrf.textfsm
--rw-r--r--   0        0        0     1108 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_vrf_detail.textfsm
--rw-r--r--   0        0        0     1654 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_vrrp_all.textfsm
--rw-r--r--   0        0        0     1802 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_vrrp_brief.textfsm
--rw-r--r--   0        0        0     1109 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_vtp_status.textfsm
--rw-r--r--   0        0        0     1669 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_traceroute.textfsm
--rw-r--r--   0        0        0      971 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nvfis_show_bridge-settings.textfsm
--rw-r--r--   0        0        0      214 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nvfis_show_configuration_commit_changes.textfsm
--rw-r--r--   0        0        0      245 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nvfis_show_nic.textfsm
--rw-r--r--   0        0        0      159 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nvfis_show_running-config_snmp_enable.textfsm
--rw-r--r--   0        0        0      292 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nvfis_show_running-config_snmp_group.textfsm
--rw-r--r--   0        0        0      385 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nvfis_show_running-config_snmp_host.textfsm
--rw-r--r--   0        0        0      437 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nvfis_show_running-config_snmp_user.textfsm
--rw-r--r--   0        0        0      394 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nvfis_show_running-config_system_settings.textfsm
--rw-r--r--   0        0        0      516 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nvfis_show_running-config_system_time.textfsm
--rw-r--r--   0        0        0      309 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nvfis_show_running-config_system_upgrade.textfsm
--rw-r--r--   0        0        0      177 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nvfis_show_version.textfsm
--rw-r--r--   0        0        0      460 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_dir.textfsm
--rw-r--r--   0        0        0     1781 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_access-lists.textfsm
--rw-r--r--   0        0        0     1497 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_bgp_vrf_all_ipv4_unicast_detail.textfsm
--rw-r--r--   0        0        0     1856 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_bgp_vrf_all_ipv4_unicast_neighbors_routes.textfsm
--rw-r--r--   0        0        0      461 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors.textfsm
--rw-r--r--   0        0        0      689 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      203 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_clock.textfsm
--rw-r--r--   0        0        0      210 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_configuration_session_summary.textfsm
--rw-r--r--   0        0        0      954 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_cts_interface_all.textfsm
--rw-r--r--   0        0        0      233 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_cts_interface_brief.textfsm
--rw-r--r--   0        0        0     2143 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_environment.textfsm
--rw-r--r--   0        0        0      384 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_environment_temperature.textfsm
--rw-r--r--   0        0        0      147 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_feature.textfsm
--rw-r--r--   0        0        0      178 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_fex.textfsm
--rw-r--r--   0        0        0     1002 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_fex_id.textfsm
--rw-r--r--   0        0        0      491 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_flogi_database.textfsm
--rw-r--r--   0        0        0     1083 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_forwarding_adjacency.textfsm
--rw-r--r--   0        0        0     1041 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_forwarding_ipv4_route.textfsm
--rw-r--r--   0        0        0    18876 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_hardware_internal_bigsur_all-ports_detail.textfsm
--rw-r--r--   0        0        0       57 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_hostname.textfsm
--rw-r--r--   0        0        0     2393 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_hsrp_all.textfsm
--rw-r--r--   0        0        0     1630 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_interface.textfsm
--rw-r--r--   0        0        0     2212 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_interface_brief.textfsm
--rw-r--r--   0        0        0      358 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_interface_description.textfsm
--rw-r--r--   0        0        0      203 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_interface_snmp-ifindex.textfsm
--rw-r--r--   0        0        0      370 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_interface_status.textfsm
--rw-r--r--   0        0        0      669 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver.textfsm
--rw-r--r--   0        0        0     2240 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver_details.textfsm
--rw-r--r--   0        0        0      812 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_interfaces_switchport.textfsm
--rw-r--r--   0        0        0      500 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_inventory.textfsm
--rw-r--r--   0        0        0      716 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_adjacency.textfsm
--rw-r--r--   0        0        0      322 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_arp.textfsm
--rw-r--r--   0        0        0      448 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_arp_detail.textfsm
--rw-r--r--   0        0        0     2778 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_bgp.textfsm
--rw-r--r--   0        0        0     4875 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_neighbors.textfsm
--rw-r--r--   0        0        0      974 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0     1014 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary_vrf.textfsm
--rw-r--r--   0        0        0      714 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_community-list.textfsm
--rw-r--r--   0        0        0      283 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_relay_address.textfsm
--rw-r--r--   0        0        0     3956 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_snooping_statistics.textfsm
--rw-r--r--   0        0        0     5936 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_interface.textfsm
--rw-r--r--   0        0        0      414 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0     5167 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_interface_vrf_all.textfsm
--rw-r--r--   0        0        0      934 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_mroutes_vrf_all.textfsm
--rw-r--r--   0        0        0      665 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_msdp_summary_vrf_all.textfsm
--rw-r--r--   0        0        0      680 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_database.textfsm
--rw-r--r--   0        0        0      526 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_interface_brief.textfsm
--rw-r--r--   0        0        0      375 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_neighbor.textfsm
--rw-r--r--   0        0        0      453 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_pim_group-range_vrf_all.textfsm
--rw-r--r--   0        0        0      480 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_pim_interface_brief_vrf_all.textfsm
--rw-r--r--   0        0        0      636 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_pim_neighbor_vrf_all.textfsm
--rw-r--r--   0        0        0      546 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_pim_rp_vrf_all.textfsm
--rw-r--r--   0        0        0     2090 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_route.textfsm
--rw-r--r--   0        0        0      244 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ipv6_interface_brief.textfsm
--rw-r--r--   0        0        0      260 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_l2rib_internal_permanently-frozen-list.textfsm
--rw-r--r--   0        0        0      411 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_license_usage.textfsm
--rw-r--r--   0        0        0      345 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      733 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      310 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_mac_address-table.textfsm
--rw-r--r--   0        0        0      351 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_module.textfsm
--rw-r--r--   0        0        0      302 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_nve_peers.textfsm
--rw-r--r--   0        0        0      495 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_nve_vni.textfsm
--rw-r--r--   0        0        0     2786 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_port-channel_summary.textfsm
--rw-r--r--   0        0        0      234 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_processes_cpu.textfsm
--rw-r--r--   0        0        0      698 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_route-map.textfsm
--rw-r--r--   0        0        0      495 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_spanning-tree_root.textfsm
--rw-r--r--   0        0        0      339 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_switching-mode.textfsm
--rw-r--r--   0        0        0      312 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_vdc.textfsm
--rwxr-xr-x   0        0        0      697 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_version.textfsm
--rw-r--r--   0        0        0     6325 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_vlan.textfsm
--rw-r--r--   0        0        0       99 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_vpc.textfsm
--rw-r--r--   0        0        0      279 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_vrf.textfsm
--rw-r--r--   0        0        0      751 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_vrf_detail.textfsm
--rw-r--r--   0        0        0      239 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_vrf_interface.textfsm
--rw-r--r--   0        0        0      403 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_interfaces_description.textfsm
--rw-r--r--   0        0        0      594 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_interfaces_status.textfsm
--rw-r--r--   0        0        0     1528 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_interfaces_switchport.textfsm
--rw-r--r--   0        0        0      907 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_ip_interface.textfsm
--rw-r--r--   0        0        0      411 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      336 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_mac_address-table.textfsm
--rw-r--r--   0        0        0      601 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_system.textfsm
--rw-r--r--   0        0        0      116 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_system_id.textfsm
--rw-r--r--   0        0        0      442 2024-04-08 14:14:45.235635 ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_version.textfsm
--rw-r--r--   0        0        0      828 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_vlan.textfsm
--rw-r--r--   0        0        0     3155 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a.textfsm
--rw-r--r--   0        0        0     4795 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a_cleanair_config.textfsm
--rw-r--r--   0        0        0     1683 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_advanced_802.11a_channel.textfsm
--rw-r--r--   0        0        0     2729 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_config_general.textfsm
--rw-r--r--   0        0        0      643 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_image_all.textfsm
--rw-r--r--   0        0        0      524 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_summary.textfsm
--rw-r--r--   0        0        0      780 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_band-select.textfsm
--rw-r--r--   0        0        0      215 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_boot.textfsm
--rw-r--r--   0        0        0      661 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_cdp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     1435 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_client_detail.textfsm
--rw-r--r--   0        0        0      292 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_exclusionlist.textfsm
--rw-r--r--   0        0        0      355 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_flexconnect_group_summary.textfsm
--rw-r--r--   0        0        0     1425 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_detailed_id.textfsm
--rw-r--r--   0        0        0      347 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_group_summary.textfsm
--rw-r--r--   0        0        0      492 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_summary.textfsm
--rw-r--r--   0        0        0      428 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_inventory.textfsm
--rw-r--r--   0        0        0      475 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_anchor.textfsm
--rw-r--r--   0        0        0      749 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_sum.textfsm
--rw-r--r--   0        0        0      655 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_port_summary.textfsm
--rw-r--r--   0        0        0     2911 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_radius_summary.textfsm
--rw-r--r--   0        0        0      842 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_detail.textfsm
--rw-r--r--   0        0        0      970 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_summary.textfsm
--rw-r--r--   0        0        0      431 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_rf-profile_summary.textfsm
--rw-r--r--   0        0        0      997 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_stats_port_summary.textfsm
--rw-r--r--   0        0        0     1238 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_sysinfo.textfsm
--rw-r--r--   0        0        0     1450 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_tacacs_summary.textfsm
--rw-r--r--   0        0        0      906 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_time.textfsm
--rw-r--r--   0        0        0      420 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_wlan_sum.textfsm
--rw-r--r--   0        0        0     6223 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_admin_show_controller_fabric_health.textfsm
--rw-r--r--   0        0        0     1379 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_admin_show_environment_fan.textfsm
--rw-r--r--   0        0        0      309 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_admin_show_environment_power.textfsm
--rw-r--r--   0        0        0      415 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_admin_show_inventory.textfsm
--rw-r--r--   0        0        0      179 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_admin_show_platform.textfsm
--rw-r--r--   0        0        0      425 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_admin_show_vm.textfsm
--rw-r--r--   0        0        0      504 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_dir.textfsm
--rw-r--r--   0        0        0      921 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_ping.textfsm
--rw-r--r--   0        0        0      537 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_arp.textfsm
--rw-r--r--   0        0        0      838 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_asic-errors_all_location.textfsm
--rw-r--r--   0        0        0      179 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_bfd_sessions.textfsm
--rw-r--r--   0        0        0     1905 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_bgp.textfsm
--rw-r--r--   0        0        0      725 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_bgp_instance_all_summary.textfsm
--rw-r--r--   0        0        0     5397 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_bgp_neighbors.textfsm
--rw-r--r--   0        0        0      228 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_bgp_vrf_all_ipv4_unicast_summary.textfsm
--rw-r--r--   0        0        0      513 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_cdp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     1544 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_cef_drops_location.textfsm
--rw-r--r--   0        0        0      337 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_configuration_commit_list.textfsm
--rw-r--r--   0        0        0      347 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_controller_fabric_plane_all.textfsm
--rw-r--r--   0        0        0     2208 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_controllers_HundredGigabitEthernet.textfsm
--rw-r--r--   0        0        0     2281 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_controllers_all_phy.textfsm
--rw-r--r--   0        0        0     2823 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_egress_location.textfsm
--rw-r--r--   0        0        0     1961 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_ingress_location.textfsm
--rw-r--r--   0        0        0      426 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_egress_location.textfsm
--rw-r--r--   0        0        0     1406 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_ingress_location.textfsm
--rw-r--r--   0        0        0     4937 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_controllers_hundredgige_all.textfsm
--rw-r--r--   0        0        0      288 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_dhcp_ipv4_proxy_binding.textfsm
--rw-r--r--   0        0        0     7430 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_drops_np_all.textfsm
--rw-r--r--   0        0        0      518 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_hsrp.textfsm
--rw-r--r--   0        0        0      665 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_install_active.textfsm
--rw-r--r--   0        0        0      268 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_interface_brief.textfsm
--rw-r--r--   0        0        0      957 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_interfaces.textfsm
--rw-r--r--   0        0        0      353 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_interfaces_summary.textfsm
--rw-r--r--   0        0        0      269 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_inventory.textfsm
--rw-r--r--   0        0        0      571 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0      196 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0     1719 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_ip_route.textfsm
--rw-r--r--   0        0        0     1869 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_ipv4_interface.textfsm
--rw-r--r--   0        0        0      288 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_ipv4_vrf_all_interface_brief.textfsm
--rw-r--r--   0        0        0      431 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_ipv6_neighbors.textfsm
--rw-r--r--   0        0        0      288 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_isis_neighbors.textfsm
--rw-r--r--   0        0        0      380 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0     1387 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      694 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_lpts_pifib_hardware_police_location.textfsm
--rw-r--r--   0        0        0      398 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_mpls_ldp_neighbor_brief.textfsm
--rw-r--r--   0        0        0      362 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_ospf_neighbor.textfsm
--rw-r--r--   0        0        0      486 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_ospf_vrf_all_interface_brief.textfsm
--rw-r--r--   0        0        0      480 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_ospf_vrf_all_neighbor.textfsm
--rw-r--r--   0        0        0      359 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_group-map.textfsm
--rw-r--r--   0        0        0      488 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_interface.textfsm
--rw-r--r--   0        0        0      447 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_neighbor.textfsm
--rw-r--r--   0        0        0      262 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_pim_neighbor.textfsm
--rw-r--r--   0        0        0     1074 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_platform_summary_location_all.textfsm
--rw-r--r--   0        0        0      205 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_processes_cpu.textfsm
--rw-r--r--   0        0        0      187 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_redundancy_summary.textfsm
--rw-r--r--   0        0        0      226 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_rsvp_neighbors.textfsm
--rw-r--r--   0        0        0      871 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_version.textfsm
--rw-r--r--   0        0        0      339 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_version_brief.textfsm
--rw-r--r--   0        0        0      422 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_vrf_all_detail.textfsm
--rw-r--r--   0        0        0      322 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/dell_force10_show_arp.textfsm
--rw-r--r--   0        0        0      231 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/dell_force10_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0      211 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/dell_force10_show_version.textfsm
--rw-r--r--   0        0        0      825 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/dell_force10_show_vlan.textfsm
--rw-r--r--   0        0        0      274 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/dell_force10_show_vlan_brief.textfsm
--rw-r--r--   0        0        0      295 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/dell_powerconnect_show_bridge_address_table.textfsm
--rw-r--r--   0        0        0      193 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/dell_powerconnect_show_interfaces_description.textfsm
--rw-r--r--   0        0        0      592 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/dell_powerconnect_show_interfaces_status.textfsm
--rw-r--r--   0        0        0      333 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/dlink_ds_show_arpentry.textfsm
--rw-r--r--   0        0        0     4086 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/eltex_show_interface.textfsm
--rw-r--r--   0        0        0     2079 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/eltex_show_interfaces_description.textfsm
--rw-r--r--   0        0        0     2498 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/eltex_show_interfaces_status.textfsm
--rw-r--r--   0        0        0     2779 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/eltex_show_interfaces_switchport.textfsm
--rw-r--r--   0        0        0     1516 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/eltex_show_ip_interface.textfsm
--rw-r--r--   0        0        0     2262 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/eltex_show_system.textfsm
--rw-r--r--   0        0        0      431 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/eltex_show_system_id.textfsm
--rw-r--r--   0        0        0     1188 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/eltex_show_vlan.textfsm
--rw-r--r--   0        0        0      663 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/ericsson_ipos_show_arp.textfsm
--rw-r--r--   0        0        0      433 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/ericsson_ipos_show_isis_adjacency.textfsm
--rw-r--r--   0        0        0      168 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/ericsson_ipos_show_version.textfsm
--rw-r--r--   0        0        0     2838 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/extreme_exos_show_ipconfig.textfsm
--rw-r--r--   0        0        0      448 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/extreme_exos_show_ports_description.textfsm
--rw-r--r--   0        0        0     1948 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/extreme_exos_show_ports_information.textfsm
--rw-r--r--   0        0        0      835 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/extreme_exos_show_ports_information_detail.textfsm
--rw-r--r--   0        0        0     1367 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/extreme_exos_show_sharing.textfsm
--rw-r--r--   0        0        0      416 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/extreme_exos_show_vlan_description.textfsm
--rw-r--r--   0        0        0      574 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/fortinet_get_router_info_bgp_summary.textfsm
--rw-r--r--   0        0        0      252 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/fortinet_get_system_arp.textfsm
--rw-r--r--   0        0        0     2048 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/fortinet_get_system_ha_status.textfsm
--rw-r--r--   0        0        0     9094 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/fortinet_get_system_interface.textfsm
--rw-r--r--   0        0        0      689 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/fortinet_get_system_interface_physical.textfsm
--rw-r--r--   0        0        0     2931 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/fortinet_get_system_status.textfsm
--rw-r--r--   0        0        0      248 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_arp.textfsm
--rw-r--r--   0        0        0      200 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_clock.textfsm
--rw-r--r--   0        0        0      519 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_counters_bound_interface.textfsm
--rw-r--r--   0        0        0      666 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_device_manuinfo.textfsm
--rw-r--r--   0        0        0     8619 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_interface.textfsm
--rw-r--r--   0        0        0     1208 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_interface_brief.textfsm
--rw-r--r--   0        0        0     1600 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_ip_interface.textfsm
--rw-r--r--   0        0        0      634 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_ip_routing-table.textfsm
--rw-r--r--   0        0        0      195 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance.textfsm
--rw-r--r--   0        0        0     5480 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance_instance-name.textfsm
--rw-r--r--   0        0        0      777 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_link-aggregation_verbose.textfsm
--rw-r--r--   0        0        0      647 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_list.textfsm
--rw-r--r--   0        0        0      932 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_verbose.textfsm
--rw-r--r--   0        0        0      195 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_mac-address.textfsm
--rw-r--r--   0        0        0      642 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_vlan_all.textfsm
--rw-r--r--   0        0        0      116 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_vlan_brief.textfsm
--rw-r--r--   0        0        0      343 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_arp.textfsm
--rw-r--r--   0        0        0      625 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_cdp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      710 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_interfaces.textfsm
--rw-r--r--   0        0        0      971 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_interfaces_brief.textfsm
--rw-r--r--   0        0        0      622 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_ip.textfsm
--rw-r--r--   0        0        0      383 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_ip_route.textfsm
--rw-r--r--   0        0        0      706 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device.textfsm
--rw-r--r--   0        0        0     1699 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device_detail.textfsm
--rw-r--r--   0        0        0      252 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_mac-address.textfsm
--rw-r--r--   0        0        0      453 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_port-security.textfsm
--rw-r--r--   0        0        0     1345 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_system.textfsm
--rw-r--r--   0        0        0      385 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_tech_buffers.textfsm
--rw-r--r--   0        0        0      407 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_trunks.textfsm
--rw-r--r--   0        0        0      300 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_vlans.textfsm
--rw-r--r--   0        0        0      371 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_board.textfsm
--rw-r--r--   0        0        0      212 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_board_serial-number.textfsm
--rw-r--r--   0        0        0       98 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_cpu.textfsm
--rw-r--r--   0        0        0      107 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_mem.textfsm
--rw-r--r--   0        0        0     1065 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_ont_autofind.textfsm
--rw-r--r--   0        0        0     5899 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_ont_info_by-sn_sn.textfsm
--rw-r--r--   0        0        0      339 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_ont_info_description.textfsm
--rw-r--r--   0        0        0      553 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_ont_info_fsp.textfsm
--rw-r--r--   0        0        0      466 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_ont_info_summary_ont.textfsm
--rw-r--r--   0        0        0      424 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_ont_info_summary_sn.textfsm
--rw-r--r--   0        0        0     2198 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_port_info.textfsm
--rw-r--r--   0        0        0      375 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_sysman_service_state.textfsm
--rw-r--r--   0        0        0      201 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_sysuptime.textfsm
--rw-r--r--   0        0        0      246 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_temperature.textfsm
--rw-r--r--   0        0        0     1043 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_version.textfsm
--rw-r--r--   0        0        0     1392 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_acl_all.textfsm
--rw-r--r--   0        0        0      530 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_arp_all.textfsm
--rw-r--r--   0        0        0      500 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_arp_brief.textfsm
--rw-r--r--   0        0        0     4401 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_interface.textfsm
--rw-r--r--   0        0        0      498 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_interface_brief.textfsm
--rw-r--r--   0        0        0      376 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_interface_description.textfsm
--rw-r--r--   0        0        0     2065 2024-04-08 14:14:45.239636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_ip_routing-table_verbose.textfsm
--rw-r--r--   0        0        0      246 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_ip_vpn-instance.textfsm
--rw-r--r--   0        0        0      346 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_ip_vpn-instance_interface.textfsm
--rw-r--r--   0        0        0      857 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_ipv6_neighbors.textfsm
--rw-r--r--   0        0        0      435 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_isis_peer.textfsm
--rw-r--r--   0        0        0     1843 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_lldp_neighbor.textfsm
--rw-r--r--   0        0        0      312 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_mac-address.textfsm
--rw-r--r--   0        0        0      713 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_nat_server.textfsm
--rw-r--r--   0        0        0     7802 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_port_vlan.textfsm
--rw-r--r--   0        0        0      193 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_service-set_all.textfsm
--rw-r--r--   0        0        0     1084 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_service-set_id_id.textfsm
--rw-r--r--   0        0        0       96 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_sn_license.textfsm
--rw-r--r--   0        0        0      424 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_snmp-agent_community_read.textfsm
--rw-r--r--   0        0        0     1346 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_startup.textfsm
--rw-r--r--   0        0        0      390 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_temperature.textfsm
--rw-r--r--   0        0        0      522 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_traffic-filter_applied-record.textfsm
--rw-r--r--   0        0        0      505 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_version.textfsm
--rw-r--r--   0        0        0     1550 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_vlan.textfsm
--rw-r--r--   0        0        0    61971 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/index
--rw-r--r--   0        0        0      536 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ipinfusion_ocnos_show_lldp_table.textfsm
--rw-r--r--   0        0        0      319 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_arp_no-resolve.textfsm
--rw-r--r--   0        0        0     3195 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_interfaces.textfsm
--rw-r--r--   0        0        0      803 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_status.textfsm
--rw-r--r--   0        0        0      341 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_chassis_firmware.textfsm
--rw-r--r--   0        0        0     4354 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_chassis_hardware.textfsm
--rw-r--r--   0        0        0      735 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_ethernet-switching_table.textfsm
--rw-r--r--   0        0        0      662 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_interfaces.textfsm
--rw-r--r--   0        0        0      267 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_isis_adjacency.textfsm
--rw-r--r--   0        0        0      603 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_lacp_interfaces.textfsm
--rw-r--r--   0        0        0      389 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      298 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_ospf_neighbor.textfsm
--rw-r--r--   0        0        0     1374 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_system_uptime.textfsm
--rw-r--r--   0        0        0     4359 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_version.textfsm
--rw-r--r--   0        0        0      318 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_vlans.textfsm
--rw-r--r--   0        0        0      844 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/juniper_screenos_get_route.textfsm
--rw-r--r--   0        0        0      338 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/linux_arp_-a.textfsm
--rw-r--r--   0        0        0      919 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/linux_ip_address_show.textfsm
--rw-r--r--   0        0        0      863 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/linux_ip_link_show.textfsm
--rw-r--r--   0        0        0      618 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/linux_ip_route_show.textfsm
--rw-r--r--   0        0        0      134 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/linux_ip_vrf_show.textfsm
--rw-r--r--   0        0        0      660 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_monitor_name_once.textfsm
--rw-r--r--   0        0        0      810 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_poe_print_without-paging.textfsm
--rw-r--r--   0        0        0      473 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_print.textfsm
--rw-r--r--   0        0        0      926 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_interface_print_terse_without-paging.textfsm
--rw-r--r--   0        0        0      328 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ip_address_export_verbose.textfsm
--rw-r--r--   0        0        0      539 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ip_address_print.textfsm
--rw-r--r--   0        0        0      396 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ip_arp_print_without-paging.textfsm
--rw-r--r--   0        0        0      955 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ip_dhcp-server_lease_print_without-paging.textfsm
--rw-r--r--   0        0        0      618 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_address-list_print_terse.textfsm
--rw-r--r--   0        0        0     2499 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_filter_print_all_without-paging.textfsm
--rw-r--r--   0        0        0     2229 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_nat_print_all_without-paging.textfsm
--rw-r--r--   0        0        0      816 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ip_route_print_terse.textfsm
--rw-r--r--   0        0        0      436 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ipv6_neighbor_print_without-paging.textfsm
--rw-r--r--   0        0        0      758 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_log_print_detail_without-paging.textfsm
--rw-r--r--   0        0        0      637 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ping.textfsm
--rw-r--r--   0        0        0     4409 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_routing_bgp_peer_print_status_without-paging.textfsm
--rw-r--r--   0        0        0      758 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_routing_ospf_neighbor_print_terse_without-paging.textfsm
--rw-r--r--   0        0        0      483 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_snmp_community_print_without-paging.textfsm
--rw-r--r--   0        0        0      470 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_system_clock_print.textfsm
--rw-r--r--   0        0        0      671 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_system_routerboard_print.textfsm
--rw-r--r--   0        0        0      445 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_user_active_print.textfsm
--rw-r--r--   0        0        0      169 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_debug_swm_status.textfsm
--rw-r--r--   0        0        0      369 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_arp_all.textfsm
--rw-r--r--   0        0        0      249 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_counter_global.textfsm
--rw-r--r--   0        0        0     1943 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_high-availability_all.textfsm
--rw-r--r--   0        0        0      252 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_interface_hardware.textfsm
--rw-r--r--   0        0        0      333 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_interface_logical.textfsm
--rw-r--r--   0        0        0      964 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_interface_management.textfsm
--rw-r--r--   0        0        0      415 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_jobs_all.textfsm
--rw-r--r--   0        0        0      258 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_mac_all.textfsm
--rw-r--r--   0        0        0      729 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_running_nat-policy.textfsm
--rw-r--r--   0        0        0      794 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_running_security-policy.textfsm
--rw-r--r--   0        0        0      856 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_system_info.textfsm
--rw-r--r--   0        0        0      975 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_test_security-policy-match.textfsm
--rw-r--r--   0        0        0      914 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ruckus_fastiron_show_arp.textfsm
--rw-r--r--   0        0        0      740 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ruckus_fastiron_show_interfaces.textfsm
--rw-r--r--   0        0        0      602 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ruckus_fastiron_show_interfaces_brief.textfsm
--rw-r--r--   0        0        0      285 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ruckus_fastiron_show_mac-address.textfsm
--rw-r--r--   0        0        0      263 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ruckus_fastiron_show_media_validation.textfsm
--rw-r--r--   0        0        0     1049 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ruckus_fastiron_show_version.textfsm
--rw-r--r--   0        0        0     2679 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ruckus_fastiron_show_vlan.textfsm
--rw-r--r--   0        0        0      433 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgerouter_show_arp.textfsm
--rw-r--r--   0        0        0      404 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgerouter_show_dhcp_leases.textfsm
--rw-r--r--   0        0        0      286 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgerouter_show_dhcpv6_server_leases.textfsm
--rw-r--r--   0        0        0      324 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgerouter_show_interfaces.textfsm
--rw-r--r--   0        0        0      307 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgerouter_show_interfaces_ethernet_physical.textfsm
--rw-r--r--   0        0        0      911 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgerouter_show_ip_route.textfsm
--rw-r--r--   0        0        0      269 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgerouter_show_ipv6_neighbors.textfsm
--rw-r--r--   0        0        0      501 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgerouter_show_ipv6_route.textfsm
--rw-r--r--   0        0        0      723 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgerouter_show_nat_rules.textfsm
--rw-r--r--   0        0        0      380 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgerouter_show_version.textfsm
--rw-r--r--   0        0        0      336 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgeswitch_show_arp.textfsm
--rw-r--r--   0        0        0      569 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgeswitch_show_version.textfsm
--rw-r--r--   0        0        0      219 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgeswitch_show_vlan.textfsm
--rw-r--r--   0        0        0      470 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/vmware_nsxv_show_ip_bgp_neighbors.textfsm
--rw-r--r--   0        0        0      307 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/vmware_nsxv_show_ip_route.textfsm
--rw-r--r--   0        0        0      303 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/vyatta_vyos_show_arp.textfsm
--rw-r--r--   0        0        0      374 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/vyatta_vyos_show_interfaces.textfsm
--rw-r--r--   0        0        0      859 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/vyatta_vyos_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0      263 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/watchguard_firebox_show_arp.textfsm
--rw-r--r--   0        0        0     1181 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/yamaha_show_environment.textfsm
--rw-r--r--   0        0        0      490 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/yamaha_show_ip_route.textfsm
--rw-r--r--   0        0        0      626 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_firewall_acl_get.textfsm
--rw-r--r--   0        0        0      402 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_intf_group_get.textfsm
--rw-r--r--   0        0        0      595 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_ipalias_get.textfsm
--rw-r--r--   0        0        0      425 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_lan_get.textfsm
--rw-r--r--   0        0        0      678 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_lan_get_--Name_name.textfsm
--rw-r--r--   0        0        0      459 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_lanhosts_get.textfsm
--rw-r--r--   0        0        0      664 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_nat_addr_map_get.textfsm
--rw-r--r--   0        0        0      751 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_nat_get.textfsm
--rw-r--r--   0        0        0      629 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_snmp_get.textfsm
--rw-r--r--   0        0        0      355 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_static_dhcp_get.textfsm
--rw-r--r--   0        0        0      635 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_static_route_get.textfsm
--rw-r--r--   0        0        0      539 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_wlan_get.textfsm
--rw-r--r--   0        0        0      857 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_sys_atsh.textfsm
--rw-r--r--   0        0        0      337 2024-04-08 14:14:45.243636 ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_zycli_Ethctl_media-type.textfsm
--rw-r--r--   0        0        0     3146 2024-04-08 14:14:53.287627 ntc_templates-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 ntc_templates-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0      601 2024-05-29 21:22:06.793360 ntc_templates-5.1.0/LICENSE
+-rw-r--r--   0        0        0     2842 2024-05-29 21:22:06.793360 ntc_templates-5.1.0/README.md
+-rw-r--r--   0        0        0      260 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/__init__.py
+-rw-r--r--   0        0        0     2292 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/parse.py
+-rw-r--r--   0        0        0      728 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_aos_show_vlan.textfsm
+-rw-r--r--   0        0        0      170 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_oam_mac-ping.textfsm
+-rw-r--r--   0        0        0      371 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_lag.textfsm
+-rw-r--r--   0        0        0      641 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_port.textfsm
+-rw-r--r--   0        0        0      475 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_bgp_routes_vpn-ipv4.textfsm
+-rw-r--r--   0        0        0      526 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_bgp_summary_family.textfsm
+-rw-r--r--   0        0        0      668 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_interface.textfsm
+-rw-r--r--   0        0        0      318 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_isis_adjacency.textfsm
+-rw-r--r--   0        0        0      336 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_isis_interface.textfsm
+-rw-r--r--   0        0        0      619 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_ldp_interface.textfsm
+-rw-r--r--   0        0        0      608 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_mpls_interface.textfsm
+-rw-r--r--   0        0        0      512 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_mpls_lsp.textfsm
+-rw-r--r--   0        0        0      547 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_ospf_interface.textfsm
+-rw-r--r--   0        0        0      425 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_pim_interface.textfsm
+-rw-r--r--   0        0        0      649 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_rsvp_interface.textfsm
+-rw-r--r--   0        0        0      544 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_service_id_base.textfsm
+-rw-r--r--   0        0        0      665 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_service_sap-using.textfsm
+-rw-r--r--   0        0        0      598 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_service_sdp-using.textfsm
+-rw-r--r--   0        0        0      642 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_service_sdp.textfsm
+-rw-r--r--   0        0        0      522 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_system_cpu.textfsm
+-rw-r--r--   0        0        0      355 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_arp.textfsm
+-rw-r--r--   0        0        0      184 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_etherchannel_summary.textfsm
+-rw-r--r--   0        0        0     1647 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_interface.textfsm
+-rw-r--r--   0        0        0     1824 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_interface_switchport.textfsm
+-rw-r--r--   0        0        0      883 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_ip_route.textfsm
+-rw-r--r--   0        0        0     1582 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      222 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_mac_address-table.textfsm
+-rw-r--r--   0        0        0      706 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_static-channel-group.textfsm
+-rw-r--r--   0        0        0      831 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_system.textfsm
+-rw-r--r--   0        0        0     1243 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_vlan_all.textfsm
+-rw-r--r--   0        0        0      371 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_bash_df_-h.textfsm
+-rw-r--r--   0        0        0      430 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_dir_flash.textfsm
+-rw-r--r--   0        0        0      121 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_boot-config.textfsm
+-rw-r--r--   0        0        0      226 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_clock.textfsm
+-rw-r--r--   0        0        0      524 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_environment_cooling.textfsm
+-rw-r--r--   0        0        0      525 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_environment_temperature.textfsm
+-rw-r--r--   0        0        0      107 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_hostname.textfsm
+-rw-r--r--   0        0        0      897 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_interfaces.textfsm
+-rw-r--r--   0        0        0      443 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_interfaces_description.textfsm
+-rw-r--r--   0        0        0      408 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0      313 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver.textfsm
+-rw-r--r--   0        0        0      757 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver_detail.textfsm
+-rw-r--r--   0        0        0      671 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_inventory.textfsm
+-rw-r--r--   0        0        0      517 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_access-lists.textfsm
+-rw-r--r--   0        0        0      246 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_arp.textfsm
+-rw-r--r--   0        0        0      664 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_bgp.textfsm
+-rw-r--r--   0        0        0     2146 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_bgp_detail.textfsm
+-rw-r--r--   0        0        0     1815 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0      246 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_helper-address.textfsm
+-rw-r--r--   0        0        0      185 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0      736 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_ospf_database.textfsm
+-rw-r--r--   0        0        0      434 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_ospf_interface_brief.textfsm
+-rw-r--r--   0        0        0      471 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0      734 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_ospf_summary.textfsm
+-rw-r--r--   0        0        0     1062 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_route.textfsm
+-rw-r--r--   0        0        0     1101 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ipv6_bgp_summary.textfsm
+-rw-r--r--   0        0        0      358 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_isis_neighbors.textfsm
+-rw-r--r--   0        0        0      190 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      627 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     1677 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_mac_address-table.textfsm
+-rw-r--r--   0        0        0      257 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_mac_security_interface.textfsm
+-rw-r--r--   0        0        0      303 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_mac_security_mka_counters.textfsm
+-rw-r--r--   0        0        0     1431 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_mac_security_participants_detail.textfsm
+-rw-r--r--   0        0        0      279 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_mlag.textfsm
+-rw-r--r--   0        0        0      716 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_module.textfsm
+-rw-r--r--   0        0        0      564 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_pim_ipv4_interface.textfsm
+-rw-r--r--   0        0        0      430 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_pim_ipv4_neighbor.textfsm
+-rw-r--r--   0        0        0     1368 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_port-channel_summary.textfsm
+-rw-r--r--   0        0        0     5405 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_processes_top_once.textfsm
+-rw-r--r--   0        0        0      573 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_reload_cause.textfsm
+-rw-r--r--   0        0        0      275 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_snmp_community.textfsm
+-rw-r--r--   0        0        0      424 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_version.textfsm
+-rw-r--r--   0        0        0     6202 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_vlan.textfsm
+-rw-r--r--   0        0        0     4153 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_vrf.textfsm
+-rw-r--r--   0        0        0      701 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_aaa_authentication_port-access_interface_all_client-status.textfsm
+-rw-r--r--   0        0        0      344 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_arp_all-vrfs.textfsm
+-rw-r--r--   0        0        0      604 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_bfd_all-vrfs.textfsm
+-rw-r--r--   0        0        0      531 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_bgp_all-vrfs_all_summary.textfsm
+-rw-r--r--   0        0        0      531 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_bgp_all_all-vrfs_summary.textfsm
+-rw-r--r--   0        0        0     4832 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_interface.textfsm
+-rw-r--r--   0        0        0     4773 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_interface_dom_detail.textfsm
+-rw-r--r--   0        0        0      420 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_ip_route_all-vrfs.textfsm
+-rw-r--r--   0        0        0      997 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_lldp_neighbors-info_detail.textfsm
+-rw-r--r--   0        0        0      262 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_mac-address-table.textfsm
+-rw-r--r--   0        0        0      380 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_ntp_associations.textfsm
+-rw-r--r--   0        0        0      956 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_system.textfsm
+-rw-r--r--   0        0        0     1150 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_vlan.textfsm
+-rw-r--r--   0        0        0      678 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_vsf_detail.textfsm
+-rw-r--r--   0        0        0      917 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_os_show_ap_bss-table_details.textfsm
+-rw-r--r--   0        0        0      768 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_os_show_ap_database.textfsm
+-rw-r--r--   0        0        0     1044 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_os_show_ap_database_long.textfsm
+-rw-r--r--   0        0        0      977 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_os_show_ap_radio-database.textfsm
+-rw-r--r--   0        0        0      757 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_os_show_arp.textfsm
+-rw-r--r--   0        0        0      200 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_os_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0      314 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/aruba_os_show_ipv6_interface_brief.textfsm
+-rw-r--r--   0        0        0      119 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/avaya_ers_show_interface_name.textfsm
+-rw-r--r--   0        0        0      702 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/avaya_ers_show_logging_config.textfsm
+-rw-r--r--   0        0        0      187 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/avaya_ers_show_mac-address-table.textfsm
+-rw-r--r--   0        0        0      878 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/avaya_ers_show_mlt.textfsm
+-rw-r--r--   0        0        0      607 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/avaya_ers_show_mlt_all-members.textfsm
+-rw-r--r--   0        0        0     1825 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/avaya_ers_show_sys-info.textfsm
+-rw-r--r--   0        0        0      495 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/avaya_ers_show_vlan.textfsm
+-rw-r--r--   0        0        0      367 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/avaya_vsp_show_software.textfsm
+-rw-r--r--   0        0        0      583 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/broadcom_icos_show_isdp_neighbors.textfsm
+-rw-r--r--   0        0        0      631 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/broadcom_icos_show_lldp_remote-device_all.textfsm
+-rw-r--r--   0        0        0      480 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/broadcom_icos_show_mac-addr-table.textfsm
+-rw-r--r--   0        0        0     1513 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/broadcom_icos_show_version.textfsm
+-rw-r--r--   0        0        0      382 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/broadcom_icos_show_vlan_brief.textfsm
+-rw-r--r--   0        0        0      358 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_arp.textfsm
+-rw-r--r--   0        0        0     5683 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_interfaces.textfsm
+-rw-r--r--   0        0        0      695 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_interfaces_brief.textfsm
+-rw-r--r--   0        0        0      367 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_lag_brief.textfsm
+-rw-r--r--   0        0        0      416 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      906 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      384 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_mac-address.textfsm
+-rw-r--r--   0        0        0     1120 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_metro.textfsm
+-rw-r--r--   0        0        0      301 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_monitor.textfsm
+-rw-r--r--   0        0        0     2278 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_running-config_vlan.textfsm
+-rw-r--r--   0        0        0      851 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_span.textfsm
+-rw-r--r--   0        0        0      351 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_topo.textfsm
+-rw-r--r--   0        0        0     2990 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_trunk.textfsm
+-rw-r--r--   0        0        0     1629 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_version.textfsm
+-rw-r--r--   0        0        0     6614 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_interfaces.textfsm
+-rw-r--r--   0        0        0      430 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_interfaces_brief.textfsm
+-rw-r--r--   0        0        0      367 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_lag_brief.textfsm
+-rw-r--r--   0        0        0      906 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     1071 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_metro.textfsm
+-rw-r--r--   0        0        0      311 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_monitor_actual.textfsm
+-rw-r--r--   0        0        0     1624 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_running-config_interface.textfsm
+-rw-r--r--   0        0        0     2277 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_running-config_vlan.textfsm
+-rw-r--r--   0        0        0      739 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_span.textfsm
+-rw-r--r--   0        0        0      591 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_topo.textfsm
+-rw-r--r--   0        0        0      167 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/checkpoint_gaia_fw_stat.textfsm
+-rw-r--r--   0        0        0      192 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/checkpoint_gaia_show_arp_dynamic_all.textfsm
+-rw-r--r--   0        0        0      398 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/checkpoint_gaia_show_asset_all.textfsm
+-rw-r--r--   0        0        0      189 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/checkpoint_gaia_show_dns.textfsm
+-rw-r--r--   0        0        0       71 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/checkpoint_gaia_show_domainname.textfsm
+-rw-r--r--   0        0        0      849 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/checkpoint_gaia_show_interfaces_all.textfsm
+-rw-r--r--   0        0        0      509 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/checkpoint_gaia_show_ipv6_route.textfsm
+-rw-r--r--   0        0        0      159 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/checkpoint_gaia_show_lom.textfsm
+-rw-r--r--   0        0        0      208 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/checkpoint_gaia_show_ntp_servers.textfsm
+-rw-r--r--   0        0        0      550 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/checkpoint_gaia_show_route.textfsm
+-rw-r--r--   0        0        0      236 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/checkpoint_gaia_show_version_all.textfsm
+-rw-r--r--   0        0        0      115 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/checkpoint_gaia_show_virtual-system_all.textfsm
+-rw-r--r--   0        0        0      419 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/ciena_saos_chassis_show_temperature.textfsm
+-rw-r--r--   0        0        0     1010 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/ciena_saos_port_show.textfsm
+-rw-r--r--   0        0        0      945 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/ciena_saos_rstp_show.textfsm
+-rw-r--r--   0        0        0      623 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/ciena_saos_software_show.textfsm
+-rw-r--r--   0        0        0      289 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/ciena_saos_ssh_server_show_key.textfsm
+-rw-r--r--   0        0        0      556 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/ciena_saos_traffic-profiling_standard-profile_show.textfsm
+-rw-r--r--   0        0        0      646 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/ciena_saos_vlan_show.textfsm
+-rw-r--r--   0        0        0      714 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/cisco_apic_fabric_show_vlan_extended.textfsm
+-rw-r--r--   0        0        0      695 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_dir.textfsm
+-rw-r--r--   0        0        0      737 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_ping.textfsm
+-rw-r--r--   0        0        0     6125 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_access-list.textfsm
+-rw-r--r--   0        0        0      347 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_arp.textfsm
+-rw-r--r--   0        0        0     9761 2024-05-29 21:22:06.797360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_asp_drop.textfsm
+-rw-r--r--   0        0        0      829 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_asp_table_vpn-context_detail.textfsm
+-rw-r--r--   0        0        0     1377 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_bgp_summary.textfsm
+-rw-r--r--   0        0        0      917 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_cpu_usage_detailed.textfsm
+-rw-r--r--   0        0        0      438 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_crypto_ikev1_sa_detail.textfsm
+-rw-r--r--   0        0        0     6136 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_crypto_ipsec_sa.textfsm
+-rw-r--r--   0        0        0     3036 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_failover.textfsm
+-rw-r--r--   0        0        0     4419 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_interface.textfsm
+-rw-r--r--   0        0        0     7392 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_interface_detail.textfsm
+-rw-r--r--   0        0        0      286 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_interface_ip_brief.textfsm
+-rw-r--r--   0        0        0      320 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_inventory.textfsm
+-rw-r--r--   0        0        0     6025 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_license_all.textfsm
+-rw-r--r--   0        0        0     2352 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_logging.textfsm
+-rw-r--r--   0        0        0      381 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_module.textfsm
+-rw-r--r--   0        0        0      540 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_module_details.textfsm
+-rw-r--r--   0        0        0      372 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_module_status.textfsm
+-rw-r--r--   0        0        0      105 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_name.textfsm
+-rw-r--r--   0        0        0     1624 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_nat.textfsm
+-rw-r--r--   0        0        0      581 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_object-group_network.textfsm
+-rw-r--r--   0        0        0      421 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_ospf_interface_brief.textfsm
+-rw-r--r--   0        0        0      380 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0     1346 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_port-channel_summary.textfsm
+-rw-r--r--   0        0        0      425 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_resource_usage.textfsm
+-rw-r--r--   0        0        0     1793 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_route.textfsm
+-rw-r--r--   0        0        0     2300 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_running-config_all_crypto_map.textfsm
+-rw-r--r--   0        0        0      437 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_ikev1.textfsm
+-rw-r--r--   0        0        0     1212 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_map.textfsm
+-rw-r--r--   0        0        0     1726 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_running-config_ipsec.textfsm
+-rw-r--r--   0        0        0      512 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_running-config_object_network.textfsm
+-rw-r--r--   0        0        0     4906 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_running-config_tunnel-group.textfsm
+-rw-r--r--   0        0        0     2556 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_version.textfsm
+-rw-r--r--   0        0        0     1625 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb.textfsm
+-rw-r--r--   0        0        0     1828 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_anyconnect.textfsm
+-rw-r--r--   0        0        0     7479 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_detail_l2l.textfsm
+-rw-r--r--   0        0        0     1126 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_xlate.textfsm
+-rw-r--r--   0        0        0     1886 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ftd_show_vpn-sessiondb_anyconnect.textfsm
+-rw-r--r--   0        0        0      481 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_dir.textfsm
+-rw-r--r--   0        0        0      935 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_ping.textfsm
+-rw-r--r--   0        0        0     1971 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_access-list.textfsm
+-rw-r--r--   0        0        0      432 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_access-session.textfsm
+-rw-r--r--   0        0        0      953 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_adjacency.textfsm
+-rw-r--r--   0        0        0      355 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_alert_counters.textfsm
+-rw-r--r--   0        0        0      310 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_aliases.textfsm
+-rw-r--r--   0        0        0      402 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ap_cdp_neighbors.textfsm
+-rw-r--r--   0        0        0      555 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ap_summary.textfsm
+-rw-r--r--   0        0        0      615 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_archive.textfsm
+-rw-r--r--   0        0        0      419 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_authentication_sessions.textfsm
+-rw-r--r--   0        0        0     2737 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_authentication_sessions_method_details.textfsm
+-rw-r--r--   0        0        0     2508 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_bfd_neighbors_details.textfsm
+-rw-r--r--   0        0        0     1704 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_boot.textfsm
+-rw-r--r--   0        0        0      264 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_capability_feature_routing.textfsm
+-rw-r--r--   0        0        0      538 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors.textfsm
+-rw-r--r--   0        0        0      937 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      317 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_clock.textfsm
+-rw-r--r--   0        0        0     2327 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_controller_t1.textfsm
+-rw-r--r--   0        0        0     6120 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_crypto_ipsec_sa_detail.textfsm
+-rw-r--r--   0        0        0     2174 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_crypto_pki_certificates.textfsm
+-rw-r--r--   0        0        0     1432 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_crypto_session_detail.textfsm
+-rw-r--r--   0        0        0     1047 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_dhcp_lease.textfsm
+-rw-r--r--   0        0        0      491 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_dmvpn.textfsm
+-rw-r--r--   0        0        0     1367 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_dot1x_all.textfsm
+-rw-r--r--   0        0        0      413 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_environment_power_all.textfsm
+-rw-r--r--   0        0        0     1603 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_environment_temperature.textfsm
+-rw-r--r--   0        0        0     1326 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_etherchannel_summary.textfsm
+-rw-r--r--   0        0        0      224 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_file_systems.textfsm
+-rw-r--r--   0        0        0      454 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_hosts_summary.textfsm
+-rw-r--r--   0        0        0     1226 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_interface_link.textfsm
+-rw-r--r--   0        0        0      320 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_interface_transceiver.textfsm
+-rw-r--r--   0        0        0     2778 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_interfaces.textfsm
+-rw-r--r--   0        0        0      423 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_interfaces_description.textfsm
+-rw-r--r--   0        0        0      934 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0     1511 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_interfaces_switchport.textfsm
+-rw-r--r--   0        0        0      570 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_inventory.textfsm
+-rw-r--r--   0        0        0     2587 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_access-lists.textfsm
+-rw-r--r--   0        0        0      558 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_arp.textfsm
+-rw-r--r--   0        0        0     2029 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_bgp.textfsm
+-rw-r--r--   0        0        0     1706 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors.textfsm
+-rw-r--r--   0        0        0     2011 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors_advertised-routes.textfsm
+-rw-r--r--   0        0        0      884 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0     1761 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_bgp_vpnv4_all_neighbors.textfsm
+-rw-r--r--   0        0        0     1286 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_cef.textfsm
+-rw-r--r--   0        0        0     3323 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_cef_detail.textfsm
+-rw-r--r--   0        0        0      740 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_device_tracking_all.textfsm
+-rw-r--r--   0        0        0     2669 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_interfaces_detail.textfsm
+-rw-r--r--   0        0        0      779 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_neighbors.textfsm
+-rw-r--r--   0        0        0     2642 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_topology.textfsm
+-rwxr-xr-x   0        0        0      459 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_flow_toptalkers.textfsm
+-rw-r--r--   0        0        0     4260 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_http_server_status.textfsm
+-rw-r--r--   0        0        0     1963 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_interface.textfsm
+-rw-r--r--   0        0        0      306 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0     1378 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_mroute.textfsm
+-rw-r--r--   0        0        0      645 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_nat_translations.textfsm
+-rw-r--r--   0        0        0      776 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database.textfsm
+-rw-r--r--   0        0        0     1362 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_network.textfsm
+-rw-r--r--   0        0        0     1807 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_router.textfsm
+-rw-r--r--   0        0        0      426 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_ospf_interface_brief.textfsm
+-rw-r--r--   0        0        0      389 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0      436 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_prefix-list.textfsm
+-rw-r--r--   0        0        0     2562 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_route.textfsm
+-rw-r--r--   0        0        0     1389 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_route_summary.textfsm
+-rw-r--r--   0        0        0      593 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_source_binding.textfsm
+-rw-r--r--   0        0        0      474 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_vrf_interfaces.textfsm
+-rw-r--r--   0        0        0      917 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ipv6_access-lists.textfsm
+-rw-r--r--   0        0        0      426 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ipv6_interface_brief.textfsm
+-rw-r--r--   0        0        0      387 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ipv6_neighbors.textfsm
+-rw-r--r--   0        0        0      523 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ipv6_route.textfsm
+-rw-r--r--   0        0        0      956 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_isdn_status.textfsm
+-rw-r--r--   0        0        0      412 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_isis_neighbors.textfsm
+-rw-r--r--   0        0        0      547 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_license.textfsm
+-rw-r--r--   0        0        0      479 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0     2769 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     5837 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_logging.textfsm
+-rw-r--r--   0        0        0     4305 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_mac-address-table.textfsm
+-rw-r--r--   0        0        0     1088 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_module.textfsm
+-rw-r--r--   0        0        0      585 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_module_online_diag.textfsm
+-rw-r--r--   0        0        0     1138 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_module_status.textfsm
+-rw-r--r--   0        0        0      760 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_module_submodule.textfsm
+-rw-r--r--   0        0        0      350 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_mpls_interfaces.textfsm
+-rw-r--r--   0        0        0      391 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_nve_peers.textfsm
+-rw-r--r--   0        0        0      346 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_nve_vni.textfsm
+-rw-r--r--   0        0        0     1215 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_object-group.textfsm
+-rw-r--r--   0        0        0     1072 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_platform_diag.textfsm
+-rw-r--r--   0        0        0      974 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_port-security_interface_interface.textfsm
+-rw-r--r--   0        0        0      922 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_power_available.textfsm
+-rw-r--r--   0        0        0      684 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_power_status.textfsm
+-rw-r--r--   0        0        0      314 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_power_supplies.textfsm
+-rw-r--r--   0        0        0      344 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_processes_cpu.textfsm
+-rw-r--r--   0        0        0      640 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_processes_memory_sorted.textfsm
+-rw-r--r--   0        0        0     3950 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_redundancy.textfsm
+-rw-r--r--   0        0        0      312 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_rep_topology.textfsm
+-rw-r--r--   0        0        0      784 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_route-map.textfsm
+-rw-r--r--   0        0        0     3318 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_running-config_partition_access-list.textfsm
+-rw-r--r--   0        0        0     1034 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_running-config_partition_route-map.textfsm
+-rw-r--r--   0        0        0      359 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_snmp_community.textfsm
+-rw-r--r--   0        0        0      802 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_snmp_group.textfsm
+-rw-r--r--   0        0        0      668 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_snmp_user.textfsm
+-rw-r--r--   0        0        0      413 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_spanning-tree.textfsm
+-rw-r--r--   0        0        0     2018 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_standby.textfsm
+-rw-r--r--   0        0        0      660 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_standby_brief.textfsm
+-rw-r--r--   0        0        0      581 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_switch_detail.textfsm
+-rw-r--r--   0        0        0      357 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_switch_detail_stack_ports.textfsm
+-rw-r--r--   0        0        0     1009 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_tacacs.textfsm
+-rw-r--r--   0        0        0     1759 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_version.textfsm
+-rw-r--r--   0        0        0     6342 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_vlan.textfsm
+-rw-r--r--   0        0        0     1374 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_vlans.textfsm
+-rw-r--r--   0        0        0      684 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_vrf.textfsm
+-rw-r--r--   0        0        0     1108 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_vrf_detail.textfsm
+-rw-r--r--   0        0        0     1654 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_vrrp_all.textfsm
+-rw-r--r--   0        0        0     1802 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_vrrp_brief.textfsm
+-rw-r--r--   0        0        0     1109 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_vtp_status.textfsm
+-rw-r--r--   0        0        0     1669 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_traceroute.textfsm
+-rw-r--r--   0        0        0      971 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nvfis_show_bridge-settings.textfsm
+-rw-r--r--   0        0        0      214 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nvfis_show_configuration_commit_changes.textfsm
+-rw-r--r--   0        0        0      245 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nvfis_show_nic.textfsm
+-rw-r--r--   0        0        0      159 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nvfis_show_running-config_snmp_enable.textfsm
+-rw-r--r--   0        0        0      292 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nvfis_show_running-config_snmp_group.textfsm
+-rw-r--r--   0        0        0      385 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nvfis_show_running-config_snmp_host.textfsm
+-rw-r--r--   0        0        0      437 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nvfis_show_running-config_snmp_user.textfsm
+-rw-r--r--   0        0        0      394 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nvfis_show_running-config_system_settings.textfsm
+-rw-r--r--   0        0        0      516 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nvfis_show_running-config_system_time.textfsm
+-rw-r--r--   0        0        0      309 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nvfis_show_running-config_system_upgrade.textfsm
+-rw-r--r--   0        0        0      177 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nvfis_show_version.textfsm
+-rw-r--r--   0        0        0      460 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_dir.textfsm
+-rw-r--r--   0        0        0     1781 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_access-lists.textfsm
+-rw-r--r--   0        0        0     1497 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_bgp_vrf_all_ipv4_unicast_detail.textfsm
+-rw-r--r--   0        0        0     1856 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_bgp_vrf_all_ipv4_unicast_neighbors_routes.textfsm
+-rw-r--r--   0        0        0      461 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors.textfsm
+-rw-r--r--   0        0        0      689 2024-05-29 21:22:06.801360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      203 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_clock.textfsm
+-rw-r--r--   0        0        0      210 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_configuration_session_summary.textfsm
+-rw-r--r--   0        0        0      954 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_cts_interface_all.textfsm
+-rw-r--r--   0        0        0      233 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_cts_interface_brief.textfsm
+-rw-r--r--   0        0        0     2143 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_environment.textfsm
+-rw-r--r--   0        0        0      384 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_environment_temperature.textfsm
+-rw-r--r--   0        0        0      147 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_feature.textfsm
+-rw-r--r--   0        0        0      178 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_fex.textfsm
+-rw-r--r--   0        0        0     1002 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_fex_id.textfsm
+-rw-r--r--   0        0        0      491 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_flogi_database.textfsm
+-rw-r--r--   0        0        0     1083 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_forwarding_adjacency.textfsm
+-rw-r--r--   0        0        0     1041 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_forwarding_ipv4_route.textfsm
+-rw-r--r--   0        0        0    18876 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_hardware_internal_bigsur_all-ports_detail.textfsm
+-rw-r--r--   0        0        0       57 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_hostname.textfsm
+-rw-r--r--   0        0        0     2393 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_hsrp_all.textfsm
+-rw-r--r--   0        0        0     1630 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_interface.textfsm
+-rw-r--r--   0        0        0     2212 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_interface_brief.textfsm
+-rw-r--r--   0        0        0      358 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_interface_description.textfsm
+-rw-r--r--   0        0        0      203 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_interface_snmp-ifindex.textfsm
+-rw-r--r--   0        0        0      370 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_interface_status.textfsm
+-rw-r--r--   0        0        0      669 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver.textfsm
+-rw-r--r--   0        0        0     2240 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver_details.textfsm
+-rw-r--r--   0        0        0      812 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_interfaces_switchport.textfsm
+-rw-r--r--   0        0        0      500 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_inventory.textfsm
+-rw-r--r--   0        0        0      716 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_adjacency.textfsm
+-rw-r--r--   0        0        0      322 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_arp.textfsm
+-rw-r--r--   0        0        0      448 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_arp_detail.textfsm
+-rw-r--r--   0        0        0     2778 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_bgp.textfsm
+-rw-r--r--   0        0        0     4875 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_neighbors.textfsm
+-rw-r--r--   0        0        0      974 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0     1014 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary_vrf.textfsm
+-rw-r--r--   0        0        0      714 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_community-list.textfsm
+-rw-r--r--   0        0        0      283 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_relay_address.textfsm
+-rw-r--r--   0        0        0     3956 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_snooping_statistics.textfsm
+-rw-r--r--   0        0        0     5936 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_interface.textfsm
+-rw-r--r--   0        0        0      414 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0     5167 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_interface_vrf_all.textfsm
+-rw-r--r--   0        0        0      934 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_mroutes_vrf_all.textfsm
+-rw-r--r--   0        0        0      665 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_msdp_summary_vrf_all.textfsm
+-rw-r--r--   0        0        0      680 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_database.textfsm
+-rw-r--r--   0        0        0      526 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_interface_brief.textfsm
+-rw-r--r--   0        0        0      375 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0      453 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_pim_group-range_vrf_all.textfsm
+-rw-r--r--   0        0        0      480 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_pim_interface_brief_vrf_all.textfsm
+-rw-r--r--   0        0        0      636 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_pim_neighbor_vrf_all.textfsm
+-rw-r--r--   0        0        0      546 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_pim_rp_vrf_all.textfsm
+-rw-r--r--   0        0        0     2090 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_route.textfsm
+-rw-r--r--   0        0        0      244 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ipv6_interface_brief.textfsm
+-rw-r--r--   0        0        0      260 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_l2rib_internal_permanently-frozen-list.textfsm
+-rw-r--r--   0        0        0      411 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_license_usage.textfsm
+-rw-r--r--   0        0        0      345 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      733 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      310 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_mac_address-table.textfsm
+-rw-r--r--   0        0        0      351 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_module.textfsm
+-rw-r--r--   0        0        0      302 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_nve_peers.textfsm
+-rw-r--r--   0        0        0      495 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_nve_vni.textfsm
+-rw-r--r--   0        0        0     2786 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_port-channel_summary.textfsm
+-rw-r--r--   0        0        0      234 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_processes_cpu.textfsm
+-rw-r--r--   0        0        0      698 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_route-map.textfsm
+-rw-r--r--   0        0        0      495 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_spanning-tree_root.textfsm
+-rw-r--r--   0        0        0      339 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_switching-mode.textfsm
+-rw-r--r--   0        0        0      312 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_vdc.textfsm
+-rwxr-xr-x   0        0        0      697 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_version.textfsm
+-rw-r--r--   0        0        0     6325 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_vlan.textfsm
+-rw-r--r--   0        0        0       99 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_vpc.textfsm
+-rw-r--r--   0        0        0      279 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_vrf.textfsm
+-rw-r--r--   0        0        0      751 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_vrf_detail.textfsm
+-rw-r--r--   0        0        0      239 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_vrf_interface.textfsm
+-rw-r--r--   0        0        0      403 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_interfaces_description.textfsm
+-rw-r--r--   0        0        0      594 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0     1528 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_interfaces_switchport.textfsm
+-rw-r--r--   0        0        0      907 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_ip_interface.textfsm
+-rw-r--r--   0        0        0      411 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      336 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_mac_address-table.textfsm
+-rw-r--r--   0        0        0      601 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_system.textfsm
+-rw-r--r--   0        0        0      116 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_system_id.textfsm
+-rw-r--r--   0        0        0      442 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_version.textfsm
+-rw-r--r--   0        0        0      828 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_vlan.textfsm
+-rw-r--r--   0        0        0     3155 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a.textfsm
+-rw-r--r--   0        0        0     4795 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a_cleanair_config.textfsm
+-rw-r--r--   0        0        0     1683 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_advanced_802.11a_channel.textfsm
+-rw-r--r--   0        0        0     2729 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_config_general.textfsm
+-rw-r--r--   0        0        0      643 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_image_all.textfsm
+-rw-r--r--   0        0        0      524 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_summary.textfsm
+-rw-r--r--   0        0        0      780 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_band-select.textfsm
+-rw-r--r--   0        0        0      215 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_boot.textfsm
+-rw-r--r--   0        0        0      661 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_cdp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     1435 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_client_detail.textfsm
+-rw-r--r--   0        0        0      292 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_exclusionlist.textfsm
+-rw-r--r--   0        0        0      355 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_flexconnect_group_summary.textfsm
+-rw-r--r--   0        0        0     1549 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_detailed_id.textfsm
+-rw-r--r--   0        0        0      347 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_group_summary.textfsm
+-rw-r--r--   0        0        0      492 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_summary.textfsm
+-rw-r--r--   0        0        0      428 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_inventory.textfsm
+-rw-r--r--   0        0        0      475 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_anchor.textfsm
+-rw-r--r--   0        0        0      749 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_sum.textfsm
+-rw-r--r--   0        0        0      655 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_port_summary.textfsm
+-rw-r--r--   0        0        0     2911 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_radius_summary.textfsm
+-rw-r--r--   0        0        0      842 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_detail.textfsm
+-rw-r--r--   0        0        0      970 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_summary.textfsm
+-rw-r--r--   0        0        0      431 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_rf-profile_summary.textfsm
+-rw-r--r--   0        0        0      997 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_stats_port_summary.textfsm
+-rw-r--r--   0        0        0     1238 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_sysinfo.textfsm
+-rw-r--r--   0        0        0     1450 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_tacacs_summary.textfsm
+-rw-r--r--   0        0        0      906 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_time.textfsm
+-rw-r--r--   0        0        0      420 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_wlan_sum.textfsm
+-rw-r--r--   0        0        0     6223 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_admin_show_controller_fabric_health.textfsm
+-rw-r--r--   0        0        0     1379 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_admin_show_environment_fan.textfsm
+-rw-r--r--   0        0        0      309 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_admin_show_environment_power.textfsm
+-rw-r--r--   0        0        0      415 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_admin_show_inventory.textfsm
+-rw-r--r--   0        0        0      179 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_admin_show_platform.textfsm
+-rw-r--r--   0        0        0      425 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_admin_show_vm.textfsm
+-rw-r--r--   0        0        0      504 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_dir.textfsm
+-rw-r--r--   0        0        0      921 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_ping.textfsm
+-rw-r--r--   0        0        0      537 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_arp.textfsm
+-rw-r--r--   0        0        0      838 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_asic-errors_all_location.textfsm
+-rw-r--r--   0        0        0      179 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_bfd_sessions.textfsm
+-rw-r--r--   0        0        0     1905 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_bgp.textfsm
+-rw-r--r--   0        0        0      725 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_bgp_instance_all_summary.textfsm
+-rw-r--r--   0        0        0     5397 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_bgp_neighbors.textfsm
+-rw-r--r--   0        0        0      228 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_bgp_vrf_all_ipv4_unicast_summary.textfsm
+-rw-r--r--   0        0        0      513 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_cdp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     1544 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_cef_drops_location.textfsm
+-rw-r--r--   0        0        0      337 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_configuration_commit_list.textfsm
+-rw-r--r--   0        0        0      347 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_controller_fabric_plane_all.textfsm
+-rw-r--r--   0        0        0     2208 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_controllers_HundredGigabitEthernet.textfsm
+-rw-r--r--   0        0        0     2281 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_controllers_all_phy.textfsm
+-rw-r--r--   0        0        0     2823 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_egress_location.textfsm
+-rw-r--r--   0        0        0     1961 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_ingress_location.textfsm
+-rw-r--r--   0        0        0      426 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_egress_location.textfsm
+-rw-r--r--   0        0        0     1406 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_ingress_location.textfsm
+-rw-r--r--   0        0        0     4937 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_controllers_hundredgige_all.textfsm
+-rw-r--r--   0        0        0      288 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_dhcp_ipv4_proxy_binding.textfsm
+-rw-r--r--   0        0        0     7430 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_drops_np_all.textfsm
+-rw-r--r--   0        0        0      518 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_hsrp.textfsm
+-rw-r--r--   0        0        0      665 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_install_active.textfsm
+-rw-r--r--   0        0        0      268 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_interface_brief.textfsm
+-rw-r--r--   0        0        0      957 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_interfaces.textfsm
+-rw-r--r--   0        0        0      353 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_interfaces_summary.textfsm
+-rw-r--r--   0        0        0      269 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_inventory.textfsm
+-rw-r--r--   0        0        0      571 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0      196 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0     1719 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_ip_route.textfsm
+-rw-r--r--   0        0        0     1869 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_ipv4_interface.textfsm
+-rw-r--r--   0        0        0      288 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_ipv4_vrf_all_interface_brief.textfsm
+-rw-r--r--   0        0        0      431 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_ipv6_neighbors.textfsm
+-rw-r--r--   0        0        0      288 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_isis_neighbors.textfsm
+-rw-r--r--   0        0        0      380 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0     1387 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      694 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_lpts_pifib_hardware_police_location.textfsm
+-rw-r--r--   0        0        0      398 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_mpls_ldp_neighbor_brief.textfsm
+-rw-r--r--   0        0        0      362 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0      486 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_ospf_vrf_all_interface_brief.textfsm
+-rw-r--r--   0        0        0      480 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_ospf_vrf_all_neighbor.textfsm
+-rw-r--r--   0        0        0      359 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_group-map.textfsm
+-rw-r--r--   0        0        0      488 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_interface.textfsm
+-rw-r--r--   0        0        0      447 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_neighbor.textfsm
+-rw-r--r--   0        0        0      262 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_pim_neighbor.textfsm
+-rw-r--r--   0        0        0     1074 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_platform_summary_location_all.textfsm
+-rw-r--r--   0        0        0      205 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_processes_cpu.textfsm
+-rw-r--r--   0        0        0      187 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_redundancy_summary.textfsm
+-rw-r--r--   0        0        0      226 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_rsvp_neighbors.textfsm
+-rw-r--r--   0        0        0      871 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_version.textfsm
+-rw-r--r--   0        0        0      339 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_version_brief.textfsm
+-rw-r--r--   0        0        0      766 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_vrf_all_detail.textfsm
+-rw-r--r--   0        0        0      322 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/dell_force10_show_arp.textfsm
+-rw-r--r--   0        0        0      231 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/dell_force10_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0      211 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/dell_force10_show_version.textfsm
+-rw-r--r--   0        0        0      825 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/dell_force10_show_vlan.textfsm
+-rw-r--r--   0        0        0      274 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/dell_force10_show_vlan_brief.textfsm
+-rw-r--r--   0        0        0      295 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/dell_powerconnect_show_bridge_address_table.textfsm
+-rw-r--r--   0        0        0      193 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/dell_powerconnect_show_interfaces_description.textfsm
+-rw-r--r--   0        0        0      592 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/dell_powerconnect_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0      333 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/dlink_ds_show_arpentry.textfsm
+-rw-r--r--   0        0        0     4086 2024-05-29 21:22:06.805360 ntc_templates-5.1.0/ntc_templates/templates/eltex_show_interface.textfsm
+-rw-r--r--   0        0        0     2079 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/eltex_show_interfaces_description.textfsm
+-rw-r--r--   0        0        0     2498 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/eltex_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0     2779 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/eltex_show_interfaces_switchport.textfsm
+-rw-r--r--   0        0        0     1516 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/eltex_show_ip_interface.textfsm
+-rw-r--r--   0        0        0     2262 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/eltex_show_system.textfsm
+-rw-r--r--   0        0        0      431 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/eltex_show_system_id.textfsm
+-rw-r--r--   0        0        0     1188 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/eltex_show_vlan.textfsm
+-rw-r--r--   0        0        0      663 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ericsson_ipos_show_arp.textfsm
+-rw-r--r--   0        0        0      433 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ericsson_ipos_show_isis_adjacency.textfsm
+-rw-r--r--   0        0        0      168 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ericsson_ipos_show_version.textfsm
+-rw-r--r--   0        0        0     2838 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/extreme_exos_show_ipconfig.textfsm
+-rw-r--r--   0        0        0      448 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/extreme_exos_show_ports_description.textfsm
+-rw-r--r--   0        0        0     1948 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/extreme_exos_show_ports_information.textfsm
+-rw-r--r--   0        0        0      835 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/extreme_exos_show_ports_information_detail.textfsm
+-rw-r--r--   0        0        0     1367 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/extreme_exos_show_sharing.textfsm
+-rw-r--r--   0        0        0      416 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/extreme_exos_show_vlan_description.textfsm
+-rw-r--r--   0        0        0      574 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/fortinet_get_router_info_bgp_summary.textfsm
+-rw-r--r--   0        0        0      252 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/fortinet_get_system_arp.textfsm
+-rw-r--r--   0        0        0     2048 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/fortinet_get_system_ha_status.textfsm
+-rw-r--r--   0        0        0     9094 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/fortinet_get_system_interface.textfsm
+-rw-r--r--   0        0        0      689 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/fortinet_get_system_interface_physical.textfsm
+-rw-r--r--   0        0        0     2931 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/fortinet_get_system_status.textfsm
+-rw-r--r--   0        0        0      248 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_arp.textfsm
+-rw-r--r--   0        0        0      200 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_clock.textfsm
+-rw-r--r--   0        0        0      519 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_counters_bound_interface.textfsm
+-rw-r--r--   0        0        0      666 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_device_manuinfo.textfsm
+-rw-r--r--   0        0        0     8619 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_interface.textfsm
+-rw-r--r--   0        0        0     1208 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_interface_brief.textfsm
+-rw-r--r--   0        0        0     1600 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_ip_interface.textfsm
+-rw-r--r--   0        0        0      634 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_ip_routing-table.textfsm
+-rw-r--r--   0        0        0      195 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance.textfsm
+-rw-r--r--   0        0        0     5480 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance_instance-name.textfsm
+-rw-r--r--   0        0        0      777 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_link-aggregation_verbose.textfsm
+-rw-r--r--   0        0        0      647 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_list.textfsm
+-rw-r--r--   0        0        0      932 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_verbose.textfsm
+-rw-r--r--   0        0        0      195 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_mac-address.textfsm
+-rw-r--r--   0        0        0      642 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_vlan_all.textfsm
+-rw-r--r--   0        0        0      116 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_vlan_brief.textfsm
+-rw-r--r--   0        0        0      343 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_arp.textfsm
+-rw-r--r--   0        0        0      625 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_cdp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      710 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_interfaces.textfsm
+-rw-r--r--   0        0        0      971 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_interfaces_brief.textfsm
+-rw-r--r--   0        0        0      622 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_ip.textfsm
+-rw-r--r--   0        0        0      383 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_ip_route.textfsm
+-rw-r--r--   0        0        0      706 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device.textfsm
+-rw-r--r--   0        0        0     1699 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device_detail.textfsm
+-rw-r--r--   0        0        0      252 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_mac-address.textfsm
+-rw-r--r--   0        0        0      453 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_port-security.textfsm
+-rw-r--r--   0        0        0     1345 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_system.textfsm
+-rw-r--r--   0        0        0      385 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_tech_buffers.textfsm
+-rw-r--r--   0        0        0      407 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_trunks.textfsm
+-rw-r--r--   0        0        0      300 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_vlans.textfsm
+-rw-r--r--   0        0        0      371 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_board.textfsm
+-rw-r--r--   0        0        0      212 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_board_serial-number.textfsm
+-rw-r--r--   0        0        0       98 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_cpu.textfsm
+-rw-r--r--   0        0        0      107 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_mem.textfsm
+-rw-r--r--   0        0        0     1065 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_ont_autofind.textfsm
+-rw-r--r--   0        0        0     5899 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_ont_info_by-sn_sn.textfsm
+-rw-r--r--   0        0        0      339 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_ont_info_description.textfsm
+-rw-r--r--   0        0        0      553 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_ont_info_fsp.textfsm
+-rw-r--r--   0        0        0      466 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_ont_info_summary_ont.textfsm
+-rw-r--r--   0        0        0      424 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_ont_info_summary_sn.textfsm
+-rw-r--r--   0        0        0     2198 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_port_info.textfsm
+-rw-r--r--   0        0        0      375 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_sysman_service_state.textfsm
+-rw-r--r--   0        0        0      201 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_sysuptime.textfsm
+-rw-r--r--   0        0        0      246 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_temperature.textfsm
+-rw-r--r--   0        0        0     1043 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_version.textfsm
+-rw-r--r--   0        0        0     1392 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_acl_all.textfsm
+-rw-r--r--   0        0        0      530 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_arp_all.textfsm
+-rw-r--r--   0        0        0      500 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_arp_brief.textfsm
+-rw-r--r--   0        0        0     4401 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_interface.textfsm
+-rw-r--r--   0        0        0      498 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_interface_brief.textfsm
+-rw-r--r--   0        0        0      376 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_interface_description.textfsm
+-rw-r--r--   0        0        0     2065 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_ip_routing-table_verbose.textfsm
+-rw-r--r--   0        0        0      246 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_ip_vpn-instance.textfsm
+-rw-r--r--   0        0        0      346 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_ip_vpn-instance_interface.textfsm
+-rw-r--r--   0        0        0      857 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_ipv6_neighbors.textfsm
+-rw-r--r--   0        0        0      435 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_isis_peer.textfsm
+-rw-r--r--   0        0        0     1843 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_lldp_neighbor.textfsm
+-rw-r--r--   0        0        0      312 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_mac-address.textfsm
+-rw-r--r--   0        0        0      713 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_nat_server.textfsm
+-rw-r--r--   0        0        0     7802 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_port_vlan.textfsm
+-rw-r--r--   0        0        0      193 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_service-set_all.textfsm
+-rw-r--r--   0        0        0     1084 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_service-set_id_id.textfsm
+-rw-r--r--   0        0        0       96 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_sn_license.textfsm
+-rw-r--r--   0        0        0      424 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_snmp-agent_community_read.textfsm
+-rw-r--r--   0        0        0     1346 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_startup.textfsm
+-rw-r--r--   0        0        0      390 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_temperature.textfsm
+-rw-r--r--   0        0        0      522 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_traffic-filter_applied-record.textfsm
+-rw-r--r--   0        0        0      505 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_version.textfsm
+-rw-r--r--   0        0        0     1550 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_vlan.textfsm
+-rw-r--r--   0        0        0    61971 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/index
+-rw-r--r--   0        0        0      536 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ipinfusion_ocnos_show_lldp_table.textfsm
+-rw-r--r--   0        0        0      319 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_arp_no-resolve.textfsm
+-rw-r--r--   0        0        0     3195 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_interfaces.textfsm
+-rw-r--r--   0        0        0      803 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_status.textfsm
+-rw-r--r--   0        0        0      341 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_chassis_firmware.textfsm
+-rw-r--r--   0        0        0     4354 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_chassis_hardware.textfsm
+-rw-r--r--   0        0        0      735 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_ethernet-switching_table.textfsm
+-rw-r--r--   0        0        0      662 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_interfaces.textfsm
+-rw-r--r--   0        0        0      267 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_isis_adjacency.textfsm
+-rw-r--r--   0        0        0      603 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_lacp_interfaces.textfsm
+-rw-r--r--   0        0        0      389 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      298 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0     1374 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_system_uptime.textfsm
+-rw-r--r--   0        0        0     4359 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_version.textfsm
+-rw-r--r--   0        0        0      318 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_vlans.textfsm
+-rw-r--r--   0        0        0      844 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/juniper_screenos_get_route.textfsm
+-rw-r--r--   0        0        0      338 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/linux_arp_-a.textfsm
+-rw-r--r--   0        0        0      919 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/linux_ip_address_show.textfsm
+-rw-r--r--   0        0        0      863 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/linux_ip_link_show.textfsm
+-rw-r--r--   0        0        0      618 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/linux_ip_route_show.textfsm
+-rw-r--r--   0        0        0      134 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/linux_ip_vrf_show.textfsm
+-rw-r--r--   0        0        0      660 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_monitor_name_once.textfsm
+-rw-r--r--   0        0        0      810 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_poe_print_without-paging.textfsm
+-rw-r--r--   0        0        0      473 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_print.textfsm
+-rw-r--r--   0        0        0      926 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_interface_print_terse_without-paging.textfsm
+-rw-r--r--   0        0        0      328 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ip_address_export_verbose.textfsm
+-rw-r--r--   0        0        0      539 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ip_address_print.textfsm
+-rw-r--r--   0        0        0      396 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ip_arp_print_without-paging.textfsm
+-rw-r--r--   0        0        0      955 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ip_dhcp-server_lease_print_without-paging.textfsm
+-rw-r--r--   0        0        0      618 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_address-list_print_terse.textfsm
+-rw-r--r--   0        0        0     2499 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_filter_print_all_without-paging.textfsm
+-rw-r--r--   0        0        0     2229 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_nat_print_all_without-paging.textfsm
+-rw-r--r--   0        0        0      816 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ip_route_print_terse.textfsm
+-rw-r--r--   0        0        0      436 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ipv6_neighbor_print_without-paging.textfsm
+-rw-r--r--   0        0        0      758 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_log_print_detail_without-paging.textfsm
+-rw-r--r--   0        0        0      637 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ping.textfsm
+-rw-r--r--   0        0        0     4409 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_routing_bgp_peer_print_status_without-paging.textfsm
+-rw-r--r--   0        0        0      758 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_routing_ospf_neighbor_print_terse_without-paging.textfsm
+-rw-r--r--   0        0        0      483 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_snmp_community_print_without-paging.textfsm
+-rw-r--r--   0        0        0      470 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_system_clock_print.textfsm
+-rw-r--r--   0        0        0      671 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_system_routerboard_print.textfsm
+-rw-r--r--   0        0        0      445 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_user_active_print.textfsm
+-rw-r--r--   0        0        0      169 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_debug_swm_status.textfsm
+-rw-r--r--   0        0        0      369 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_arp_all.textfsm
+-rw-r--r--   0        0        0      249 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_counter_global.textfsm
+-rw-r--r--   0        0        0     1943 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_high-availability_all.textfsm
+-rw-r--r--   0        0        0      252 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_interface_hardware.textfsm
+-rw-r--r--   0        0        0      333 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_interface_logical.textfsm
+-rw-r--r--   0        0        0      964 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_interface_management.textfsm
+-rw-r--r--   0        0        0      415 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_jobs_all.textfsm
+-rw-r--r--   0        0        0      258 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_mac_all.textfsm
+-rw-r--r--   0        0        0      729 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_running_nat-policy.textfsm
+-rw-r--r--   0        0        0      794 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_running_security-policy.textfsm
+-rw-r--r--   0        0        0      856 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_system_info.textfsm
+-rw-r--r--   0        0        0      975 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_test_security-policy-match.textfsm
+-rw-r--r--   0        0        0      914 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ruckus_fastiron_show_arp.textfsm
+-rw-r--r--   0        0        0      740 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ruckus_fastiron_show_interfaces.textfsm
+-rw-r--r--   0        0        0      602 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ruckus_fastiron_show_interfaces_brief.textfsm
+-rw-r--r--   0        0        0      285 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ruckus_fastiron_show_mac-address.textfsm
+-rw-r--r--   0        0        0      263 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ruckus_fastiron_show_media_validation.textfsm
+-rw-r--r--   0        0        0     1049 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ruckus_fastiron_show_version.textfsm
+-rw-r--r--   0        0        0     2679 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ruckus_fastiron_show_vlan.textfsm
+-rw-r--r--   0        0        0      433 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgerouter_show_arp.textfsm
+-rw-r--r--   0        0        0      404 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgerouter_show_dhcp_leases.textfsm
+-rw-r--r--   0        0        0      286 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgerouter_show_dhcpv6_server_leases.textfsm
+-rw-r--r--   0        0        0      324 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgerouter_show_interfaces.textfsm
+-rw-r--r--   0        0        0      307 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgerouter_show_interfaces_ethernet_physical.textfsm
+-rw-r--r--   0        0        0      911 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgerouter_show_ip_route.textfsm
+-rw-r--r--   0        0        0      269 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgerouter_show_ipv6_neighbors.textfsm
+-rw-r--r--   0        0        0      501 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgerouter_show_ipv6_route.textfsm
+-rw-r--r--   0        0        0      723 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgerouter_show_nat_rules.textfsm
+-rw-r--r--   0        0        0      380 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgerouter_show_version.textfsm
+-rw-r--r--   0        0        0      336 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgeswitch_show_arp.textfsm
+-rw-r--r--   0        0        0      569 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgeswitch_show_version.textfsm
+-rw-r--r--   0        0        0      219 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgeswitch_show_vlan.textfsm
+-rw-r--r--   0        0        0      470 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/vmware_nsxv_show_ip_bgp_neighbors.textfsm
+-rw-r--r--   0        0        0      307 2024-05-29 21:22:06.809360 ntc_templates-5.1.0/ntc_templates/templates/vmware_nsxv_show_ip_route.textfsm
+-rw-r--r--   0        0        0      303 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/vyatta_vyos_show_arp.textfsm
+-rw-r--r--   0        0        0      374 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/vyatta_vyos_show_interfaces.textfsm
+-rw-r--r--   0        0        0      859 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/vyatta_vyos_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0      263 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/watchguard_firebox_show_arp.textfsm
+-rw-r--r--   0        0        0     1181 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/yamaha_show_environment.textfsm
+-rw-r--r--   0        0        0      490 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/yamaha_show_ip_route.textfsm
+-rw-r--r--   0        0        0      626 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_firewall_acl_get.textfsm
+-rw-r--r--   0        0        0      402 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_intf_group_get.textfsm
+-rw-r--r--   0        0        0      595 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_ipalias_get.textfsm
+-rw-r--r--   0        0        0      425 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_lan_get.textfsm
+-rw-r--r--   0        0        0      678 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_lan_get_--Name_name.textfsm
+-rw-r--r--   0        0        0      459 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_lanhosts_get.textfsm
+-rw-r--r--   0        0        0      664 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_nat_addr_map_get.textfsm
+-rw-r--r--   0        0        0      751 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_nat_get.textfsm
+-rw-r--r--   0        0        0      629 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_snmp_get.textfsm
+-rw-r--r--   0        0        0      355 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_static_dhcp_get.textfsm
+-rw-r--r--   0        0        0      635 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_static_route_get.textfsm
+-rw-r--r--   0        0        0      539 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_wlan_get.textfsm
+-rw-r--r--   0        0        0      857 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_sys_atsh.textfsm
+-rw-r--r--   0        0        0      337 2024-05-29 21:22:06.813360 ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_zycli_Ethctl_media-type.textfsm
+-rw-r--r--   0        0        0     3146 2024-05-29 21:22:16.697464 ntc_templates-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 ntc_templates-5.1.0/PKG-INFO
```

### Comparing `ntc_templates-5.0.0/LICENSE` & `ntc_templates-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/README.md` & `ntc_templates-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/parse.py` & `ntc_templates-5.1.0/ntc_templates/parse.py`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/alcatel_aos_show_vlan.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/alcatel_aos_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_port.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_port.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_bgp_summary_family.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_bgp_summary_family.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_ldp_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_ldp_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_mpls_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_mpls_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_mpls_lsp.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_mpls_lsp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_ospf_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_ospf_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_router_rsvp_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_router_rsvp_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_service_id_base.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_service_id_base.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_service_sap-using.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_service_sap-using.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_service_sdp-using.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_service_sdp-using.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_service_sdp.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_service_sdp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/alcatel_sros_show_system_cpu.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/alcatel_sros_show_system_cpu.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_interface_switchport.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_interface_switchport.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_ip_route.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_lldp_neighbors_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_static-channel-group.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_static-channel-group.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_system.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_system.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/allied_telesis_awplus_show_vlan_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/allied_telesis_awplus_show_vlan_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_environment_cooling.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_environment_cooling.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_environment_temperature.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_environment_temperature.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_interfaces.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_inventory.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_inventory.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_access-lists.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_access-lists.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_bgp.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_bgp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_bgp_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_bgp_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_bgp_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_ospf_database.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_ospf_database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_ospf_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_ospf_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ip_route.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_ipv6_bgp_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_ipv6_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_lldp_neighbors_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_mac_address-table.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_mac_address-table.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_mac_security_participants_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_mac_security_participants_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_module.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_module.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_pim_ipv4_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_pim_ipv4_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_port-channel_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_port-channel_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_processes_top_once.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_processes_top_once.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_reload_cause.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_reload_cause.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_vlan.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/arista_eos_show_vrf.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/arista_eos_show_vrf.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_aaa_authentication_port-access_interface_all_client-status.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_aaa_authentication_port-access_interface_all_client-status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_bfd_all-vrfs.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_bfd_all-vrfs.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_bgp_all-vrfs_all_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_bgp_all-vrfs_all_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_bgp_all_all-vrfs_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_bgp_all_all-vrfs_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_interface_dom_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_interface_dom_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_lldp_neighbors-info_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_lldp_neighbors-info_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_system.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_system.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_vlan.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_aoscx_show_vsf_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_aoscx_show_vsf_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_os_show_ap_bss-table_details.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_os_show_ap_bss-table_details.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_os_show_ap_database.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_os_show_ap_database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_os_show_ap_database_long.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_os_show_ap_database_long.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_os_show_ap_radio-database.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_os_show_ap_radio-database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/aruba_os_show_arp.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/aruba_os_show_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/avaya_ers_show_logging_config.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/avaya_ers_show_logging_config.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/avaya_ers_show_mlt.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/avaya_ers_show_mlt.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/avaya_ers_show_mlt_all-members.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/avaya_ers_show_mlt_all-members.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/avaya_ers_show_sys-info.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/avaya_ers_show_sys-info.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/broadcom_icos_show_isdp_neighbors.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/broadcom_icos_show_isdp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/broadcom_icos_show_lldp_remote-device_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/broadcom_icos_show_lldp_remote-device_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/broadcom_icos_show_version.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/broadcom_icos_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_interfaces.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_interfaces_brief.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_interfaces_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_metro.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_metro.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_running-config_vlan.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_running-config_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_span.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_span.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_trunk.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_trunk.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_fastiron_show_version.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_fastiron_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_interfaces.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_lldp_neighbors_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_metro.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_metro.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_running-config_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_running-config_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_running-config_vlan.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_running-config_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_span.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_span.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/brocade_netiron_show_topo.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/brocade_netiron_show_topo.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/checkpoint_gaia_show_interfaces_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/checkpoint_gaia_show_interfaces_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/checkpoint_gaia_show_route.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/checkpoint_gaia_show_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ciena_saos_port_show.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ciena_saos_port_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ciena_saos_rstp_show.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ciena_saos_rstp_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ciena_saos_software_show.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ciena_saos_software_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ciena_saos_traffic-profiling_standard-profile_show.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ciena_saos_traffic-profiling_standard-profile_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ciena_saos_vlan_show.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ciena_saos_vlan_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_apic_fabric_show_vlan_extended.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_apic_fabric_show_vlan_extended.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_dir.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_dir.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_ping.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_ping.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_access-list.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_access-list.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_asp_drop.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_asp_drop.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_asp_table_vpn-context_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_asp_table_vpn-context_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_bgp_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_cpu_usage_detailed.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_cpu_usage_detailed.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_crypto_ipsec_sa.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_crypto_ipsec_sa.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_failover.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_failover.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_interface_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_interface_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_license_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_license_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_logging.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_logging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_module_details.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_module_details.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_nat.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_nat.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_object-group_network.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_object-group_network.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_port-channel_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_port-channel_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_route.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_running-config_all_crypto_map.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_running-config_all_crypto_map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_map.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_running-config_ipsec.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_running-config_ipsec.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_running-config_object_network.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_running-config_object_network.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_running-config_tunnel-group.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_running-config_tunnel-group.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_version.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_anyconnect.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_anyconnect.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_detail_l2l.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_detail_l2l.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_asa_show_xlate.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_asa_show_xlate.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ftd_show_vpn-sessiondb_anyconnect.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ftd_show_vpn-sessiondb_anyconnect.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_ping.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_ping.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_access-list.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_access-list.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_adjacency.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_adjacency.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ap_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ap_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_archive.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_archive.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_authentication_sessions_method_details.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_authentication_sessions_method_details.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_bfd_neighbors_details.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_bfd_neighbors_details.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_boot.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_boot.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_controller_t1.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_controller_t1.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_crypto_ipsec_sa_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_crypto_ipsec_sa_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_crypto_pki_certificates.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_crypto_pki_certificates.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_crypto_session_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_crypto_session_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_dhcp_lease.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_dhcp_lease.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_dot1x_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_dot1x_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_environment_temperature.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_environment_temperature.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_etherchannel_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_etherchannel_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_interface_link.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_interface_link.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_interfaces.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_interfaces_status.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_interfaces_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_interfaces_switchport.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_interfaces_switchport.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_inventory.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_inventory.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_access-lists.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_access-lists.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_arp.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_bgp.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_bgp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors_advertised-routes.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors_advertised-routes.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_bgp_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_bgp_vpnv4_all_neighbors.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_bgp_vpnv4_all_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_cef.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_cef.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_cef_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_cef_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_device_tracking_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_device_tracking_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_interfaces_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_interfaces_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_neighbors.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_topology.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_topology.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_http_server_status.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_http_server_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_mroute.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_mroute.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_nat_translations.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_nat_translations.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_network.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_network.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_router.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_router.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_route.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_route_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_route_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ip_source_binding.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ip_source_binding.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ipv6_access-lists.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ipv6_access-lists.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_ipv6_route.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_ipv6_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_isdn_status.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_isdn_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_license.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_license.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_logging.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_logging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_mac-address-table.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_mac-address-table.textfsm`

 * *Files 7% similar despite different names*

```diff
@@ -19,41 +19,41 @@
   ^Destination\s+Address\s+Address\s+Type\s+VLAN\s+Destination\s+Port
   ^\s*$$
   ^Multicast\s+Entries -> End
   ^. -> Error
 
 TYPE2
   # Order of the group in brackets here matters
-  ^\s*(\*\s+R|\*|R|\s)\s*(\d+|-+|[Nn]/[Aa]) -> Continue.Record
+  ^\s*(\*\s+[R,S,D]|\*|[R,S,D]|\s)\s*(\d+|-+|[Nn]/[Aa]) -> Continue.Record
   # using 20 spaces should ensure that lines only match destination port flowing to next line
   ^\s{20}\s+${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
   ^\s{20}\s+${DESTINATION_PORT},*\s*$$
   ^\s{20}\s+[^,\s]+(\s+|,\s*)${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
   ^\s{20}\s+[^,\s]+(\s+|,\s*)${DESTINATION_PORT},*\s*$$
   ^\s{20}\s+([^,\s]+(\s+|,\s*)){2}${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
   ^\s{20}\s+([^,\s]+(\s+|,\s*)){2}${DESTINATION_PORT},*\s*$$
   ^\s{20}\s+([^,\s]+(\s+|,\s*)){3}${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
   ^\s{20}\s+([^,\s]+(\s+|,\s*)){3}${DESTINATION_PORT},*\s*$$
   ^\s{20}\s+([^,\s]+(\s+|,\s*)){4}${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
   ^\s{20}\s+([^,\s]+(\s+|,\s*)){4}${DESTINATION_PORT},*\s*$$
   ^\s{20}\s+([^,\s]+(\s+|,\s*)){5}${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
   ^\s{20}\s+([^,\s]+(\s+|,\s*)){5}${DESTINATION_PORT},*\s*$$
-  ^\s*(\*\s+R|\*|R|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s*$$
-  ^\s*(\*\s+R|\*|R|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
-  ^\s*(\*\s+R|\*|R|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+${DESTINATION_PORT},*\s*$$
-  ^\s*(\*\s+R|\*|R|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+[^,\s]+(\s+|,\s*)${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
-  ^\s*(\*\s+R|\*|R|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+[^,\s]+?(\s+|,\s*)${DESTINATION_PORT},*\s*$$
-  ^\s*(\*\s+R|\*|R|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){2}${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
-  ^\s*(\*\s+R|\*|R|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){2}${DESTINATION_PORT},*\s*$$
-  ^\s*(\*\s+R|\*|R|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){3}${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
-  ^\s*(\*\s+R|\*|R|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){3}${DESTINATION_PORT},*\s*$$
-  ^\s*(\*\s+R|\*|R|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){4}${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
-  ^\s*(\*\s+R|\*|R|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){4}${DESTINATION_PORT},*\s*$$
-  ^\s*(\*\s+R|\*|R|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){5}${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
-  ^\s*(\*\s+R|\*|R|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){5}${DESTINATION_PORT},*\s*$$
+  ^\s*(\*\s+[R,S,D]|\*|[R,S,D]|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s*$$
+  ^\s*(\*\s+[R,S,D]|\*|[R,S,D]|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
+  ^\s*(\*\s+[R,S,D]|\*|[R,S,D]|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+${DESTINATION_PORT},*\s*$$
+  ^\s*(\*\s+[R,S,D]|\*|[R,S,D]|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+[^,\s]+(\s+|,\s*)${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
+  ^\s*(\*\s+[R,S,D]|\*|[R,S,D]|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+[^,\s]+?(\s+|,\s*)${DESTINATION_PORT},*\s*$$
+  ^\s*(\*\s+[R,S,D]|\*|[R,S,D]|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){2}${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
+  ^\s*(\*\s+[R,S,D]|\*|[R,S,D]|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){2}${DESTINATION_PORT},*\s*$$
+  ^\s*(\*\s+[R,S,D]|\*|[R,S,D]|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){3}${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
+  ^\s*(\*\s+[R,S,D]|\*|[R,S,D]|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){3}${DESTINATION_PORT},*\s*$$
+  ^\s*(\*\s+[R,S,D]|\*|[R,S,D]|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){4}${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
+  ^\s*(\*\s+[R,S,D]|\*|[R,S,D]|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){4}${DESTINATION_PORT},*\s*$$
+  ^\s*(\*\s+[R,S,D]|\*|[R,S,D]|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){5}${DESTINATION_PORT}(\s+|,\s*)\S -> Continue
+  ^\s*(\*\s+[R,S,D]|\*|[R,S,D]|\s)\s*${VLAN_ID}\s+${DESTINATION_ADDRESS}\s+${TYPE}\s+\S+\s+\S+\s+([^,\s]+(\s+|,\s*)){5}${DESTINATION_PORT},*\s*$$
   ^-+\+-+
   ^Displaying\s+entries
   ^\s+vlan\s+mac address\s+type\s+learn\s+age\s+ports
   ^\s*$$
   ^Multicast\s+Entries -> End
   ^. -> Error
```

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_module.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_module.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_module_online_diag.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_module_online_diag.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_module_status.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_module_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_module_submodule.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_module_submodule.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_object-group.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_object-group.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_platform_diag.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_platform_diag.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_port-security_interface_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_port-security_interface_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_power_available.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_power_available.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_power_status.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_power_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_processes_memory_sorted.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_processes_memory_sorted.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_redundancy.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_redundancy.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_route-map.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_route-map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_running-config_partition_access-list.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_running-config_partition_access-list.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_running-config_partition_route-map.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_running-config_partition_route-map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_snmp_group.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_snmp_group.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_snmp_user.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_snmp_user.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_standby.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_standby.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_standby_brief.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_standby_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_switch_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_switch_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_tacacs.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_tacacs.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_version.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_vlan.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_vlans.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_vlans.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_vrf.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_vrf.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_vrf_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_vrf_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_vrrp_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_vrrp_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_vrrp_brief.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_vrrp_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_show_vtp_status.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_show_vtp_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_ios_traceroute.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_ios_traceroute.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nvfis_show_bridge-settings.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nvfis_show_bridge-settings.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nvfis_show_running-config_system_time.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nvfis_show_running-config_system_time.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_access-lists.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_access-lists.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_bgp_vrf_all_ipv4_unicast_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_bgp_vrf_all_ipv4_unicast_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_bgp_vrf_all_ipv4_unicast_neighbors_routes.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_bgp_vrf_all_ipv4_unicast_neighbors_routes.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_cts_interface_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_cts_interface_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_environment.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_environment.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_fex_id.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_fex_id.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_forwarding_adjacency.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_forwarding_adjacency.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_forwarding_ipv4_route.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_forwarding_ipv4_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_hardware_internal_bigsur_all-ports_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_hardware_internal_bigsur_all-ports_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_hsrp_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_hsrp_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_interface_brief.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_interface_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver_details.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver_details.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_interfaces_switchport.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_interfaces_switchport.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_adjacency.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_adjacency.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_bgp.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_bgp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_neighbors.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary_vrf.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary_vrf.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_community-list.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_community-list.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_snooping_statistics.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_snooping_statistics.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_interface_vrf_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_interface_vrf_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_mroutes_vrf_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_mroutes_vrf_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_msdp_summary_vrf_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_msdp_summary_vrf_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_database.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_interface_brief.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_interface_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_pim_neighbor_vrf_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_pim_neighbor_vrf_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_pim_rp_vrf_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_pim_rp_vrf_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_ip_route.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_port-channel_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_port-channel_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_route-map.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_route-map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_version.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_vlan.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_nxos_show_vrf_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_nxos_show_vrf_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_interfaces_status.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_interfaces_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_interfaces_switchport.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_interfaces_switchport.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_ip_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_ip_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_system.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_system.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_s300_show_vlan.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_s300_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a_cleanair_config.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a_cleanair_config.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_advanced_802.11a_channel.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_advanced_802.11a_channel.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_config_general.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_config_general.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_image_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_image_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_band-select.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_band-select.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_cdp_neighbors_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_cdp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_client_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_client_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_detailed_id.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_detailed_id.textfsm`

 * *Files 16% similar despite different names*

```diff
@@ -14,29 +14,33 @@
   ^\s*IP\s+Gateway\.+\s+${GATEWAY}\s*$$
   ^\s*Primary\s+DHCP\s+Server\.+\s+${PRIMARY_DHCP_SERVER}\s*$$
   ^\s*Secondary\s+DHCP\s+Server\.+\s+${SECONDARY_DHCP_SERVER}\s*$$ -> Record
   ^\s*External\s+NAT\s+IP\s+State.*$$
   ^\s*External\s+NAT\s+IP\s+Address.*$$
   ^\s*Link\s+Local\s+IPv6\s+Address.*$$
   ^\s*STATE.*$$
+  ^\s*Primary\s+IPv6\s+Address.*$$
   ^\s*IPv6\s+Address.*$$
+  ^\s*Primary\s+IPv6\s+Gateway.*$$
   ^\s*IPv6\s+Gateway.*$$
+  ^\s*Primary\s+IPv6\s+Gateway\s+Mac\s+Address.*$$
   ^\s*IPv6\s+Gateway\s+Mac\s+Address.*$$
   ^\s*VLAN.*$$
   ^\s*Quarantine-vlan.*$$
   ^\s*NAS-Identifier.*$$
   ^\s*Active\s+Physical\s+Port.*$$
   ^\s*Primary\s+Physical\s+Port.*$$
   ^\s*Backup\s+Physical\s+Port.*$$
   ^\s*DHCP\s+Proxy\s+Mode.*$$
   ^\s*DHCP\s+Option\s+82.*$$
-  ^\s*DHCP\s+Option\s+82\s+bridge\s+mode\s+insertion.*$$
+  ^\s*DHCP\s+Option\s+82\s+bridge.*$$
   ^\s*DHCP\s+Option\s+6\s+Opendns\s+Override.*$$
   ^\s*IPv4\s+ACL.*$$
+  ^\s*URL\s+ACL.*$$
   ^\s*mDNS\s+Profile\s+Name.*$$
   ^\s*AP\s+Manager.*$$
   ^\s*Guest\s+Interface.*$$
   ^\s*3G\s+VLAN.*$$
   ^\s*L2\s+Multicast.*$$
-  ^\s*URL\s+ACL.*$$
+  ^\s*IPv6\s+ACL.*$$
   ^\s*$$
-  ^. -> Error
+  ^.* -> Error
```

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_sum.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_sum.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_port_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_port_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_radius_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_radius_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_stats_port_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_stats_port_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_sysinfo.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_sysinfo.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_tacacs_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_tacacs_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_wlc_ssh_show_time.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_wlc_ssh_show_time.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_admin_show_controller_fabric_health.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_admin_show_controller_fabric_health.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_admin_show_environment_fan.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_admin_show_environment_fan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_ping.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_ping.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_arp.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_asic-errors_all_location.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_asic-errors_all_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_bgp.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_bgp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_bgp_instance_all_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_bgp_instance_all_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_bgp_neighbors.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_bgp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_cdp_neighbors_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_cdp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_cef_drops_location.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_cef_drops_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_controllers_HundredGigabitEthernet.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_controllers_HundredGigabitEthernet.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_controllers_all_phy.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_controllers_all_phy.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_egress_location.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_egress_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_ingress_location.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_ingress_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_ingress_location.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_ingress_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_controllers_hundredgige_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_controllers_hundredgige_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_drops_np_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_drops_np_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_hsrp.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_hsrp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_install_active.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_install_active.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_interfaces.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_ip_bgp_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_ip_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_ip_route.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_ipv4_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_ipv4_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_lldp_neighbors_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_lpts_pifib_hardware_police_location.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_lpts_pifib_hardware_police_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_platform_summary_location_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_platform_summary_location_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/cisco_xr_show_version.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/cisco_xr_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/dell_force10_show_vlan.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/dell_force10_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/dell_powerconnect_show_interfaces_status.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/dell_powerconnect_show_interfaces_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/eltex_show_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/eltex_show_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/eltex_show_interfaces_description.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/eltex_show_interfaces_description.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/eltex_show_interfaces_status.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/eltex_show_interfaces_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/eltex_show_interfaces_switchport.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/eltex_show_interfaces_switchport.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/eltex_show_ip_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/eltex_show_ip_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/eltex_show_system.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/eltex_show_system.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/eltex_show_vlan.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/eltex_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ericsson_ipos_show_arp.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ericsson_ipos_show_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/extreme_exos_show_ipconfig.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/extreme_exos_show_ipconfig.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/extreme_exos_show_ports_information.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/extreme_exos_show_ports_information.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/extreme_exos_show_ports_information_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/extreme_exos_show_ports_information_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/extreme_exos_show_sharing.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/extreme_exos_show_sharing.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/fortinet_get_router_info_bgp_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/fortinet_get_router_info_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/fortinet_get_system_ha_status.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/fortinet_get_system_ha_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/fortinet_get_system_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/fortinet_get_system_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/fortinet_get_system_interface_physical.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/fortinet_get_system_interface_physical.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/fortinet_get_system_status.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/fortinet_get_system_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_counters_bound_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_counters_bound_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_device_manuinfo.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_device_manuinfo.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_interface_brief.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_interface_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_ip_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_ip_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_ip_routing-table.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_ip_routing-table.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance_instance-name.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance_instance-name.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_link-aggregation_verbose.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_link-aggregation_verbose.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_list.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_list.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_verbose.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_verbose.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_comware_display_vlan_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_comware_display_vlan_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_cdp_neighbors_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_cdp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_interfaces.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_interfaces_brief.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_interfaces_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_ip.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_ip.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device_detail.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/hp_procurve_show_system.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/hp_procurve_show_system.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_ont_autofind.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_ont_autofind.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_ont_info_by-sn_sn.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_ont_info_by-sn_sn.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_ont_info_fsp.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_ont_info_fsp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_port_info.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_port_info.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_smartax_display_version.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_smartax_display_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_acl_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_acl_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_arp_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_arp_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_interface.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_ip_routing-table_verbose.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_ip_routing-table_verbose.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_ipv6_neighbors.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_ipv6_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_lldp_neighbor.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_lldp_neighbor.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_nat_server.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_nat_server.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_port_vlan.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_port_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_service-set_id_id.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_service-set_id_id.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_startup.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_startup.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_traffic-filter_applied-record.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_traffic-filter_applied-record.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/huawei_vrp_display_vlan.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/huawei_vrp_display_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/index` & `ntc_templates-5.1.0/ntc_templates/templates/index`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ipinfusion_ocnos_show_lldp_table.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ipinfusion_ocnos_show_lldp_table.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_interfaces.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_status.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_chassis_hardware.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_chassis_hardware.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_ethernet-switching_table.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_ethernet-switching_table.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_interfaces.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_lacp_interfaces.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_lacp_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_system_uptime.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_system_uptime.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/juniper_junos_show_version.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/juniper_junos_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/juniper_screenos_get_route.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/juniper_screenos_get_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/linux_ip_address_show.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/linux_ip_address_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/linux_ip_link_show.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/linux_ip_link_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/linux_ip_route_show.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/linux_ip_route_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_monitor_name_once.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_monitor_name_once.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_poe_print_without-paging.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_poe_print_without-paging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_interface_print_terse_without-paging.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_interface_print_terse_without-paging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ip_address_print.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ip_address_print.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ip_dhcp-server_lease_print_without-paging.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ip_dhcp-server_lease_print_without-paging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_address-list_print_terse.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_address-list_print_terse.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_filter_print_all_without-paging.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_filter_print_all_without-paging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_nat_print_all_without-paging.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_nat_print_all_without-paging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ip_route_print_terse.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ip_route_print_terse.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_log_print_detail_without-paging.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_log_print_detail_without-paging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_ping.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_ping.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_routing_bgp_peer_print_status_without-paging.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_routing_bgp_peer_print_status_without-paging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_routing_ospf_neighbor_print_terse_without-paging.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_routing_ospf_neighbor_print_terse_without-paging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/mikrotik_routeros_system_routerboard_print.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/mikrotik_routeros_system_routerboard_print.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_high-availability_all.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_high-availability_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_interface_management.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_interface_management.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_running_nat-policy.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_running_nat-policy.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_running_security-policy.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_running_security-policy.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_show_system_info.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_show_system_info.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/paloalto_panos_test_security-policy-match.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/paloalto_panos_test_security-policy-match.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ruckus_fastiron_show_arp.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ruckus_fastiron_show_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ruckus_fastiron_show_interfaces.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ruckus_fastiron_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ruckus_fastiron_show_interfaces_brief.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ruckus_fastiron_show_interfaces_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ruckus_fastiron_show_version.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ruckus_fastiron_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ruckus_fastiron_show_vlan.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ruckus_fastiron_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgerouter_show_ip_route.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgerouter_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgerouter_show_nat_rules.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgerouter_show_nat_rules.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/ubiquiti_edgeswitch_show_version.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/ubiquiti_edgeswitch_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/vyatta_vyos_show_ip_bgp_summary.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/vyatta_vyos_show_ip_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/yamaha_show_environment.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/yamaha_show_environment.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_firewall_acl_get.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_firewall_acl_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_ipalias_get.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_ipalias_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_lan_get_--Name_name.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_lan_get_--Name_name.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_nat_addr_map_get.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_nat_addr_map_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_nat_get.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_nat_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_snmp_get.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_snmp_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_static_route_get.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_static_route_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_cfg_wlan_get.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_cfg_wlan_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/ntc_templates/templates/zyxel_os_sys_atsh.textfsm` & `ntc_templates-5.1.0/ntc_templates/templates/zyxel_os_sys_atsh.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-5.0.0/pyproject.toml` & `ntc_templates-5.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ntc_templates"
-version = "v5.0.0"
+version = "v5.1.0"
 description = "TextFSM Templates for Network Devices, and Python wrapper for TextFSM's CliTable."
 authors = ["Network to Code <info@networktocode.com>"]
 license = "Apache-2.0"
 homepage = "https://ntc-templates.readthedocs.io"
 repository = "https://github.com/networktocode/ntc-templates"
 documentation = "https://ntc-templates.readthedocs.io"
 readme = "README.md"
```

### Comparing `ntc_templates-5.0.0/PKG-INFO` & `ntc_templates-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntc_templates
-Version: 5.0.0
+Version: 5.1.0
 Summary: TextFSM Templates for Network Devices, and Python wrapper for TextFSM's CliTable.
 Home-page: https://ntc-templates.readthedocs.io
 License: Apache-2.0
 Keywords: textfsm,network parsers
 Author: Network to Code
 Author-email: info@networktocode.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ntc_templates Version: 5.0.0 Summary: TextFSM
+Metadata-Version: 2.1 Name: ntc_templates Version: 5.1.0 Summary: TextFSM
 Templates for Network Devices, and Python wrapper for TextFSM's CliTable. Home-
 page: https://ntc-templates.readthedocs.io License: Apache-2.0 Keywords:
 textfsm,network parsers Author: Network to Code Author-email:
 info@networktocode.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
```

