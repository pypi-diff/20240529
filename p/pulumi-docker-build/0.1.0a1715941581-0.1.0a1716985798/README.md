# Comparing `tmp/pulumi_docker_build-0.1.0a1715941581.tar.gz` & `tmp/pulumi_docker_build-0.1.0a1716985798.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_docker_build-0.1.0a1715941581.tar", last modified: Fri May 17 10:29:49 2024, max compression
+gzip compressed data, was "pulumi_docker_build-0.1.0a1716985798.tar", last modified: Wed May 29 12:35:18 2024, max compression
```

## Comparing `pulumi_docker_build-0.1.0a1715941581.tar` & `pulumi_docker_build-0.1.0a1716985798.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-17 10:29:49.875678 pulumi_docker_build-0.1.0a1715941581/
--rw-r--r--   0 runner    (1000) runner    (1000)     2554 2024-05-17 10:29:49.875678 pulumi_docker_build-0.1.0a1715941581/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     2057 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-17 10:29:49.875678 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/
--rw-------   0 runner    (1000) runner    (1000)      983 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     1928 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/_enums.py
--rw-------   0 runner    (1000) runner    (1000)    97964 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/_inputs.py
--rw-------   0 runner    (1000) runner    (1000)     9230 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/_utilities.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-17 10:29:49.875678 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/config/
--rw-------   0 runner    (1000) runner    (1000)      267 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/config/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      441 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/config/__init__.pyi
--rw-------   0 runner    (1000) runner    (1000)      756 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/config/vars.py
--rw-------   0 runner    (1000) runner    (1000)    75687 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/image.py
--rw-------   0 runner    (1000) runner    (1000)    14598 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/index.py
--rw-------   0 runner    (1000) runner    (1000)    83253 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/outputs.py
--rw-------   0 runner    (1000) runner    (1000)     4780 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/provider.py
--rw-------   0 runner    (1000) runner    (1000)       49 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/pulumi-plugin.json
--rw-------   0 runner    (1000) runner    (1000)        0 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/py.typed
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-17 10:29:49.875678 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2554 2024-05-17 10:29:49.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      668 2024-05-17 10:29:49.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-17 10:29:49.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       49 2024-05-17 10:29:49.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-05-17 10:29:49.000000 pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      736 2024-05-17 10:29:34.000000 pulumi_docker_build-0.1.0a1715941581/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-17 10:29:49.875678 pulumi_docker_build-0.1.0a1715941581/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-29 12:35:18.687388 pulumi_docker_build-0.1.0a1716985798/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2554 2024-05-29 12:35:18.687388 pulumi_docker_build-0.1.0a1716985798/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2057 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-29 12:35:18.687388 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/
+-rw-------   0 runner    (1000) runner    (1000)      983 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     1928 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/_enums.py
+-rw-------   0 runner    (1000) runner    (1000)    97952 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/_inputs.py
+-rw-------   0 runner    (1000) runner    (1000)     9230 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/_utilities.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-29 12:35:18.687388 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/config/
+-rw-------   0 runner    (1000) runner    (1000)      267 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/config/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      441 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/config/__init__.pyi
+-rw-------   0 runner    (1000) runner    (1000)      756 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/config/vars.py
+-rw-------   0 runner    (1000) runner    (1000)    75687 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/image.py
+-rw-------   0 runner    (1000) runner    (1000)    14598 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/index.py
+-rw-------   0 runner    (1000) runner    (1000)    83241 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/outputs.py
+-rw-------   0 runner    (1000) runner    (1000)     4780 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/provider.py
+-rw-------   0 runner    (1000) runner    (1000)       49 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/pulumi-plugin.json
+-rw-------   0 runner    (1000) runner    (1000)        0 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/py.typed
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-29 12:35:18.687388 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2554 2024-05-29 12:35:18.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      668 2024-05-29 12:35:18.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-29 12:35:18.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       49 2024-05-29 12:35:18.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-05-29 12:35:18.000000 pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      736 2024-05-29 12:35:07.000000 pulumi_docker_build-0.1.0a1716985798/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-29 12:35:18.687388 pulumi_docker_build-0.1.0a1716985798/setup.cfg
```

### Comparing `pulumi_docker_build-0.1.0a1715941581/PKG-INFO` & `pulumi_docker_build-0.1.0a1716985798/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_docker_build
-Version: 0.1.0a1715941581
+Version: 0.1.0a1716985798
 Summary: A Pulumi provider for building modern Docker images with buildx and BuildKit.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-docker-build
 Keywords: docker,buildkit,buildx,kind/native
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_docker_build-0.1.0a1715941581/README.md` & `pulumi_docker_build-0.1.0a1716985798/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/__init__.py` & `pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/_enums.py` & `pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/_inputs.py` & `pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,28 +204,28 @@
                and is typically generated automatically as part of each job.
                
                Defaults to `$ACTIONS_RUNTIME_TOKEN`, although a separate action like
                `crazy-max/ghaction-github-runtime` is recommended to expose this
                environment variable to your jobs.
         :param pulumi.Input[str] url: The cache server URL to use for artifacts.
                
-               Defaults to `$ACTIONS_RUNTIME_URL`, although a separate action like
+               Defaults to `$ACTIONS_CACHE_URL`, although a separate action like
                `crazy-max/ghaction-github-runtime` is recommended to expose this
                environment variable to your jobs.
         """
         if scope is None:
             scope = (_utilities.get_env('buildkit') or '')
         if scope is not None:
             pulumi.set(__self__, "scope", scope)
         if token is None:
             token = (_utilities.get_env('ACTIONS_RUNTIME_TOKEN') or '')
         if token is not None:
             pulumi.set(__self__, "token", token)
         if url is None:
-            url = (_utilities.get_env('ACTIONS_RUNTIME_URL') or '')
+            url = (_utilities.get_env('ACTIONS_CACHE_URL') or '')
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
     def scope(self) -> Optional[pulumi.Input[str]]:
         """
@@ -259,15 +259,15 @@
 
     @property
     @pulumi.getter
     def url(self) -> Optional[pulumi.Input[str]]:
         """
         The cache server URL to use for artifacts.
 
-        Defaults to `$ACTIONS_RUNTIME_URL`, although a separate action like
+        Defaults to `$ACTIONS_CACHE_URL`, although a separate action like
         `crazy-max/ghaction-github-runtime` is recommended to expose this
         environment variable to your jobs.
         """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: Optional[pulumi.Input[str]]):
@@ -745,15 +745,15 @@
                and is typically generated automatically as part of each job.
                
                Defaults to `$ACTIONS_RUNTIME_TOKEN`, although a separate action like
                `crazy-max/ghaction-github-runtime` is recommended to expose this
                environment variable to your jobs.
         :param pulumi.Input[str] url: The cache server URL to use for artifacts.
                
-               Defaults to `$ACTIONS_RUNTIME_URL`, although a separate action like
+               Defaults to `$ACTIONS_CACHE_URL`, although a separate action like
                `crazy-max/ghaction-github-runtime` is recommended to expose this
                environment variable to your jobs.
         """
         if ignore_error is None:
             ignore_error = False
         if ignore_error is not None:
             pulumi.set(__self__, "ignore_error", ignore_error)
@@ -766,15 +766,15 @@
         if scope is not None:
             pulumi.set(__self__, "scope", scope)
         if token is None:
             token = (_utilities.get_env('ACTIONS_RUNTIME_TOKEN') or '')
         if token is not None:
             pulumi.set(__self__, "token", token)
         if url is None:
-            url = (_utilities.get_env('ACTIONS_RUNTIME_URL') or '')
+            url = (_utilities.get_env('ACTIONS_CACHE_URL') or '')
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter(name="ignoreError")
     def ignore_error(self) -> Optional[pulumi.Input[bool]]:
         """
@@ -832,15 +832,15 @@
 
     @property
     @pulumi.getter
     def url(self) -> Optional[pulumi.Input[str]]:
         """
         The cache server URL to use for artifacts.
 
-        Defaults to `$ACTIONS_RUNTIME_URL`, although a separate action like
+        Defaults to `$ACTIONS_CACHE_URL`, although a separate action like
         `crazy-max/ghaction-github-runtime` is recommended to expose this
         environment variable to your jobs.
         """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: Optional[pulumi.Input[str]]):
```

### Comparing `pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/_utilities.py` & `pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/config/vars.py` & `pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/image.py` & `pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/index.py` & `pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/index.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/outputs.py` & `pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,28 +301,28 @@
                and is typically generated automatically as part of each job.
                
                Defaults to `$ACTIONS_RUNTIME_TOKEN`, although a separate action like
                `crazy-max/ghaction-github-runtime` is recommended to expose this
                environment variable to your jobs.
         :param str url: The cache server URL to use for artifacts.
                
-               Defaults to `$ACTIONS_RUNTIME_URL`, although a separate action like
+               Defaults to `$ACTIONS_CACHE_URL`, although a separate action like
                `crazy-max/ghaction-github-runtime` is recommended to expose this
                environment variable to your jobs.
         """
         if scope is None:
             scope = (_utilities.get_env('buildkit') or '')
         if scope is not None:
             pulumi.set(__self__, "scope", scope)
         if token is None:
             token = (_utilities.get_env('ACTIONS_RUNTIME_TOKEN') or '')
         if token is not None:
             pulumi.set(__self__, "token", token)
         if url is None:
-            url = (_utilities.get_env('ACTIONS_RUNTIME_URL') or '')
+            url = (_utilities.get_env('ACTIONS_CACHE_URL') or '')
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
     def scope(self) -> Optional[str]:
         """
@@ -348,15 +348,15 @@
 
     @property
     @pulumi.getter
     def url(self) -> Optional[str]:
         """
         The cache server URL to use for artifacts.
 
-        Defaults to `$ACTIONS_RUNTIME_URL`, although a separate action like
+        Defaults to `$ACTIONS_CACHE_URL`, although a separate action like
         `crazy-max/ghaction-github-runtime` is recommended to expose this
         environment variable to your jobs.
         """
         return pulumi.get(self, "url")
 
 
 @pulumi.output_type
@@ -813,15 +813,15 @@
                and is typically generated automatically as part of each job.
                
                Defaults to `$ACTIONS_RUNTIME_TOKEN`, although a separate action like
                `crazy-max/ghaction-github-runtime` is recommended to expose this
                environment variable to your jobs.
         :param str url: The cache server URL to use for artifacts.
                
-               Defaults to `$ACTIONS_RUNTIME_URL`, although a separate action like
+               Defaults to `$ACTIONS_CACHE_URL`, although a separate action like
                `crazy-max/ghaction-github-runtime` is recommended to expose this
                environment variable to your jobs.
         """
         if ignore_error is None:
             ignore_error = False
         if ignore_error is not None:
             pulumi.set(__self__, "ignore_error", ignore_error)
@@ -834,15 +834,15 @@
         if scope is not None:
             pulumi.set(__self__, "scope", scope)
         if token is None:
             token = (_utilities.get_env('ACTIONS_RUNTIME_TOKEN') or '')
         if token is not None:
             pulumi.set(__self__, "token", token)
         if url is None:
-            url = (_utilities.get_env('ACTIONS_RUNTIME_URL') or '')
+            url = (_utilities.get_env('ACTIONS_CACHE_URL') or '')
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter(name="ignoreError")
     def ignore_error(self) -> Optional[bool]:
         """
@@ -884,15 +884,15 @@
 
     @property
     @pulumi.getter
     def url(self) -> Optional[str]:
         """
         The cache server URL to use for artifacts.
 
-        Defaults to `$ACTIONS_RUNTIME_URL`, although a separate action like
+        Defaults to `$ACTIONS_CACHE_URL`, although a separate action like
         `crazy-max/ghaction-github-runtime` is recommended to expose this
         environment variable to your jobs.
         """
         return pulumi.get(self, "url")
 
 
 @pulumi.output_type
```

### Comparing `pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build/provider.py` & `pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build.egg-info/PKG-INFO` & `pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_docker_build
-Version: 0.1.0a1715941581
+Version: 0.1.0a1716985798
 Summary: A Pulumi provider for building modern Docker images with buildx and BuildKit.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-docker-build
 Keywords: docker,buildkit,buildx,kind/native
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_docker_build-0.1.0a1715941581/pulumi_docker_build.egg-info/SOURCES.txt` & `pulumi_docker_build-0.1.0a1716985798/pulumi_docker_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715941581/pyproject.toml` & `pulumi_docker_build-0.1.0a1716985798/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_docker_build"
   description = "A Pulumi provider for building modern Docker images with buildx and BuildKit."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["docker", "buildkit", "buildx", "kind/native"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.1.0a1715941581"
+  version = "0.1.0a1716985798"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-docker-build"
 
 [build-system]
```

