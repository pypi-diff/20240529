# Comparing `tmp/spindrift-4.6-py3-none-any.whl.zip` & `tmp/spindrift-4.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15376 bytes, number of entries: 11
--rw-rw-r--  2.0 unx       59 b- defN 24-May-18 14:44 spindrift/__init__.py
+Zip file size: 15604 bytes, number of entries: 11
+-rw-rw-r--  2.0 unx       59 b- defN 24-May-27 15:31 spindrift/__init__.py
 -rw-rw-r--  2.0 unx     3369 b- defN 24-Jan-05 05:39 spindrift/cli.py
 -rw-rw-r--  2.0 unx      518 b- defN 24-Jan-05 05:39 spindrift/compat.py
--rw-rw-r--  2.0 unx    39420 b- defN 24-May-18 14:44 spindrift/packager.py
+-rw-rw-r--  2.0 unx    41001 b- defN 24-May-27 16:13 spindrift/packager.py
 -rw-rw-r--  2.0 unx     4145 b- defN 24-Jan-05 05:39 spindrift/wsgi.py
--rwxrwxr-x  2.0 unx      102 b- defN 24-May-18 14:45 spindrift-4.6.data/scripts/spindrift
--rw-r--r--  2.0 unx     1062 b- defN 24-May-18 14:45 spindrift-4.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx      999 b- defN 24-May-18 14:45 spindrift-4.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-18 14:45 spindrift-4.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 24-May-18 14:45 spindrift-4.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      854 b- defN 24-May-18 14:45 spindrift-4.6.dist-info/RECORD
-11 files, 50630 bytes uncompressed, 13940 bytes compressed:  72.5%
+-rwxrwxr-x  2.0 unx      102 b- defN 24-May-27 16:15 spindrift-4.7.data/scripts/spindrift
+-rw-r--r--  2.0 unx     1062 b- defN 24-May-27 16:15 spindrift-4.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      999 b- defN 24-May-27 16:15 spindrift-4.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-27 16:15 spindrift-4.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 24-May-27 16:15 spindrift-4.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      854 b- defN 24-May-27 16:15 spindrift-4.7.dist-info/RECORD
+11 files, 52211 bytes uncompressed, 14168 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: spindrift/packager.py
 Comment: 
 
 Filename: spindrift/wsgi.py
 Comment: 
 
-Filename: spindrift-4.6.data/scripts/spindrift
+Filename: spindrift-4.7.data/scripts/spindrift
 Comment: 
 
-Filename: spindrift-4.6.dist-info/LICENSE
+Filename: spindrift-4.7.dist-info/LICENSE
 Comment: 
 
-Filename: spindrift-4.6.dist-info/METADATA
+Filename: spindrift-4.7.dist-info/METADATA
 Comment: 
 
-Filename: spindrift-4.6.dist-info/WHEEL
+Filename: spindrift-4.7.dist-info/WHEEL
 Comment: 
 
-Filename: spindrift-4.6.dist-info/top_level.txt
+Filename: spindrift-4.7.dist-info/top_level.txt
 Comment: 
 
-Filename: spindrift-4.6.dist-info/RECORD
+Filename: spindrift-4.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spindrift/__init__.py

```diff
@@ -1,3 +1,3 @@
 # Copyright 2017-2024, Ryan P. Kelly.
 
-__version__ = "4.6"
+__version__ = "4.7"
```

## spindrift/packager.py

```diff
@@ -182,58 +182,117 @@
 
             # output our zip bundle to the given destination
             output_zip_bundle(temp_file.name, destination)
 
     logger.info("done outputting archive")
 
 
-def find_dependencies(type, package_name, renamed_packages, boto_handling="default"):
-    import pip._vendor.pkg_resources
+def find_dependencies(type, package_name, renamed_packages, boto_handling="default", dependencies_for_package=None):
+    if dependencies_for_package is None:
+        dependencies_for_package = []
+
+    package = get_package_from_name(
+        type,
+        package_name,
+        renamed_packages,
+        boto_handling=boto_handling,
+    )
+
+    if package is None:
+        return dependencies_for_package
+
+    dependencies_for_package.append(package)
+    processed_dependencies = {package}
+    dependencies_to_process = [package]
+
+    while dependencies_to_process:
+
+        local_package = dependencies_to_process[0]
+        dependencies_to_process = dependencies_to_process[1:]
+
+        local_dependencies = _find_dependencies(
+            type,
+            local_package.key,
+            renamed_packages,
+            boto_handling=boto_handling,
+        )
 
-    if renamed_packages is not None:
+        for local_dependency in local_dependencies:
+            if local_dependency in processed_dependencies:
+                continue
 
-        if isinstance(renamed_packages, dict):
-            if package_name in renamed_packages:
-                package_name = renamed_packages[package_name]
-        elif callable(renamed_packages):
-            package_name = renamed_packages(package_name)
+            processed_dependencies.add(local_dependency)
 
-    if package_name is None:
-        return []
+            dependencies_to_process.append(local_dependency)
+            dependencies_for_package.append(local_dependency)
 
-    package = pip._vendor.pkg_resources.working_set.by_key[package_name]
+    return dependencies_for_package
 
-    # boto is available on lambda, don't always repackage it
-    if package.key in ("boto3", "botocore") and boto_handling == "default":
-        if type not in ("flask-eb", "flask-eb-reqs"):
-            return []
+
+def _find_dependencies(type, package_name, renamed_packages, boto_handling="default"):
+
+    package = get_package_from_name(
+        type,
+        package_name,
+        renamed_packages,
+        boto_handling=boto_handling,
+    )
+
+    if package is None:
+        return []
 
     ret = [package]
 
     requires = package.requires()
     for requirement in requires:
 
         # if this requirement is conditional on the environment, skip it if we
         # don't need it
         if requirement.marker is not None:
             if not requirement.marker.evaluate():
                 continue
 
-        ret.extend(
-            find_dependencies(
-                type,
-                requirement.key,
-                renamed_packages,
-                boto_handling=boto_handling,
-            ),
+        requirement_package = get_package_from_name(
+            type,
+            requirement.key,
+            renamed_packages,
+            boto_handling=boto_handling,
         )
 
+        if requirement_package is not None:
+            ret.append(requirement_package)
+
     return sorted(list(set(ret)))
 
 
+def get_package_from_name(type, package_name, renamed_packages, boto_handling="default"):
+
+    import pip._vendor.pkg_resources
+
+    if renamed_packages is not None:
+
+        if isinstance(renamed_packages, dict):
+            if package_name in renamed_packages:
+                package_name = renamed_packages[package_name]
+        elif callable(renamed_packages):
+            package_name = renamed_packages(package_name)
+
+    if package_name is None:
+        return None
+
+    package = pip._vendor.pkg_resources.working_set.by_key[package_name]
+
+    # boto is available on lambda, don't always repackage it
+    if package.key in ("boto3", "botocore") and boto_handling == "default":
+        if type not in ("flask-eb", "flask-eb-reqs"):
+            return None
+
+    return package
+
+
 def install_dependencies(path, package, runtime, dependencies, download=True, cache_path=None):
 
     logger.info("[{}] installing dependencies".format(package))
 
     # we will return our dependencies, grouped by the method in which they were
     # installed
     installed_dependencies = {}
```

## Comparing `spindrift-4.6.dist-info/LICENSE` & `spindrift-4.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `spindrift-4.6.dist-info/METADATA` & `spindrift-4.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spindrift
-Version: 4.6
+Version: 4.7
 Summary: package python applications for AWS Lambda, AWS Elastic Beanstalk, AWS Batch (Docker)
 Home-page: https://github.com/f0rk/spindrift
 Author: Ryan P. Kelly
 Author-email: ryan@ryankelly.us
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

