# Comparing `tmp/keyring_proxy-0.1.2.tar.gz` & `tmp/keyring_proxy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_proxy-0.1.2.tar", last modified: Wed May 29 14:06:55 2024, max compression
+gzip compressed data, was "keyring_proxy-0.1.3.tar", last modified: Wed May 29 14:35:53 2024, max compression
```

## Comparing `keyring_proxy-0.1.2.tar` & `keyring_proxy-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       19 2024-05-29 13:29:53.354115 keyring_proxy-0.1.2/README.md
--rw-r--r--   0        0        0      724 2024-05-29 14:06:55.218976 keyring_proxy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.2/src/keyring_proxy/__init__.py
--rw-r--r--   0        0        0     6872 2024-05-29 14:03:20.644194 keyring_proxy-0.1.2/src/keyring_proxy/transport.py
--rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 keyring_proxy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-29 13:29:53.354115 keyring_proxy-0.1.3/README.md
+-rw-r--r--   0        0        0      724 2024-05-29 14:35:53.680591 keyring_proxy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.3/src/keyring_proxy/__init__.py
+-rw-r--r--   0        0        0     6872 2024-05-29 14:03:20.644194 keyring_proxy-0.1.3/src/keyring_proxy/transport.py
+-rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 keyring_proxy-0.1.3/PKG-INFO
```

### Comparing `keyring_proxy-0.1.2/pyproject.toml` & `keyring_proxy-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "keyring-proxy"
-version = "0.1.2"
+version = "0.1.3"
 description = "Proxy Base for pypi keyring"
 authors = [
     { name = "Kalle M. Aagaard", email = "git@k-moeller.dk" },
 ]
 dependencies = [
     "keyring>=25.2.1",
 ]
@@ -13,20 +13,14 @@
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Repository = "https://github.com/KalleDK/py-keyring-proxy"
 
-[build-system]
-requires = [
-    "pdm-backend",
-]
-build-backend = "pdm.backend"
-
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 tools = [
     "ruff>=0.4.6",
     "black>=24.4.2",
@@ -41,7 +35,13 @@
 line-length = 120
 
 [tool.pyright]
 include = [
     "src",
     "tests",
 ]
+
+[build-system]
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
```

### Comparing `keyring_proxy-0.1.2/src/keyring_proxy/transport.py` & `keyring_proxy-0.1.3/src/keyring_proxy/transport.py`

 * *Files identical despite different names*

