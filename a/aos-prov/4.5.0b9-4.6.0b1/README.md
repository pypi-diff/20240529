# Comparing `tmp/aos_prov-4.5.0b9-py3-none-any.whl.zip` & `tmp/aos_prov-4.6.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,68 +1,81 @@
-Zip file size: 71451 bytes, number of entries: 66
--rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/__init__.py
--rw-rw-r--  2.0 unx     3203 b- defN 24-Feb-02 11:35 aos_prov/actions.py
--rw-rw-r--  2.0 unx     8747 b- defN 24-Mar-20 16:06 aos_prov/main.py
--rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/commands/__init__.py
--rw-rw-r--  2.0 unx     7018 b- defN 24-Feb-02 11:35 aos_prov/commands/command_provision.py
--rw-rw-r--  2.0 unx     5050 b- defN 23-Dec-13 16:53 aos_prov/commands/command_vm.py
--rw-rw-r--  2.0 unx    17537 b- defN 24-Feb-02 11:35 aos_prov/commands/command_vm_multi_node_manage.py
--rw-rw-r--  2.0 unx     2300 b- defN 24-Feb-02 11:35 aos_prov/commands/download.py
--rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/__init__.py
--rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/cloud/__init__.py
--rw-rw-r--  2.0 unx     7892 b- defN 24-Mar-20 16:13 aos_prov/communication/cloud/cloud_api.py
--rw-rw-r--  2.0 unx       89 b- defN 22-Apr-10 14:06 aos_prov/communication/unit/__init__.py
--rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v0/__init__.py
--rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Dec-13 10:51 aos_prov/communication/unit/v2/__init__.py
--rw-rw-r--  2.0 unx     6965 b- defN 24-Feb-02 11:35 aos_prov/communication/unit/v2/unit_communication_v2.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Dec-26 17:29 aos_prov/communication/unit/v2/generated/__init__.py
--rw-rw-r--  2.0 unx     5410 b- defN 24-Feb-02 11:35 aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py
--rw-rw-r--  2.0 unx      159 b- defN 23-Dec-26 17:29 aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py
--rw-rw-r--  2.0 unx    24479 b- defN 24-Feb-02 11:35 aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py
--rw-rw-r--  2.0 unx    16471 b- defN 24-Feb-02 11:35 aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py
--rw-rw-r--  2.0 unx    17275 b- defN 24-Feb-02 11:35 aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py
--rw-rw-r--  2.0 unx    12921 b- defN 24-Feb-02 11:35 aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Dec-13 10:51 aos_prov/communication/unit/v3/__init__.py
--rw-rw-r--  2.0 unx     6757 b- defN 24-Jan-25 11:39 aos_prov/communication/unit/v3/unit_communication_v3.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Oct-12 12:56 aos_prov/communication/unit/v3/generated/__init__.py
--rw-rw-r--  2.0 unx     5409 b- defN 23-Dec-13 11:17 aos_prov/communication/unit/v3/generated/iamanagercommon_pb2.py
--rw-rw-r--  2.0 unx      159 b- defN 22-Oct-12 12:56 aos_prov/communication/unit/v3/generated/iamanagercommon_pb2_grpc.py
--rw-rw-r--  2.0 unx    24470 b- defN 23-Dec-13 11:40 aos_prov/communication/unit/v3/generated/iamanagerprotected_pb2.py
--rw-rw-r--  2.0 unx    16454 b- defN 23-Dec-13 11:41 aos_prov/communication/unit/v3/generated/iamanagerprotected_pb2_grpc.py
--rw-rw-r--  2.0 unx    17266 b- defN 23-Dec-13 11:41 aos_prov/communication/unit/v3/generated/iamanagerpublic_pb2.py
--rw-rw-r--  2.0 unx    12904 b- defN 23-Dec-13 11:41 aos_prov/communication/unit/v3/generated/iamanagerpublic_pb2_grpc.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/__init__.py
--rw-rw-r--  2.0 unx     8695 b- defN 24-Feb-02 11:35 aos_prov/communication/unit/v4/unit_communication_v4.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/generated/__init__.py
--rw-rw-r--  2.0 unx    18433 b- defN 24-Feb-02 11:35 aos_prov/communication/unit/v4/generated/iamanager_pb2.py
--rw-rw-r--  2.0 unx    33413 b- defN 24-Feb-02 11:35 aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py
--rw-rw-r--  2.0 unx     2705 b- defN 22-Apr-10 14:06 aos_prov/files/1rootCA.crt
--rw-rw-r--  2.0 unx      748 b- defN 22-Nov-13 13:27 aos_prov/utils/__init__.py
--rw-rw-r--  2.0 unx     1634 b- defN 24-Feb-02 11:35 aos_prov/utils/common.py
--rw-rw-r--  2.0 unx     2153 b- defN 24-Feb-02 11:35 aos_prov/utils/config.py
--rw-rw-r--  2.0 unx      645 b- defN 24-Feb-02 11:35 aos_prov/utils/errors.py
--rw-rw-r--  2.0 unx      972 b- defN 24-Feb-02 11:35 aos_prov/utils/unit_certificate.py
--rw-rw-r--  2.0 unx     5977 b- defN 24-Mar-20 17:03 aos_prov/utils/user_credentials.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Jan-04 11:02 test/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Jan-04 11:02 test/utils/__init__.py
--rw-rw-r--  2.0 unx      642 b- defN 24-Jan-04 11:02 test/utils/test_config.py
--rw-rw-r--  2.0 unx      632 b- defN 24-Jan-04 11:02 test/utils/test_unit_certificate.py
--rw-rw-r--  2.0 unx      439 b- defN 24-Jan-04 11:02 test/utils/test_user_credentials.py
--rw-rw-r--  2.0 unx       89 b- defN 24-Feb-02 11:35 tests/__init__.py
--rw-rw-r--  2.0 unx     4390 b- defN 24-Feb-02 11:35 tests/fixtures.py
--rw-rw-r--  2.0 unx     3257 b- defN 24-Feb-02 11:35 tests/test_actions.py
--rw-rw-r--  2.0 unx       89 b- defN 24-Feb-02 11:35 tests/commands/__init__.py
--rw-rw-r--  2.0 unx    17566 b- defN 24-Feb-02 11:35 tests/commands/test_command_provision.py
--rw-rw-r--  2.0 unx    13737 b- defN 24-Feb-02 11:35 tests/commands/test_command_vm_multi_node_manage.py
--rw-rw-r--  2.0 unx     3584 b- defN 24-Feb-02 11:35 tests/commands/test_download.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Feb-02 11:35 tests/utils/__init__.py
--rw-rw-r--  2.0 unx     1798 b- defN 24-Feb-02 11:35 tests/utils/test_common.py
--rw-rw-r--  2.0 unx     1120 b- defN 24-Feb-02 11:35 tests/utils/test_config.py
--rw-rw-r--  2.0 unx      721 b- defN 24-Feb-02 11:35 tests/utils/test_unit_certificate.py
--rw-rw-r--  2.0 unx     3693 b- defN 24-Mar-20 17:02 tests/utils/test_user_credentials.py
--rw-rw-r--  2.0 unx     2549 b- defN 24-Mar-20 17:04 aos_prov-4.5.0b9.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-20 17:04 aos_prov-4.5.0b9.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 24-Mar-20 17:04 aos_prov-4.5.0b9.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       15 b- defN 24-Mar-20 17:04 aos_prov-4.5.0b9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6352 b- defN 24-Mar-20 17:04 aos_prov-4.5.0b9.dist-info/RECORD
-66 files, 355657 bytes uncompressed, 61031 bytes compressed:  82.8%
+Zip file size: 94293 bytes, number of entries: 79
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/__init__.py
+-rw-rw-rw-  2.0 fat     3301 b- defN 24-Apr-03 14:52 aos_prov/actions.py
+-rw-rw-rw-  2.0 fat     9864 b- defN 24-Apr-04 12:00 aos_prov/main.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/commands/__init__.py
+-rw-rw-rw-  2.0 fat     7181 b- defN 24-Feb-20 14:19 aos_prov/commands/command_provision.py
+-rw-rw-rw-  2.0 fat     5021 b- defN 23-Jan-19 15:42 aos_prov/commands/command_vm.py
+-rw-rw-rw-  2.0 fat     2406 b- defN 22-Dec-15 18:20 aos_prov/commands/command_vm_libvirt.py
+-rw-rw-rw-  2.0 fat     5627 b- defN 23-Feb-01 10:29 aos_prov/commands/command_vm_multi_node.py
+-rw-rw-rw-  2.0 fat    18100 b- defN 24-Apr-03 14:52 aos_prov/commands/command_vm_multi_node_manage.py
+-rw-rw-rw-  2.0 fat     2371 b- defN 24-Jan-24 11:32 aos_prov/commands/download.py
+-rw-rw-rw-  2.0 fat     1721 b- defN 23-Jan-23 12:22 aos_prov/commands/vbox_sdk.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/__init__.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/cloud/__init__.py
+-rw-rw-rw-  2.0 fat     8075 b- defN 24-Apr-03 14:52 aos_prov/communication/cloud/cloud_api.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Feb-07 18:56 aos_prov/communication/unit/__init__.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/__init__.py
+-rw-rw-rw-  2.0 fat     5403 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/unit_communacation.py
+-rw-rw-rw-  2.0 fat     5346 b- defN 23-Mar-13 10:35 aos_prov/communication/unit/v0/unit_communication.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/generated/__init__.py
+-rw-rw-rw-  2.0 fat    29503 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2.py
+-rw-rw-rw-  2.0 fat    20612 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2_grpc.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/__init__.py
+-rw-rw-rw-  2.0 fat     6942 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/unit_communacation_v1.py
+-rw-rw-rw-  2.0 fat     6528 b- defN 23-Mar-13 10:35 aos_prov/communication/unit/v1/unit_communication_v1.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/__init__.py
+-rw-rw-rw-  2.0 fat     5568 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagercommon_pb2.py
+-rw-rw-rw-  2.0 fat      163 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagercommon_pb2_grpc.py
+-rw-rw-rw-  2.0 fat    31801 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2.py
+-rw-rw-rw-  2.0 fat    20208 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2_grpc.py
+-rw-rw-rw-  2.0 fat     9306 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2.py
+-rw-rw-rw-  2.0 fat     8101 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2_grpc.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/__init__.py
+-rw-rw-rw-  2.0 fat     7346 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/unit_communacation_v2.py
+-rw-rw-rw-  2.0 fat     7139 b- defN 24-Feb-20 14:19 aos_prov/communication/unit/v2/unit_communication_v2.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Dec-27 18:37 aos_prov/communication/unit/v2/generated/__init__.py
+-rw-rw-rw-  2.0 fat     5570 b- defN 24-Jan-24 11:32 aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py
+-rw-rw-rw-  2.0 fat      163 b- defN 23-Dec-27 18:37 aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py
+-rw-rw-rw-  2.0 fat    25112 b- defN 24-Jan-24 11:32 aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py
+-rw-rw-rw-  2.0 fat    16806 b- defN 24-Jan-24 11:32 aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py
+-rw-rw-rw-  2.0 fat    17726 b- defN 24-Jan-24 11:32 aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py
+-rw-rw-rw-  2.0 fat    13190 b- defN 24-Jan-24 11:32 aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Dec-02 13:22 aos_prov/communication/unit/v4/__init__.py
+-rw-rw-rw-  2.0 fat     8897 b- defN 24-Feb-20 14:19 aos_prov/communication/unit/v4/unit_communication_v4.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Dec-02 13:22 aos_prov/communication/unit/v4/generated/__init__.py
+-rw-rw-rw-  2.0 fat    18732 b- defN 24-Jan-24 11:32 aos_prov/communication/unit/v4/generated/iamanager_pb2.py
+-rw-rw-rw-  2.0 fat    34149 b- defN 24-Jan-24 11:32 aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py
+-rw-rw-rw-  2.0 fat     2750 b- defN 22-Feb-07 18:56 aos_prov/files/1rootCA.crt
+-rw-rw-rw-  2.0 fat     2767 b- defN 22-Oct-13 13:59 aos_prov/files/vm.xml
+-rw-rw-rw-  2.0 fat      771 b- defN 22-Oct-13 13:59 aos_prov/utils/__init__.py
+-rw-rw-rw-  2.0 fat     1702 b- defN 24-May-29 10:10 aos_prov/utils/common.py
+-rw-rw-rw-  2.0 fat     2234 b- defN 24-Jan-24 11:32 aos_prov/utils/config.py
+-rw-rw-rw-  2.0 fat      681 b- defN 24-Jan-24 11:32 aos_prov/utils/errors.py
+-rw-rw-rw-  2.0 fat     1020 b- defN 24-Jan-24 11:32 aos_prov/utils/unit_certificate.py
+-rw-rw-rw-  2.0 fat     6176 b- defN 24-Apr-30 06:25 aos_prov/utils/user_credentials.py
+-rw-rw-rw-  2.0 fat     2096 b- defN 24-Apr-30 06:25 aos_prov/utils/pem/__init__.py
+-rw-rw-rw-  2.0 fat     1839 b- defN 24-Apr-30 06:25 aos_prov/utils/pem/_core.py
+-rw-rw-rw-  2.0 fat     6807 b- defN 24-Apr-30 06:25 aos_prov/utils/pem/_object_types.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-13 13:59 test/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-13 13:59 test/utils/__init__.py
+-rw-rw-rw-  2.0 fat      665 b- defN 22-Dec-02 13:22 test/utils/test_config.py
+-rw-rw-rw-  2.0 fat      656 b- defN 22-Dec-02 13:22 test/utils/test_unit_certificate.py
+-rw-rw-rw-  2.0 fat      456 b- defN 22-Oct-13 13:59 test/utils/test_user_credentials.py
+-rw-rw-rw-  2.0 fat       93 b- defN 24-Jan-24 11:32 tests/__init__.py
+-rw-rw-rw-  2.0 fat     4520 b- defN 24-Jan-24 11:32 tests/fixtures.py
+-rw-rw-rw-  2.0 fat     3355 b- defN 24-Jan-24 11:32 tests/test_actions.py
+-rw-rw-rw-  2.0 fat       93 b- defN 24-Jan-24 11:32 tests/commands/__init__.py
+-rw-rw-rw-  2.0 fat    17979 b- defN 24-Feb-20 14:19 tests/commands/test_command_provision.py
+-rw-rw-rw-  2.0 fat    14118 b- defN 24-Jan-24 11:32 tests/commands/test_command_vm_multi_node_manage.py
+-rw-rw-rw-  2.0 fat     3666 b- defN 24-Jan-24 11:32 tests/commands/test_download.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Jan-24 11:32 tests/utils/__init__.py
+-rw-rw-rw-  2.0 fat     1867 b- defN 24-Jan-24 11:32 tests/utils/test_common.py
+-rw-rw-rw-  2.0 fat     1159 b- defN 24-Jan-24 11:32 tests/utils/test_config.py
+-rw-rw-rw-  2.0 fat      749 b- defN 24-Jan-24 11:32 tests/utils/test_unit_certificate.py
+-rw-rw-rw-  2.0 fat     3797 b- defN 24-Apr-03 14:52 tests/utils/test_user_credentials.py
+-rw-rw-rw-  2.0 fat     2538 b- defN 24-May-29 10:11 aos_prov-4.6.0b1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-29 10:11 aos_prov-4.6.0b1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       49 b- defN 24-May-29 10:11 aos_prov-4.6.0b1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       15 b- defN 24-May-29 10:11 aos_prov-4.6.0b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     7690 b- defN 24-May-29 10:11 aos_prov-4.6.0b1.dist-info/RECORD
+79 files, 461215 bytes uncompressed, 81697 bytes compressed:  82.3%
```

## zipnote {}

```diff
@@ -12,20 +12,29 @@
 
 Filename: aos_prov/commands/command_provision.py
 Comment: 
 
 Filename: aos_prov/commands/command_vm.py
 Comment: 
 
+Filename: aos_prov/commands/command_vm_libvirt.py
+Comment: 
+
+Filename: aos_prov/commands/command_vm_multi_node.py
+Comment: 
+
 Filename: aos_prov/commands/command_vm_multi_node_manage.py
 Comment: 
 
 Filename: aos_prov/commands/download.py
 Comment: 
 
+Filename: aos_prov/commands/vbox_sdk.py
+Comment: 
+
 Filename: aos_prov/communication/__init__.py
 Comment: 
 
 Filename: aos_prov/communication/cloud/__init__.py
 Comment: 
 
 Filename: aos_prov/communication/cloud/cloud_api.py
@@ -33,69 +42,87 @@
 
 Filename: aos_prov/communication/unit/__init__.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v0/__init__.py
 Comment: 
 
+Filename: aos_prov/communication/unit/v0/unit_communacation.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v0/unit_communication.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v0/generated/__init__.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2_grpc.py
+Comment: 
+
 Filename: aos_prov/communication/unit/v1/__init__.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v2/__init__.py
+Filename: aos_prov/communication/unit/v1/unit_communacation_v1.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v2/unit_communication_v2.py
+Filename: aos_prov/communication/unit/v1/unit_communication_v1.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v2/generated/__init__.py
+Filename: aos_prov/communication/unit/v1/generated/__init__.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py
+Filename: aos_prov/communication/unit/v1/generated/iamanagercommon_pb2.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py
+Filename: aos_prov/communication/unit/v1/generated/iamanagercommon_pb2_grpc.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py
+Filename: aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py
+Filename: aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2_grpc.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py
+Filename: aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py
+Filename: aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2_grpc.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v3/__init__.py
+Filename: aos_prov/communication/unit/v2/__init__.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v3/unit_communication_v3.py
+Filename: aos_prov/communication/unit/v2/unit_communacation_v2.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v3/generated/__init__.py
+Filename: aos_prov/communication/unit/v2/unit_communication_v2.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v3/generated/iamanagercommon_pb2.py
+Filename: aos_prov/communication/unit/v2/generated/__init__.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v3/generated/iamanagercommon_pb2_grpc.py
+Filename: aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v3/generated/iamanagerprotected_pb2.py
+Filename: aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v3/generated/iamanagerprotected_pb2_grpc.py
+Filename: aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v3/generated/iamanagerpublic_pb2.py
+Filename: aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v3/generated/iamanagerpublic_pb2_grpc.py
+Filename: aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v4/__init__.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v4/unit_communication_v4.py
 Comment: 
@@ -108,14 +135,17 @@
 
 Filename: aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py
 Comment: 
 
 Filename: aos_prov/files/1rootCA.crt
 Comment: 
 
+Filename: aos_prov/files/vm.xml
+Comment: 
+
 Filename: aos_prov/utils/__init__.py
 Comment: 
 
 Filename: aos_prov/utils/common.py
 Comment: 
 
 Filename: aos_prov/utils/config.py
@@ -126,14 +156,23 @@
 
 Filename: aos_prov/utils/unit_certificate.py
 Comment: 
 
 Filename: aos_prov/utils/user_credentials.py
 Comment: 
 
+Filename: aos_prov/utils/pem/__init__.py
+Comment: 
+
+Filename: aos_prov/utils/pem/_core.py
+Comment: 
+
+Filename: aos_prov/utils/pem/_object_types.py
+Comment: 
+
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/utils/__init__.py
 Comment: 
 
 Filename: test/utils/test_config.py
@@ -177,23 +216,23 @@
 
 Filename: tests/utils/test_unit_certificate.py
 Comment: 
 
 Filename: tests/utils/test_user_credentials.py
 Comment: 
 
-Filename: aos_prov-4.5.0b9.dist-info/METADATA
+Filename: aos_prov-4.6.0b1.dist-info/METADATA
 Comment: 
 
-Filename: aos_prov-4.5.0b9.dist-info/WHEEL
+Filename: aos_prov-4.6.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: aos_prov-4.5.0b9.dist-info/entry_points.txt
+Filename: aos_prov-4.6.0b1.dist-info/entry_points.txt
 Comment: 
 
-Filename: aos_prov-4.5.0b9.dist-info/top_level.txt
+Filename: aos_prov-4.6.0b1.dist-info/top_level.txt
 Comment: 
 
-Filename: aos_prov-4.5.0b9.dist-info/RECORD
+Filename: aos_prov-4.6.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aos_prov/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
```

## aos_prov/actions.py

 * *Ordering differences only*

```diff
@@ -1,98 +1,98 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-"""aos-prov supported actions module."""
-import time
-
-from aos_prov.commands.command_provision import run_provision
-from aos_prov.commands.command_vm_multi_node_manage import (
-    new_vms,
-    remove_vms_in_group,
-    start_vms,
-)
-from aos_prov.commands.download import download_and_save_multinode
-from aos_prov.communication.cloud.cloud_api import CloudAPI
-from aos_prov.utils.common import DOWNLOADS_PATH, RECONNECT_TIMEOUT, print_message
-from aos_prov.utils.user_credentials import UserCredentials
-
-
-def provision_unit(unit_address: str, cloud_api: CloudAPI, reconnect_times: int = 1) -> None:
-    """
-    Rub provisioning process for the unit.
-
-    Args:
-        unit_address (str): address:port of the unit.
-        cloud_api (CloudAPI): instance of CloudAPI with user info.
-        reconnect_times (int): Number of connections retries.
-    """
-    run_provision(unit_address, cloud_api, reconnect_times)
-
-
-def create_new_unit(
-    vm_name: str,
-    user_creds: UserCredentials,
-    disk_location: str,
-    do_provision=False,
-    nodes_count=2,
-    headless=False,
-) -> []:
-    """
-    Create a new VirtualBox multi-node Unit.
-
-    Args:
-        vm_name (str): Name of the group of units.
-        user_creds (UserCredentials): UserCredentials instance.
-        disk_location (str): Full path to the folder with nodes images.
-        do_provision (Boolean): Provision unit after creation or not.
-        nodes_count (int): Count of nodes to create. Supported 1 or 2 nodes.
-        headless (bool): Start VM in headless mode if True
-
-    Returns:
-        [provisioning_port, node0_ssh_port, node1_ssh_port]: Forwarded ports.
-    """
-    cloud_api = CloudAPI(user_creds)
-
-    if do_provision:
-        cloud_api.check_cloud_access()
-
-    provisioning_port, node0_ssh_port, node1_ssh_port = new_vms(vm_name, disk_location, nodes_count)
-
-    if do_provision:
-        start_vms(f'/AosUnits/{vm_name}', headless=headless)
-        time.sleep(10)
-        run_provision(f'127.0.0.1:{provisioning_port}', cloud_api, reconnect_times=RECONNECT_TIMEOUT)
-
-    return [provisioning_port, node0_ssh_port, node1_ssh_port]
-
-
-def remove_vm_unit(name: str) -> None:
-    """Remove all VMs in the group.
-
-    Args:
-        name (str): Name of the group for removing without root AosUnits group.
-    """
-    remove_vms_in_group(name)
-
-
-def start_vm_unit(name: str, headless=False) -> None:
-    """Start all VMs in the group.
-
-    Args:
-        name (str): Name of the group to start without root AosUnits group.
-        headless (bool): Start VM in headless mode if True.
-    """
-    start_vms(f'/AosUnits/{name}', check_virtualbox=True, headless=headless)
-
-
-def download_image(download_url: str, force: bool = False) -> None:
-    """
-    Download unit image.
-
-    Args:
-        download_url (str): URL to download from.
-        force (bool): If set downloaded image will overwrite existing one.
-    """
-    download_and_save_multinode(download_url, DOWNLOADS_PATH, force)
-    resolve_download_path = str(DOWNLOADS_PATH.resolve())
-    print_message(f'Download finished. You may find Unit images in: [b]{resolve_download_path}[/b]')
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+"""aos-prov supported actions module."""
+import time
+
+from aos_prov.commands.command_provision import run_provision
+from aos_prov.commands.command_vm_multi_node_manage import (
+    new_vms,
+    remove_vms_in_group,
+    start_vms,
+)
+from aos_prov.commands.download import download_and_save_multinode
+from aos_prov.communication.cloud.cloud_api import CloudAPI
+from aos_prov.utils.common import DOWNLOADS_PATH, RECONNECT_TIMEOUT, print_message
+from aos_prov.utils.user_credentials import UserCredentials
+
+
+def provision_unit(unit_address: str, cloud_api: CloudAPI, reconnect_times: int = 1) -> None:
+    """
+    Rub provisioning process for the unit.
+
+    Args:
+        unit_address (str): address:port of the unit.
+        cloud_api (CloudAPI): instance of CloudAPI with user info.
+        reconnect_times (int): Number of connections retries.
+    """
+    run_provision(unit_address, cloud_api, reconnect_times)
+
+
+def create_new_unit(
+    vm_name: str,
+    user_creds: UserCredentials,
+    disk_location: str,
+    do_provision=False,
+    nodes_count=2,
+    headless=False,
+) -> []:
+    """
+    Create a new VirtualBox multi-node Unit.
+
+    Args:
+        vm_name (str): Name of the group of units.
+        user_creds (UserCredentials): UserCredentials instance.
+        disk_location (str): Full path to the folder with nodes images.
+        do_provision (Boolean): Provision unit after creation or not.
+        nodes_count (int): Count of nodes to create. Supported 1 or 2 nodes.
+        headless (bool): Start VM in headless mode if True
+
+    Returns:
+        [provisioning_port, node0_ssh_port, node1_ssh_port]: Forwarded ports.
+    """
+    cloud_api = CloudAPI(user_creds)
+
+    if do_provision:
+        cloud_api.check_cloud_access()
+
+    provisioning_port, node0_ssh_port, node1_ssh_port = new_vms(vm_name, disk_location, nodes_count)
+
+    if do_provision:
+        start_vms(f'/AosUnits/{vm_name}', headless=headless)
+        time.sleep(10)
+        run_provision(f'127.0.0.1:{provisioning_port}', cloud_api, reconnect_times=RECONNECT_TIMEOUT)
+
+    return [provisioning_port, node0_ssh_port, node1_ssh_port]
+
+
+def remove_vm_unit(name: str) -> None:
+    """Remove all VMs in the group.
+
+    Args:
+        name (str): Name of the group for removing without root AosUnits group.
+    """
+    remove_vms_in_group(name)
+
+
+def start_vm_unit(name: str, headless=False) -> None:
+    """Start all VMs in the group.
+
+    Args:
+        name (str): Name of the group to start without root AosUnits group.
+        headless (bool): Start VM in headless mode if True.
+    """
+    start_vms(f'/AosUnits/{name}', check_virtualbox=True, headless=headless)
+
+
+def download_image(download_url: str, force: bool = False) -> None:
+    """
+    Download unit image.
+
+    Args:
+        download_url (str): URL to download from.
+        force (bool): If set downloaded image will overwrite existing one.
+    """
+    download_and_save_multinode(download_url, DOWNLOADS_PATH, force)
+    resolve_download_path = str(DOWNLOADS_PATH.resolve())
+    print_message(f'Download finished. You may find Unit images in: [b]{resolve_download_path}[/b]')
```

## aos_prov/main.py

```diff
@@ -1,304 +1,321 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-# pylint: disable=too-many-statements
-import argparse
-import logging
-import os
-import sys
-from pathlib import Path
-
-from aos_prov.actions import (
-    create_new_unit,
-    download_image,
-    provision_unit,
-    remove_vm_unit,
-    start_vm_unit,
-)
-from aos_prov.communication.cloud.cloud_api import DEFAULT_REGISTER_PORT, CloudAPI
-from aos_prov.utils import DEFAULT_USER_CERT_PATH, DEFAULT_USER_KEY_PATH
-from aos_prov.utils.common import AOS_DISKS_PATH, DISK_IMAGE_DOWNLOAD_URL, print_error
-from aos_prov.utils.errors import (
-    CloudAccessError,
-    DeviceRegisterError,
-    OnUnitError,
-    UnitError,
-)
-from aos_prov.utils.user_credentials import UserCredentials
-
-try:
-    from importlib.metadata import version  # noqa: WPS433
-except ImportError:
-    import importlib_metadata as version  # noqa: WPS433,WPS432,WPS440
-
-_ARGUMENT_USER_CERTIFICATE = '--cert'
-_ARGUMENT_USER_KEY = '--key'
-_ARGUMENT_USER_PKCS12 = '--pkcs12'
-
-_COMMAND_NEW_VM = 'vm-new'
-_COMMAND_REMOVE_VM = 'vm-remove'
-_COMMAND_START_VM = 'vm-start'
-_COMMAND_UNIT_CREATE = 'unit-new'
-_COMMAND_DOWNLOAD = 'download'
-
-_DEFAULT_USER_CERTIFICATE = str(Path.home() / '.aos' / 'security' / 'aos-user-oem.p12')
-
-_MAX_PORT = 65535
-
-logger = logging.getLogger(__name__)
-
-
-def _is_path_traversal(path):
-    if not path:
-        return False
-    return not os.path.commonprefix([path, Path.home()])
-
-
-def _parse_args():  # noqa: WPS213
-    parser = argparse.ArgumentParser(
-        prog='aos-prov',
-        description='The unit provisioning tool using gRPC protocol',
-        epilog="Run 'aos-prov [COMMAND] --help' for more information about commands",
-    )
-
-    parser.add_argument(
-        '-u',
-        '--unit',
-        required=False,
-        help='Unit address in format IP_ADDRESS or IP_ADDRESS:PORT',
-    )
-
-    parser.add_argument(
-        _ARGUMENT_USER_CERTIFICATE,
-        default=DEFAULT_USER_CERT_PATH,
-        help=f'User certificate file. Default: {DEFAULT_USER_CERT_PATH}',
-    )
-
-    parser.add_argument(
-        _ARGUMENT_USER_KEY,
-        default=DEFAULT_USER_KEY_PATH,
-        help=f'User key file. Default: {DEFAULT_USER_KEY_PATH}',
-    )
-
-    parser.add_argument(
-        '-p',
-        _ARGUMENT_USER_PKCS12,
-        required=False,
-        help='Path to user certificate in pkcs12 format.',
-        dest='pkcs',
-        default=_DEFAULT_USER_CERTIFICATE,
-    )
-
-    parser.add_argument(
-        '--register-port',
-        default=DEFAULT_REGISTER_PORT,
-        help=f'Cloud port. Default: {DEFAULT_REGISTER_PORT}',
-        type=int,
-    )
-
-    parser.add_argument(
-        '-w',
-        '--wait-unit',
-        action='store',
-        metavar='N',
-        help='Wait for unit to respond for the first time in seconds. Default value 0 means wait for 5 seconds',
-        dest='wait_unit',
-        default=0,
-        type=int,
-    )
-
-    parser.set_defaults(which=None)
-
-    sub_parser = parser.add_subparsers(title='Commands')
-
-    new_vm_command = sub_parser.add_parser(
-        _COMMAND_NEW_VM,
-        help='Create new Oracle VM',
-    )
-    new_vm_command.set_defaults(which=_COMMAND_NEW_VM)
-
-    new_vm_command.add_argument(
-        '-N',
-        '--name',
-        required=True,
-        help='Name of the VM',
-    )
-
-    new_vm_command.add_argument(
-        '-D',
-        '--disk',
-        required=False,
-        help='Full path to the AosCore-powered disk.',
-        default=AOS_DISKS_PATH,
-    )
-
-    remove_vm_command = sub_parser.add_parser(
-        _COMMAND_REMOVE_VM,
-        help='Remove Oracle VM',
-    )
-    remove_vm_command.set_defaults(which=_COMMAND_REMOVE_VM)
-
-    remove_vm_command.add_argument(
-        '-N',
-        '--name',
-        required=True,
-        help='Name of the VM',
-    )
-
-    start_vm_command = sub_parser.add_parser(
-        _COMMAND_START_VM,
-        help='Start the VM',
-    )
-    start_vm_command.add_argument(
-        '-N',
-        '--name',
-        required=True,
-        help='Name of the VirtualBox group where VMs are located.',
-    )
-
-    start_vm_command.add_argument(
-        '-H',
-        '--headless',
-        action='store_true',
-        help='Start VMs in headless mode.',
-    )
-    start_vm_command.set_defaults(which=_COMMAND_START_VM)
-
-    create_unit_command = sub_parser.add_parser(
-        _COMMAND_UNIT_CREATE,
-        help='Create and provision new VirtualBox-based unit',
-    )
-    create_unit_command.set_defaults(which=_COMMAND_UNIT_CREATE)
-
-    create_unit_command.add_argument(
-        '--name',
-        required=True,
-        help='Name of the VM',
-    )
-
-    create_unit_command.add_argument(
-        '--disk',
-        required=False,
-        help='Full path to the AosCore-powered disk.',
-        default=AOS_DISKS_PATH,
-    )
-
-    create_unit_command.add_argument(
-        '-H',
-        '--headless',
-        action='store_true',
-        help='Start created VMs in headless mode.',
-    )
-
-    create_unit_command.add_argument(
-        '-p',
-        _ARGUMENT_USER_PKCS12,
-        required=False,
-        help='Path to user certificate in pkcs12 format',
-        dest='pkcs',
-        default=_DEFAULT_USER_CERTIFICATE,
-    )
-
-    parser.add_argument(
-        '-V',
-        '--version',
-        action='version',
-        version=f'%(prog)s {version("aos-prov")}',  # noqa: WPS323,WPS237
-    )
-
-    download_command = sub_parser.add_parser(_COMMAND_DOWNLOAD, help='Download image')
-    download_command.set_defaults(which=_COMMAND_DOWNLOAD)
-    download_command.add_argument(
-        '-a',
-        '--address',
-        dest='download_address',
-        help='Address to download image',
-    )
-
-    download_command.add_argument(
-        '-f',
-        '--force',
-        action='store_true',
-        help='Force overwrite existing file',
-    )
-
-    return parser.parse_args()
-
-
-def _parse_user_creds(args) -> UserCredentials:
-    is_default_pkcs = args.pkcs == _DEFAULT_USER_CERTIFICATE
-    if is_default_pkcs and (args.cert != DEFAULT_USER_CERT_PATH or args.key != DEFAULT_USER_KEY_PATH):
-        args.pkcs = None
-    if _is_path_traversal(args.cert):
-        raise CloudAccessError('Path to certificate is not safe! Use absolute path')
-    cert = args.cert
-    if _is_path_traversal(args.key):
-        raise CloudAccessError('Path to key is not safe! Use absolute path')
-    key = args.key
-    if _is_path_traversal(args.pkcs):
-        raise CloudAccessError('Path to pkcs certificate is not safe! Use absolute path')
-    pkcs = args.pkcs
-    return UserCredentials(cert_file_path=cert, key_file_path=key, pkcs12=pkcs)
-
-
-def main():
-    status = 0
-    args = _parse_args()
-
-    try:  # noqa: WPS225
-        if args.which is None:
-            user_creds = _parse_user_creds(args)
-            register_port = args.register_port
-            if register_port < 1 or register_port > _MAX_PORT:
-                raise CloudAccessError(f'Port is not valid: {register_port}. Should be in range 1..{_MAX_PORT}')
-            cloud_api = CloudAPI(user_creds, register_port)
-            cloud_api.check_cloud_access()
-            wait = args.wait_unit // 5 or 1
-            provision_unit(args.unit, cloud_api, wait)
-
-        if args.which == _COMMAND_DOWNLOAD:
-            url = DISK_IMAGE_DOWNLOAD_URL
-            if args.download_address:
-                url = args.download_address
-            download_image(url, args.force)
-
-        if args.which == _COMMAND_NEW_VM:
-            user_creds = _parse_user_creds(args)
-            if _is_path_traversal(args.disk):
-                raise UnitError('Path to VM disk is not safe! Use absolute path')
-            disk = args.disk
-            create_new_unit(args.name, user_creds, disk)
-
-        if args.which == _COMMAND_REMOVE_VM:
-            remove_vm_unit(args.name)
-
-        if args.which == _COMMAND_START_VM:
-            start_vm_unit(args.name, args.headless)
-
-        if args.which == _COMMAND_UNIT_CREATE:
-            user_creds = _parse_user_creds(args)
-            create_new_unit(args.name, user_creds, args.disk, do_provision=True, headless=args.headless)
-
-    except CloudAccessError as exc:
-        print_error(f'Failed during communication with the AosCloud with error: {exc}')
-        status = 1
-    except DeviceRegisterError as exc:
-        print_error(f'FAILED with error: {exc}')
-        status = 1
-    except UnitError as exc:
-        print_error(f'Failed during communication with device with error: \n {exc}')
-        status = 1
-    except OnUnitError as exc:
-        print_error('Failed to execute the command!')
-        print_error(f'Error: {exc} ')
-        status = 1
-    except (AssertionError, KeyboardInterrupt):
-        print_error('Stopped by keyboard...')
-        status = 1
-
-    sys.exit(status)
-
-
-if __name__ == '__main__':
-    main()
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+# pylint: disable=too-many-statements
+import argparse
+import logging
+import os
+import sys
+import typing
+from pathlib import Path
+
+from aos_prov.actions import (
+    create_new_unit,
+    download_image,
+    provision_unit,
+    remove_vm_unit,
+    start_vm_unit,
+)
+from aos_prov.communication.cloud.cloud_api import DEFAULT_REGISTER_PORT, CloudAPI
+from aos_prov.utils import DEFAULT_USER_CERT_PATH, DEFAULT_USER_KEY_PATH
+from aos_prov.utils.common import AOS_DISKS_PATH, DISK_IMAGE_DOWNLOAD_URL, print_error
+from aos_prov.utils.errors import (
+    CloudAccessError,
+    DeviceRegisterError,
+    OnUnitError,
+    UnitError,
+)
+from aos_prov.utils.user_credentials import UserCredentials
+
+try:
+    from importlib.metadata import version  # noqa: WPS433
+except ImportError:
+    import importlib_metadata as version  # noqa: WPS433,WPS432,WPS440
+
+_ARGUMENT_USER_CERTIFICATE = '--cert'
+_ARGUMENT_USER_KEY = '--key'
+_ARGUMENT_USER_PKCS12 = '--pkcs12'
+
+_COMMAND_NEW_VM = 'vm-new'
+_COMMAND_REMOVE_VM = 'vm-remove'
+_COMMAND_START_VM = 'vm-start'
+_COMMAND_UNIT_CREATE = 'unit-new'
+_COMMAND_DOWNLOAD = 'download'
+
+_DEFAULT_USER_CERTIFICATE = str(Path.home() / '.aos' / 'security' / 'aos-user-oem.p12')
+
+_MAX_PORT = 65535
+
+logger = logging.getLogger(__name__)
+
+
+def sanitize_path_to_file(path: typing.Union[str, None]) -> typing.Union[str, None]:
+    if path is None:
+        return None
+    # According to the requirement, aos-prov should allow any real path to be used
+    absolute_path = os.path.abspath(path)
+    if not os.path.isfile(absolute_path):
+        raise CloudAccessError(f'Path: {path} is not a file or does not exist.')
+    return absolute_path
+
+
+def sanitize_path_to_dir(path: typing.Union[str, None]) -> typing.Union[str, None]:
+    if path is None:
+        return None
+    # According to the requirement, aos-prov should allow any real path to be used
+    absolute_path = os.path.abspath(path)
+    if not os.path.isdir(absolute_path):
+        raise CloudAccessError(f'Path: {path} is not a directory or does not exist.')
+    return absolute_path
+
+
+def sanitize_port(port: typing.Union[int, None]) -> typing.Union[int, None]:
+    if not isinstance(port, int) or port < 1 or port > _MAX_PORT:
+        raise CloudAccessError(f'Port is not valid: {port}. Should be in range 1..{_MAX_PORT}')
+    return port
+
+
+def _parse_args():  # noqa: WPS213
+    parser = argparse.ArgumentParser(
+        prog='aos-prov',
+        description='The unit provisioning tool using gRPC protocol',
+        epilog="Run 'aos-prov [COMMAND] --help' for more information about commands",
+    )
+
+    parser.add_argument(
+        '-u',
+        '--unit',
+        required=False,
+        help='Unit address in format IP_ADDRESS or IP_ADDRESS:PORT',
+    )
+
+    parser.add_argument(
+        _ARGUMENT_USER_CERTIFICATE,
+        default=DEFAULT_USER_CERT_PATH,
+        help=f'User certificate file. Default: {DEFAULT_USER_CERT_PATH}',
+    )
+
+    parser.add_argument(
+        _ARGUMENT_USER_KEY,
+        default=DEFAULT_USER_KEY_PATH,
+        help=f'User key file. Default: {DEFAULT_USER_KEY_PATH}',
+    )
+
+    parser.add_argument(
+        '-p',
+        _ARGUMENT_USER_PKCS12,
+        required=False,
+        help='Path to user certificate in pkcs12 format.',
+        dest='pkcs',
+        default=_DEFAULT_USER_CERTIFICATE,
+    )
+
+    parser.add_argument(
+        '--register-port',
+        default=DEFAULT_REGISTER_PORT,
+        help=f'Cloud port. Default: {DEFAULT_REGISTER_PORT}',
+        type=int,
+    )
+
+    parser.add_argument(
+        '-w',
+        '--wait-unit',
+        action='store',
+        metavar='N',
+        help='Wait for unit to respond for the first time in seconds. Default value 0 means wait for 5 seconds',
+        dest='wait_unit',
+        default=0,
+        type=int,
+    )
+
+    parser.set_defaults(which=None)
+
+    sub_parser = parser.add_subparsers(title='Commands')
+
+    new_vm_command = sub_parser.add_parser(
+        _COMMAND_NEW_VM,
+        help='Create new Oracle VM',
+    )
+    new_vm_command.set_defaults(which=_COMMAND_NEW_VM)
+
+    new_vm_command.add_argument(
+        '-N',
+        '--name',
+        required=True,
+        help='Name of the VM',
+    )
+
+    new_vm_command.add_argument(
+        '-D',
+        '--disk',
+        required=False,
+        help='Full path to the AosCore-powered disk.',
+        default=AOS_DISKS_PATH,
+    )
+
+    remove_vm_command = sub_parser.add_parser(
+        _COMMAND_REMOVE_VM,
+        help='Remove Oracle VM',
+    )
+    remove_vm_command.set_defaults(which=_COMMAND_REMOVE_VM)
+
+    remove_vm_command.add_argument(
+        '-N',
+        '--name',
+        required=True,
+        help='Name of the VM',
+    )
+
+    start_vm_command = sub_parser.add_parser(
+        _COMMAND_START_VM,
+        help='Start the VM',
+    )
+    start_vm_command.add_argument(
+        '-N',
+        '--name',
+        required=True,
+        help='Name of the VirtualBox group where VMs are located.',
+    )
+
+    start_vm_command.add_argument(
+        '-H',
+        '--headless',
+        action='store_true',
+        help='Start VMs in headless mode.',
+    )
+    start_vm_command.set_defaults(which=_COMMAND_START_VM)
+
+    create_unit_command = sub_parser.add_parser(
+        _COMMAND_UNIT_CREATE,
+        help='Create and provision new VirtualBox-based unit',
+    )
+    create_unit_command.set_defaults(which=_COMMAND_UNIT_CREATE)
+
+    create_unit_command.add_argument(
+        '--name',
+        required=True,
+        help='Name of the VM',
+    )
+
+    create_unit_command.add_argument(
+        '--disk',
+        required=False,
+        help='Full path to the AosCore-powered disk.',
+        default=AOS_DISKS_PATH,
+    )
+
+    create_unit_command.add_argument(
+        '-H',
+        '--headless',
+        action='store_true',
+        help='Start created VMs in headless mode.',
+    )
+
+    create_unit_command.add_argument(
+        '-p',
+        _ARGUMENT_USER_PKCS12,
+        required=False,
+        help='Path to user certificate in pkcs12 format',
+        dest='pkcs',
+        default=_DEFAULT_USER_CERTIFICATE,
+    )
+
+    parser.add_argument(
+        '-V',
+        '--version',
+        action='version',
+        version=f'%(prog)s {version("aos-prov")}',  # noqa: WPS323,WPS237
+    )
+
+    download_command = sub_parser.add_parser(_COMMAND_DOWNLOAD, help='Download image')
+    download_command.set_defaults(which=_COMMAND_DOWNLOAD)
+    download_command.add_argument(
+        '-a',
+        '--address',
+        dest='download_address',
+        help='Address to download image',
+    )
+
+    download_command.add_argument(
+        '-f',
+        '--force',
+        action='store_true',
+        help='Force overwrite existing file',
+    )
+
+    return parser.parse_args()
+
+
+def create_and_sanitize_user_creds(args) -> UserCredentials:
+    is_default_pkcs = args.pkcs == _DEFAULT_USER_CERTIFICATE
+    if not is_default_pkcs and (args.cert != DEFAULT_USER_CERT_PATH or args.key != DEFAULT_USER_KEY_PATH):
+        raise CloudAccessError('Only --pkcs12 or (--cert, --key) can be specified, but not both options.')
+    cert: typing.Union[str, None] = None
+    key: typing.Union[str, None] = None
+    pkcs: typing.Union[str, None] = None
+    if args.cert == DEFAULT_USER_CERT_PATH and args.key == DEFAULT_USER_KEY_PATH:
+        pkcs = sanitize_path_to_file(args.pkcs)
+    else:
+        cert = sanitize_path_to_file(args.cert)
+        key = sanitize_path_to_file(args.key)
+    return UserCredentials(cert_file_path=cert, key_file_path=key, pkcs12=pkcs)
+
+
+def main():
+    status = 0
+    args = _parse_args()
+
+    try:  # noqa: WPS225
+        if args.which is None:
+            user_creds = create_and_sanitize_user_creds(args)
+            register_port = sanitize_port(args.register_port)
+            cloud_api = CloudAPI(user_creds, register_port)
+            cloud_api.check_cloud_access()
+            wait = args.wait_unit // 5 or 1
+            provision_unit(args.unit, cloud_api, wait)
+
+        if args.which == _COMMAND_DOWNLOAD:
+            url = DISK_IMAGE_DOWNLOAD_URL
+            if args.download_address:
+                url = args.download_address
+            download_image(url, args.force)
+
+        if args.which == _COMMAND_NEW_VM:
+            user_creds = create_and_sanitize_user_creds(args)
+            disk = sanitize_path_to_dir(args.disk)
+            create_new_unit(args.name, user_creds, disk)
+
+        if args.which == _COMMAND_REMOVE_VM:
+            remove_vm_unit(args.name)
+
+        if args.which == _COMMAND_START_VM:
+            start_vm_unit(args.name, args.headless)
+
+        if args.which == _COMMAND_UNIT_CREATE:
+            user_creds = create_and_sanitize_user_creds(args)
+            disk = sanitize_path_to_dir(args.disk)
+            create_new_unit(args.name, user_creds, disk, do_provision=True, headless=args.headless)
+
+    except CloudAccessError as exc:
+        print_error(f'Failed during communication with the AosCloud with error: {exc}')
+        status = 1
+    except DeviceRegisterError as exc:
+        print_error(f'FAILED with error: {exc}')
+        status = 1
+    except UnitError as exc:
+        print_error(f'Failed during communication with device with error: \n {exc}')
+        status = 1
+    except OnUnitError as exc:
+        print_error('Failed to execute the command!')
+        print_error(f'Error: {exc} ')
+        status = 1
+    except (AssertionError, KeyboardInterrupt):
+        print_error('Stopped by keyboard...')
+        status = 1
+
+    sys.exit(status)
+
+
+if __name__ == '__main__':
+    main()
```

## aos_prov/commands/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
```

## aos_prov/commands/command_provision.py

 * *Ordering differences only*

```diff
@@ -1,163 +1,163 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-# pylint: disable=R0912,R0914,R0915,R1702
-"""Provision unit."""
-
-import time
-
-from aos_prov.communication.cloud.cloud_api import CloudAPI
-from aos_prov.communication.unit.v2.unit_communication_v2 import UnitCommunicationV2
-from aos_prov.communication.unit.v4.unit_communication_v4 import UnitCommunicationV4
-from aos_prov.utils.common import generate_random_password, print_message
-from aos_prov.utils.config import Config
-from aos_prov.utils.errors import GrpcUnimplemented, UnitError
-
-COMMAND_TO_DECRYPT = 'diskencryption'
-
-
-def run_provision(unit_address: str, cloud_api: CloudAPI, reconnect_times: int = 1):  # noqa: WPS210,WPS213
-    """
-    Provision Unit. This function will try to provision starting from the newest to the oldest.
-
-    Args:
-         unit_address (str): Address of the Unit
-         cloud_api (CloudAPI): URL to download
-         reconnect_times (int): URL to download
-
-    Raises:
-         GrpcUnimplemented: If provision fails.
-         UnitError: If provision fails.
-    """
-    config = Config()
-    unit_communication = UnitCommunicationV4(unit_address)
-    model_name = ''
-    for retry in range(reconnect_times):
-        try:
-            print_message('Starting provisioning...')
-            config.system_id, model_name = unit_communication.get_system_info()  # noqa: WPS414
-            config.protocol_version = unit_communication.get_protocol_version()
-            break
-        except GrpcUnimplemented:
-            try:  # noqa: WPS505
-                print_message('v4 is not supported. Starting provisioning using protocol v3')
-                unit_communication = UnitCommunicationV2(unit_address)
-                config.system_id, model_name = unit_communication.get_system_info()  # noqa: WPS414
-                config.protocol_version = unit_communication.get_protocol_version()
-                if config.protocol_version == 3:
-                    unit_communication.need_set_users = False
-                break
-            except GrpcUnimplemented as gu_exc:
-                print_message(f'[red]Grpc protocol error: {gu_exc}.')
-                raise gu_exc
-        except UnitError as unit_exc:
-            print_message('[yellow]Connection failed')
-            if retry + 1 < reconnect_times:
-                time.sleep(5)
-            else:
-                raise unit_exc
-
-    if config.system_id is None:
-        raise UnitError('Cannot read system_id')
-
-    config.set_model(model_name)
-    cloud_api.check_unit_is_not_provisioned(config.system_id)
-    if config.protocol_version >= 4:  # support of multi domains
-        config.node_ids = unit_communication.get_all_node_ids()
-        for node_id in config.node_ids:
-            config.supported_cert_types = unit_communication.get_cert_types(node_id)
-            need_disk_encryption = COMMAND_TO_DECRYPT in config.supported_cert_types
-
-            password = generate_random_password()
-
-            for clear_cert_type in config.supported_cert_types:
-                unit_communication.clear(clear_cert_type, node_id)
-
-            for set_cert_type in config.supported_cert_types:
-                unit_communication.set_cert_owner(set_cert_type, password, node_id)
-
-            if need_disk_encryption:
-                unit_communication.encrypt_disk(password, node_id)
-                config.supported_cert_types.remove(COMMAND_TO_DECRYPT)
-
-            for create_cert_type in config.supported_cert_types:
-                config.unit_certificates.append(unit_communication.create_keys(create_cert_type, password, node_id))
-    elif config.protocol_version == 3:
-        config.supported_cert_types = unit_communication.get_cert_types()
-        need_disk_encryption = COMMAND_TO_DECRYPT in config.supported_cert_types
-
-        password = generate_random_password()
-
-        for clear_cert_type in config.supported_cert_types:  # noqa: WPS440
-            unit_communication.clear(clear_cert_type)
-
-        for set_cert_type in config.supported_cert_types:  # noqa: WPS440
-            unit_communication.set_cert_owner(set_cert_type, password)
-
-        if need_disk_encryption:
-            unit_communication.encrypt_disk(password)
-            config.supported_cert_types.remove(COMMAND_TO_DECRYPT)
-            if config.protocol_version < 4:
-                unit_communication.wait_for_connection()
-
-        for create_cert_type in config.supported_cert_types:  # noqa: WPS440
-            config.unit_certificates.append(unit_communication.create_keys(create_cert_type, password))
-    else:
-        raise UnitError(f'aos-prov does not support {config.protocol_version} protocol of the Unit')
-
-    register_payload = {
-        'hardware_id': config.system_id,
-        'system_uid': config.system_id,
-        'model_name': config.model_name,
-        'model_version': config.model_version,
-        'provisioning_software': 'aos-provisioning:3.1',
-        'additional_csrs': [],
-    }
-
-    for csr_cert in config.unit_certificates:
-        if csr_cert.cert_type == 'online':
-            register_payload['online_public_csr'] = csr_cert.csr
-            if csr_cert.node_id:
-                register_payload['online_public_node_id'] = csr_cert.node_id
-        elif csr_cert.cert_type == 'offline':
-            register_payload['offline_public_csr'] = csr_cert.csr
-            if csr_cert.node_id:
-                register_payload['offline_public_node_id'] = csr_cert.node_id
-        else:
-            register_payload['additional_csrs'].append({
-                'cert_type': csr_cert.cert_type,
-                'csr': csr_cert.csr,
-                'node_id': csr_cert.node_id,
-            })
-
-    response = cloud_api.register_device(register_payload)
-    system_uid = response.get('system_uid')
-    additional_certs = response.get('additional_certs', [])
-    for cert in config.unit_certificates:
-        if cert.cert_type == 'online':
-            cert.certificate = response.get('online_certificate')
-        elif cert.cert_type == 'offline':
-            cert.certificate = response.get('offline_certificate')
-        else:
-            for additional_cert in additional_certs:
-                if additional_cert['cert_type'] == cert.cert_type:
-                    if additional_cert.get('node_id'):
-                        if additional_cert.get('node_id') == cert.node_id:
-                            cert.certificate = additional_cert['cert']
-                            break
-                    else:
-                        cert.certificate = additional_cert['cert']
-                        cert.node_id = additional_cert.get('node_id')
-                        break
-
-    for apply_cert in config.unit_certificates:
-        unit_communication.apply_certificate(apply_cert)
-
-    unit_communication.finish_provisioning()
-
-    print_message('[green]Finished successfully!')
-    link = cloud_api.get_unit_link_by_system_uid(system_uid)
-
-    if link:
-        print_message(f'You may find your unit on the cloud here: [green]{link}')
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+# pylint: disable=R0912,R0914,R0915,R1702
+"""Provision unit."""
+
+import time
+
+from aos_prov.communication.cloud.cloud_api import CloudAPI
+from aos_prov.communication.unit.v2.unit_communication_v2 import UnitCommunicationV2
+from aos_prov.communication.unit.v4.unit_communication_v4 import UnitCommunicationV4
+from aos_prov.utils.common import generate_random_password, print_message
+from aos_prov.utils.config import Config
+from aos_prov.utils.errors import GrpcUnimplemented, UnitError
+
+COMMAND_TO_DECRYPT = 'diskencryption'
+
+
+def run_provision(unit_address: str, cloud_api: CloudAPI, reconnect_times: int = 1):  # noqa: WPS210,WPS213
+    """
+    Provision Unit. This function will try to provision starting from the newest to the oldest.
+
+    Args:
+         unit_address (str): Address of the Unit
+         cloud_api (CloudAPI): URL to download
+         reconnect_times (int): URL to download
+
+    Raises:
+         GrpcUnimplemented: If provision fails.
+         UnitError: If provision fails.
+    """
+    config = Config()
+    unit_communication = UnitCommunicationV4(unit_address)
+    model_name = ''
+    for retry in range(reconnect_times):
+        try:
+            print_message('Starting provisioning...')
+            config.system_id, model_name = unit_communication.get_system_info()  # noqa: WPS414
+            config.protocol_version = unit_communication.get_protocol_version()
+            break
+        except GrpcUnimplemented:
+            try:  # noqa: WPS505
+                print_message('v4 is not supported. Starting provisioning using protocol v3')
+                unit_communication = UnitCommunicationV2(unit_address)
+                config.system_id, model_name = unit_communication.get_system_info()  # noqa: WPS414
+                config.protocol_version = unit_communication.get_protocol_version()
+                if config.protocol_version == 3:
+                    unit_communication.need_set_users = False
+                break
+            except GrpcUnimplemented as gu_exc:
+                print_message(f'[red]Grpc protocol error: {gu_exc}.')
+                raise gu_exc
+        except UnitError as unit_exc:
+            print_message('[yellow]Connection failed')
+            if retry + 1 < reconnect_times:
+                time.sleep(5)
+            else:
+                raise unit_exc
+
+    if config.system_id is None:
+        raise UnitError('Cannot read system_id')
+
+    config.set_model(model_name)
+    cloud_api.check_unit_is_not_provisioned(config.system_id)
+    if config.protocol_version >= 4:  # support of multi domains
+        config.node_ids = unit_communication.get_all_node_ids()
+        for node_id in config.node_ids:
+            config.supported_cert_types = unit_communication.get_cert_types(node_id)
+            need_disk_encryption = COMMAND_TO_DECRYPT in config.supported_cert_types
+
+            password = generate_random_password()
+
+            for clear_cert_type in config.supported_cert_types:
+                unit_communication.clear(clear_cert_type, node_id)
+
+            for set_cert_type in config.supported_cert_types:
+                unit_communication.set_cert_owner(set_cert_type, password, node_id)
+
+            if need_disk_encryption:
+                unit_communication.encrypt_disk(password, node_id)
+                config.supported_cert_types.remove(COMMAND_TO_DECRYPT)
+
+            for create_cert_type in config.supported_cert_types:
+                config.unit_certificates.append(unit_communication.create_keys(create_cert_type, password, node_id))
+    elif config.protocol_version == 3:
+        config.supported_cert_types = unit_communication.get_cert_types()
+        need_disk_encryption = COMMAND_TO_DECRYPT in config.supported_cert_types
+
+        password = generate_random_password()
+
+        for clear_cert_type in config.supported_cert_types:  # noqa: WPS440
+            unit_communication.clear(clear_cert_type)
+
+        for set_cert_type in config.supported_cert_types:  # noqa: WPS440
+            unit_communication.set_cert_owner(set_cert_type, password)
+
+        if need_disk_encryption:
+            unit_communication.encrypt_disk(password)
+            config.supported_cert_types.remove(COMMAND_TO_DECRYPT)
+            if config.protocol_version < 4:
+                unit_communication.wait_for_connection()
+
+        for create_cert_type in config.supported_cert_types:  # noqa: WPS440
+            config.unit_certificates.append(unit_communication.create_keys(create_cert_type, password))
+    else:
+        raise UnitError(f'aos-prov does not support {config.protocol_version} protocol of the Unit')
+
+    register_payload = {
+        'hardware_id': config.system_id,
+        'system_uid': config.system_id,
+        'model_name': config.model_name,
+        'model_version': config.model_version,
+        'provisioning_software': 'aos-provisioning:3.1',
+        'additional_csrs': [],
+    }
+
+    for csr_cert in config.unit_certificates:
+        if csr_cert.cert_type == 'online':
+            register_payload['online_public_csr'] = csr_cert.csr
+            if csr_cert.node_id:
+                register_payload['online_public_node_id'] = csr_cert.node_id
+        elif csr_cert.cert_type == 'offline':
+            register_payload['offline_public_csr'] = csr_cert.csr
+            if csr_cert.node_id:
+                register_payload['offline_public_node_id'] = csr_cert.node_id
+        else:
+            register_payload['additional_csrs'].append({
+                'cert_type': csr_cert.cert_type,
+                'csr': csr_cert.csr,
+                'node_id': csr_cert.node_id,
+            })
+
+    response = cloud_api.register_device(register_payload)
+    system_uid = response.get('system_uid')
+    additional_certs = response.get('additional_certs', [])
+    for cert in config.unit_certificates:
+        if cert.cert_type == 'online':
+            cert.certificate = response.get('online_certificate')
+        elif cert.cert_type == 'offline':
+            cert.certificate = response.get('offline_certificate')
+        else:
+            for additional_cert in additional_certs:
+                if additional_cert['cert_type'] == cert.cert_type:
+                    if additional_cert.get('node_id'):
+                        if additional_cert.get('node_id') == cert.node_id:
+                            cert.certificate = additional_cert['cert']
+                            break
+                    else:
+                        cert.certificate = additional_cert['cert']
+                        cert.node_id = additional_cert.get('node_id')
+                        break
+
+    for apply_cert in config.unit_certificates:
+        unit_communication.apply_certificate(apply_cert)
+
+    unit_communication.finish_provisioning()
+
+    print_message('[green]Finished successfully!')
+    link = cloud_api.get_unit_link_by_system_uid(system_uid)
+
+    if link:
+        print_message(f'You may find your unit on the cloud here: [green]{link}')
```

## aos_prov/commands/command_vm.py

```diff
@@ -1,142 +1,138 @@
-#
-#  Copyright (c) 2018-2023 Renesas Inc.
-#  Copyright (c) 2018-2023 EPAM Systems Inc.
-#
-import platform
-import socket
-import sys
-from pathlib import Path
-from random import randint
-from shutil import copyfile
-
-if platform.system() == 'Linux':
-    sys.path.append('/usr/lib/virtualbox')
-    sys.path.append('/usr/lib/virtualbox/sdk/bindings/xpcom/python/')
-elif platform.system() == 'Darwin':
-    sys.path.append('/Applications/VirtualBox.app/Contents/MacOS')
-    sys.path.append('/Applications/VirtualBox.app/Contents/MacOS/sdk/bindings/xpcom/python/')
-
-from aos_prov.utils.common import IMAGE_WITHOUT_NODES_FILENAME, AOS_DISKS_PATH
-from aos_prov.utils.errors import AosProvError, OnUnitError
-
-try:
-    import virtualbox
-    from virtualbox.library import StorageBus, StorageControllerType, IMachine, \
-        DeviceType, AccessMode, NATProtocol, FirmwareType
-except Exception:
-    pass
-
-
-def __create_storage_controller(machine: IMachine):
-    storage_controller = machine.add_storage_controller('IDE', StorageBus.ide)
-    storage_controller.controller_type = StorageControllerType.piix4
-    storage_controller.use_host_io_cache = True
-
-
-def __attach_disk(machine: IMachine, location):
-    medium = machine.parent.open_medium(
-        location,
-        DeviceType.hard_disk,
-        AccessMode.read_write,
-        True
-    )
-    machine.attach_device('IDE', 0, 0, DeviceType.hard_disk, medium)
-
-
-def __check_disk_exist(disk_location: str):
-    disk = Path(disk_location)
-    if not disk.is_file():
-        raise OnUnitError('Disk file not found')
-
-
-def new_vm(vm_name: str, disk_location: str):
-    print('Creating new virtual machine...')
-
-    disk_location_path = Path(disk_location)
-
-    if not (disk_location_path / IMAGE_WITHOUT_NODES_FILENAME).exists():
-        raise AosProvError(
-            'Disk image ' + (disk_location_path / IMAGE_WITHOUT_NODES_FILENAME) + ' not found or not a file',
-        )
-
-    vbox = virtualbox.VirtualBox()
-    try:
-        machine = vbox.create_machine('', vm_name, ['/AosUnits'], 'Linux_64', '')
-    except virtualbox.library_base.VBoxError as e:
-        print(e)
-        raise Exception('Such VM exist')
-    machine.vram_size = 32
-    machine.memory_size = 256
-    machine.cpu_count = 1
-    machine.firmware_type = FirmwareType.efi
-    machine.bios_settings.ioapic_enabled = platform.system() != 'Windows'
-    __create_storage_controller(machine)
-    vbox.register_machine(machine)
-
-    machine_folder = vbox.system_properties.default_machine_folder
-    machine_config_file_name = vbox.compose_machine_filename(vm_name, '/AosUnits', '', machine_folder)
-    vm_dir = Path(machine_config_file_name).parent
-    disk_image = str(Path(vm_dir / 'aos-disk.vmdk').absolute())
-    copyfile((disk_location_path / IMAGE_WITHOUT_NODES_FILENAME), disk_image)
-
-    with machine.create_session() as session:
-        __attach_disk(session.machine, location=disk_image)
-        session.machine.save_settings()
-
-    return forward_provisioning_ports(vm_name, vm_name + 'PortForward')
-
-
-def start_vm(vm_name: str):
-    print('Starting virtual machine...')
-    vbox = virtualbox.VirtualBox()
-    machine = vbox.find_machine(vm_name)
-    session = virtualbox.Session()
-    vm = machine.launch_vm_process(session, 'gui', [])
-    vm.wait_for_completion(timeout=-1)
-
-
-def remove_vm(vm_name: str):
-    print('Removing virtual machine...')
-    vbox = virtualbox.VirtualBox()
-    machine = vbox.find_machine(vm_name)
-    machine.remove(delete=True)
-
-def forward_provisioning_ports(vm_name: str, redirect_name: str = 'provisioningPortForward', forward_to_port=None):
-    if forward_to_port is None:
-        forward_to_port = randint(8090, 8999)
-        while _is_port_in_use(forward_to_port):
-            forward_to_port = randint(8090, 8999)
-
-    print(f'...will forward provisioning port {8089} to {forward_to_port}')
-    vbox = virtualbox.VirtualBox()
-    machine = vbox.find_machine(vm_name)
-    session = virtualbox.Session()
-    try:
-        machine.lock_machine(session, virtualbox.library.LockType.write)
-        mutable_machine = session.machine
-        adapter = mutable_machine.get_network_adapter(0)
-        adapter.nat_engine.add_redirect(redirect_name, NATProtocol(1), '', forward_to_port, '0.0.0.0', 8089)
-        session.machine.save_settings()
-    finally:
-        session.unlock_machine()
-    return forward_to_port
-
-
-def delete_provisioning_ports(vm_name: str, redirect_name: str = 'provisioningPortForward'):
-    vbox = virtualbox.VirtualBox()
-    machine = vbox.find_machine(vm_name)
-    session = virtualbox.Session()
-    try:
-        machine.lock_machine(session, virtualbox.library.LockType.write)
-        mutable_machine = session.machine
-        adapter = mutable_machine.get_network_adapter(0)
-        adapter.nat_engine.remove_redirect(redirect_name)
-        session.machine.save_settings()
-        session.unlock_machine()
-    except Exception:
-        pass
-
-
-def _is_port_in_use(port):
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-        return s.connect_ex(('localhost', port)) == 0
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
+import platform
+import socket
+import sys
+from pathlib import Path
+from random import randint
+from shutil import copyfile
+
+if platform.system() == 'Linux':
+    sys.path.append('/usr/lib/virtualbox')
+    sys.path.append('/usr/lib/virtualbox/sdk/bindings/xpcom/python/')
+elif platform.system() == 'Darwin':
+    sys.path.append('/Applications/VirtualBox.app/Contents/MacOS')
+    sys.path.append('/Applications/VirtualBox.app/Contents/MacOS/sdk/bindings/xpcom/python/')
+
+
+from aos_prov.actions import download_image
+from aos_prov.utils.common import DISK_IMAGE_DOWNLOAD_URL, AOS_DISK_PATH
+from aos_prov.utils.errors import OnBoardingError, AosProvError
+
+try:
+    import virtualbox
+    from virtualbox.library import StorageBus, StorageControllerType, IMachine, \
+        DeviceType, AccessMode, NATProtocol, FirmwareType
+except Exception:
+    pass
+
+
+def __create_storage_controller(machine: IMachine):
+    storage_controller = machine.add_storage_controller('IDE', StorageBus.ide)
+    storage_controller.controller_type = StorageControllerType.piix4
+    storage_controller.use_host_io_cache = True
+
+
+def __attach_disk(machine: IMachine, location):
+    medium = machine.parent.open_medium(
+        location,
+        DeviceType.hard_disk,
+        AccessMode.read_write,
+        True
+    )
+    machine.attach_device('IDE', 0, 0, DeviceType.hard_disk, medium)
+
+
+def __check_disk_exist(disk_location: str):
+    disk = Path(disk_location)
+    if not disk.is_file():
+        raise OnBoardingError("Disk file not found")
+
+
+def new_vm(vm_name: str, disk_location: str):
+    print('Creating new virtual machine...')
+
+    disk_location_path = Path(disk_location)
+
+    if not disk_location_path.is_file():
+        if disk_location_path == AOS_DISK_PATH:
+            download_image(DISK_IMAGE_DOWNLOAD_URL)
+        else:
+            raise AosProvError('Disk image ' + disk_location + ' not found or not a file')
+
+    vbox = virtualbox.VirtualBox()
+    try:
+        machine = vbox.create_machine('', vm_name, ['/AosUnits'], 'Linux_64', '')
+    except virtualbox.library_base.VBoxError:
+        raise Exception('Such VM exist')
+    machine.vram_size = 32
+    machine.memory_size = 256
+    machine.cpu_count = 1
+    machine.firmware_type = FirmwareType.efi
+    machine.bios_settings.ioapic_enabled = platform.system() != 'Windows'
+    __create_storage_controller(machine)
+    vbox.register_machine(machine)
+
+    machine_folder = vbox.system_properties.default_machine_folder
+    machine_config_file_name = vbox.compose_machine_filename(vm_name, '/AosUnits', '', machine_folder)
+    vm_dir = Path(machine_config_file_name).parent
+    disk_image = str(Path(vm_dir / 'aos-disk.vmdk').absolute())
+    copyfile(disk_location, disk_image)
+
+    with machine.create_session() as session:
+        __attach_disk(session.machine, location=disk_image)
+        session.machine.save_settings()
+
+    return forward_provisioning_ports(vm_name, vm_name + 'PortForward')
+
+
+def start_vm(vm_name: str):
+    print('Starting virtual machine...')
+    vbox = virtualbox.VirtualBox()
+    machine = vbox.find_machine(vm_name)
+    session = virtualbox.Session()
+    vm = machine.launch_vm_process(session, "gui", [])
+    vm.wait_for_completion(timeout=-1)
+
+
+def forward_provisioning_ports(vm_name: str, redirect_name: str = 'provisioningPortForward', forward_to_port=None):
+    if forward_to_port is None:
+        forward_to_port = randint(8090, 8999)
+        while _is_port_in_use(forward_to_port):
+            forward_to_port = randint(8090, 8999)
+
+    print(f'...will forward provisioning port {8089} to {forward_to_port}')
+    vbox = virtualbox.VirtualBox()
+    machine = vbox.find_machine(vm_name)
+    session = virtualbox.Session()
+    try:
+        machine.lock_machine(session, virtualbox.library.LockType.write)
+        mutable_machine = session.machine
+        adapter = mutable_machine.get_network_adapter(0)
+        adapter.nat_engine.add_redirect(redirect_name, NATProtocol(1), '', forward_to_port, '0.0.0.0', 8089)
+        session.machine.save_settings()
+    finally:
+        session.unlock_machine()
+    return forward_to_port
+
+
+def delete_provisioning_ports(vm_name: str, redirect_name: str = 'provisioningPortForward'):
+    vbox = virtualbox.VirtualBox()
+    machine = vbox.find_machine(vm_name)
+    session = virtualbox.Session()
+    try:
+        machine.lock_machine(session, virtualbox.library.LockType.write)
+        mutable_machine = session.machine
+        adapter = mutable_machine.get_network_adapter(0)
+        adapter.nat_engine.remove_redirect(redirect_name)
+        session.machine.save_settings()
+        session.unlock_machine()
+    except Exception:
+        pass
+
+
+def _is_port_in_use(port):
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+        return s.connect_ex(('localhost', port)) == 0
```

## aos_prov/commands/command_vm_multi_node_manage.py

 * *Ordering differences only*

```diff
@@ -1,563 +1,563 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-# pylint: disable=R0913,R0914,R0915
-import os
-import platform
-import socket
-import subprocess
-import uuid
-from pathlib import Path
-from random import randint
-from shutil import copyfile
-
-from aos_prov.commands.download import download_and_save_multinode
-from aos_prov.utils.common import (
-    AOS_DISKS_PATH,
-    DISK_IMAGE_DOWNLOAD_URL,
-    DOWNLOADS_PATH,
-    IMAGE_WITHOUT_NODES_FILENAME,
-    NODE0_IMAGE_FILENAME,
-    NODE1_IMAGE_FILENAME,
-    print_done,
-    print_error,
-    print_left,
-    print_message,
-    print_success,
-)
-from aos_prov.utils.errors import AosProvError
-
-_MIN_PORT = 8090
-_MAX_PORT = 8999
-_PROVISION_PORT = 8089
-_SSH_PORT = 22
-
-
-def _is_port_in_use(port):
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as socket_handler:
-        return socket_handler.connect_ex(('localhost', port)) == 0
-
-
-def _delete_controller(vm_uuid: str, controller_name: str):
-    command = [
-        'VBoxManage',
-        'storagectl',
-        vm_uuid,
-        f'--name={controller_name}',
-        '--controller=',
-        '--remove',
-    ]
-    execute_command(command, catch_error=False)
-
-
-def _create_storage_controller_ahci(vm_uuid: str, controller_name: str):
-    """Create SATA controller for VM.
-
-    Args:
-        vm_uuid (str): UUID or Name of VM to attach controller.
-         controller_name (str): Name of the controller.
-    """
-    command = [
-        'VBoxManage',
-        'storagectl',
-        vm_uuid,
-        f'--name={controller_name}',
-        '--add=sata',
-        '--controller=IntelAhci',
-        '--portcount=1',
-        '--hostiocache=on',
-        '--bootable=on',
-    ]
-    execute_command(command)
-
-
-def _create_storage_controller_piix4(vm_uuid: str, controller_name: str):
-    """Create SATA controller for VM.
-
-    Args:
-         vm_uuid (str): UUID or Name of VM to attach controller.
-         controller_name (str): Name of the controller.
-    """
-    # TODO: remove in case support of old version R3.0.1 is not required
-    command = [
-        'VBoxManage',
-        'storagectl',
-        vm_uuid,
-        f'--name={controller_name}',
-        '--add=ide',
-        '--controller=PIIX4',
-        '--portcount=2',
-        '--hostiocache=on',
-        '--bootable=on',
-    ]
-    execute_command(command)
-
-
-def _attach_disk(vm_uuid: str, attach_to_controller_name: str, disk_location: str, add_disk=False):
-    """Attach disk file to the controller.
-
-    Args:
-         vm_uuid (str): UUID or Name of VM to attach controller.
-         attach_to_controller_name (str): Name of the controller where disk will be attached.
-         disk_location (str): path to the disk file.
-         add_disk (bool): If true, add disk file to the VM
-    """
-    command = [
-        'VBoxManage',
-        'storageattach',
-        vm_uuid,
-        '--storagectl',
-        attach_to_controller_name,
-        '--port',
-        '0',
-        '--type',
-        'hdd',
-        '--medium',
-        disk_location,
-    ]
-
-    if add_disk:
-        command.append('--device')
-        command.append('0')
-
-    execute_command(command)
-
-
-def _create_network(network_name: str):
-    print_left('Creating a network for the units...')
-    command = [
-        'VBoxManage',
-        'natnetwork',
-        'add',
-        '--netname',
-        network_name,
-        '--network',
-        '10.0.0.0/24',
-        '--enable',
-        '--dhcp',
-        'on',
-    ]
-    execute_command(command)
-    print_success(f'Network {network_name} has been created')
-
-
-def _remove_network(network_name: str):
-    print_left(f'Removing a network: {network_name} for the units...')
-    command = [
-        'VBoxManage',
-        'natnetwork',
-        'remove',
-        '--netname',
-        network_name,
-    ]
-    execute_command(command, catch_error=True)
-    print_message('Network has been removed')
-
-
-def _forward_port_nat_network(network_name: str, forward_name: str, from_ip: str, from_port: int, to_port=None) -> int:
-    if to_port is None:
-        to_port = randint(_MIN_PORT, _MAX_PORT)  # noqa: S311
-        while _is_port_in_use(to_port):
-            to_port = randint(_MIN_PORT, _MAX_PORT)  # noqa: S311
-
-    command = [
-        'VBoxManage',
-        'natnetwork',
-        'modify',
-        '--netname',
-        network_name,
-        '--port-forward-4',
-        f'{forward_name}:tcp:[]:{to_port}:[{from_ip}]:{from_port}',
-    ]
-
-    execute_command(command)
-    return to_port
-
-
-def _forward_port_nat(forward_name: str, from_port: int, to_port=None, vm_uuid: str = '') -> int:
-    # TODO: remove in case support of old version R3.0.1 is not required
-    if to_port is None:
-        to_port = randint(_MIN_PORT, _MAX_PORT)  # noqa: S311
-        while _is_port_in_use(to_port):
-            to_port = randint(_MIN_PORT, _MAX_PORT)  # noqa: S311
-    command_nat = [
-        'VBoxManage',
-        'modifyvm',
-        vm_uuid,
-        '--nic1',
-        'nat',
-        '--nic-type1',
-        '82545EM',
-    ]
-    execute_command(command_nat)
-
-    command_forward = [
-        'VBoxManage',
-        'modifyvm',
-        vm_uuid,
-        '--natpf1',
-        f'{forward_name},tcp,,{to_port},,{from_port}',
-    ]
-
-    execute_command(command_forward)
-
-    return to_port
-
-
-def check_virtual_box():
-    print_left('Checking VirtualBox...')
-
-    if platform.machine().lower() not in {'amd64', 'x86_64'}:
-        raise AosProvError('Only amd64 architecture is supported.')
-
-    try:
-        response = execute_command(['VBoxManage', '--version'], catch_error=False)
-    except AosProvError as exc:
-        raise AosProvError('VirtualBox is not installed or it is not in the PATH') from exc
-
-    if 'WARNING: The vboxdrv kernel module is not loaded' in response:
-        raise AosProvError('VirtualBox kernel modules is not installed.')
-
-    if not response.startswith('7'):
-        raise AosProvError('VirtualBox 7 is only supported')
-
-    print_success(response)
-
-
-def new_vms(vm_name: str, disk_location: str, nodes_count=2, check_virtualbox=True) -> ():
-    if check_virtualbox:
-        check_virtual_box()
-    print_message('Creating a new virtual machines...')
-
-    disk_location_path = Path(disk_location)
-    is_image_without_nodes = False
-
-    if (disk_location_path / IMAGE_WITHOUT_NODES_FILENAME).exists():
-        # TODO: remove in case support of old version R3.0.1 is not required
-        print_message('Found VM image (v3.0.1) without supporting Nodes functionality. Use it as one node VM.')
-        nodes_count = 1
-        nodes = [
-            {
-                'name': 'node0',
-                'uuid': str(uuid.uuid4()),
-                'disk_name': IMAGE_WITHOUT_NODES_FILENAME,
-                'disk_location': Path(disk_location_path / IMAGE_WITHOUT_NODES_FILENAME),
-            },
-        ]
-        is_image_without_nodes = True
-    else:
-        node0_exists = (disk_location_path / NODE0_IMAGE_FILENAME).exists()
-        node1_exists = (disk_location_path / NODE1_IMAGE_FILENAME).exists()
-        if not node0_exists or not node1_exists:
-            if disk_location_path != AOS_DISKS_PATH:
-                raise AosProvError(f'Disk images not found in directory {disk_location}. Cannot proceed!')
-            print_message('Local images not found. Downloading...')
-            download_and_save_multinode(DISK_IMAGE_DOWNLOAD_URL, DOWNLOADS_PATH, force_overwrite=False)
-            print_success('Download finished. You may find Unit images in: ' + str(DOWNLOADS_PATH.resolve()))
-        nodes = [
-            {
-                'name': 'node0',
-                'uuid': str(uuid.uuid4()),
-                'disk_name': NODE0_IMAGE_FILENAME,
-                'disk_location': Path(disk_location_path / NODE0_IMAGE_FILENAME),
-            },
-        ]
-
-        if nodes_count != 1:
-            nodes.append(
-                {
-                    'name': 'node1',
-                    'uuid': str(uuid.uuid4()),
-                    'disk_name': NODE1_IMAGE_FILENAME,
-                    'disk_location': Path(disk_location_path / NODE1_IMAGE_FILENAME),
-                },
-            )
-
-    units_network_name = f'aos-network-{vm_name}'
-    units_vm_group = f'/AosUnits/{vm_name}'
-    try:
-        provisioning_port, node0_ssh_port, node1_ssh_port = None, None, None
-        if not is_image_without_nodes:
-            _create_network(units_network_name)
-            print_left('Forwarding provisioning port...')
-            provisioning_port = _forward_port_nat_network(
-                units_network_name,
-                forward_name='provisioningPortForward',
-                from_ip='10.0.0.100',
-                from_port=_PROVISION_PORT,
-            )
-            print_success(provisioning_port)
-
-            print_left('Forwarding ssh port to node0...')
-            node0_ssh_port = _forward_port_nat_network(
-                units_network_name,
-                forward_name='node0ssh',
-                from_ip='10.0.0.100',
-                from_port=_SSH_PORT,
-            )
-            print_success(node0_ssh_port)
-
-            node1_ssh_port = None
-            if nodes_count > 1:
-                print_left('Forwarding ssh port to node1...')
-                node1_ssh_port = _forward_port_nat_network(
-                    units_network_name,
-                    forward_name='node1ssh',
-                    from_ip='10.0.0.101',
-                    from_port=_SSH_PORT,
-                )
-                print_success(node1_ssh_port)
-
-        for node in nodes:
-            print_left(f'Creating a new VM for {node["name"]}...')
-            create_node_vm(
-                node['name'],
-                node['uuid'],
-                units_vm_group,
-                node['disk_location'],
-                node['disk_name'],
-                units_network_name,
-                is_image_without_nodes,
-            )
-            print_done()
-
-            if is_image_without_nodes:
-                # TODO: remove in case support of old version R3.0.1 is not required
-                print_left('Forwarding provisioning port...')
-                provisioning_port = _forward_port_nat(
-                    forward_name='provisioningPortForward',
-                    from_port=_PROVISION_PORT,
-                    vm_uuid=node['uuid'],
-                )
-                print_success(provisioning_port)
-
-                print_left('Forwarding ssh port to node0...')
-                node0_ssh_port = _forward_port_nat(
-                    forward_name='node0ssh',
-                    from_port=_SSH_PORT,
-                    vm_uuid=node['uuid'],
-                )
-                print_success(node0_ssh_port)
-
-        return provisioning_port, node0_ssh_port, node1_ssh_port
-    except AosProvError as error:
-        print_error('Cannot create VM. Clean up all related resources. Try again.')
-        remove_vms_in_group(vm_name)
-        raise error
-
-
-def create_node_vm(  # noqa: WPS211
-    vm_name: str,
-    vm_uuid: str,
-    group: str,
-    original_disk_path: Path,
-    disk_name: str,
-    network_name,
-    is_image_without_nodes: bool,
-):
-    create_vm_command = [
-        'VBoxManage',
-        'createvm',
-        f'--name={vm_name}',
-        '--ostype=Linux_64',
-        f'--uuid={vm_uuid}',
-        f'--groups={group}',
-        '--default',
-        '--register',
-    ]
-
-    cpu_count = 1
-    if platform.system() in {'Windows', 'Darwin'}:
-        cpu_count = 4
-
-    set_vm_params = [
-        'VBoxManage',
-        'modifyvm',
-        vm_uuid,
-        '--memory=1024',
-        '--firmware=efi',
-        f'--cpus={cpu_count}',
-    ]
-
-    set_vm_net = [
-        'VBoxManage',
-        'modifyvm',
-        vm_uuid,
-        '--nic1=natnetwork',
-        f'--nat-network1={network_name}',
-    ]
-
-    # Set paravirtualization to KVM
-    set_vm_kvm = [
-        'VBoxManage',
-        'modifyvm',
-        vm_uuid,
-        '--paravirt-provider=kvm',
-    ]
-
-    disable_time_sync = [
-        'VBoxManage',
-        'setextradata',
-        vm_uuid,
-        '"VBoxInternal/Devices/VMMDev/0/Config/GetHostTimeDisabled" 1',
-    ]
-
-    execute_command(create_vm_command)
-    execute_command(set_vm_params)
-    if not is_image_without_nodes:
-        execute_command(set_vm_net)
-    execute_command(set_vm_kvm)
-    execute_command(disable_time_sync)
-    _delete_controller(vm_uuid, 'SATA')
-    _delete_controller(vm_uuid, 'IDE')
-
-    if is_image_without_nodes:
-        # TODO: remove in case support of old version R3.0.1 is not required
-        _create_storage_controller_piix4(vm_uuid, 'SATA')
-    else:
-        _create_storage_controller_ahci(vm_uuid, 'SATA')
-
-    destination_image = str((_find_vm_location(vm_uuid) / disk_name).resolve())
-    copyfile(original_disk_path.absolute(), destination_image)
-
-    try:
-        _attach_disk(vm_uuid, 'SATA', disk_location=destination_image, add_disk=is_image_without_nodes)
-    except AosProvError as error:
-        print_error(f'Cannot attach disk {destination_image} to VM. Clean up all related resources. Try again.')
-        os.remove(destination_image)
-        raise error
-
-
-def remove_vms_in_group(vm_name: str):
-    units_network_name = f'aos-network-{vm_name}'
-    vm_group = f'/AosUnits/{vm_name}'
-
-    print_message(f'Removing VMs in Groups: {vm_group} for the units...')
-
-    # find uuids of all VMs into the required Group
-    detailed_list_vms_command = [
-        'VBoxManage',
-        'list',
-        'vms',
-        '--long',
-    ]
-    detailed_list_vms_out = execute_command(detailed_list_vms_command, catch_error=True)
-    detailed_list_vms = {}
-    processed_group_vm = ''
-    for output_line in detailed_list_vms_out.splitlines():
-        if output_line.startswith('Groups:'):
-            # line format is: 'Groups:                      /AosUnits/my-test-vm1'
-            if len(output_line.split()) == 2:
-                processed_group_vm = output_line.split()[1]
-        elif output_line.startswith('UUID:'):
-            # line format is: 'UUID:                        49f87eef-838b-43cb-b6eb-604989b15f9f'
-            if len(output_line.split()) == 2:
-                vm_uuid = output_line.split()[1]
-                list_of_uuids = []
-                if detailed_list_vms.get(processed_group_vm):
-                    list_of_uuids = detailed_list_vms[processed_group_vm]
-                if vm_uuid not in list_of_uuids:
-                    list_of_uuids.append(vm_uuid)
-                    detailed_list_vms[processed_group_vm] = list_of_uuids
-
-    _remove_network(units_network_name)
-
-    if not detailed_list_vms.get(vm_group):
-        print_error(f'VM Group: {vm_group} is not presented on system.')
-        return
-
-    for vm_uuid in detailed_list_vms[vm_group]:  # noqa: WPS440
-        delete_vm_command = [
-            'VBoxManage',
-            'unregistervm',
-            vm_uuid,
-            '--delete',
-        ]
-        execute_command(delete_vm_command, catch_error=False)
-    print_message('VMs have been deleted')
-
-
-def _find_vm_location(vm_uuid) -> Path:
-    set_vm_params = [
-        'VBoxManage',
-        'showvminfo',
-        vm_uuid,
-        '--machinereadable',
-    ]
-
-    response = execute_command(set_vm_params)
-
-    for row in response.splitlines():
-        param_from_row = row.split('=')
-        if param_from_row[0] == 'CfgFile':
-            return Path(param_from_row[1].replace('"', '')).parent
-    return Path()
-
-
-def start_vms(group: str, check_virtualbox: bool = False, headless=False):
-    """Start all VMs in the group.
-
-    Args:
-        group (str): Name of the group to start
-        check_virtualbox (bool): Check VirtualBox status before execution
-        headless (bool): Start VM in headless mode if True
-
-    Raises:
-        AosProvError: If no VMs to start found.
-    """
-    if check_virtualbox:
-        check_virtual_box()
-
-    message = f'Starting VMs in group [bold]{group}[/bold]'
-
-    if headless:
-        message += ' in headless mode'
-
-    print_message(message)
-    vms_to_start = []
-    vms = execute_command(['VBoxManage', 'list', 'vms'])
-
-    for virtual_machines in vms.splitlines():
-        guid = virtual_machines[virtual_machines.find('{') + 1:virtual_machines.find('}')]
-        info_out = request_vm_info(guid)
-
-        for row in info_out.splitlines():
-            if row.startswith('groups='):
-                vm_group = row.replace('"', '').split('=')[1]
-                if group == vm_group:
-                    vms_to_start.append(guid)
-                    break
-
-    if not vms_to_start:
-        raise AosProvError(f'No VMs found in group {group} to start!')
-
-    start_type = 'headless' if headless else 'gui'
-
-    for vm_guid in vms_to_start:
-        start_command = ['VBoxManage', 'startvm', vm_guid, f'--type={start_type}']
-        print_left(f'Starting VM {vm_guid}...')
-        try:
-            execute_command(start_command, catch_error=True)
-        except AosProvError as exc:
-            if 'is already locked by a session' in str(exc):
-                print_message('[YELLOW]SKIPPING due to lock')
-            else:
-                print_message('[RED]ERROR')
-                print_error(str(exc))
-        print_done()
-
-
-def request_vm_info(vm_guid):
-    return execute_command(['VBoxManage', 'showvminfo', vm_guid, '--machinereadable'])
-
-
-def execute_command(command, catch_error=False) -> str:
-    execution_status = subprocess.run(command, shell=False, env=os.environ.copy(), capture_output=True, check=False)
-    if execution_status.returncode == 0:
-        return execution_status.stdout.decode('utf-8')
-
-    if not catch_error:
-        raise AosProvError(execution_status.stderr.decode('utf-8'))
-
-    return ''
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+# pylint: disable=R0913,R0914,R0915
+import os
+import platform
+import socket
+import subprocess
+import uuid
+from pathlib import Path
+from random import randint
+from shutil import copyfile
+
+from aos_prov.commands.download import download_and_save_multinode
+from aos_prov.utils.common import (
+    AOS_DISKS_PATH,
+    DISK_IMAGE_DOWNLOAD_URL,
+    DOWNLOADS_PATH,
+    IMAGE_WITHOUT_NODES_FILENAME,
+    NODE0_IMAGE_FILENAME,
+    NODE1_IMAGE_FILENAME,
+    print_done,
+    print_error,
+    print_left,
+    print_message,
+    print_success,
+)
+from aos_prov.utils.errors import AosProvError
+
+_MIN_PORT = 8090
+_MAX_PORT = 8999
+_PROVISION_PORT = 8089
+_SSH_PORT = 22
+
+
+def _is_port_in_use(port):
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as socket_handler:
+        return socket_handler.connect_ex(('localhost', port)) == 0
+
+
+def _delete_controller(vm_uuid: str, controller_name: str):
+    command = [
+        'VBoxManage',
+        'storagectl',
+        vm_uuid,
+        f'--name={controller_name}',
+        '--controller=',
+        '--remove',
+    ]
+    execute_command(command, catch_error=False)
+
+
+def _create_storage_controller_ahci(vm_uuid: str, controller_name: str):
+    """Create SATA controller for VM.
+
+    Args:
+        vm_uuid (str): UUID or Name of VM to attach controller.
+         controller_name (str): Name of the controller.
+    """
+    command = [
+        'VBoxManage',
+        'storagectl',
+        vm_uuid,
+        f'--name={controller_name}',
+        '--add=sata',
+        '--controller=IntelAhci',
+        '--portcount=1',
+        '--hostiocache=on',
+        '--bootable=on',
+    ]
+    execute_command(command)
+
+
+def _create_storage_controller_piix4(vm_uuid: str, controller_name: str):
+    """Create SATA controller for VM.
+
+    Args:
+         vm_uuid (str): UUID or Name of VM to attach controller.
+         controller_name (str): Name of the controller.
+    """
+    # TODO: remove in case support of old version R3.0.1 is not required
+    command = [
+        'VBoxManage',
+        'storagectl',
+        vm_uuid,
+        f'--name={controller_name}',
+        '--add=ide',
+        '--controller=PIIX4',
+        '--portcount=2',
+        '--hostiocache=on',
+        '--bootable=on',
+    ]
+    execute_command(command)
+
+
+def _attach_disk(vm_uuid: str, attach_to_controller_name: str, disk_location: str, add_disk=False):
+    """Attach disk file to the controller.
+
+    Args:
+         vm_uuid (str): UUID or Name of VM to attach controller.
+         attach_to_controller_name (str): Name of the controller where disk will be attached.
+         disk_location (str): path to the disk file.
+         add_disk (bool): If true, add disk file to the VM
+    """
+    command = [
+        'VBoxManage',
+        'storageattach',
+        vm_uuid,
+        '--storagectl',
+        attach_to_controller_name,
+        '--port',
+        '0',
+        '--type',
+        'hdd',
+        '--medium',
+        disk_location,
+    ]
+
+    if add_disk:
+        command.append('--device')
+        command.append('0')
+
+    execute_command(command)
+
+
+def _create_network(network_name: str):
+    print_left('Creating a network for the units...')
+    command = [
+        'VBoxManage',
+        'natnetwork',
+        'add',
+        '--netname',
+        network_name,
+        '--network',
+        '10.0.0.0/24',
+        '--enable',
+        '--dhcp',
+        'on',
+    ]
+    execute_command(command)
+    print_success(f'Network {network_name} has been created')
+
+
+def _remove_network(network_name: str):
+    print_left(f'Removing a network: {network_name} for the units...')
+    command = [
+        'VBoxManage',
+        'natnetwork',
+        'remove',
+        '--netname',
+        network_name,
+    ]
+    execute_command(command, catch_error=True)
+    print_message('Network has been removed')
+
+
+def _forward_port_nat_network(network_name: str, forward_name: str, from_ip: str, from_port: int, to_port=None) -> int:
+    if to_port is None:
+        to_port = randint(_MIN_PORT, _MAX_PORT)  # noqa: S311
+        while _is_port_in_use(to_port):
+            to_port = randint(_MIN_PORT, _MAX_PORT)  # noqa: S311
+
+    command = [
+        'VBoxManage',
+        'natnetwork',
+        'modify',
+        '--netname',
+        network_name,
+        '--port-forward-4',
+        f'{forward_name}:tcp:[]:{to_port}:[{from_ip}]:{from_port}',
+    ]
+
+    execute_command(command)
+    return to_port
+
+
+def _forward_port_nat(forward_name: str, from_port: int, to_port=None, vm_uuid: str = '') -> int:
+    # TODO: remove in case support of old version R3.0.1 is not required
+    if to_port is None:
+        to_port = randint(_MIN_PORT, _MAX_PORT)  # noqa: S311
+        while _is_port_in_use(to_port):
+            to_port = randint(_MIN_PORT, _MAX_PORT)  # noqa: S311
+    command_nat = [
+        'VBoxManage',
+        'modifyvm',
+        vm_uuid,
+        '--nic1',
+        'nat',
+        '--nic-type1',
+        '82545EM',
+    ]
+    execute_command(command_nat)
+
+    command_forward = [
+        'VBoxManage',
+        'modifyvm',
+        vm_uuid,
+        '--natpf1',
+        f'{forward_name},tcp,,{to_port},,{from_port}',
+    ]
+
+    execute_command(command_forward)
+
+    return to_port
+
+
+def check_virtual_box():
+    print_left('Checking VirtualBox...')
+
+    if platform.machine().lower() not in {'amd64', 'x86_64'}:
+        raise AosProvError('Only amd64 architecture is supported.')
+
+    try:
+        response = execute_command(['VBoxManage', '--version'], catch_error=False)
+    except AosProvError as exc:
+        raise AosProvError('VirtualBox is not installed or it is not in the PATH') from exc
+
+    if 'WARNING: The vboxdrv kernel module is not loaded' in response:
+        raise AosProvError('VirtualBox kernel modules is not installed.')
+
+    if not response.startswith('7'):
+        raise AosProvError('VirtualBox 7 is only supported')
+
+    print_success(response)
+
+
+def new_vms(vm_name: str, disk_location: str, nodes_count=2, check_virtualbox=True) -> ():
+    if check_virtualbox:
+        check_virtual_box()
+    print_message('Creating a new virtual machines...')
+
+    disk_location_path = Path(disk_location)
+    is_image_without_nodes = False
+
+    if (disk_location_path / IMAGE_WITHOUT_NODES_FILENAME).exists():
+        # TODO: remove in case support of old version R3.0.1 is not required
+        print_message('Found VM image (v3.0.1) without supporting Nodes functionality. Use it as one node VM.')
+        nodes_count = 1
+        nodes = [
+            {
+                'name': 'node0',
+                'uuid': str(uuid.uuid4()),
+                'disk_name': IMAGE_WITHOUT_NODES_FILENAME,
+                'disk_location': Path(disk_location_path / IMAGE_WITHOUT_NODES_FILENAME),
+            },
+        ]
+        is_image_without_nodes = True
+    else:
+        node0_exists = (disk_location_path / NODE0_IMAGE_FILENAME).exists()
+        node1_exists = (disk_location_path / NODE1_IMAGE_FILENAME).exists()
+        if not node0_exists or not node1_exists:
+            if disk_location_path != AOS_DISKS_PATH:
+                raise AosProvError(f'Disk images not found in directory {disk_location}. Cannot proceed!')
+            print_message('Local images not found. Downloading...')
+            download_and_save_multinode(DISK_IMAGE_DOWNLOAD_URL, DOWNLOADS_PATH, force_overwrite=False)
+            print_success('Download finished. You may find Unit images in: ' + str(DOWNLOADS_PATH.resolve()))
+        nodes = [
+            {
+                'name': 'node0',
+                'uuid': str(uuid.uuid4()),
+                'disk_name': NODE0_IMAGE_FILENAME,
+                'disk_location': Path(disk_location_path / NODE0_IMAGE_FILENAME),
+            },
+        ]
+
+        if nodes_count != 1:
+            nodes.append(
+                {
+                    'name': 'node1',
+                    'uuid': str(uuid.uuid4()),
+                    'disk_name': NODE1_IMAGE_FILENAME,
+                    'disk_location': Path(disk_location_path / NODE1_IMAGE_FILENAME),
+                },
+            )
+
+    units_network_name = f'aos-network-{vm_name}'
+    units_vm_group = f'/AosUnits/{vm_name}'
+    try:
+        provisioning_port, node0_ssh_port, node1_ssh_port = None, None, None
+        if not is_image_without_nodes:
+            _create_network(units_network_name)
+            print_left('Forwarding provisioning port...')
+            provisioning_port = _forward_port_nat_network(
+                units_network_name,
+                forward_name='provisioningPortForward',
+                from_ip='10.0.0.100',
+                from_port=_PROVISION_PORT,
+            )
+            print_success(provisioning_port)
+
+            print_left('Forwarding ssh port to node0...')
+            node0_ssh_port = _forward_port_nat_network(
+                units_network_name,
+                forward_name='node0ssh',
+                from_ip='10.0.0.100',
+                from_port=_SSH_PORT,
+            )
+            print_success(node0_ssh_port)
+
+            node1_ssh_port = None
+            if nodes_count > 1:
+                print_left('Forwarding ssh port to node1...')
+                node1_ssh_port = _forward_port_nat_network(
+                    units_network_name,
+                    forward_name='node1ssh',
+                    from_ip='10.0.0.101',
+                    from_port=_SSH_PORT,
+                )
+                print_success(node1_ssh_port)
+
+        for node in nodes:
+            print_left(f'Creating a new VM for {node["name"]}...')
+            create_node_vm(
+                node['name'],
+                node['uuid'],
+                units_vm_group,
+                node['disk_location'],
+                node['disk_name'],
+                units_network_name,
+                is_image_without_nodes,
+            )
+            print_done()
+
+            if is_image_without_nodes:
+                # TODO: remove in case support of old version R3.0.1 is not required
+                print_left('Forwarding provisioning port...')
+                provisioning_port = _forward_port_nat(
+                    forward_name='provisioningPortForward',
+                    from_port=_PROVISION_PORT,
+                    vm_uuid=node['uuid'],
+                )
+                print_success(provisioning_port)
+
+                print_left('Forwarding ssh port to node0...')
+                node0_ssh_port = _forward_port_nat(
+                    forward_name='node0ssh',
+                    from_port=_SSH_PORT,
+                    vm_uuid=node['uuid'],
+                )
+                print_success(node0_ssh_port)
+
+        return provisioning_port, node0_ssh_port, node1_ssh_port
+    except AosProvError as error:
+        print_error('Cannot create VM. Clean up all related resources. Try again.')
+        remove_vms_in_group(vm_name)
+        raise error
+
+
+def create_node_vm(  # noqa: WPS211
+    vm_name: str,
+    vm_uuid: str,
+    group: str,
+    original_disk_path: Path,
+    disk_name: str,
+    network_name,
+    is_image_without_nodes: bool,
+):
+    create_vm_command = [
+        'VBoxManage',
+        'createvm',
+        f'--name={vm_name}',
+        '--ostype=Linux_64',
+        f'--uuid={vm_uuid}',
+        f'--groups={group}',
+        '--default',
+        '--register',
+    ]
+
+    cpu_count = 1
+    if platform.system() in {'Windows', 'Darwin'}:
+        cpu_count = 4
+
+    set_vm_params = [
+        'VBoxManage',
+        'modifyvm',
+        vm_uuid,
+        '--memory=1024',
+        '--firmware=efi',
+        f'--cpus={cpu_count}',
+    ]
+
+    set_vm_net = [
+        'VBoxManage',
+        'modifyvm',
+        vm_uuid,
+        '--nic1=natnetwork',
+        f'--nat-network1={network_name}',
+    ]
+
+    # Set paravirtualization to KVM
+    set_vm_kvm = [
+        'VBoxManage',
+        'modifyvm',
+        vm_uuid,
+        '--paravirt-provider=kvm',
+    ]
+
+    disable_time_sync = [
+        'VBoxManage',
+        'setextradata',
+        vm_uuid,
+        '"VBoxInternal/Devices/VMMDev/0/Config/GetHostTimeDisabled" 1',
+    ]
+
+    execute_command(create_vm_command)
+    execute_command(set_vm_params)
+    if not is_image_without_nodes:
+        execute_command(set_vm_net)
+    execute_command(set_vm_kvm)
+    execute_command(disable_time_sync)
+    _delete_controller(vm_uuid, 'SATA')
+    _delete_controller(vm_uuid, 'IDE')
+
+    if is_image_without_nodes:
+        # TODO: remove in case support of old version R3.0.1 is not required
+        _create_storage_controller_piix4(vm_uuid, 'SATA')
+    else:
+        _create_storage_controller_ahci(vm_uuid, 'SATA')
+
+    destination_image = str((_find_vm_location(vm_uuid) / disk_name).resolve())
+    copyfile(original_disk_path.absolute(), destination_image)
+
+    try:
+        _attach_disk(vm_uuid, 'SATA', disk_location=destination_image, add_disk=is_image_without_nodes)
+    except AosProvError as error:
+        print_error(f'Cannot attach disk {destination_image} to VM. Clean up all related resources. Try again.')
+        os.remove(destination_image)
+        raise error
+
+
+def remove_vms_in_group(vm_name: str):
+    units_network_name = f'aos-network-{vm_name}'
+    vm_group = f'/AosUnits/{vm_name}'
+
+    print_message(f'Removing VMs in Groups: {vm_group} for the units...')
+
+    # find uuids of all VMs into the required Group
+    detailed_list_vms_command = [
+        'VBoxManage',
+        'list',
+        'vms',
+        '--long',
+    ]
+    detailed_list_vms_out = execute_command(detailed_list_vms_command, catch_error=True)
+    detailed_list_vms = {}
+    processed_group_vm = ''
+    for output_line in detailed_list_vms_out.splitlines():
+        if output_line.startswith('Groups:'):
+            # line format is: 'Groups:                      /AosUnits/my-test-vm1'
+            if len(output_line.split()) == 2:
+                processed_group_vm = output_line.split()[1]
+        elif output_line.startswith('UUID:'):
+            # line format is: 'UUID:                        49f87eef-838b-43cb-b6eb-604989b15f9f'
+            if len(output_line.split()) == 2:
+                vm_uuid = output_line.split()[1]
+                list_of_uuids = []
+                if detailed_list_vms.get(processed_group_vm):
+                    list_of_uuids = detailed_list_vms[processed_group_vm]
+                if vm_uuid not in list_of_uuids:
+                    list_of_uuids.append(vm_uuid)
+                    detailed_list_vms[processed_group_vm] = list_of_uuids
+
+    _remove_network(units_network_name)
+
+    if not detailed_list_vms.get(vm_group):
+        print_error(f'VM Group: {vm_group} is not presented on system.')
+        return
+
+    for vm_uuid in detailed_list_vms[vm_group]:  # noqa: WPS440
+        delete_vm_command = [
+            'VBoxManage',
+            'unregistervm',
+            vm_uuid,
+            '--delete',
+        ]
+        execute_command(delete_vm_command, catch_error=False)
+    print_message('VMs have been deleted')
+
+
+def _find_vm_location(vm_uuid) -> Path:
+    set_vm_params = [
+        'VBoxManage',
+        'showvminfo',
+        vm_uuid,
+        '--machinereadable',
+    ]
+
+    response = execute_command(set_vm_params)
+
+    for row in response.splitlines():
+        param_from_row = row.split('=')
+        if param_from_row[0] == 'CfgFile':
+            return Path(param_from_row[1].replace('"', '')).parent
+    return Path()
+
+
+def start_vms(group: str, check_virtualbox: bool = False, headless=False):
+    """Start all VMs in the group.
+
+    Args:
+        group (str): Name of the group to start
+        check_virtualbox (bool): Check VirtualBox status before execution
+        headless (bool): Start VM in headless mode if True
+
+    Raises:
+        AosProvError: If no VMs to start found.
+    """
+    if check_virtualbox:
+        check_virtual_box()
+
+    message = f'Starting VMs in group [bold]{group}[/bold]'
+
+    if headless:
+        message += ' in headless mode'
+
+    print_message(message)
+    vms_to_start = []
+    vms = execute_command(['VBoxManage', 'list', 'vms'])
+
+    for virtual_machines in vms.splitlines():
+        guid = virtual_machines[virtual_machines.find('{') + 1:virtual_machines.find('}')]
+        info_out = request_vm_info(guid)
+
+        for row in info_out.splitlines():
+            if row.startswith('groups='):
+                vm_group = row.replace('"', '').split('=')[1]
+                if group == vm_group:
+                    vms_to_start.append(guid)
+                    break
+
+    if not vms_to_start:
+        raise AosProvError(f'No VMs found in group {group} to start!')
+
+    start_type = 'headless' if headless else 'gui'
+
+    for vm_guid in vms_to_start:
+        start_command = ['VBoxManage', 'startvm', vm_guid, f'--type={start_type}']
+        print_left(f'Starting VM {vm_guid}...')
+        try:
+            execute_command(start_command, catch_error=True)
+        except AosProvError as exc:
+            if 'is already locked by a session' in str(exc):
+                print_message('[YELLOW]SKIPPING due to lock')
+            else:
+                print_message('[RED]ERROR')
+                print_error(str(exc))
+        print_done()
+
+
+def request_vm_info(vm_guid):
+    return execute_command(['VBoxManage', 'showvminfo', vm_guid, '--machinereadable'])
+
+
+def execute_command(command, catch_error=False) -> str:
+    execution_status = subprocess.run(command, shell=False, env=os.environ.copy(), capture_output=True, check=False)
+    if execution_status.returncode == 0:
+        return execution_status.stdout.decode('utf-8')
+
+    if not catch_error:
+        raise AosProvError(execution_status.stderr.decode('utf-8'))
+
+    return ''
```

## aos_prov/commands/download.py

 * *Ordering differences only*

```diff
@@ -1,71 +1,71 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-"""Download and save files command."""
-import os
-import tarfile
-from pathlib import Path
-
-import requests
-from aos_prov.utils.common import (
-    DOWNLOADS_PATH,
-    NODE0_IMAGE_FILENAME,
-    NODE1_IMAGE_FILENAME,
-    REQUEST_TIMEOUT,
-)
-from aos_prov.utils.errors import AosProvError
-from rich.progress import Progress
-
-_SAVE_CHUNK = 8192
-
-
-def _create_downloads_directory():
-    Path(DOWNLOADS_PATH).mkdir(parents=True, exist_ok=True)
-
-
-def download_and_save_multinode(download_url: str, save_path: Path, force_overwrite: bool = False) -> None:
-    """Download and save multi-node images.
-
-    Args:
-         download_url (str): URL to download
-         save_path (Path): Save destination url
-         force_overwrite (bool): Force to overwrite files
-
-    Raises:
-        AosProvError: If files exists and force_overwrite is false.
-    """
-    _create_downloads_directory()
-
-    node_files = [save_path / NODE0_IMAGE_FILENAME, save_path / NODE1_IMAGE_FILENAME]
-
-    for node_file in node_files:
-        if force_overwrite:
-            if os.path.exists(node_file):
-                os.remove(node_file)
-        elif node_file.exists():
-            raise AosProvError(f'Destination file {node_file} already exist. Delete it or download with -f key')
-
-    download_file_name = save_path / 'downloaded-multi-node-images.tar.gz'
-
-    with open(download_file_name, 'wb') as save_context:
-        response = requests.get(download_url, stream=True, timeout=REQUEST_TIMEOUT)
-        response.raise_for_status()
-
-        total_length = response.headers.get('content-length')
-
-        if total_length is None:  # no content length header
-            save_context.write(response.content)
-            return
-
-        with Progress() as progress:
-            task_id = progress.add_task('[cyan]Downloading...', total=int(total_length))
-            for received_data in response.iter_content(chunk_size=_SAVE_CHUNK):
-                progress.update(task_id, advance=len(received_data))
-                save_context.write(received_data)
-
-    with tarfile.open(download_file_name) as archive:
-        archive.extractall(save_path)  # noqa: S202
-
-    if os.path.exists(download_file_name):
-        os.remove(download_file_name)
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+"""Download and save files command."""
+import os
+import tarfile
+from pathlib import Path
+
+import requests
+from aos_prov.utils.common import (
+    DOWNLOADS_PATH,
+    NODE0_IMAGE_FILENAME,
+    NODE1_IMAGE_FILENAME,
+    REQUEST_TIMEOUT,
+)
+from aos_prov.utils.errors import AosProvError
+from rich.progress import Progress
+
+_SAVE_CHUNK = 8192
+
+
+def _create_downloads_directory():
+    Path(DOWNLOADS_PATH).mkdir(parents=True, exist_ok=True)
+
+
+def download_and_save_multinode(download_url: str, save_path: Path, force_overwrite: bool = False) -> None:
+    """Download and save multi-node images.
+
+    Args:
+         download_url (str): URL to download
+         save_path (Path): Save destination url
+         force_overwrite (bool): Force to overwrite files
+
+    Raises:
+        AosProvError: If files exists and force_overwrite is false.
+    """
+    _create_downloads_directory()
+
+    node_files = [save_path / NODE0_IMAGE_FILENAME, save_path / NODE1_IMAGE_FILENAME]
+
+    for node_file in node_files:
+        if force_overwrite:
+            if os.path.exists(node_file):
+                os.remove(node_file)
+        elif node_file.exists():
+            raise AosProvError(f'Destination file {node_file} already exist. Delete it or download with -f key')
+
+    download_file_name = save_path / 'downloaded-multi-node-images.tar.gz'
+
+    with open(download_file_name, 'wb') as save_context:
+        response = requests.get(download_url, stream=True, timeout=REQUEST_TIMEOUT)
+        response.raise_for_status()
+
+        total_length = response.headers.get('content-length')
+
+        if total_length is None:  # no content length header
+            save_context.write(response.content)
+            return
+
+        with Progress() as progress:
+            task_id = progress.add_task('[cyan]Downloading...', total=int(total_length))
+            for received_data in response.iter_content(chunk_size=_SAVE_CHUNK):
+                progress.update(task_id, advance=len(received_data))
+                save_context.write(received_data)
+
+    with tarfile.open(download_file_name) as archive:
+        archive.extractall(save_path)  # noqa: S202
+
+    if os.path.exists(download_file_name):
+        os.remove(download_file_name)
```

## aos_prov/communication/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
```

## aos_prov/communication/cloud/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
```

## aos_prov/communication/cloud/cloud_api.py

 * *Ordering differences only*

```diff
@@ -1,183 +1,183 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-import sys
-from urllib.parse import urlencode
-
-import requests
-from aos_prov.utils.common import (
-    REQUEST_TIMEOUT,
-    print_error,
-    print_left,
-    print_message,
-    print_success,
-)
-from aos_prov.utils.errors import CloudAccessError, DeviceRegisterError
-from aos_prov.utils.user_credentials import UserCredentials
-
-if sys.version_info > (3, 9):
-    from importlib import resources as pkg_resources  # noqa: WPS433, WPS440
-else:
-    import importlib_resources as pkg_resources  # noqa: WPS433, WPS440
-
-DEFAULT_REGISTER_HOST = 'aoscloud.io'
-DEFAULT_REGISTER_PORT = 10000
-
-
-class CloudAPI:
-    FILES_DIR = 'aos_prov'
-    ROOT_CA_CERT_FILENAME = 'files/1rootCA.crt'
-    REGISTER_URI_TPL = 'https://{}:{}/api/v1/units/provisioning/'
-    USER_ME_URI_TPL = 'https://{}:{}/api/v1/users/me/'
-    UNIT_STATUS_URL = 'https://{}:{}/api/v1/units/?{}'
-    FIND_UNIT_TPL = 'https://{}:{}/api/v1/units/?{}'
-    LINK_TO_THE_UNIT_ON_CLOUD_TPL = 'https://{}/oem/units/{}'
-
-    def __init__(self, user_credentials: UserCredentials, cloud_api_port: int = DEFAULT_REGISTER_PORT):
-        self._cloud_api_host = user_credentials.cloud_url
-        self._cloud_api_port = cloud_api_port if cloud_api_port else DEFAULT_REGISTER_PORT
-        self._user_credentials = user_credentials
-
-    def check_cloud_access(self):
-        """Check user access on the cloud and his role is OEM.
-
-        Raises:
-            CloudAccessError: If user haven't access to the cloud or his role is not OEM.
-        """
-        try:
-            url = self.USER_ME_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
-            server_certificate = pkg_resources.files(self.FILES_DIR) / self.ROOT_CA_CERT_FILENAME
-            with pkg_resources.as_file(server_certificate) as server_certificate_path:
-                with self._user_credentials.user_credentials as temp_creds:
-                    resp = requests.get(
-                        url,
-                        verify=server_certificate_path,
-                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name),
-                        timeout=REQUEST_TIMEOUT,
-                    )
-
-                if resp.status_code != 200:  # noqa: WPS432
-                    print_message('[red]Received not HTTP 200 response. ' + str(resp.text))
-                    raise CloudAccessError('You do not have access to the cloud!')
-
-                user_info = resp.json()
-                if user_info['role'] != 'oem':
-                    print_message(f'[red]invalid user role: {resp.text}')
-                    raise CloudAccessError('You should use OEM account!')
-
-            print_left('Operation will be executed on domain:')
-            print_success(self._cloud_api_host)
-            print_left('OEM:')
-            print_success(user_info['oem']['title'])
-            print_left('user:')
-            print_success(user_info['username'])
-        except ConnectionError as exc:
-            raise CloudAccessError('Failed to connect to the cloud with error: ' + str(exc)) from exc
-        except (requests.exceptions.RequestException, ValueError, OSError) as exc:
-            raise CloudAccessError('Failed to connect to the cloud with error: ' + str(exc)) from exc
-
-    def register_device(self, payload):
-        """Register device in cloud.
-
-        Args:
-            payload: Payload to register Unit
-
-        Raises:
-            DeviceRegisterError: Failed to register unit.
-
-        Returns:
-            registered metadata from Cloud
-        """
-        print_message('Registering the unit ...')
-        end_point = self.REGISTER_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
-
-        try:
-            server_certificate = pkg_resources.files(self.FILES_DIR) / self.ROOT_CA_CERT_FILENAME
-            with pkg_resources.as_file(server_certificate) as server_certificate_path:
-                with self._user_credentials.user_credentials as temp_creds:
-                    ret = requests.post(
-                        end_point,
-                        json=payload,
-                        verify=server_certificate_path,
-                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name),
-                        timeout=REQUEST_TIMEOUT,
-                    )
-
-                    if ret.status_code == 400:  # noqa: WPS432
-                        try:  # noqa: WPS505
-                            try:  # noqa: WPS505
-                                answer = ret.json()['non_field_errors'][0]
-                                print_error(f'Registration error: {answer}')
-                            except Exception:  # noqa: S110
-                                pass  # noqa: WPS420
-
-                        except UnicodeDecodeError:
-                            pass  # noqa: WPS420
-                    ret.raise_for_status()
-                    response = ret.json()
-        except (requests.exceptions.RequestException, ValueError, OSError) as exc:
-            raise DeviceRegisterError('Failed to register unit.') from exc
-
-        return response
-
-    def check_unit_is_not_provisioned(self, system_uid):
-        print_message("Getting unit's status on the cloud ...")
-        try:
-            end_point = self.UNIT_STATUS_URL.format(
-                self._cloud_api_host,
-                self._cloud_api_port,
-                urlencode({'system_uid': system_uid}),
-            )
-            server_certificate = pkg_resources.files(self.FILES_DIR) / self.ROOT_CA_CERT_FILENAME
-            with pkg_resources.as_file(server_certificate) as server_certificate_path:
-                with self._user_credentials.user_credentials as temp_creds:
-                    response = requests.get(
-                        end_point,
-                        verify=server_certificate_path,
-                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name),
-                        timeout=REQUEST_TIMEOUT,
-                    )
-
-        except (requests.exceptions.RequestException, ValueError, OSError) as exc:
-            raise DeviceRegisterError('Failed to HTTP GET: ', exc) from exc
-
-        response_json = response.json()
-
-        if response_json.get('results') is None or response_json.get('count') is None:
-            raise DeviceRegisterError('Invalid answer from the cloud. Please update current library')
-
-        if response_json.get('count') == 0:
-            # There is no such unit on the cloud
-            return
-
-        status = response_json.get('results', [{}])[0].get('status')
-        if status is None:
-            return
-
-        if status != 'new':
-            raise DeviceRegisterError(f'Unit is in status "{status}". Please do deprovisioning first.')
-
-    def get_unit_link_by_system_uid(self, system_uid):
-        end_point = self.FIND_UNIT_TPL.format(
-            self._cloud_api_host,
-            self._cloud_api_port,
-            urlencode({'system_uid': system_uid}),
-        )
-        try:
-            server_certificate = pkg_resources.files(self.FILES_DIR) / self.ROOT_CA_CERT_FILENAME
-            with pkg_resources.as_file(server_certificate) as server_certificate_path:
-                with self._user_credentials.user_credentials as temp_creds:
-                    response = requests.get(
-                        end_point,
-                        verify=server_certificate_path,
-                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name),
-                        timeout=REQUEST_TIMEOUT,
-                    )
-            unit_id = response.json()['results'][0]['id']
-            unit_domain = self._cloud_api_host
-            if not unit_domain.startswith('oem.'):
-                unit_domain = f'oem.{unit_domain}'
-            return self.LINK_TO_THE_UNIT_ON_CLOUD_TPL.format(unit_domain, unit_id)
-        except Exception:
-            return None
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+import sys
+from urllib.parse import urlencode
+
+import requests
+from aos_prov.utils.common import (
+    REQUEST_TIMEOUT,
+    print_error,
+    print_left,
+    print_message,
+    print_success,
+)
+from aos_prov.utils.errors import CloudAccessError, DeviceRegisterError
+from aos_prov.utils.user_credentials import UserCredentials
+
+if sys.version_info > (3, 9):
+    from importlib import resources as pkg_resources  # noqa: WPS433, WPS440
+else:
+    import importlib_resources as pkg_resources  # noqa: WPS433, WPS440
+
+DEFAULT_REGISTER_HOST = 'aoscloud.io'
+DEFAULT_REGISTER_PORT = 10000
+
+
+class CloudAPI:
+    FILES_DIR = 'aos_prov'
+    ROOT_CA_CERT_FILENAME = 'files/1rootCA.crt'
+    REGISTER_URI_TPL = 'https://{}:{}/api/v1/units/provisioning/'
+    USER_ME_URI_TPL = 'https://{}:{}/api/v1/users/me/'
+    UNIT_STATUS_URL = 'https://{}:{}/api/v1/units/?{}'
+    FIND_UNIT_TPL = 'https://{}:{}/api/v1/units/?{}'
+    LINK_TO_THE_UNIT_ON_CLOUD_TPL = 'https://{}/oem/units/{}'
+
+    def __init__(self, user_credentials: UserCredentials, cloud_api_port: int = DEFAULT_REGISTER_PORT):
+        self._cloud_api_host = user_credentials.cloud_url
+        self._cloud_api_port = cloud_api_port if cloud_api_port else DEFAULT_REGISTER_PORT
+        self._user_credentials = user_credentials
+
+    def check_cloud_access(self):
+        """Check user access on the cloud and his role is OEM.
+
+        Raises:
+            CloudAccessError: If user haven't access to the cloud or his role is not OEM.
+        """
+        try:
+            url = self.USER_ME_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
+            server_certificate = pkg_resources.files(self.FILES_DIR) / self.ROOT_CA_CERT_FILENAME
+            with pkg_resources.as_file(server_certificate) as server_certificate_path:
+                with self._user_credentials.user_credentials as temp_creds:
+                    resp = requests.get(
+                        url,
+                        verify=server_certificate_path,
+                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name),
+                        timeout=REQUEST_TIMEOUT,
+                    )
+
+                if resp.status_code != 200:  # noqa: WPS432
+                    print_message('[red]Received not HTTP 200 response. ' + str(resp.text))
+                    raise CloudAccessError('You do not have access to the cloud!')
+
+                user_info = resp.json()
+                if user_info['role'] != 'oem':
+                    print_message(f'[red]invalid user role: {resp.text}')
+                    raise CloudAccessError('You should use OEM account!')
+
+            print_left('Operation will be executed on domain:')
+            print_success(self._cloud_api_host)
+            print_left('OEM:')
+            print_success(user_info['oem']['title'])
+            print_left('user:')
+            print_success(user_info['username'])
+        except ConnectionError as exc:
+            raise CloudAccessError('Failed to connect to the cloud with error: ' + str(exc)) from exc
+        except (requests.exceptions.RequestException, ValueError, OSError) as exc:
+            raise CloudAccessError('Failed to connect to the cloud with error: ' + str(exc)) from exc
+
+    def register_device(self, payload):
+        """Register device in cloud.
+
+        Args:
+            payload: Payload to register Unit
+
+        Raises:
+            DeviceRegisterError: Failed to register unit.
+
+        Returns:
+            registered metadata from Cloud
+        """
+        print_message('Registering the unit ...')
+        end_point = self.REGISTER_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
+
+        try:
+            server_certificate = pkg_resources.files(self.FILES_DIR) / self.ROOT_CA_CERT_FILENAME
+            with pkg_resources.as_file(server_certificate) as server_certificate_path:
+                with self._user_credentials.user_credentials as temp_creds:
+                    ret = requests.post(
+                        end_point,
+                        json=payload,
+                        verify=server_certificate_path,
+                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name),
+                        timeout=REQUEST_TIMEOUT,
+                    )
+
+                    if ret.status_code == 400:  # noqa: WPS432
+                        try:  # noqa: WPS505
+                            try:  # noqa: WPS505
+                                answer = ret.json()['non_field_errors'][0]
+                                print_error(f'Registration error: {answer}')
+                            except Exception:  # noqa: S110
+                                pass  # noqa: WPS420
+
+                        except UnicodeDecodeError:
+                            pass  # noqa: WPS420
+                    ret.raise_for_status()
+                    response = ret.json()
+        except (requests.exceptions.RequestException, ValueError, OSError) as exc:
+            raise DeviceRegisterError('Failed to register unit.') from exc
+
+        return response
+
+    def check_unit_is_not_provisioned(self, system_uid):
+        print_message("Getting unit's status on the cloud ...")
+        try:
+            end_point = self.UNIT_STATUS_URL.format(
+                self._cloud_api_host,
+                self._cloud_api_port,
+                urlencode({'system_uid': system_uid}),
+            )
+            server_certificate = pkg_resources.files(self.FILES_DIR) / self.ROOT_CA_CERT_FILENAME
+            with pkg_resources.as_file(server_certificate) as server_certificate_path:
+                with self._user_credentials.user_credentials as temp_creds:
+                    response = requests.get(
+                        end_point,
+                        verify=server_certificate_path,
+                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name),
+                        timeout=REQUEST_TIMEOUT,
+                    )
+
+        except (requests.exceptions.RequestException, ValueError, OSError) as exc:
+            raise DeviceRegisterError('Failed to HTTP GET: ', exc) from exc
+
+        response_json = response.json()
+
+        if response_json.get('results') is None or response_json.get('count') is None:
+            raise DeviceRegisterError('Invalid answer from the cloud. Please update current library')
+
+        if response_json.get('count') == 0:
+            # There is no such unit on the cloud
+            return
+
+        status = response_json.get('results', [{}])[0].get('status')
+        if status is None:
+            return
+
+        if status != 'new':
+            raise DeviceRegisterError(f'Unit is in status "{status}". Please do deprovisioning first.')
+
+    def get_unit_link_by_system_uid(self, system_uid):
+        end_point = self.FIND_UNIT_TPL.format(
+            self._cloud_api_host,
+            self._cloud_api_port,
+            urlencode({'system_uid': system_uid}),
+        )
+        try:
+            server_certificate = pkg_resources.files(self.FILES_DIR) / self.ROOT_CA_CERT_FILENAME
+            with pkg_resources.as_file(server_certificate) as server_certificate_path:
+                with self._user_credentials.user_credentials as temp_creds:
+                    response = requests.get(
+                        end_point,
+                        verify=server_certificate_path,
+                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name),
+                        timeout=REQUEST_TIMEOUT,
+                    )
+            unit_id = response.json()['results'][0]['id']
+            unit_domain = self._cloud_api_host
+            if not unit_domain.startswith('oem.'):
+                unit_domain = f'oem.{unit_domain}'
+            return self.LINK_TO_THE_UNIT_ON_CLOUD_TPL.format(unit_domain, unit_id)
+        except Exception:
+            return None
```

## aos_prov/communication/unit/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
```

## aos_prov/communication/unit/v0/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
```

## aos_prov/communication/unit/v1/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
```

## aos_prov/communication/unit/v2/unit_communication_v2.py

 * *Ordering differences only*

```diff
@@ -1,174 +1,174 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-import time
-from contextlib import contextmanager
-
-import grpc
-from aos_prov.communication.unit.v2.generated import (
-    iamanagercommon_pb2 as iam_manager_common,
-)
-from aos_prov.communication.unit.v2.generated import (
-    iamanagerprotected_pb2 as iam_manager,
-)
-from aos_prov.communication.unit.v2.generated import (
-    iamanagerprotected_pb2_grpc as api_iam_manager_grpc,
-)
-from aos_prov.communication.unit.v2.generated import (
-    iamanagerpublic_pb2_grpc as iam_manager_public_grpc,
-)
-from aos_prov.utils.common import print_done, print_left, print_message, print_success
-from aos_prov.utils.errors import GrpcUnimplemented, UnitError
-from aos_prov.utils.unit_certificate import UnitCertificate
-from google.protobuf import empty_pb2
-
-UNIT_DEFAULT_PORT = 8089
-_MAX_PORT = 65535
-
-
-class UnitCommunicationV2:
-    def __init__(self, address: str = 'localhost:8089', set_users=True):
-        self._need_set_users = set_users
-
-        if not address:
-            address = 'localhost:8089'
-
-        parts = address.split(':')
-        if len(parts) == 2:
-            try:
-                port = int(parts[1])
-                if port not in range(1, _MAX_PORT):
-                    raise UnitError('Unit port is invalid')
-            except (ValueError, UnitError) as exc:
-                raise UnitError('Unit port is invalid') from exc
-        else:
-            address = address + ':' + str(UNIT_DEFAULT_PORT)
-        self._unit_address = address
-
-    @property
-    def need_set_users(self):
-        return self._need_set_users
-
-    @need_set_users.setter
-    def need_set_users(self, set_users):
-        self._need_set_users = set_users
-
-    @contextmanager
-    def unit_stub(self, catch_inactive=False, wait_for_close=False):
-        try:
-            with grpc.insecure_channel(self._unit_address) as channel:
-                stub = api_iam_manager_grpc.IAMProtectedServiceStub(channel)
-                if wait_for_close:
-                    def _stop_wait(state):  # noqa: WPS430
-                        if state is grpc.ChannelConnectivity.SHUTDOWN:
-                            channel.unsubscribe(_stop_wait)
-                            return
-                    channel.subscribe(_stop_wait, try_to_connect=False)
-                yield stub
-
-        except grpc.RpcError as exc:
-            e_code = exc.code()
-            e_detail = exc.details()
-            if catch_inactive and not (e_code == grpc.StatusCode.UNAVAILABLE.value and e_detail == 'Socket closed'):
-                return
-            if wait_for_close and (e_code == grpc.StatusCode.UNKNOWN.value and e_detail == 'Stream removed'):
-                return
-            raise UnitError(f'FAILED! Error occurred: \n{e_code}: {e_detail}') from exc
-
-    @contextmanager
-    def unit_public_stub(self):
-        try:
-            with grpc.insecure_channel(self._unit_address) as channel:
-                stub = iam_manager_public_grpc.IAMPublicServiceStub(channel)
-                yield stub
-
-        except grpc.RpcError as exc:
-            e_code = exc.code()
-            e_detail = exc.details()
-            if e_code.value == grpc.StatusCode.UNIMPLEMENTED.value:
-                raise GrpcUnimplemented(f'Protocol V3 is not supported: \n{e_code}: {e_detail}') from exc
-            raise UnitError(f'FAILED! Error occurred: \n{e_code}: {e_detail}') from exc
-
-    def get_protocol_version(self) -> int:
-        with self.unit_public_stub() as stub:
-            print_left('Getting protocol version...')
-            response = stub.GetAPIVersion(empty_pb2.Empty())
-            print_success(str(response.version))
-            return int(response.version)
-
-    def get_system_info(self) -> (str, str):
-        with self.unit_public_stub() as stub:
-            print_left('Getting System Info...')
-            response = stub.GetSystemInfo(empty_pb2.Empty())
-            print_done()
-            print_left('System ID:')
-            print_success(response.system_id)
-            print_left('Model name:')
-            print_success(response.board_model)
-            return response.system_id, response.board_model
-
-    def clear(self, certificate_type: str) -> None:
-        with self.unit_stub() as stub:
-            print_left('Clear certificate: ' + certificate_type)
-            response = stub.Clear(iam_manager.ClearRequest(type=certificate_type))
-            print_done()
-            return response
-
-    def set_cert_owner(self, certificate_type: str, password: str) -> None:
-        with self.unit_stub() as stub:
-            print_left('Set owner: ' + certificate_type)
-            response = stub.SetOwner(iam_manager.SetOwnerRequest(type=certificate_type, password=password))
-            print_done()
-            return response
-
-    def get_cert_types(self) -> [str]:
-        with self.unit_public_stub() as stub:
-            print_left('Getting certificate types to renew')
-            response = stub.GetCertTypes(empty_pb2.Empty())
-            print_done()
-            return response.types
-
-    def create_keys(self, cert_type: str, password: str) -> UnitCertificate:
-        with self.unit_stub() as stub:
-            print_left('Generating key type: ' + cert_type)
-            response = stub.CreateKey(iam_manager.CreateKeyRequest(type=cert_type, password=password))
-            user_creds = UnitCertificate()
-            user_creds.cert_type = response.type
-            user_creds.csr = response.csr
-            print_done()
-            return user_creds
-
-    def apply_certificate(self, unit_cert: UnitCertificate):
-        with self.unit_stub() as stub:
-            print_left('Applying type: ' + unit_cert.cert_type)
-            stub.ApplyCert(iam_manager.ApplyCertRequest(type=unit_cert.cert_type, cert=unit_cert.certificate))
-            print_done()
-
-    def set_users(self, users: [str]):
-        with self.unit_stub() as stub:
-            print_left('Setting users...')
-            stub.SetUsers(iam_manager_common.Users(users=users))
-            print_done()
-
-    def encrypt_disk(self, password: str):
-        print_left('Starting disk encryption...')
-        with self.unit_stub(wait_for_close=True) as stub:
-            stub.EncryptDisk(iam_manager.EncryptDiskRequest(password=password))
-            print_done()
-
-    def finish_provisioning(self):
-        with self.unit_stub(True) as stub:
-            print_left('Finishing provisioning')
-            stub.FinishProvisioning(empty_pb2.Empty())
-            print_done()
-
-    def wait_for_connection(self):
-        try:
-            print_message('Sleep for 5 seconds...')
-            time.sleep(5)
-            print_message('Waiting for Unit reboot...')
-            grpc.channel_ready_future(grpc.insecure_channel(self._unit_address)).result(timeout=300)  # noqa: WPS432
-            print_message('Unit is online')
-        except grpc.FutureTimeoutError as exc:
-            raise UnitError('Unit did not go online') from exc
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+import time
+from contextlib import contextmanager
+
+import grpc
+from aos_prov.communication.unit.v2.generated import (
+    iamanagercommon_pb2 as iam_manager_common,
+)
+from aos_prov.communication.unit.v2.generated import (
+    iamanagerprotected_pb2 as iam_manager,
+)
+from aos_prov.communication.unit.v2.generated import (
+    iamanagerprotected_pb2_grpc as api_iam_manager_grpc,
+)
+from aos_prov.communication.unit.v2.generated import (
+    iamanagerpublic_pb2_grpc as iam_manager_public_grpc,
+)
+from aos_prov.utils.common import print_done, print_left, print_message, print_success
+from aos_prov.utils.errors import GrpcUnimplemented, UnitError
+from aos_prov.utils.unit_certificate import UnitCertificate
+from google.protobuf import empty_pb2
+
+UNIT_DEFAULT_PORT = 8089
+_MAX_PORT = 65535
+
+
+class UnitCommunicationV2:
+    def __init__(self, address: str = 'localhost:8089', set_users=True):
+        self._need_set_users = set_users
+
+        if not address:
+            address = 'localhost:8089'
+
+        parts = address.split(':')
+        if len(parts) == 2:
+            try:
+                port = int(parts[1])
+                if port not in range(1, _MAX_PORT):
+                    raise UnitError('Unit port is invalid')
+            except (ValueError, UnitError) as exc:
+                raise UnitError('Unit port is invalid') from exc
+        else:
+            address = address + ':' + str(UNIT_DEFAULT_PORT)
+        self._unit_address = address
+
+    @property
+    def need_set_users(self):
+        return self._need_set_users
+
+    @need_set_users.setter
+    def need_set_users(self, set_users):
+        self._need_set_users = set_users
+
+    @contextmanager
+    def unit_stub(self, catch_inactive=False, wait_for_close=False):
+        try:
+            with grpc.insecure_channel(self._unit_address) as channel:
+                stub = api_iam_manager_grpc.IAMProtectedServiceStub(channel)
+                if wait_for_close:
+                    def _stop_wait(state):  # noqa: WPS430
+                        if state is grpc.ChannelConnectivity.SHUTDOWN:
+                            channel.unsubscribe(_stop_wait)
+                            return
+                    channel.subscribe(_stop_wait, try_to_connect=False)
+                yield stub
+
+        except grpc.RpcError as exc:
+            e_code = exc.code()
+            e_detail = exc.details()
+            if catch_inactive and not (e_code == grpc.StatusCode.UNAVAILABLE.value and e_detail == 'Socket closed'):
+                return
+            if wait_for_close and (e_code == grpc.StatusCode.UNKNOWN.value and e_detail == 'Stream removed'):
+                return
+            raise UnitError(f'FAILED! Error occurred: \n{e_code}: {e_detail}') from exc
+
+    @contextmanager
+    def unit_public_stub(self):
+        try:
+            with grpc.insecure_channel(self._unit_address) as channel:
+                stub = iam_manager_public_grpc.IAMPublicServiceStub(channel)
+                yield stub
+
+        except grpc.RpcError as exc:
+            e_code = exc.code()
+            e_detail = exc.details()
+            if e_code.value == grpc.StatusCode.UNIMPLEMENTED.value:
+                raise GrpcUnimplemented(f'Protocol V3 is not supported: \n{e_code}: {e_detail}') from exc
+            raise UnitError(f'FAILED! Error occurred: \n{e_code}: {e_detail}') from exc
+
+    def get_protocol_version(self) -> int:
+        with self.unit_public_stub() as stub:
+            print_left('Getting protocol version...')
+            response = stub.GetAPIVersion(empty_pb2.Empty())
+            print_success(str(response.version))
+            return int(response.version)
+
+    def get_system_info(self) -> (str, str):
+        with self.unit_public_stub() as stub:
+            print_left('Getting System Info...')
+            response = stub.GetSystemInfo(empty_pb2.Empty())
+            print_done()
+            print_left('System ID:')
+            print_success(response.system_id)
+            print_left('Model name:')
+            print_success(response.board_model)
+            return response.system_id, response.board_model
+
+    def clear(self, certificate_type: str) -> None:
+        with self.unit_stub() as stub:
+            print_left('Clear certificate: ' + certificate_type)
+            response = stub.Clear(iam_manager.ClearRequest(type=certificate_type))
+            print_done()
+            return response
+
+    def set_cert_owner(self, certificate_type: str, password: str) -> None:
+        with self.unit_stub() as stub:
+            print_left('Set owner: ' + certificate_type)
+            response = stub.SetOwner(iam_manager.SetOwnerRequest(type=certificate_type, password=password))
+            print_done()
+            return response
+
+    def get_cert_types(self) -> [str]:
+        with self.unit_public_stub() as stub:
+            print_left('Getting certificate types to renew')
+            response = stub.GetCertTypes(empty_pb2.Empty())
+            print_done()
+            return response.types
+
+    def create_keys(self, cert_type: str, password: str) -> UnitCertificate:
+        with self.unit_stub() as stub:
+            print_left('Generating key type: ' + cert_type)
+            response = stub.CreateKey(iam_manager.CreateKeyRequest(type=cert_type, password=password))
+            user_creds = UnitCertificate()
+            user_creds.cert_type = response.type
+            user_creds.csr = response.csr
+            print_done()
+            return user_creds
+
+    def apply_certificate(self, unit_cert: UnitCertificate):
+        with self.unit_stub() as stub:
+            print_left('Applying type: ' + unit_cert.cert_type)
+            stub.ApplyCert(iam_manager.ApplyCertRequest(type=unit_cert.cert_type, cert=unit_cert.certificate))
+            print_done()
+
+    def set_users(self, users: [str]):
+        with self.unit_stub() as stub:
+            print_left('Setting users...')
+            stub.SetUsers(iam_manager_common.Users(users=users))
+            print_done()
+
+    def encrypt_disk(self, password: str):
+        print_left('Starting disk encryption...')
+        with self.unit_stub(wait_for_close=True) as stub:
+            stub.EncryptDisk(iam_manager.EncryptDiskRequest(password=password))
+            print_done()
+
+    def finish_provisioning(self):
+        with self.unit_stub(True) as stub:
+            print_left('Finishing provisioning')
+            stub.FinishProvisioning(empty_pb2.Empty())
+            print_done()
+
+    def wait_for_connection(self):
+        try:
+            print_message('Sleep for 5 seconds...')
+            time.sleep(5)
+            print_message('Waiting for Unit reboot...')
+            grpc.channel_ready_future(grpc.insecure_channel(self._unit_address)).result(timeout=300)  # noqa: WPS432
+            print_message('Unit is online')
+        except grpc.FutureTimeoutError as exc:
+            raise UnitError('Unit did not go online') from exc
```

## aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py

 * *Ordering differences only*

```diff
@@ -1,160 +1,160 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: iamanager/v2/iamanagercommon.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='iamanager/v2/iamanagercommon.proto',
-  package='iamanager.v2',
-  syntax='proto3',
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\"iamanager/v2/iamanagercommon.proto\x12\x0ciamanager.v2\"\x82\x01\n\x0bPermissions\x12?\n\x0bpermissions\x18\x01 \x03(\x0b\x32*.iamanager.v2.Permissions.PermissionsEntry\x1a\x32\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x16\n\x05Users\x12\r\n\x05users\x18\x01 \x03(\tb\x06proto3'
-)
-
-
-
-
-_PERMISSIONS_PERMISSIONSENTRY = _descriptor.Descriptor(
-  name='PermissionsEntry',
-  full_name='iamanager.v2.Permissions.PermissionsEntry',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='key', full_name='iamanager.v2.Permissions.PermissionsEntry.key', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='value', full_name='iamanager.v2.Permissions.PermissionsEntry.value', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=b'8\001',
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=133,
-  serialized_end=183,
-)
-
-_PERMISSIONS = _descriptor.Descriptor(
-  name='Permissions',
-  full_name='iamanager.v2.Permissions',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='permissions', full_name='iamanager.v2.Permissions.permissions', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[_PERMISSIONS_PERMISSIONSENTRY, ],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=53,
-  serialized_end=183,
-)
-
-
-_USERS = _descriptor.Descriptor(
-  name='Users',
-  full_name='iamanager.v2.Users',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='users', full_name='iamanager.v2.Users.users', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=185,
-  serialized_end=207,
-)
-
-_PERMISSIONS_PERMISSIONSENTRY.containing_type = _PERMISSIONS
-_PERMISSIONS.fields_by_name['permissions'].message_type = _PERMISSIONS_PERMISSIONSENTRY
-DESCRIPTOR.message_types_by_name['Permissions'] = _PERMISSIONS
-DESCRIPTOR.message_types_by_name['Users'] = _USERS
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-Permissions = _reflection.GeneratedProtocolMessageType('Permissions', (_message.Message,), {
-
-  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _PERMISSIONS_PERMISSIONSENTRY,
-    '__module__' : 'iamanager.v2.iamanagercommon_pb2'
-    # @@protoc_insertion_point(class_scope:iamanager.v2.Permissions.PermissionsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _PERMISSIONS,
-  '__module__' : 'iamanager.v2.iamanagercommon_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.Permissions)
-  })
-_sym_db.RegisterMessage(Permissions)
-_sym_db.RegisterMessage(Permissions.PermissionsEntry)
-
-Users = _reflection.GeneratedProtocolMessageType('Users', (_message.Message,), {
-  'DESCRIPTOR' : _USERS,
-  '__module__' : 'iamanager.v2.iamanagercommon_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.Users)
-  })
-_sym_db.RegisterMessage(Users)
-
-
-_PERMISSIONS_PERMISSIONSENTRY._options = None
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: iamanager/v2/iamanagercommon.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='iamanager/v2/iamanagercommon.proto',
+  package='iamanager.v2',
+  syntax='proto3',
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_pb=b'\n\"iamanager/v2/iamanagercommon.proto\x12\x0ciamanager.v2\"\x82\x01\n\x0bPermissions\x12?\n\x0bpermissions\x18\x01 \x03(\x0b\x32*.iamanager.v2.Permissions.PermissionsEntry\x1a\x32\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x16\n\x05Users\x12\r\n\x05users\x18\x01 \x03(\tb\x06proto3'
+)
+
+
+
+
+_PERMISSIONS_PERMISSIONSENTRY = _descriptor.Descriptor(
+  name='PermissionsEntry',
+  full_name='iamanager.v2.Permissions.PermissionsEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='iamanager.v2.Permissions.PermissionsEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='iamanager.v2.Permissions.PermissionsEntry.value', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=133,
+  serialized_end=183,
+)
+
+_PERMISSIONS = _descriptor.Descriptor(
+  name='Permissions',
+  full_name='iamanager.v2.Permissions',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='permissions', full_name='iamanager.v2.Permissions.permissions', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_PERMISSIONS_PERMISSIONSENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=53,
+  serialized_end=183,
+)
+
+
+_USERS = _descriptor.Descriptor(
+  name='Users',
+  full_name='iamanager.v2.Users',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='users', full_name='iamanager.v2.Users.users', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=185,
+  serialized_end=207,
+)
+
+_PERMISSIONS_PERMISSIONSENTRY.containing_type = _PERMISSIONS
+_PERMISSIONS.fields_by_name['permissions'].message_type = _PERMISSIONS_PERMISSIONSENTRY
+DESCRIPTOR.message_types_by_name['Permissions'] = _PERMISSIONS
+DESCRIPTOR.message_types_by_name['Users'] = _USERS
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+Permissions = _reflection.GeneratedProtocolMessageType('Permissions', (_message.Message,), {
+
+  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _PERMISSIONS_PERMISSIONSENTRY,
+    '__module__' : 'iamanager.v2.iamanagercommon_pb2'
+    # @@protoc_insertion_point(class_scope:iamanager.v2.Permissions.PermissionsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _PERMISSIONS,
+  '__module__' : 'iamanager.v2.iamanagercommon_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.Permissions)
+  })
+_sym_db.RegisterMessage(Permissions)
+_sym_db.RegisterMessage(Permissions.PermissionsEntry)
+
+Users = _reflection.GeneratedProtocolMessageType('Users', (_message.Message,), {
+  'DESCRIPTOR' : _USERS,
+  '__module__' : 'iamanager.v2.iamanagercommon_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.Users)
+  })
+_sym_db.RegisterMessage(Users)
+
+
+_PERMISSIONS_PERMISSIONSENTRY._options = None
+# @@protoc_insertion_point(module_scope)
```

## aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
```

## aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py

 * *Ordering differences only*

```diff
@@ -1,633 +1,633 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: iamanager/v2/iamanagerprotected.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from aos_prov.communication.unit.v2.generated import (
-    iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2,
-)
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='iamanager/v2/iamanagerprotected.proto',
-  package='iamanager.v2',
-  syntax='proto3',
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n%iamanager/v2/iamanagerprotected.proto\x12\x0ciamanager.v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\"iamanager/v2/iamanagercommon.proto\"\x1c\n\x0c\x43learRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\"1\n\x0fSetOwnerRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"2\n\x10\x43reateKeyRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\".\n\x11\x43reateKeyResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0b\n\x03\x63sr\x18\x02 \x01(\t\".\n\x10\x41pplyCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x02 \x01(\t\"3\n\x11\x41pplyCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\"\xc7\x01\n\x16RegisterServiceRequest\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12J\n\x0bpermissions\x18\x02 \x03(\x0b\x32\x35.iamanager.v2.RegisterServiceRequest.PermissionsEntry\x1aM\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.iamanager.v2.Permissions:\x02\x38\x01\")\n\x17RegisterServiceResponse\x12\x0e\n\x06secret\x18\x01 \x01(\t\".\n\x18UnregisterServiceRequest\x12\x12\n\nservice_id\x18\x01 \x01(\t\"&\n\x12\x45ncryptDiskRequest\x12\x10\n\x08password\x18\x01 \x01(\t2\xc0\x05\n\x13IAMProtectedService\x12\x43\n\x08SetOwner\x12\x1d.iamanager.v2.SetOwnerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x05\x43lear\x12\x1a.iamanager.v2.ClearRequest\x1a\x16.google.protobuf.Empty\"\x00\x12N\n\tCreateKey\x12\x1e.iamanager.v2.CreateKeyRequest\x1a\x1f.iamanager.v2.CreateKeyResponse\"\x00\x12N\n\tApplyCert\x12\x1e.iamanager.v2.ApplyCertRequest\x1a\x1f.iamanager.v2.ApplyCertResponse\"\x00\x12I\n\x0b\x45ncryptDisk\x12 .iamanager.v2.EncryptDiskRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x39\n\x08SetUsers\x12\x13.iamanager.v2.Users\x1a\x16.google.protobuf.Empty\"\x00\x12`\n\x0fRegisterService\x12$.iamanager.v2.RegisterServiceRequest\x1a%.iamanager.v2.RegisterServiceResponse\"\x00\x12U\n\x11UnregisterService\x12&.iamanager.v2.UnregisterServiceRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3'
-  ,
-  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,iamanager_dot_v2_dot_iamanagercommon__pb2.DESCRIPTOR,])
-
-
-
-
-_CLEARREQUEST = _descriptor.Descriptor(
-  name='ClearRequest',
-  full_name='iamanager.v2.ClearRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.ClearRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=120,
-  serialized_end=148,
-)
-
-
-_SETOWNERREQUEST = _descriptor.Descriptor(
-  name='SetOwnerRequest',
-  full_name='iamanager.v2.SetOwnerRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.SetOwnerRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.v2.SetOwnerRequest.password', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=150,
-  serialized_end=199,
-)
-
-
-_CREATEKEYREQUEST = _descriptor.Descriptor(
-  name='CreateKeyRequest',
-  full_name='iamanager.v2.CreateKeyRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.CreateKeyRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.v2.CreateKeyRequest.password', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=201,
-  serialized_end=251,
-)
-
-
-_CREATEKEYRESPONSE = _descriptor.Descriptor(
-  name='CreateKeyResponse',
-  full_name='iamanager.v2.CreateKeyResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.CreateKeyResponse.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='csr', full_name='iamanager.v2.CreateKeyResponse.csr', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=253,
-  serialized_end=299,
-)
-
-
-_APPLYCERTREQUEST = _descriptor.Descriptor(
-  name='ApplyCertRequest',
-  full_name='iamanager.v2.ApplyCertRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.ApplyCertRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cert', full_name='iamanager.v2.ApplyCertRequest.cert', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=301,
-  serialized_end=347,
-)
-
-
-_APPLYCERTRESPONSE = _descriptor.Descriptor(
-  name='ApplyCertResponse',
-  full_name='iamanager.v2.ApplyCertResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.ApplyCertResponse.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cert_url', full_name='iamanager.v2.ApplyCertResponse.cert_url', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=349,
-  serialized_end=400,
-)
-
-
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY = _descriptor.Descriptor(
-  name='PermissionsEntry',
-  full_name='iamanager.v2.RegisterServiceRequest.PermissionsEntry',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='key', full_name='iamanager.v2.RegisterServiceRequest.PermissionsEntry.key', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='value', full_name='iamanager.v2.RegisterServiceRequest.PermissionsEntry.value', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=b'8\001',
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=525,
-  serialized_end=602,
-)
-
-_REGISTERSERVICEREQUEST = _descriptor.Descriptor(
-  name='RegisterServiceRequest',
-  full_name='iamanager.v2.RegisterServiceRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='service_id', full_name='iamanager.v2.RegisterServiceRequest.service_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='permissions', full_name='iamanager.v2.RegisterServiceRequest.permissions', index=1,
-      number=2, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[_REGISTERSERVICEREQUEST_PERMISSIONSENTRY, ],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=403,
-  serialized_end=602,
-)
-
-
-_REGISTERSERVICERESPONSE = _descriptor.Descriptor(
-  name='RegisterServiceResponse',
-  full_name='iamanager.v2.RegisterServiceResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='secret', full_name='iamanager.v2.RegisterServiceResponse.secret', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=604,
-  serialized_end=645,
-)
-
-
-_UNREGISTERSERVICEREQUEST = _descriptor.Descriptor(
-  name='UnregisterServiceRequest',
-  full_name='iamanager.v2.UnregisterServiceRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='service_id', full_name='iamanager.v2.UnregisterServiceRequest.service_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=647,
-  serialized_end=693,
-)
-
-
-_ENCRYPTDISKREQUEST = _descriptor.Descriptor(
-  name='EncryptDiskRequest',
-  full_name='iamanager.v2.EncryptDiskRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.v2.EncryptDiskRequest.password', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=695,
-  serialized_end=733,
-)
-
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY.fields_by_name['value'].message_type = iamanager_dot_v2_dot_iamanagercommon__pb2._PERMISSIONS
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY.containing_type = _REGISTERSERVICEREQUEST
-_REGISTERSERVICEREQUEST.fields_by_name['permissions'].message_type = _REGISTERSERVICEREQUEST_PERMISSIONSENTRY
-DESCRIPTOR.message_types_by_name['ClearRequest'] = _CLEARREQUEST
-DESCRIPTOR.message_types_by_name['SetOwnerRequest'] = _SETOWNERREQUEST
-DESCRIPTOR.message_types_by_name['CreateKeyRequest'] = _CREATEKEYREQUEST
-DESCRIPTOR.message_types_by_name['CreateKeyResponse'] = _CREATEKEYRESPONSE
-DESCRIPTOR.message_types_by_name['ApplyCertRequest'] = _APPLYCERTREQUEST
-DESCRIPTOR.message_types_by_name['ApplyCertResponse'] = _APPLYCERTRESPONSE
-DESCRIPTOR.message_types_by_name['RegisterServiceRequest'] = _REGISTERSERVICEREQUEST
-DESCRIPTOR.message_types_by_name['RegisterServiceResponse'] = _REGISTERSERVICERESPONSE
-DESCRIPTOR.message_types_by_name['UnregisterServiceRequest'] = _UNREGISTERSERVICEREQUEST
-DESCRIPTOR.message_types_by_name['EncryptDiskRequest'] = _ENCRYPTDISKREQUEST
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-ClearRequest = _reflection.GeneratedProtocolMessageType('ClearRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CLEARREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.ClearRequest)
-  })
-_sym_db.RegisterMessage(ClearRequest)
-
-SetOwnerRequest = _reflection.GeneratedProtocolMessageType('SetOwnerRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SETOWNERREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.SetOwnerRequest)
-  })
-_sym_db.RegisterMessage(SetOwnerRequest)
-
-CreateKeyRequest = _reflection.GeneratedProtocolMessageType('CreateKeyRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.CreateKeyRequest)
-  })
-_sym_db.RegisterMessage(CreateKeyRequest)
-
-CreateKeyResponse = _reflection.GeneratedProtocolMessageType('CreateKeyResponse', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYRESPONSE,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.CreateKeyResponse)
-  })
-_sym_db.RegisterMessage(CreateKeyResponse)
-
-ApplyCertRequest = _reflection.GeneratedProtocolMessageType('ApplyCertRequest', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.ApplyCertRequest)
-  })
-_sym_db.RegisterMessage(ApplyCertRequest)
-
-ApplyCertResponse = _reflection.GeneratedProtocolMessageType('ApplyCertResponse', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTRESPONSE,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.ApplyCertResponse)
-  })
-_sym_db.RegisterMessage(ApplyCertResponse)
-
-RegisterServiceRequest = _reflection.GeneratedProtocolMessageType('RegisterServiceRequest', (_message.Message,), {
-
-  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _REGISTERSERVICEREQUEST_PERMISSIONSENTRY,
-    '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-    # @@protoc_insertion_point(class_scope:iamanager.v2.RegisterServiceRequest.PermissionsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _REGISTERSERVICEREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.RegisterServiceRequest)
-  })
-_sym_db.RegisterMessage(RegisterServiceRequest)
-_sym_db.RegisterMessage(RegisterServiceRequest.PermissionsEntry)
-
-RegisterServiceResponse = _reflection.GeneratedProtocolMessageType('RegisterServiceResponse', (_message.Message,), {
-  'DESCRIPTOR' : _REGISTERSERVICERESPONSE,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.RegisterServiceResponse)
-  })
-_sym_db.RegisterMessage(RegisterServiceResponse)
-
-UnregisterServiceRequest = _reflection.GeneratedProtocolMessageType('UnregisterServiceRequest', (_message.Message,), {
-  'DESCRIPTOR' : _UNREGISTERSERVICEREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.UnregisterServiceRequest)
-  })
-_sym_db.RegisterMessage(UnregisterServiceRequest)
-
-EncryptDiskRequest = _reflection.GeneratedProtocolMessageType('EncryptDiskRequest', (_message.Message,), {
-  'DESCRIPTOR' : _ENCRYPTDISKREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.EncryptDiskRequest)
-  })
-_sym_db.RegisterMessage(EncryptDiskRequest)
-
-
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY._options = None
-
-_IAMPROTECTEDSERVICE = _descriptor.ServiceDescriptor(
-  name='IAMProtectedService',
-  full_name='iamanager.v2.IAMProtectedService',
-  file=DESCRIPTOR,
-  index=0,
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_start=736,
-  serialized_end=1440,
-  methods=[
-  _descriptor.MethodDescriptor(
-    name='SetOwner',
-    full_name='iamanager.v2.IAMProtectedService.SetOwner',
-    index=0,
-    containing_service=None,
-    input_type=_SETOWNERREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='Clear',
-    full_name='iamanager.v2.IAMProtectedService.Clear',
-    index=1,
-    containing_service=None,
-    input_type=_CLEARREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='CreateKey',
-    full_name='iamanager.v2.IAMProtectedService.CreateKey',
-    index=2,
-    containing_service=None,
-    input_type=_CREATEKEYREQUEST,
-    output_type=_CREATEKEYRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='ApplyCert',
-    full_name='iamanager.v2.IAMProtectedService.ApplyCert',
-    index=3,
-    containing_service=None,
-    input_type=_APPLYCERTREQUEST,
-    output_type=_APPLYCERTRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='EncryptDisk',
-    full_name='iamanager.v2.IAMProtectedService.EncryptDisk',
-    index=4,
-    containing_service=None,
-    input_type=_ENCRYPTDISKREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='FinishProvisioning',
-    full_name='iamanager.v2.IAMProtectedService.FinishProvisioning',
-    index=5,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='SetUsers',
-    full_name='iamanager.v2.IAMProtectedService.SetUsers',
-    index=6,
-    containing_service=None,
-    input_type=iamanager_dot_v2_dot_iamanagercommon__pb2._USERS,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='RegisterService',
-    full_name='iamanager.v2.IAMProtectedService.RegisterService',
-    index=7,
-    containing_service=None,
-    input_type=_REGISTERSERVICEREQUEST,
-    output_type=_REGISTERSERVICERESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='UnregisterService',
-    full_name='iamanager.v2.IAMProtectedService.UnregisterService',
-    index=8,
-    containing_service=None,
-    input_type=_UNREGISTERSERVICEREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-])
-_sym_db.RegisterServiceDescriptor(_IAMPROTECTEDSERVICE)
-
-DESCRIPTOR.services_by_name['IAMProtectedService'] = _IAMPROTECTEDSERVICE
-
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: iamanager/v2/iamanagerprotected.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from aos_prov.communication.unit.v2.generated import (
+    iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2,
+)
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='iamanager/v2/iamanagerprotected.proto',
+  package='iamanager.v2',
+  syntax='proto3',
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_pb=b'\n%iamanager/v2/iamanagerprotected.proto\x12\x0ciamanager.v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\"iamanager/v2/iamanagercommon.proto\"\x1c\n\x0c\x43learRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\"1\n\x0fSetOwnerRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"2\n\x10\x43reateKeyRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\".\n\x11\x43reateKeyResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0b\n\x03\x63sr\x18\x02 \x01(\t\".\n\x10\x41pplyCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x02 \x01(\t\"3\n\x11\x41pplyCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\"\xc7\x01\n\x16RegisterServiceRequest\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12J\n\x0bpermissions\x18\x02 \x03(\x0b\x32\x35.iamanager.v2.RegisterServiceRequest.PermissionsEntry\x1aM\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.iamanager.v2.Permissions:\x02\x38\x01\")\n\x17RegisterServiceResponse\x12\x0e\n\x06secret\x18\x01 \x01(\t\".\n\x18UnregisterServiceRequest\x12\x12\n\nservice_id\x18\x01 \x01(\t\"&\n\x12\x45ncryptDiskRequest\x12\x10\n\x08password\x18\x01 \x01(\t2\xc0\x05\n\x13IAMProtectedService\x12\x43\n\x08SetOwner\x12\x1d.iamanager.v2.SetOwnerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x05\x43lear\x12\x1a.iamanager.v2.ClearRequest\x1a\x16.google.protobuf.Empty\"\x00\x12N\n\tCreateKey\x12\x1e.iamanager.v2.CreateKeyRequest\x1a\x1f.iamanager.v2.CreateKeyResponse\"\x00\x12N\n\tApplyCert\x12\x1e.iamanager.v2.ApplyCertRequest\x1a\x1f.iamanager.v2.ApplyCertResponse\"\x00\x12I\n\x0b\x45ncryptDisk\x12 .iamanager.v2.EncryptDiskRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x39\n\x08SetUsers\x12\x13.iamanager.v2.Users\x1a\x16.google.protobuf.Empty\"\x00\x12`\n\x0fRegisterService\x12$.iamanager.v2.RegisterServiceRequest\x1a%.iamanager.v2.RegisterServiceResponse\"\x00\x12U\n\x11UnregisterService\x12&.iamanager.v2.UnregisterServiceRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3'
+  ,
+  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,iamanager_dot_v2_dot_iamanagercommon__pb2.DESCRIPTOR,])
+
+
+
+
+_CLEARREQUEST = _descriptor.Descriptor(
+  name='ClearRequest',
+  full_name='iamanager.v2.ClearRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.ClearRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=120,
+  serialized_end=148,
+)
+
+
+_SETOWNERREQUEST = _descriptor.Descriptor(
+  name='SetOwnerRequest',
+  full_name='iamanager.v2.SetOwnerRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.SetOwnerRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.v2.SetOwnerRequest.password', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=150,
+  serialized_end=199,
+)
+
+
+_CREATEKEYREQUEST = _descriptor.Descriptor(
+  name='CreateKeyRequest',
+  full_name='iamanager.v2.CreateKeyRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.CreateKeyRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.v2.CreateKeyRequest.password', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=201,
+  serialized_end=251,
+)
+
+
+_CREATEKEYRESPONSE = _descriptor.Descriptor(
+  name='CreateKeyResponse',
+  full_name='iamanager.v2.CreateKeyResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.CreateKeyResponse.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='csr', full_name='iamanager.v2.CreateKeyResponse.csr', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=253,
+  serialized_end=299,
+)
+
+
+_APPLYCERTREQUEST = _descriptor.Descriptor(
+  name='ApplyCertRequest',
+  full_name='iamanager.v2.ApplyCertRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.ApplyCertRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert', full_name='iamanager.v2.ApplyCertRequest.cert', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=301,
+  serialized_end=347,
+)
+
+
+_APPLYCERTRESPONSE = _descriptor.Descriptor(
+  name='ApplyCertResponse',
+  full_name='iamanager.v2.ApplyCertResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.ApplyCertResponse.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert_url', full_name='iamanager.v2.ApplyCertResponse.cert_url', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=349,
+  serialized_end=400,
+)
+
+
+_REGISTERSERVICEREQUEST_PERMISSIONSENTRY = _descriptor.Descriptor(
+  name='PermissionsEntry',
+  full_name='iamanager.v2.RegisterServiceRequest.PermissionsEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='iamanager.v2.RegisterServiceRequest.PermissionsEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='iamanager.v2.RegisterServiceRequest.PermissionsEntry.value', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=525,
+  serialized_end=602,
+)
+
+_REGISTERSERVICEREQUEST = _descriptor.Descriptor(
+  name='RegisterServiceRequest',
+  full_name='iamanager.v2.RegisterServiceRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='service_id', full_name='iamanager.v2.RegisterServiceRequest.service_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='permissions', full_name='iamanager.v2.RegisterServiceRequest.permissions', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_REGISTERSERVICEREQUEST_PERMISSIONSENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=403,
+  serialized_end=602,
+)
+
+
+_REGISTERSERVICERESPONSE = _descriptor.Descriptor(
+  name='RegisterServiceResponse',
+  full_name='iamanager.v2.RegisterServiceResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='secret', full_name='iamanager.v2.RegisterServiceResponse.secret', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=604,
+  serialized_end=645,
+)
+
+
+_UNREGISTERSERVICEREQUEST = _descriptor.Descriptor(
+  name='UnregisterServiceRequest',
+  full_name='iamanager.v2.UnregisterServiceRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='service_id', full_name='iamanager.v2.UnregisterServiceRequest.service_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=647,
+  serialized_end=693,
+)
+
+
+_ENCRYPTDISKREQUEST = _descriptor.Descriptor(
+  name='EncryptDiskRequest',
+  full_name='iamanager.v2.EncryptDiskRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.v2.EncryptDiskRequest.password', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=695,
+  serialized_end=733,
+)
+
+_REGISTERSERVICEREQUEST_PERMISSIONSENTRY.fields_by_name['value'].message_type = iamanager_dot_v2_dot_iamanagercommon__pb2._PERMISSIONS
+_REGISTERSERVICEREQUEST_PERMISSIONSENTRY.containing_type = _REGISTERSERVICEREQUEST
+_REGISTERSERVICEREQUEST.fields_by_name['permissions'].message_type = _REGISTERSERVICEREQUEST_PERMISSIONSENTRY
+DESCRIPTOR.message_types_by_name['ClearRequest'] = _CLEARREQUEST
+DESCRIPTOR.message_types_by_name['SetOwnerRequest'] = _SETOWNERREQUEST
+DESCRIPTOR.message_types_by_name['CreateKeyRequest'] = _CREATEKEYREQUEST
+DESCRIPTOR.message_types_by_name['CreateKeyResponse'] = _CREATEKEYRESPONSE
+DESCRIPTOR.message_types_by_name['ApplyCertRequest'] = _APPLYCERTREQUEST
+DESCRIPTOR.message_types_by_name['ApplyCertResponse'] = _APPLYCERTRESPONSE
+DESCRIPTOR.message_types_by_name['RegisterServiceRequest'] = _REGISTERSERVICEREQUEST
+DESCRIPTOR.message_types_by_name['RegisterServiceResponse'] = _REGISTERSERVICERESPONSE
+DESCRIPTOR.message_types_by_name['UnregisterServiceRequest'] = _UNREGISTERSERVICEREQUEST
+DESCRIPTOR.message_types_by_name['EncryptDiskRequest'] = _ENCRYPTDISKREQUEST
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+ClearRequest = _reflection.GeneratedProtocolMessageType('ClearRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CLEARREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.ClearRequest)
+  })
+_sym_db.RegisterMessage(ClearRequest)
+
+SetOwnerRequest = _reflection.GeneratedProtocolMessageType('SetOwnerRequest', (_message.Message,), {
+  'DESCRIPTOR' : _SETOWNERREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.SetOwnerRequest)
+  })
+_sym_db.RegisterMessage(SetOwnerRequest)
+
+CreateKeyRequest = _reflection.GeneratedProtocolMessageType('CreateKeyRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.CreateKeyRequest)
+  })
+_sym_db.RegisterMessage(CreateKeyRequest)
+
+CreateKeyResponse = _reflection.GeneratedProtocolMessageType('CreateKeyResponse', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYRESPONSE,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.CreateKeyResponse)
+  })
+_sym_db.RegisterMessage(CreateKeyResponse)
+
+ApplyCertRequest = _reflection.GeneratedProtocolMessageType('ApplyCertRequest', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.ApplyCertRequest)
+  })
+_sym_db.RegisterMessage(ApplyCertRequest)
+
+ApplyCertResponse = _reflection.GeneratedProtocolMessageType('ApplyCertResponse', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTRESPONSE,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.ApplyCertResponse)
+  })
+_sym_db.RegisterMessage(ApplyCertResponse)
+
+RegisterServiceRequest = _reflection.GeneratedProtocolMessageType('RegisterServiceRequest', (_message.Message,), {
+
+  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _REGISTERSERVICEREQUEST_PERMISSIONSENTRY,
+    '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+    # @@protoc_insertion_point(class_scope:iamanager.v2.RegisterServiceRequest.PermissionsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _REGISTERSERVICEREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.RegisterServiceRequest)
+  })
+_sym_db.RegisterMessage(RegisterServiceRequest)
+_sym_db.RegisterMessage(RegisterServiceRequest.PermissionsEntry)
+
+RegisterServiceResponse = _reflection.GeneratedProtocolMessageType('RegisterServiceResponse', (_message.Message,), {
+  'DESCRIPTOR' : _REGISTERSERVICERESPONSE,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.RegisterServiceResponse)
+  })
+_sym_db.RegisterMessage(RegisterServiceResponse)
+
+UnregisterServiceRequest = _reflection.GeneratedProtocolMessageType('UnregisterServiceRequest', (_message.Message,), {
+  'DESCRIPTOR' : _UNREGISTERSERVICEREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.UnregisterServiceRequest)
+  })
+_sym_db.RegisterMessage(UnregisterServiceRequest)
+
+EncryptDiskRequest = _reflection.GeneratedProtocolMessageType('EncryptDiskRequest', (_message.Message,), {
+  'DESCRIPTOR' : _ENCRYPTDISKREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerprotected_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.EncryptDiskRequest)
+  })
+_sym_db.RegisterMessage(EncryptDiskRequest)
+
+
+_REGISTERSERVICEREQUEST_PERMISSIONSENTRY._options = None
+
+_IAMPROTECTEDSERVICE = _descriptor.ServiceDescriptor(
+  name='IAMProtectedService',
+  full_name='iamanager.v2.IAMProtectedService',
+  file=DESCRIPTOR,
+  index=0,
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_start=736,
+  serialized_end=1440,
+  methods=[
+  _descriptor.MethodDescriptor(
+    name='SetOwner',
+    full_name='iamanager.v2.IAMProtectedService.SetOwner',
+    index=0,
+    containing_service=None,
+    input_type=_SETOWNERREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='Clear',
+    full_name='iamanager.v2.IAMProtectedService.Clear',
+    index=1,
+    containing_service=None,
+    input_type=_CLEARREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='CreateKey',
+    full_name='iamanager.v2.IAMProtectedService.CreateKey',
+    index=2,
+    containing_service=None,
+    input_type=_CREATEKEYREQUEST,
+    output_type=_CREATEKEYRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='ApplyCert',
+    full_name='iamanager.v2.IAMProtectedService.ApplyCert',
+    index=3,
+    containing_service=None,
+    input_type=_APPLYCERTREQUEST,
+    output_type=_APPLYCERTRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='EncryptDisk',
+    full_name='iamanager.v2.IAMProtectedService.EncryptDisk',
+    index=4,
+    containing_service=None,
+    input_type=_ENCRYPTDISKREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='FinishProvisioning',
+    full_name='iamanager.v2.IAMProtectedService.FinishProvisioning',
+    index=5,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetUsers',
+    full_name='iamanager.v2.IAMProtectedService.SetUsers',
+    index=6,
+    containing_service=None,
+    input_type=iamanager_dot_v2_dot_iamanagercommon__pb2._USERS,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='RegisterService',
+    full_name='iamanager.v2.IAMProtectedService.RegisterService',
+    index=7,
+    containing_service=None,
+    input_type=_REGISTERSERVICEREQUEST,
+    output_type=_REGISTERSERVICERESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='UnregisterService',
+    full_name='iamanager.v2.IAMProtectedService.UnregisterService',
+    index=8,
+    containing_service=None,
+    input_type=_UNREGISTERSERVICEREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+])
+_sym_db.RegisterServiceDescriptor(_IAMPROTECTEDSERVICE)
+
+DESCRIPTOR.services_by_name['IAMProtectedService'] = _IAMPROTECTEDSERVICE
+
+# @@protoc_insertion_point(module_scope)
```

## aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py

 * *Ordering differences only*

```diff
@@ -1,335 +1,335 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-from aos_prov.communication.unit.v2.generated import (
-    iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2,
-)
-from aos_prov.communication.unit.v2.generated import (
-    iamanagerprotected_pb2 as iamanager_dot_v2_dot_iamanagerprotected__pb2,
-)
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-
-
-class IAMProtectedServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.SetOwner = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/SetOwner',
-                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.SetOwnerRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.Clear = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/Clear',
-                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ClearRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.CreateKey = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/CreateKey',
-                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyResponse.FromString,
-                )
-        self.ApplyCert = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/ApplyCert',
-                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertResponse.FromString,
-                )
-        self.EncryptDisk = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/EncryptDisk',
-                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.EncryptDiskRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.FinishProvisioning = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/FinishProvisioning',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.SetUsers = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/SetUsers',
-                request_serializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.RegisterService = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/RegisterService',
-                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceResponse.FromString,
-                )
-        self.UnregisterService = channel.unary_unary(
-                '/iamanager.v2.IAMProtectedService/UnregisterService',
-                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.UnregisterServiceRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-
-
-class IAMProtectedServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def SetOwner(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Clear(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def CreateKey(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def ApplyCert(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def EncryptDisk(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def FinishProvisioning(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SetUsers(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def RegisterService(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def UnregisterService(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMProtectedServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'SetOwner': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetOwner,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.SetOwnerRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'Clear': grpc.unary_unary_rpc_method_handler(
-                    servicer.Clear,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ClearRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'CreateKey': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateKey,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyRequest.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyResponse.SerializeToString,
-            ),
-            'ApplyCert': grpc.unary_unary_rpc_method_handler(
-                    servicer.ApplyCert,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertRequest.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertResponse.SerializeToString,
-            ),
-            'EncryptDisk': grpc.unary_unary_rpc_method_handler(
-                    servicer.EncryptDisk,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.EncryptDiskRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'FinishProvisioning': grpc.unary_unary_rpc_method_handler(
-                    servicer.FinishProvisioning,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'SetUsers': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetUsers,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'RegisterService': grpc.unary_unary_rpc_method_handler(
-                    servicer.RegisterService,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceRequest.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceResponse.SerializeToString,
-            ),
-            'UnregisterService': grpc.unary_unary_rpc_method_handler(
-                    servicer.UnregisterService,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.UnregisterServiceRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v2.IAMProtectedService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMProtectedService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def SetOwner(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/SetOwner',
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.SetOwnerRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Clear(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/Clear',
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.ClearRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def CreateKey(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/CreateKey',
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyRequest.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ApplyCert(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/ApplyCert',
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertRequest.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def EncryptDisk(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/EncryptDisk',
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.EncryptDiskRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def FinishProvisioning(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/FinishProvisioning',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SetUsers(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/SetUsers',
-            iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def RegisterService(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/RegisterService',
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceRequest.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def UnregisterService(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/UnregisterService',
-            iamanager_dot_v2_dot_iamanagerprotected__pb2.UnregisterServiceRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+from aos_prov.communication.unit.v2.generated import (
+    iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2,
+)
+from aos_prov.communication.unit.v2.generated import (
+    iamanagerprotected_pb2 as iamanager_dot_v2_dot_iamanagerprotected__pb2,
+)
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+
+
+class IAMProtectedServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.SetOwner = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/SetOwner',
+                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.SetOwnerRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.Clear = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/Clear',
+                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ClearRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.CreateKey = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/CreateKey',
+                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyResponse.FromString,
+                )
+        self.ApplyCert = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/ApplyCert',
+                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertResponse.FromString,
+                )
+        self.EncryptDisk = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/EncryptDisk',
+                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.EncryptDiskRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.FinishProvisioning = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/FinishProvisioning',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.SetUsers = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/SetUsers',
+                request_serializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.RegisterService = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/RegisterService',
+                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceResponse.FromString,
+                )
+        self.UnregisterService = channel.unary_unary(
+                '/iamanager.v2.IAMProtectedService/UnregisterService',
+                request_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.UnregisterServiceRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+
+
+class IAMProtectedServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def SetOwner(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Clear(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def CreateKey(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ApplyCert(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def EncryptDisk(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def FinishProvisioning(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SetUsers(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def RegisterService(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def UnregisterService(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMProtectedServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'SetOwner': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetOwner,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.SetOwnerRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'Clear': grpc.unary_unary_rpc_method_handler(
+                    servicer.Clear,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ClearRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'CreateKey': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateKey,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyRequest.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyResponse.SerializeToString,
+            ),
+            'ApplyCert': grpc.unary_unary_rpc_method_handler(
+                    servicer.ApplyCert,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertRequest.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertResponse.SerializeToString,
+            ),
+            'EncryptDisk': grpc.unary_unary_rpc_method_handler(
+                    servicer.EncryptDisk,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.EncryptDiskRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'FinishProvisioning': grpc.unary_unary_rpc_method_handler(
+                    servicer.FinishProvisioning,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'SetUsers': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetUsers,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'RegisterService': grpc.unary_unary_rpc_method_handler(
+                    servicer.RegisterService,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceRequest.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceResponse.SerializeToString,
+            ),
+            'UnregisterService': grpc.unary_unary_rpc_method_handler(
+                    servicer.UnregisterService,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerprotected__pb2.UnregisterServiceRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v2.IAMProtectedService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMProtectedService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def SetOwner(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/SetOwner',
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.SetOwnerRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Clear(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/Clear',
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.ClearRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CreateKey(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/CreateKey',
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyRequest.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.CreateKeyResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ApplyCert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/ApplyCert',
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertRequest.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.ApplyCertResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def EncryptDisk(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/EncryptDisk',
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.EncryptDiskRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def FinishProvisioning(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/FinishProvisioning',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetUsers(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/SetUsers',
+            iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def RegisterService(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/RegisterService',
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceRequest.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.RegisterServiceResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UnregisterService(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMProtectedService/UnregisterService',
+            iamanager_dot_v2_dot_iamanagerprotected__pb2.UnregisterServiceRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py

 * *Ordering differences only*

```diff
@@ -1,451 +1,451 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: iamanager/v2/iamanagerpublic.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from aos_prov.communication.unit.v2.generated import (
-    iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2,
-)
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='iamanager/v2/iamanagerpublic.proto',
-  package='iamanager.v2',
-  syntax='proto3',
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\"iamanager/v2/iamanagerpublic.proto\x12\x0ciamanager.v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\"iamanager/v2/iamanagercommon.proto\"4\n\nSystemInfo\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t\"\x1a\n\tCertTypes\x12\r\n\x05types\x18\x01 \x03(\t\">\n\x0eGetCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"B\n\x0fGetCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\"B\n\x12PermissionsRequest\x12\x0e\n\x06secret\x18\x01 \x01(\t\x12\x1c\n\x14\x66unctional_server_id\x18\x02 \x01(\t\"Y\n\x13PermissionsResponse\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12.\n\x0bpermissions\x18\x02 \x01(\x0b\x32\x19.iamanager.v2.Permissions\"\x1d\n\nAPIVersion\x12\x0f\n\x07version\x18\x01 \x01(\x04\x32\x87\x04\n\x10IAMPublicService\x12\x43\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v2.SystemInfo\"\x00\x12\x41\n\x0cGetCertTypes\x12\x16.google.protobuf.Empty\x1a\x17.iamanager.v2.CertTypes\"\x00\x12H\n\x07GetCert\x12\x1c.iamanager.v2.GetCertRequest\x1a\x1d.iamanager.v2.GetCertResponse\"\x00\x12W\n\x0eGetPermissions\x12 .iamanager.v2.PermissionsRequest\x1a!.iamanager.v2.PermissionsResponse\"\x00\x12\x39\n\x08GetUsers\x12\x16.google.protobuf.Empty\x1a\x13.iamanager.v2.Users\"\x00\x12H\n\x15SubscribeUsersChanged\x12\x16.google.protobuf.Empty\x1a\x13.iamanager.v2.Users\"\x00\x30\x01\x12\x43\n\rGetAPIVersion\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v2.APIVersion\"\x00\x62\x06proto3'
-  ,
-  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,iamanager_dot_v2_dot_iamanagercommon__pb2.DESCRIPTOR,])
-
-
-
-
-_SYSTEMINFO = _descriptor.Descriptor(
-  name='SystemInfo',
-  full_name='iamanager.v2.SystemInfo',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='system_id', full_name='iamanager.v2.SystemInfo.system_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='board_model', full_name='iamanager.v2.SystemInfo.board_model', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=117,
-  serialized_end=169,
-)
-
-
-_CERTTYPES = _descriptor.Descriptor(
-  name='CertTypes',
-  full_name='iamanager.v2.CertTypes',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='types', full_name='iamanager.v2.CertTypes.types', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=171,
-  serialized_end=197,
-)
-
-
-_GETCERTREQUEST = _descriptor.Descriptor(
-  name='GetCertRequest',
-  full_name='iamanager.v2.GetCertRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.GetCertRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='issuer', full_name='iamanager.v2.GetCertRequest.issuer', index=1,
-      number=2, type=12, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"",
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='serial', full_name='iamanager.v2.GetCertRequest.serial', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=199,
-  serialized_end=261,
-)
-
-
-_GETCERTRESPONSE = _descriptor.Descriptor(
-  name='GetCertResponse',
-  full_name='iamanager.v2.GetCertResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v2.GetCertResponse.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cert_url', full_name='iamanager.v2.GetCertResponse.cert_url', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='key_url', full_name='iamanager.v2.GetCertResponse.key_url', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=263,
-  serialized_end=329,
-)
-
-
-_PERMISSIONSREQUEST = _descriptor.Descriptor(
-  name='PermissionsRequest',
-  full_name='iamanager.v2.PermissionsRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='secret', full_name='iamanager.v2.PermissionsRequest.secret', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='functional_server_id', full_name='iamanager.v2.PermissionsRequest.functional_server_id', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=331,
-  serialized_end=397,
-)
-
-
-_PERMISSIONSRESPONSE = _descriptor.Descriptor(
-  name='PermissionsResponse',
-  full_name='iamanager.v2.PermissionsResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='service_id', full_name='iamanager.v2.PermissionsResponse.service_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='permissions', full_name='iamanager.v2.PermissionsResponse.permissions', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=399,
-  serialized_end=488,
-)
-
-
-_APIVERSION = _descriptor.Descriptor(
-  name='APIVersion',
-  full_name='iamanager.v2.APIVersion',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='version', full_name='iamanager.v2.APIVersion.version', index=0,
-      number=1, type=4, cpp_type=4, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=490,
-  serialized_end=519,
-)
-
-_PERMISSIONSRESPONSE.fields_by_name['permissions'].message_type = iamanager_dot_v2_dot_iamanagercommon__pb2._PERMISSIONS
-DESCRIPTOR.message_types_by_name['SystemInfo'] = _SYSTEMINFO
-DESCRIPTOR.message_types_by_name['CertTypes'] = _CERTTYPES
-DESCRIPTOR.message_types_by_name['GetCertRequest'] = _GETCERTREQUEST
-DESCRIPTOR.message_types_by_name['GetCertResponse'] = _GETCERTRESPONSE
-DESCRIPTOR.message_types_by_name['PermissionsRequest'] = _PERMISSIONSREQUEST
-DESCRIPTOR.message_types_by_name['PermissionsResponse'] = _PERMISSIONSRESPONSE
-DESCRIPTOR.message_types_by_name['APIVersion'] = _APIVERSION
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-SystemInfo = _reflection.GeneratedProtocolMessageType('SystemInfo', (_message.Message,), {
-  'DESCRIPTOR' : _SYSTEMINFO,
-  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.SystemInfo)
-  })
-_sym_db.RegisterMessage(SystemInfo)
-
-CertTypes = _reflection.GeneratedProtocolMessageType('CertTypes', (_message.Message,), {
-  'DESCRIPTOR' : _CERTTYPES,
-  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.CertTypes)
-  })
-_sym_db.RegisterMessage(CertTypes)
-
-GetCertRequest = _reflection.GeneratedProtocolMessageType('GetCertRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.GetCertRequest)
-  })
-_sym_db.RegisterMessage(GetCertRequest)
-
-GetCertResponse = _reflection.GeneratedProtocolMessageType('GetCertResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTRESPONSE,
-  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.GetCertResponse)
-  })
-_sym_db.RegisterMessage(GetCertResponse)
-
-PermissionsRequest = _reflection.GeneratedProtocolMessageType('PermissionsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _PERMISSIONSREQUEST,
-  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.PermissionsRequest)
-  })
-_sym_db.RegisterMessage(PermissionsRequest)
-
-PermissionsResponse = _reflection.GeneratedProtocolMessageType('PermissionsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _PERMISSIONSRESPONSE,
-  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.PermissionsResponse)
-  })
-_sym_db.RegisterMessage(PermissionsResponse)
-
-APIVersion = _reflection.GeneratedProtocolMessageType('APIVersion', (_message.Message,), {
-  'DESCRIPTOR' : _APIVERSION,
-  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v2.APIVersion)
-  })
-_sym_db.RegisterMessage(APIVersion)
-
-
-
-_IAMPUBLICSERVICE = _descriptor.ServiceDescriptor(
-  name='IAMPublicService',
-  full_name='iamanager.v2.IAMPublicService',
-  file=DESCRIPTOR,
-  index=0,
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_start=522,
-  serialized_end=1041,
-  methods=[
-  _descriptor.MethodDescriptor(
-    name='GetSystemInfo',
-    full_name='iamanager.v2.IAMPublicService.GetSystemInfo',
-    index=0,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=_SYSTEMINFO,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetCertTypes',
-    full_name='iamanager.v2.IAMPublicService.GetCertTypes',
-    index=1,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=_CERTTYPES,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetCert',
-    full_name='iamanager.v2.IAMPublicService.GetCert',
-    index=2,
-    containing_service=None,
-    input_type=_GETCERTREQUEST,
-    output_type=_GETCERTRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetPermissions',
-    full_name='iamanager.v2.IAMPublicService.GetPermissions',
-    index=3,
-    containing_service=None,
-    input_type=_PERMISSIONSREQUEST,
-    output_type=_PERMISSIONSRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetUsers',
-    full_name='iamanager.v2.IAMPublicService.GetUsers',
-    index=4,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=iamanager_dot_v2_dot_iamanagercommon__pb2._USERS,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='SubscribeUsersChanged',
-    full_name='iamanager.v2.IAMPublicService.SubscribeUsersChanged',
-    index=5,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=iamanager_dot_v2_dot_iamanagercommon__pb2._USERS,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='GetAPIVersion',
-    full_name='iamanager.v2.IAMPublicService.GetAPIVersion',
-    index=6,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=_APIVERSION,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-])
-_sym_db.RegisterServiceDescriptor(_IAMPUBLICSERVICE)
-
-DESCRIPTOR.services_by_name['IAMPublicService'] = _IAMPUBLICSERVICE
-
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: iamanager/v2/iamanagerpublic.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from aos_prov.communication.unit.v2.generated import (
+    iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2,
+)
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='iamanager/v2/iamanagerpublic.proto',
+  package='iamanager.v2',
+  syntax='proto3',
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_pb=b'\n\"iamanager/v2/iamanagerpublic.proto\x12\x0ciamanager.v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\"iamanager/v2/iamanagercommon.proto\"4\n\nSystemInfo\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t\"\x1a\n\tCertTypes\x12\r\n\x05types\x18\x01 \x03(\t\">\n\x0eGetCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"B\n\x0fGetCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\"B\n\x12PermissionsRequest\x12\x0e\n\x06secret\x18\x01 \x01(\t\x12\x1c\n\x14\x66unctional_server_id\x18\x02 \x01(\t\"Y\n\x13PermissionsResponse\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12.\n\x0bpermissions\x18\x02 \x01(\x0b\x32\x19.iamanager.v2.Permissions\"\x1d\n\nAPIVersion\x12\x0f\n\x07version\x18\x01 \x01(\x04\x32\x87\x04\n\x10IAMPublicService\x12\x43\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v2.SystemInfo\"\x00\x12\x41\n\x0cGetCertTypes\x12\x16.google.protobuf.Empty\x1a\x17.iamanager.v2.CertTypes\"\x00\x12H\n\x07GetCert\x12\x1c.iamanager.v2.GetCertRequest\x1a\x1d.iamanager.v2.GetCertResponse\"\x00\x12W\n\x0eGetPermissions\x12 .iamanager.v2.PermissionsRequest\x1a!.iamanager.v2.PermissionsResponse\"\x00\x12\x39\n\x08GetUsers\x12\x16.google.protobuf.Empty\x1a\x13.iamanager.v2.Users\"\x00\x12H\n\x15SubscribeUsersChanged\x12\x16.google.protobuf.Empty\x1a\x13.iamanager.v2.Users\"\x00\x30\x01\x12\x43\n\rGetAPIVersion\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v2.APIVersion\"\x00\x62\x06proto3'
+  ,
+  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,iamanager_dot_v2_dot_iamanagercommon__pb2.DESCRIPTOR,])
+
+
+
+
+_SYSTEMINFO = _descriptor.Descriptor(
+  name='SystemInfo',
+  full_name='iamanager.v2.SystemInfo',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='system_id', full_name='iamanager.v2.SystemInfo.system_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='board_model', full_name='iamanager.v2.SystemInfo.board_model', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=117,
+  serialized_end=169,
+)
+
+
+_CERTTYPES = _descriptor.Descriptor(
+  name='CertTypes',
+  full_name='iamanager.v2.CertTypes',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='types', full_name='iamanager.v2.CertTypes.types', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=171,
+  serialized_end=197,
+)
+
+
+_GETCERTREQUEST = _descriptor.Descriptor(
+  name='GetCertRequest',
+  full_name='iamanager.v2.GetCertRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.GetCertRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='issuer', full_name='iamanager.v2.GetCertRequest.issuer', index=1,
+      number=2, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='serial', full_name='iamanager.v2.GetCertRequest.serial', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=199,
+  serialized_end=261,
+)
+
+
+_GETCERTRESPONSE = _descriptor.Descriptor(
+  name='GetCertResponse',
+  full_name='iamanager.v2.GetCertResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.v2.GetCertResponse.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert_url', full_name='iamanager.v2.GetCertResponse.cert_url', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='key_url', full_name='iamanager.v2.GetCertResponse.key_url', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=263,
+  serialized_end=329,
+)
+
+
+_PERMISSIONSREQUEST = _descriptor.Descriptor(
+  name='PermissionsRequest',
+  full_name='iamanager.v2.PermissionsRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='secret', full_name='iamanager.v2.PermissionsRequest.secret', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='functional_server_id', full_name='iamanager.v2.PermissionsRequest.functional_server_id', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=331,
+  serialized_end=397,
+)
+
+
+_PERMISSIONSRESPONSE = _descriptor.Descriptor(
+  name='PermissionsResponse',
+  full_name='iamanager.v2.PermissionsResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='service_id', full_name='iamanager.v2.PermissionsResponse.service_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='permissions', full_name='iamanager.v2.PermissionsResponse.permissions', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=399,
+  serialized_end=488,
+)
+
+
+_APIVERSION = _descriptor.Descriptor(
+  name='APIVersion',
+  full_name='iamanager.v2.APIVersion',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='version', full_name='iamanager.v2.APIVersion.version', index=0,
+      number=1, type=4, cpp_type=4, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=490,
+  serialized_end=519,
+)
+
+_PERMISSIONSRESPONSE.fields_by_name['permissions'].message_type = iamanager_dot_v2_dot_iamanagercommon__pb2._PERMISSIONS
+DESCRIPTOR.message_types_by_name['SystemInfo'] = _SYSTEMINFO
+DESCRIPTOR.message_types_by_name['CertTypes'] = _CERTTYPES
+DESCRIPTOR.message_types_by_name['GetCertRequest'] = _GETCERTREQUEST
+DESCRIPTOR.message_types_by_name['GetCertResponse'] = _GETCERTRESPONSE
+DESCRIPTOR.message_types_by_name['PermissionsRequest'] = _PERMISSIONSREQUEST
+DESCRIPTOR.message_types_by_name['PermissionsResponse'] = _PERMISSIONSRESPONSE
+DESCRIPTOR.message_types_by_name['APIVersion'] = _APIVERSION
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+SystemInfo = _reflection.GeneratedProtocolMessageType('SystemInfo', (_message.Message,), {
+  'DESCRIPTOR' : _SYSTEMINFO,
+  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.SystemInfo)
+  })
+_sym_db.RegisterMessage(SystemInfo)
+
+CertTypes = _reflection.GeneratedProtocolMessageType('CertTypes', (_message.Message,), {
+  'DESCRIPTOR' : _CERTTYPES,
+  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.CertTypes)
+  })
+_sym_db.RegisterMessage(CertTypes)
+
+GetCertRequest = _reflection.GeneratedProtocolMessageType('GetCertRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.GetCertRequest)
+  })
+_sym_db.RegisterMessage(GetCertRequest)
+
+GetCertResponse = _reflection.GeneratedProtocolMessageType('GetCertResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTRESPONSE,
+  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.GetCertResponse)
+  })
+_sym_db.RegisterMessage(GetCertResponse)
+
+PermissionsRequest = _reflection.GeneratedProtocolMessageType('PermissionsRequest', (_message.Message,), {
+  'DESCRIPTOR' : _PERMISSIONSREQUEST,
+  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.PermissionsRequest)
+  })
+_sym_db.RegisterMessage(PermissionsRequest)
+
+PermissionsResponse = _reflection.GeneratedProtocolMessageType('PermissionsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _PERMISSIONSRESPONSE,
+  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.PermissionsResponse)
+  })
+_sym_db.RegisterMessage(PermissionsResponse)
+
+APIVersion = _reflection.GeneratedProtocolMessageType('APIVersion', (_message.Message,), {
+  'DESCRIPTOR' : _APIVERSION,
+  '__module__' : 'iamanager.v2.iamanagerpublic_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v2.APIVersion)
+  })
+_sym_db.RegisterMessage(APIVersion)
+
+
+
+_IAMPUBLICSERVICE = _descriptor.ServiceDescriptor(
+  name='IAMPublicService',
+  full_name='iamanager.v2.IAMPublicService',
+  file=DESCRIPTOR,
+  index=0,
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_start=522,
+  serialized_end=1041,
+  methods=[
+  _descriptor.MethodDescriptor(
+    name='GetSystemInfo',
+    full_name='iamanager.v2.IAMPublicService.GetSystemInfo',
+    index=0,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_SYSTEMINFO,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetCertTypes',
+    full_name='iamanager.v2.IAMPublicService.GetCertTypes',
+    index=1,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_CERTTYPES,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetCert',
+    full_name='iamanager.v2.IAMPublicService.GetCert',
+    index=2,
+    containing_service=None,
+    input_type=_GETCERTREQUEST,
+    output_type=_GETCERTRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetPermissions',
+    full_name='iamanager.v2.IAMPublicService.GetPermissions',
+    index=3,
+    containing_service=None,
+    input_type=_PERMISSIONSREQUEST,
+    output_type=_PERMISSIONSRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetUsers',
+    full_name='iamanager.v2.IAMPublicService.GetUsers',
+    index=4,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=iamanager_dot_v2_dot_iamanagercommon__pb2._USERS,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SubscribeUsersChanged',
+    full_name='iamanager.v2.IAMPublicService.SubscribeUsersChanged',
+    index=5,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=iamanager_dot_v2_dot_iamanagercommon__pb2._USERS,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetAPIVersion',
+    full_name='iamanager.v2.IAMPublicService.GetAPIVersion',
+    index=6,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_APIVERSION,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+])
+_sym_db.RegisterServiceDescriptor(_IAMPUBLICSERVICE)
+
+DESCRIPTOR.services_by_name['IAMPublicService'] = _IAMPUBLICSERVICE
+
+# @@protoc_insertion_point(module_scope)
```

## aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py

 * *Ordering differences only*

```diff
@@ -1,269 +1,269 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-from aos_prov.communication.unit.v2.generated import (
-    iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2,
-)
-from aos_prov.communication.unit.v2.generated import (
-    iamanagerpublic_pb2 as iamanager_dot_v2_dot_iamanagerpublic__pb2,
-)
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-
-
-class IAMPublicServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetSystemInfo = channel.unary_unary(
-                '/iamanager.v2.IAMPublicService/GetSystemInfo',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.SystemInfo.FromString,
-                )
-        self.GetCertTypes = channel.unary_unary(
-                '/iamanager.v2.IAMPublicService/GetCertTypes',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.CertTypes.FromString,
-                )
-        self.GetCert = channel.unary_unary(
-                '/iamanager.v2.IAMPublicService/GetCert',
-                request_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertResponse.FromString,
-                )
-        self.GetPermissions = channel.unary_unary(
-                '/iamanager.v2.IAMPublicService/GetPermissions',
-                request_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsResponse.FromString,
-                )
-        self.GetUsers = channel.unary_unary(
-                '/iamanager.v2.IAMPublicService/GetUsers',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
-                )
-        self.SubscribeUsersChanged = channel.unary_stream(
-                '/iamanager.v2.IAMPublicService/SubscribeUsersChanged',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
-                )
-        self.GetAPIVersion = channel.unary_unary(
-                '/iamanager.v2.IAMPublicService/GetAPIVersion',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.APIVersion.FromString,
-                )
-
-
-class IAMPublicServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetSystemInfo(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetCertTypes(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetCert(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetPermissions(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetUsers(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SubscribeUsersChanged(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetAPIVersion(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPublicServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetSystemInfo': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetSystemInfo,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.SystemInfo.SerializeToString,
-            ),
-            'GetCertTypes': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCertTypes,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.CertTypes.SerializeToString,
-            ),
-            'GetCert': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCert,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertRequest.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertResponse.SerializeToString,
-            ),
-            'GetPermissions': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetPermissions,
-                    request_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsRequest.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsResponse.SerializeToString,
-            ),
-            'GetUsers': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetUsers,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
-            ),
-            'SubscribeUsersChanged': grpc.unary_stream_rpc_method_handler(
-                    servicer.SubscribeUsersChanged,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
-            ),
-            'GetAPIVersion': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAPIVersion,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.APIVersion.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v2.IAMPublicService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPublicService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetSystemInfo(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetSystemInfo',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerpublic__pb2.SystemInfo.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetCertTypes(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetCertTypes',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerpublic__pb2.CertTypes.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetCert(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetCert',
-            iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertRequest.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetPermissions(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetPermissions',
-            iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsRequest.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetUsers(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetUsers',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SubscribeUsersChanged(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/iamanager.v2.IAMPublicService/SubscribeUsersChanged',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetAPIVersion(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetAPIVersion',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v2_dot_iamanagerpublic__pb2.APIVersion.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+from aos_prov.communication.unit.v2.generated import (
+    iamanagercommon_pb2 as iamanager_dot_v2_dot_iamanagercommon__pb2,
+)
+from aos_prov.communication.unit.v2.generated import (
+    iamanagerpublic_pb2 as iamanager_dot_v2_dot_iamanagerpublic__pb2,
+)
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+
+
+class IAMPublicServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetSystemInfo = channel.unary_unary(
+                '/iamanager.v2.IAMPublicService/GetSystemInfo',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.SystemInfo.FromString,
+                )
+        self.GetCertTypes = channel.unary_unary(
+                '/iamanager.v2.IAMPublicService/GetCertTypes',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.CertTypes.FromString,
+                )
+        self.GetCert = channel.unary_unary(
+                '/iamanager.v2.IAMPublicService/GetCert',
+                request_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertResponse.FromString,
+                )
+        self.GetPermissions = channel.unary_unary(
+                '/iamanager.v2.IAMPublicService/GetPermissions',
+                request_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsResponse.FromString,
+                )
+        self.GetUsers = channel.unary_unary(
+                '/iamanager.v2.IAMPublicService/GetUsers',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
+                )
+        self.SubscribeUsersChanged = channel.unary_stream(
+                '/iamanager.v2.IAMPublicService/SubscribeUsersChanged',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
+                )
+        self.GetAPIVersion = channel.unary_unary(
+                '/iamanager.v2.IAMPublicService/GetAPIVersion',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.APIVersion.FromString,
+                )
+
+
+class IAMPublicServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetSystemInfo(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetCertTypes(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetCert(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetPermissions(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetUsers(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubscribeUsersChanged(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetAPIVersion(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPublicServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetSystemInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSystemInfo,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.SystemInfo.SerializeToString,
+            ),
+            'GetCertTypes': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCertTypes,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.CertTypes.SerializeToString,
+            ),
+            'GetCert': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCert,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertRequest.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertResponse.SerializeToString,
+            ),
+            'GetPermissions': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetPermissions,
+                    request_deserializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsRequest.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsResponse.SerializeToString,
+            ),
+            'GetUsers': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetUsers,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
+            ),
+            'SubscribeUsersChanged': grpc.unary_stream_rpc_method_handler(
+                    servicer.SubscribeUsersChanged,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagercommon__pb2.Users.SerializeToString,
+            ),
+            'GetAPIVersion': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAPIVersion,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v2_dot_iamanagerpublic__pb2.APIVersion.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v2.IAMPublicService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPublicService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetSystemInfo(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetSystemInfo',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerpublic__pb2.SystemInfo.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetCertTypes(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetCertTypes',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerpublic__pb2.CertTypes.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetCert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetCert',
+            iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertRequest.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerpublic__pb2.GetCertResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetPermissions(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetPermissions',
+            iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsRequest.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerpublic__pb2.PermissionsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetUsers(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetUsers',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubscribeUsersChanged(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/iamanager.v2.IAMPublicService/SubscribeUsersChanged',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v2_dot_iamanagercommon__pb2.Users.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetAPIVersion(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v2.IAMPublicService/GetAPIVersion',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v2_dot_iamanagerpublic__pb2.APIVersion.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## aos_prov/communication/unit/v4/unit_communication_v4.py

 * *Ordering differences only*

```diff
@@ -1,202 +1,202 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-from contextlib import contextmanager
-
-import grpc
-from aos_prov.communication.unit.v4.generated import iamanager_pb2 as iam_manager
-from aos_prov.communication.unit.v4.generated import (
-    iamanager_pb2_grpc as iam_manager_grpc,
-)
-from aos_prov.utils.common import print_done, print_left, print_success
-from aos_prov.utils.errors import GrpcUnimplemented, UnitError
-from aos_prov.utils.unit_certificate import UnitCertificate
-from google.protobuf import empty_pb2
-
-UNIT_DEFAULT_PORT = 8089
-_MAX_PORT = 65535
-
-
-class UnitCommunicationV4:
-    def __init__(self, address: str = 'localhost:8089'):
-        self._need_set_users = False
-
-        if not address:
-            address = 'localhost:8089'
-
-        parts = address.split(':')
-        if len(parts) == 2:
-            try:
-                port = int(parts[1])
-                if port not in range(1, _MAX_PORT):
-                    raise UnitError('Unit port is invalid')
-            except ValueError as exc:
-                raise UnitError('Unit port is invalid') from exc
-        else:
-            address = address + ':' + str(UNIT_DEFAULT_PORT)
-        self._unit_address = address
-
-    @property
-    def need_set_users(self):
-        return self._need_set_users
-
-    @need_set_users.setter
-    def need_set_users(self, set_users):
-        self._need_set_users = set_users
-
-    @contextmanager
-    def unit_certificate_stub(self, catch_inactive=False, wait_for_close=False):
-        try:
-            with grpc.insecure_channel(self._unit_address) as channel:
-                stub = iam_manager_grpc.IAMCertificateServiceStub(channel)
-                if wait_for_close:
-                    def _stop_wait(state):  # noqa: WPS430
-                        if state is grpc.ChannelConnectivity.SHUTDOWN:
-                            channel.unsubscribe(_stop_wait)
-                            return
-                    channel.subscribe(_stop_wait, try_to_connect=False)
-                yield stub
-
-        except grpc.RpcError as exc:
-            e_code = exc.code()
-            e_detail = exc.details()
-            if catch_inactive and not (e_code == grpc.StatusCode.UNAVAILABLE.value and e_detail == 'Socket closed'):
-                return
-            if wait_for_close and (e_code == grpc.StatusCode.UNKNOWN.value and e_detail == 'Stream removed'):
-                return
-            raise UnitError(f'FAILED! Error occurred: \n{e_code}: {e_detail}') from exc
-
-    @contextmanager
-    def unit_identify_stub(self):
-        try:
-            with grpc.insecure_channel(self._unit_address) as channel:
-                stub = iam_manager_grpc.IAMPublicIdentityServiceStub(channel)
-                yield stub
-
-        except grpc.RpcError as exc:
-            e_code = exc.code()
-            e_detail = exc.details()
-            if e_code.value == grpc.StatusCode.UNIMPLEMENTED.value:
-                raise GrpcUnimplemented(f'Protocol V4 is not supported: \n{e_code}: {e_detail}') from exc
-            raise UnitError(f'FAILED! Error occurred: \n{e_code}: {e_detail}') from exc
-
-    @contextmanager
-    def unit_provisioning_stub(self, catch_inactive=False, wait_for_close=False):
-        try:
-            with grpc.insecure_channel(self._unit_address) as channel:
-                stub = iam_manager_grpc.IAMProvisioningServiceStub(channel)
-                if wait_for_close:
-                    def _stop_wait(state):  # noqa: WPS430
-                        if state is grpc.ChannelConnectivity.SHUTDOWN:
-                            channel.unsubscribe(_stop_wait)
-                            return
-                    channel.subscribe(_stop_wait, try_to_connect=False)
-                yield stub
-
-        except grpc.RpcError as exc:
-            e_code = exc.code()
-            e_detail = exc.details()
-            if catch_inactive and not (e_code == grpc.StatusCode.UNAVAILABLE.value and e_detail == 'Socket closed'):
-                return
-            if wait_for_close and (e_code == grpc.StatusCode.UNKNOWN.value and e_detail == 'Stream removed'):
-                return
-            raise UnitError(f'FAILED! Error occurred: \n{e_code}: {e_detail}') from exc
-
-    @contextmanager
-    def unit_public_stub(self):
-        try:
-            with grpc.insecure_channel(self._unit_address) as channel:
-                stub = iam_manager_grpc.IAMPublicServiceStub(channel)
-                yield stub
-
-        except grpc.RpcError as exc:
-            e_code = exc.code()
-            e_detail = exc.details()
-            if e_code.value == grpc.StatusCode.UNIMPLEMENTED.value:
-                raise GrpcUnimplemented(f'Protocol V4 is not supported: \n{e_code}: {e_detail}') from exc
-            raise UnitError(f'FAILED! Error occurred: \n{e_code}: {e_detail}') from exc
-
-    def get_protocol_version(self) -> int:
-        with self.unit_public_stub() as stub:
-            print_left('Getting protocol version...')
-            response = stub.GetAPIVersion(empty_pb2.Empty())
-            print_success(str(response.version))
-            return int(response.version)
-
-    def get_system_info(self) -> (str, str):
-        with self.unit_identify_stub() as stub:
-            print_left('Getting System Info...')
-            response = stub.GetSystemInfo(empty_pb2.Empty())
-            print_done()
-            print_left('System ID:')
-            print_success(response.system_id)
-            print_left('Model name:')
-            print_success(response.board_model)
-            return response.system_id, response.board_model
-
-    def clear(self, certificate_type: str, node_id: str = '') -> None:
-        with self.unit_provisioning_stub() as stub:
-            print_left(f'Clearing certificate: {certificate_type} on Node ID: {node_id}...')
-            response = stub.Clear(iam_manager.ClearRequest(type=certificate_type, node_id=node_id))
-            print_done()
-            return response
-
-    def set_cert_owner(self, certificate_type: str, password: str, node_id: str = '') -> None:
-        with self.unit_provisioning_stub() as stub:
-            print_left(f'Setting owner for: {certificate_type} on Node ID: {node_id}...')
-            response = stub.SetOwner(
-                iam_manager.SetOwnerRequest(type=certificate_type, password=password, node_id=node_id),
-            )
-            print_done()
-            return response
-
-    def get_all_node_ids(self) -> [str]:
-        with self.unit_provisioning_stub() as stub:
-            print_left('Getting Node IDs...')
-            response = stub.GetAllNodeIDs(empty_pb2.Empty())
-            print_success(response.ids)
-            return response.ids
-
-    def get_cert_types(self, node_id: str = '') -> [str]:
-        with self.unit_provisioning_stub() as stub:
-            print_left(f'Getting certificate types to renew on node {node_id}...')
-            response = stub.GetCertTypes(iam_manager.GetCertTypesRequest(node_id=node_id))
-            print_success(response.types)
-            return response.types
-
-    def create_keys(self, cert_type: str, password: str, node_id: str = '') -> UnitCertificate:
-        with self.unit_certificate_stub() as stub:
-            print_left(f'Generating key type: {cert_type} on Node: {node_id}...')
-            response = stub.CreateKey(iam_manager.CreateKeyRequest(type=cert_type, password=password, node_id=node_id))
-            user_creds = UnitCertificate()
-            user_creds.cert_type = response.type
-            user_creds.node_id = response.node_id
-            user_creds.csr = response.csr
-            print_done()
-            return user_creds
-
-    def apply_certificate(self, unit_cert: UnitCertificate):
-        with self.unit_certificate_stub() as stub:
-            node_id = ''
-            if unit_cert.node_id:
-                node_id = str(unit_cert.node_id)
-            print_left(f'Applying certificate type: {unit_cert.cert_type} Node ID: {node_id}...')
-            stub.ApplyCert(iam_manager.ApplyCertRequest(
-                type=unit_cert.cert_type,
-                cert=unit_cert.certificate,
-                node_id=node_id,
-            ))
-            print_done()
-
-    def encrypt_disk(self, password: str, node_id: str = ''):
-        print_left(f'Starting disk encryption on node {node_id}...')
-        with self.unit_provisioning_stub(wait_for_close=False) as stub:
-            stub.EncryptDisk(iam_manager.EncryptDiskRequest(password=password, node_id=node_id))
-            print_done()
-
-    def finish_provisioning(self):
-        with self.unit_provisioning_stub(True) as stub:
-            print_left('Finishing provisioning...')
-            stub.FinishProvisioning(empty_pb2.Empty())
-            print_done()
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+from contextlib import contextmanager
+
+import grpc
+from aos_prov.communication.unit.v4.generated import iamanager_pb2 as iam_manager
+from aos_prov.communication.unit.v4.generated import (
+    iamanager_pb2_grpc as iam_manager_grpc,
+)
+from aos_prov.utils.common import print_done, print_left, print_success
+from aos_prov.utils.errors import GrpcUnimplemented, UnitError
+from aos_prov.utils.unit_certificate import UnitCertificate
+from google.protobuf import empty_pb2
+
+UNIT_DEFAULT_PORT = 8089
+_MAX_PORT = 65535
+
+
+class UnitCommunicationV4:
+    def __init__(self, address: str = 'localhost:8089'):
+        self._need_set_users = False
+
+        if not address:
+            address = 'localhost:8089'
+
+        parts = address.split(':')
+        if len(parts) == 2:
+            try:
+                port = int(parts[1])
+                if port not in range(1, _MAX_PORT):
+                    raise UnitError('Unit port is invalid')
+            except ValueError as exc:
+                raise UnitError('Unit port is invalid') from exc
+        else:
+            address = address + ':' + str(UNIT_DEFAULT_PORT)
+        self._unit_address = address
+
+    @property
+    def need_set_users(self):
+        return self._need_set_users
+
+    @need_set_users.setter
+    def need_set_users(self, set_users):
+        self._need_set_users = set_users
+
+    @contextmanager
+    def unit_certificate_stub(self, catch_inactive=False, wait_for_close=False):
+        try:
+            with grpc.insecure_channel(self._unit_address) as channel:
+                stub = iam_manager_grpc.IAMCertificateServiceStub(channel)
+                if wait_for_close:
+                    def _stop_wait(state):  # noqa: WPS430
+                        if state is grpc.ChannelConnectivity.SHUTDOWN:
+                            channel.unsubscribe(_stop_wait)
+                            return
+                    channel.subscribe(_stop_wait, try_to_connect=False)
+                yield stub
+
+        except grpc.RpcError as exc:
+            e_code = exc.code()
+            e_detail = exc.details()
+            if catch_inactive and not (e_code == grpc.StatusCode.UNAVAILABLE.value and e_detail == 'Socket closed'):
+                return
+            if wait_for_close and (e_code == grpc.StatusCode.UNKNOWN.value and e_detail == 'Stream removed'):
+                return
+            raise UnitError(f'FAILED! Error occurred: \n{e_code}: {e_detail}') from exc
+
+    @contextmanager
+    def unit_identify_stub(self):
+        try:
+            with grpc.insecure_channel(self._unit_address) as channel:
+                stub = iam_manager_grpc.IAMPublicIdentityServiceStub(channel)
+                yield stub
+
+        except grpc.RpcError as exc:
+            e_code = exc.code()
+            e_detail = exc.details()
+            if e_code.value == grpc.StatusCode.UNIMPLEMENTED.value:
+                raise GrpcUnimplemented(f'Protocol V4 is not supported: \n{e_code}: {e_detail}') from exc
+            raise UnitError(f'FAILED! Error occurred: \n{e_code}: {e_detail}') from exc
+
+    @contextmanager
+    def unit_provisioning_stub(self, catch_inactive=False, wait_for_close=False):
+        try:
+            with grpc.insecure_channel(self._unit_address) as channel:
+                stub = iam_manager_grpc.IAMProvisioningServiceStub(channel)
+                if wait_for_close:
+                    def _stop_wait(state):  # noqa: WPS430
+                        if state is grpc.ChannelConnectivity.SHUTDOWN:
+                            channel.unsubscribe(_stop_wait)
+                            return
+                    channel.subscribe(_stop_wait, try_to_connect=False)
+                yield stub
+
+        except grpc.RpcError as exc:
+            e_code = exc.code()
+            e_detail = exc.details()
+            if catch_inactive and not (e_code == grpc.StatusCode.UNAVAILABLE.value and e_detail == 'Socket closed'):
+                return
+            if wait_for_close and (e_code == grpc.StatusCode.UNKNOWN.value and e_detail == 'Stream removed'):
+                return
+            raise UnitError(f'FAILED! Error occurred: \n{e_code}: {e_detail}') from exc
+
+    @contextmanager
+    def unit_public_stub(self):
+        try:
+            with grpc.insecure_channel(self._unit_address) as channel:
+                stub = iam_manager_grpc.IAMPublicServiceStub(channel)
+                yield stub
+
+        except grpc.RpcError as exc:
+            e_code = exc.code()
+            e_detail = exc.details()
+            if e_code.value == grpc.StatusCode.UNIMPLEMENTED.value:
+                raise GrpcUnimplemented(f'Protocol V4 is not supported: \n{e_code}: {e_detail}') from exc
+            raise UnitError(f'FAILED! Error occurred: \n{e_code}: {e_detail}') from exc
+
+    def get_protocol_version(self) -> int:
+        with self.unit_public_stub() as stub:
+            print_left('Getting protocol version...')
+            response = stub.GetAPIVersion(empty_pb2.Empty())
+            print_success(str(response.version))
+            return int(response.version)
+
+    def get_system_info(self) -> (str, str):
+        with self.unit_identify_stub() as stub:
+            print_left('Getting System Info...')
+            response = stub.GetSystemInfo(empty_pb2.Empty())
+            print_done()
+            print_left('System ID:')
+            print_success(response.system_id)
+            print_left('Model name:')
+            print_success(response.board_model)
+            return response.system_id, response.board_model
+
+    def clear(self, certificate_type: str, node_id: str = '') -> None:
+        with self.unit_provisioning_stub() as stub:
+            print_left(f'Clearing certificate: {certificate_type} on Node ID: {node_id}...')
+            response = stub.Clear(iam_manager.ClearRequest(type=certificate_type, node_id=node_id))
+            print_done()
+            return response
+
+    def set_cert_owner(self, certificate_type: str, password: str, node_id: str = '') -> None:
+        with self.unit_provisioning_stub() as stub:
+            print_left(f'Setting owner for: {certificate_type} on Node ID: {node_id}...')
+            response = stub.SetOwner(
+                iam_manager.SetOwnerRequest(type=certificate_type, password=password, node_id=node_id),
+            )
+            print_done()
+            return response
+
+    def get_all_node_ids(self) -> [str]:
+        with self.unit_provisioning_stub() as stub:
+            print_left('Getting Node IDs...')
+            response = stub.GetAllNodeIDs(empty_pb2.Empty())
+            print_success(response.ids)
+            return response.ids
+
+    def get_cert_types(self, node_id: str = '') -> [str]:
+        with self.unit_provisioning_stub() as stub:
+            print_left(f'Getting certificate types to renew on node {node_id}...')
+            response = stub.GetCertTypes(iam_manager.GetCertTypesRequest(node_id=node_id))
+            print_success(response.types)
+            return response.types
+
+    def create_keys(self, cert_type: str, password: str, node_id: str = '') -> UnitCertificate:
+        with self.unit_certificate_stub() as stub:
+            print_left(f'Generating key type: {cert_type} on Node: {node_id}...')
+            response = stub.CreateKey(iam_manager.CreateKeyRequest(type=cert_type, password=password, node_id=node_id))
+            user_creds = UnitCertificate()
+            user_creds.cert_type = response.type
+            user_creds.node_id = response.node_id
+            user_creds.csr = response.csr
+            print_done()
+            return user_creds
+
+    def apply_certificate(self, unit_cert: UnitCertificate):
+        with self.unit_certificate_stub() as stub:
+            node_id = ''
+            if unit_cert.node_id:
+                node_id = str(unit_cert.node_id)
+            print_left(f'Applying certificate type: {unit_cert.cert_type} Node ID: {node_id}...')
+            stub.ApplyCert(iam_manager.ApplyCertRequest(
+                type=unit_cert.cert_type,
+                cert=unit_cert.certificate,
+                node_id=node_id,
+            ))
+            print_done()
+
+    def encrypt_disk(self, password: str, node_id: str = ''):
+        print_left(f'Starting disk encryption on node {node_id}...')
+        with self.unit_provisioning_stub(wait_for_close=False) as stub:
+            stub.EncryptDisk(iam_manager.EncryptDiskRequest(password=password, node_id=node_id))
+            print_done()
+
+    def finish_provisioning(self):
+        with self.unit_provisioning_stub(True) as stub:
+            print_left('Finishing provisioning...')
+            stub.FinishProvisioning(empty_pb2.Empty())
+            print_done()
```

## aos_prov/communication/unit/v4/generated/iamanager_pb2.py

 * *Ordering differences only*

```diff
@@ -1,299 +1,299 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: iamanager/v4/iamanager.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ciamanager/v4/iamanager.proto\x12\x0ciamanager.v4\x1a\x1bgoogle/protobuf/empty.proto\"\x1d\n\nAPIVersion\x12\x0f\n\x07version\x18\x01 \x01(\x04\"\x19\n\x06NodeID\x12\x0f\n\x07node_id\x18\x01 \x01(\t\">\n\x0eGetCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"B\n\x0fGetCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\"4\n\nSystemInfo\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t\"\x1c\n\x08Subjects\x12\x10\n\x08subjects\x18\x01 \x03(\t\"B\n\x12PermissionsRequest\x12\x0e\n\x06secret\x18\x01 \x01(\t\x12\x1c\n\x14\x66unctional_server_id\x18\x02 \x01(\t\"I\n\rInstanceIdent\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12\x12\n\nsubject_id\x18\x02 \x01(\t\x12\x10\n\x08instance\x18\x03 \x01(\x04\"t\n\x13PermissionsResponse\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent\x12.\n\x0bpermissions\x18\x02 \x01(\x0b\x32\x19.iamanager.v4.Permissions\"\x16\n\x07NodesID\x12\x0b\n\x03ids\x18\x01 \x03(\t\"&\n\x13GetCertTypesRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\"\x1a\n\tCertTypes\x12\r\n\x05types\x18\x01 \x03(\t\"B\n\x0fSetOwnerRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"-\n\x0c\x43learRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"7\n\x12\x45ncryptDiskRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"T\n\x10\x43reateKeyRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\"?\n\x11\x43reateKeyResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03\x63sr\x18\x03 \x01(\t\"?\n\x10\x41pplyCertRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x03 \x01(\t\"D\n\x11\x41pplyCertResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x03 \x01(\t\"\x82\x01\n\x0bPermissions\x12?\n\x0bpermissions\x18\x01 \x03(\x0b\x32*.iamanager.v4.Permissions.PermissionsEntry\x1a\x32\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe4\x01\n\x17RegisterInstanceRequest\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent\x12K\n\x0bpermissions\x18\x02 \x03(\x0b\x32\x36.iamanager.v4.RegisterInstanceRequest.PermissionsEntry\x1aM\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.iamanager.v4.Permissions:\x02\x38\x01\"*\n\x18RegisterInstanceResponse\x12\x0e\n\x06secret\x18\x01 \x01(\t\"J\n\x19UnregisterInstanceRequest\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent2\xde\x01\n\x10IAMPublicService\x12\x43\n\rGetAPIVersion\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v4.APIVersion\"\x00\x12;\n\tGetNodeID\x12\x16.google.protobuf.Empty\x1a\x14.iamanager.v4.NodeID\"\x00\x12H\n\x07GetCert\x12\x1c.iamanager.v4.GetCertRequest\x1a\x1d.iamanager.v4.GetCertResponse\"\x00\x32\xf0\x01\n\x18IAMPublicIdentityService\x12\x43\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v4.SystemInfo\"\x00\x12?\n\x0bGetSubjects\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.v4.Subjects\"\x00\x12N\n\x18SubscribeSubjectsChanged\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.v4.Subjects\"\x00\x30\x01\x32v\n\x1bIAMPublicPermissionsService\x12W\n\x0eGetPermissions\x12 .iamanager.v4.PermissionsRequest\x1a!.iamanager.v4.PermissionsResponse\"\x00\x32\xbf\x03\n\x16IAMProvisioningService\x12@\n\rGetAllNodeIDs\x12\x16.google.protobuf.Empty\x1a\x15.iamanager.v4.NodesID\"\x00\x12L\n\x0cGetCertTypes\x12!.iamanager.v4.GetCertTypesRequest\x1a\x17.iamanager.v4.CertTypes\"\x00\x12\x43\n\x08SetOwner\x12\x1d.iamanager.v4.SetOwnerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x05\x43lear\x12\x1a.iamanager.v4.ClearRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0b\x45ncryptDisk\x12 .iamanager.v4.EncryptDiskRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x32\xb7\x01\n\x15IAMCertificateService\x12N\n\tCreateKey\x12\x1e.iamanager.v4.CreateKeyRequest\x1a\x1f.iamanager.v4.CreateKeyResponse\"\x00\x12N\n\tApplyCert\x12\x1e.iamanager.v4.ApplyCertRequest\x1a\x1f.iamanager.v4.ApplyCertResponse\"\x00\x32\xd5\x01\n\x15IAMPermissionsService\x12\x63\n\x10RegisterInstance\x12%.iamanager.v4.RegisterInstanceRequest\x1a&.iamanager.v4.RegisterInstanceResponse\"\x00\x12W\n\x12UnregisterInstance\x12\'.iamanager.v4.UnregisterInstanceRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
-
-
-
-_APIVERSION = DESCRIPTOR.message_types_by_name['APIVersion']
-_NODEID = DESCRIPTOR.message_types_by_name['NodeID']
-_GETCERTREQUEST = DESCRIPTOR.message_types_by_name['GetCertRequest']
-_GETCERTRESPONSE = DESCRIPTOR.message_types_by_name['GetCertResponse']
-_SYSTEMINFO = DESCRIPTOR.message_types_by_name['SystemInfo']
-_SUBJECTS = DESCRIPTOR.message_types_by_name['Subjects']
-_PERMISSIONSREQUEST = DESCRIPTOR.message_types_by_name['PermissionsRequest']
-_INSTANCEIDENT = DESCRIPTOR.message_types_by_name['InstanceIdent']
-_PERMISSIONSRESPONSE = DESCRIPTOR.message_types_by_name['PermissionsResponse']
-_NODESID = DESCRIPTOR.message_types_by_name['NodesID']
-_GETCERTTYPESREQUEST = DESCRIPTOR.message_types_by_name['GetCertTypesRequest']
-_CERTTYPES = DESCRIPTOR.message_types_by_name['CertTypes']
-_SETOWNERREQUEST = DESCRIPTOR.message_types_by_name['SetOwnerRequest']
-_CLEARREQUEST = DESCRIPTOR.message_types_by_name['ClearRequest']
-_ENCRYPTDISKREQUEST = DESCRIPTOR.message_types_by_name['EncryptDiskRequest']
-_CREATEKEYREQUEST = DESCRIPTOR.message_types_by_name['CreateKeyRequest']
-_CREATEKEYRESPONSE = DESCRIPTOR.message_types_by_name['CreateKeyResponse']
-_APPLYCERTREQUEST = DESCRIPTOR.message_types_by_name['ApplyCertRequest']
-_APPLYCERTRESPONSE = DESCRIPTOR.message_types_by_name['ApplyCertResponse']
-_PERMISSIONS = DESCRIPTOR.message_types_by_name['Permissions']
-_PERMISSIONS_PERMISSIONSENTRY = _PERMISSIONS.nested_types_by_name['PermissionsEntry']
-_REGISTERINSTANCEREQUEST = DESCRIPTOR.message_types_by_name['RegisterInstanceRequest']
-_REGISTERINSTANCEREQUEST_PERMISSIONSENTRY = _REGISTERINSTANCEREQUEST.nested_types_by_name['PermissionsEntry']
-_REGISTERINSTANCERESPONSE = DESCRIPTOR.message_types_by_name['RegisterInstanceResponse']
-_UNREGISTERINSTANCEREQUEST = DESCRIPTOR.message_types_by_name['UnregisterInstanceRequest']
-APIVersion = _reflection.GeneratedProtocolMessageType('APIVersion', (_message.Message,), {
-  'DESCRIPTOR' : _APIVERSION,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.APIVersion)
-  })
-_sym_db.RegisterMessage(APIVersion)
-
-NodeID = _reflection.GeneratedProtocolMessageType('NodeID', (_message.Message,), {
-  'DESCRIPTOR' : _NODEID,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.NodeID)
-  })
-_sym_db.RegisterMessage(NodeID)
-
-GetCertRequest = _reflection.GeneratedProtocolMessageType('GetCertRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertRequest)
-  })
-_sym_db.RegisterMessage(GetCertRequest)
-
-GetCertResponse = _reflection.GeneratedProtocolMessageType('GetCertResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTRESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertResponse)
-  })
-_sym_db.RegisterMessage(GetCertResponse)
-
-SystemInfo = _reflection.GeneratedProtocolMessageType('SystemInfo', (_message.Message,), {
-  'DESCRIPTOR' : _SYSTEMINFO,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.SystemInfo)
-  })
-_sym_db.RegisterMessage(SystemInfo)
-
-Subjects = _reflection.GeneratedProtocolMessageType('Subjects', (_message.Message,), {
-  'DESCRIPTOR' : _SUBJECTS,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.Subjects)
-  })
-_sym_db.RegisterMessage(Subjects)
-
-PermissionsRequest = _reflection.GeneratedProtocolMessageType('PermissionsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _PERMISSIONSREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.PermissionsRequest)
-  })
-_sym_db.RegisterMessage(PermissionsRequest)
-
-InstanceIdent = _reflection.GeneratedProtocolMessageType('InstanceIdent', (_message.Message,), {
-  'DESCRIPTOR' : _INSTANCEIDENT,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.InstanceIdent)
-  })
-_sym_db.RegisterMessage(InstanceIdent)
-
-PermissionsResponse = _reflection.GeneratedProtocolMessageType('PermissionsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _PERMISSIONSRESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.PermissionsResponse)
-  })
-_sym_db.RegisterMessage(PermissionsResponse)
-
-NodesID = _reflection.GeneratedProtocolMessageType('NodesID', (_message.Message,), {
-  'DESCRIPTOR' : _NODESID,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.NodesID)
-  })
-_sym_db.RegisterMessage(NodesID)
-
-GetCertTypesRequest = _reflection.GeneratedProtocolMessageType('GetCertTypesRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTTYPESREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertTypesRequest)
-  })
-_sym_db.RegisterMessage(GetCertTypesRequest)
-
-CertTypes = _reflection.GeneratedProtocolMessageType('CertTypes', (_message.Message,), {
-  'DESCRIPTOR' : _CERTTYPES,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.CertTypes)
-  })
-_sym_db.RegisterMessage(CertTypes)
-
-SetOwnerRequest = _reflection.GeneratedProtocolMessageType('SetOwnerRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SETOWNERREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.SetOwnerRequest)
-  })
-_sym_db.RegisterMessage(SetOwnerRequest)
-
-ClearRequest = _reflection.GeneratedProtocolMessageType('ClearRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CLEARREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.ClearRequest)
-  })
-_sym_db.RegisterMessage(ClearRequest)
-
-EncryptDiskRequest = _reflection.GeneratedProtocolMessageType('EncryptDiskRequest', (_message.Message,), {
-  'DESCRIPTOR' : _ENCRYPTDISKREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.EncryptDiskRequest)
-  })
-_sym_db.RegisterMessage(EncryptDiskRequest)
-
-CreateKeyRequest = _reflection.GeneratedProtocolMessageType('CreateKeyRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.CreateKeyRequest)
-  })
-_sym_db.RegisterMessage(CreateKeyRequest)
-
-CreateKeyResponse = _reflection.GeneratedProtocolMessageType('CreateKeyResponse', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYRESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.CreateKeyResponse)
-  })
-_sym_db.RegisterMessage(CreateKeyResponse)
-
-ApplyCertRequest = _reflection.GeneratedProtocolMessageType('ApplyCertRequest', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.ApplyCertRequest)
-  })
-_sym_db.RegisterMessage(ApplyCertRequest)
-
-ApplyCertResponse = _reflection.GeneratedProtocolMessageType('ApplyCertResponse', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTRESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.ApplyCertResponse)
-  })
-_sym_db.RegisterMessage(ApplyCertResponse)
-
-Permissions = _reflection.GeneratedProtocolMessageType('Permissions', (_message.Message,), {
-
-  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _PERMISSIONS_PERMISSIONSENTRY,
-    '__module__' : 'iamanager.v4.iamanager_pb2'
-    # @@protoc_insertion_point(class_scope:iamanager.v4.Permissions.PermissionsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _PERMISSIONS,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.Permissions)
-  })
-_sym_db.RegisterMessage(Permissions)
-_sym_db.RegisterMessage(Permissions.PermissionsEntry)
-
-RegisterInstanceRequest = _reflection.GeneratedProtocolMessageType('RegisterInstanceRequest', (_message.Message,), {
-
-  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY,
-    '__module__' : 'iamanager.v4.iamanager_pb2'
-    # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceRequest.PermissionsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _REGISTERINSTANCEREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceRequest)
-  })
-_sym_db.RegisterMessage(RegisterInstanceRequest)
-_sym_db.RegisterMessage(RegisterInstanceRequest.PermissionsEntry)
-
-RegisterInstanceResponse = _reflection.GeneratedProtocolMessageType('RegisterInstanceResponse', (_message.Message,), {
-  'DESCRIPTOR' : _REGISTERINSTANCERESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceResponse)
-  })
-_sym_db.RegisterMessage(RegisterInstanceResponse)
-
-UnregisterInstanceRequest = _reflection.GeneratedProtocolMessageType('UnregisterInstanceRequest', (_message.Message,), {
-  'DESCRIPTOR' : _UNREGISTERINSTANCEREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.UnregisterInstanceRequest)
-  })
-_sym_db.RegisterMessage(UnregisterInstanceRequest)
-
-_IAMPUBLICSERVICE = DESCRIPTOR.services_by_name['IAMPublicService']
-_IAMPUBLICIDENTITYSERVICE = DESCRIPTOR.services_by_name['IAMPublicIdentityService']
-_IAMPUBLICPERMISSIONSSERVICE = DESCRIPTOR.services_by_name['IAMPublicPermissionsService']
-_IAMPROVISIONINGSERVICE = DESCRIPTOR.services_by_name['IAMProvisioningService']
-_IAMCERTIFICATESERVICE = DESCRIPTOR.services_by_name['IAMCertificateService']
-_IAMPERMISSIONSSERVICE = DESCRIPTOR.services_by_name['IAMPermissionsService']
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  _PERMISSIONS_PERMISSIONSENTRY._options = None
-  _PERMISSIONS_PERMISSIONSENTRY._serialized_options = b'8\001'
-  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._options = None
-  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_options = b'8\001'
-  _APIVERSION._serialized_start=75
-  _APIVERSION._serialized_end=104
-  _NODEID._serialized_start=106
-  _NODEID._serialized_end=131
-  _GETCERTREQUEST._serialized_start=133
-  _GETCERTREQUEST._serialized_end=195
-  _GETCERTRESPONSE._serialized_start=197
-  _GETCERTRESPONSE._serialized_end=263
-  _SYSTEMINFO._serialized_start=265
-  _SYSTEMINFO._serialized_end=317
-  _SUBJECTS._serialized_start=319
-  _SUBJECTS._serialized_end=347
-  _PERMISSIONSREQUEST._serialized_start=349
-  _PERMISSIONSREQUEST._serialized_end=415
-  _INSTANCEIDENT._serialized_start=417
-  _INSTANCEIDENT._serialized_end=490
-  _PERMISSIONSRESPONSE._serialized_start=492
-  _PERMISSIONSRESPONSE._serialized_end=608
-  _NODESID._serialized_start=610
-  _NODESID._serialized_end=632
-  _GETCERTTYPESREQUEST._serialized_start=634
-  _GETCERTTYPESREQUEST._serialized_end=672
-  _CERTTYPES._serialized_start=674
-  _CERTTYPES._serialized_end=700
-  _SETOWNERREQUEST._serialized_start=702
-  _SETOWNERREQUEST._serialized_end=768
-  _CLEARREQUEST._serialized_start=770
-  _CLEARREQUEST._serialized_end=815
-  _ENCRYPTDISKREQUEST._serialized_start=817
-  _ENCRYPTDISKREQUEST._serialized_end=872
-  _CREATEKEYREQUEST._serialized_start=874
-  _CREATEKEYREQUEST._serialized_end=958
-  _CREATEKEYRESPONSE._serialized_start=960
-  _CREATEKEYRESPONSE._serialized_end=1023
-  _APPLYCERTREQUEST._serialized_start=1025
-  _APPLYCERTREQUEST._serialized_end=1088
-  _APPLYCERTRESPONSE._serialized_start=1090
-  _APPLYCERTRESPONSE._serialized_end=1158
-  _PERMISSIONS._serialized_start=1161
-  _PERMISSIONS._serialized_end=1291
-  _PERMISSIONS_PERMISSIONSENTRY._serialized_start=1241
-  _PERMISSIONS_PERMISSIONSENTRY._serialized_end=1291
-  _REGISTERINSTANCEREQUEST._serialized_start=1294
-  _REGISTERINSTANCEREQUEST._serialized_end=1522
-  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_start=1445
-  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_end=1522
-  _REGISTERINSTANCERESPONSE._serialized_start=1524
-  _REGISTERINSTANCERESPONSE._serialized_end=1566
-  _UNREGISTERINSTANCEREQUEST._serialized_start=1568
-  _UNREGISTERINSTANCEREQUEST._serialized_end=1642
-  _IAMPUBLICSERVICE._serialized_start=1645
-  _IAMPUBLICSERVICE._serialized_end=1867
-  _IAMPUBLICIDENTITYSERVICE._serialized_start=1870
-  _IAMPUBLICIDENTITYSERVICE._serialized_end=2110
-  _IAMPUBLICPERMISSIONSSERVICE._serialized_start=2112
-  _IAMPUBLICPERMISSIONSSERVICE._serialized_end=2230
-  _IAMPROVISIONINGSERVICE._serialized_start=2233
-  _IAMPROVISIONINGSERVICE._serialized_end=2680
-  _IAMCERTIFICATESERVICE._serialized_start=2683
-  _IAMCERTIFICATESERVICE._serialized_end=2866
-  _IAMPERMISSIONSSERVICE._serialized_start=2869
-  _IAMPERMISSIONSSERVICE._serialized_end=3082
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: iamanager/v4/iamanager.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ciamanager/v4/iamanager.proto\x12\x0ciamanager.v4\x1a\x1bgoogle/protobuf/empty.proto\"\x1d\n\nAPIVersion\x12\x0f\n\x07version\x18\x01 \x01(\x04\"\x19\n\x06NodeID\x12\x0f\n\x07node_id\x18\x01 \x01(\t\">\n\x0eGetCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"B\n\x0fGetCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\"4\n\nSystemInfo\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t\"\x1c\n\x08Subjects\x12\x10\n\x08subjects\x18\x01 \x03(\t\"B\n\x12PermissionsRequest\x12\x0e\n\x06secret\x18\x01 \x01(\t\x12\x1c\n\x14\x66unctional_server_id\x18\x02 \x01(\t\"I\n\rInstanceIdent\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12\x12\n\nsubject_id\x18\x02 \x01(\t\x12\x10\n\x08instance\x18\x03 \x01(\x04\"t\n\x13PermissionsResponse\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent\x12.\n\x0bpermissions\x18\x02 \x01(\x0b\x32\x19.iamanager.v4.Permissions\"\x16\n\x07NodesID\x12\x0b\n\x03ids\x18\x01 \x03(\t\"&\n\x13GetCertTypesRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\"\x1a\n\tCertTypes\x12\r\n\x05types\x18\x01 \x03(\t\"B\n\x0fSetOwnerRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"-\n\x0c\x43learRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"7\n\x12\x45ncryptDiskRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"T\n\x10\x43reateKeyRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\"?\n\x11\x43reateKeyResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03\x63sr\x18\x03 \x01(\t\"?\n\x10\x41pplyCertRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x03 \x01(\t\"D\n\x11\x41pplyCertResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x03 \x01(\t\"\x82\x01\n\x0bPermissions\x12?\n\x0bpermissions\x18\x01 \x03(\x0b\x32*.iamanager.v4.Permissions.PermissionsEntry\x1a\x32\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe4\x01\n\x17RegisterInstanceRequest\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent\x12K\n\x0bpermissions\x18\x02 \x03(\x0b\x32\x36.iamanager.v4.RegisterInstanceRequest.PermissionsEntry\x1aM\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.iamanager.v4.Permissions:\x02\x38\x01\"*\n\x18RegisterInstanceResponse\x12\x0e\n\x06secret\x18\x01 \x01(\t\"J\n\x19UnregisterInstanceRequest\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent2\xde\x01\n\x10IAMPublicService\x12\x43\n\rGetAPIVersion\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v4.APIVersion\"\x00\x12;\n\tGetNodeID\x12\x16.google.protobuf.Empty\x1a\x14.iamanager.v4.NodeID\"\x00\x12H\n\x07GetCert\x12\x1c.iamanager.v4.GetCertRequest\x1a\x1d.iamanager.v4.GetCertResponse\"\x00\x32\xf0\x01\n\x18IAMPublicIdentityService\x12\x43\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v4.SystemInfo\"\x00\x12?\n\x0bGetSubjects\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.v4.Subjects\"\x00\x12N\n\x18SubscribeSubjectsChanged\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.v4.Subjects\"\x00\x30\x01\x32v\n\x1bIAMPublicPermissionsService\x12W\n\x0eGetPermissions\x12 .iamanager.v4.PermissionsRequest\x1a!.iamanager.v4.PermissionsResponse\"\x00\x32\xbf\x03\n\x16IAMProvisioningService\x12@\n\rGetAllNodeIDs\x12\x16.google.protobuf.Empty\x1a\x15.iamanager.v4.NodesID\"\x00\x12L\n\x0cGetCertTypes\x12!.iamanager.v4.GetCertTypesRequest\x1a\x17.iamanager.v4.CertTypes\"\x00\x12\x43\n\x08SetOwner\x12\x1d.iamanager.v4.SetOwnerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x05\x43lear\x12\x1a.iamanager.v4.ClearRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0b\x45ncryptDisk\x12 .iamanager.v4.EncryptDiskRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x32\xb7\x01\n\x15IAMCertificateService\x12N\n\tCreateKey\x12\x1e.iamanager.v4.CreateKeyRequest\x1a\x1f.iamanager.v4.CreateKeyResponse\"\x00\x12N\n\tApplyCert\x12\x1e.iamanager.v4.ApplyCertRequest\x1a\x1f.iamanager.v4.ApplyCertResponse\"\x00\x32\xd5\x01\n\x15IAMPermissionsService\x12\x63\n\x10RegisterInstance\x12%.iamanager.v4.RegisterInstanceRequest\x1a&.iamanager.v4.RegisterInstanceResponse\"\x00\x12W\n\x12UnregisterInstance\x12\'.iamanager.v4.UnregisterInstanceRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
+
+
+
+_APIVERSION = DESCRIPTOR.message_types_by_name['APIVersion']
+_NODEID = DESCRIPTOR.message_types_by_name['NodeID']
+_GETCERTREQUEST = DESCRIPTOR.message_types_by_name['GetCertRequest']
+_GETCERTRESPONSE = DESCRIPTOR.message_types_by_name['GetCertResponse']
+_SYSTEMINFO = DESCRIPTOR.message_types_by_name['SystemInfo']
+_SUBJECTS = DESCRIPTOR.message_types_by_name['Subjects']
+_PERMISSIONSREQUEST = DESCRIPTOR.message_types_by_name['PermissionsRequest']
+_INSTANCEIDENT = DESCRIPTOR.message_types_by_name['InstanceIdent']
+_PERMISSIONSRESPONSE = DESCRIPTOR.message_types_by_name['PermissionsResponse']
+_NODESID = DESCRIPTOR.message_types_by_name['NodesID']
+_GETCERTTYPESREQUEST = DESCRIPTOR.message_types_by_name['GetCertTypesRequest']
+_CERTTYPES = DESCRIPTOR.message_types_by_name['CertTypes']
+_SETOWNERREQUEST = DESCRIPTOR.message_types_by_name['SetOwnerRequest']
+_CLEARREQUEST = DESCRIPTOR.message_types_by_name['ClearRequest']
+_ENCRYPTDISKREQUEST = DESCRIPTOR.message_types_by_name['EncryptDiskRequest']
+_CREATEKEYREQUEST = DESCRIPTOR.message_types_by_name['CreateKeyRequest']
+_CREATEKEYRESPONSE = DESCRIPTOR.message_types_by_name['CreateKeyResponse']
+_APPLYCERTREQUEST = DESCRIPTOR.message_types_by_name['ApplyCertRequest']
+_APPLYCERTRESPONSE = DESCRIPTOR.message_types_by_name['ApplyCertResponse']
+_PERMISSIONS = DESCRIPTOR.message_types_by_name['Permissions']
+_PERMISSIONS_PERMISSIONSENTRY = _PERMISSIONS.nested_types_by_name['PermissionsEntry']
+_REGISTERINSTANCEREQUEST = DESCRIPTOR.message_types_by_name['RegisterInstanceRequest']
+_REGISTERINSTANCEREQUEST_PERMISSIONSENTRY = _REGISTERINSTANCEREQUEST.nested_types_by_name['PermissionsEntry']
+_REGISTERINSTANCERESPONSE = DESCRIPTOR.message_types_by_name['RegisterInstanceResponse']
+_UNREGISTERINSTANCEREQUEST = DESCRIPTOR.message_types_by_name['UnregisterInstanceRequest']
+APIVersion = _reflection.GeneratedProtocolMessageType('APIVersion', (_message.Message,), {
+  'DESCRIPTOR' : _APIVERSION,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.APIVersion)
+  })
+_sym_db.RegisterMessage(APIVersion)
+
+NodeID = _reflection.GeneratedProtocolMessageType('NodeID', (_message.Message,), {
+  'DESCRIPTOR' : _NODEID,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.NodeID)
+  })
+_sym_db.RegisterMessage(NodeID)
+
+GetCertRequest = _reflection.GeneratedProtocolMessageType('GetCertRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertRequest)
+  })
+_sym_db.RegisterMessage(GetCertRequest)
+
+GetCertResponse = _reflection.GeneratedProtocolMessageType('GetCertResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTRESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertResponse)
+  })
+_sym_db.RegisterMessage(GetCertResponse)
+
+SystemInfo = _reflection.GeneratedProtocolMessageType('SystemInfo', (_message.Message,), {
+  'DESCRIPTOR' : _SYSTEMINFO,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.SystemInfo)
+  })
+_sym_db.RegisterMessage(SystemInfo)
+
+Subjects = _reflection.GeneratedProtocolMessageType('Subjects', (_message.Message,), {
+  'DESCRIPTOR' : _SUBJECTS,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.Subjects)
+  })
+_sym_db.RegisterMessage(Subjects)
+
+PermissionsRequest = _reflection.GeneratedProtocolMessageType('PermissionsRequest', (_message.Message,), {
+  'DESCRIPTOR' : _PERMISSIONSREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.PermissionsRequest)
+  })
+_sym_db.RegisterMessage(PermissionsRequest)
+
+InstanceIdent = _reflection.GeneratedProtocolMessageType('InstanceIdent', (_message.Message,), {
+  'DESCRIPTOR' : _INSTANCEIDENT,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.InstanceIdent)
+  })
+_sym_db.RegisterMessage(InstanceIdent)
+
+PermissionsResponse = _reflection.GeneratedProtocolMessageType('PermissionsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _PERMISSIONSRESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.PermissionsResponse)
+  })
+_sym_db.RegisterMessage(PermissionsResponse)
+
+NodesID = _reflection.GeneratedProtocolMessageType('NodesID', (_message.Message,), {
+  'DESCRIPTOR' : _NODESID,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.NodesID)
+  })
+_sym_db.RegisterMessage(NodesID)
+
+GetCertTypesRequest = _reflection.GeneratedProtocolMessageType('GetCertTypesRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTTYPESREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertTypesRequest)
+  })
+_sym_db.RegisterMessage(GetCertTypesRequest)
+
+CertTypes = _reflection.GeneratedProtocolMessageType('CertTypes', (_message.Message,), {
+  'DESCRIPTOR' : _CERTTYPES,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.CertTypes)
+  })
+_sym_db.RegisterMessage(CertTypes)
+
+SetOwnerRequest = _reflection.GeneratedProtocolMessageType('SetOwnerRequest', (_message.Message,), {
+  'DESCRIPTOR' : _SETOWNERREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.SetOwnerRequest)
+  })
+_sym_db.RegisterMessage(SetOwnerRequest)
+
+ClearRequest = _reflection.GeneratedProtocolMessageType('ClearRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CLEARREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.ClearRequest)
+  })
+_sym_db.RegisterMessage(ClearRequest)
+
+EncryptDiskRequest = _reflection.GeneratedProtocolMessageType('EncryptDiskRequest', (_message.Message,), {
+  'DESCRIPTOR' : _ENCRYPTDISKREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.EncryptDiskRequest)
+  })
+_sym_db.RegisterMessage(EncryptDiskRequest)
+
+CreateKeyRequest = _reflection.GeneratedProtocolMessageType('CreateKeyRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.CreateKeyRequest)
+  })
+_sym_db.RegisterMessage(CreateKeyRequest)
+
+CreateKeyResponse = _reflection.GeneratedProtocolMessageType('CreateKeyResponse', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYRESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.CreateKeyResponse)
+  })
+_sym_db.RegisterMessage(CreateKeyResponse)
+
+ApplyCertRequest = _reflection.GeneratedProtocolMessageType('ApplyCertRequest', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.ApplyCertRequest)
+  })
+_sym_db.RegisterMessage(ApplyCertRequest)
+
+ApplyCertResponse = _reflection.GeneratedProtocolMessageType('ApplyCertResponse', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTRESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.ApplyCertResponse)
+  })
+_sym_db.RegisterMessage(ApplyCertResponse)
+
+Permissions = _reflection.GeneratedProtocolMessageType('Permissions', (_message.Message,), {
+
+  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _PERMISSIONS_PERMISSIONSENTRY,
+    '__module__' : 'iamanager.v4.iamanager_pb2'
+    # @@protoc_insertion_point(class_scope:iamanager.v4.Permissions.PermissionsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _PERMISSIONS,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.Permissions)
+  })
+_sym_db.RegisterMessage(Permissions)
+_sym_db.RegisterMessage(Permissions.PermissionsEntry)
+
+RegisterInstanceRequest = _reflection.GeneratedProtocolMessageType('RegisterInstanceRequest', (_message.Message,), {
+
+  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY,
+    '__module__' : 'iamanager.v4.iamanager_pb2'
+    # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceRequest.PermissionsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _REGISTERINSTANCEREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceRequest)
+  })
+_sym_db.RegisterMessage(RegisterInstanceRequest)
+_sym_db.RegisterMessage(RegisterInstanceRequest.PermissionsEntry)
+
+RegisterInstanceResponse = _reflection.GeneratedProtocolMessageType('RegisterInstanceResponse', (_message.Message,), {
+  'DESCRIPTOR' : _REGISTERINSTANCERESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceResponse)
+  })
+_sym_db.RegisterMessage(RegisterInstanceResponse)
+
+UnregisterInstanceRequest = _reflection.GeneratedProtocolMessageType('UnregisterInstanceRequest', (_message.Message,), {
+  'DESCRIPTOR' : _UNREGISTERINSTANCEREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.UnregisterInstanceRequest)
+  })
+_sym_db.RegisterMessage(UnregisterInstanceRequest)
+
+_IAMPUBLICSERVICE = DESCRIPTOR.services_by_name['IAMPublicService']
+_IAMPUBLICIDENTITYSERVICE = DESCRIPTOR.services_by_name['IAMPublicIdentityService']
+_IAMPUBLICPERMISSIONSSERVICE = DESCRIPTOR.services_by_name['IAMPublicPermissionsService']
+_IAMPROVISIONINGSERVICE = DESCRIPTOR.services_by_name['IAMProvisioningService']
+_IAMCERTIFICATESERVICE = DESCRIPTOR.services_by_name['IAMCertificateService']
+_IAMPERMISSIONSSERVICE = DESCRIPTOR.services_by_name['IAMPermissionsService']
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _PERMISSIONS_PERMISSIONSENTRY._options = None
+  _PERMISSIONS_PERMISSIONSENTRY._serialized_options = b'8\001'
+  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._options = None
+  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_options = b'8\001'
+  _APIVERSION._serialized_start=75
+  _APIVERSION._serialized_end=104
+  _NODEID._serialized_start=106
+  _NODEID._serialized_end=131
+  _GETCERTREQUEST._serialized_start=133
+  _GETCERTREQUEST._serialized_end=195
+  _GETCERTRESPONSE._serialized_start=197
+  _GETCERTRESPONSE._serialized_end=263
+  _SYSTEMINFO._serialized_start=265
+  _SYSTEMINFO._serialized_end=317
+  _SUBJECTS._serialized_start=319
+  _SUBJECTS._serialized_end=347
+  _PERMISSIONSREQUEST._serialized_start=349
+  _PERMISSIONSREQUEST._serialized_end=415
+  _INSTANCEIDENT._serialized_start=417
+  _INSTANCEIDENT._serialized_end=490
+  _PERMISSIONSRESPONSE._serialized_start=492
+  _PERMISSIONSRESPONSE._serialized_end=608
+  _NODESID._serialized_start=610
+  _NODESID._serialized_end=632
+  _GETCERTTYPESREQUEST._serialized_start=634
+  _GETCERTTYPESREQUEST._serialized_end=672
+  _CERTTYPES._serialized_start=674
+  _CERTTYPES._serialized_end=700
+  _SETOWNERREQUEST._serialized_start=702
+  _SETOWNERREQUEST._serialized_end=768
+  _CLEARREQUEST._serialized_start=770
+  _CLEARREQUEST._serialized_end=815
+  _ENCRYPTDISKREQUEST._serialized_start=817
+  _ENCRYPTDISKREQUEST._serialized_end=872
+  _CREATEKEYREQUEST._serialized_start=874
+  _CREATEKEYREQUEST._serialized_end=958
+  _CREATEKEYRESPONSE._serialized_start=960
+  _CREATEKEYRESPONSE._serialized_end=1023
+  _APPLYCERTREQUEST._serialized_start=1025
+  _APPLYCERTREQUEST._serialized_end=1088
+  _APPLYCERTRESPONSE._serialized_start=1090
+  _APPLYCERTRESPONSE._serialized_end=1158
+  _PERMISSIONS._serialized_start=1161
+  _PERMISSIONS._serialized_end=1291
+  _PERMISSIONS_PERMISSIONSENTRY._serialized_start=1241
+  _PERMISSIONS_PERMISSIONSENTRY._serialized_end=1291
+  _REGISTERINSTANCEREQUEST._serialized_start=1294
+  _REGISTERINSTANCEREQUEST._serialized_end=1522
+  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_start=1445
+  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_end=1522
+  _REGISTERINSTANCERESPONSE._serialized_start=1524
+  _REGISTERINSTANCERESPONSE._serialized_end=1566
+  _UNREGISTERINSTANCEREQUEST._serialized_start=1568
+  _UNREGISTERINSTANCEREQUEST._serialized_end=1642
+  _IAMPUBLICSERVICE._serialized_start=1645
+  _IAMPUBLICSERVICE._serialized_end=1867
+  _IAMPUBLICIDENTITYSERVICE._serialized_start=1870
+  _IAMPUBLICIDENTITYSERVICE._serialized_end=2110
+  _IAMPUBLICPERMISSIONSSERVICE._serialized_start=2112
+  _IAMPUBLICPERMISSIONSSERVICE._serialized_end=2230
+  _IAMPROVISIONINGSERVICE._serialized_start=2233
+  _IAMPROVISIONINGSERVICE._serialized_end=2680
+  _IAMCERTIFICATESERVICE._serialized_start=2683
+  _IAMCERTIFICATESERVICE._serialized_end=2866
+  _IAMPERMISSIONSSERVICE._serialized_start=2869
+  _IAMPERMISSIONSSERVICE._serialized_end=3082
+# @@protoc_insertion_point(module_scope)
```

## aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py

 * *Ordering differences only*

```diff
@@ -1,736 +1,736 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-from aos_prov.communication.unit.v4.generated import (
-    iamanager_pb2 as iamanager_dot_v4_dot_iamanager__pb2,
-)
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-
-
-class IAMPublicServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetAPIVersion = channel.unary_unary(
-                '/iamanager.v4.IAMPublicService/GetAPIVersion',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.APIVersion.FromString,
-                )
-        self.GetNodeID = channel.unary_unary(
-                '/iamanager.v4.IAMPublicService/GetNodeID',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.NodeID.FromString,
-                )
-        self.GetCert = channel.unary_unary(
-                '/iamanager.v4.IAMPublicService/GetCert',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.FromString,
-                )
-
-
-class IAMPublicServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetAPIVersion(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetNodeID(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetCert(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPublicServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetAPIVersion': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAPIVersion,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.APIVersion.SerializeToString,
-            ),
-            'GetNodeID': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetNodeID,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.NodeID.SerializeToString,
-            ),
-            'GetCert': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCert,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMPublicService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPublicService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetAPIVersion(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetAPIVersion',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.APIVersion.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetNodeID(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetNodeID',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.NodeID.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetCert(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetCert',
-            iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMPublicIdentityServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetSystemInfo = channel.unary_unary(
-                '/iamanager.v4.IAMPublicIdentityService/GetSystemInfo',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.FromString,
-                )
-        self.GetSubjects = channel.unary_unary(
-                '/iamanager.v4.IAMPublicIdentityService/GetSubjects',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
-                )
-        self.SubscribeSubjectsChanged = channel.unary_stream(
-                '/iamanager.v4.IAMPublicIdentityService/SubscribeSubjectsChanged',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
-                )
-
-
-class IAMPublicIdentityServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetSystemInfo(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetSubjects(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SubscribeSubjectsChanged(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPublicIdentityServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetSystemInfo': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetSystemInfo,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.SerializeToString,
-            ),
-            'GetSubjects': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetSubjects,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.SerializeToString,
-            ),
-            'SubscribeSubjectsChanged': grpc.unary_stream_rpc_method_handler(
-                    servicer.SubscribeSubjectsChanged,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMPublicIdentityService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPublicIdentityService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetSystemInfo(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicIdentityService/GetSystemInfo',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetSubjects(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicIdentityService/GetSubjects',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SubscribeSubjectsChanged(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/iamanager.v4.IAMPublicIdentityService/SubscribeSubjectsChanged',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMPublicPermissionsServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetPermissions = channel.unary_unary(
-                '/iamanager.v4.IAMPublicPermissionsService/GetPermissions',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.FromString,
-                )
-
-
-class IAMPublicPermissionsServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetPermissions(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPublicPermissionsServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetPermissions': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetPermissions,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMPublicPermissionsService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPublicPermissionsService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetPermissions(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicPermissionsService/GetPermissions',
-            iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMProvisioningServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetAllNodeIDs = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/GetAllNodeIDs',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.NodesID.FromString,
-                )
-        self.GetCertTypes = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/GetCertTypes',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CertTypes.FromString,
-                )
-        self.SetOwner = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/SetOwner',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.Clear = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/Clear',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.EncryptDisk = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/EncryptDisk',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.FinishProvisioning = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/FinishProvisioning',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-
-
-class IAMProvisioningServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetAllNodeIDs(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetCertTypes(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SetOwner(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Clear(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def EncryptDisk(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def FinishProvisioning(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMProvisioningServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetAllNodeIDs': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAllNodeIDs,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.NodesID.SerializeToString,
-            ),
-            'GetCertTypes': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCertTypes,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.CertTypes.SerializeToString,
-            ),
-            'SetOwner': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetOwner,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'Clear': grpc.unary_unary_rpc_method_handler(
-                    servicer.Clear,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'EncryptDisk': grpc.unary_unary_rpc_method_handler(
-                    servicer.EncryptDisk,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'FinishProvisioning': grpc.unary_unary_rpc_method_handler(
-                    servicer.FinishProvisioning,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMProvisioningService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMProvisioningService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetAllNodeIDs(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/GetAllNodeIDs',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.NodesID.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetCertTypes(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/GetCertTypes',
-            iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.CertTypes.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SetOwner(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/SetOwner',
-            iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Clear(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/Clear',
-            iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def EncryptDisk(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/EncryptDisk',
-            iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def FinishProvisioning(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/FinishProvisioning',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMCertificateServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.CreateKey = channel.unary_unary(
-                '/iamanager.v4.IAMCertificateService/CreateKey',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.FromString,
-                )
-        self.ApplyCert = channel.unary_unary(
-                '/iamanager.v4.IAMCertificateService/ApplyCert',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.FromString,
-                )
-
-
-class IAMCertificateServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def CreateKey(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def ApplyCert(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMCertificateServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'CreateKey': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateKey,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.SerializeToString,
-            ),
-            'ApplyCert': grpc.unary_unary_rpc_method_handler(
-                    servicer.ApplyCert,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMCertificateService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMCertificateService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def CreateKey(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMCertificateService/CreateKey',
-            iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ApplyCert(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMCertificateService/ApplyCert',
-            iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMPermissionsServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.RegisterInstance = channel.unary_unary(
-                '/iamanager.v4.IAMPermissionsService/RegisterInstance',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.FromString,
-                )
-        self.UnregisterInstance = channel.unary_unary(
-                '/iamanager.v4.IAMPermissionsService/UnregisterInstance',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-
-
-class IAMPermissionsServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def RegisterInstance(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def UnregisterInstance(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPermissionsServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'RegisterInstance': grpc.unary_unary_rpc_method_handler(
-                    servicer.RegisterInstance,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.SerializeToString,
-            ),
-            'UnregisterInstance': grpc.unary_unary_rpc_method_handler(
-                    servicer.UnregisterInstance,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMPermissionsService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPermissionsService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def RegisterInstance(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPermissionsService/RegisterInstance',
-            iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def UnregisterInstance(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPermissionsService/UnregisterInstance',
-            iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+from aos_prov.communication.unit.v4.generated import (
+    iamanager_pb2 as iamanager_dot_v4_dot_iamanager__pb2,
+)
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+
+
+class IAMPublicServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetAPIVersion = channel.unary_unary(
+                '/iamanager.v4.IAMPublicService/GetAPIVersion',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.APIVersion.FromString,
+                )
+        self.GetNodeID = channel.unary_unary(
+                '/iamanager.v4.IAMPublicService/GetNodeID',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.NodeID.FromString,
+                )
+        self.GetCert = channel.unary_unary(
+                '/iamanager.v4.IAMPublicService/GetCert',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.FromString,
+                )
+
+
+class IAMPublicServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetAPIVersion(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetNodeID(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetCert(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPublicServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetAPIVersion': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAPIVersion,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.APIVersion.SerializeToString,
+            ),
+            'GetNodeID': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetNodeID,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.NodeID.SerializeToString,
+            ),
+            'GetCert': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCert,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMPublicService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPublicService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetAPIVersion(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetAPIVersion',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.APIVersion.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetNodeID(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetNodeID',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.NodeID.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetCert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetCert',
+            iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMPublicIdentityServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetSystemInfo = channel.unary_unary(
+                '/iamanager.v4.IAMPublicIdentityService/GetSystemInfo',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.FromString,
+                )
+        self.GetSubjects = channel.unary_unary(
+                '/iamanager.v4.IAMPublicIdentityService/GetSubjects',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
+                )
+        self.SubscribeSubjectsChanged = channel.unary_stream(
+                '/iamanager.v4.IAMPublicIdentityService/SubscribeSubjectsChanged',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
+                )
+
+
+class IAMPublicIdentityServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetSystemInfo(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetSubjects(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubscribeSubjectsChanged(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPublicIdentityServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetSystemInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSystemInfo,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.SerializeToString,
+            ),
+            'GetSubjects': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSubjects,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.SerializeToString,
+            ),
+            'SubscribeSubjectsChanged': grpc.unary_stream_rpc_method_handler(
+                    servicer.SubscribeSubjectsChanged,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMPublicIdentityService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPublicIdentityService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetSystemInfo(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicIdentityService/GetSystemInfo',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetSubjects(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicIdentityService/GetSubjects',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubscribeSubjectsChanged(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/iamanager.v4.IAMPublicIdentityService/SubscribeSubjectsChanged',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMPublicPermissionsServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetPermissions = channel.unary_unary(
+                '/iamanager.v4.IAMPublicPermissionsService/GetPermissions',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.FromString,
+                )
+
+
+class IAMPublicPermissionsServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetPermissions(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPublicPermissionsServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetPermissions': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetPermissions,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMPublicPermissionsService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPublicPermissionsService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetPermissions(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicPermissionsService/GetPermissions',
+            iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMProvisioningServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetAllNodeIDs = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/GetAllNodeIDs',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.NodesID.FromString,
+                )
+        self.GetCertTypes = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/GetCertTypes',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CertTypes.FromString,
+                )
+        self.SetOwner = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/SetOwner',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.Clear = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/Clear',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.EncryptDisk = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/EncryptDisk',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.FinishProvisioning = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/FinishProvisioning',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+
+
+class IAMProvisioningServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetAllNodeIDs(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetCertTypes(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SetOwner(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Clear(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def EncryptDisk(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def FinishProvisioning(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMProvisioningServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetAllNodeIDs': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAllNodeIDs,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.NodesID.SerializeToString,
+            ),
+            'GetCertTypes': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCertTypes,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.CertTypes.SerializeToString,
+            ),
+            'SetOwner': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetOwner,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'Clear': grpc.unary_unary_rpc_method_handler(
+                    servicer.Clear,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'EncryptDisk': grpc.unary_unary_rpc_method_handler(
+                    servicer.EncryptDisk,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'FinishProvisioning': grpc.unary_unary_rpc_method_handler(
+                    servicer.FinishProvisioning,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMProvisioningService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMProvisioningService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetAllNodeIDs(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/GetAllNodeIDs',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.NodesID.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetCertTypes(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/GetCertTypes',
+            iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.CertTypes.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetOwner(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/SetOwner',
+            iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Clear(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/Clear',
+            iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def EncryptDisk(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/EncryptDisk',
+            iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def FinishProvisioning(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/FinishProvisioning',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMCertificateServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.CreateKey = channel.unary_unary(
+                '/iamanager.v4.IAMCertificateService/CreateKey',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.FromString,
+                )
+        self.ApplyCert = channel.unary_unary(
+                '/iamanager.v4.IAMCertificateService/ApplyCert',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.FromString,
+                )
+
+
+class IAMCertificateServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def CreateKey(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ApplyCert(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMCertificateServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'CreateKey': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateKey,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.SerializeToString,
+            ),
+            'ApplyCert': grpc.unary_unary_rpc_method_handler(
+                    servicer.ApplyCert,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMCertificateService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMCertificateService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def CreateKey(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMCertificateService/CreateKey',
+            iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ApplyCert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMCertificateService/ApplyCert',
+            iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMPermissionsServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.RegisterInstance = channel.unary_unary(
+                '/iamanager.v4.IAMPermissionsService/RegisterInstance',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.FromString,
+                )
+        self.UnregisterInstance = channel.unary_unary(
+                '/iamanager.v4.IAMPermissionsService/UnregisterInstance',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+
+
+class IAMPermissionsServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def RegisterInstance(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def UnregisterInstance(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPermissionsServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'RegisterInstance': grpc.unary_unary_rpc_method_handler(
+                    servicer.RegisterInstance,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.SerializeToString,
+            ),
+            'UnregisterInstance': grpc.unary_unary_rpc_method_handler(
+                    servicer.UnregisterInstance,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMPermissionsService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPermissionsService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def RegisterInstance(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPermissionsService/RegisterInstance',
+            iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UnregisterInstance(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPermissionsService/UnregisterInstance',
+            iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## aos_prov/files/1rootCA.crt

 * *Ordering differences only*

```diff
@@ -1,45 +1,45 @@
------BEGIN CERTIFICATE-----
-MIIEAjCCAuqgAwIBAgIJAPwk2NFfSDPjMA0GCSqGSIb3DQEBCwUAMIGNMRcwFQYD
-VQQDDA5GdXNpb24gUm9vdCBDQTEpMCcGCSqGSIb3DQEJARYadm9sb2R5bXlyX2Jh
-YmNodWtAZXBhbS5jb20xDTALBgNVBAoMBEVQQU0xHDAaBgNVBAsME05vdnVzIE9y
-ZG8gU2VjbG9ydW0xDTALBgNVBAcMBEt5aXYxCzAJBgNVBAYTAlVBMB4XDTE4MDQx
-MDExMzMwMFoXDTI2MDYyNzExMzMwMFowgY0xFzAVBgNVBAMMDkZ1c2lvbiBSb290
-IENBMSkwJwYJKoZIhvcNAQkBFhp2b2xvZHlteXJfYmFiY2h1a0BlcGFtLmNvbTEN
-MAsGA1UECgwERVBBTTEcMBoGA1UECwwTTm92dXMgT3JkbyBTZWNsb3J1bTENMAsG
-A1UEBwwES3lpdjELMAkGA1UEBhMCVUEwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAw
-ggEKAoIBAQC+K2ow2HO7+SUVfOq5tTtmHj4LQijHJ803mLk9pkPef+Glmeyp9HXe
-jDlQC04MeovMBeNTaq0wibf7qas9niXbeXRVzheZIFziMXqRuwLqc0KXdDxIDPTb
-TW3K0HE6M/eAtTfn9+Z/LnkWt4zMXasc02hvufsmIVEuNbc1VhrsJJg5uk88ldPM
-LSF7nff9eYZTHYgCyBkt9aL+fwoXO6eSDSAhjopX3lhdidkM+ni7EOhlN7STmgDM
-WKh9nMjXD5f28PGhtW/dZvn4SzasRE5MeaExIlBmhkWEUgVCyP7LvuQGRUPK+NYz
-FE2CLRuirLCWy1HIt9lLziPjlZ4361mNAgMBAAGjYzBhMB0GA1UdDgQWBBR0Shhz
-OuM95BhD0mWxC1j+KrE6UjAMBgNVHRMEBTADAQH/MAsGA1UdDwQEAwIBBjAlBgNV
-HREEHjAcgRp2b2xvZHlteXJfYmFiY2h1a0BlcGFtLmNvbTANBgkqhkiG9w0BAQsF
-AAOCAQEAl8bv1HTYe3l4Y+g0TVZR7bYL5BNsnGgqy0qS5fu991khXWf+Zwa2MLVn
-YakMnLkjvdHqUpWMJ/S82o2zWGmmuxca56ehjxCiP/nkm4M74yXz2R8cu52WxYnF
-yMvgawzQ6c1yhvZiv/gEE7KdbYRVKLHPgBzfyup21i5ngSlTcMRRS7oOBmoye4qc
-6adq6HtY6X/OnZ9I5xoRN1GcvaLUgUE6igTiVa1pF8kedWhHY7wzTXBxzSvIZkCU
-VHEOzvaGk9miP6nBrDfNv7mIkgEKARrjjSpmJasIEU+mNtzeOIEiMtW1EMRc457o
-0PdFI3jseyLVPVhEzUkuC7mwjb7CeQ==
------END CERTIFICATE-----
------BEGIN CERTIFICATE-----
-MIIDcTCCAlmgAwIBAgIUaAae9+vWnKVtQK/SllTCnikMCfowDQYJKoZIhvcNAQEL
-BQAwQjEUMBIGA1UEAwwLQW9zIFJvb3QgQ0ExDzANBgNVBAoMBk51YW5jZTEMMAoG
-A1UECwwDQW9zMQswCQYDVQQGEwJVUzAgFw0yMDExMTcxMDI4MDNaGA8yMDUwMTEx
-MDEwMjgwM1owQjEUMBIGA1UEAwwLQW9zIFJvb3QgQ0ExDzANBgNVBAoMBk51YW5j
-ZTEMMAoGA1UECwwDQW9zMQswCQYDVQQGEwJVUzCCASIwDQYJKoZIhvcNAQEBBQAD
-ggEPADCCAQoCggEBANsJebKMor2xDlQrA79EfLQ51YncDtZmxLK8+YhLxL/24XSB
-XDToDGLatecrs61EQiSotLO7IlZwB3gfZUKmLdQySgWAiRSihlzvx9m0CHsSfH3e
-rpJLjnjiS6ZJhBkQws+bAViN4yZuQpcKsxygb1wz7arOyl2nYEDMz+hyd8cs7U1H
-0JJgI1pPBULcKeLfCGPGZufB6YeIfPTUP/CE49hbwMuHXhpDc5Ls0SBXWUVfkBME
-JrueMIzJRQwU29N+32PhgbLZuwoTJVi+VcKRfF2ObwsdzcH63dTAiyjCrMYY4gdc
-20ubjdynW7x3gxOWQh0O2ikni/OTxozwX78lrCECAwEAAaNdMFswDAYDVR0TBAUw
-AwEB/zAdBgNVHQ4EFgQUOenD6UbOClI3DMgJ60A2fU7SjY8wHwYDVR0jBBgwFoAU
-OenD6UbOClI3DMgJ60A2fU7SjY8wCwYDVR0PBAQDAgGGMA0GCSqGSIb3DQEBCwUA
-A4IBAQBQQoi68lmEAPmcsIAiX3gilmvueadicZeoBKaKaHFJlL1CAvHWHTLc0GLr
-oL3XqVW5iqeGL8eu3OmiaxPIY4f2zxoAHGLTY3ur/O03GBQE2jBuV6uOpXtNc0d6
-XDp4/w/pMcEdXs7T9O8lLIjyvS+hfoSGd9X4kNKiMa5Smo5U0VoALOMFgRE6VZFf
-Wq2EuuATEx7FCZd4PkcOLsFfoaLteEa2lW45oWIbllMn3eWyo8+C2Q9Rw3kbzIot
-2YbPYkPbsF3E/cR4UZF8jGBneH80Mtk04EwV5obngFBqt3UeZyjVXAhwumZt6R+J
-rFzZldCbm4xj+pRFhy5FCkHIpiPj
------END CERTIFICATE-----
+-----BEGIN CERTIFICATE-----
+MIIEAjCCAuqgAwIBAgIJAPwk2NFfSDPjMA0GCSqGSIb3DQEBCwUAMIGNMRcwFQYD
+VQQDDA5GdXNpb24gUm9vdCBDQTEpMCcGCSqGSIb3DQEJARYadm9sb2R5bXlyX2Jh
+YmNodWtAZXBhbS5jb20xDTALBgNVBAoMBEVQQU0xHDAaBgNVBAsME05vdnVzIE9y
+ZG8gU2VjbG9ydW0xDTALBgNVBAcMBEt5aXYxCzAJBgNVBAYTAlVBMB4XDTE4MDQx
+MDExMzMwMFoXDTI2MDYyNzExMzMwMFowgY0xFzAVBgNVBAMMDkZ1c2lvbiBSb290
+IENBMSkwJwYJKoZIhvcNAQkBFhp2b2xvZHlteXJfYmFiY2h1a0BlcGFtLmNvbTEN
+MAsGA1UECgwERVBBTTEcMBoGA1UECwwTTm92dXMgT3JkbyBTZWNsb3J1bTENMAsG
+A1UEBwwES3lpdjELMAkGA1UEBhMCVUEwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAw
+ggEKAoIBAQC+K2ow2HO7+SUVfOq5tTtmHj4LQijHJ803mLk9pkPef+Glmeyp9HXe
+jDlQC04MeovMBeNTaq0wibf7qas9niXbeXRVzheZIFziMXqRuwLqc0KXdDxIDPTb
+TW3K0HE6M/eAtTfn9+Z/LnkWt4zMXasc02hvufsmIVEuNbc1VhrsJJg5uk88ldPM
+LSF7nff9eYZTHYgCyBkt9aL+fwoXO6eSDSAhjopX3lhdidkM+ni7EOhlN7STmgDM
+WKh9nMjXD5f28PGhtW/dZvn4SzasRE5MeaExIlBmhkWEUgVCyP7LvuQGRUPK+NYz
+FE2CLRuirLCWy1HIt9lLziPjlZ4361mNAgMBAAGjYzBhMB0GA1UdDgQWBBR0Shhz
+OuM95BhD0mWxC1j+KrE6UjAMBgNVHRMEBTADAQH/MAsGA1UdDwQEAwIBBjAlBgNV
+HREEHjAcgRp2b2xvZHlteXJfYmFiY2h1a0BlcGFtLmNvbTANBgkqhkiG9w0BAQsF
+AAOCAQEAl8bv1HTYe3l4Y+g0TVZR7bYL5BNsnGgqy0qS5fu991khXWf+Zwa2MLVn
+YakMnLkjvdHqUpWMJ/S82o2zWGmmuxca56ehjxCiP/nkm4M74yXz2R8cu52WxYnF
+yMvgawzQ6c1yhvZiv/gEE7KdbYRVKLHPgBzfyup21i5ngSlTcMRRS7oOBmoye4qc
+6adq6HtY6X/OnZ9I5xoRN1GcvaLUgUE6igTiVa1pF8kedWhHY7wzTXBxzSvIZkCU
+VHEOzvaGk9miP6nBrDfNv7mIkgEKARrjjSpmJasIEU+mNtzeOIEiMtW1EMRc457o
+0PdFI3jseyLVPVhEzUkuC7mwjb7CeQ==
+-----END CERTIFICATE-----
+-----BEGIN CERTIFICATE-----
+MIIDcTCCAlmgAwIBAgIUaAae9+vWnKVtQK/SllTCnikMCfowDQYJKoZIhvcNAQEL
+BQAwQjEUMBIGA1UEAwwLQW9zIFJvb3QgQ0ExDzANBgNVBAoMBk51YW5jZTEMMAoG
+A1UECwwDQW9zMQswCQYDVQQGEwJVUzAgFw0yMDExMTcxMDI4MDNaGA8yMDUwMTEx
+MDEwMjgwM1owQjEUMBIGA1UEAwwLQW9zIFJvb3QgQ0ExDzANBgNVBAoMBk51YW5j
+ZTEMMAoGA1UECwwDQW9zMQswCQYDVQQGEwJVUzCCASIwDQYJKoZIhvcNAQEBBQAD
+ggEPADCCAQoCggEBANsJebKMor2xDlQrA79EfLQ51YncDtZmxLK8+YhLxL/24XSB
+XDToDGLatecrs61EQiSotLO7IlZwB3gfZUKmLdQySgWAiRSihlzvx9m0CHsSfH3e
+rpJLjnjiS6ZJhBkQws+bAViN4yZuQpcKsxygb1wz7arOyl2nYEDMz+hyd8cs7U1H
+0JJgI1pPBULcKeLfCGPGZufB6YeIfPTUP/CE49hbwMuHXhpDc5Ls0SBXWUVfkBME
+JrueMIzJRQwU29N+32PhgbLZuwoTJVi+VcKRfF2ObwsdzcH63dTAiyjCrMYY4gdc
+20ubjdynW7x3gxOWQh0O2ikni/OTxozwX78lrCECAwEAAaNdMFswDAYDVR0TBAUw
+AwEB/zAdBgNVHQ4EFgQUOenD6UbOClI3DMgJ60A2fU7SjY8wHwYDVR0jBBgwFoAU
+OenD6UbOClI3DMgJ60A2fU7SjY8wCwYDVR0PBAQDAgGGMA0GCSqGSIb3DQEBCwUA
+A4IBAQBQQoi68lmEAPmcsIAiX3gilmvueadicZeoBKaKaHFJlL1CAvHWHTLc0GLr
+oL3XqVW5iqeGL8eu3OmiaxPIY4f2zxoAHGLTY3ur/O03GBQE2jBuV6uOpXtNc0d6
+XDp4/w/pMcEdXs7T9O8lLIjyvS+hfoSGd9X4kNKiMa5Smo5U0VoALOMFgRE6VZFf
+Wq2EuuATEx7FCZd4PkcOLsFfoaLteEa2lW45oWIbllMn3eWyo8+C2Q9Rw3kbzIot
+2YbPYkPbsF3E/cR4UZF8jGBneH80Mtk04EwV5obngFBqt3UeZyjVXAhwumZt6R+J
+rFzZldCbm4xj+pRFhy5FCkHIpiPj
+-----END CERTIFICATE-----
```

## aos_prov/utils/__init__.py

 * *Ordering differences only*

```diff
@@ -1,23 +1,23 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
-
-import os
-
-# SDK home directory name
-SDK_TOOL_DIR_NAME = '.aos'
-# SDK home directory full path
-SDK_FULL_PATH = os.path.join(os.path.expanduser("~"), SDK_TOOL_DIR_NAME)
-# Default directory with user keys and certificates
-SDK_SECURITY_PATH = os.path.join(SDK_FULL_PATH, 'security')
-
-# Default user certificate filename
-USER_CERTIFICATE_FILE_NAME = 'oem-client.pem'
-# Default user key filename
-USER_KEY_FILE_NAME = 'private_key.pem'
-
-# Default user certificate full path
-DEFAULT_USER_CERT_PATH = os.path.join(SDK_SECURITY_PATH, USER_CERTIFICATE_FILE_NAME)
-# Default user key full path
-DEFAULT_USER_KEY_PATH = os.path.join(SDK_SECURITY_PATH, USER_KEY_FILE_NAME)
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
+
+import os
+
+# SDK home directory name
+SDK_TOOL_DIR_NAME = '.aos'
+# SDK home directory full path
+SDK_FULL_PATH = os.path.join(os.path.expanduser("~"), SDK_TOOL_DIR_NAME)
+# Default directory with user keys and certificates
+SDK_SECURITY_PATH = os.path.join(SDK_FULL_PATH, 'security')
+
+# Default user certificate filename
+USER_CERTIFICATE_FILE_NAME = 'oem-client.pem'
+# Default user key filename
+USER_KEY_FILE_NAME = 'private_key.pem'
+
+# Default user certificate full path
+DEFAULT_USER_CERT_PATH = os.path.join(SDK_SECURITY_PATH, USER_CERTIFICATE_FILE_NAME)
+# Default user key full path
+DEFAULT_USER_KEY_PATH = os.path.join(SDK_SECURITY_PATH, USER_KEY_FILE_NAME)
```

## aos_prov/utils/common.py

```diff
@@ -1,61 +1,61 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-
-import random
-import string
-from pathlib import Path
-
-from rich.console import Console
-
-CONTENT_ENCRYPTION_ALGORITHM = 'aes256_cbc'
-DOWNLOADS_PATH = Path.home() / '.aos' / 'downloads'
-AOS_DISKS_PATH = DOWNLOADS_PATH
-IMAGE_WITHOUT_NODES_FILENAME = 'aos-image-vm-genericx86-64_3.0.1.wic.vmdk'
-NODE0_IMAGE_FILENAME = 'aos-vm-node0-genericx86-64.wic.vmdk'
-NODE1_IMAGE_FILENAME = 'aos-vm-node1-genericx86-64.wic.vmdk'
-
-DISK_IMAGE_DOWNLOAD_URL = 'https://d2aa62nq4kg5j3.cloudfront.net/aos-vm-v4.2.1.tar.gz'
-REQUEST_TIMEOUT = 30
-RECONNECT_TIMEOUT = 40
-
-console = Console()
-error_console = Console(stderr=True, style='red')
-ALLOW_PRINT = True
-
-
-def print_message(formatted_text, end='\n', ljust: int = 0):
-    if ALLOW_PRINT:
-        if ljust > 0:
-            formatted_text = formatted_text.ljust(ljust)
-        console.print(formatted_text, end=end)
-
-
-def print_left(formatted_text, ljust=60):
-    print_message(formatted_text, end='', ljust=ljust)
-
-
-def print_done():
-    print_message('[green]DONE')
-
-
-def print_success(message):
-    print_message(f'[green]{str(message)}')  # noqa: WPS237
-
-
-def print_error(message):
-    if ALLOW_PRINT:
-        error_console.print(message)
-
-
-def generate_random_password() -> str:
-    """
-    Generate random password from letters and digits.
-
-    Returns:
-        str: Random string password
-    """
-    dictionary = string.ascii_letters + string.digits
-    password_length = random.randint(10, 15)  # noqa: S311,WPS432
-    return ''.join(random.choice(dictionary) for _ in range(password_length))  # noqa: S311
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+
+import random
+import string
+from pathlib import Path
+
+from rich.console import Console
+
+CONTENT_ENCRYPTION_ALGORITHM = 'aes256_cbc'
+DOWNLOADS_PATH = Path.home() / '.aos' / 'downloads'
+AOS_DISKS_PATH = DOWNLOADS_PATH
+IMAGE_WITHOUT_NODES_FILENAME = 'aos-image-vm-genericx86-64_3.0.1.wic.vmdk'
+NODE0_IMAGE_FILENAME = 'aos-vm-node0-genericx86-64.wic.vmdk'
+NODE1_IMAGE_FILENAME = 'aos-vm-node1-genericx86-64.wic.vmdk'
+
+DISK_IMAGE_DOWNLOAD_URL = 'https://d2aa62nq4kg5j3.cloudfront.net/aos-vm-v4.3.1-beta.1.tar.gz'
+REQUEST_TIMEOUT = 30
+RECONNECT_TIMEOUT = 40
+
+console = Console()
+error_console = Console(stderr=True, style='red')
+ALLOW_PRINT = True
+
+
+def print_message(formatted_text, end='\n', ljust: int = 0):
+    if ALLOW_PRINT:
+        if ljust > 0:
+            formatted_text = formatted_text.ljust(ljust)
+        console.print(formatted_text, end=end)
+
+
+def print_left(formatted_text, ljust=60):
+    print_message(formatted_text, end='', ljust=ljust)
+
+
+def print_done():
+    print_message('[green]DONE')
+
+
+def print_success(message):
+    print_message(f'[green]{str(message)}')  # noqa: WPS237
+
+
+def print_error(message):
+    if ALLOW_PRINT:
+        error_console.print(message)
+
+
+def generate_random_password() -> str:
+    """
+    Generate random password from letters and digits.
+
+    Returns:
+        str: Random string password
+    """
+    dictionary = string.ascii_letters + string.digits
+    password_length = random.randint(10, 15)  # noqa: S311,WPS432
+    return ''.join(random.choice(dictionary) for _ in range(password_length))  # noqa: S311
```

## aos_prov/utils/config.py

 * *Ordering differences only*

```diff
@@ -1,81 +1,81 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-
-from aos_prov.utils.unit_certificate import UnitCertificate
-
-
-class Config:
-    """Contains a provisioning procedure configuration."""
-
-    def __init__(self):
-        self._system_id = None
-        self._model_name = None
-        self._model_version = None
-        self._user_claim = None
-        self._supported_cert_types = None
-        self._protocol_version = None
-        self._node_ids = None
-        self._unit_certificates = []
-
-    @property
-    def system_id(self) -> str:
-        return self._system_id
-
-    @system_id.setter
-    def system_id(self, sys_id):
-        self._system_id = sys_id
-
-    @property
-    def model_name(self) -> str:
-        return self._model_name
-
-    @property
-    def model_version(self) -> str:
-        return self._model_version
-
-    @property
-    def supported_cert_types(self) -> [str]:
-        return self._supported_cert_types
-
-    @supported_cert_types.setter
-    def supported_cert_types(self, cert_types):
-        self._supported_cert_types = cert_types
-
-    @property
-    def protocol_version(self) -> int:
-        return self._protocol_version
-
-    @protocol_version.setter
-    def protocol_version(self, protocol_version):
-        self._protocol_version = protocol_version
-
-    @property
-    def node_ids(self) -> [str]:
-        return self._node_ids
-
-    @node_ids.setter
-    def node_ids(self, node_ids):
-        self._node_ids = node_ids
-
-    @property
-    def unit_certificates(self) -> [UnitCertificate]:
-        return self._unit_certificates
-
-    @unit_certificates.setter
-    def unit_certificates(self, unit_certs):
-        self._unit_certificates = unit_certs
-
-    def set_model(self, model_string):
-        """Parse model name and version received from the Unit.
-
-        Args:
-            model_string: model info returned by Unit.
-        """
-        model_chunks = model_string.strip().split(';')
-        self._model_name = model_chunks[0].strip()
-        if len(model_chunks) > 1:
-            self._model_version = model_chunks[1].strip()
-        else:
-            self._model_version = 'Unknown'
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+
+from aos_prov.utils.unit_certificate import UnitCertificate
+
+
+class Config:
+    """Contains a provisioning procedure configuration."""
+
+    def __init__(self):
+        self._system_id = None
+        self._model_name = None
+        self._model_version = None
+        self._user_claim = None
+        self._supported_cert_types = None
+        self._protocol_version = None
+        self._node_ids = None
+        self._unit_certificates = []
+
+    @property
+    def system_id(self) -> str:
+        return self._system_id
+
+    @system_id.setter
+    def system_id(self, sys_id):
+        self._system_id = sys_id
+
+    @property
+    def model_name(self) -> str:
+        return self._model_name
+
+    @property
+    def model_version(self) -> str:
+        return self._model_version
+
+    @property
+    def supported_cert_types(self) -> [str]:
+        return self._supported_cert_types
+
+    @supported_cert_types.setter
+    def supported_cert_types(self, cert_types):
+        self._supported_cert_types = cert_types
+
+    @property
+    def protocol_version(self) -> int:
+        return self._protocol_version
+
+    @protocol_version.setter
+    def protocol_version(self, protocol_version):
+        self._protocol_version = protocol_version
+
+    @property
+    def node_ids(self) -> [str]:
+        return self._node_ids
+
+    @node_ids.setter
+    def node_ids(self, node_ids):
+        self._node_ids = node_ids
+
+    @property
+    def unit_certificates(self) -> [UnitCertificate]:
+        return self._unit_certificates
+
+    @unit_certificates.setter
+    def unit_certificates(self, unit_certs):
+        self._unit_certificates = unit_certs
+
+    def set_model(self, model_string):
+        """Parse model name and version received from the Unit.
+
+        Args:
+            model_string: model info returned by Unit.
+        """
+        model_chunks = model_string.strip().split(';')
+        self._model_name = model_chunks[0].strip()
+        if len(model_chunks) > 1:
+            self._model_version = model_chunks[1].strip()
+        else:
+            self._model_version = 'Unknown'
```

## aos_prov/utils/errors.py

 * *Ordering differences only*

```diff
@@ -1,36 +1,36 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-
-
-class OnUnitError(Exception):
-    """On Unit Error."""
-
-
-class UserCredentialsError(OnUnitError):
-    """User Credentials Error."""
-
-
-class DeviceRegisterError(OnUnitError):
-    """Device Register Error."""
-
-
-class DeviceDeregisterError(OnUnitError):
-    """Device Deregister Error."""
-
-
-class UnitError(OnUnitError):
-    """Unit Error."""
-
-
-class GrpcUnimplemented(OnUnitError):  # noqa: N818
-    """Grpc Unimplemented."""
-
-
-class CloudAccessError(OnUnitError):
-    """Cloud Access Error."""
-
-
-class AosProvError(OnUnitError):
-    """Aos Prov Error."""
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+
+
+class OnUnitError(Exception):
+    """On Unit Error."""
+
+
+class UserCredentialsError(OnUnitError):
+    """User Credentials Error."""
+
+
+class DeviceRegisterError(OnUnitError):
+    """Device Register Error."""
+
+
+class DeviceDeregisterError(OnUnitError):
+    """Device Deregister Error."""
+
+
+class UnitError(OnUnitError):
+    """Unit Error."""
+
+
+class GrpcUnimplemented(OnUnitError):  # noqa: N818
+    """Grpc Unimplemented."""
+
+
+class CloudAccessError(OnUnitError):
+    """Cloud Access Error."""
+
+
+class AosProvError(OnUnitError):
+    """Aos Prov Error."""
```

## aos_prov/utils/unit_certificate.py

 * *Ordering differences only*

```diff
@@ -1,48 +1,48 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-
-"""Unit certificate object."""
-
-
-class UnitCertificate:
-    """Unit certificate object."""
-
-    def __init__(self):
-        self._cert_type = None
-        self._csr = None
-        self._node_id = None
-        self._certificate = None
-
-    @property
-    def cert_type(self) -> str:
-        return self._cert_type
-
-    @cert_type.setter
-    def cert_type(self, cert_type):
-        self._cert_type = cert_type
-
-    @property
-    def csr(self) -> str:
-        return self._csr
-
-    @csr.setter
-    def csr(self, csr_value):
-        self._csr = csr_value
-
-    @property
-    def node_id(self) -> str:
-        return self._node_id
-
-    @node_id.setter
-    def node_id(self, node_id):
-        self._node_id = node_id
-
-    @property
-    def certificate(self) -> str:
-        return self._certificate
-
-    @certificate.setter
-    def certificate(self, cert):
-        self._certificate = cert
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+
+"""Unit certificate object."""
+
+
+class UnitCertificate:
+    """Unit certificate object."""
+
+    def __init__(self):
+        self._cert_type = None
+        self._csr = None
+        self._node_id = None
+        self._certificate = None
+
+    @property
+    def cert_type(self) -> str:
+        return self._cert_type
+
+    @cert_type.setter
+    def cert_type(self, cert_type):
+        self._cert_type = cert_type
+
+    @property
+    def csr(self) -> str:
+        return self._csr
+
+    @csr.setter
+    def csr(self, csr_value):
+        self._csr = csr_value
+
+    @property
+    def node_id(self) -> str:
+        return self._node_id
+
+    @node_id.setter
+    def node_id(self, node_id):
+        self._node_id = node_id
+
+    @property
+    def certificate(self) -> str:
+        return self._certificate
+
+    @certificate.setter
+    def certificate(self, cert):
+        self._certificate = cert
```

## aos_prov/utils/user_credentials.py

```diff
@@ -1,179 +1,179 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-import os
-import tempfile
-from pathlib import Path
-from typing import Optional
-
-import pem
-from aos_prov.utils.errors import UserCredentialsError
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives._serialization import (  # noqa: WPS436
-    Encoding,
-    NoEncryption,
-    PrivateFormat,
-)
-from cryptography.hazmat.primitives.serialization.pkcs12 import (
-    load_key_and_certificates,
-    load_pkcs12,
-)
-from cryptography.x509 import load_pem_x509_certificate
-from cryptography.x509.oid import NameOID
-
-
-def _extract_cloud_domain_from_cert(cert_bytes: bytes) -> str:
-    """Get the Cloud domain name from user certificate.
-
-    Args:
-        cert_bytes: certificate content in bytes
-
-    Returns:
-        cloud domain from user certificate
-    """
-    _, certificate, _ = load_key_and_certificates(cert_bytes, None)
-    return certificate.subject.get_attributes_for_oid(NameOID.ORGANIZATION_NAME)[0].value
-
-
-def _pkcs12_to_pem(pkcs12_bytes: bytes):
-    private_key, certificate, additional_certificates = load_key_and_certificates(
-        pkcs12_bytes,
-        ''.encode('utf8'),
-        default_backend(),
-    )
-
-    cert_bytes = bytearray(certificate.public_bytes(Encoding.PEM))
-    for add_cert in additional_certificates:  # noqa: WPS519
-        cert_bytes += add_cert.public_bytes(Encoding.PEM)
-    key_bytes = private_key.private_bytes(Encoding.PEM, PrivateFormat.PKCS8, NoEncryption())
-    cert_bytes = bytes(cert_bytes)
-    return cert_bytes, key_bytes
-
-
-def _create_temp_file(data_write: bytes):
-    tmp_file = tempfile.NamedTemporaryFile(delete=False)  # pylint: disable=R1732
-    tmp_file.write(data_write)
-    tmp_file.close()
-    return tmp_file.name
-
-
-class TempCredentials:
-    def __init__(
-        self,
-        certificate: Optional[bytes],
-        key: Optional[bytes],
-        cert_file_name: Optional[str],
-        key_file_name: Optional[str],
-    ):
-        self._key_file_name = key_file_name
-        self._cert_file_name = cert_file_name
-
-        self._key = None
-        self._certificate = None
-
-        if certificate and key:
-            self._key = key
-            self._certificate = certificate
-
-    def __enter__(self):  # noqa: D105
-        if not self._key_file_name:
-            self._key_file_name = _create_temp_file(self._key)
-        if not self._cert_file_name:
-            self._cert_file_name = _create_temp_file(self._certificate)
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):  # noqa: D105
-        if self._key:
-            os.unlink(self._key_file_name)
-            self._key_file_name = None
-        if self._certificate:
-            os.unlink(self._cert_file_name)
-            self._cert_file_name = None
-
-    @property
-    def key_file_name(self):
-        return self._key_file_name
-
-    @property
-    def cert_file_name(self):
-        return self._cert_file_name
-
-
-class UserCredentials:
-
-    def __init__(self, cert_file_path: Optional[str], key_file_path: Optional[str], pkcs12: Optional[str]):
-        self._cert_file_path = cert_file_path
-        self._key_file_path = key_file_path
-        self._cloud_url = None
-        if pkcs12:
-            if Path(pkcs12).exists():
-                with open(pkcs12, 'rb') as pkcs12_file:
-                    pkcs12_file_content = pkcs12_file.read()
-                    cert_bytes, key_bytes = _pkcs12_to_pem(pkcs12_file_content)
-                    self._user_credentials = TempCredentials(
-                        certificate=cert_bytes, key=key_bytes, cert_file_name=None, key_file_name=None,
-                    )
-                    self._cloud_url = _extract_cloud_domain_from_cert(pkcs12_file_content)
-            else:
-                if not Path(cert_file_path).exists() or not Path(key_file_path).exists():
-                    raise UserCredentialsError(f'User credentials file {pkcs12} not found.')
-
-                self._user_credentials = TempCredentials(
-                    cert_file_name=cert_file_path,
-                    key_file_name=key_file_path,
-                    certificate=None,
-                    key=None,
-                )
-                self._cloud_url = self._extract_cloud_url()
-
-        else:
-            if not Path(cert_file_path).exists():
-                raise UserCredentialsError(f'User credentials file {cert_file_path} not found.')
-            if not Path(key_file_path).exists():
-                raise UserCredentialsError(f'User credentials file {key_file_path} not found.')
-
-            self._user_credentials = TempCredentials(
-                cert_file_name=cert_file_path,
-                key_file_name=key_file_path,
-                certificate=None,
-                key=None,
-            )
-            self._cloud_url = self._extract_cloud_url()
-
-    @property
-    def cloud_url(self):
-        return self._cloud_url
-
-    @property
-    def user_credentials(self):
-        return self._user_credentials
-
-    def _extract_cloud_url(self):
-        """Get the Cloud domain name from user certificate.
-
-        Returns:
-            Organization name (url) from certificate content
-        """
-        with open(self._cert_file_path, 'rb') as cert:
-            cert_data = cert.read()
-            try:
-                certificate = load_pkcs12(cert_data, password=None).cert.certificate
-            except Exception:
-                certificate = self._parse_pem(cert_data)
-
-            org_list = certificate.subject.get_attributes_for_oid(NameOID.ORGANIZATION_NAME)
-            if org_list:
-                return org_list[0].value
-            return 'aoscloud.io'
-
-    def _parse_pem(self, input_data: bytes):
-        if not input_data:
-            return None
-
-        obj_list = pem.parse(input_data)
-
-        for inst in obj_list:
-            if isinstance(inst, pem.Certificate):
-                return load_pem_x509_certificate(data=inst.as_bytes())
-        return None
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+import os
+import tempfile
+from pathlib import Path
+from typing import Optional
+
+from aos_prov.utils import pem
+from aos_prov.utils.errors import UserCredentialsError
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives._serialization import (  # noqa: WPS436
+    Encoding,
+    NoEncryption,
+    PrivateFormat,
+)
+from cryptography.hazmat.primitives.serialization.pkcs12 import (
+    load_key_and_certificates,
+    load_pkcs12,
+)
+from cryptography.x509 import load_pem_x509_certificate
+from cryptography.x509.oid import NameOID
+
+
+def _extract_cloud_domain_from_cert(cert_bytes: bytes) -> str:
+    """Get the Cloud domain name from user certificate.
+
+    Args:
+        cert_bytes: certificate content in bytes
+
+    Returns:
+        cloud domain from user certificate
+    """
+    _, certificate, _ = load_key_and_certificates(cert_bytes, None)
+    return certificate.subject.get_attributes_for_oid(NameOID.ORGANIZATION_NAME)[0].value
+
+
+def _pkcs12_to_pem(pkcs12_bytes: bytes):
+    private_key, certificate, additional_certificates = load_key_and_certificates(
+        pkcs12_bytes,
+        ''.encode('utf8'),
+        default_backend(),
+    )
+
+    cert_bytes = bytearray(certificate.public_bytes(Encoding.PEM))
+    for add_cert in additional_certificates:  # noqa: WPS519
+        cert_bytes += add_cert.public_bytes(Encoding.PEM)
+    key_bytes = private_key.private_bytes(Encoding.PEM, PrivateFormat.PKCS8, NoEncryption())
+    cert_bytes = bytes(cert_bytes)
+    return cert_bytes, key_bytes
+
+
+def _create_temp_file(data_write: bytes):
+    tmp_file = tempfile.NamedTemporaryFile(delete=False)  # pylint: disable=R1732
+    tmp_file.write(data_write)
+    tmp_file.close()
+    return tmp_file.name
+
+
+class TempCredentials:
+    def __init__(
+        self,
+        certificate: Optional[bytes],
+        key: Optional[bytes],
+        cert_file_name: Optional[str],
+        key_file_name: Optional[str],
+    ):
+        self._key_file_name = key_file_name
+        self._cert_file_name = cert_file_name
+
+        self._key = None
+        self._certificate = None
+
+        if certificate and key:
+            self._key = key
+            self._certificate = certificate
+
+    def __enter__(self):  # noqa: D105
+        if not self._key_file_name:
+            self._key_file_name = _create_temp_file(self._key)
+        if not self._cert_file_name:
+            self._cert_file_name = _create_temp_file(self._certificate)
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):  # noqa: D105
+        if self._key:
+            os.unlink(self._key_file_name)
+            self._key_file_name = None
+        if self._certificate:
+            os.unlink(self._cert_file_name)
+            self._cert_file_name = None
+
+    @property
+    def key_file_name(self):
+        return self._key_file_name
+
+    @property
+    def cert_file_name(self):
+        return self._cert_file_name
+
+
+class UserCredentials:
+
+    def __init__(self, cert_file_path: Optional[str], key_file_path: Optional[str], pkcs12: Optional[str]):
+        self._cert_file_path = cert_file_path
+        self._key_file_path = key_file_path
+        self._cloud_url = None
+        if pkcs12:
+            if Path(pkcs12).exists():
+                with open(pkcs12, 'rb') as pkcs12_file:
+                    pkcs12_file_content = pkcs12_file.read()
+                    cert_bytes, key_bytes = _pkcs12_to_pem(pkcs12_file_content)
+                    self._user_credentials = TempCredentials(
+                        certificate=cert_bytes, key=key_bytes, cert_file_name=None, key_file_name=None,
+                    )
+                    self._cloud_url = _extract_cloud_domain_from_cert(pkcs12_file_content)
+            else:
+                if not Path(cert_file_path).exists() or not Path(key_file_path).exists():
+                    raise UserCredentialsError(f'User credentials file {pkcs12} not found.')
+
+                self._user_credentials = TempCredentials(
+                    cert_file_name=cert_file_path,
+                    key_file_name=key_file_path,
+                    certificate=None,
+                    key=None,
+                )
+                self._cloud_url = self._extract_cloud_url()
+
+        else:
+            if not Path(cert_file_path).exists():
+                raise UserCredentialsError(f'User credentials file {cert_file_path} not found.')
+            if not Path(key_file_path).exists():
+                raise UserCredentialsError(f'User credentials file {key_file_path} not found.')
+
+            self._user_credentials = TempCredentials(
+                cert_file_name=cert_file_path,
+                key_file_name=key_file_path,
+                certificate=None,
+                key=None,
+            )
+            self._cloud_url = self._extract_cloud_url()
+
+    @property
+    def cloud_url(self):
+        return self._cloud_url
+
+    @property
+    def user_credentials(self):
+        return self._user_credentials
+
+    def _extract_cloud_url(self):
+        """Get the Cloud domain name from user certificate.
+
+        Returns:
+            Organization name (url) from certificate content
+        """
+        with open(self._cert_file_path, 'rb') as cert:
+            cert_data = cert.read()
+            try:
+                certificate = load_pkcs12(cert_data, password=None).cert.certificate
+            except Exception:
+                certificate = self._parse_pem(cert_data)
+
+            org_list = certificate.subject.get_attributes_for_oid(NameOID.ORGANIZATION_NAME)
+            if org_list:
+                return org_list[0].value
+            return 'aoscloud.io'
+
+    def _parse_pem(self, input_data: bytes):
+        if not input_data:
+            return None
+
+        obj_list = pem.parse(input_data)
+
+        for inst in obj_list:
+            if isinstance(inst, pem.Certificate):
+                return load_pem_x509_certificate(data=inst.as_bytes())
+        return None
```

## test/utils/test_config.py

 * *Ordering differences only*

```diff
@@ -1,23 +1,23 @@
-import unittest
-from aos_prov.utils.config import Config
-
-
-class TestConfig(unittest.TestCase):
-    def test_config_can_be_created(self):
-        c = Config()
-        self.assertIsInstance(c, Config)
-
-    def test_setters_and_getters(self):
-        c = Config()
-        c.system_id = 'some system id'
-        self.assertEqual(c.system_id, 'some system id')
-
-        c.protocol_version = 5
-        self.assertEqual(c.protocol_version, 5)
-
-        c.node_ids = ['dom0', 'dom1']
-        self.assertEqual(c.node_ids, ['dom0', 'dom1'])
-
-        c.supported_cert_types = ['um', 'sm']
-        self.assertEqual(c.supported_cert_types, ['um', 'sm'])
-
+import unittest
+from aos_prov.utils.config import Config
+
+
+class TestConfig(unittest.TestCase):
+    def test_config_can_be_created(self):
+        c = Config()
+        self.assertIsInstance(c, Config)
+
+    def test_setters_and_getters(self):
+        c = Config()
+        c.system_id = 'some system id'
+        self.assertEqual(c.system_id, 'some system id')
+
+        c.protocol_version = 5
+        self.assertEqual(c.protocol_version, 5)
+
+        c.node_ids = ['dom0', 'dom1']
+        self.assertEqual(c.node_ids, ['dom0', 'dom1'])
+
+        c.supported_cert_types = ['um', 'sm']
+        self.assertEqual(c.supported_cert_types, ['um', 'sm'])
+
```

## test/utils/test_unit_certificate.py

 * *Ordering differences only*

```diff
@@ -1,24 +1,24 @@
-import unittest
-
-from aos_prov.utils.unit_certificate import UnitCertificate
-
-
-class TestUnitCertificate(unittest.TestCase):
-    def test_object_can_be_created(self):
-        uc = UnitCertificate()
-        self.assertIsInstance(uc, UnitCertificate)
-
-    def test_attributes(self):
-        uc = UnitCertificate()
-
-        uc.cert_type = 'type1'
-        self.assertEqual(uc.cert_type, 'type1')
-
-        uc.certificate = 'some cert 1'
-        self.assertEqual(uc.certificate, 'some cert 1')
-
-        uc.node_id = 'node_id'
-        self.assertEqual(uc.node_id, 'node_id')
-
-        uc.csr = 'csr'
-        self.assertEqual(uc.csr, 'csr')
+import unittest
+
+from aos_prov.utils.unit_certificate import UnitCertificate
+
+
+class TestUnitCertificate(unittest.TestCase):
+    def test_object_can_be_created(self):
+        uc = UnitCertificate()
+        self.assertIsInstance(uc, UnitCertificate)
+
+    def test_attributes(self):
+        uc = UnitCertificate()
+
+        uc.cert_type = 'type1'
+        self.assertEqual(uc.cert_type, 'type1')
+
+        uc.certificate = 'some cert 1'
+        self.assertEqual(uc.certificate, 'some cert 1')
+
+        uc.node_id = 'node_id'
+        self.assertEqual(uc.node_id, 'node_id')
+
+        uc.csr = 'csr'
+        self.assertEqual(uc.csr, 'csr')
```

## test/utils/test_user_credentials.py

 * *Ordering differences only*

```diff
@@ -1,17 +1,17 @@
-import unittest
-
-from aos_prov.utils.user_credentials import UserCredentials
-
-
-class TestUserCredentials(unittest.TestCase):
-    def test_attributes(self):
-        uc = UserCredentials('zzz', 'zz1')
-
-        uc.cert_type = 'type1'
-        self.assertEqual(uc.cert_type, 'type1')
-
-        uc.certificate = 'some cert 1'
-        self.assertEqual(uc.certificate, 'some cert 1')
-
-        uc.csr = 'csr'
-        self.assertEqual(uc.csr, 'csr')
+import unittest
+
+from aos_prov.utils.user_credentials import UserCredentials
+
+
+class TestUserCredentials(unittest.TestCase):
+    def test_attributes(self):
+        uc = UserCredentials('zzz', 'zz1')
+
+        uc.cert_type = 'type1'
+        self.assertEqual(uc.cert_type, 'type1')
+
+        uc.certificate = 'some cert 1'
+        self.assertEqual(uc.certificate, 'some cert 1')
+
+        uc.csr = 'csr'
+        self.assertEqual(uc.csr, 'csr')
```

## tests/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
```

## tests/fixtures.py

 * *Ordering differences only*

```diff
@@ -1,130 +1,130 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-import uuid
-from datetime import datetime, timedelta
-from unittest import mock
-
-from cryptography import x509
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes
-from cryptography.hazmat.primitives.asymmetric import rsa
-from cryptography.hazmat.primitives.serialization import (
-    Encoding,
-    NoEncryption,
-    PrivateFormat,
-)
-from cryptography.hazmat.primitives.serialization.pkcs12 import (
-    serialize_key_and_certificates,
-)
-from cryptography.x509.oid import NameOID
-
-
-def generate_ca_key_and_cert():
-    private_key = rsa.generate_private_key(public_exponent=65537, key_size=2048)
-    attributes = [
-        x509.NameAttribute(NameOID.COUNTRY_NAME, u'UA'),
-        x509.NameAttribute(NameOID.LOCALITY_NAME, u'Kyiv'),
-        x509.NameAttribute(NameOID.ORGANIZATIONAL_UNIT_NAME, u'Novus Ordo Seclorum'),
-        x509.NameAttribute(NameOID.ORGANIZATION_NAME, u'Epam'),
-        x509.NameAttribute(NameOID.EMAIL_ADDRESS, u'support@aoscloud.io'),
-        x509.NameAttribute(NameOID.COMMON_NAME, u'TEST Fusion Root CA'),
-    ]
-
-    builder = x509.CertificateBuilder()
-    builder = builder.subject_name(x509.Name(attributes))
-    builder = builder.issuer_name(x509.Name(attributes))
-    builder = builder.not_valid_before(datetime.today() - timedelta(days=1))
-    builder = builder.not_valid_after(datetime.today() + timedelta(days=100))
-    builder = builder.serial_number(int(uuid.uuid4()))
-    builder = builder.public_key(private_key.public_key())
-    builder = builder.add_extension(
-        x509.BasicConstraints(ca=True, path_length=None), critical=True,
-    )
-
-    certificate = builder.sign(
-        private_key=private_key, algorithm=hashes.SHA256(),
-        backend=default_backend()
-    )
-
-    return private_key, certificate
-
-
-def generate_test_key_certificate(ca_key, domain=u"developer.test.local"):
-    private_key = rsa.generate_private_key(public_exponent=65537, key_size=2048)
-
-    subject = issuer = x509.Name([
-        x509.NameAttribute(NameOID.COUNTRY_NAME, u"US"),
-        x509.NameAttribute(NameOID.STATE_OR_PROVINCE_NAME, u"California"),
-        x509.NameAttribute(NameOID.LOCALITY_NAME, u"San Francisco"),
-        x509.NameAttribute(NameOID.ORGANIZATION_NAME, domain),
-        x509.NameAttribute(NameOID.COMMON_NAME, domain),
-    ])
-    cert = x509.CertificateBuilder().subject_name(
-        subject
-    ).issuer_name(
-        issuer
-    ).public_key(
-        private_key.public_key()
-    ).serial_number(
-        x509.random_serial_number()
-    ).not_valid_before(
-        datetime.utcnow()
-    ).not_valid_after(
-        datetime.utcnow() + timedelta(days=10)
-    ).sign(ca_key, hashes.SHA256())
-
-    return private_key, cert
-
-
-def key_cert_to_pem(private_key, cert, ca_cert):
-    private_key_pem_bytes = private_key.private_bytes(
-        encoding=Encoding.PEM,
-        format=PrivateFormat.PKCS8,
-        encryption_algorithm=NoEncryption(),
-    )
-    return private_key_pem_bytes, b''.join([cert.public_bytes(Encoding.PEM), ca_cert.public_bytes(Encoding.PEM)])
-
-
-def key_cert_to_pkcs12(private_key, cert, ca_cert):
-    return serialize_key_and_certificates(
-        name=b'TEST friendly name',
-        key=private_key,
-        cert=cert,
-        cas=[ca_cert],
-        encryption_algorithm=NoEncryption(),
-    )
-
-
-def mock_response(
-        status=200,
-        content=b'CONTENT',
-        json_data=None,
-        raise_for_status=None,
-        content_length=True,
-):
-    """
-    since we typically test a bunch of different
-    requests calls for a service, we are going to do
-    a lot of mock responses, so its usually a good idea
-    to have a helper function that builds these things
-    """
-    mock_resp = mock.Mock()
-    # mock raise_for_status call w/optional error
-    mock_resp.raise_for_status = mock.Mock()
-    if raise_for_status:
-        mock_resp.raise_for_status.side_effect = raise_for_status
-    # set status code and content
-    mock_resp.status_code = status
-    mock_resp.content = content
-    mock_resp.headers = {
-        'content-length': len(content) if content_length else None,
-    }
-    mock_resp.iter_content = mock.Mock(
-        return_value=[content]
-    )
-    # add json data if provided
-    if json_data:
-        mock_resp.json.return_value = json_data
-    return mock_resp
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+import uuid
+from datetime import datetime, timedelta
+from unittest import mock
+
+from cryptography import x509
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes
+from cryptography.hazmat.primitives.asymmetric import rsa
+from cryptography.hazmat.primitives.serialization import (
+    Encoding,
+    NoEncryption,
+    PrivateFormat,
+)
+from cryptography.hazmat.primitives.serialization.pkcs12 import (
+    serialize_key_and_certificates,
+)
+from cryptography.x509.oid import NameOID
+
+
+def generate_ca_key_and_cert():
+    private_key = rsa.generate_private_key(public_exponent=65537, key_size=2048)
+    attributes = [
+        x509.NameAttribute(NameOID.COUNTRY_NAME, u'UA'),
+        x509.NameAttribute(NameOID.LOCALITY_NAME, u'Kyiv'),
+        x509.NameAttribute(NameOID.ORGANIZATIONAL_UNIT_NAME, u'Novus Ordo Seclorum'),
+        x509.NameAttribute(NameOID.ORGANIZATION_NAME, u'Epam'),
+        x509.NameAttribute(NameOID.EMAIL_ADDRESS, u'support@aoscloud.io'),
+        x509.NameAttribute(NameOID.COMMON_NAME, u'TEST Fusion Root CA'),
+    ]
+
+    builder = x509.CertificateBuilder()
+    builder = builder.subject_name(x509.Name(attributes))
+    builder = builder.issuer_name(x509.Name(attributes))
+    builder = builder.not_valid_before(datetime.today() - timedelta(days=1))
+    builder = builder.not_valid_after(datetime.today() + timedelta(days=100))
+    builder = builder.serial_number(int(uuid.uuid4()))
+    builder = builder.public_key(private_key.public_key())
+    builder = builder.add_extension(
+        x509.BasicConstraints(ca=True, path_length=None), critical=True,
+    )
+
+    certificate = builder.sign(
+        private_key=private_key, algorithm=hashes.SHA256(),
+        backend=default_backend()
+    )
+
+    return private_key, certificate
+
+
+def generate_test_key_certificate(ca_key, domain=u"developer.test.local"):
+    private_key = rsa.generate_private_key(public_exponent=65537, key_size=2048)
+
+    subject = issuer = x509.Name([
+        x509.NameAttribute(NameOID.COUNTRY_NAME, u"US"),
+        x509.NameAttribute(NameOID.STATE_OR_PROVINCE_NAME, u"California"),
+        x509.NameAttribute(NameOID.LOCALITY_NAME, u"San Francisco"),
+        x509.NameAttribute(NameOID.ORGANIZATION_NAME, domain),
+        x509.NameAttribute(NameOID.COMMON_NAME, domain),
+    ])
+    cert = x509.CertificateBuilder().subject_name(
+        subject
+    ).issuer_name(
+        issuer
+    ).public_key(
+        private_key.public_key()
+    ).serial_number(
+        x509.random_serial_number()
+    ).not_valid_before(
+        datetime.utcnow()
+    ).not_valid_after(
+        datetime.utcnow() + timedelta(days=10)
+    ).sign(ca_key, hashes.SHA256())
+
+    return private_key, cert
+
+
+def key_cert_to_pem(private_key, cert, ca_cert):
+    private_key_pem_bytes = private_key.private_bytes(
+        encoding=Encoding.PEM,
+        format=PrivateFormat.PKCS8,
+        encryption_algorithm=NoEncryption(),
+    )
+    return private_key_pem_bytes, b''.join([cert.public_bytes(Encoding.PEM), ca_cert.public_bytes(Encoding.PEM)])
+
+
+def key_cert_to_pkcs12(private_key, cert, ca_cert):
+    return serialize_key_and_certificates(
+        name=b'TEST friendly name',
+        key=private_key,
+        cert=cert,
+        cas=[ca_cert],
+        encryption_algorithm=NoEncryption(),
+    )
+
+
+def mock_response(
+        status=200,
+        content=b'CONTENT',
+        json_data=None,
+        raise_for_status=None,
+        content_length=True,
+):
+    """
+    since we typically test a bunch of different
+    requests calls for a service, we are going to do
+    a lot of mock responses, so its usually a good idea
+    to have a helper function that builds these things
+    """
+    mock_resp = mock.Mock()
+    # mock raise_for_status call w/optional error
+    mock_resp.raise_for_status = mock.Mock()
+    if raise_for_status:
+        mock_resp.raise_for_status.side_effect = raise_for_status
+    # set status code and content
+    mock_resp.status_code = status
+    mock_resp.content = content
+    mock_resp.headers = {
+        'content-length': len(content) if content_length else None,
+    }
+    mock_resp.iter_content = mock.Mock(
+        return_value=[content]
+    )
+    # add json data if provided
+    if json_data:
+        mock_resp.json.return_value = json_data
+    return mock_resp
```

## tests/test_actions.py

 * *Ordering differences only*

```diff
@@ -1,98 +1,98 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-import io
-import tempfile
-
-from aos_prov.actions import (
-    create_new_unit,
-    download_image,
-    provision_unit,
-    remove_vm_unit,
-    start_vm_unit,
-)
-from aos_prov.communication.cloud.cloud_api import CloudAPI
-from aos_prov.utils.common import DOWNLOADS_PATH
-from aos_prov.utils.user_credentials import UserCredentials
-from rich.console import Console
-from tests.fixtures import (
-    generate_ca_key_and_cert,
-    generate_test_key_certificate,
-    key_cert_to_pem,
-    key_cert_to_pkcs12,
-)
-
-
-def test_provision_unit(mocker):
-    run_provision = mocker.patch('aos_prov.actions.run_provision')
-
-    ca_key, ca_cert = generate_ca_key_and_cert()
-    key, cert = generate_test_key_certificate(ca_key)
-    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
-
-    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
-        temp_cert.write(pkcs_12_cert)
-        temp_cert.seek(0)
-        uc = UserCredentials('cert', 'key', temp_cert.name)
-
-        cloud_api = CloudAPI(uc)
-        provision_unit('unit_address', cloud_api)
-        assert run_provision.call_count == 1
-
-
-def test_create_new_unit(mocker):
-    cloud_api = mocker.patch('aos_prov.actions.CloudAPI')
-    new_vms = mocker.patch('aos_prov.actions.new_vms', return_value=(1, 2, 3))
-    start_vms = mocker.patch('aos_prov.actions.start_vms')
-    run_provision = mocker.patch('aos_prov.actions.run_provision')
-    mocker.patch('time.sleep')
-
-    ca_key, ca_cert = generate_ca_key_and_cert()
-    key, cert = generate_test_key_certificate(ca_key)
-    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
-
-    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
-        temp_cert.write(pkcs_12_cert)
-        temp_cert.seek(0)
-        uc = UserCredentials('cert', 'key', temp_cert.name)
-
-        provisioning_port, node0_ssh_port, node1_ssh_port = create_new_unit(
-            'vm_name',
-            uc,
-            'disk_location',
-            do_provision=True,
-        )
-        assert cloud_api.call_count == 1
-        assert new_vms.call_count == 1
-        assert start_vms.call_count == 1
-        assert run_provision.call_count == 1
-        assert provisioning_port == 1
-        assert node0_ssh_port == 2
-        assert node1_ssh_port == 3
-
-
-def test_remove_vm_unit(mocker):
-    remove_vms_in_group = mocker.patch('aos_prov.actions.remove_vms_in_group')
-    remove_vm_unit('vm_unit')
-    assert remove_vms_in_group.call_count == 1
-
-
-def test_start_vm_unit(mocker):
-    start_vms = mocker.patch('aos_prov.actions.start_vms')
-    start_vm_unit('vm_unit')
-    assert start_vms.call_count == 1
-
-
-def test_download_image(mocker):
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-    download_and_save_multinode = mocker.patch('aos_prov.actions.download_and_save_multinode')
-    download_image('download_url')
-    assert download_and_save_multinode.call_count == 1
-
-    resolve_download_path = str(DOWNLOADS_PATH.resolve())
-    console_message = f'Download finished. You may find Unit images in: {resolve_download_path}\n'
-    assert console_message == console_patched.file.getvalue()
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+import io
+import tempfile
+
+from aos_prov.actions import (
+    create_new_unit,
+    download_image,
+    provision_unit,
+    remove_vm_unit,
+    start_vm_unit,
+)
+from aos_prov.communication.cloud.cloud_api import CloudAPI
+from aos_prov.utils.common import DOWNLOADS_PATH
+from aos_prov.utils.user_credentials import UserCredentials
+from rich.console import Console
+from tests.fixtures import (
+    generate_ca_key_and_cert,
+    generate_test_key_certificate,
+    key_cert_to_pem,
+    key_cert_to_pkcs12,
+)
+
+
+def test_provision_unit(mocker):
+    run_provision = mocker.patch('aos_prov.actions.run_provision')
+
+    ca_key, ca_cert = generate_ca_key_and_cert()
+    key, cert = generate_test_key_certificate(ca_key)
+    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
+
+    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
+        temp_cert.write(pkcs_12_cert)
+        temp_cert.seek(0)
+        uc = UserCredentials('cert', 'key', temp_cert.name)
+
+        cloud_api = CloudAPI(uc)
+        provision_unit('unit_address', cloud_api)
+        assert run_provision.call_count == 1
+
+
+def test_create_new_unit(mocker):
+    cloud_api = mocker.patch('aos_prov.actions.CloudAPI')
+    new_vms = mocker.patch('aos_prov.actions.new_vms', return_value=(1, 2, 3))
+    start_vms = mocker.patch('aos_prov.actions.start_vms')
+    run_provision = mocker.patch('aos_prov.actions.run_provision')
+    mocker.patch('time.sleep')
+
+    ca_key, ca_cert = generate_ca_key_and_cert()
+    key, cert = generate_test_key_certificate(ca_key)
+    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
+
+    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
+        temp_cert.write(pkcs_12_cert)
+        temp_cert.seek(0)
+        uc = UserCredentials('cert', 'key', temp_cert.name)
+
+        provisioning_port, node0_ssh_port, node1_ssh_port = create_new_unit(
+            'vm_name',
+            uc,
+            'disk_location',
+            do_provision=True,
+        )
+        assert cloud_api.call_count == 1
+        assert new_vms.call_count == 1
+        assert start_vms.call_count == 1
+        assert run_provision.call_count == 1
+        assert provisioning_port == 1
+        assert node0_ssh_port == 2
+        assert node1_ssh_port == 3
+
+
+def test_remove_vm_unit(mocker):
+    remove_vms_in_group = mocker.patch('aos_prov.actions.remove_vms_in_group')
+    remove_vm_unit('vm_unit')
+    assert remove_vms_in_group.call_count == 1
+
+
+def test_start_vm_unit(mocker):
+    start_vms = mocker.patch('aos_prov.actions.start_vms')
+    start_vm_unit('vm_unit')
+    assert start_vms.call_count == 1
+
+
+def test_download_image(mocker):
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+    download_and_save_multinode = mocker.patch('aos_prov.actions.download_and_save_multinode')
+    download_image('download_url')
+    assert download_and_save_multinode.call_count == 1
+
+    resolve_download_path = str(DOWNLOADS_PATH.resolve())
+    console_message = f'Download finished. You may find Unit images in: {resolve_download_path}\n'
+    assert console_message == console_patched.file.getvalue()
```

## tests/commands/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
```

## tests/commands/test_command_provision.py

 * *Ordering differences only*

```diff
@@ -1,413 +1,413 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-import io
-import tempfile
-
-from aos_prov.commands.command_provision import COMMAND_TO_DECRYPT, run_provision
-from aos_prov.communication.cloud.cloud_api import CloudAPI
-from aos_prov.utils.errors import GrpcUnimplemented, UnitError
-from aos_prov.utils.unit_certificate import UnitCertificate
-from aos_prov.utils.user_credentials import UserCredentials
-from pytest import raises
-from rich.console import Console
-from tests.fixtures import (
-    generate_ca_key_and_cert,
-    generate_test_key_certificate,
-    key_cert_to_pem,
-    key_cert_to_pkcs12,
-)
-
-
-def test_provision_unit_v4(mocker):
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    get_system_info = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.get_system_info', return_value=('system_id', 'model'),
-    )
-    get_protocol_version = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.get_protocol_version', return_value=4,
-    )
-    get_all_node_ids = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.get_all_node_ids', return_value=['node1', 'node2'],
-    )
-    get_cert_types = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.get_cert_types',
-        return_value=['online', 'offline', COMMAND_TO_DECRYPT],
-    )
-    clear = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV4.clear', return_value=None)
-    set_cert_owner = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.set_cert_owner', return_value=None,
-    )
-    encrypt_disk = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.encrypt_disk', return_value=None,
-    )
-    uc = UnitCertificate()
-    uc.cert_type = 'online'
-    uc.node_id = 'node1'
-    create_keys = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV4.create_keys', return_value=uc)
-    apply_certificate = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.apply_certificate', return_value=None,
-    )
-    finish_provisioning = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.finish_provisioning', return_value=None,
-    )
-
-    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.check_unit_is_not_provisioned', return_value=None)
-    mocker.patch(
-        'aos_prov.communication.cloud.cloud_api.CloudAPI.register_device',
-        return_value={
-            'system_uid': 'system_id',
-            'online_certificate': 'online_certificate_content',
-            'offline_certificate': 'offline_certificate_content',
-            'additional_certs': [
-                {
-                    'cert_type': COMMAND_TO_DECRYPT,
-                    'node_id': 'node1',
-                    'cert': 'cert_content',
-                },
-            ],
-        },
-    )
-    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.get_unit_link_by_system_uid', return_value='link')
-
-    ca_key, ca_cert = generate_ca_key_and_cert()
-    key, cert = generate_test_key_certificate(ca_key)
-    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
-
-    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
-        temp_cert.write(pkcs_12_cert)
-        temp_cert.seek(0)
-        uc = UserCredentials('cert', 'key', temp_cert.name)
-
-        cloud_api = CloudAPI(uc)
-        run_provision('unit_address', cloud_api)
-
-    assert get_system_info.call_count == 1
-    assert get_protocol_version.call_count == 1
-    assert get_all_node_ids.call_count == 1
-    assert get_cert_types.call_count == 2
-    assert set_cert_owner.call_count == 5
-    assert clear.call_count == 5
-    assert encrypt_disk.call_count == 1
-    assert create_keys.call_count == 4
-    assert apply_certificate.call_count == 4
-    assert finish_provisioning.call_count == 1
-    assert 'Starting provisioning...\n' in console_patched.file.getvalue()
-    assert 'Finished successfully!\n' in console_patched.file.getvalue()
-    assert 'You may find your unit on the cloud here: link\n' in console_patched.file.getvalue()
-
-
-def test_provision_unit_v3(mocker):
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.get_system_info', side_effect=GrpcUnimplemented(),
-    )
-
-    get_system_info = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.get_system_info', return_value=('system_id', 'model'),
-    )
-    get_protocol_version = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.get_protocol_version', return_value=3,
-    )
-    get_cert_types = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.get_cert_types',
-        return_value=['online', 'offline', COMMAND_TO_DECRYPT],
-    )
-    clear = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV2.clear', return_value=None)
-    set_cert_owner = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.set_cert_owner', return_value=None,
-    )
-    encrypt_disk = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.encrypt_disk', return_value=None,
-    )
-    wait_for_connection = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.wait_for_connection', return_value=None,
-    )
-    uc = UnitCertificate()
-    uc.cert_type = 'offline'
-    create_keys = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV2.create_keys', return_value=uc)
-    apply_certificate = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.apply_certificate', return_value=None,
-    )
-    finish_provisioning = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.finish_provisioning', return_value=None,
-    )
-
-    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.check_unit_is_not_provisioned', return_value=None)
-    mocker.patch(
-        'aos_prov.communication.cloud.cloud_api.CloudAPI.register_device',
-        return_value={
-            'system_uid': 'system_id',
-            'online_certificate': 'online_certificate_content',
-            'offline_certificate': 'offline_certificate_content',
-            'additional_certs': [
-                {
-                    'cert_type': COMMAND_TO_DECRYPT,
-                    'cert': 'cert_content',
-                },
-            ],
-        },
-    )
-    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.get_unit_link_by_system_uid', return_value='link')
-
-    ca_key, ca_cert = generate_ca_key_and_cert()
-    key, cert = generate_test_key_certificate(ca_key)
-    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
-
-    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
-        temp_cert.write(pkcs_12_cert)
-        temp_cert.seek(0)
-        uc = UserCredentials('cert', 'key', temp_cert.name)
-
-        cloud_api = CloudAPI(uc)
-        run_provision('unit_address', cloud_api)
-
-    assert get_system_info.call_count == 1
-    assert get_protocol_version.call_count == 1
-    assert get_cert_types.call_count == 1
-    assert set_cert_owner.call_count == 3
-    assert clear.call_count == 3
-    assert encrypt_disk.call_count == 1
-    assert wait_for_connection.call_count == 1
-    assert create_keys.call_count == 2
-    assert apply_certificate.call_count == 2
-    assert finish_provisioning.call_count == 1
-    assert 'Starting provisioning...\n' in console_patched.file.getvalue()
-    assert 'v4 is not supported. Starting provisioning using protocol v3\n' in console_patched.file.getvalue()
-    assert 'Finished successfully!\n' in console_patched.file.getvalue()
-    assert 'You may find your unit on the cloud here: link\n' in console_patched.file.getvalue()
-
-
-def test_provision_unit_unsupported_protocol(mocker):
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    get_system_info_v4 = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.get_system_info', side_effect=GrpcUnimplemented(),
-    )
-
-    get_system_info_v2 = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.get_system_info', side_effect=GrpcUnimplemented(),
-    )
-
-    ca_key, ca_cert = generate_ca_key_and_cert()
-    key, cert = generate_test_key_certificate(ca_key)
-    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
-
-    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
-        temp_cert.write(pkcs_12_cert)
-        temp_cert.seek(0)
-        uc = UserCredentials('cert', 'key', temp_cert.name)
-
-        cloud_api = CloudAPI(uc)
-        with raises(GrpcUnimplemented):
-            run_provision('unit_address', cloud_api)
-
-    assert get_system_info_v4.call_count == 1
-    assert get_system_info_v2.call_count == 1
-    assert 'Grpc protocol error:' in console_patched.file.getvalue()
-
-
-def test_provision_unit_connection_error(mocker):
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-    get_system_info_v4 = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.get_system_info', side_effect=UnitError(),
-    )
-    mocker.patch('time.sleep')
-
-    ca_key, ca_cert = generate_ca_key_and_cert()
-    key, cert = generate_test_key_certificate(ca_key)
-    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
-
-    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
-        temp_cert.write(pkcs_12_cert)
-        temp_cert.seek(0)
-        uc = UserCredentials('cert', 'key', temp_cert.name)
-
-        cloud_api = CloudAPI(uc)
-        with raises(UnitError):
-            run_provision('unit_address', cloud_api, reconnect_times=2)
-
-    assert get_system_info_v4.call_count == 2
-    assert 'Connection failed' in console_patched.file.getvalue()
-
-
-def test_provision_unit_v4_additional_cert(mocker):
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    get_system_info = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.get_system_info', return_value=('system_id', 'model'),
-    )
-    get_protocol_version = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.get_protocol_version', return_value=4,
-    )
-    get_all_node_ids = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.get_all_node_ids', return_value=['node1', 'node2'],
-    )
-    get_cert_types = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.get_cert_types',
-        return_value=['online', 'offline', COMMAND_TO_DECRYPT],
-    )
-    clear = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV4.clear', return_value=None)
-    set_cert_owner = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.set_cert_owner', return_value=None,
-    )
-    encrypt_disk = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.encrypt_disk', return_value=None,
-    )
-    uc = UnitCertificate()
-    uc.cert_type = 'sm'
-    uc.node_id = 'node1'
-    create_keys = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV4.create_keys', return_value=uc)
-    apply_certificate = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.apply_certificate', return_value=None,
-    )
-    finish_provisioning = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.finish_provisioning', return_value=None,
-    )
-
-    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.check_unit_is_not_provisioned', return_value=None)
-    mocker.patch(
-        'aos_prov.communication.cloud.cloud_api.CloudAPI.register_device',
-        return_value={
-            'system_uid': 'system_id',
-            'online_certificate': 'online_certificate_content',
-            'offline_certificate': 'offline_certificate_content',
-            'additional_certs': [
-                {
-                    'cert_type': 'sm',
-                    'node_id': 'node1',
-                    'cert': 'cert_content',
-                },
-            ],
-        },
-    )
-    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.get_unit_link_by_system_uid', return_value='link')
-
-    ca_key, ca_cert = generate_ca_key_and_cert()
-    key, cert = generate_test_key_certificate(ca_key)
-    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
-
-    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
-        temp_cert.write(pkcs_12_cert)
-        temp_cert.seek(0)
-        uc = UserCredentials('cert', 'key', temp_cert.name)
-
-        cloud_api = CloudAPI(uc)
-        run_provision('unit_address', cloud_api)
-
-    assert get_system_info.call_count == 1
-    assert get_protocol_version.call_count == 1
-    assert get_all_node_ids.call_count == 1
-    assert get_cert_types.call_count == 2
-    assert set_cert_owner.call_count == 5
-    assert clear.call_count == 5
-    assert encrypt_disk.call_count == 1
-    assert create_keys.call_count == 4
-    assert apply_certificate.call_count == 4
-    assert finish_provisioning.call_count == 1
-    assert 'Starting provisioning...\n' in console_patched.file.getvalue()
-    assert 'Finished successfully!\n' in console_patched.file.getvalue()
-    assert 'You may find your unit on the cloud here: link\n' in console_patched.file.getvalue()
-
-
-def test_provision_unit_v3_additional_cert(mocker):
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV4.get_system_info', side_effect=GrpcUnimplemented(),
-    )
-
-    get_system_info = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.get_system_info', return_value=('system_id', 'model'),
-    )
-    get_protocol_version = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.get_protocol_version', return_value=3,
-    )
-    get_cert_types = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.get_cert_types',
-        return_value=['online', 'offline', COMMAND_TO_DECRYPT],
-    )
-    clear = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV2.clear', return_value=None)
-    set_cert_owner = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.set_cert_owner', return_value=None,
-    )
-    encrypt_disk = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.encrypt_disk', return_value=None,
-    )
-    wait_for_connection = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.wait_for_connection', return_value=None,
-    )
-    uc = UnitCertificate()
-    uc.cert_type = 'sm'
-    create_keys = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV2.create_keys', return_value=uc)
-    apply_certificate = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.apply_certificate', return_value=None,
-    )
-    finish_provisioning = mocker.patch(
-        'aos_prov.commands.command_provision.UnitCommunicationV2.finish_provisioning', return_value=None,
-    )
-
-    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.check_unit_is_not_provisioned', return_value=None)
-    mocker.patch(
-        'aos_prov.communication.cloud.cloud_api.CloudAPI.register_device',
-        return_value={
-            'system_uid': 'system_id',
-            'online_certificate': 'online_certificate_content',
-            'offline_certificate': 'offline_certificate_content',
-            'additional_certs': [
-                {
-                    'cert_type': 'sm',
-                    'cert': 'cert_content',
-                },
-            ],
-        },
-    )
-    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.get_unit_link_by_system_uid', return_value='link')
-
-    ca_key, ca_cert = generate_ca_key_and_cert()
-    key, cert = generate_test_key_certificate(ca_key)
-    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
-
-    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
-        temp_cert.write(pkcs_12_cert)
-        temp_cert.seek(0)
-        uc = UserCredentials('cert', 'key', temp_cert.name)
-
-        cloud_api = CloudAPI(uc)
-        run_provision('unit_address', cloud_api)
-
-    assert get_system_info.call_count == 1
-    assert get_protocol_version.call_count == 1
-    assert get_cert_types.call_count == 1
-    assert set_cert_owner.call_count == 3
-    assert clear.call_count == 3
-    assert encrypt_disk.call_count == 1
-    assert wait_for_connection.call_count == 1
-    assert create_keys.call_count == 2
-    assert apply_certificate.call_count == 2
-    assert finish_provisioning.call_count == 1
-    assert 'Starting provisioning...\n' in console_patched.file.getvalue()
-    assert 'v4 is not supported. Starting provisioning using protocol v3\n' in console_patched.file.getvalue()
-    assert 'Finished successfully!\n' in console_patched.file.getvalue()
-    assert 'You may find your unit on the cloud here: link\n' in console_patched.file.getvalue()
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+import io
+import tempfile
+
+from aos_prov.commands.command_provision import COMMAND_TO_DECRYPT, run_provision
+from aos_prov.communication.cloud.cloud_api import CloudAPI
+from aos_prov.utils.errors import GrpcUnimplemented, UnitError
+from aos_prov.utils.unit_certificate import UnitCertificate
+from aos_prov.utils.user_credentials import UserCredentials
+from pytest import raises
+from rich.console import Console
+from tests.fixtures import (
+    generate_ca_key_and_cert,
+    generate_test_key_certificate,
+    key_cert_to_pem,
+    key_cert_to_pkcs12,
+)
+
+
+def test_provision_unit_v4(mocker):
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    get_system_info = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.get_system_info', return_value=('system_id', 'model'),
+    )
+    get_protocol_version = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.get_protocol_version', return_value=4,
+    )
+    get_all_node_ids = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.get_all_node_ids', return_value=['node1', 'node2'],
+    )
+    get_cert_types = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.get_cert_types',
+        return_value=['online', 'offline', COMMAND_TO_DECRYPT],
+    )
+    clear = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV4.clear', return_value=None)
+    set_cert_owner = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.set_cert_owner', return_value=None,
+    )
+    encrypt_disk = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.encrypt_disk', return_value=None,
+    )
+    uc = UnitCertificate()
+    uc.cert_type = 'online'
+    uc.node_id = 'node1'
+    create_keys = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV4.create_keys', return_value=uc)
+    apply_certificate = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.apply_certificate', return_value=None,
+    )
+    finish_provisioning = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.finish_provisioning', return_value=None,
+    )
+
+    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.check_unit_is_not_provisioned', return_value=None)
+    mocker.patch(
+        'aos_prov.communication.cloud.cloud_api.CloudAPI.register_device',
+        return_value={
+            'system_uid': 'system_id',
+            'online_certificate': 'online_certificate_content',
+            'offline_certificate': 'offline_certificate_content',
+            'additional_certs': [
+                {
+                    'cert_type': COMMAND_TO_DECRYPT,
+                    'node_id': 'node1',
+                    'cert': 'cert_content',
+                },
+            ],
+        },
+    )
+    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.get_unit_link_by_system_uid', return_value='link')
+
+    ca_key, ca_cert = generate_ca_key_and_cert()
+    key, cert = generate_test_key_certificate(ca_key)
+    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
+
+    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
+        temp_cert.write(pkcs_12_cert)
+        temp_cert.seek(0)
+        uc = UserCredentials('cert', 'key', temp_cert.name)
+
+        cloud_api = CloudAPI(uc)
+        run_provision('unit_address', cloud_api)
+
+    assert get_system_info.call_count == 1
+    assert get_protocol_version.call_count == 1
+    assert get_all_node_ids.call_count == 1
+    assert get_cert_types.call_count == 2
+    assert set_cert_owner.call_count == 5
+    assert clear.call_count == 5
+    assert encrypt_disk.call_count == 1
+    assert create_keys.call_count == 4
+    assert apply_certificate.call_count == 4
+    assert finish_provisioning.call_count == 1
+    assert 'Starting provisioning...\n' in console_patched.file.getvalue()
+    assert 'Finished successfully!\n' in console_patched.file.getvalue()
+    assert 'You may find your unit on the cloud here: link\n' in console_patched.file.getvalue()
+
+
+def test_provision_unit_v3(mocker):
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.get_system_info', side_effect=GrpcUnimplemented(),
+    )
+
+    get_system_info = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.get_system_info', return_value=('system_id', 'model'),
+    )
+    get_protocol_version = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.get_protocol_version', return_value=3,
+    )
+    get_cert_types = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.get_cert_types',
+        return_value=['online', 'offline', COMMAND_TO_DECRYPT],
+    )
+    clear = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV2.clear', return_value=None)
+    set_cert_owner = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.set_cert_owner', return_value=None,
+    )
+    encrypt_disk = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.encrypt_disk', return_value=None,
+    )
+    wait_for_connection = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.wait_for_connection', return_value=None,
+    )
+    uc = UnitCertificate()
+    uc.cert_type = 'offline'
+    create_keys = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV2.create_keys', return_value=uc)
+    apply_certificate = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.apply_certificate', return_value=None,
+    )
+    finish_provisioning = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.finish_provisioning', return_value=None,
+    )
+
+    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.check_unit_is_not_provisioned', return_value=None)
+    mocker.patch(
+        'aos_prov.communication.cloud.cloud_api.CloudAPI.register_device',
+        return_value={
+            'system_uid': 'system_id',
+            'online_certificate': 'online_certificate_content',
+            'offline_certificate': 'offline_certificate_content',
+            'additional_certs': [
+                {
+                    'cert_type': COMMAND_TO_DECRYPT,
+                    'cert': 'cert_content',
+                },
+            ],
+        },
+    )
+    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.get_unit_link_by_system_uid', return_value='link')
+
+    ca_key, ca_cert = generate_ca_key_and_cert()
+    key, cert = generate_test_key_certificate(ca_key)
+    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
+
+    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
+        temp_cert.write(pkcs_12_cert)
+        temp_cert.seek(0)
+        uc = UserCredentials('cert', 'key', temp_cert.name)
+
+        cloud_api = CloudAPI(uc)
+        run_provision('unit_address', cloud_api)
+
+    assert get_system_info.call_count == 1
+    assert get_protocol_version.call_count == 1
+    assert get_cert_types.call_count == 1
+    assert set_cert_owner.call_count == 3
+    assert clear.call_count == 3
+    assert encrypt_disk.call_count == 1
+    assert wait_for_connection.call_count == 1
+    assert create_keys.call_count == 2
+    assert apply_certificate.call_count == 2
+    assert finish_provisioning.call_count == 1
+    assert 'Starting provisioning...\n' in console_patched.file.getvalue()
+    assert 'v4 is not supported. Starting provisioning using protocol v3\n' in console_patched.file.getvalue()
+    assert 'Finished successfully!\n' in console_patched.file.getvalue()
+    assert 'You may find your unit on the cloud here: link\n' in console_patched.file.getvalue()
+
+
+def test_provision_unit_unsupported_protocol(mocker):
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    get_system_info_v4 = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.get_system_info', side_effect=GrpcUnimplemented(),
+    )
+
+    get_system_info_v2 = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.get_system_info', side_effect=GrpcUnimplemented(),
+    )
+
+    ca_key, ca_cert = generate_ca_key_and_cert()
+    key, cert = generate_test_key_certificate(ca_key)
+    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
+
+    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
+        temp_cert.write(pkcs_12_cert)
+        temp_cert.seek(0)
+        uc = UserCredentials('cert', 'key', temp_cert.name)
+
+        cloud_api = CloudAPI(uc)
+        with raises(GrpcUnimplemented):
+            run_provision('unit_address', cloud_api)
+
+    assert get_system_info_v4.call_count == 1
+    assert get_system_info_v2.call_count == 1
+    assert 'Grpc protocol error:' in console_patched.file.getvalue()
+
+
+def test_provision_unit_connection_error(mocker):
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+    get_system_info_v4 = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.get_system_info', side_effect=UnitError(),
+    )
+    mocker.patch('time.sleep')
+
+    ca_key, ca_cert = generate_ca_key_and_cert()
+    key, cert = generate_test_key_certificate(ca_key)
+    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
+
+    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
+        temp_cert.write(pkcs_12_cert)
+        temp_cert.seek(0)
+        uc = UserCredentials('cert', 'key', temp_cert.name)
+
+        cloud_api = CloudAPI(uc)
+        with raises(UnitError):
+            run_provision('unit_address', cloud_api, reconnect_times=2)
+
+    assert get_system_info_v4.call_count == 2
+    assert 'Connection failed' in console_patched.file.getvalue()
+
+
+def test_provision_unit_v4_additional_cert(mocker):
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    get_system_info = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.get_system_info', return_value=('system_id', 'model'),
+    )
+    get_protocol_version = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.get_protocol_version', return_value=4,
+    )
+    get_all_node_ids = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.get_all_node_ids', return_value=['node1', 'node2'],
+    )
+    get_cert_types = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.get_cert_types',
+        return_value=['online', 'offline', COMMAND_TO_DECRYPT],
+    )
+    clear = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV4.clear', return_value=None)
+    set_cert_owner = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.set_cert_owner', return_value=None,
+    )
+    encrypt_disk = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.encrypt_disk', return_value=None,
+    )
+    uc = UnitCertificate()
+    uc.cert_type = 'sm'
+    uc.node_id = 'node1'
+    create_keys = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV4.create_keys', return_value=uc)
+    apply_certificate = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.apply_certificate', return_value=None,
+    )
+    finish_provisioning = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.finish_provisioning', return_value=None,
+    )
+
+    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.check_unit_is_not_provisioned', return_value=None)
+    mocker.patch(
+        'aos_prov.communication.cloud.cloud_api.CloudAPI.register_device',
+        return_value={
+            'system_uid': 'system_id',
+            'online_certificate': 'online_certificate_content',
+            'offline_certificate': 'offline_certificate_content',
+            'additional_certs': [
+                {
+                    'cert_type': 'sm',
+                    'node_id': 'node1',
+                    'cert': 'cert_content',
+                },
+            ],
+        },
+    )
+    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.get_unit_link_by_system_uid', return_value='link')
+
+    ca_key, ca_cert = generate_ca_key_and_cert()
+    key, cert = generate_test_key_certificate(ca_key)
+    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
+
+    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
+        temp_cert.write(pkcs_12_cert)
+        temp_cert.seek(0)
+        uc = UserCredentials('cert', 'key', temp_cert.name)
+
+        cloud_api = CloudAPI(uc)
+        run_provision('unit_address', cloud_api)
+
+    assert get_system_info.call_count == 1
+    assert get_protocol_version.call_count == 1
+    assert get_all_node_ids.call_count == 1
+    assert get_cert_types.call_count == 2
+    assert set_cert_owner.call_count == 5
+    assert clear.call_count == 5
+    assert encrypt_disk.call_count == 1
+    assert create_keys.call_count == 4
+    assert apply_certificate.call_count == 4
+    assert finish_provisioning.call_count == 1
+    assert 'Starting provisioning...\n' in console_patched.file.getvalue()
+    assert 'Finished successfully!\n' in console_patched.file.getvalue()
+    assert 'You may find your unit on the cloud here: link\n' in console_patched.file.getvalue()
+
+
+def test_provision_unit_v3_additional_cert(mocker):
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV4.get_system_info', side_effect=GrpcUnimplemented(),
+    )
+
+    get_system_info = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.get_system_info', return_value=('system_id', 'model'),
+    )
+    get_protocol_version = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.get_protocol_version', return_value=3,
+    )
+    get_cert_types = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.get_cert_types',
+        return_value=['online', 'offline', COMMAND_TO_DECRYPT],
+    )
+    clear = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV2.clear', return_value=None)
+    set_cert_owner = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.set_cert_owner', return_value=None,
+    )
+    encrypt_disk = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.encrypt_disk', return_value=None,
+    )
+    wait_for_connection = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.wait_for_connection', return_value=None,
+    )
+    uc = UnitCertificate()
+    uc.cert_type = 'sm'
+    create_keys = mocker.patch('aos_prov.commands.command_provision.UnitCommunicationV2.create_keys', return_value=uc)
+    apply_certificate = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.apply_certificate', return_value=None,
+    )
+    finish_provisioning = mocker.patch(
+        'aos_prov.commands.command_provision.UnitCommunicationV2.finish_provisioning', return_value=None,
+    )
+
+    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.check_unit_is_not_provisioned', return_value=None)
+    mocker.patch(
+        'aos_prov.communication.cloud.cloud_api.CloudAPI.register_device',
+        return_value={
+            'system_uid': 'system_id',
+            'online_certificate': 'online_certificate_content',
+            'offline_certificate': 'offline_certificate_content',
+            'additional_certs': [
+                {
+                    'cert_type': 'sm',
+                    'cert': 'cert_content',
+                },
+            ],
+        },
+    )
+    mocker.patch('aos_prov.communication.cloud.cloud_api.CloudAPI.get_unit_link_by_system_uid', return_value='link')
+
+    ca_key, ca_cert = generate_ca_key_and_cert()
+    key, cert = generate_test_key_certificate(ca_key)
+    pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
+
+    with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
+        temp_cert.write(pkcs_12_cert)
+        temp_cert.seek(0)
+        uc = UserCredentials('cert', 'key', temp_cert.name)
+
+        cloud_api = CloudAPI(uc)
+        run_provision('unit_address', cloud_api)
+
+    assert get_system_info.call_count == 1
+    assert get_protocol_version.call_count == 1
+    assert get_cert_types.call_count == 1
+    assert set_cert_owner.call_count == 3
+    assert clear.call_count == 3
+    assert encrypt_disk.call_count == 1
+    assert wait_for_connection.call_count == 1
+    assert create_keys.call_count == 2
+    assert apply_certificate.call_count == 2
+    assert finish_provisioning.call_count == 1
+    assert 'Starting provisioning...\n' in console_patched.file.getvalue()
+    assert 'v4 is not supported. Starting provisioning using protocol v3\n' in console_patched.file.getvalue()
+    assert 'Finished successfully!\n' in console_patched.file.getvalue()
+    assert 'You may find your unit on the cloud here: link\n' in console_patched.file.getvalue()
```

## tests/commands/test_command_vm_multi_node_manage.py

 * *Ordering differences only*

```diff
@@ -1,381 +1,381 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-import io
-import os.path
-import tempfile
-import uuid
-from pathlib import Path
-from subprocess import CompletedProcess
-
-from aos_prov.commands.command_vm_multi_node_manage import (
-    _MAX_PORT,
-    _MIN_PORT,
-    check_virtual_box,
-    create_node_vm,
-    execute_command,
-    new_vms,
-    remove_vms_in_group,
-    start_vms,
-)
-from aos_prov.utils.common import (
-    IMAGE_WITHOUT_NODES_FILENAME,
-    NODE0_IMAGE_FILENAME,
-    NODE1_IMAGE_FILENAME,
-)
-from aos_prov.utils.errors import AosProvError
-from pytest import raises
-from rich.console import Console
-
-
-def test_execute_command(mocker):
-    stdout_message = 'message'
-    mocker.patch(
-        'subprocess.run',
-        return_value=CompletedProcess(None, stdout=stdout_message.encode(), returncode=0),
-    )
-
-    assert execute_command('echo') == stdout_message
-
-
-def test_execute_command_error(mocker):
-    stderr_message = 'message'
-    mocker.patch(
-        'subprocess.run',
-        return_value=CompletedProcess(None, stderr=stderr_message.encode(), returncode=1),
-    )
-
-    with raises(AosProvError) as exc:
-        execute_command('echo', catch_error=False)
-    assert stderr_message in str(exc.value)
-
-
-def test_check_virtual_box(mocker):
-    stdout_message = '7.0.12r159484'
-    mocker.patch(
-        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
-        return_value=stdout_message,
-    )
-    mocker.patch('platform.machine', return_value='amd64')
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    check_virtual_box()
-    assert 'Checking VirtualBox...' in console_patched.file.getvalue()
-    assert stdout_message in console_patched.file.getvalue()
-
-
-def test_check_virtual_box_unsupported_platform(mocker):
-    mocker.patch('platform.machine', return_value='armv7')
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    with raises(AosProvError) as exc:
-        check_virtual_box()
-    assert 'Only amd64 architecture is supported.' in str(exc.value)
-    assert 'Checking VirtualBox...' in console_patched.file.getvalue()
-
-
-def test_check_virtual_box_not_installed(mocker):
-    mocker.patch(
-        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
-        side_effect=AosProvError(),
-    )
-    mocker.patch('platform.machine', return_value='amd64')
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    with raises(AosProvError) as exc:
-        check_virtual_box()
-    assert 'VirtualBox is not installed or it is not in the PATH' in str(exc.value)
-    assert 'Checking VirtualBox...' in console_patched.file.getvalue()
-
-
-def test_check_virtual_box_not_loaded_kernel_monules(mocker):
-    stdout_message = 'WARNING: The vboxdrv kernel module is not loaded'
-    mocker.patch(
-        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
-        return_value=stdout_message,
-    )
-    mocker.patch('platform.machine', return_value='amd64')
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    with raises(AosProvError) as exc:
-        check_virtual_box()
-    assert 'VirtualBox kernel modules is not installed.' in str(exc.value)
-    assert 'Checking VirtualBox...' in console_patched.file.getvalue()
-
-
-def test_check_virtual_box_not_7(mocker):
-    stdout_message = '6.0.12r159484'
-    mocker.patch(
-        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
-        return_value=stdout_message,
-    )
-    mocker.patch('platform.machine', return_value='amd64')
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    with raises(AosProvError) as exc:
-        check_virtual_box()
-    assert 'VirtualBox 7 is only supported' in str(exc.value)
-    assert 'Checking VirtualBox...' in console_patched.file.getvalue()
-
-
-def test_create_node_vm_multinode(mocker):
-    stdout_message = '7.0.12r159484'
-    mocker.patch(
-        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
-        return_value=stdout_message,
-    )
-    m_copyfile = mocker.patch('aos_prov.commands.command_vm_multi_node_manage.copyfile')
-
-    with tempfile.TemporaryDirectory() as tmp_directory:
-        create_node_vm(
-            'vm_name',
-            uuid.uuid4(),
-            'group',
-            Path(tmp_directory),
-            'node1',
-            'network1',
-            is_image_without_nodes=False,
-        )
-    assert m_copyfile.call_count == 1
-
-
-def test_create_node_vm_onenode(mocker):
-    stdout_message = '7.0.12r159484'
-    mocker.patch(
-        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
-        return_value=stdout_message,
-    )
-    m_copyfile = mocker.patch('aos_prov.commands.command_vm_multi_node_manage.copyfile')
-
-    with tempfile.TemporaryDirectory() as tmp_directory:
-        create_node_vm(
-            'vm_name',
-            uuid.uuid4(),
-            'group',
-            Path(tmp_directory),
-            'node1',
-            'network1',
-            is_image_without_nodes=True,
-        )
-    assert m_copyfile.call_count == 1
-
-
-def test_remove_vms_in_group(mocker):
-    stdout_message = """
-Name:                        node0
-Encryption:     disabled
-Groups:                      /AosUnits/R4
-Guest OS:                    Other Linux (64-bit)
-UUID:                        6f400be7-5178-4f79-898c-90a86350eec1
-
-Name:                        node1
-Encryption:     disabled
-Groups:                      /AosUnits/R4
-Guest OS:                    Other Linux (64-bit)
-UUID:                        156f8a8c-7f5d-4332-a793-f9fe961e966e
-    """
-    mocker.patch(
-        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
-        return_value=stdout_message,
-    )
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-    remove_vms_in_group('R4')
-    assert 'Removing VMs in Groups: /AosUnits/R4 for the units...' in console_patched.file.getvalue()
-    assert 'VMs have been deleted' in console_patched.file.getvalue()
-
-
-def test_remove_vms_in_group_not_found(mocker):
-    stdout_message = """
-Name:                        node0
-Encryption:     disabled
-Groups:                      /AosUnits/R4
-Guest OS:                    Other Linux (64-bit)
-UUID:                        6f400be7-5178-4f79-898c-90a86350eec1
-
-Name:                        node1
-Encryption:     disabled
-Groups:                      /AosUnits/R4
-Guest OS:                    Other Linux (64-bit)
-UUID:                        156f8a8c-7f5d-4332-a793-f9fe961e966e
-    """
-    mocker.patch(
-        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
-        return_value=stdout_message,
-    )
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-    error_console_patched = mocker.patch(
-        'aos_prov.utils.common.error_console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True, stderr=True),
-    )
-    remove_vms_in_group('R3')
-    assert 'Removing VMs in Groups: /AosUnits/R3 for the units...' in console_patched.file.getvalue()
-    assert 'VM Group: /AosUnits/R3 is not presented on system.' in error_console_patched.file.getvalue()
-
-
-def test_start_vms(mocker):
-    mocker.patch('platform.machine', return_value='amd64')
-    vm_list = """
-"node0" {a87f7c95-adf2-4a6c-ae64-706df2b31f5e}
-"node0" {8cfe08c1-32bb-4d7e-8a5c-8e30b687bb30}
-"node0" {6f400be7-5178-4f79-898c-90a86350eec1}
-"node1" {156f8a8c-7f5d-4332-a793-f9fe961e966e}
-"node0" {ccc6ed3a-ddf2-4457-8cdf-0851f27d0e18}
-    """
-    mocker.patch(
-        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
-        return_value=vm_list,
-    )
-    vm_info = """
-name="node0"
-Encryption:     disabled
-groups="/AosUnits/R4"
-ostype="Other Linux (64-bit)"
-UUID="a87f7c95-adf2-4a6c-ae64-706df2b31f5e"
-    """
-    mocker.patch(
-        'aos_prov.commands.command_vm_multi_node_manage.request_vm_info',
-        return_value=vm_info,
-    )
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-    start_vms('/AosUnits/R4', False)
-    assert 'Starting VMs in group /AosUnits/R4' in console_patched.file.getvalue()
-    assert 'Starting VM a87f7c95-adf2-4a6c-ae64-706df2b31f5e...' in console_patched.file.getvalue()
-    assert 'DONE' in console_patched.file.getvalue()
-
-
-def test_start_vms_error(mocker):
-    mocker.patch('platform.machine', return_value='amd64')
-    vm_list = """
-"node0" {a87f7c95-adf2-4a6c-ae64-706df2b31f5e}
-"node0" {8cfe08c1-32bb-4d7e-8a5c-8e30b687bb30}
-"node0" {6f400be7-5178-4f79-898c-90a86350eec1}
-"node1" {156f8a8c-7f5d-4332-a793-f9fe961e966e}
-"node0" {ccc6ed3a-ddf2-4457-8cdf-0851f27d0e18}
-    """
-    mocker.patch(
-        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
-        return_value=vm_list,
-    )
-    vm_info = """
-name="node0"
-Encryption:     disabled
-groups="/AosUnits/R4"
-ostype="Other Linux (64-bit)"
-UUID="a87f7c95-adf2-4a6c-ae64-706df2b31f5e"
-    """
-    mocker.patch(
-        'aos_prov.commands.command_vm_multi_node_manage.request_vm_info',
-        return_value=vm_info,
-    )
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-    with raises(AosProvError) as exc:
-        start_vms('/AosUnits/R3', False)
-    assert 'Starting VMs in group /AosUnits/R3' in console_patched.file.getvalue()
-    assert 'No VMs found in group /AosUnits/R3 to start!' in str(exc.value)
-
-
-def test_new_vms_multinode(mocker):
-    stdout_message = '100'
-    mocker.patch(
-        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
-        return_value=stdout_message,
-    )
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-    mocker.patch('aos_prov.commands.command_vm_multi_node_manage.copyfile')
-
-    with tempfile.TemporaryDirectory() as tmp_directory:
-        node0_tmp_file = open(os.path.join(tmp_directory, NODE0_IMAGE_FILENAME), 'w')
-        node0_tmp_file.write('data')
-        node0_tmp_file.close()
-        node1_tmp_file = open(os.path.join(tmp_directory, NODE1_IMAGE_FILENAME), 'w')
-        node1_tmp_file.write('data')
-        node1_tmp_file.close()
-        provisioning_port, node0_ssh_port, node1_ssh_port = new_vms('vm_name', tmp_directory, 2, False)
-        assert provisioning_port in range(_MIN_PORT - 1, _MAX_PORT + 1)
-        assert node0_ssh_port in range(_MIN_PORT - 1, _MAX_PORT + 1)
-        assert node1_ssh_port in range(_MIN_PORT - 1, _MAX_PORT + 1)
-        assert 'Creating a new virtual machines...' in console_patched.file.getvalue()
-        assert 'Forwarding provisioning port...' in console_patched.file.getvalue()
-        assert 'Forwarding ssh port to node0...' in console_patched.file.getvalue()
-        assert 'Forwarding ssh port to node1...' in console_patched.file.getvalue()
-        assert 'Creating a new VM for node0...' in console_patched.file.getvalue()
-        assert 'DONE' in console_patched.file.getvalue()
-        assert 'Creating a new VM for node1...' in console_patched.file.getvalue()
-        assert 'DONE' in console_patched.file.getvalue()
-
-
-def test_new_vms_onenode(mocker):
-    stdout_message = '100'
-    mocker.patch(
-        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
-        return_value=stdout_message,
-    )
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-    mocker.patch('aos_prov.commands.command_vm_multi_node_manage.copyfile')
-
-    with tempfile.TemporaryDirectory() as tmp_directory:
-        node0_tmp_file = open(os.path.join(tmp_directory, IMAGE_WITHOUT_NODES_FILENAME), 'w')
-        node0_tmp_file.write('data')
-        node0_tmp_file.close()
-
-        provisioning_port, node0_ssh_port, node1_ssh_port = new_vms('vm_name', tmp_directory, 1, False)
-        assert provisioning_port in range(_MIN_PORT - 1, _MAX_PORT + 1)
-        assert node0_ssh_port in range(_MIN_PORT - 1, _MAX_PORT + 1)
-        assert node1_ssh_port == None
-        assert 'Creating a new virtual machines...' in console_patched.file.getvalue()
-        assert 'Forwarding provisioning port...' in console_patched.file.getvalue()
-        assert 'Forwarding ssh port to node0...' in console_patched.file.getvalue()
-        assert 'Creating a new VM for node0...' in console_patched.file.getvalue()
-        assert 'DONE' in console_patched.file.getvalue()
-
-
-def test_new_vms_disks_not_found(mocker):
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    with tempfile.TemporaryDirectory() as tmp_directory:
-        with raises(AosProvError) as exc:
-            new_vms(
-                'vm_name',
-                tmp_directory,
-                2,
-                False,
-            )
-        assert 'Creating a new virtual machines...' in console_patched.file.getvalue()
-        assert f'Disk images not found in directory {tmp_directory}. Cannot proceed!' in str(exc.value)
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+import io
+import os.path
+import tempfile
+import uuid
+from pathlib import Path
+from subprocess import CompletedProcess
+
+from aos_prov.commands.command_vm_multi_node_manage import (
+    _MAX_PORT,
+    _MIN_PORT,
+    check_virtual_box,
+    create_node_vm,
+    execute_command,
+    new_vms,
+    remove_vms_in_group,
+    start_vms,
+)
+from aos_prov.utils.common import (
+    IMAGE_WITHOUT_NODES_FILENAME,
+    NODE0_IMAGE_FILENAME,
+    NODE1_IMAGE_FILENAME,
+)
+from aos_prov.utils.errors import AosProvError
+from pytest import raises
+from rich.console import Console
+
+
+def test_execute_command(mocker):
+    stdout_message = 'message'
+    mocker.patch(
+        'subprocess.run',
+        return_value=CompletedProcess(None, stdout=stdout_message.encode(), returncode=0),
+    )
+
+    assert execute_command('echo') == stdout_message
+
+
+def test_execute_command_error(mocker):
+    stderr_message = 'message'
+    mocker.patch(
+        'subprocess.run',
+        return_value=CompletedProcess(None, stderr=stderr_message.encode(), returncode=1),
+    )
+
+    with raises(AosProvError) as exc:
+        execute_command('echo', catch_error=False)
+    assert stderr_message in str(exc.value)
+
+
+def test_check_virtual_box(mocker):
+    stdout_message = '7.0.12r159484'
+    mocker.patch(
+        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
+        return_value=stdout_message,
+    )
+    mocker.patch('platform.machine', return_value='amd64')
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    check_virtual_box()
+    assert 'Checking VirtualBox...' in console_patched.file.getvalue()
+    assert stdout_message in console_patched.file.getvalue()
+
+
+def test_check_virtual_box_unsupported_platform(mocker):
+    mocker.patch('platform.machine', return_value='armv7')
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    with raises(AosProvError) as exc:
+        check_virtual_box()
+    assert 'Only amd64 architecture is supported.' in str(exc.value)
+    assert 'Checking VirtualBox...' in console_patched.file.getvalue()
+
+
+def test_check_virtual_box_not_installed(mocker):
+    mocker.patch(
+        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
+        side_effect=AosProvError(),
+    )
+    mocker.patch('platform.machine', return_value='amd64')
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    with raises(AosProvError) as exc:
+        check_virtual_box()
+    assert 'VirtualBox is not installed or it is not in the PATH' in str(exc.value)
+    assert 'Checking VirtualBox...' in console_patched.file.getvalue()
+
+
+def test_check_virtual_box_not_loaded_kernel_monules(mocker):
+    stdout_message = 'WARNING: The vboxdrv kernel module is not loaded'
+    mocker.patch(
+        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
+        return_value=stdout_message,
+    )
+    mocker.patch('platform.machine', return_value='amd64')
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    with raises(AosProvError) as exc:
+        check_virtual_box()
+    assert 'VirtualBox kernel modules is not installed.' in str(exc.value)
+    assert 'Checking VirtualBox...' in console_patched.file.getvalue()
+
+
+def test_check_virtual_box_not_7(mocker):
+    stdout_message = '6.0.12r159484'
+    mocker.patch(
+        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
+        return_value=stdout_message,
+    )
+    mocker.patch('platform.machine', return_value='amd64')
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    with raises(AosProvError) as exc:
+        check_virtual_box()
+    assert 'VirtualBox 7 is only supported' in str(exc.value)
+    assert 'Checking VirtualBox...' in console_patched.file.getvalue()
+
+
+def test_create_node_vm_multinode(mocker):
+    stdout_message = '7.0.12r159484'
+    mocker.patch(
+        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
+        return_value=stdout_message,
+    )
+    m_copyfile = mocker.patch('aos_prov.commands.command_vm_multi_node_manage.copyfile')
+
+    with tempfile.TemporaryDirectory() as tmp_directory:
+        create_node_vm(
+            'vm_name',
+            uuid.uuid4(),
+            'group',
+            Path(tmp_directory),
+            'node1',
+            'network1',
+            is_image_without_nodes=False,
+        )
+    assert m_copyfile.call_count == 1
+
+
+def test_create_node_vm_onenode(mocker):
+    stdout_message = '7.0.12r159484'
+    mocker.patch(
+        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
+        return_value=stdout_message,
+    )
+    m_copyfile = mocker.patch('aos_prov.commands.command_vm_multi_node_manage.copyfile')
+
+    with tempfile.TemporaryDirectory() as tmp_directory:
+        create_node_vm(
+            'vm_name',
+            uuid.uuid4(),
+            'group',
+            Path(tmp_directory),
+            'node1',
+            'network1',
+            is_image_without_nodes=True,
+        )
+    assert m_copyfile.call_count == 1
+
+
+def test_remove_vms_in_group(mocker):
+    stdout_message = """
+Name:                        node0
+Encryption:     disabled
+Groups:                      /AosUnits/R4
+Guest OS:                    Other Linux (64-bit)
+UUID:                        6f400be7-5178-4f79-898c-90a86350eec1
+
+Name:                        node1
+Encryption:     disabled
+Groups:                      /AosUnits/R4
+Guest OS:                    Other Linux (64-bit)
+UUID:                        156f8a8c-7f5d-4332-a793-f9fe961e966e
+    """
+    mocker.patch(
+        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
+        return_value=stdout_message,
+    )
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+    remove_vms_in_group('R4')
+    assert 'Removing VMs in Groups: /AosUnits/R4 for the units...' in console_patched.file.getvalue()
+    assert 'VMs have been deleted' in console_patched.file.getvalue()
+
+
+def test_remove_vms_in_group_not_found(mocker):
+    stdout_message = """
+Name:                        node0
+Encryption:     disabled
+Groups:                      /AosUnits/R4
+Guest OS:                    Other Linux (64-bit)
+UUID:                        6f400be7-5178-4f79-898c-90a86350eec1
+
+Name:                        node1
+Encryption:     disabled
+Groups:                      /AosUnits/R4
+Guest OS:                    Other Linux (64-bit)
+UUID:                        156f8a8c-7f5d-4332-a793-f9fe961e966e
+    """
+    mocker.patch(
+        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
+        return_value=stdout_message,
+    )
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+    error_console_patched = mocker.patch(
+        'aos_prov.utils.common.error_console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True, stderr=True),
+    )
+    remove_vms_in_group('R3')
+    assert 'Removing VMs in Groups: /AosUnits/R3 for the units...' in console_patched.file.getvalue()
+    assert 'VM Group: /AosUnits/R3 is not presented on system.' in error_console_patched.file.getvalue()
+
+
+def test_start_vms(mocker):
+    mocker.patch('platform.machine', return_value='amd64')
+    vm_list = """
+"node0" {a87f7c95-adf2-4a6c-ae64-706df2b31f5e}
+"node0" {8cfe08c1-32bb-4d7e-8a5c-8e30b687bb30}
+"node0" {6f400be7-5178-4f79-898c-90a86350eec1}
+"node1" {156f8a8c-7f5d-4332-a793-f9fe961e966e}
+"node0" {ccc6ed3a-ddf2-4457-8cdf-0851f27d0e18}
+    """
+    mocker.patch(
+        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
+        return_value=vm_list,
+    )
+    vm_info = """
+name="node0"
+Encryption:     disabled
+groups="/AosUnits/R4"
+ostype="Other Linux (64-bit)"
+UUID="a87f7c95-adf2-4a6c-ae64-706df2b31f5e"
+    """
+    mocker.patch(
+        'aos_prov.commands.command_vm_multi_node_manage.request_vm_info',
+        return_value=vm_info,
+    )
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+    start_vms('/AosUnits/R4', False)
+    assert 'Starting VMs in group /AosUnits/R4' in console_patched.file.getvalue()
+    assert 'Starting VM a87f7c95-adf2-4a6c-ae64-706df2b31f5e...' in console_patched.file.getvalue()
+    assert 'DONE' in console_patched.file.getvalue()
+
+
+def test_start_vms_error(mocker):
+    mocker.patch('platform.machine', return_value='amd64')
+    vm_list = """
+"node0" {a87f7c95-adf2-4a6c-ae64-706df2b31f5e}
+"node0" {8cfe08c1-32bb-4d7e-8a5c-8e30b687bb30}
+"node0" {6f400be7-5178-4f79-898c-90a86350eec1}
+"node1" {156f8a8c-7f5d-4332-a793-f9fe961e966e}
+"node0" {ccc6ed3a-ddf2-4457-8cdf-0851f27d0e18}
+    """
+    mocker.patch(
+        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
+        return_value=vm_list,
+    )
+    vm_info = """
+name="node0"
+Encryption:     disabled
+groups="/AosUnits/R4"
+ostype="Other Linux (64-bit)"
+UUID="a87f7c95-adf2-4a6c-ae64-706df2b31f5e"
+    """
+    mocker.patch(
+        'aos_prov.commands.command_vm_multi_node_manage.request_vm_info',
+        return_value=vm_info,
+    )
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+    with raises(AosProvError) as exc:
+        start_vms('/AosUnits/R3', False)
+    assert 'Starting VMs in group /AosUnits/R3' in console_patched.file.getvalue()
+    assert 'No VMs found in group /AosUnits/R3 to start!' in str(exc.value)
+
+
+def test_new_vms_multinode(mocker):
+    stdout_message = '100'
+    mocker.patch(
+        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
+        return_value=stdout_message,
+    )
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+    mocker.patch('aos_prov.commands.command_vm_multi_node_manage.copyfile')
+
+    with tempfile.TemporaryDirectory() as tmp_directory:
+        node0_tmp_file = open(os.path.join(tmp_directory, NODE0_IMAGE_FILENAME), 'w')
+        node0_tmp_file.write('data')
+        node0_tmp_file.close()
+        node1_tmp_file = open(os.path.join(tmp_directory, NODE1_IMAGE_FILENAME), 'w')
+        node1_tmp_file.write('data')
+        node1_tmp_file.close()
+        provisioning_port, node0_ssh_port, node1_ssh_port = new_vms('vm_name', tmp_directory, 2, False)
+        assert provisioning_port in range(_MIN_PORT - 1, _MAX_PORT + 1)
+        assert node0_ssh_port in range(_MIN_PORT - 1, _MAX_PORT + 1)
+        assert node1_ssh_port in range(_MIN_PORT - 1, _MAX_PORT + 1)
+        assert 'Creating a new virtual machines...' in console_patched.file.getvalue()
+        assert 'Forwarding provisioning port...' in console_patched.file.getvalue()
+        assert 'Forwarding ssh port to node0...' in console_patched.file.getvalue()
+        assert 'Forwarding ssh port to node1...' in console_patched.file.getvalue()
+        assert 'Creating a new VM for node0...' in console_patched.file.getvalue()
+        assert 'DONE' in console_patched.file.getvalue()
+        assert 'Creating a new VM for node1...' in console_patched.file.getvalue()
+        assert 'DONE' in console_patched.file.getvalue()
+
+
+def test_new_vms_onenode(mocker):
+    stdout_message = '100'
+    mocker.patch(
+        'aos_prov.commands.command_vm_multi_node_manage.execute_command',
+        return_value=stdout_message,
+    )
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+    mocker.patch('aos_prov.commands.command_vm_multi_node_manage.copyfile')
+
+    with tempfile.TemporaryDirectory() as tmp_directory:
+        node0_tmp_file = open(os.path.join(tmp_directory, IMAGE_WITHOUT_NODES_FILENAME), 'w')
+        node0_tmp_file.write('data')
+        node0_tmp_file.close()
+
+        provisioning_port, node0_ssh_port, node1_ssh_port = new_vms('vm_name', tmp_directory, 1, False)
+        assert provisioning_port in range(_MIN_PORT - 1, _MAX_PORT + 1)
+        assert node0_ssh_port in range(_MIN_PORT - 1, _MAX_PORT + 1)
+        assert node1_ssh_port == None
+        assert 'Creating a new virtual machines...' in console_patched.file.getvalue()
+        assert 'Forwarding provisioning port...' in console_patched.file.getvalue()
+        assert 'Forwarding ssh port to node0...' in console_patched.file.getvalue()
+        assert 'Creating a new VM for node0...' in console_patched.file.getvalue()
+        assert 'DONE' in console_patched.file.getvalue()
+
+
+def test_new_vms_disks_not_found(mocker):
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    with tempfile.TemporaryDirectory() as tmp_directory:
+        with raises(AosProvError) as exc:
+            new_vms(
+                'vm_name',
+                tmp_directory,
+                2,
+                False,
+            )
+        assert 'Creating a new virtual machines...' in console_patched.file.getvalue()
+        assert f'Disk images not found in directory {tmp_directory}. Cannot proceed!' in str(exc.value)
```

## tests/commands/test_download.py

 * *Ordering differences only*

```diff
@@ -1,82 +1,82 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-import os
-import tarfile
-import tempfile
-import unittest
-from pathlib import Path
-from unittest import mock
-
-from aos_prov.commands.download import download_and_save_multinode
-from aos_prov.utils.common import NODE0_IMAGE_FILENAME
-from aos_prov.utils.errors import AosProvError
-from requests import HTTPError
-from tests.fixtures import mock_response
-
-
-class TestDownload(unittest.TestCase):
-    @mock.patch('pathlib.Path.home')
-    @mock.patch('requests.get')
-    def test_download_and_save_multinode(self, mock_get, mock_home):
-        image_test_path = tempfile.NamedTemporaryFile(delete=False)
-        image_test_path.write(b'some_data')
-        image_test_path.close()
-        tar_test_path = tempfile.NamedTemporaryFile(delete=False)
-        # opening the file in write mode
-        tar_test = tarfile.open(tar_test_path.name, 'w')
-        tar_test.add(image_test_path.name)
-        tar_test.close()
-        mock_resp = mock_response(content=tar_test_path.read())
-        tar_test_path.close()
-        mock_get.return_value = mock_resp
-        with tempfile.TemporaryDirectory() as tmp_directory:
-            mock_home.return_value = Path(tmp_directory)
-            download_and_save_multinode('developer.cloud.io', Path(tmp_directory), True)
-
-            self.assertIn('tmp', os.listdir(f'{tmp_directory}/'))
-            self.assertIn(os.path.basename(image_test_path.name), os.listdir(f'{tmp_directory}/tmp/'))
-
-    @mock.patch('pathlib.Path.home')
-    @mock.patch('requests.get')
-    def test_download_and_save_multinode_without_extract(self, mock_get, mock_home):
-        image_test_path = tempfile.NamedTemporaryFile(delete=False)
-        image_test_path.write(b'some_data')
-        image_test_path.close()
-        tar_test_path = tempfile.NamedTemporaryFile(delete=False)
-        # opening the file in write mode
-        tar_test = tarfile.open(tar_test_path.name, 'w')
-        tar_test.add(image_test_path.name)
-        tar_test.close()
-        mock_resp = mock_response(content=tar_test_path.read(), content_length=False)
-        tar_test_path.close()
-        mock_get.return_value = mock_resp
-        with tempfile.TemporaryDirectory() as tmp_directory:
-            mock_home.return_value = Path(tmp_directory)
-            download_and_save_multinode('developer.cloud.io', Path(tmp_directory), True)
-
-            self.assertIn('downloaded-multi-node-images.tar.gz', os.listdir(f'{tmp_directory}/'))
-
-    @mock.patch('pathlib.Path.home')
-    @mock.patch('requests.get')
-    def test_download_and_save_multinode_failed_response(self, mock_get, mock_home):
-        mock_resp = mock_response(status=500, raise_for_status=HTTPError('cloud is down'))
-        mock_get.return_value = mock_resp
-        with tempfile.TemporaryDirectory() as tmp_directory:
-            mock_home.return_value = Path(tmp_directory)
-            self.assertRaises(HTTPError, download_and_save_multinode, 'developer.cloud.io', Path(tmp_directory), True)
-
-    @mock.patch('pathlib.Path.home')
-    def test_download_and_save_multinode_failed_file_exists(self, mock_home):
-        with tempfile.TemporaryDirectory() as tmp_directory:
-            mock_home.return_value = Path(tmp_directory)
-
-            file_node = open(os.path.join(tmp_directory, NODE0_IMAGE_FILENAME), 'w')
-            file_node.write('data')
-            file_node.close()
-            self.assertRaises(
-                AosProvError,
-                download_and_save_multinode, 'developer.cloud.io', Path(tmp_directory), False,
-            )
-
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+import os
+import tarfile
+import tempfile
+import unittest
+from pathlib import Path
+from unittest import mock
+
+from aos_prov.commands.download import download_and_save_multinode
+from aos_prov.utils.common import NODE0_IMAGE_FILENAME
+from aos_prov.utils.errors import AosProvError
+from requests import HTTPError
+from tests.fixtures import mock_response
+
+
+class TestDownload(unittest.TestCase):
+    @mock.patch('pathlib.Path.home')
+    @mock.patch('requests.get')
+    def test_download_and_save_multinode(self, mock_get, mock_home):
+        image_test_path = tempfile.NamedTemporaryFile(delete=False)
+        image_test_path.write(b'some_data')
+        image_test_path.close()
+        tar_test_path = tempfile.NamedTemporaryFile(delete=False)
+        # opening the file in write mode
+        tar_test = tarfile.open(tar_test_path.name, 'w')
+        tar_test.add(image_test_path.name)
+        tar_test.close()
+        mock_resp = mock_response(content=tar_test_path.read())
+        tar_test_path.close()
+        mock_get.return_value = mock_resp
+        with tempfile.TemporaryDirectory() as tmp_directory:
+            mock_home.return_value = Path(tmp_directory)
+            download_and_save_multinode('developer.cloud.io', Path(tmp_directory), True)
+
+            self.assertIn('tmp', os.listdir(f'{tmp_directory}/'))
+            self.assertIn(os.path.basename(image_test_path.name), os.listdir(f'{tmp_directory}/tmp/'))
+
+    @mock.patch('pathlib.Path.home')
+    @mock.patch('requests.get')
+    def test_download_and_save_multinode_without_extract(self, mock_get, mock_home):
+        image_test_path = tempfile.NamedTemporaryFile(delete=False)
+        image_test_path.write(b'some_data')
+        image_test_path.close()
+        tar_test_path = tempfile.NamedTemporaryFile(delete=False)
+        # opening the file in write mode
+        tar_test = tarfile.open(tar_test_path.name, 'w')
+        tar_test.add(image_test_path.name)
+        tar_test.close()
+        mock_resp = mock_response(content=tar_test_path.read(), content_length=False)
+        tar_test_path.close()
+        mock_get.return_value = mock_resp
+        with tempfile.TemporaryDirectory() as tmp_directory:
+            mock_home.return_value = Path(tmp_directory)
+            download_and_save_multinode('developer.cloud.io', Path(tmp_directory), True)
+
+            self.assertIn('downloaded-multi-node-images.tar.gz', os.listdir(f'{tmp_directory}/'))
+
+    @mock.patch('pathlib.Path.home')
+    @mock.patch('requests.get')
+    def test_download_and_save_multinode_failed_response(self, mock_get, mock_home):
+        mock_resp = mock_response(status=500, raise_for_status=HTTPError('cloud is down'))
+        mock_get.return_value = mock_resp
+        with tempfile.TemporaryDirectory() as tmp_directory:
+            mock_home.return_value = Path(tmp_directory)
+            self.assertRaises(HTTPError, download_and_save_multinode, 'developer.cloud.io', Path(tmp_directory), True)
+
+    @mock.patch('pathlib.Path.home')
+    def test_download_and_save_multinode_failed_file_exists(self, mock_home):
+        with tempfile.TemporaryDirectory() as tmp_directory:
+            mock_home.return_value = Path(tmp_directory)
+
+            file_node = open(os.path.join(tmp_directory, NODE0_IMAGE_FILENAME), 'w')
+            file_node.write('data')
+            file_node.close()
+            self.assertRaises(
+                AosProvError,
+                download_and_save_multinode, 'developer.cloud.io', Path(tmp_directory), False,
+            )
+
```

## tests/utils/test_common.py

 * *Ordering differences only*

```diff
@@ -1,69 +1,69 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-import io
-
-from aos_prov.utils.common import (
-    generate_random_password,
-    print_done,
-    print_error,
-    print_left,
-    print_message,
-    print_success,
-)
-from rich.console import Console
-
-
-def test_print_message(mocker):
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    print_message('test_message', ljust=1)
-    assert 'test_message\n' == console_patched.file.getvalue()
-
-
-def test_print_left(mocker):
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    print_left('test_message')
-    assert 'test_message' in console_patched.file.getvalue()
-
-
-def test_print_done(mocker):
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    print_done()
-    assert 'DONE\n' == console_patched.file.getvalue()
-
-
-def test_print_error(mocker):
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.error_console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True, stderr=True),
-    )
-
-    print_error('test_message')
-    assert 'test_message\n' == console_patched.file.getvalue()
-
-
-def test_print_success(mocker):
-    console_patched = mocker.patch(
-        'aos_prov.utils.common.console',
-        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
-    )
-
-    print_success('test_message')
-    assert 'test_message\n' == console_patched.file.getvalue()
-
-
-def test_generate_random_password():
-    assert generate_random_password() != generate_random_password()
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+import io
+
+from aos_prov.utils.common import (
+    generate_random_password,
+    print_done,
+    print_error,
+    print_left,
+    print_message,
+    print_success,
+)
+from rich.console import Console
+
+
+def test_print_message(mocker):
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    print_message('test_message', ljust=1)
+    assert 'test_message\n' == console_patched.file.getvalue()
+
+
+def test_print_left(mocker):
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    print_left('test_message')
+    assert 'test_message' in console_patched.file.getvalue()
+
+
+def test_print_done(mocker):
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    print_done()
+    assert 'DONE\n' == console_patched.file.getvalue()
+
+
+def test_print_error(mocker):
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.error_console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True, stderr=True),
+    )
+
+    print_error('test_message')
+    assert 'test_message\n' == console_patched.file.getvalue()
+
+
+def test_print_success(mocker):
+    console_patched = mocker.patch(
+        'aos_prov.utils.common.console',
+        new=Console(file=io.StringIO(), width=120, soft_wrap=True),
+    )
+
+    print_success('test_message')
+    assert 'test_message\n' == console_patched.file.getvalue()
+
+
+def test_generate_random_password():
+    assert generate_random_password() != generate_random_password()
```

## tests/utils/test_config.py

 * *Ordering differences only*

```diff
@@ -1,39 +1,39 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-import unittest
-
-from aos_prov.utils.config import Config
-
-
-class TestConfig(unittest.TestCase):
-    def test_config_can_be_created(self):
-        c = Config()
-        self.assertIsInstance(c, Config)
-
-    def test_setters_and_getters(self):
-        c = Config()
-        c.system_id = 'some system id'
-        self.assertEqual(c.system_id, 'some system id')
-
-        c.protocol_version = 5
-        self.assertEqual(c.protocol_version, 5)
-
-        c.node_ids = ['dom0', 'dom1']
-        self.assertEqual(c.node_ids, ['dom0', 'dom1'])
-
-        c.supported_cert_types = ['um', 'sm']
-        self.assertEqual(c.supported_cert_types, ['um', 'sm'])
-
-        c.set_model('model;1.0.0')
-        self.assertEqual(c.model_name, 'model')
-        self.assertEqual(c.model_version, '1.0.0')
-
-        c.set_model('model')
-        self.assertEqual(c.model_name, 'model')
-        self.assertEqual(c.model_version, 'Unknown')
-
-        c.unit_certificates = ['online', 'offline']
-        self.assertEqual(c.unit_certificates, ['online', 'offline'])
-
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+import unittest
+
+from aos_prov.utils.config import Config
+
+
+class TestConfig(unittest.TestCase):
+    def test_config_can_be_created(self):
+        c = Config()
+        self.assertIsInstance(c, Config)
+
+    def test_setters_and_getters(self):
+        c = Config()
+        c.system_id = 'some system id'
+        self.assertEqual(c.system_id, 'some system id')
+
+        c.protocol_version = 5
+        self.assertEqual(c.protocol_version, 5)
+
+        c.node_ids = ['dom0', 'dom1']
+        self.assertEqual(c.node_ids, ['dom0', 'dom1'])
+
+        c.supported_cert_types = ['um', 'sm']
+        self.assertEqual(c.supported_cert_types, ['um', 'sm'])
+
+        c.set_model('model;1.0.0')
+        self.assertEqual(c.model_name, 'model')
+        self.assertEqual(c.model_version, '1.0.0')
+
+        c.set_model('model')
+        self.assertEqual(c.model_name, 'model')
+        self.assertEqual(c.model_version, 'Unknown')
+
+        c.unit_certificates = ['online', 'offline']
+        self.assertEqual(c.unit_certificates, ['online', 'offline'])
+
```

## tests/utils/test_unit_certificate.py

 * *Ordering differences only*

```diff
@@ -1,28 +1,28 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-import unittest
-
-from aos_prov.utils.unit_certificate import UnitCertificate
-
-
-class TestUnitCertificate(unittest.TestCase):
-    def test_object_can_be_created(self):
-        uc = UnitCertificate()
-        self.assertIsInstance(uc, UnitCertificate)
-
-    def test_attributes(self):
-        uc = UnitCertificate()
-
-        uc.cert_type = 'type1'
-        self.assertEqual(uc.cert_type, 'type1')
-
-        uc.certificate = 'some cert 1'
-        self.assertEqual(uc.certificate, 'some cert 1')
-
-        uc.node_id = 'node_id'
-        self.assertEqual(uc.node_id, 'node_id')
-
-        uc.csr = 'csr'
-        self.assertEqual(uc.csr, 'csr')
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+import unittest
+
+from aos_prov.utils.unit_certificate import UnitCertificate
+
+
+class TestUnitCertificate(unittest.TestCase):
+    def test_object_can_be_created(self):
+        uc = UnitCertificate()
+        self.assertIsInstance(uc, UnitCertificate)
+
+    def test_attributes(self):
+        uc = UnitCertificate()
+
+        uc.cert_type = 'type1'
+        self.assertEqual(uc.cert_type, 'type1')
+
+        uc.certificate = 'some cert 1'
+        self.assertEqual(uc.certificate, 'some cert 1')
+
+        uc.node_id = 'node_id'
+        self.assertEqual(uc.node_id, 'node_id')
+
+        uc.csr = 'csr'
+        self.assertEqual(uc.csr, 'csr')
```

## tests/utils/test_user_credentials.py

 * *Ordering differences only*

```diff
@@ -1,104 +1,104 @@
-#
-#  Copyright (c) 2018-2024 Renesas Inc.
-#  Copyright (c) 2018-2024 EPAM Systems Inc.
-#
-import tempfile
-import unittest
-
-from aos_prov.utils.errors import UserCredentialsError
-from aos_prov.utils.user_credentials import TempCredentials, UserCredentials
-from cryptography.hazmat.primitives._serialization import (
-    Encoding,
-    NoEncryption,
-    PrivateFormat,
-)
-from tests.fixtures import (
-    generate_ca_key_and_cert,
-    generate_test_key_certificate,
-    key_cert_to_pkcs12,
-)
-
-
-class TestTempCredentials(unittest.TestCase):
-    def test_context_management(self):
-        ca_key, ca_cert = generate_ca_key_and_cert()
-        key, cert = generate_test_key_certificate(ca_key)
-
-        cert_pem_bytes = cert.public_bytes(encoding=Encoding.PEM)
-
-        private_key_pem_bytes = key.private_bytes(
-            encoding=Encoding.PEM,
-            format=PrivateFormat.PKCS8,
-            encryption_algorithm=NoEncryption(),
-        )
-        with TempCredentials(cert_pem_bytes, private_key_pem_bytes, None, None) as temp_creds:
-            self.assertIsNotNone(temp_creds.cert_file_name)
-            self.assertIsNotNone(temp_creds.key_file_name)
-
-
-class TestUserCredentials(unittest.TestCase):
-    def test_create_with_pkcs12(self):
-        ca_key, ca_cert = generate_ca_key_and_cert()
-        key, cert = generate_test_key_certificate(ca_key)
-        pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
-
-        with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
-            temp_cert.write(pkcs_12_cert)
-            temp_cert.seek(0)
-            uc = UserCredentials('cert', 'key', temp_cert.name)
-
-        uc.cert_type = 'type1'
-        self.assertEqual(uc.cert_type, 'type1')
-
-        uc.certificate = 'some cert 1'
-        self.assertEqual(uc.certificate, 'some cert 1')
-
-        uc.csr = 'csr'
-        self.assertEqual(uc.csr, 'csr')
-
-        self.assertEqual(uc.cloud_url, 'developer.test.local')
-        self.assertIsNotNone(uc.user_credentials)
-
-    def test_create_without_pkcs12(self):
-        ca_key, ca_cert = generate_ca_key_and_cert()
-        key, cert = generate_test_key_certificate(ca_key)
-
-        cert_pem_bytes = cert.public_bytes(encoding=Encoding.PEM)
-        cert_file = tempfile.NamedTemporaryFile(delete=True)
-        cert_file.write(cert_pem_bytes)
-        cert_file.seek(0)
-
-        private_key_pem_bytes = key.private_bytes(
-            encoding=Encoding.PEM,
-            format=PrivateFormat.PKCS8,
-            encryption_algorithm=NoEncryption(),
-        )
-        key_file = tempfile.NamedTemporaryFile(delete=True)
-        key_file.write(private_key_pem_bytes)
-        key_file.seek(0)
-
-        uc1 = UserCredentials(cert_file.name, key_file.name, 'fake_pkcs12')
-
-        self.assertEqual(uc1.cloud_url, 'developer.test.local')
-        self.assertIsNotNone(uc1.user_credentials)
-
-        uc2 = UserCredentials(cert_file.name, key_file.name, None)
-
-        self.assertEqual(uc2.cloud_url, 'developer.test.local')
-        self.assertIsNotNone(uc2.user_credentials)
-
-        with self.assertRaises(UserCredentialsError) as exc:
-            UserCredentials('cert_file', key_file.name, None)
-
-        self.assertEqual(str(exc.exception), 'User credentials file cert_file not found.')
-
-        with self.assertRaises(UserCredentialsError) as exc:
-            UserCredentials(cert_file.name, 'key_file', None)
-
-        self.assertEqual(str(exc.exception), 'User credentials file key_file not found.')
-
-    def test_file_not_found(self):
-        with self.assertRaises(UserCredentialsError) as exc:
-            UserCredentials('cert', 'key', 'fake_pkcs12')
-
-        self.assertEqual(str(exc.exception), 'User credentials file fake_pkcs12 not found.')
+#
+#  Copyright (c) 2018-2024 Renesas Inc.
+#  Copyright (c) 2018-2024 EPAM Systems Inc.
+#
+import tempfile
+import unittest
+
+from aos_prov.utils.errors import UserCredentialsError
+from aos_prov.utils.user_credentials import TempCredentials, UserCredentials
+from cryptography.hazmat.primitives._serialization import (
+    Encoding,
+    NoEncryption,
+    PrivateFormat,
+)
+from tests.fixtures import (
+    generate_ca_key_and_cert,
+    generate_test_key_certificate,
+    key_cert_to_pkcs12,
+)
+
+
+class TestTempCredentials(unittest.TestCase):
+    def test_context_management(self):
+        ca_key, ca_cert = generate_ca_key_and_cert()
+        key, cert = generate_test_key_certificate(ca_key)
+
+        cert_pem_bytes = cert.public_bytes(encoding=Encoding.PEM)
+
+        private_key_pem_bytes = key.private_bytes(
+            encoding=Encoding.PEM,
+            format=PrivateFormat.PKCS8,
+            encryption_algorithm=NoEncryption(),
+        )
+        with TempCredentials(cert_pem_bytes, private_key_pem_bytes, None, None) as temp_creds:
+            self.assertIsNotNone(temp_creds.cert_file_name)
+            self.assertIsNotNone(temp_creds.key_file_name)
+
+
+class TestUserCredentials(unittest.TestCase):
+    def test_create_with_pkcs12(self):
+        ca_key, ca_cert = generate_ca_key_and_cert()
+        key, cert = generate_test_key_certificate(ca_key)
+        pkcs_12_cert = key_cert_to_pkcs12(key, cert, ca_cert)
+
+        with tempfile.NamedTemporaryFile(delete=True) as temp_cert:
+            temp_cert.write(pkcs_12_cert)
+            temp_cert.seek(0)
+            uc = UserCredentials('cert', 'key', temp_cert.name)
+
+        uc.cert_type = 'type1'
+        self.assertEqual(uc.cert_type, 'type1')
+
+        uc.certificate = 'some cert 1'
+        self.assertEqual(uc.certificate, 'some cert 1')
+
+        uc.csr = 'csr'
+        self.assertEqual(uc.csr, 'csr')
+
+        self.assertEqual(uc.cloud_url, 'developer.test.local')
+        self.assertIsNotNone(uc.user_credentials)
+
+    def test_create_without_pkcs12(self):
+        ca_key, ca_cert = generate_ca_key_and_cert()
+        key, cert = generate_test_key_certificate(ca_key)
+
+        cert_pem_bytes = cert.public_bytes(encoding=Encoding.PEM)
+        cert_file = tempfile.NamedTemporaryFile(delete=True)
+        cert_file.write(cert_pem_bytes)
+        cert_file.seek(0)
+
+        private_key_pem_bytes = key.private_bytes(
+            encoding=Encoding.PEM,
+            format=PrivateFormat.PKCS8,
+            encryption_algorithm=NoEncryption(),
+        )
+        key_file = tempfile.NamedTemporaryFile(delete=True)
+        key_file.write(private_key_pem_bytes)
+        key_file.seek(0)
+
+        uc1 = UserCredentials(cert_file.name, key_file.name, 'fake_pkcs12')
+
+        self.assertEqual(uc1.cloud_url, 'developer.test.local')
+        self.assertIsNotNone(uc1.user_credentials)
+
+        uc2 = UserCredentials(cert_file.name, key_file.name, None)
+
+        self.assertEqual(uc2.cloud_url, 'developer.test.local')
+        self.assertIsNotNone(uc2.user_credentials)
+
+        with self.assertRaises(UserCredentialsError) as exc:
+            UserCredentials('cert_file', key_file.name, None)
+
+        self.assertEqual(str(exc.exception), 'User credentials file cert_file not found.')
+
+        with self.assertRaises(UserCredentialsError) as exc:
+            UserCredentials(cert_file.name, 'key_file', None)
+
+        self.assertEqual(str(exc.exception), 'User credentials file key_file not found.')
+
+    def test_file_not_found(self):
+        with self.assertRaises(UserCredentialsError) as exc:
+            UserCredentials('cert', 'key', 'fake_pkcs12')
+
+        self.assertEqual(str(exc.exception), 'User credentials file fake_pkcs12 not found.')
```

## Comparing `aos_prov/communication/unit/v3/generated/iamanagerprotected_pb2.py` & `aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,631 +1,799 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: iamanager/v3/iamanagerprotected.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from aos_prov.communication.unit.v3.generated import iamanagercommon_pb2 as iamanager_dot_v3_dot_iamanagercommon__pb2
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='iamanager/v3/iamanagerprotected.proto',
-  package='iamanager.v3',
-  syntax='proto3',
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n%iamanager/v3/iamanagerprotected.proto\x12\x0ciamanager.v3\x1a\x1bgoogle/protobuf/empty.proto\x1a\"iamanager/v3/iamanagercommon.proto\"\x1c\n\x0c\x43learRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\"1\n\x0fSetOwnerRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"2\n\x10\x43reateKeyRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\".\n\x11\x43reateKeyResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0b\n\x03\x63sr\x18\x02 \x01(\t\".\n\x10\x41pplyCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x02 \x01(\t\"3\n\x11\x41pplyCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\"\xc7\x01\n\x16RegisterServiceRequest\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12J\n\x0bpermissions\x18\x02 \x03(\x0b\x32\x35.iamanager.v3.RegisterServiceRequest.PermissionsEntry\x1aM\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.iamanager.v3.Permissions:\x02\x38\x01\")\n\x17RegisterServiceResponse\x12\x0e\n\x06secret\x18\x01 \x01(\t\".\n\x18UnregisterServiceRequest\x12\x12\n\nservice_id\x18\x01 \x01(\t\"&\n\x12\x45ncryptDiskRequest\x12\x10\n\x08password\x18\x01 \x01(\t2\xc0\x05\n\x13IAMProtectedService\x12\x43\n\x08SetOwner\x12\x1d.iamanager.v3.SetOwnerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x05\x43lear\x12\x1a.iamanager.v3.ClearRequest\x1a\x16.google.protobuf.Empty\"\x00\x12N\n\tCreateKey\x12\x1e.iamanager.v3.CreateKeyRequest\x1a\x1f.iamanager.v3.CreateKeyResponse\"\x00\x12N\n\tApplyCert\x12\x1e.iamanager.v3.ApplyCertRequest\x1a\x1f.iamanager.v3.ApplyCertResponse\"\x00\x12I\n\x0b\x45ncryptDisk\x12 .iamanager.v3.EncryptDiskRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x39\n\x08SetUsers\x12\x13.iamanager.v3.Users\x1a\x16.google.protobuf.Empty\"\x00\x12`\n\x0fRegisterService\x12$.iamanager.v3.RegisterServiceRequest\x1a%.iamanager.v3.RegisterServiceResponse\"\x00\x12U\n\x11UnregisterService\x12&.iamanager.v3.UnregisterServiceRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3'
-  ,
-  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,iamanager_dot_v3_dot_iamanagercommon__pb2.DESCRIPTOR,])
-
-
-
-
-_CLEARREQUEST = _descriptor.Descriptor(
-  name='ClearRequest',
-  full_name='iamanager.v3.ClearRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v3.ClearRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=120,
-  serialized_end=148,
-)
-
-
-_SETOWNERREQUEST = _descriptor.Descriptor(
-  name='SetOwnerRequest',
-  full_name='iamanager.v3.SetOwnerRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v3.SetOwnerRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.v3.SetOwnerRequest.password', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=150,
-  serialized_end=199,
-)
-
-
-_CREATEKEYREQUEST = _descriptor.Descriptor(
-  name='CreateKeyRequest',
-  full_name='iamanager.v3.CreateKeyRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v3.CreateKeyRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.v3.CreateKeyRequest.password', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=201,
-  serialized_end=251,
-)
-
-
-_CREATEKEYRESPONSE = _descriptor.Descriptor(
-  name='CreateKeyResponse',
-  full_name='iamanager.v3.CreateKeyResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v3.CreateKeyResponse.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='csr', full_name='iamanager.v3.CreateKeyResponse.csr', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=253,
-  serialized_end=299,
-)
-
-
-_APPLYCERTREQUEST = _descriptor.Descriptor(
-  name='ApplyCertRequest',
-  full_name='iamanager.v3.ApplyCertRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v3.ApplyCertRequest.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cert', full_name='iamanager.v3.ApplyCertRequest.cert', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=301,
-  serialized_end=347,
-)
-
-
-_APPLYCERTRESPONSE = _descriptor.Descriptor(
-  name='ApplyCertResponse',
-  full_name='iamanager.v3.ApplyCertResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='iamanager.v3.ApplyCertResponse.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cert_url', full_name='iamanager.v3.ApplyCertResponse.cert_url', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=349,
-  serialized_end=400,
-)
-
-
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY = _descriptor.Descriptor(
-  name='PermissionsEntry',
-  full_name='iamanager.v3.RegisterServiceRequest.PermissionsEntry',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='key', full_name='iamanager.v3.RegisterServiceRequest.PermissionsEntry.key', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='value', full_name='iamanager.v3.RegisterServiceRequest.PermissionsEntry.value', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=b'8\001',
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=525,
-  serialized_end=602,
-)
-
-_REGISTERSERVICEREQUEST = _descriptor.Descriptor(
-  name='RegisterServiceRequest',
-  full_name='iamanager.v3.RegisterServiceRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='service_id', full_name='iamanager.v3.RegisterServiceRequest.service_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='permissions', full_name='iamanager.v3.RegisterServiceRequest.permissions', index=1,
-      number=2, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[_REGISTERSERVICEREQUEST_PERMISSIONSENTRY, ],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=403,
-  serialized_end=602,
-)
-
-
-_REGISTERSERVICERESPONSE = _descriptor.Descriptor(
-  name='RegisterServiceResponse',
-  full_name='iamanager.v3.RegisterServiceResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='secret', full_name='iamanager.v3.RegisterServiceResponse.secret', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=604,
-  serialized_end=645,
-)
-
-
-_UNREGISTERSERVICEREQUEST = _descriptor.Descriptor(
-  name='UnregisterServiceRequest',
-  full_name='iamanager.v3.UnregisterServiceRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='service_id', full_name='iamanager.v3.UnregisterServiceRequest.service_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=647,
-  serialized_end=693,
-)
-
-
-_ENCRYPTDISKREQUEST = _descriptor.Descriptor(
-  name='EncryptDiskRequest',
-  full_name='iamanager.v3.EncryptDiskRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='password', full_name='iamanager.v3.EncryptDiskRequest.password', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=695,
-  serialized_end=733,
-)
-
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY.fields_by_name['value'].message_type = iamanager_dot_v3_dot_iamanagercommon__pb2._PERMISSIONS
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY.containing_type = _REGISTERSERVICEREQUEST
-_REGISTERSERVICEREQUEST.fields_by_name['permissions'].message_type = _REGISTERSERVICEREQUEST_PERMISSIONSENTRY
-DESCRIPTOR.message_types_by_name['ClearRequest'] = _CLEARREQUEST
-DESCRIPTOR.message_types_by_name['SetOwnerRequest'] = _SETOWNERREQUEST
-DESCRIPTOR.message_types_by_name['CreateKeyRequest'] = _CREATEKEYREQUEST
-DESCRIPTOR.message_types_by_name['CreateKeyResponse'] = _CREATEKEYRESPONSE
-DESCRIPTOR.message_types_by_name['ApplyCertRequest'] = _APPLYCERTREQUEST
-DESCRIPTOR.message_types_by_name['ApplyCertResponse'] = _APPLYCERTRESPONSE
-DESCRIPTOR.message_types_by_name['RegisterServiceRequest'] = _REGISTERSERVICEREQUEST
-DESCRIPTOR.message_types_by_name['RegisterServiceResponse'] = _REGISTERSERVICERESPONSE
-DESCRIPTOR.message_types_by_name['UnregisterServiceRequest'] = _UNREGISTERSERVICEREQUEST
-DESCRIPTOR.message_types_by_name['EncryptDiskRequest'] = _ENCRYPTDISKREQUEST
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-ClearRequest = _reflection.GeneratedProtocolMessageType('ClearRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CLEARREQUEST,
-  '__module__' : 'iamanager.v3.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v3.ClearRequest)
-  })
-_sym_db.RegisterMessage(ClearRequest)
-
-SetOwnerRequest = _reflection.GeneratedProtocolMessageType('SetOwnerRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SETOWNERREQUEST,
-  '__module__' : 'iamanager.v3.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v3.SetOwnerRequest)
-  })
-_sym_db.RegisterMessage(SetOwnerRequest)
-
-CreateKeyRequest = _reflection.GeneratedProtocolMessageType('CreateKeyRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYREQUEST,
-  '__module__' : 'iamanager.v3.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v3.CreateKeyRequest)
-  })
-_sym_db.RegisterMessage(CreateKeyRequest)
-
-CreateKeyResponse = _reflection.GeneratedProtocolMessageType('CreateKeyResponse', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYRESPONSE,
-  '__module__' : 'iamanager.v3.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v3.CreateKeyResponse)
-  })
-_sym_db.RegisterMessage(CreateKeyResponse)
-
-ApplyCertRequest = _reflection.GeneratedProtocolMessageType('ApplyCertRequest', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTREQUEST,
-  '__module__' : 'iamanager.v3.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v3.ApplyCertRequest)
-  })
-_sym_db.RegisterMessage(ApplyCertRequest)
-
-ApplyCertResponse = _reflection.GeneratedProtocolMessageType('ApplyCertResponse', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTRESPONSE,
-  '__module__' : 'iamanager.v3.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v3.ApplyCertResponse)
-  })
-_sym_db.RegisterMessage(ApplyCertResponse)
-
-RegisterServiceRequest = _reflection.GeneratedProtocolMessageType('RegisterServiceRequest', (_message.Message,), {
-
-  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _REGISTERSERVICEREQUEST_PERMISSIONSENTRY,
-    '__module__' : 'iamanager.v3.iamanagerprotected_pb2'
-    # @@protoc_insertion_point(class_scope:iamanager.v3.RegisterServiceRequest.PermissionsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _REGISTERSERVICEREQUEST,
-  '__module__' : 'iamanager.v3.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v3.RegisterServiceRequest)
-  })
-_sym_db.RegisterMessage(RegisterServiceRequest)
-_sym_db.RegisterMessage(RegisterServiceRequest.PermissionsEntry)
-
-RegisterServiceResponse = _reflection.GeneratedProtocolMessageType('RegisterServiceResponse', (_message.Message,), {
-  'DESCRIPTOR' : _REGISTERSERVICERESPONSE,
-  '__module__' : 'iamanager.v3.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v3.RegisterServiceResponse)
-  })
-_sym_db.RegisterMessage(RegisterServiceResponse)
-
-UnregisterServiceRequest = _reflection.GeneratedProtocolMessageType('UnregisterServiceRequest', (_message.Message,), {
-  'DESCRIPTOR' : _UNREGISTERSERVICEREQUEST,
-  '__module__' : 'iamanager.v3.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v3.UnregisterServiceRequest)
-  })
-_sym_db.RegisterMessage(UnregisterServiceRequest)
-
-EncryptDiskRequest = _reflection.GeneratedProtocolMessageType('EncryptDiskRequest', (_message.Message,), {
-  'DESCRIPTOR' : _ENCRYPTDISKREQUEST,
-  '__module__' : 'iamanager.v3.iamanagerprotected_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v3.EncryptDiskRequest)
-  })
-_sym_db.RegisterMessage(EncryptDiskRequest)
-
-
-_REGISTERSERVICEREQUEST_PERMISSIONSENTRY._options = None
-
-_IAMPROTECTEDSERVICE = _descriptor.ServiceDescriptor(
-  name='IAMProtectedService',
-  full_name='iamanager.v3.IAMProtectedService',
-  file=DESCRIPTOR,
-  index=0,
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_start=736,
-  serialized_end=1440,
-  methods=[
-  _descriptor.MethodDescriptor(
-    name='SetOwner',
-    full_name='iamanager.v3.IAMProtectedService.SetOwner',
-    index=0,
-    containing_service=None,
-    input_type=_SETOWNERREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='Clear',
-    full_name='iamanager.v3.IAMProtectedService.Clear',
-    index=1,
-    containing_service=None,
-    input_type=_CLEARREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='CreateKey',
-    full_name='iamanager.v3.IAMProtectedService.CreateKey',
-    index=2,
-    containing_service=None,
-    input_type=_CREATEKEYREQUEST,
-    output_type=_CREATEKEYRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='ApplyCert',
-    full_name='iamanager.v3.IAMProtectedService.ApplyCert',
-    index=3,
-    containing_service=None,
-    input_type=_APPLYCERTREQUEST,
-    output_type=_APPLYCERTRESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='EncryptDisk',
-    full_name='iamanager.v3.IAMProtectedService.EncryptDisk',
-    index=4,
-    containing_service=None,
-    input_type=_ENCRYPTDISKREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='FinishProvisioning',
-    full_name='iamanager.v3.IAMProtectedService.FinishProvisioning',
-    index=5,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='SetUsers',
-    full_name='iamanager.v3.IAMProtectedService.SetUsers',
-    index=6,
-    containing_service=None,
-    input_type=iamanager_dot_v3_dot_iamanagercommon__pb2._USERS,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='RegisterService',
-    full_name='iamanager.v3.IAMProtectedService.RegisterService',
-    index=7,
-    containing_service=None,
-    input_type=_REGISTERSERVICEREQUEST,
-    output_type=_REGISTERSERVICERESPONSE,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='UnregisterService',
-    full_name='iamanager.v3.IAMProtectedService.UnregisterService',
-    index=8,
-    containing_service=None,
-    input_type=_UNREGISTERSERVICEREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-])
-_sym_db.RegisterServiceDescriptor(_IAMPROTECTEDSERVICE)
-
-DESCRIPTOR.services_by_name['IAMProtectedService'] = _IAMPROTECTEDSERVICE
-
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: api_iamanager_iamanager.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='api_iamanager_iamanager.proto',
+  package='iamanager',
+  syntax='proto3',
+  serialized_options=b'Z2gitpct.epam.com/epmd-aepr/aos_common/api/iamanager',
+  create_key=_descriptor._internal_create_key,
+  serialized_pb=b'\n\x1d\x61pi_iamanager_iamanager.proto\x12\tiamanager\x1a\x1bgoogle/protobuf/empty.proto\" \n\x0fGetCertTypesRsp\x12\r\n\x05types\x18\x01 \x03(\t\"\x18\n\x08\x43learReq\x12\x0c\n\x04type\x18\x01 \x01(\t\"-\n\x0bSetOwnerReq\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\".\n\x0c\x43reateKeyReq\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\")\n\x0c\x43reateKeyRsp\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0b\n\x03\x63sr\x18\x02 \x01(\t\"*\n\x0c\x41pplyCertReq\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x02 \x01(\t\".\n\x0c\x41pplyCertRsp\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\":\n\nGetCertReq\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"=\n\nGetCertRsp\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\":\n\x10GetSystemInfoRsp\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t\"\x1c\n\x0bSetUsersReq\x12\r\n\x05users\x18\x01 \x03(\t\"\x1c\n\x0bGetUsersRsp\x12\r\n\x05users\x18\x01 \x03(\t\" \n\x0fUsersChangedNtf\x12\r\n\x05users\x18\x01 \x03(\t\"\"\n\x0e\x45ncryptDiskReq\x12\x10\n\x08password\x18\x01 \x01(\t2\xa5\x06\n\tIAManager\x12\x44\n\x0cGetCertTypes\x12\x16.google.protobuf.Empty\x1a\x1a.iamanager.GetCertTypesRsp\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x36\n\x05\x43lear\x12\x13.iamanager.ClearReq\x1a\x16.google.protobuf.Empty\"\x00\x12<\n\x08SetOwner\x12\x16.iamanager.SetOwnerReq\x1a\x16.google.protobuf.Empty\"\x00\x12?\n\tCreateKey\x12\x17.iamanager.CreateKeyReq\x1a\x17.iamanager.CreateKeyRsp\"\x00\x12?\n\tApplyCert\x12\x17.iamanager.ApplyCertReq\x1a\x17.iamanager.ApplyCertRsp\"\x00\x12\x39\n\x07GetCert\x12\x15.iamanager.GetCertReq\x1a\x15.iamanager.GetCertRsp\"\x00\x12\x46\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x1b.iamanager.GetSystemInfoRsp\"\x00\x12<\n\x08SetUsers\x12\x16.iamanager.SetUsersReq\x1a\x16.google.protobuf.Empty\"\x00\x12<\n\x08GetUsers\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.GetUsersRsp\"\x00\x12O\n\x15SubscribeUsersChanged\x12\x16.google.protobuf.Empty\x1a\x1a.iamanager.UsersChangedNtf\"\x00\x30\x01\x12\x42\n\x0b\x45ncryptDisk\x12\x19.iamanager.EncryptDiskReq\x1a\x16.google.protobuf.Empty\"\x00\x42\x34Z2gitpct.epam.com/epmd-aepr/aos_common/api/iamanagerb\x06proto3'
+  ,
+  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,])
+
+
+
+
+_GETCERTTYPESRSP = _descriptor.Descriptor(
+  name='GetCertTypesRsp',
+  full_name='iamanager.GetCertTypesRsp',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='types', full_name='iamanager.GetCertTypesRsp.types', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=73,
+  serialized_end=105,
+)
+
+
+_CLEARREQ = _descriptor.Descriptor(
+  name='ClearReq',
+  full_name='iamanager.ClearReq',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.ClearReq.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=107,
+  serialized_end=131,
+)
+
+
+_SETOWNERREQ = _descriptor.Descriptor(
+  name='SetOwnerReq',
+  full_name='iamanager.SetOwnerReq',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.SetOwnerReq.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.SetOwnerReq.password', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=133,
+  serialized_end=178,
+)
+
+
+_CREATEKEYREQ = _descriptor.Descriptor(
+  name='CreateKeyReq',
+  full_name='iamanager.CreateKeyReq',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.CreateKeyReq.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.CreateKeyReq.password', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=180,
+  serialized_end=226,
+)
+
+
+_CREATEKEYRSP = _descriptor.Descriptor(
+  name='CreateKeyRsp',
+  full_name='iamanager.CreateKeyRsp',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.CreateKeyRsp.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='csr', full_name='iamanager.CreateKeyRsp.csr', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=228,
+  serialized_end=269,
+)
+
+
+_APPLYCERTREQ = _descriptor.Descriptor(
+  name='ApplyCertReq',
+  full_name='iamanager.ApplyCertReq',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.ApplyCertReq.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert', full_name='iamanager.ApplyCertReq.cert', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=271,
+  serialized_end=313,
+)
+
+
+_APPLYCERTRSP = _descriptor.Descriptor(
+  name='ApplyCertRsp',
+  full_name='iamanager.ApplyCertRsp',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.ApplyCertRsp.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert_url', full_name='iamanager.ApplyCertRsp.cert_url', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=315,
+  serialized_end=361,
+)
+
+
+_GETCERTREQ = _descriptor.Descriptor(
+  name='GetCertReq',
+  full_name='iamanager.GetCertReq',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.GetCertReq.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='issuer', full_name='iamanager.GetCertReq.issuer', index=1,
+      number=2, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='serial', full_name='iamanager.GetCertReq.serial', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=363,
+  serialized_end=421,
+)
+
+
+_GETCERTRSP = _descriptor.Descriptor(
+  name='GetCertRsp',
+  full_name='iamanager.GetCertRsp',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='iamanager.GetCertRsp.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cert_url', full_name='iamanager.GetCertRsp.cert_url', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='key_url', full_name='iamanager.GetCertRsp.key_url', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=423,
+  serialized_end=484,
+)
+
+
+_GETSYSTEMINFORSP = _descriptor.Descriptor(
+  name='GetSystemInfoRsp',
+  full_name='iamanager.GetSystemInfoRsp',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='system_id', full_name='iamanager.GetSystemInfoRsp.system_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='board_model', full_name='iamanager.GetSystemInfoRsp.board_model', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=486,
+  serialized_end=544,
+)
+
+
+_SETUSERSREQ = _descriptor.Descriptor(
+  name='SetUsersReq',
+  full_name='iamanager.SetUsersReq',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='users', full_name='iamanager.SetUsersReq.users', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=546,
+  serialized_end=574,
+)
+
+
+_GETUSERSRSP = _descriptor.Descriptor(
+  name='GetUsersRsp',
+  full_name='iamanager.GetUsersRsp',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='users', full_name='iamanager.GetUsersRsp.users', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=576,
+  serialized_end=604,
+)
+
+
+_USERSCHANGEDNTF = _descriptor.Descriptor(
+  name='UsersChangedNtf',
+  full_name='iamanager.UsersChangedNtf',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='users', full_name='iamanager.UsersChangedNtf.users', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=606,
+  serialized_end=638,
+)
+
+
+_ENCRYPTDISKREQ = _descriptor.Descriptor(
+  name='EncryptDiskReq',
+  full_name='iamanager.EncryptDiskReq',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='password', full_name='iamanager.EncryptDiskReq.password', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=640,
+  serialized_end=674,
+)
+
+DESCRIPTOR.message_types_by_name['GetCertTypesRsp'] = _GETCERTTYPESRSP
+DESCRIPTOR.message_types_by_name['ClearReq'] = _CLEARREQ
+DESCRIPTOR.message_types_by_name['SetOwnerReq'] = _SETOWNERREQ
+DESCRIPTOR.message_types_by_name['CreateKeyReq'] = _CREATEKEYREQ
+DESCRIPTOR.message_types_by_name['CreateKeyRsp'] = _CREATEKEYRSP
+DESCRIPTOR.message_types_by_name['ApplyCertReq'] = _APPLYCERTREQ
+DESCRIPTOR.message_types_by_name['ApplyCertRsp'] = _APPLYCERTRSP
+DESCRIPTOR.message_types_by_name['GetCertReq'] = _GETCERTREQ
+DESCRIPTOR.message_types_by_name['GetCertRsp'] = _GETCERTRSP
+DESCRIPTOR.message_types_by_name['GetSystemInfoRsp'] = _GETSYSTEMINFORSP
+DESCRIPTOR.message_types_by_name['SetUsersReq'] = _SETUSERSREQ
+DESCRIPTOR.message_types_by_name['GetUsersRsp'] = _GETUSERSRSP
+DESCRIPTOR.message_types_by_name['UsersChangedNtf'] = _USERSCHANGEDNTF
+DESCRIPTOR.message_types_by_name['EncryptDiskReq'] = _ENCRYPTDISKREQ
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+GetCertTypesRsp = _reflection.GeneratedProtocolMessageType('GetCertTypesRsp', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTTYPESRSP,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.GetCertTypesRsp)
+  })
+_sym_db.RegisterMessage(GetCertTypesRsp)
+
+ClearReq = _reflection.GeneratedProtocolMessageType('ClearReq', (_message.Message,), {
+  'DESCRIPTOR' : _CLEARREQ,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.ClearReq)
+  })
+_sym_db.RegisterMessage(ClearReq)
+
+SetOwnerReq = _reflection.GeneratedProtocolMessageType('SetOwnerReq', (_message.Message,), {
+  'DESCRIPTOR' : _SETOWNERREQ,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.SetOwnerReq)
+  })
+_sym_db.RegisterMessage(SetOwnerReq)
+
+CreateKeyReq = _reflection.GeneratedProtocolMessageType('CreateKeyReq', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYREQ,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.CreateKeyReq)
+  })
+_sym_db.RegisterMessage(CreateKeyReq)
+
+CreateKeyRsp = _reflection.GeneratedProtocolMessageType('CreateKeyRsp', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYRSP,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.CreateKeyRsp)
+  })
+_sym_db.RegisterMessage(CreateKeyRsp)
+
+ApplyCertReq = _reflection.GeneratedProtocolMessageType('ApplyCertReq', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTREQ,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.ApplyCertReq)
+  })
+_sym_db.RegisterMessage(ApplyCertReq)
+
+ApplyCertRsp = _reflection.GeneratedProtocolMessageType('ApplyCertRsp', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTRSP,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.ApplyCertRsp)
+  })
+_sym_db.RegisterMessage(ApplyCertRsp)
+
+GetCertReq = _reflection.GeneratedProtocolMessageType('GetCertReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTREQ,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.GetCertReq)
+  })
+_sym_db.RegisterMessage(GetCertReq)
+
+GetCertRsp = _reflection.GeneratedProtocolMessageType('GetCertRsp', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTRSP,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.GetCertRsp)
+  })
+_sym_db.RegisterMessage(GetCertRsp)
+
+GetSystemInfoRsp = _reflection.GeneratedProtocolMessageType('GetSystemInfoRsp', (_message.Message,), {
+  'DESCRIPTOR' : _GETSYSTEMINFORSP,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.GetSystemInfoRsp)
+  })
+_sym_db.RegisterMessage(GetSystemInfoRsp)
+
+SetUsersReq = _reflection.GeneratedProtocolMessageType('SetUsersReq', (_message.Message,), {
+  'DESCRIPTOR' : _SETUSERSREQ,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.SetUsersReq)
+  })
+_sym_db.RegisterMessage(SetUsersReq)
+
+GetUsersRsp = _reflection.GeneratedProtocolMessageType('GetUsersRsp', (_message.Message,), {
+  'DESCRIPTOR' : _GETUSERSRSP,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.GetUsersRsp)
+  })
+_sym_db.RegisterMessage(GetUsersRsp)
+
+UsersChangedNtf = _reflection.GeneratedProtocolMessageType('UsersChangedNtf', (_message.Message,), {
+  'DESCRIPTOR' : _USERSCHANGEDNTF,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.UsersChangedNtf)
+  })
+_sym_db.RegisterMessage(UsersChangedNtf)
+
+EncryptDiskReq = _reflection.GeneratedProtocolMessageType('EncryptDiskReq', (_message.Message,), {
+  'DESCRIPTOR' : _ENCRYPTDISKREQ,
+  '__module__' : 'api_iamanager_iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.EncryptDiskReq)
+  })
+_sym_db.RegisterMessage(EncryptDiskReq)
+
+
+DESCRIPTOR._options = None
+
+_IAMANAGER = _descriptor.ServiceDescriptor(
+  name='IAManager',
+  full_name='iamanager.IAManager',
+  file=DESCRIPTOR,
+  index=0,
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_start=677,
+  serialized_end=1482,
+  methods=[
+  _descriptor.MethodDescriptor(
+    name='GetCertTypes',
+    full_name='iamanager.IAManager.GetCertTypes',
+    index=0,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_GETCERTTYPESRSP,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='FinishProvisioning',
+    full_name='iamanager.IAManager.FinishProvisioning',
+    index=1,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='Clear',
+    full_name='iamanager.IAManager.Clear',
+    index=2,
+    containing_service=None,
+    input_type=_CLEARREQ,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetOwner',
+    full_name='iamanager.IAManager.SetOwner',
+    index=3,
+    containing_service=None,
+    input_type=_SETOWNERREQ,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='CreateKey',
+    full_name='iamanager.IAManager.CreateKey',
+    index=4,
+    containing_service=None,
+    input_type=_CREATEKEYREQ,
+    output_type=_CREATEKEYRSP,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='ApplyCert',
+    full_name='iamanager.IAManager.ApplyCert',
+    index=5,
+    containing_service=None,
+    input_type=_APPLYCERTREQ,
+    output_type=_APPLYCERTRSP,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetCert',
+    full_name='iamanager.IAManager.GetCert',
+    index=6,
+    containing_service=None,
+    input_type=_GETCERTREQ,
+    output_type=_GETCERTRSP,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetSystemInfo',
+    full_name='iamanager.IAManager.GetSystemInfo',
+    index=7,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_GETSYSTEMINFORSP,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetUsers',
+    full_name='iamanager.IAManager.SetUsers',
+    index=8,
+    containing_service=None,
+    input_type=_SETUSERSREQ,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetUsers',
+    full_name='iamanager.IAManager.GetUsers',
+    index=9,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_GETUSERSRSP,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SubscribeUsersChanged',
+    full_name='iamanager.IAManager.SubscribeUsersChanged',
+    index=10,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_USERSCHANGEDNTF,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='EncryptDisk',
+    full_name='iamanager.IAManager.EncryptDisk',
+    index=11,
+    containing_service=None,
+    input_type=_ENCRYPTDISKREQ,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+])
+_sym_db.RegisterServiceDescriptor(_IAMANAGER)
+
+DESCRIPTOR.services_by_name['IAManager'] = _IAMANAGER
+
+# @@protoc_insertion_point(module_scope)
```

## Comparing `aos_prov-4.5.0b9.dist-info/METADATA` & `aos_prov-4.6.0b1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: aos-prov
-Version: 4.5.0b9
+Version: 4.6.0b1
 Summary: AosEdge Unit provisioning tool
+Home-page: UNKNOWN
 Author: EPAM Systems
 Author-email: support@aoscloud.io
 License: Apache License 2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: aos-keys (>=1.7.0b2)
+Requires-Dist: aos-keys (>=1.7.0)
 Requires-Dist: grpcio (>=1.44.0)
 Requires-Dist: requests (>=2.22.0)
 Requires-Dist: protobuf (<=3.20.1,>=3.14)
 Requires-Dist: protobuf (==3.20.*)
 Requires-Dist: asn1crypto (>=1.4.0)
 Requires-Dist: rich (>=10.13)
-Requires-Dist: pem (>=23.1.0)
 Requires-Dist: importlib-metadata (==4.2.0) ; python_version < "3.8"
 Requires-Dist: importlib-resources (>=3.0) ; python_version < "3.9"
 Provides-Extra: dev
 Requires-Dist: grpcio-tools (~=1.34) ; extra == 'dev'
 
 Aos provisioning tool
 =====================
@@ -99,7 +99,9 @@
 aos-prov vm-remove --name {vm-name}
 ```
 
 ### Start Unit VMs:
 ```bash
 aos-prov vm-start --name {vm-name}
 ```
+
+
```

## Comparing `aos_prov-4.5.0b9.dist-info/RECORD` & `aos_prov-4.6.0b1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,79 @@
-aos_prov/__init__.py,sha256=GG0w5d4OL0uOtGiHjbqIxaTR64BEYWYw1CULBI3cz-8,89
-aos_prov/actions.py,sha256=o6bM5bMtGdykduw22inKkUx1tOMXkvb7LBExkBVX-80,3203
-aos_prov/main.py,sha256=zXCsO9GxzLfs6VdmY9gSgNs816tP5Wr198LAPuWFyXU,8747
-aos_prov/commands/__init__.py,sha256=GG0w5d4OL0uOtGiHjbqIxaTR64BEYWYw1CULBI3cz-8,89
-aos_prov/commands/command_provision.py,sha256=1rQlc4NmBDMgIAtkM09HOD3YG8LHcweOz6kkFFFNvAs,7018
-aos_prov/commands/command_vm.py,sha256=H7O1R6tjjSUqNCSG8NnnpVv_g5FkCQhO5uRicTYxAb8,5050
-aos_prov/commands/command_vm_multi_node_manage.py,sha256=Ll4i74iVQoHEMfTeiMewM7rNkk76iRKWGgUWtoTMnlc,17537
-aos_prov/commands/download.py,sha256=cgxPjiHGdDY9v6TWvPT2cP9xVNDkoqrFQ2kwp3TI-z8,2300
-aos_prov/communication/__init__.py,sha256=g_G31XwUu8TLcWqYs29k7BIMKlsnQ_NS49zwy4o8ZPg,89
-aos_prov/communication/cloud/__init__.py,sha256=GG0w5d4OL0uOtGiHjbqIxaTR64BEYWYw1CULBI3cz-8,89
-aos_prov/communication/cloud/cloud_api.py,sha256=KSZZwdNK9yhrxGhoPUH0Q6Z4giKg28gUnMqSs-HLAms,7892
-aos_prov/communication/unit/__init__.py,sha256=g_G31XwUu8TLcWqYs29k7BIMKlsnQ_NS49zwy4o8ZPg,89
-aos_prov/communication/unit/v0/__init__.py,sha256=g_G31XwUu8TLcWqYs29k7BIMKlsnQ_NS49zwy4o8ZPg,89
-aos_prov/communication/unit/v1/__init__.py,sha256=g_G31XwUu8TLcWqYs29k7BIMKlsnQ_NS49zwy4o8ZPg,89
+aos_prov/__init__.py,sha256=lJlMhnUS4oONIEGs9ER8BXIp3GPfTurWn3Ko52JUvAk,93
+aos_prov/actions.py,sha256=BxAaq7kTggrFT7miDCR7CTST2bGphU_AA85VfP0KW60,3301
+aos_prov/main.py,sha256=cZko92jo4rwzyEFtl7mDrZABXQRkwrYmLx_wRKWYDJQ,9864
+aos_prov/commands/__init__.py,sha256=lJlMhnUS4oONIEGs9ER8BXIp3GPfTurWn3Ko52JUvAk,93
+aos_prov/commands/command_provision.py,sha256=05zJ4Fa1PtillRh20hXV3pc6441S8-aVSsmicbrmhpY,7181
+aos_prov/commands/command_vm.py,sha256=PL3qv5ggk-teSZIbWnvUZ2hPQL4KFkT7YGOp2vIZX-s,5021
+aos_prov/commands/command_vm_libvirt.py,sha256=OUrIgwOlg-AcR-6dkwX8dK1RtqiRK6PUikdOXflt91A,2406
+aos_prov/commands/command_vm_multi_node.py,sha256=qxNcrpdNThkGynC1-7D3XutY3L6R3QBzoXTx5iw8260,5627
+aos_prov/commands/command_vm_multi_node_manage.py,sha256=Dk95jHpAc4rs_NHjPHK8BLOdXNcXXgdYuNBO_k-YZTo,18100
+aos_prov/commands/download.py,sha256=NTQluPo9E7_5ybG4EtWEOUOxmmUkA5IbVSMq19JdmgI,2371
+aos_prov/commands/vbox_sdk.py,sha256=8nSYAcqwQDXhGOdDYhqINKNPWJsL_sdrPjZ1zO8UCYA,1721
+aos_prov/communication/__init__.py,sha256=XoyBkCyjJwW4582JvDMjfGckXOXALHe124ICNhhu4JQ,93
+aos_prov/communication/cloud/__init__.py,sha256=lJlMhnUS4oONIEGs9ER8BXIp3GPfTurWn3Ko52JUvAk,93
+aos_prov/communication/cloud/cloud_api.py,sha256=csPCnHfswjTBMJvM7NOMZAsgEcO5Ye8AyyDWPyTS3tM,8075
+aos_prov/communication/unit/__init__.py,sha256=XoyBkCyjJwW4582JvDMjfGckXOXALHe124ICNhhu4JQ,93
+aos_prov/communication/unit/v0/__init__.py,sha256=XoyBkCyjJwW4582JvDMjfGckXOXALHe124ICNhhu4JQ,93
+aos_prov/communication/unit/v0/unit_communacation.py,sha256=UQiVrAesx9DudZTk1cEP6ABxHD4hBsl5LzuAr3OmqLo,5403
+aos_prov/communication/unit/v0/unit_communication.py,sha256=glRiahy4o1mh8aIZ9vB1I43NrIBJyz9pqLKZzxtvv8c,5346
+aos_prov/communication/unit/v0/generated/__init__.py,sha256=XoyBkCyjJwW4582JvDMjfGckXOXALHe124ICNhhu4JQ,93
+aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2.py,sha256=Gqx7tDoWsZSuxbW0fypbAWahUzcHWumeFZZiyZmc9To,29503
+aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2_grpc.py,sha256=BjS_7qY0yPjiT0lL7wwsEs82tFDWBpeBrQYGSoGJ4IQ,20612
+aos_prov/communication/unit/v1/__init__.py,sha256=XoyBkCyjJwW4582JvDMjfGckXOXALHe124ICNhhu4JQ,93
+aos_prov/communication/unit/v1/unit_communacation_v1.py,sha256=YLlrJ6ntjHja4GBsWQHrWbwBEBniJygPjIeC0npjW2g,6942
+aos_prov/communication/unit/v1/unit_communication_v1.py,sha256=xsGWcpXqczs7e06ZQEhuUAfVkjvBVajesuqJKmneuEM,6528
+aos_prov/communication/unit/v1/generated/__init__.py,sha256=XoyBkCyjJwW4582JvDMjfGckXOXALHe124ICNhhu4JQ,93
+aos_prov/communication/unit/v1/generated/iamanagercommon_pb2.py,sha256=14W0zcUq2O_2fJK7W0LiGhYAMThduF0q6rGgM7Dd_J0,5568
+aos_prov/communication/unit/v1/generated/iamanagercommon_pb2_grpc.py,sha256=_bXoS025FcWrXR1E_3Mh4GHB1RMvgz8lIpit-Awnf-s,163
+aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2.py,sha256=qpB2-86Yn9avtG1H7Z-e5X8G2aehFSc3NIJECXcCxiM,31801
+aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2_grpc.py,sha256=URWN8YCm0W6sOVDZGCS-HyZ700S4cHEcJJBLE3gtC8w,20208
+aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2.py,sha256=MOsdukOrcgOI-Dgde8swlUCTTYzG2zJsfGmZiEUQz-g,9306
+aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2_grpc.py,sha256=OVb5eMqUlTmE2MVe6BTk9Qx8i-spafJjun4irYr1SrM,8101
 aos_prov/communication/unit/v2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aos_prov/communication/unit/v2/unit_communication_v2.py,sha256=oLADC7CpP4TE_DPuUlzK5SnNHJNg1VuDT6zbq5_1NJs,6965
+aos_prov/communication/unit/v2/unit_communacation_v2.py,sha256=bkL8neI0c5TOjP-0yqAWxUMhLkdIJO6OAoTNGL3ggNM,7346
+aos_prov/communication/unit/v2/unit_communication_v2.py,sha256=zJ0bzINcDVWwqZF0jMDHrh85yDqKzdpmHUqlQ9Hjldg,7139
 aos_prov/communication/unit/v2/generated/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py,sha256=YvHemzD0F2T4BA18FrKD_llZF2Pm4QL-r7bkIJvUX5M,5410
-aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py,sha256=yYvi-SGfANWQFkRnF7Wil1WIcLgAp8qTj4PC6mSLnwg,24479
-aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py,sha256=fFl4J6mMRcY5nfPo4Z28vUxS21tLSBj3pu53nnRTI1c,16471
-aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py,sha256=XunmdPpxiQzWkSVr5wjE9J-5-NGeD3iVKPGaCCH82oQ,17275
-aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py,sha256=pOlOIFoAjVExEkAL2k3sSIPeMR-Aw5nzYjf58kZx4I0,12921
-aos_prov/communication/unit/v3/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aos_prov/communication/unit/v3/unit_communication_v3.py,sha256=VcpCZt2z8pfzihNvq_85e-o6fKniv7y3p79kr-BdwsM,6757
-aos_prov/communication/unit/v3/generated/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aos_prov/communication/unit/v3/generated/iamanagercommon_pb2.py,sha256=rvHdMjDvJxN7c_9_Mwup-McyjLoBrEoav0JPlLGUPAw,5409
-aos_prov/communication/unit/v3/generated/iamanagercommon_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-aos_prov/communication/unit/v3/generated/iamanagerprotected_pb2.py,sha256=YNUZAHS-3Cu8mJQpw4-ATndo_ylsgdvexz4vQ8vUcLo,24470
-aos_prov/communication/unit/v3/generated/iamanagerprotected_pb2_grpc.py,sha256=UvtLozc2FFTFmKYOH4jvosBane_xLK67dsQVQv6glAI,16454
-aos_prov/communication/unit/v3/generated/iamanagerpublic_pb2.py,sha256=TFYsVt75KbuR6CNmLFBJb5soWGKZgJdczJxSonyHsSk,17266
-aos_prov/communication/unit/v3/generated/iamanagerpublic_pb2_grpc.py,sha256=ZTaB7o8hWDkOFHmkCygbi428cCLsplS4RBKDHJoPn84,12904
+aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py,sha256=3LP2EwlhrmHVruLZODbnmL4tDfQv26jXq742lyZpNyY,5570
+aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py,sha256=_bXoS025FcWrXR1E_3Mh4GHB1RMvgz8lIpit-Awnf-s,163
+aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py,sha256=mZvbwMZX9fxcf470LSVFhuWvNynkeCHwuwzeIKlrAjc,25112
+aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py,sha256=9aPASzChmdsPLDAnvXuN3tXHfzZR-HlxcpWs5LEv38E,16806
+aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py,sha256=rW9Fb5axuPNOMXQVF248UF8Yll9pi8MM0ovcnDcUS7g,17726
+aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py,sha256=aL5doTnhPGtUHivzx5iyR4pcOZa-djCsK8bqGzVeqUI,13190
 aos_prov/communication/unit/v4/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aos_prov/communication/unit/v4/unit_communication_v4.py,sha256=dvtFf4p5dZqg7AmTrqfMPxL2aNSe3lJyCxfhN_8dgEc,8695
+aos_prov/communication/unit/v4/unit_communication_v4.py,sha256=8Hdosjusz9WYUaVXGC7jZgp18cBPelfTuBdqvTl8Rug,8897
 aos_prov/communication/unit/v4/generated/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aos_prov/communication/unit/v4/generated/iamanager_pb2.py,sha256=ymskEIofG68AvhkwDGbvK2f_TykTUL6s-sCeCPMFJcE,18433
-aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py,sha256=eCSV3uoEEHd2L8IrU13EYXZKzWF6jPc-a1zERsk9efc,33413
-aos_prov/files/1rootCA.crt,sha256=ToJxPHzLkJQmYdXNPVJA3ACBf7uv0THJK8ypR18etws,2705
-aos_prov/utils/__init__.py,sha256=FXJpTks2FyzbRUI3vSk-bRK1EPpQfyc2mC1OCMmPnw4,748
-aos_prov/utils/common.py,sha256=vhh5xmCJ9NZg9WRDVMhufnOZmaxdO54A3QdiYTO04EU,1634
-aos_prov/utils/config.py,sha256=CZKUMn0n5J-rts2evDB46Kf3NNIefSi0hZQoLoF2CpA,2153
-aos_prov/utils/errors.py,sha256=EBxaDSqxPWLTJrd9rrwLoXf_Eqgfs5oIJ31390WFABY,645
-aos_prov/utils/unit_certificate.py,sha256=0XkWRReDsLAdlvzEHg1OA62oavDC77RwtkAufzXClgM,972
-aos_prov/utils/user_credentials.py,sha256=-28UNmE3Mi-P2eLqrTQbe5gTvXprI0NLgHBfvEEILcY,5977
+aos_prov/communication/unit/v4/generated/iamanager_pb2.py,sha256=RyP895KNz296C8xftpKEcyBEH-E02i19gh0ypLx8qb4,18732
+aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py,sha256=0BNJN1iWUB1ZBilmik-zAPLzt8QeTc9ekfJTAQrkoDA,34149
+aos_prov/files/1rootCA.crt,sha256=X3mH5kWiKpchVXfrW0HAhI94103mLhjftx2dR4KyWbw,2750
+aos_prov/files/vm.xml,sha256=67Z-mGXFGmiekJCfV1vzluEZWKKKeQXfcAmFn4DwKf8,2767
+aos_prov/utils/__init__.py,sha256=EfRSGsK_O0hF3vTrYEs5StBNfhuDk-RDquRYIm1aGBc,771
+aos_prov/utils/common.py,sha256=i2WbTkcAFs7-Uzm4Tae8pkvnbod4kvoqTf7buMP_ug4,1702
+aos_prov/utils/config.py,sha256=CKpw4sKF-LHf7v266xzt85PorGJQNgL1fxLx9zvup0E,2234
+aos_prov/utils/errors.py,sha256=7WT04FHtU7E4-k1LTohrAtyE5wgBgdg8dWfNIf-FTOU,681
+aos_prov/utils/unit_certificate.py,sha256=ET5BZLoNPO6VGV0K9l-GRqTtG5h6aDbNxU3e_OopGmI,1020
+aos_prov/utils/user_credentials.py,sha256=qLY4bYyADZ9fjjEOTRzaZzHy0Uq1fB83Jz-dt6XUpWI,6176
+aos_prov/utils/pem/__init__.py,sha256=SbPtCG7_-lKNjutiaSMxGRt4vWXAGlUi3zBaBe6YMT4,2096
+aos_prov/utils/pem/_core.py,sha256=QUsBxLOG4SlFzfcaum7Q896UED13uSCNPwG_ydhM_AE,1839
+aos_prov/utils/pem/_object_types.py,sha256=VilTmUKr-RoSFWEZJHCdr3H78Ul45TMs7HnIczx8dQ4,6807
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-test/utils/test_config.py,sha256=696gxCTKBDuXMe3aKd3ucGsx8qZItMGNlp53NgczEOI,642
-test/utils/test_unit_certificate.py,sha256=hh6fN3qCeZbizfgzF1V5DEYUSuCxzSNDq1qI7YrpZqs,632
-test/utils/test_user_credentials.py,sha256=CGjW9zhm3NxGP3JXTMI8p1gupqSWozbWHUCou7EUUw0,439
-tests/__init__.py,sha256=S3WC3mYsT7185m-P4yOMUsTVuJOwLR-Km7mJOSghjVI,89
-tests/fixtures.py,sha256=xz0eNBF-5xYzBOR-vCVMEkm73rLjPUzjTvuRwhXYC5U,4390
-tests/test_actions.py,sha256=2J1yUKtuuI7fomQpbgOEVizxqBMqTadoQPgapEZTeSM,3257
-tests/commands/__init__.py,sha256=S3WC3mYsT7185m-P4yOMUsTVuJOwLR-Km7mJOSghjVI,89
-tests/commands/test_command_provision.py,sha256=oBWIYWGCVJWDYbq3NKeHH0QFnFTIHFMS80Ffy5nS5dE,17566
-tests/commands/test_command_vm_multi_node_manage.py,sha256=mQ0XGaLrqj8Qyq-RT3wjyyXPsbuFnZo4k-sCyX1IS-4,13737
-tests/commands/test_download.py,sha256=C45iqXoS4RkxLPxCZvjtayDLsW0EA94aTKgKa85B-t4,3584
+test/utils/test_config.py,sha256=JuofpwzS7FGqWcfRHOaGSlrvqVYu9rS55K-yE5JhrNs,665
+test/utils/test_unit_certificate.py,sha256=ayJbD0Qrj1FICnDRjVPBpH0zMqLEMjqzR3ZNTxSAzHU,656
+test/utils/test_user_credentials.py,sha256=_g-oGXprFMiqRD9ZklnTiqxWsvsXtW0As5oJpWOqQW0,456
+tests/__init__.py,sha256=iyHD1Wa89dC3Nv7z_bBdqeChdkMpvsm-2F7FOActlBc,93
+tests/fixtures.py,sha256=ZsNX7TplK7_HUPaeZ-De7gFWeV2GYJ3iw5qxcjWolfE,4520
+tests/test_actions.py,sha256=Uqg2MBQtmiX5LL9gBa_Lx59Gw5e9QS33DnbZ_ohkNSo,3355
+tests/commands/__init__.py,sha256=iyHD1Wa89dC3Nv7z_bBdqeChdkMpvsm-2F7FOActlBc,93
+tests/commands/test_command_provision.py,sha256=hOoSNQoohL1cE4LOjuUkaSyPkzz2bgiXd72YAHKjyJw,17979
+tests/commands/test_command_vm_multi_node_manage.py,sha256=oqNGtb_pdyRXwZg9ioi2MCWi_QI1UDeNrIe92o5Rf8Q,14118
+tests/commands/test_download.py,sha256=zVgp2LgBnBMdvPZnDK0gBm_HFgcB4p4szjwmFI2285E,3666
 tests/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/utils/test_common.py,sha256=eCEAcYW3Q8Yl1LDFwi5ogswQ6aNPaKYHPQmr7bmN2S0,1798
-tests/utils/test_config.py,sha256=8xVNhCZhxrTC_Y1MC4Z0oleBQ81q5VT--eXacaOChUY,1120
-tests/utils/test_unit_certificate.py,sha256=3JjU9TOzcinAF6FL70jy6nnmahvb9QpCB9H5HpQ8_Ek,721
-tests/utils/test_user_credentials.py,sha256=jwy2c28wcuRuMxbe9hO65N6BJ4o8VMq7RyLVB2dM_C0,3693
-aos_prov-4.5.0b9.dist-info/METADATA,sha256=NpIosPfzFZjWiqvzps_KCsn46qfOOl4164iU_Jo-zjE,2549
-aos_prov-4.5.0b9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-aos_prov-4.5.0b9.dist-info/entry_points.txt,sha256=fkaEe75Sm0Z8TQtunDs5iah-ilcOouPDsCnNyQaZg18,48
-aos_prov-4.5.0b9.dist-info/top_level.txt,sha256=vaXqAwkIMSxecvTOPj_AlP4Rkw4ZQzstNWzXFpZgDBY,15
-aos_prov-4.5.0b9.dist-info/RECORD,,
+tests/utils/test_common.py,sha256=wjj8EAIYf-FkGPswWr6Z9EVhBEQs_o80-uatdoJKczg,1867
+tests/utils/test_config.py,sha256=idyyxXZCI9iLUJMoFOm7Y1mKBKAuaHwDIwbMsZtnTxE,1159
+tests/utils/test_unit_certificate.py,sha256=__luL2AQuGiQ2Mr0Jlvf3SQyXQUQcoo4NCl-FGUmLas,749
+tests/utils/test_user_credentials.py,sha256=pQYR6dqGPtEzRVF9QEVAcyZVZO8HeOklNwo_Xvf5BI0,3797
+aos_prov-4.6.0b1.dist-info/METADATA,sha256=XkVtoRWBNkvVqRvWL51aKvSnwOjuLxYeMNoVFPjE_7Q,2538
+aos_prov-4.6.0b1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+aos_prov-4.6.0b1.dist-info/entry_points.txt,sha256=pSYEWtSRNsmqfdoCn0tQJAqVxSOeLGpaSi6UPJv_kfA,49
+aos_prov-4.6.0b1.dist-info/top_level.txt,sha256=vaXqAwkIMSxecvTOPj_AlP4Rkw4ZQzstNWzXFpZgDBY,15
+aos_prov-4.6.0b1.dist-info/RECORD,,
```

