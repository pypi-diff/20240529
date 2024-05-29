# Comparing `tmp/dagknows-0.0.98-py3-none-any.whl.zip` & `tmp/dagknows-0.0.99-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 50037 bytes, number of entries: 39
--rw-r--r--  2.0 unx       23 b- defN 24-Mar-11 20:24 dagcli/__init__.py
+Zip file size: 50149 bytes, number of entries: 39
+-rw-r--r--  2.0 unx       23 b- defN 24-Mar-13 05:53 dagcli/__init__.py
 -rw-r--r--  2.0 unx     6297 b- defN 23-Dec-17 07:58 dagcli/client.py
 -rw-r--r--  2.0 unx     3737 b- defN 24-Mar-01 19:29 dagcli/config.py
 -rw-r--r--  2.0 unx     4353 b- defN 23-Nov-15 01:21 dagcli/configs.py
 -rw-r--r--  2.0 unx     7308 b- defN 24-Mar-08 22:23 dagcli/forwarder.py
 -rw-r--r--  2.0 unx      864 b- defN 24-Feb-12 18:05 dagcli/jobs.py
 -rw-r--r--  2.0 unx     2290 b- defN 23-Apr-22 21:07 dagcli/messages.py
--rw-r--r--  2.0 unx     8998 b- defN 24-Mar-11 20:24 dagcli/proxy.py
+-rw-r--r--  2.0 unx     9347 b- defN 24-Mar-13 05:59 dagcli/proxy.py
 -rw-r--r--  2.0 unx    13057 b- defN 24-Mar-01 18:44 dagcli/publish.py
 -rw-r--r--  2.0 unx     3204 b- defN 23-Dec-15 21:59 dagcli/root.py
 -rw-r--r--  2.0 unx      496 b- defN 24-Mar-07 01:52 dagcli/run.py
 -rw-r--r--  2.0 unx    12081 b- defN 24-Mar-08 22:23 dagcli/sessions.py
 -rw-r--r--  2.0 unx    13492 b- defN 23-Dec-29 21:19 dagcli/tasks.py
 -rw-r--r--  2.0 unx     1155 b- defN 23-Nov-15 01:31 dagcli/tokens.py
 -rw-r--r--  2.0 unx     4190 b- defN 23-Nov-15 01:32 dagcli/transformers.py
@@ -27,15 +27,15 @@
 -rw-r--r--  2.0 unx     3368 b- defN 23-Jul-20 20:41 dagcli/vault/ips.py
 -rw-r--r--  2.0 unx    16355 b- defN 24-Jan-18 06:03 dagcli/vault/lib.py
 -rw-r--r--  2.0 unx      707 b- defN 23-Jul-20 20:07 dagcli/vault/roles.py
 -rw-r--r--  2.0 unx     1621 b- defN 23-Aug-04 19:05 dagcli/vault/root.py
 -rw-r--r--  2.0 unx     1582 b- defN 23-Jul-20 21:37 dagcli/vault/urls.py
 -rw-r--r--  2.0 unx     1171 b- defN 23-Jul-20 20:31 dagcli/vault/users.py
 -rw-r--r--  2.0 unx     1995 b- defN 23-Jul-20 20:42 dagcli/vault/utils.py
--rw-r--r--  2.0 unx     7048 b- defN 24-Mar-11 20:24 dagknows-0.0.98.dist-info/LICENSE
--rw-r--r--  2.0 unx     1238 b- defN 24-Mar-11 20:24 dagknows-0.0.98.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-11 20:24 dagknows-0.0.98.dist-info/WHEEL
--rw-r--r--  2.0 unx       85 b- defN 24-Mar-11 20:24 dagknows-0.0.98.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Mar-11 20:24 dagknows-0.0.98.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-11 20:24 dagknows-0.0.98.dist-info/zip-safe
--rw-rw-r--  2.0 unx     3002 b- defN 24-Mar-11 20:24 dagknows-0.0.98.dist-info/RECORD
-39 files, 152261 bytes uncompressed, 45353 bytes compressed:  70.2%
+-rw-r--r--  2.0 unx     7048 b- defN 24-Mar-13 06:04 dagknows-0.0.99.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1238 b- defN 24-Mar-13 06:04 dagknows-0.0.99.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-13 06:04 dagknows-0.0.99.dist-info/WHEEL
+-rw-r--r--  2.0 unx       85 b- defN 24-Mar-13 06:04 dagknows-0.0.99.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Mar-13 06:04 dagknows-0.0.99.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Mar-13 06:04 dagknows-0.0.99.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     3002 b- defN 24-Mar-13 06:04 dagknows-0.0.99.dist-info/RECORD
+39 files, 152610 bytes uncompressed, 45465 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -90,29 +90,29 @@
 
 Filename: dagcli/vault/users.py
 Comment: 
 
 Filename: dagcli/vault/utils.py
 Comment: 
 
-Filename: dagknows-0.0.98.dist-info/LICENSE
+Filename: dagknows-0.0.99.dist-info/LICENSE
 Comment: 
 
-Filename: dagknows-0.0.98.dist-info/METADATA
+Filename: dagknows-0.0.99.dist-info/METADATA
 Comment: 
 
-Filename: dagknows-0.0.98.dist-info/WHEEL
+Filename: dagknows-0.0.99.dist-info/WHEEL
 Comment: 
 
-Filename: dagknows-0.0.98.dist-info/entry_points.txt
+Filename: dagknows-0.0.99.dist-info/entry_points.txt
 Comment: 
 
-Filename: dagknows-0.0.98.dist-info/top_level.txt
+Filename: dagknows-0.0.99.dist-info/top_level.txt
 Comment: 
 
-Filename: dagknows-0.0.98.dist-info/zip-safe
+Filename: dagknows-0.0.99.dist-info/zip-safe
 Comment: 
 
-Filename: dagknows-0.0.98.dist-info/RECORD
+Filename: dagknows-0.0.99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dagcli/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.98"
+__version__ = "0.0.99"
```

## dagcli/proxy.py

```diff
@@ -1,8 +1,9 @@
 import subprocess
+from base64 import b64decode
 import typer
 from typing_extensions import Annotated
 from typing import Optional
 from pathlib import Path
 import os, sys
 from typing import List
 import requests
@@ -84,14 +85,21 @@
             newenv = [f"{k}={v}" for k,v in newenvfile.items()]
 
         print("New Updated Env: ")
         print("\n".join(newenv))
 
         with open(envfile, "w") as ef:
             ef.write("\n".join(newenv))
+
+        # See if k8s config exists
+        k8s_proxy_configs = resp.get("k8s_proxy_configs", None)
+        if k8s_proxy_configs:
+            os.makedirs(f"./k8s/proxies", exist_ok=True)
+            with open(f"./k8s/proxies/{label}.tar.gz", 'wb') as tarball:
+                tarball.write(b64decode(k8s_proxy_configs))
     else:
         print("Failed: ", resp.content)
 
 @app.command()
 def get(ctx: typer.Context,
         label: str = typer.Argument(..., help="Label of the new proxy to create"),
         folder: str = typer.Option(None, help="Directory to install proxy files in.  Default to ./{label}")):
```

## Comparing `dagknows-0.0.98.dist-info/LICENSE` & `dagknows-0.0.99.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dagknows-0.0.98.dist-info/METADATA` & `dagknows-0.0.99.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagknows
-Version: 0.0.98
+Version: 0.0.99
 Summary: Our CLI utilities for DagKnows
 Home-page: https://github.com/dagknows/dagclis
 Author: Sriram Panyam
 Author-email: sri@dagknows.com
 License: BSD 3-Clause License
 Keywords: dagknows,cli,api,setuptools
 Classifier: License :: OSI Approved :: BSD License
```

## Comparing `dagknows-0.0.98.dist-info/RECORD` & `dagknows-0.0.99.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-dagcli/__init__.py,sha256=R0_ti3PsltPx4mNjqmHCovLdHboKsuVdrODhlZ0ELGk,23
+dagcli/__init__.py,sha256=3svy--sM0f1CbY-gO0A9g6zDgvjpar3s5vNWbJeQ08Q,23
 dagcli/client.py,sha256=8hxLH0f25TxYT1iO9-ddZsAiQlE6BP0xuhL8d6ypCn4,6297
 dagcli/config.py,sha256=5Oz4zaltU3PImshXppABXCgsoJOnKlNzqjrFFvYmZ1o,3737
 dagcli/configs.py,sha256=BgQF_2eM6LScm-oH1FBiIAWeOG28VuAKVWVT3MNLlwU,4353
 dagcli/forwarder.py,sha256=HxofHMPG5AjQKpFpfNscLfMbECuiNsec32mfrA6zZzQ,7308
 dagcli/jobs.py,sha256=97xVbgWPoM7wzH6TotHGCLtjL7_cQZK1VQRu-qVwcHM,864
 dagcli/messages.py,sha256=ffmd5HmdYa1E1esl1epMPxuG9nKAhMfLokdG0MC9v68,2290
-dagcli/proxy.py,sha256=b1b-M0weQjgKuyUMOiVneqMEQQ5LmKkgb9xX8UgKyn8,8998
+dagcli/proxy.py,sha256=2TW4nvePc-s3wBXqAcN60Mk8KdYxN65qN8AJJ1NrO2M,9347
 dagcli/publish.py,sha256=b_LWSb5-o04Scdv6sJmtKiqAWcXVgS2M5zwe5tX5uKg,13057
 dagcli/root.py,sha256=-2YJcTJLtypl8DwWuf8oGWoHa3OI3OeIqfnDRRK9XtA,3204
 dagcli/run.py,sha256=A3P3FuyNajeQjfCRAfhifxuhEaw0hGJ_Ql9gNvfdo08,496
 dagcli/sessions.py,sha256=DObXd7zsQDPr4wem2-bogZ__JK6aeWAupmG6lEir1C4,12081
 dagcli/tasks.py,sha256=rQa7NLLxyFvS9bgSyT4TG2zdlYq8bQu6mj9m9HQstI4,13492
 dagcli/tokens.py,sha256=vvZP-9DGle9Az6bKJD0eCHhFuk62apztCOoRoTNBnbQ,1155
 dagcli/transformers.py,sha256=US8PrPhTqhpe34veFb-f30nkVgi9UT8wmGizNRWVaVU,4190
@@ -26,14 +26,14 @@
 dagcli/vault/ips.py,sha256=Y8MXrx62ijA--ZyNkiIUMmGImT2sA7zeSXuSJvNJOcs,3368
 dagcli/vault/lib.py,sha256=AOKRk-5U0BhL24eOCN_eevdCHb0RhJtdCxWJGYtt70g,16355
 dagcli/vault/roles.py,sha256=xg1wMZjuQFAkjeQJYhwCar0jruxZSikXuhStJSM-BQg,707
 dagcli/vault/root.py,sha256=Spo_wRRQYic4NCc9gzIK4osFA9XpOyWDzL1VbHwanII,1621
 dagcli/vault/urls.py,sha256=zFi_mF4jogLsNjLse5N0_inhtNNLHd7UIPcp50xzkrw,1582
 dagcli/vault/users.py,sha256=yLHKDTaDb_63mXr63lw5DFh_lxCBYJx9uFtXeaoKsRY,1171
 dagcli/vault/utils.py,sha256=X86aS04ZGyPmBGglgxQ_XqHuULm85ZJVv2sz4ggrS_8,1995
-dagknows-0.0.98.dist-info/LICENSE,sha256=ogEPNDSH0_dhiv_lT3ifVIdgIzHAqNA_SemnxUfPBJk,7048
-dagknows-0.0.98.dist-info/METADATA,sha256=A2tHKGBtFvr3Ai-MLJMJvXIsITElbv08dwGhiflZnOo,1238
-dagknows-0.0.98.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-dagknows-0.0.98.dist-info/entry_points.txt,sha256=s_T37iWvTWRutkyHi6w__7zd2fVz68GQ5fFtStYxM-s,85
-dagknows-0.0.98.dist-info/top_level.txt,sha256=ZyrCJ5UVk8RcMTCA5ZmGRiBB1YoUkaM1a77Biq0nThQ,7
-dagknows-0.0.98.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-dagknows-0.0.98.dist-info/RECORD,,
+dagknows-0.0.99.dist-info/LICENSE,sha256=ogEPNDSH0_dhiv_lT3ifVIdgIzHAqNA_SemnxUfPBJk,7048
+dagknows-0.0.99.dist-info/METADATA,sha256=ZujNgk23DRT7gfWQ255O1BXcl9EQclBETI1g1KweovA,1238
+dagknows-0.0.99.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dagknows-0.0.99.dist-info/entry_points.txt,sha256=s_T37iWvTWRutkyHi6w__7zd2fVz68GQ5fFtStYxM-s,85
+dagknows-0.0.99.dist-info/top_level.txt,sha256=ZyrCJ5UVk8RcMTCA5ZmGRiBB1YoUkaM1a77Biq0nThQ,7
+dagknows-0.0.99.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+dagknows-0.0.99.dist-info/RECORD,,
```

