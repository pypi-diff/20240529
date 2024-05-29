# Comparing `tmp/swanspawner-1.2.0.tar.gz` & `tmp/swanspawner-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swanspawner-1.2.0.tar", last modified: Wed Apr 24 13:01:14 2024, max compression
+gzip compressed data, was "swanspawner-1.2.1.tar", last modified: Wed May 29 08:40:35 2024, max compression
```

## Comparing `swanspawner-1.2.0.tar` & `swanspawner-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:14.890463 swanspawner-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-24 13:01:05.000000 swanspawner-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-24 13:01:14.890463 swanspawner-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-24 13:01:05.000000 swanspawner-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 13:01:05.000000 swanspawner-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:01:14.890463 swanspawner-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-24 13:01:05.000000 swanspawner-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:14.886463 swanspawner-1.2.0/swanspawner/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-24 13:01:05.000000 swanspawner-1.2.0/swanspawner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 13:01:05.000000 swanspawner-1.2.0/swanspawner/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-04-24 13:01:05.000000 swanspawner-1.2.0/swanspawner/swandockerspawner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-24 13:01:05.000000 swanspawner-1.2.0/swanspawner/swankubespawner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-04-24 13:01:05.000000 swanspawner-1.2.0/swanspawner/swanspawner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:14.890463 swanspawner-1.2.0/swanspawner/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-24 13:01:05.000000 swanspawner-1.2.0/swanspawner/templates/options_form_template.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:14.890463 swanspawner-1.2.0/swanspawner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-24 13:01:14.000000 swanspawner-1.2.0/swanspawner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-24 13:01:14.000000 swanspawner-1.2.0/swanspawner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:01:14.000000 swanspawner-1.2.0/swanspawner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:01:14.000000 swanspawner-1.2.0/swanspawner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 13:01:14.000000 swanspawner-1.2.0/swanspawner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 13:01:14.000000 swanspawner-1.2.0/swanspawner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:40:35.761073 swanspawner-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-29 08:40:24.000000 swanspawner-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-29 08:40:35.761073 swanspawner-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-29 08:40:24.000000 swanspawner-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-29 08:40:24.000000 swanspawner-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:40:35.761073 swanspawner-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-29 08:40:24.000000 swanspawner-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:40:35.757073 swanspawner-1.2.1/swanspawner/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-29 08:40:24.000000 swanspawner-1.2.1/swanspawner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-29 08:40:24.000000 swanspawner-1.2.1/swanspawner/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-05-29 08:40:24.000000 swanspawner-1.2.1/swanspawner/swandockerspawner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-29 08:40:24.000000 swanspawner-1.2.1/swanspawner/swankubespawner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-05-29 08:40:24.000000 swanspawner-1.2.1/swanspawner/swanspawner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:40:35.761073 swanspawner-1.2.1/swanspawner/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-05-29 08:40:24.000000 swanspawner-1.2.1/swanspawner/templates/options_form_template.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:40:35.761073 swanspawner-1.2.1/swanspawner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-29 08:40:35.000000 swanspawner-1.2.1/swanspawner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-29 08:40:35.000000 swanspawner-1.2.1/swanspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:40:35.000000 swanspawner-1.2.1/swanspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:40:35.000000 swanspawner-1.2.1/swanspawner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-29 08:40:35.000000 swanspawner-1.2.1/swanspawner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 08:40:35.000000 swanspawner-1.2.1/swanspawner.egg-info/top_level.txt
```

### Comparing `swanspawner-1.2.0/PKG-INFO` & `swanspawner-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swanspawner
-Version: 1.2.0
+Version: 1.2.1
 Summary: SWAN JupyterHub spawner
 Home-page: https://github.com/swan-cern/jupyterhub-extensions
 Author: SWAN Admins
 License: AGPL-3.0
 Keywords: JupyterHub,Spawner,SWAN,CERN
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `swanspawner-1.2.0/README.md` & `swanspawner-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `swanspawner-1.2.0/setup.py` & `swanspawner-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `swanspawner-1.2.0/swanspawner/swandockerspawner.py` & `swanspawner-1.2.1/swanspawner/swandockerspawner.py`

 * *Files identical despite different names*

### Comparing `swanspawner-1.2.0/swanspawner/swankubespawner.py` & `swanspawner-1.2.1/swanspawner/swankubespawner.py`

 * *Files identical despite different names*

### Comparing `swanspawner-1.2.0/swanspawner/swanspawner.py` & `swanspawner-1.2.1/swanspawner/swanspawner.py`

 * *Files identical despite different names*

### Comparing `swanspawner-1.2.0/swanspawner/templates/options_form_template.html` & `swanspawner-1.2.1/swanspawner/templates/options_form_template.html`

 * *Files 5% similar despite different names*

```diff
@@ -140,14 +140,18 @@
         selectCluster.innerHTML = '';
         // Make sure Spark cluster options are enabled on LCG release change
         selectCluster.removeAttribute('disabled');
 
         for( var i = 0 ; i < lcgData.clusters.length ; i++ ){
             var lcgCluster = lcgData.clusters[i];
 
+            if (lcgCluster.value === "k8s" && lcgCluster.value === "hadoop-qa") {
+                continue;
+            }
+
             var selectClusterOption = document.createElement("option");
             selectClusterOption.value = lcgCluster.value;
             selectClusterOption.text = lcgCluster.text;
             if (i === 0) {
                 selectClusterOption.selected = true;
             }
 
@@ -173,27 +177,44 @@
     }
 
     /**
      * Modifies the selection of Spark clusters depending on the chosen platform
      */
     function adjust_spark() {
         var platformOptions = document.getElementById('platformOptions');
-        var clusterOptions  = document.getElementById('clusterOptions');
+
+        function removeCluster(cluster) {
+            var clusterOptions  = document.getElementById('clusterOptions');
+            for (var i = 0; i < clusterOptions.options.length; i++) {
+                if (clusterOptions.options[i].value === cluster) {
+                    clusterOptions.remove(i);
+                    break;
+                }
+            }
+        }
+
+        function addCluster(clusterValue, clusterName) {
+            var selectClusterOption = document.createElement("option");
+            selectClusterOption.value = clusterValue;
+            selectClusterOption.text = clusterName;
+            clusterOptions.add(selectClusterOption);
+        }
 
         var isAlma = platformOptions.selectedOptions[0].text.startsWith('AlmaLinux 9');
 
         if (isAlma) {
-            // Disable Spark cluster selection, since Spark is still not supported
-            // on Alma9
-            clusterOptions.setAttribute('disabled', '');
             clusterOptions.selectedIndex = 0;
+            removeCluster("analytix")
+            addCluster("k8s", "Cloud Containers (K8s)")
+            addCluster("hadoop-qa", "QA")
         }
         else {
-            // On CentOS7, make sure cluster selection is enabled
-            clusterOptions.removeAttribute('disabled');
+            addCluster("analytix", "General Purpose (Analytix)")
+            removeCluster("k8s")
+            removeCluster("hadoop-qa")
         }
     }
 
     window.onload = adjust_form;
 //-->
 </script>
 <div>
```

### Comparing `swanspawner-1.2.0/swanspawner.egg-info/PKG-INFO` & `swanspawner-1.2.1/swanspawner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swanspawner
-Version: 1.2.0
+Version: 1.2.1
 Summary: SWAN JupyterHub spawner
 Home-page: https://github.com/swan-cern/jupyterhub-extensions
 Author: SWAN Admins
 License: AGPL-3.0
 Keywords: JupyterHub,Spawner,SWAN,CERN
 Platform: Linux
 Platform: Mac OS X
```

