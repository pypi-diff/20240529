# Comparing `tmp/lasutils-1.0.67-py3-none-any.whl.zip` & `tmp/lasutils-1.0.68-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 15188 bytes, number of entries: 15
+Zip file size: 15220 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 lasutils/__init__.py
 -rw-r--r--  2.0 unx    14464 b- defN 20-Feb-02 00:00 lasutils/api_poller.py
 -rw-r--r--  2.0 unx     2191 b- defN 20-Feb-02 00:00 lasutils/connector.py
 -rw-r--r--  2.0 unx     2164 b- defN 20-Feb-02 00:00 lasutils/deserializer.py
 -rw-r--r--  2.0 unx      112 b- defN 20-Feb-02 00:00 lasutils/exceptions.py
 -rw-r--r--  2.0 unx     5147 b- defN 20-Feb-02 00:00 lasutils/helpers.py
 -rw-r--r--  2.0 unx     2362 b- defN 20-Feb-02 00:00 lasutils/keyvault.py
 -rw-r--r--  2.0 unx    17042 b- defN 20-Feb-02 00:00 lasutils/las_api.py
 -rw-r--r--  2.0 unx     1082 b- defN 20-Feb-02 00:00 lasutils/my_ffmpeg.py
 -rw-r--r--  2.0 unx     1588 b- defN 20-Feb-02 00:00 lasutils/serializer.py
--rw-r--r--  2.0 unx     1328 b- defN 20-Feb-02 00:00 lasutils/settings.py
+-rw-r--r--  2.0 unx     1391 b- defN 20-Feb-02 00:00 lasutils/settings.py
 -rw-r--r--  2.0 unx     1025 b- defN 20-Feb-02 00:00 lasutils/variable_parser.py
-?rw-r--r--  2.0 unx      650 b- defN 20-Feb-02 00:00 lasutils-1.0.67.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 lasutils-1.0.67.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1150 b- defN 20-Feb-02 00:00 lasutils-1.0.67.dist-info/RECORD
-15 files, 50392 bytes uncompressed, 13318 bytes compressed:  73.6%
+?rw-r--r--  2.0 unx      650 b- defN 20-Feb-02 00:00 lasutils-1.0.68.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 lasutils-1.0.68.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1150 b- defN 20-Feb-02 00:00 lasutils-1.0.68.dist-info/RECORD
+15 files, 50455 bytes uncompressed, 13350 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -30,17 +30,17 @@
 
 Filename: lasutils/settings.py
 Comment: 
 
 Filename: lasutils/variable_parser.py
 Comment: 
 
-Filename: lasutils-1.0.67.dist-info/METADATA
+Filename: lasutils-1.0.68.dist-info/METADATA
 Comment: 
 
-Filename: lasutils-1.0.67.dist-info/WHEEL
+Filename: lasutils-1.0.68.dist-info/WHEEL
 Comment: 
 
-Filename: lasutils-1.0.67.dist-info/RECORD
+Filename: lasutils-1.0.68.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lasutils/settings.py

```diff
@@ -4,14 +4,17 @@
 from pathlib import Path
 import yaml
 
 load_dotenv(find_dotenv())
 
 
 class ConnectorSettings:
+    def __init__(self) -> None:
+        print("Setting init")
+
     def load_settings(self, yaml_file: str):
         settings = yaml.safe_load(open(Path(yaml_file)).read())
         os.environ["POLLER_CLASS"] = settings["spec"]["class"]
         if settings["spec"].get("config"):
             os.environ["CONFIG"] = json.dumps(settings["spec"]["config"])
         if settings["spec"].get("secrets"):
             os.environ["SECRETS"] = json.dumps(settings["spec"]["secrets"])
```

## Comparing `lasutils-1.0.67.dist-info/METADATA` & `lasutils-1.0.68.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lasutils
-Version: 1.0.67
+Version: 1.0.68
 Summary: LAS utils
 Project-URL: Homepage, https://livearenasports.com/
 Author-email: Johan Gustavsson <johan.gustavsson@sportway.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

## Comparing `lasutils-1.0.67.dist-info/RECORD` & `lasutils-1.0.68.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 lasutils/deserializer.py,sha256=1_vh9iq_G5VFbgePd1doK6EMoblPw955WtsgWA6jvhY,2164
 lasutils/exceptions.py,sha256=Zhxtn9PUSiU6aDf5x-yxiWI7gpKWA9oYbrsrOJR_Dd0,112
 lasutils/helpers.py,sha256=JaCgW1EeHre23F9iuEWgzRjbIeY-zJp4v8OkIijgy5M,5147
 lasutils/keyvault.py,sha256=gS4MheMfHQ_nIkoCgEWn6vxqqF29k77nh9qH-74xZMY,2362
 lasutils/las_api.py,sha256=zvyt5ODRiY_fEcb8s6W0n-jmfZDgp9H_HQNZDgZ1mt8,17042
 lasutils/my_ffmpeg.py,sha256=3w6_Zf_YWcH-f8xlP-uiB1UJYPtfJwfbQ-fyLjSyDQk,1082
 lasutils/serializer.py,sha256=WUy6wadA_JJhWCBXuz-mJFhJRh-S9UVD2baTVzVXMus,1588
-lasutils/settings.py,sha256=o29dH0R8gKcpEXATunGIEsdMT3TSgbUjSbV5b7aevf8,1328
+lasutils/settings.py,sha256=nR4U8PR7PrlqqA-F3lMg0askgtjNevzFISTLFcOohfc,1391
 lasutils/variable_parser.py,sha256=Mt02n0wIbSO3OZwFKnDDsraDO1qhz6bpfk78ZJ002fc,1025
-lasutils-1.0.67.dist-info/METADATA,sha256=XQ8JjCWBTqUmBIzBHc-2m-8zhPpubddtMtbolalhKbM,650
-lasutils-1.0.67.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-lasutils-1.0.67.dist-info/RECORD,,
+lasutils-1.0.68.dist-info/METADATA,sha256=MBckNGIUN-6-fARkLVd4lnIcAaq3vqKWMKlSjFfSG6o,650
+lasutils-1.0.68.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+lasutils-1.0.68.dist-info/RECORD,,
```

