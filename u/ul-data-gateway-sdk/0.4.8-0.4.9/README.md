# Comparing `tmp/ul-data-gateway-sdk-0.4.8.tar.gz` & `tmp/ul-data-gateway-sdk-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-data-gateway-sdk-0.4.8.tar", last modified: Tue Sep 19 10:18:38 2023, max compression
+gzip compressed data, was "ul-data-gateway-sdk-0.4.9.tar", last modified: Tue Sep 19 11:11:32 2023, max compression
```

## Comparing `ul-data-gateway-sdk-0.4.8.tar` & `ul-data-gateway-sdk-0.4.9.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.643185 ul-data-gateway-sdk-0.4.8/
--rw-r--r--   0 root         (0) root         (0)    13358 2023-09-19 10:18:38.639185 ul-data-gateway-sdk-0.4.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12799 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.611184 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.611184 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1465 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/__tests__/test_encryption.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.611184 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.611184 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3900 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/__tests__/crypto_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.611184 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/constants/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/constants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3510 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/constants/constants_aes.py
--rw-rw-rw-   0 root         (0) root         (0)     6855 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/constants/constants_kuz.py
--rw-rw-rw-   0 root         (0) root         (0)   132363 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/constants/kuz_tables.bin
--rw-rw-rw-   0 root         (0) root         (0)    14821 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/crypto_aes.py
--rw-rw-rw-   0 root         (0) root         (0)     9175 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/crypto_kuznechik.py
--rw-rw-rw-   0 root         (0) root         (0)     4405 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/crypto_xtea.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.611184 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/extensions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/extensions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/extensions/errors.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/extensions/type_alias.py
--rw-rw-rw-   0 root         (0) root         (0)    18900 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/device_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2305 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/device_data_encryption.py
--rw-rw-rw-   0 root         (0) root         (0)     5322 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/device_data_protocol.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.611184 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/messages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/messages/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/messages/input_bs_http_nero_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1652 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/nero_bs_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.611184 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.611184 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.611184 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    49906 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/__tests__/test_device_protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     1964 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/device_packet.py
--rw-rw-rw-   0 root         (0) root         (0)     2830 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/ncp_smp_device_packet.py
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/smp_device_packet.py
--rw-rw-rw-   0 root         (0) root         (0)     7800 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/smpm_device_packet.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/water5_device_packet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.615184 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/nero_bs_packet/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/nero_bs_packet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.615184 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/nero_bs_packet/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/nero_bs_packet/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11930 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/nero_bs_packet/__tests__/http_nero_bs_packet.py
--rw-rw-rw-   0 root         (0) root         (0)    14061 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/nero_bs_packet/__tests__/test_bs_protocol.py
--rw-rw-rw-   0 root         (0) root         (0)    12290 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/nero_bs_packet/http_nero_bs_packet.py
--rw-rw-rw-   0 root         (0) root         (0)     4736 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/nero_bs_packet/kafka_nero_bs_packet.py
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/nero_bs_packet/nero_bs_packet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.619184 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.631185 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20286 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_consumed.py
--rw-rw-rw-   0 root         (0) root         (0)    20421 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_generated.py
--rw-rw-rw-   0 root         (0) root         (0)    41491 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)    16998 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_device_info.py
--rw-rw-rw-   0 root         (0) root         (0)   695189 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_electricity_params.py
--rw-rw-rw-   0 root         (0) root         (0)     4850 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_info.py
--rw-rw-rw-   0 root         (0) root         (0)    10024 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_journal.py
--rw-rw-rw-   0 root         (0) root         (0)     6985 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h1_energy.py
--rw-rw-rw-   0 root         (0) root         (0)     6985 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h2_energy.py
--rw-rw-rw-   0 root         (0) root         (0)     6985 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h3_energy.py
--rw-rw-rw-   0 root         (0) root         (0)     6432 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_ar.py
--rw-rw-rw-   0 root         (0) root         (0)     4474 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_energy.py
--rw-rw-rw-   0 root         (0) root         (0)     3748 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_f.py
--rw-rw-rw-   0 root         (0) root         (0)     6627 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_pqs.py
--rw-rw-rw-   0 root         (0) root         (0)    55642 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_retrospective_energy.py
--rw-rw-rw-   0 root         (0) root         (0)    21368 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_status_info.py
--rw-rw-rw-   0 root         (0) root         (0)    24530 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_consumed.py
--rw-rw-rw-   0 root         (0) root         (0)    24665 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_generated.py
--rw-rw-rw-   0 root         (0) root         (0)     8394 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_08b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)   381664 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_16b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)  5475148 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_group_meter_daily.py
--rw-rw-rw-   0 root         (0) root         (0)    21659 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_proxy_meter_16b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_internal_info.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter.py
--rw-rw-rw-   0 root         (0) root         (0)     4907 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch1.py
--rw-rw-rw-   0 root         (0) root         (0)     4907 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch2.py
--rw-rw-rw-   0 root         (0) root         (0)    10076 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_12b_counter.py
--rw-rw-rw-   0 root         (0) root         (0)   127594 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_16b_counter.py
--rw-rw-rw-   0 root         (0) root         (0)     3651 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_04b_event.py
--rw-rw-rw-   0 root         (0) root         (0)     9461 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)     3003 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_info.py
--rw-rw-rw-   0 root         (0) root         (0)   166938 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_12b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)   394524 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_16b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/test_self_package_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     8772 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_consumed.py
--rw-rw-rw-   0 root         (0) root         (0)     8631 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_generated.py
--rw-rw-rw-   0 root         (0) root         (0)    14021 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)     5174 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_device_info.py
--rw-rw-rw-   0 root         (0) root         (0)    11000 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_electricity_params.py
--rw-rw-rw-   0 root         (0) root         (0)     6353 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_info.py
--rw-rw-rw-   0 root         (0) root         (0)    33661 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_journal.py
--rw-rw-rw-   0 root         (0) root         (0)    12665 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h1_energy.py
--rw-rw-rw-   0 root         (0) root         (0)    12664 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h2_energy.py
--rw-rw-rw-   0 root         (0) root         (0)    12645 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h3_energy.py
--rw-rw-rw-   0 root         (0) root         (0)    19205 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_ar.py
--rw-rw-rw-   0 root         (0) root         (0)    16881 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_energy.py
--rw-rw-rw-   0 root         (0) root         (0)    17912 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_f.py
--rw-rw-rw-   0 root         (0) root         (0)    29940 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_pqs.py
--rw-rw-rw-   0 root         (0) root         (0)    13774 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_retrospective_energy.py
--rw-rw-rw-   0 root         (0) root         (0)     6805 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_status_info.py
--rw-rw-rw-   0 root         (0) root         (0)    11094 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_consumed.py
--rw-rw-rw-   0 root         (0) root         (0)    11037 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_generated.py
--rw-rw-rw-   0 root         (0) root         (0)     7867 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_08b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)    16487 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_16b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)    88824 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_group_meter_daily.py
--rw-rw-rw-   0 root         (0) root         (0)    10826 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_proxy_meter_16b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)     4409 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_internal_info.py
--rw-rw-rw-   0 root         (0) root         (0)     4404 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter.py
--rw-rw-rw-   0 root         (0) root         (0)     4992 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch1.py
--rw-rw-rw-   0 root         (0) root         (0)     4986 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch2.py
--rw-rw-rw-   0 root         (0) root         (0)     6540 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_12b_counter.py
--rw-rw-rw-   0 root         (0) root         (0)    11572 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_16b_counter.py
--rw-rw-rw-   0 root         (0) root         (0)     5696 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_04b_event.py
--rw-rw-rw-   0 root         (0) root         (0)     9447 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)     5068 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_info.py
--rw-rw-rw-   0 root         (0) root         (0)    14449 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_12b_daily.py
--rw-rw-rw-   0 root         (0) root         (0)    17079 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_16b_daily.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.631185 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/udp_wrapper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/udp_wrapper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.631185 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/udp_wrapper/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/udp_wrapper/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/udp_wrapper/__tests__/unbp_len.py
--rw-rw-rw-   0 root         (0) root         (0)     5542 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/udp_wrapper/unbp_len.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.635185 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.639185 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/test_self_package_tests.py
--rw-rw-rw-   0 root         (0) root         (0)      771 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_cold_reset.py
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_daily.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch1.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch2.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_magnet.py
--rw-rw-rw-   0 root         (0) root         (0)     3930 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_a.py
--rw-rw-rw-   0 root         (0) root         (0)     8688 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_freescale.py
--rw-rw-rw-   0 root         (0) root         (0)     8271 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_stm.py
--rw-rw-rw-   0 root         (0) root         (0)     8892 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_freescale.py
--rw-rw-rw-   0 root         (0) root         (0)     4121 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_stm.py
--rw-rw-rw-   0 root         (0) root         (0)     8338 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_metano_a.py
--rw-rw-rw-   0 root         (0) root         (0)     3539 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1.py
--rw-rw-rw-   0 root         (0) root         (0)     3796 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse.py
--rw-rw-rw-   0 root         (0) root         (0)     3880 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     3539 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2.py
--rw-rw-rw-   0 root         (0) root         (0)     3796 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse.py
--rw-rw-rw-   0 root         (0) root         (0)     3880 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_cold_reset.py
--rw-rw-rw-   0 root         (0) root         (0)     2522 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_daily.py
--rw-rw-rw-   0 root         (0) root         (0)     2525 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch1.py
--rw-rw-rw-   0 root         (0) root         (0)     2589 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch2.py
--rw-rw-rw-   0 root         (0) root         (0)     1795 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_magnet.py
--rw-rw-rw-   0 root         (0) root         (0)     3913 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_a.py
--rw-rw-rw-   0 root         (0) root         (0)     4665 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_freescale.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_stm.py
--rw-rw-rw-   0 root         (0) root         (0)     4333 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_freescale.py
--rw-rw-rw-   0 root         (0) root         (0)     4063 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_stm.py
--rw-rw-rw-   0 root         (0) root         (0)     4697 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_metano_a.py
--rw-rw-rw-   0 root         (0) root         (0)     3682 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1.py
--rw-rw-rw-   0 root         (0) root         (0)     3700 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse.py
--rw-rw-rw-   0 root         (0) root         (0)     3771 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     3682 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2.py
--rw-rw-rw-   0 root         (0) root         (0)     3762 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse.py
--rw-rw-rw-   0 root         (0) root         (0)     3709 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse_v2.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.639185 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.639185 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/utils/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/utils/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1387 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/utils/__tests__/timestamp_calculation.py
--rw-rw-rw-   0 root         (0) root         (0)     2086 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/utils/buf_ref.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/utils/days_ago_calculation.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/utils/packet.py
--rw-rw-rw-   0 root         (0) root         (0)     1514 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/utils/timestamp_calculation.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/data_gateway_sdk/utils/true_round.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-19 10:18:38.643185 ul-data-gateway-sdk-0.4.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1533 2023-09-19 10:18:31.000000 ul-data-gateway-sdk-0.4.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 10:18:38.639185 ul-data-gateway-sdk-0.4.8/ul_data_gateway_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13358 2023-09-19 10:18:38.000000 ul-data-gateway-sdk-0.4.8/ul_data_gateway_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11227 2023-09-19 10:18:38.000000 ul-data-gateway-sdk-0.4.8/ul_data_gateway_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-19 10:18:38.000000 ul-data-gateway-sdk-0.4.8/ul_data_gateway_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-09-19 10:18:38.000000 ul-data-gateway-sdk-0.4.8/ul_data_gateway_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-09-19 10:18:38.000000 ul-data-gateway-sdk-0.4.8/ul_data_gateway_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.760398 ul-data-gateway-sdk-0.4.9/
+-rw-r--r--   0 root         (0) root         (0)    13358 2023-09-19 11:11:32.760398 ul-data-gateway-sdk-0.4.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12799 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.724394 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.724394 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1465 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/__tests__/test_encryption.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.724394 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.724394 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3900 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/__tests__/crypto_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.724394 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/constants/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/constants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3510 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/constants/constants_aes.py
+-rw-rw-rw-   0 root         (0) root         (0)     6855 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/constants/constants_kuz.py
+-rw-rw-rw-   0 root         (0) root         (0)   132363 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/constants/kuz_tables.bin
+-rw-rw-rw-   0 root         (0) root         (0)    14821 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/crypto_aes.py
+-rw-rw-rw-   0 root         (0) root         (0)     9175 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/crypto_kuznechik.py
+-rw-rw-rw-   0 root         (0) root         (0)     4405 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/crypto_xtea.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.724394 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/extensions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/extensions/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/extensions/type_alias.py
+-rw-rw-rw-   0 root         (0) root         (0)    18900 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/device_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/device_data_encryption.py
+-rw-rw-rw-   0 root         (0) root         (0)     5322 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/device_data_protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.724394 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/messages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/messages/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/messages/input_bs_http_nero_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1652 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/nero_bs_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.724394 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.728394 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.728394 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    49906 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/__tests__/test_device_protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/device_packet.py
+-rw-rw-rw-   0 root         (0) root         (0)     2830 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/ncp_smp_device_packet.py
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/smp_device_packet.py
+-rw-rw-rw-   0 root         (0) root         (0)     7800 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/smpm_device_packet.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/water5_device_packet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.728394 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/nero_bs_packet/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/nero_bs_packet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.728394 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/nero_bs_packet/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/nero_bs_packet/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11930 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/nero_bs_packet/__tests__/http_nero_bs_packet.py
+-rw-rw-rw-   0 root         (0) root         (0)    14061 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/nero_bs_packet/__tests__/test_bs_protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)    12290 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/nero_bs_packet/http_nero_bs_packet.py
+-rw-rw-rw-   0 root         (0) root         (0)     4736 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/nero_bs_packet/kafka_nero_bs_packet.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/nero_bs_packet/nero_bs_packet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.736395 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.752397 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20286 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_consumed.py
+-rw-rw-rw-   0 root         (0) root         (0)    20421 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_generated.py
+-rw-rw-rw-   0 root         (0) root         (0)    41491 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)    16998 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_device_info.py
+-rw-rw-rw-   0 root         (0) root         (0)   695189 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_electricity_params.py
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    10024 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_journal.py
+-rw-rw-rw-   0 root         (0) root         (0)     6985 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h1_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6985 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h2_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6985 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h3_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6432 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_ar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4474 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3748 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_f.py
+-rw-rw-rw-   0 root         (0) root         (0)     6627 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_pqs.py
+-rw-rw-rw-   0 root         (0) root         (0)    55642 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_retrospective_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)    21368 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_status_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    24530 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_consumed.py
+-rw-rw-rw-   0 root         (0) root         (0)    24665 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_generated.py
+-rw-rw-rw-   0 root         (0) root         (0)     8394 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_08b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)   381664 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_16b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)  5475148 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_group_meter_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)    21659 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_proxy_meter_16b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_internal_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4907 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4907 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10076 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_12b_counter.py
+-rw-rw-rw-   0 root         (0) root         (0)   127594 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_16b_counter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3651 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_04b_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     9461 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)     3003 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_info.py
+-rw-rw-rw-   0 root         (0) root         (0)   166938 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_12b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)   394524 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_16b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/test_self_package_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     8772 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_consumed.py
+-rw-rw-rw-   0 root         (0) root         (0)     8631 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_generated.py
+-rw-rw-rw-   0 root         (0) root         (0)    14021 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)     5174 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_device_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    11000 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_electricity_params.py
+-rw-rw-rw-   0 root         (0) root         (0)     6353 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    33661 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_journal.py
+-rw-rw-rw-   0 root         (0) root         (0)    12665 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h1_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)    12664 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h2_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)    12645 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h3_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)    19205 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_ar.py
+-rw-rw-rw-   0 root         (0) root         (0)    16881 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)    17912 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_f.py
+-rw-rw-rw-   0 root         (0) root         (0)    29940 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_pqs.py
+-rw-rw-rw-   0 root         (0) root         (0)    13774 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_retrospective_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6805 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_status_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    11094 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_consumed.py
+-rw-rw-rw-   0 root         (0) root         (0)    11037 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_generated.py
+-rw-rw-rw-   0 root         (0) root         (0)     7867 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_08b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)    16487 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_16b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)    88824 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_group_meter_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)    10826 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_proxy_meter_16b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)     4409 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_internal_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     4404 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4992 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4986 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6540 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_12b_counter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11572 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_16b_counter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5696 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_04b_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     9447 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)     5068 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    14449 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_12b_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)    17079 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_16b_daily.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.752397 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/udp_wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/udp_wrapper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.752397 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/udp_wrapper/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/udp_wrapper/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/udp_wrapper/__tests__/unbp_len.py
+-rw-rw-rw-   0 root         (0) root         (0)     5542 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/udp_wrapper/unbp_len.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.756397 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.756397 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/test_self_package_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      771 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_cold_reset.py
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch1.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch2.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_magnet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3930 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_a.py
+-rw-rw-rw-   0 root         (0) root         (0)     8688 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_freescale.py
+-rw-rw-rw-   0 root         (0) root         (0)     8271 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_stm.py
+-rw-rw-rw-   0 root         (0) root         (0)     8892 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_freescale.py
+-rw-rw-rw-   0 root         (0) root         (0)     4121 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_stm.py
+-rw-rw-rw-   0 root         (0) root         (0)     8338 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_metano_a.py
+-rw-rw-rw-   0 root         (0) root         (0)     3539 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3796 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3539 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3796 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_cold_reset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2522 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_daily.py
+-rw-rw-rw-   0 root         (0) root         (0)     2525 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch1.py
+-rw-rw-rw-   0 root         (0) root         (0)     2589 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_magnet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3913 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_a.py
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_freescale.py
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_stm.py
+-rw-rw-rw-   0 root         (0) root         (0)     4333 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_freescale.py
+-rw-rw-rw-   0 root         (0) root         (0)     4063 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_stm.py
+-rw-rw-rw-   0 root         (0) root         (0)     4697 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_metano_a.py
+-rw-rw-rw-   0 root         (0) root         (0)     3682 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3700 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3682 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3762 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3709 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.760398 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.760398 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/utils/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/utils/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1387 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/utils/__tests__/timestamp_calculation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/utils/buf_ref.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/utils/days_ago_calculation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/utils/packet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1514 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/utils/timestamp_calculation.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/data_gateway_sdk/utils/true_round.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-19 11:11:32.760398 ul-data-gateway-sdk-0.4.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2023-09-19 11:11:25.000000 ul-data-gateway-sdk-0.4.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 11:11:32.760398 ul-data-gateway-sdk-0.4.9/ul_data_gateway_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13358 2023-09-19 11:11:32.000000 ul-data-gateway-sdk-0.4.9/ul_data_gateway_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11227 2023-09-19 11:11:32.000000 ul-data-gateway-sdk-0.4.9/ul_data_gateway_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-19 11:11:32.000000 ul-data-gateway-sdk-0.4.9/ul_data_gateway_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-09-19 11:11:32.000000 ul-data-gateway-sdk-0.4.9/ul_data_gateway_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-09-19 11:11:32.000000 ul-data-gateway-sdk-0.4.9/ul_data_gateway_sdk.egg-info/top_level.txt
```

### Comparing `ul-data-gateway-sdk-0.4.8/PKG-INFO` & `ul-data-gateway-sdk-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-gateway-sdk
-Version: 0.4.8
+Version: 0.4.9
 Summary: Data gateway sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-gateway-sdk-0.4.8/README.md` & `ul-data-gateway-sdk-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/__tests__/test_encryption.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/__tests__/test_encryption.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/__tests__/crypto_test.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/__tests__/crypto_test.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/constants/constants_aes.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/constants/constants_aes.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/constants/constants_kuz.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/constants/constants_kuz.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/constants/kuz_tables.bin` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/constants/kuz_tables.bin`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/crypto_aes.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/crypto_aes.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/crypto_kuznechik.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/crypto_kuznechik.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/crypto_xtea.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/crypto_xtea.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/crypto_algorithms/extensions/errors.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/crypto_algorithms/extensions/errors.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/device_data.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/device_data.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/device_data_encryption.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/device_data_encryption.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/device_data_protocol.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/device_data_protocol.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/nero_bs_protocol.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/nero_bs_protocol.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/__tests__/test_device_protocol.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/__tests__/test_device_protocol.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/device_packet.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/device_packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/ncp_smp_device_packet.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/ncp_smp_device_packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/smp_device_packet.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/smp_device_packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/smpm_device_packet.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/smpm_device_packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/device_packet/water5_device_packet.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/device_packet/water5_device_packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/nero_bs_packet/__tests__/http_nero_bs_packet.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/nero_bs_packet/__tests__/http_nero_bs_packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/nero_bs_packet/__tests__/test_bs_protocol.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/nero_bs_packet/__tests__/test_bs_protocol.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/nero_bs_packet/http_nero_bs_packet.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/nero_bs_packet/http_nero_bs_packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/nero_bs_packet/kafka_nero_bs_packet.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/nero_bs_packet/kafka_nero_bs_packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_consumed.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_consumed.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_generated.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_3phase_generated.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_device_info.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_device_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_electricity_params.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_electricity_params.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_info.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_journal.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_journal.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h1_energy.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h1_energy.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h2_energy.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h2_energy.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h3_energy.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h3_energy.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_ar.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_ar.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_energy.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_energy.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_f.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_f.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_pqs.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_profile_8h_pqs.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_retrospective_energy.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_retrospective_energy.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_status_info.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_status_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_consumed.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_consumed.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_generated.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_energy_16b_tariff_generated.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_08b_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_08b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_16b_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_gaz_flow_16b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_group_meter_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_group_meter_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_proxy_meter_16b_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_heat_proxy_meter_16b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_internal_info.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_internal_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch1.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch1.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch2.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_08b_counter_ch2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_12b_counter.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_12b_counter.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_16b_counter.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_jupiter_16b_counter.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_04b_event.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_04b_event.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_info.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_08b_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_12b_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_12b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_16b_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/smpm_ul_device_water_meter_16b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/__tests__/test_self_package_tests.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/__tests__/test_self_package_tests.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_consumed.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_consumed.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_generated.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_3phase_generated.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_device_info.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_device_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_electricity_params.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_electricity_params.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_info.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_journal.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_journal.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h1_energy.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h1_energy.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h2_energy.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h2_energy.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h3_energy.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h3_energy.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_ar.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_ar.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_energy.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_energy.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_f.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_f.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_pqs.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_profile_8h_pqs.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_retrospective_energy.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_retrospective_energy.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_status_info.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_status_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_consumed.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_consumed.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_generated.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_energy_16b_tariff_generated.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_08b_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_08b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_16b_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_gaz_flow_16b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_group_meter_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_group_meter_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_proxy_meter_16b_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_heat_proxy_meter_16b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_internal_info.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_internal_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch1.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch1.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch2.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_08b_counter_ch2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_12b_counter.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_12b_counter.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_16b_counter.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_jupiter_16b_counter.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_04b_event.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_04b_event.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_info.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_08b_info.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_12b_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_12b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_16b_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/smpm/smpm_ul_device_water_meter_16b_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/udp_wrapper/__tests__/unbp_len.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/udp_wrapper/__tests__/unbp_len.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/udp_wrapper/unbp_len.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/udp_wrapper/unbp_len.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/test_self_package_tests.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/test_self_package_tests.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_cold_reset.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_cold_reset.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch1.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch1.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch2.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_info_ch2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_a.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_a.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_freescale.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_freescale.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_stm.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_fluo_stm.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_freescale.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_freescale.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_stm.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_jupiter_stm.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_metano_a.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_warm_reset_v_metano_a.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse_v2.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch1_impulse_v2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse_v2.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/__tests__/water5_device_weekly_ch2_impulse_v2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_cold_reset.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_cold_reset.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_daily.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_daily.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch1.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch1.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch2.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_info_ch2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_magnet.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_magnet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_a.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_a.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_freescale.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_freescale.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_stm.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_fluo_stm.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_freescale.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_freescale.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_stm.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_jupiter_stm.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_metano_a.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_warm_reset_v_metano_a.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse_v2.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch1_impulse_v2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse_v2.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/protocols/water5_v_nero/water5_device_weekly_ch2_impulse_v2.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/utils/__tests__/timestamp_calculation.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/utils/__tests__/timestamp_calculation.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/utils/buf_ref.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/utils/buf_ref.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/utils/packet.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/utils/packet.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/data_gateway_sdk/utils/timestamp_calculation.py` & `ul-data-gateway-sdk-0.4.9/data_gateway_sdk/utils/timestamp_calculation.py`

 * *Files identical despite different names*

### Comparing `ul-data-gateway-sdk-0.4.8/setup.py` & `ul-data-gateway-sdk-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-data-gateway-sdk',
-    version='0.4.8',
+    version='0.4.9',
     description='Data gateway sdk',
     author='Unic-lab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(include=['data_gateway_sdk*']),
     include_package_data=True,
     package_data={
```

### Comparing `ul-data-gateway-sdk-0.4.8/ul_data_gateway_sdk.egg-info/PKG-INFO` & `ul-data-gateway-sdk-0.4.9/ul_data_gateway_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-gateway-sdk
-Version: 0.4.8
+Version: 0.4.9
 Summary: Data gateway sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-gateway-sdk-0.4.8/ul_data_gateway_sdk.egg-info/SOURCES.txt` & `ul-data-gateway-sdk-0.4.9/ul_data_gateway_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

