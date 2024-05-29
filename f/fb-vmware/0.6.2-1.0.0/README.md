# Comparing `tmp/fb_vmware-0.6.2.tar.gz` & `tmp/fb_vmware-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb_vmware-0.6.2.tar", last modified: Tue Oct 17 14:17:48 2023, max compression
+gzip compressed data, was "fb_vmware-1.0.0.tar", last modified: Wed May 29 07:34:34 2024, max compression
```

## Comparing `fb_vmware-0.6.2.tar` & `fb_vmware-1.0.0.tar`

### file list

```diff
@@ -1,74 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 14:17:48.072914 fb_vmware-0.6.2/
--rw-r--r--   0 root         (0) root         (0)     7652 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       52 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1396 2023-10-17 14:17:48.072914 fb_vmware-0.6.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       93 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 14:17:48.060914 fb_vmware-0.6.2/bin/
--rwxr-xr-x   0 root         (0) root         (0)     2012 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/bin/get-vsphere-host-list
--rwxr-xr-x   0 root         (0) root         (0)     1981 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/bin/get-vsphere-vm-info
--rwxr-xr-x   0 root         (0) root         (0)     1986 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/bin/get-vsphere-vm-list
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 14:17:48.056914 fb_vmware-0.6.2/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 14:17:48.064914 fb_vmware-0.6.2/lib/fb_vmware/
--rw-r--r--   0 root         (0) root         (0)     2146 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11253 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 14:17:48.068914 fb_vmware-0.6.2/lib/fb_vmware/app/
--rw-r--r--   0 root         (0) root         (0)     7891 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/app/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12757 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/app/get_host_list.py
--rw-r--r--   0 root         (0) root         (0)    10223 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/app/get_vm_info.py
--rw-r--r--   0 root         (0) root         (0)    17673 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/app/get_vm_list.py
--rw-r--r--   0 root         (0) root         (0)     8159 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/base.py
--rw-r--r--   0 root         (0) root         (0)    13594 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 14:17:48.068914 fb_vmware-0.6.2/lib/fb_vmware/config/
--rw-r--r--   0 root         (0) root         (0)    16498 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55811 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/connect.py
--rw-r--r--   0 root         (0) root         (0)    18764 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/controller.py
--rw-r--r--   0 root         (0) root         (0)    24206 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/datastore.py
--rw-r--r--   0 root         (0) root         (0)     8675 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/dc.py
--rw-r--r--   0 root         (0) root         (0)    20969 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/disk.py
--rw-r--r--   0 root         (0) root         (0)    17073 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/ds_cluster.py
--rw-r--r--   0 root         (0) root         (0)     9993 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/errors.py
--rw-r--r--   0 root         (0) root         (0)    25970 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/ether.py
--rw-r--r--   0 root         (0) root         (0)    32498 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/host.py
--rw-r--r--   0 root         (0) root         (0)    15962 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/host_port_group.py
--rw-r--r--   0 root         (0) root         (0)     5422 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/iface.py
--rw-r--r--   0 root         (0) root         (0)      474 2023-10-17 14:17:47.000000 fb_vmware-0.6.2/lib/fb_vmware/local_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 14:17:48.056914 fb_vmware-0.6.2/lib/fb_vmware/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 14:17:48.056914 fb_vmware-0.6.2/lib/fb_vmware/locale/de_DE/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 14:17:48.068914 fb_vmware-0.6.2/lib/fb_vmware/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    27481 2023-10-17 14:17:46.000000 fb_vmware-0.6.2/lib/fb_vmware/locale/de_DE/LC_MESSAGES/fb_vmware.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 14:17:48.056914 fb_vmware-0.6.2/lib/fb_vmware/locale/en_US/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 14:17:48.068914 fb_vmware-0.6.2/lib/fb_vmware/locale/en_US/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     4481 2023-10-17 14:17:46.000000 fb_vmware-0.6.2/lib/fb_vmware/locale/en_US/LC_MESSAGES/fb_vmware.mo
--rw-r--r--   0 root         (0) root         (0)    18889 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/network.py
--rw-r--r--   0 root         (0) root         (0)    10021 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/obj.py
--rw-r--r--   0 root         (0) root         (0)     3726 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/spinner.py
--rw-r--r--   0 root         (0) root         (0)    29777 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/vm.py
--rw-r--r--   0 root         (0) root         (0)     3161 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/lib/fb_vmware/xlate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 14:17:48.064914 fb_vmware-0.6.2/lib/fb_vmware.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1396 2023-10-17 14:17:48.000000 fb_vmware-0.6.2/lib/fb_vmware.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1528 2023-10-17 14:17:48.000000 fb_vmware-0.6.2/lib/fb_vmware.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 14:17:48.000000 fb_vmware-0.6.2/lib/fb_vmware.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-10-17 14:17:48.000000 fb_vmware-0.6.2/lib/fb_vmware.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-10-17 14:17:48.000000 fb_vmware-0.6.2/lib/fb_vmware.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1251 2023-10-17 14:17:48.076913 fb_vmware-0.6.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6975 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 14:17:48.072914 fb_vmware-0.6.2/test/
--rw-r--r--   0 root         (0) root         (0)     3583 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/general.py
--rwxr-xr-x   0 root         (0) root         (0)     9433 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_00-errors.py
--rwxr-xr-x   0 root         (0) root         (0)     4172 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_10-base.py
--rwxr-xr-x   0 root         (0) root         (0)     2819 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_20-obj.py
--rwxr-xr-x   0 root         (0) root         (0)     4644 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_31_about_info.py
--rwxr-xr-x   0 root         (0) root         (0)     5139 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_32_cluster.py
--rwxr-xr-x   0 root         (0) root         (0)     4866 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_33_dc.py
--rwxr-xr-x   0 root         (0) root         (0)     2749 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_34_disk.py
--rwxr-xr-x   0 root         (0) root         (0)     3297 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_35_datastore.py
--rwxr-xr-x   0 root         (0) root         (0)     3372 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_36_ds_cluster.py
--rwxr-xr-x   0 root         (0) root         (0)     2767 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_37_ether.py
--rwxr-xr-x   0 root         (0) root         (0)     2817 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_38_iface.py
--rwxr-xr-x   0 root         (0) root         (0)     4523 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_39_network.py
--rwxr-xr-x   0 root         (0) root         (0)     2847 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_40_controller.py
--rwxr-xr-x   0 root         (0) root         (0)     2866 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_41_host_port_group.py
--rwxr-xr-x   0 root         (0) root         (0)     3097 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_50_host.py
--rwxr-xr-x   0 root         (0) root         (0)     3039 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_55_vm.py
--rwxr-xr-x   0 root         (0) root         (0)     3539 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_60_config.py
--rwxr-xr-x   0 root         (0) root         (0)     3211 2023-10-17 14:17:18.000000 fb_vmware-0.6.2/test/test_70_connect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.662663 fb_vmware-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)     7652 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1497 2024-05-29 07:34:34.662663 fb_vmware-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       93 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.650663 fb_vmware-1.0.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     2012 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/bin/get-vsphere-host-list
+-rwxr-xr-x   0 root         (0) root         (0)     1981 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/bin/get-vsphere-vm-info
+-rwxr-xr-x   0 root         (0) root         (0)     1986 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/bin/get-vsphere-vm-list
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.650663 fb_vmware-1.0.0/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.658663 fb_vmware-1.0.0/lib/fb_vmware/
+-rw-r--r--   0 root         (0) root         (0)     2146 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11253 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.658663 fb_vmware-1.0.0/lib/fb_vmware/app/
+-rw-r--r--   0 root         (0) root         (0)     7891 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12757 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/app/get_host_list.py
+-rw-r--r--   0 root         (0) root         (0)    10223 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/app/get_vm_info.py
+-rw-r--r--   0 root         (0) root         (0)    17673 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/app/get_vm_list.py
+-rw-r--r--   0 root         (0) root         (0)     8159 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/base.py
+-rw-r--r--   0 root         (0) root         (0)    13594 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.658663 fb_vmware-1.0.0/lib/fb_vmware/config/
+-rw-r--r--   0 root         (0) root         (0)    16498 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55811 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/connect.py
+-rw-r--r--   0 root         (0) root         (0)    18764 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/controller.py
+-rw-r--r--   0 root         (0) root         (0)    24206 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/datastore.py
+-rw-r--r--   0 root         (0) root         (0)     8675 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/dc.py
+-rw-r--r--   0 root         (0) root         (0)    20969 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/disk.py
+-rw-r--r--   0 root         (0) root         (0)    17073 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/ds_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     9993 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/errors.py
+-rw-r--r--   0 root         (0) root         (0)    25970 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/ether.py
+-rw-r--r--   0 root         (0) root         (0)    32498 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/host.py
+-rw-r--r--   0 root         (0) root         (0)    15962 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/host_port_group.py
+-rw-r--r--   0 root         (0) root         (0)     5422 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/iface.py
+-rw-r--r--   0 root         (0) root         (0)      474 2024-05-29 07:34:34.000000 fb_vmware-1.0.0/lib/fb_vmware/local_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.650663 fb_vmware-1.0.0/lib/fb_vmware/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.650663 fb_vmware-1.0.0/lib/fb_vmware/locale/de_DE/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.658663 fb_vmware-1.0.0/lib/fb_vmware/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    26174 2024-05-29 07:34:34.000000 fb_vmware-1.0.0/lib/fb_vmware/locale/de_DE/LC_MESSAGES/fb_vmware.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.650663 fb_vmware-1.0.0/lib/fb_vmware/locale/en_US/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.658663 fb_vmware-1.0.0/lib/fb_vmware/locale/en_US/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     5340 2024-05-29 07:34:34.000000 fb_vmware-1.0.0/lib/fb_vmware/locale/en_US/LC_MESSAGES/fb_vmware.mo
+-rw-r--r--   0 root         (0) root         (0)    18889 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/network.py
+-rw-r--r--   0 root         (0) root         (0)    10021 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/obj.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/spinner.py
+-rw-r--r--   0 root         (0) root         (0)    29777 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/vm.py
+-rw-r--r--   0 root         (0) root         (0)     3238 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/lib/fb_vmware/xlate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.662663 fb_vmware-1.0.0/lib/fb_vmware.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1497 2024-05-29 07:34:34.000000 fb_vmware-1.0.0/lib/fb_vmware.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-05-29 07:34:34.000000 fb_vmware-1.0.0/lib/fb_vmware.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 07:34:34.000000 fb_vmware-1.0.0/lib/fb_vmware.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-29 07:34:34.000000 fb_vmware-1.0.0/lib/fb_vmware.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-29 07:34:34.000000 fb_vmware-1.0.0/lib/fb_vmware.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.650663 fb_vmware-1.0.0/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.650663 fb_vmware-1.0.0/locale/de_DE/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.658663 fb_vmware-1.0.0/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    26174 2024-05-29 07:34:34.000000 fb_vmware-1.0.0/locale/de_DE/LC_MESSAGES/fb_vmware.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.650663 fb_vmware-1.0.0/locale/en_US/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.658663 fb_vmware-1.0.0/locale/en_US/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     5340 2024-05-29 07:34:34.000000 fb_vmware-1.0.0/locale/en_US/LC_MESSAGES/fb_vmware.mo
+-rw-r--r--   0 root         (0) root         (0)     1813 2024-05-29 07:34:34.666664 fb_vmware-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8949 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 07:34:34.662663 fb_vmware-1.0.0/test/
+-rw-r--r--   0 root         (0) root         (0)     3583 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/general.py
+-rwxr-xr-x   0 root         (0) root         (0)     9433 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_00-errors.py
+-rwxr-xr-x   0 root         (0) root         (0)     4172 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_10-base.py
+-rwxr-xr-x   0 root         (0) root         (0)     2819 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_20-obj.py
+-rwxr-xr-x   0 root         (0) root         (0)     4644 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_31_about_info.py
+-rwxr-xr-x   0 root         (0) root         (0)     5139 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_32_cluster.py
+-rwxr-xr-x   0 root         (0) root         (0)     4866 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_33_dc.py
+-rwxr-xr-x   0 root         (0) root         (0)     2749 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_34_disk.py
+-rwxr-xr-x   0 root         (0) root         (0)     3297 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_35_datastore.py
+-rwxr-xr-x   0 root         (0) root         (0)     3372 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_36_ds_cluster.py
+-rwxr-xr-x   0 root         (0) root         (0)     2767 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_37_ether.py
+-rwxr-xr-x   0 root         (0) root         (0)     2817 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_38_iface.py
+-rwxr-xr-x   0 root         (0) root         (0)     4523 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_39_network.py
+-rwxr-xr-x   0 root         (0) root         (0)     2847 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_40_controller.py
+-rwxr-xr-x   0 root         (0) root         (0)     2866 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_41_host_port_group.py
+-rwxr-xr-x   0 root         (0) root         (0)     3097 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_50_host.py
+-rwxr-xr-x   0 root         (0) root         (0)     3039 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_55_vm.py
+-rwxr-xr-x   0 root         (0) root         (0)     3539 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_60_config.py
+-rwxr-xr-x   0 root         (0) root         (0)     3211 2024-05-29 07:34:08.000000 fb_vmware-1.0.0/test/test_70_connect.py
```

### Comparing `fb_vmware-0.6.2/LICENSE` & `fb_vmware-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.6.2/PKG-INFO` & `fb_vmware-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: fb_vmware
-Version: 0.6.2
+Version: 1.0.0
 Summary: A wrapper module around the pyvmomi module to simplify work and handling.
 Home-page: https://github.com/fbrehm/fb-vmware
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires: fb_tools
 Requires: argparse
 Requires: six
 Requires: pyvmomi
 Requires: fb_logging
 Requires: packaging
```

### Comparing `fb_vmware-0.6.2/bin/get-vsphere-host-list` & `fb_vmware-1.0.0/bin/get-vsphere-host-list`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @summary: An application to print a list of all physical hosts in a VMWare VSphere.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 
 from __future__ import print_function
 
 import locale
 import os
 import sys
@@ -48,15 +48,15 @@
 
 from fb_vmware.app.get_host_list import GetHostsListApplication
 from fb_vmware.xlate import XLATOR
 
 _ = XLATOR.gettext
 
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
-__copyright__ = '(C) 2023 by Frank Brehm, Berlin'
+__copyright__ = '(C) 2024 by Frank Brehm, Berlin'
 
 appname = os.path.basename(sys.argv[0])
 
 locale.setlocale(locale.LC_ALL, '')
 
 app = GetHostsListApplication(appname=appname, base_dir=base_dir)
 app.initialized = True
```

### Comparing `fb_vmware-0.6.2/bin/get-vsphere-vm-info` & `fb_vmware-1.0.0/bin/get-vsphere-vm-info`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @summary: Print information about a particular VM in VMWare VSphere.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 
 from __future__ import print_function
 
 import locale
 import os
 import sys
@@ -48,15 +48,15 @@
 
 from fb_vmware.app.get_vm_info import GetVmApplication
 from fb_vmware.xlate import XLATOR
 
 _ = XLATOR.gettext
 
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
-__copyright__ = '(C) 2023 by Frank Brehm, Berlin'
+__copyright__ = '(C) 2024 by Frank Brehm, Berlin'
 
 appname = os.path.basename(sys.argv[0])
 
 locale.setlocale(locale.LC_ALL, '')
 
 app = GetVmApplication(appname=appname, base_dir=base_dir)
 app.initialized = True
```

### Comparing `fb_vmware-0.6.2/bin/get-vsphere-vm-list` & `fb_vmware-1.0.0/bin/get-vsphere-vm-list`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @summary: Print a list of all virtual machines in VMWare VSphere.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 
 from __future__ import print_function
 
 import locale
 import os
 import sys
@@ -48,15 +48,15 @@
 
 from fb_vmware.app.get_vm_list import GetVmListApplication
 from fb_vmware.xlate import XLATOR
 
 _ = XLATOR.gettext
 
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
-__copyright__ = '(C) 2023 by Frank Brehm, Berlin'
+__copyright__ = '(C) 2024 by Frank Brehm, Berlin'
 
 appname = os.path.basename(sys.argv[0])
 
 locale.setlocale(locale.LC_ALL, '')
 
 app = GetVmListApplication(appname=appname, base_dir=base_dir)
 app.initialized = True
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/__init__.py` & `fb_vmware-1.0.0/lib/fb_vmware/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a base VSphere handler object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 # flake8: noqa
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 
@@ -48,15 +48,15 @@
 from .obj import DEFAULT_OBJ_STATUS
 from .obj import VsphereObject
 from .vm import VsphereVm
 from .vm import VsphereVmList
 from .xlate import XLATOR
 
 
-__version__ = '0.6.2'
+__version__ = '1.0.0'
 
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/about.py` & `fb_vmware-1.0.0/lib/fb_vmware/about.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for capsulating a VSphere about info object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 import uuid
 
@@ -20,15 +20,15 @@
 from fb_tools.xlate import format_list
 
 from pyVmomi import vim
 
 # Own modules
 from .xlate import XLATOR
 
-__version__ = '0.3.4'
+__version__ = '1.0.0'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereAboutInfo(FbBaseObject):
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/app/__init__.py` & `fb_vmware-1.0.0/lib/fb_vmware/app/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: A base module for all VMWare/VSPhere application classes.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
 import copy
 import getpass
 import logging
@@ -25,15 +25,15 @@
 # Own modules
 from .. import __version__ as GLOBAL_VERSION
 from ..config import VmwareConfiguration
 from ..connect import VsphereConnection
 from ..errors import VSphereExpectedError
 from ..xlate import XLATOR
 
-__version__ = '0.2.2'
+__version__ = '1.0.0'
 LOG = logging.getLogger(__name__)
 TZ = pytz.timezone('Europe/Berlin')
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/app/get_host_list.py` & `fb_vmware-1.0.0/lib/fb_vmware/app/get_host_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for the application object of the get-vsphere-host-list application.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
 import logging
 import re
 import sys
@@ -22,15 +22,15 @@
 
 # Own modules
 from . import BaseVmwareApplication, VmwareAppError
 from .. import __version__ as GLOBAL_VERSION
 from ..spinner import Spinner
 from ..xlate import XLATOR
 
-__version__ = '0.3.3'
+__version__ = '1.0.0'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 
 # =============================================================================
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/app/get_vm_info.py` & `fb_vmware-1.0.0/lib/fb_vmware/app/get_vm_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for the application object of the get-vsphere-vm-info application.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
 import logging
 from operator import attrgetter
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/app/get_vm_list.py` & `fb_vmware-1.0.0/lib/fb_vmware/app/get_vm_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for the application object of the get-vsphere-vm-list application.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
 import logging
 import re
 import sys
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/base.py` & `fb_vmware-1.0.0/lib/fb_vmware/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a base VSphere handler object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 import ssl
 from abc import ABCMeta, abstractmethod
@@ -31,15 +31,15 @@
 from .config import DEFAULT_VSPHERE_CLUSTER
 from .config import VSPhereConfigInfo
 from .errors import BaseVSphereHandlerError
 from .errors import VSphereCannotConnectError
 from .errors import VSphereVimFault
 from .xlate import XLATOR
 
-__version__ = '0.2.5'
+__version__ = '1.0.0'
 
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 DEFAULT_TZ_NAME = 'Europe/Berlin'
 DEFAULT_MAX_SEARCH_DEPTH = 10
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/cluster.py` & `fb_vmware-1.0.0/lib/fb_vmware/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for capsulating a VSphere calculation cluster object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 
 # Third party modules
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/config/__init__.py` & `fb_vmware-1.0.0/lib/fb_vmware/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: A module for providing a configuration for VSPhere.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard module
 import copy
 import logging
 
@@ -25,15 +25,15 @@
 from fb_tools.obj import FbGenericBaseObject
 
 # Own modules
 from ..errors import WrongPortTypeError
 from ..errors import WrongPortValueError
 from ..xlate import XLATOR
 
-__version__ = '0.5.6'
+__version__ = '1.0.0'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 DEFAULT_CONFIG_DIR = 'pixelpark'
 
 DEFAULT_VSPHERE_PORT = 443
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/connect.py` & `fb_vmware-1.0.0/lib/fb_vmware/connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a VSphere connection object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import datetime
 import logging
 import re
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/controller.py` & `fb_vmware-1.0.0/lib/fb_vmware/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a VSphere disk controller object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import copy
 import logging
 try:
@@ -23,15 +23,15 @@
 from fb_tools.xlate import format_list
 
 from pyVmomi import vim
 
 # Own modules
 from .xlate import XLATOR
 
-__version__ = '0.3.2'
+__version__ = '1.0.0'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereDiskController(FbBaseObject):
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/datastore.py` & `fb_vmware-1.0.0/lib/fb_vmware/datastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a VSphere datastore object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 import random
 import re
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/dc.py` & `fb_vmware-1.0.0/lib/fb_vmware/dc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for capsulating a VSphere datacenter object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 
 # Third party modules
@@ -19,15 +19,15 @@
 from pyVmomi import vim
 
 # Own modules
 from .obj import DEFAULT_OBJ_STATUS
 from .obj import VsphereObject
 from .xlate import XLATOR
 
-__version__ = '0.4.1'
+__version__ = '1.0.0'
 LOG = logging.getLogger(__name__)
 
 DEFAULT_HOST_FOLDER = 'host'
 DEFAULT_VM_FOLDER = 'vm'
 DEFAULT_DS_FOLDER = 'datastore'
 DEFAULT_NETWORK_FOLDER = 'network'
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/disk.py` & `fb_vmware-1.0.0/lib/fb_vmware/disk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: Mdule for capsulating a VSphere disk object, which can be assigned to a VM.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 import re
 import uuid
@@ -24,15 +24,15 @@
 from fb_tools.xlate import format_list
 
 from pyVmomi import vim
 
 # Own modules
 from .xlate import XLATOR
 
-__version__ = '0.4.2'
+__version__ = '1.0.0'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereDisk(FbBaseObject):
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/ds_cluster.py` & `fb_vmware-1.0.0/lib/fb_vmware/ds_cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a VSphere datastore cluster object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 try:
     from collections.abc import MutableMapping
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/errors.py` & `fb_vmware-1.0.0/lib/fb_vmware/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for special error classes on VSphere API operations.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 
 # Third party modules
 
 from fb_tools.errors import FbHandlerError
 
 # Own modules
 from .xlate import XLATOR
 
-__version__ = '0.3.4'
+__version__ = '1.0.0'
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class FbVMWareError(FbHandlerError):
     """Base class for all exception belonging to VSphere/VMWare."""
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/ether.py` & `fb_vmware-1.0.0/lib/fb_vmware/ether.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a VSphere ethernet card object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import copy
 import logging
 try:
@@ -23,15 +23,15 @@
 from fb_tools.xlate import format_list
 
 from pyVmomi import vim
 
 # Own modules
 from .xlate import XLATOR
 
-__version__ = '0.3.3'
+__version__ = '1.0.0'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereEthernetcard(FbBaseObject):
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/host.py` & `fb_vmware-1.0.0/lib/fb_vmware/host.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for capsulating a VSphere host system object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import copy
 import datetime
 import ipaddress
@@ -31,15 +31,15 @@
 from .about import VsphereAboutInfo
 from .errors import VSphereHandlerError
 from .host_port_group import VsphereHostPortgroup, VsphereHostPortgroupList
 from .obj import DEFAULT_OBJ_STATUS, OBJ_STATUS_GREEN
 from .obj import VsphereObject
 from .xlate import XLATOR
 
-__version__ = '0.7.4'
+__version__ = '1.0.0'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereHostBiosInfo(FbBaseObject):
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/host_port_group.py` & `fb_vmware-1.0.0/lib/fb_vmware/host_port_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a VSphere host portgroup object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import copy
 import logging
 try:
@@ -24,15 +24,15 @@
 from fb_tools.xlate import format_list
 
 from pyVmomi import vim
 
 # Own modules
 from .xlate import XLATOR
 
-__version__ = '0.2.4'
+__version__ = '1.0.0'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereHostPortgroup(FbBaseObject):
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/iface.py` & `fb_vmware-1.0.0/lib/fb_vmware/iface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a VSphere object for a network interface of a VM.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 
 # Third party modules
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/locale/de_DE/LC_MESSAGES/fb_vmware.mo` & `fb_vmware-1.0.0/lib/fb_vmware/locale/de_DE/LC_MESSAGES/fb_vmware.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: fb_vmware 0.5.7\n"
 "Report-Msgid-Bugs-To: frank@brehm-online.com\n"
+"POT-Creation-Date: 2023-07-13 17:15+0200\n"
 "PO-Revision-Date: 2023-07-13 17:20+0200\n"
 "Last-Translator: Frank Brehm <frank@brehm-online.com>\n"
 "Language: de_DE\n"
 "Language-Team: Frank Brehm <frank@brehm-online.com>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid ""
 "A regular expression to filter the output list of VMs by the VMWare hardware "
 "configuration version (e.g. '{}')."
 msgstr ""
 "Ein regulärer Ausdruck, um die Ausgabeliste der VMs nach ihrer VMWare-"
 "Hardwarekonfigurationsversion zu filtern (z.Bsp. '{}')."
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/network.py` & `fb_vmware-1.0.0/lib/fb_vmware/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a VSphere network object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import functools
 import ipaddress
 import logging
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/obj.py` & `fb_vmware-1.0.0/lib/fb_vmware/obj.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a base VSphere class.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import copy
 import logging
 import re
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/spinner.py` & `fb_vmware-1.0.0/lib/fb_vmware/spinner.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                 from fb_vmware.spinner import Spinner
 
                 with Spinner("just waiting a bit.. "):
                     time.sleep(3)
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 
 import itertools
 import sys
 import threading
 import time
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/vm.py` & `fb_vmware-1.0.0/lib/fb_vmware/vm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @summary: The module for a VSphere virtual machine or template object.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import copy
 import logging
 import re
@@ -32,15 +32,15 @@
 from .errors import VSphereHandlerError
 from .ether import VsphereEthernetcard, VsphereEthernetcardList
 from .obj import DEFAULT_OBJ_STATUS
 from .obj import OBJ_STATUS_GREEN
 from .obj import VsphereObject
 from .xlate import XLATOR
 
-__version__ = '0.6.4'
+__version__ = '1.0.0'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereVm(VsphereObject):
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware/xlate.py` & `fb_vmware-1.0.0/lib/fb_vmware/xlate.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @summary: The module for i18n.
 
           It provides a translation object, usable from all other
           modules in this package.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2023 by Frank Brehm, Berlin
+@copyright: © 2024 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
 import copy
 import gettext
 import logging
@@ -31,32 +31,36 @@
 except ImportError:
     from distutils.version import LooseVersion as Version
 
 DOMAIN = 'fb_vmware'
 
 LOG = logging.getLogger(__name__)
 
-__version__ = '0.1.4'
+__version__ = '1.0.1'
 
 __me__ = Path(__file__).resolve()
 __module_dir__ = __me__.parent
 __lib_dir__ = __module_dir__.parent
 __base_dir__ = __lib_dir__.parent
 LOCALE_DIR = __base_dir__.joinpath('locale')
 if not LOCALE_DIR.is_dir():
     LOCALE_DIR = __module_dir__.joinpath('locale')
     if not LOCALE_DIR.is_dir():
         LOCALE_DIR = None
 
+USED_LOCALE_DIR = None
+if LOCALE_DIR:
+    USED_LOCALE_DIR = str(LOCALE_DIR)
+
 DEFAULT_LOCALE_DEF = 'en_US'
 DEFAULT_LOCALE = babel.core.default_locale()
 if not DEFAULT_LOCALE:
     DEFAULT_LOCALE = DEFAULT_LOCALE_DEF
 
-__mo_file__ = gettext.find(DOMAIN, str(LOCALE_DIR))
+__mo_file__ = gettext.find(DOMAIN, USED_LOCALE_DIR)
 if __mo_file__:
     try:
         with open(__mo_file__, 'rb') as F:
             XLATOR = Translations(F, DOMAIN)
     except IOError:
         XLATOR = gettext.NullTranslations()
 else:
@@ -98,15 +102,15 @@
 # =============================================================================
 
 if __name__ == '__main__':
 
     out_list = []
     out_list.append([_('Module directory:'), str(__module_dir__)])
     out_list.append([_('Base directory:'), str(__base_dir__)])
-    out_list.append([_('Locale directory:'), str(LOCALE_DIR)])
+    out_list.append([_('Locale directory:'), USED_LOCALE_DIR])
     out_list.append([_('Locale domain:'), DOMAIN])
     out_list.append([_('Found .mo-file:'), __mo_file__])
 
     max_len = 1
     for pair in out_list:
         if len(pair[0]) > max_len:
             max_len = len(pair[0])
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware.egg-info/PKG-INFO` & `fb_vmware-1.0.0/lib/fb_vmware.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
-Name: fb-vmware
-Version: 0.6.2
+Name: fb_vmware
+Version: 1.0.0
 Summary: A wrapper module around the pyvmomi module to simplify work and handling.
 Home-page: https://github.com/fbrehm/fb-vmware
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires: fb_tools
 Requires: argparse
 Requires: six
 Requires: pyvmomi
 Requires: fb_logging
 Requires: packaging
```

### Comparing `fb_vmware-0.6.2/lib/fb_vmware.egg-info/SOURCES.txt` & `fb_vmware-1.0.0/lib/fb_vmware.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 lib/fb_vmware/app/__init__.py
 lib/fb_vmware/app/get_host_list.py
 lib/fb_vmware/app/get_vm_info.py
 lib/fb_vmware/app/get_vm_list.py
 lib/fb_vmware/config/__init__.py
 lib/fb_vmware/locale/de_DE/LC_MESSAGES/fb_vmware.mo
 lib/fb_vmware/locale/en_US/LC_MESSAGES/fb_vmware.mo
+locale/de_DE/LC_MESSAGES/fb_vmware.mo
+locale/en_US/LC_MESSAGES/fb_vmware.mo
 test/general.py
 test/test_00-errors.py
 test/test_10-base.py
 test/test_20-obj.py
 test/test_31_about_info.py
 test/test_32_cluster.py
 test/test_33_dc.py
```

### Comparing `fb_vmware-0.6.2/setup.py` & `fb_vmware-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,41 +3,46 @@
 
 """
 @summary: A wrapper module around the pyvmomi module to simplify work and handling.
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
 @license: LGPL3+
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 """
 from __future__ import print_function
 
 import datetime
 import glob
 import os
-import pathlib
 import pprint
 import re
 import subprocess
 import sys
 import textwrap
+from pathlib import Path
 
 # own modules:
 __base_dir__ = os.path.abspath(os.path.dirname(__file__))
 __bin_dir__ = os.path.join(__base_dir__, 'bin')
 __lib_dir__ = os.path.join(__base_dir__, 'lib')
 __module_dir__ = os.path.join(__lib_dir__, 'fb_vmware')
 __init_py__ = os.path.join(__module_dir__, '__init__.py')
+__local_usr_dir__ = Path(__base_dir__) / 'usr'
+__share_dir__ = Path(sys.base_prefix) / 'share'
+__locale_dir__ = __share_dir__ / 'locale'
 
 PATHS = {
     '__base_dir__': __base_dir__,
     '__bin_dir__': __bin_dir__,
     '__lib_dir__': __lib_dir__,
     '__module_dir__': __module_dir__,
     '__init_py__': __init_py__,
+    '__share_dir__': __share_dir__,
+    '__locale_dir__': __locale_dir__,
 }
 
 # -----------------------------------
 def pp(obj):
     """Human friendly output of data structures."""
     pprinter = pprint.PrettyPrinter(indent=4)
     return pprinter.pformat(obj)
@@ -45,30 +50,34 @@
 # print("Paths:\n{}".format(pp(PATHS)))
 
 
 if os.path.exists(__module_dir__) and os.path.isfile(__init_py__):
     sys.path.insert(0, os.path.abspath(__lib_dir__))
 
 # Third party modules
+from babel.messages import frontend as babel
+
+# Third party modules
 import fb_vmware
 
 from setuptools import setup
+from setuptools.command.sdist import sdist
 
 # from fb_tools.common import pp
 
 ENCODING = 'utf-8'
 
 __packet_version__ = fb_vmware.__version__
 
 __packet_name__ = 'fb_vmware'
 __debian_pkg_name__ = 'fb-vmware'
 
 __author__ = 'Frank Brehm'
 __contact__ = 'frank@brehm-online.com'
-__copyright__ = '(C) 2022 Frank Brehm, Berlin'
+__copyright__ = '(C) 2024 Frank Brehm, Berlin'
 __license__ = 'LGPL3+'
 __url__ = 'https://github.com/fbrehm/fb-vmware'
 
 
 __open_args__ = {}
 if sys.version_info[0] < 3:
     __open_args__ = {'encoding': ENCODING, 'errors': 'surrogateescape'}
@@ -221,39 +230,90 @@
 
     # print("Found scripts: {}\n".format(pp(__scripts__)))
 
 
 get_scripts()
 
 # -----------------------------------
-MO_FILES = 'locale/*/LC_MESSAGES/*.mo'
+__data_files__ = []
+
+re_usr = re.compile(r'^usr/')
+if __local_usr_dir__.is_dir():
+    usr_files = {}
+    for f in __local_usr_dir__.glob('**/*'):
+        if f.is_file():
+            relpath = Path(os.path.relpath(str(f), __base_dir__))
+            reldir = re_usr.sub('', str(relpath.parent))
+            if reldir not in usr_files:
+                usr_files[reldir] = []
+            usr_files[reldir].append(str(relpath))
+    for udir in usr_files.keys():
+        __data_files__.append((udir, usr_files[udir]))
+
+# -----------------------------------
 PO_FILES = 'locale/*/LC_MESSAGES/*.po'
+__package_data__ = {}
 
 def create_mo_files():
     """Compile the translation files."""
     mo_files = []
     for po_path in glob.glob(PO_FILES):
-        mo = pathlib.Path(po_path.replace('.po', '.mo'))
+        mo = Path(po_path.replace('.po', '.mo'))
         if not mo.exists():
             subprocess.call(['msgfmt', '-o', str(mo), po_path])
-        mo_files.append(str(mo))
+        mo_files.append(mo)
 
     # print("Found mo files: {}\n".format(pp(mo_files)))
     return mo_files
 
 
+__pkg_mo_paths__ = create_mo_files()
+__pkg_mo_files__ = []
+for mo_file in __pkg_mo_paths__:
+    __pkg_mo_files__.append(str(mo_file))
+
+__package_data__[''] = __pkg_mo_files__
+# print("Package_data:\n" + pp(__package_data__) + "\n")
+
+
+for mo_file in __pkg_mo_paths__:
+    ltype = mo_file.parent.name
+    lname = mo_file.parent.parent.name
+    ldir = __locale_dir__ / lname / ltype
+    mo_file_rel = str(mo_file).lstrip('/')
+    __data_files__.append((str(ldir), [mo_file_rel]))
+
+# print("Found data files:\n" + pp(__data_files__) + "\n")
+
+# -----------------------------------
+class Sdist(sdist):
+    """Custom ``sdist`` command to ensure that mo files are always created."""
+
+    def run(self):
+        """Compile the l18n catalog."""
+        self.run_command('compile_catalog')
+        # sdist is an old style class so super cannot be used.
+        sdist.run(self)
+
+
 # -----------------------------------
 setup(
     version=__packet_version__,
-    long_description=read('README.md'),
+    long_description=read(__readme_file__),
     scripts=__scripts__,
     requires=__requirements__,
     package_dir={'': 'lib'},
-    package_data={
-        '': create_mo_files(),
+    package_data=__package_data__,
+    data_files=__data_files__,
+    cmdclass={
+        'compile_catalog': babel.compile_catalog,
+        'extract_messages': babel.extract_messages,
+        'init_catalog': babel.init_catalog,
+        'update_catalog': babel.update_catalog,
+        'sdist': Sdist,
     },
 )
 
 
 # =======================================================================
 
 # vim: fileencoding=utf-8 filetype=python ts=4 expandtab
```

### Comparing `fb_vmware-0.6.2/test/general.py` & `fb_vmware-1.0.0/test/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: general used functions an objects used for unit tests on
           the VMWare/VSphere python modules
 """
 
 import os
 import sys
```

### Comparing `fb_vmware-0.6.2/test/test_00-errors.py` & `fb_vmware-1.0.0/test/test_00-errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on error (exception) classes
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_10-base.py` & `fb_vmware-1.0.0/test/test_10-base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.base
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_20-obj.py` & `fb_vmware-1.0.0/test/test_20-obj.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.obj
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_31_about_info.py` & `fb_vmware-1.0.0/test/test_31_about_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.about
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_32_cluster.py` & `fb_vmware-1.0.0/test/test_32_cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.cluster
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_33_dc.py` & `fb_vmware-1.0.0/test/test_33_dc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.dc
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_34_disk.py` & `fb_vmware-1.0.0/test/test_34_disk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.disk
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_35_datastore.py` & `fb_vmware-1.0.0/test/test_35_datastore.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.datastore
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_36_ds_cluster.py` & `fb_vmware-1.0.0/test/test_36_ds_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.ds_cluster
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_37_ether.py` & `fb_vmware-1.0.0/test/test_37_ether.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.ether
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_38_iface.py` & `fb_vmware-1.0.0/test/test_38_iface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.iface
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_39_network.py` & `fb_vmware-1.0.0/test/test_39_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.network
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_40_controller.py` & `fb_vmware-1.0.0/test/test_40_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.controller
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_41_host_port_group.py` & `fb_vmware-1.0.0/test/test_41_host_port_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.host_port_group
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_50_host.py` & `fb_vmware-1.0.0/test/test_50_host.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.host
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_55_vm.py` & `fb_vmware-1.0.0/test/test_55_vm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.vm
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_60_config.py` & `fb_vmware-1.0.0/test/test_60_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.config
 '''
 
 import os
 import sys
 import logging
```

### Comparing `fb_vmware-0.6.2/test/test_70_connect.py` & `fb_vmware-1.0.0/test/test_70_connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
+@copyright: © 2024 Frank Brehm, Berlin
 @license: GPL3
 @summary: test script (and module) for unit tests on module fb_vmware.connect
 '''
 
 import os
 import sys
 import logging
```

