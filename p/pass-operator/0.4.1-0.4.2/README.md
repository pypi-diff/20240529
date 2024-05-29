# Comparing `tmp/pass_operator-0.4.1.tar.gz` & `tmp/pass_operator-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pass_operator-0.4.1.tar", max compression
+gzip compressed data, was "pass_operator-0.4.2.tar", max compression
```

## Comparing `pass_operator-0.4.1.tar` & `pass_operator-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35140 2024-05-21 06:10:18.891776 pass_operator-0.4.1/LICENSE
--rw-r--r--   0        0        0     3343 2024-05-21 06:10:18.891776 pass_operator-0.4.1/README.md
--rw-r--r--   0        0        0     1606 2024-05-21 06:10:31.815980 pass_operator-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1562 2024-05-21 06:10:18.899777 pass_operator-0.4.1/src/passoperator/__init__.py
--rw-r--r--   0        0        0    14494 2024-05-21 06:10:18.899777 pass_operator-0.4.1/src/passoperator/daemon.py
--rw-r--r--   0        0        0     2017 2024-05-21 06:10:18.899777 pass_operator-0.4.1/src/passoperator/git.py
--rw-r--r--   0        0        0     1218 2024-05-21 06:10:18.899777 pass_operator-0.4.1/src/passoperator/gpg.py
--rw-r--r--   0        0        0     8500 2024-05-21 06:10:18.899777 pass_operator-0.4.1/src/passoperator/secret.py
--rw-r--r--   0        0        0     1313 2024-05-21 06:10:18.899777 pass_operator-0.4.1/src/passoperator/utils.py
--rw-r--r--   0        0        0     4280 1970-01-01 00:00:00.000000 pass_operator-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35140 2024-05-28 16:07:07.505051 pass_operator-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3338 2024-05-28 16:07:07.505051 pass_operator-0.4.2/README.md
+-rw-r--r--   0        0        0     1606 2024-05-28 16:07:23.913194 pass_operator-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1562 2024-05-28 16:07:07.513051 pass_operator-0.4.2/src/passoperator/__init__.py
+-rw-r--r--   0        0        0    15025 2024-05-28 16:07:07.513051 pass_operator-0.4.2/src/passoperator/daemon.py
+-rw-r--r--   0        0        0     2017 2024-05-28 16:07:07.513051 pass_operator-0.4.2/src/passoperator/git.py
+-rw-r--r--   0        0        0     1218 2024-05-28 16:07:07.513051 pass_operator-0.4.2/src/passoperator/gpg.py
+-rw-r--r--   0        0        0     8500 2024-05-28 16:07:07.513051 pass_operator-0.4.2/src/passoperator/secret.py
+-rw-r--r--   0        0        0     1313 2024-05-28 16:07:07.513051 pass_operator-0.4.2/src/passoperator/utils.py
+-rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 pass_operator-0.4.2/PKG-INFO
```

### Comparing `pass_operator-0.4.1/LICENSE` & `pass_operator-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.1/README.md` & `pass_operator-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
   mykey: <decrypted contents of premiscale/mydata>
 immutable: false
 type: Opaque
 ```
 
 ## Installation
 
-See the [chart README](https://github.com/premiscale/pass-operator/tree/helm-readme/helm/operator) for an overview of operator installation and configuration options.
+See the [chart README](https://github.com/premiscale/pass-operator/tree/master/helm/operator) for an overview of operator installation and configuration options.
 
 ## Development
 
 ### Unit tests
 
 Run unit tests with
```

### Comparing `pass_operator-0.4.1/pyproject.toml` & `pass_operator-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pass-operator"
-version = "v0.4.1"
+version = "v0.4.2"
 description = "A kubernetes operator that syncs and decrypts secrets from pass git repositories"
 authors = ["Emma Doyle <emma@premiscale.com>"]
 maintainers = ["Emma Doyle <emma@premiscale.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [
   { include = "passoperator", from = "src" }
```

### Comparing `pass_operator-0.4.1/src/passoperator/__init__.py` & `pass_operator-0.4.2/src/passoperator/__init__.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.1/src/passoperator/daemon.py` & `pass_operator-0.4.2/src/passoperator/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 A kubernetes operator that syncs and decrypts secrets from Linux password store (https://www.passwordstore.org/) git repositories.
 """
 
 
-from typing import Any, List
+from typing import Any
 from pathlib import Path
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 from importlib import metadata
 from kubernetes import client, config
 from http import HTTPStatus
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
-from time import sleep
 
 from passoperator.git import pull, clone
 from passoperator.utils import LogLevel
 from passoperator.secret import PassSecret, ManagedSecret
 from passoperator import env
 
 import asyncio
@@ -68,14 +67,15 @@
 
     log.info(
         f'Reconciling PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" in Namespace "{passSecretObj.spec.managedSecret.metadata.namespace}" against password store.'
     )
 
     v1 = client.CoreV1Api()
 
+
     try:
         secret = v1.read_namespaced_secret(
             name=passSecretObj.spec.managedSecret.metadata.name,
             namespace=passSecretObj.spec.managedSecret.metadata.namespace
         )
 
         log.debug(secret)
@@ -94,17 +94,28 @@
                 namespace=passSecretObj.spec.managedSecret.metadata.namespace,
                 body=client.V1Secret(
                     **passSecretObj.spec.managedSecret.to_client_dict(finalizers=False)
                 )
             )
 
             log.info(f'Reconciliation successfully updated Secret "{_managedSecret.metadata.name}".')
+        else:
+            log.info(f'Secret "{_managedSecret.metadata.name}" is up-to-date.')
     except client.ApiException as e:
-        raise kopf.PermanentError(e)
+        if e.status == HTTPStatus.NOT_FOUND:
+            log.warning(f'Secret "{passSecretObj.spec.managedSecret.metadata.name}" not found. Recreating managed secret.')
 
+            v1.create_namespaced_secret(
+                namespace=passSecretObj.spec.managedSecret.metadata.namespace,
+                body=client.V1Secret(
+                    **passSecretObj.spec.managedSecret.to_client_dict(finalizers=False)
+                )
+            )
+        else:
+            raise kopf.PermanentError(e)
 
 # @kopf.on.cleanup()
 # def cleanup(**kwargs) -> None:
 #     pass
 
 # @kopf.on.resume()
 # def resume(**kwargs) -> None:
```

### Comparing `pass_operator-0.4.1/src/passoperator/git.py` & `pass_operator-0.4.2/src/passoperator/git.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.1/src/passoperator/gpg.py` & `pass_operator-0.4.2/src/passoperator/gpg.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.1/src/passoperator/secret.py` & `pass_operator-0.4.2/src/passoperator/secret.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.1/src/passoperator/utils.py` & `pass_operator-0.4.2/src/passoperator/utils.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.1/PKG-INFO` & `pass_operator-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pass-operator
-Version: 0.4.1
+Version: 0.4.2
 Summary: A kubernetes operator that syncs and decrypts secrets from pass git repositories
 License: GPL-3.0-or-later
 Keywords: python,kubernetes,secrets,operator,pass
 Author: Emma Doyle
 Author-email: emma@premiscale.com
 Maintainer: Emma Doyle
 Maintainer-email: emma@premiscale.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: attrs (>=23.2.0,<24.0.0)
 Requires-Dist: cattrs (>=23.2.3,<24.0.0)
 Requires-Dist: gitpython (>=3.1.43,<4.0.0)
 Requires-Dist: kopf (>=1.37.2,<2.0.0)
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0)
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: python-gnupg (>=0.5.2,<0.6.0)
@@ -73,15 +74,15 @@
   mykey: <decrypted contents of premiscale/mydata>
 immutable: false
 type: Opaque
 ```
 
 ## Installation
 
-See the [chart README](https://github.com/premiscale/pass-operator/tree/helm-readme/helm/operator) for an overview of operator installation and configuration options.
+See the [chart README](https://github.com/premiscale/pass-operator/tree/master/helm/operator) for an overview of operator installation and configuration options.
 
 ## Development
 
 ### Unit tests
 
 Run unit tests with
```

