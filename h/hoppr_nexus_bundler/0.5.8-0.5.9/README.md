# Comparing `tmp/hoppr_nexus_bundler-0.5.8.tar.gz` & `tmp/hoppr_nexus_bundler-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_nexus_bundler-0.5.8.tar", max compression
+gzip compressed data, was "hoppr_nexus_bundler-0.5.9.tar", max compression
```

## Comparing `hoppr_nexus_bundler-0.5.8.tar` & `hoppr_nexus_bundler-0.5.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1084 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/LICENSE
--rw-r--r--   0        0        0     1694 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/README.md
--rw-r--r--   0        0        0       89 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/__init__.py
--rw-r--r--   0        0        0     7354 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/bundler.py
--rw-r--r--   0        0        0     1998 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/nexus_instance.py
--rw-r--r--   0        0        0        0 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/__init__.py
--rw-r--r--   0        0        0     4373 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/apt_publisher.py
--rw-r--r--   0        0        0     9582 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/base_publisher.py
--rw-r--r--   0        0        0     6537 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/docker_publisher.py
--rw-r--r--   0        0        0     2278 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/git_publisher.py
--rw-r--r--   0        0        0      833 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/helm_publisher.py
--rw-r--r--   0        0        0     1873 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/maven_publisher.py
--rw-r--r--   0        0        0      859 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/npm_publisher.py
--rw-r--r--   0        0        0      871 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/nuget_publisher.py
--rw-r--r--   0        0        0        0 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/py.typed
--rw-r--r--   0        0        0      832 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/pypi_publisher.py
--rw-r--r--   0        0        0     1861 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/raw_publisher.py
--rw-r--r--   0        0        0     5741 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/yum_publisher.py
--rw-r--r--   0        0        0        0 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/nexus_bundler/py.typed
--rw-r--r--   0        0        0     1241 2024-01-28 01:06:06.000000 hoppr_nexus_bundler-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     2708 1970-01-01 00:00:00.000000 hoppr_nexus_bundler-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/LICENSE
+-rw-r--r--   0        0        0     1694 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/README.md
+-rw-r--r--   0        0        0       89 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/__init__.py
+-rw-r--r--   0        0        0     7354 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/bundler.py
+-rw-r--r--   0        0        0     1998 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/nexus_instance.py
+-rw-r--r--   0        0        0        0 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/__init__.py
+-rw-r--r--   0        0        0     4373 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/apt_publisher.py
+-rw-r--r--   0        0        0     9582 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/base_publisher.py
+-rw-r--r--   0        0        0     6643 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/docker_publisher.py
+-rw-r--r--   0        0        0     2278 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/git_publisher.py
+-rw-r--r--   0        0        0      833 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/helm_publisher.py
+-rw-r--r--   0        0        0     1873 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/maven_publisher.py
+-rw-r--r--   0        0        0      859 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/npm_publisher.py
+-rw-r--r--   0        0        0      871 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/nuget_publisher.py
+-rw-r--r--   0        0        0        0 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/py.typed
+-rw-r--r--   0        0        0      832 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/pypi_publisher.py
+-rw-r--r--   0        0        0     1861 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/raw_publisher.py
+-rw-r--r--   0        0        0     5741 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/yum_publisher.py
+-rw-r--r--   0        0        0        0 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/nexus_bundler/py.typed
+-rw-r--r--   0        0        0     1241 2024-02-12 17:06:00.000000 hoppr_nexus_bundler-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     2708 1970-01-01 00:00:00.000000 hoppr_nexus_bundler-0.5.9/PKG-INFO
```

### Comparing `hoppr_nexus_bundler-0.5.8/LICENSE` & `hoppr_nexus_bundler-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.5.8/README.md` & `hoppr_nexus_bundler-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.5.8/nexus_bundler/bundler.py` & `hoppr_nexus_bundler-0.5.9/nexus_bundler/bundler.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.5.8/nexus_bundler/nexus_instance.py` & `hoppr_nexus_bundler-0.5.9/nexus_bundler/nexus_instance.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/apt_publisher.py` & `hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/apt_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/base_publisher.py` & `hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/base_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/docker_publisher.py` & `hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/docker_publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,19 @@
         path_from_root = path.absolute().relative_to(self.root_dir)
         dest = "/".join(path_from_root.parts[2:])
         docker_url = re.sub(
             r"https?://", "docker://", str(self.nexus_instance.docker_url)
         )
 
         hoppr_version = dist_version("hoppr")
-        if Version.parse(hoppr_version.removeprefix("v")) < Version.parse("1.8.6"):
+        hoppr_version = re.sub(
+            r"v?(?P<version>[\d\.]+\d)(\.dev.*)?", r"\g<version>", hoppr_version
+        )
+
+        if Version.parse(hoppr_version) < Version.parse("1.8.6"):
             dest = docker_url + re.sub(r"(.*)_(.*)", r"\1:\2", dest)
         else:
             dest = docker_url + re.sub(r"(.*)@(.*)", r"\1:\2", dest)
 
         src = f"docker-archive:{path}"
 
         command = [
```

### Comparing `hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/git_publisher.py` & `hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/git_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/helm_publisher.py` & `hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/helm_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/maven_publisher.py` & `hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/maven_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/npm_publisher.py` & `hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/npm_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/nuget_publisher.py` & `hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/nuget_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/pypi_publisher.py` & `hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/pypi_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/raw_publisher.py` & `hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/raw_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.5.8/nexus_bundler/publishers/yum_publisher.py` & `hoppr_nexus_bundler-0.5.9/nexus_bundler/publishers/yum_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.5.8/pyproject.toml` & `hoppr_nexus_bundler-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr_nexus_bundler"
-version = "0.5.8"
+version = "0.5.9"
 description = "Plug-in for Hoppr to bundle artifacts into a Nexus Repository"
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev"
 repository = "https://gitlab.com/hoppr/plugins/hoppr-nexus-bundler"
```

### Comparing `hoppr_nexus_bundler-0.5.8/PKG-INFO` & `hoppr_nexus_bundler-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr_nexus_bundler
-Version: 0.5.8
+Version: 0.5.9
 Summary: Plug-in for Hoppr to bundle artifacts into a Nexus Repository
 Home-page: https://hoppr.dev
 License: MIT
 Keywords: hoppr,plugin,nexus
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
```

