# Comparing `tmp/netbox_nas-1.0.2.tar.gz` & `tmp/netbox_nas-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_nas-1.0.2.tar", last modified: Wed May 22 15:53:40 2024, max compression
+gzip compressed data, was "netbox_nas-1.0.3.tar", last modified: Wed May 29 13:24:01 2024, max compression
```

## Comparing `netbox_nas-1.0.2.tar` & `netbox_nas-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:40.446907 netbox_nas-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-22 15:53:40.446907 netbox_nas-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:40.442907 netbox_nas-1.0.2/netbox_nas/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:40.442907 netbox_nas-1.0.2/netbox_nas/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:40.442907 netbox_nas-1.0.2/netbox_nas/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:40.438907 netbox_nas-1.0.2/netbox_nas/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:40.446907 netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nascluster.html
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nasmount.html
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nasshare.html
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nasvolume.html
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/netbox_nas/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:40.446907 netbox_nas-1.0.2/netbox_nas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-22 15:53:40.000000 netbox_nas-1.0.2/netbox_nas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-22 15:53:40.000000 netbox_nas-1.0.2/netbox_nas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:53:40.000000 netbox_nas-1.0.2/netbox_nas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:53:40.000000 netbox_nas-1.0.2/netbox_nas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 15:53:40.000000 netbox_nas-1.0.2/netbox_nas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:53:40.446907 netbox_nas-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-22 15:53:30.000000 netbox_nas-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:24:01.987910 netbox_nas-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-29 13:24:01.987910 netbox_nas-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:24:01.983910 netbox_nas-1.0.3/netbox_nas/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:24:01.983910 netbox_nas-1.0.3/netbox_nas/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:24:01.983910 netbox_nas-1.0.3/netbox_nas/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:24:01.979910 netbox_nas-1.0.3/netbox_nas/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:24:01.983910 netbox_nas-1.0.3/netbox_nas/templates/netbox_nas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/templates/netbox_nas/nascluster.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/templates/netbox_nas/nasmount.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/templates/netbox_nas/nasshare.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/templates/netbox_nas/nasvolume.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/netbox_nas/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:24:01.983910 netbox_nas-1.0.3/netbox_nas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-29 13:24:01.000000 netbox_nas-1.0.3/netbox_nas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-29 13:24:01.000000 netbox_nas-1.0.3/netbox_nas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:24:01.000000 netbox_nas-1.0.3/netbox_nas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:24:01.000000 netbox_nas-1.0.3/netbox_nas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 13:24:01.000000 netbox_nas-1.0.3/netbox_nas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:24:01.987910 netbox_nas-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-29 13:23:54.000000 netbox_nas-1.0.3/setup.py
```

### Comparing `netbox_nas-1.0.2/PKG-INFO` & `netbox_nas-1.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 2.1
 Name: netbox-nas
-Version: 1.0.2
+Version: 1.0.3
 Summary: Add NAS entities to NetBox
 Description-Content-Type: text/markdown
 
 ## netbox-nas
 
 A plugin to enable managment of NAS resources.
 
 This plugin introduces four new models:
   - NAS Cluster: The NAS resource provider, e.g. a NAS head node or cluster of nodes. NetBox Devices can be linked to this.
   - NAS Volume: The share backing volume used by the NAS cluster.
   - NAS Share: The share itself, e.g. NFS export, CIFS share, CephFS path, etc.
   - NAS Mount: The mount definition. This describes how a share should be mounted on a particular resource. NetBox Devices, Virtual Machines, and Prefixes can be linked to this currently.
 
 ![Object Links](assets/images/model-links.png)
+
+## Requirements
+Minimum NetBox version:
+  - v1.0.3: NetBox 3.7.8
+  - v1.0.2: NetBox 4.0.0
+  - v1.0.1: NetBox 3.4.0
+  - v1.0.0: NetBox 3.4.0
```

### Comparing `netbox_nas-1.0.2/README.md` & `netbox_nas-1.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,7 +5,14 @@
 This plugin introduces four new models:
   - NAS Cluster: The NAS resource provider, e.g. a NAS head node or cluster of nodes. NetBox Devices can be linked to this.
   - NAS Volume: The share backing volume used by the NAS cluster.
   - NAS Share: The share itself, e.g. NFS export, CIFS share, CephFS path, etc.
   - NAS Mount: The mount definition. This describes how a share should be mounted on a particular resource. NetBox Devices, Virtual Machines, and Prefixes can be linked to this currently.
 
 ![Object Links](assets/images/model-links.png)
+
+## Requirements
+Minimum NetBox version:
+  - v1.0.3: NetBox 3.7.8
+  - v1.0.2: NetBox 4.0.0
+  - v1.0.1: NetBox 3.4.0
+  - v1.0.0: NetBox 3.4.0
```

### Comparing `netbox_nas-1.0.2/netbox_nas/api/serializers.py` & `netbox_nas-1.0.3/netbox_nas/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas/api/views.py` & `netbox_nas-1.0.3/netbox_nas/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas/filtersets.py` & `netbox_nas-1.0.3/netbox_nas/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas/forms.py` & `netbox_nas-1.0.3/netbox_nas/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas/migrations/0001_initial.py` & `netbox_nas-1.0.3/netbox_nas/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas/models.py` & `netbox_nas-1.0.3/netbox_nas/models.py`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas/navigation.py` & `netbox_nas-1.0.3/netbox_nas/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas/search.py` & `netbox_nas-1.0.3/netbox_nas/search.py`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas/tables.py` & `netbox_nas-1.0.3/netbox_nas/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nascluster.html` & `netbox_nas-1.0.3/netbox_nas/templates/netbox_nas/nascluster.html`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nasmount.html` & `netbox_nas-1.0.3/netbox_nas/templates/netbox_nas/nasmount.html`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nasshare.html` & `netbox_nas-1.0.3/netbox_nas/templates/netbox_nas/nasshare.html`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas/templates/netbox_nas/nasvolume.html` & `netbox_nas-1.0.3/netbox_nas/templates/netbox_nas/nasvolume.html`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas/urls.py` & `netbox_nas-1.0.3/netbox_nas/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas/views.py` & `netbox_nas-1.0.3/netbox_nas/views.py`

 * *Files identical despite different names*

### Comparing `netbox_nas-1.0.2/netbox_nas.egg-info/PKG-INFO` & `netbox_nas-1.0.3/netbox_nas.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 2.1
 Name: netbox-nas
-Version: 1.0.2
+Version: 1.0.3
 Summary: Add NAS entities to NetBox
 Description-Content-Type: text/markdown
 
 ## netbox-nas
 
 A plugin to enable managment of NAS resources.
 
 This plugin introduces four new models:
   - NAS Cluster: The NAS resource provider, e.g. a NAS head node or cluster of nodes. NetBox Devices can be linked to this.
   - NAS Volume: The share backing volume used by the NAS cluster.
   - NAS Share: The share itself, e.g. NFS export, CIFS share, CephFS path, etc.
   - NAS Mount: The mount definition. This describes how a share should be mounted on a particular resource. NetBox Devices, Virtual Machines, and Prefixes can be linked to this currently.
 
 ![Object Links](assets/images/model-links.png)
+
+## Requirements
+Minimum NetBox version:
+  - v1.0.3: NetBox 3.7.8
+  - v1.0.2: NetBox 4.0.0
+  - v1.0.1: NetBox 3.4.0
+  - v1.0.0: NetBox 3.4.0
```

### Comparing `netbox_nas-1.0.2/netbox_nas.egg-info/SOURCES.txt` & `netbox_nas-1.0.3/netbox_nas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

