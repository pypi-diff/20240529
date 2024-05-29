# Comparing `tmp/lasutils-1.0.65-py3-none-any.whl.zip` & `tmp/lasutils-1.0.67-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 15214 bytes, number of entries: 15
+Zip file size: 15188 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 lasutils/__init__.py
 -rw-r--r--  2.0 unx    14464 b- defN 20-Feb-02 00:00 lasutils/api_poller.py
 -rw-r--r--  2.0 unx     2191 b- defN 20-Feb-02 00:00 lasutils/connector.py
 -rw-r--r--  2.0 unx     2164 b- defN 20-Feb-02 00:00 lasutils/deserializer.py
 -rw-r--r--  2.0 unx      112 b- defN 20-Feb-02 00:00 lasutils/exceptions.py
--rw-r--r--  2.0 unx     5132 b- defN 20-Feb-02 00:00 lasutils/helpers.py
+-rw-r--r--  2.0 unx     5147 b- defN 20-Feb-02 00:00 lasutils/helpers.py
 -rw-r--r--  2.0 unx     2362 b- defN 20-Feb-02 00:00 lasutils/keyvault.py
--rw-r--r--  2.0 unx    16707 b- defN 20-Feb-02 00:00 lasutils/las_api.py
+-rw-r--r--  2.0 unx    17042 b- defN 20-Feb-02 00:00 lasutils/las_api.py
 -rw-r--r--  2.0 unx     1082 b- defN 20-Feb-02 00:00 lasutils/my_ffmpeg.py
 -rw-r--r--  2.0 unx     1588 b- defN 20-Feb-02 00:00 lasutils/serializer.py
--rw-r--r--  2.0 unx     1633 b- defN 20-Feb-02 00:00 lasutils/settings.py
+-rw-r--r--  2.0 unx     1328 b- defN 20-Feb-02 00:00 lasutils/settings.py
 -rw-r--r--  2.0 unx     1025 b- defN 20-Feb-02 00:00 lasutils/variable_parser.py
-?rw-r--r--  2.0 unx      650 b- defN 20-Feb-02 00:00 lasutils-1.0.65.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 lasutils-1.0.65.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1150 b- defN 20-Feb-02 00:00 lasutils-1.0.65.dist-info/RECORD
-15 files, 50347 bytes uncompressed, 13344 bytes compressed:  73.5%
+?rw-r--r--  2.0 unx      650 b- defN 20-Feb-02 00:00 lasutils-1.0.67.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 lasutils-1.0.67.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1150 b- defN 20-Feb-02 00:00 lasutils-1.0.67.dist-info/RECORD
+15 files, 50392 bytes uncompressed, 13318 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -30,17 +30,17 @@
 
 Filename: lasutils/settings.py
 Comment: 
 
 Filename: lasutils/variable_parser.py
 Comment: 
 
-Filename: lasutils-1.0.65.dist-info/METADATA
+Filename: lasutils-1.0.67.dist-info/METADATA
 Comment: 
 
-Filename: lasutils-1.0.65.dist-info/WHEEL
+Filename: lasutils-1.0.67.dist-info/WHEEL
 Comment: 
 
-Filename: lasutils-1.0.65.dist-info/RECORD
+Filename: lasutils-1.0.67.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lasutils/helpers.py

```diff
@@ -146,14 +146,15 @@
         formatter = logging.Formatter(log_fmt)
         return formatter.format(record)
 
 
 def create_csv_report(dir: str, filename: str, items: list):
     if not items:
         log.warn(f"No data found. Report not created.")
+        return
     try:
         csv_file_name = f"{dir}/{filename}"
         with open(csv_file_name, "w", encoding="utf-8-sig", newline="") as csv_file:
             fieldnames = items[0].keys()
             csv_writer = csv.DictWriter(
                 csv_file,
                 fieldnames=fieldnames,
```

## lasutils/las_api.py

```diff
@@ -151,15 +151,15 @@
             API_SITE_ID: site_id,
             "start-from": sf,
             "start-to": st,
             "competition-id": comp_id,
             "hide-cancelled": True,
         }
         params = self._remove_nulls(params)
-        return self.poll("broadcast", params=params, page_size=200)
+        return self.poll("broadcast", params=params, page_size=199)
 
     def get_broadcast_by_id(self, broadcast_id: str):
         params = {
             # API_SITE_ID: self._site_id,
             "broadcastId": broadcast_id,
         }
         return self.poll("broadcast/internal", params=params)
@@ -331,22 +331,27 @@
         params = {
             API_SITE_ID: site_id,
         }
         return self.poll(f"venue", params=params, page_size=200)
 
     # Sites
     def get_sites(self):
-        return self.poll(f"site/config/settings", page_size=200)
+        params = {
+            "sort-column": "siteId",
+            "sort-order": "Ascending",
+        }
+        return self.poll(f"site/config/settings", params=params, page_size=200)
 
     # Cameras
     def get_camera(self, cam_id):
         return self.poll(f"venue/camera/{cam_id}")
 
     def get_cameras(self):
-        return self.poll(f"venue/camera", page_size=200)
+        # return self.poll(f"venue/camera", page_size=200)
+        return self.poll(f"venue/camera")
 
     # Comment
     # Competitions
     def get_competitions(self, ext_id: str = None, site_id: str = None):
         site_id = site_id if site_id else self._site_id
         params = {
             API_SITE_ID: site_id,
@@ -376,18 +381,25 @@
             "siteId": sid,
         }
         return self.post(f"competition", payload=params)
 
     # Groups
     def get_groups(self, site_id: str = None, external_id: str = None):
         site_id = site_id if site_id else self._site_id
-        params = {API_SITE_ID: site_id, "external-id": external_id}
+        params = {
+            API_SITE_ID: site_id,
+            "external-id": external_id,
+            "sort-column": "name",
+            "sort-order": "Ascending",
+        }
         return self.poll("group", params=self._remove_nulls(params), page_size=200)
 
-    def get_group(self, group_id):
+    def get_group(self, group_id: str) -> list:
+        if not group_id:
+            return None
         params = {
             # API_SITE_ID: self._site_id,
         }
         return self.poll(f"group/{group_id}", params=params)
 
     def create_group(
         self,
```

## lasutils/settings.py

```diff
@@ -4,50 +4,41 @@
 from pathlib import Path
 import yaml
 
 load_dotenv(find_dotenv())
 
 
 class ConnectorSettings:
-    def __init__(self, yaml_file: str):
-        self._yaml_file = yaml_file
-        self._config = None
-        self._secrets = None
-        self._settings = self._load_settings(yaml_file)
-
-    def _load_settings(self, yaml_file: str):
+    def load_settings(self, yaml_file: str):
         settings = yaml.safe_load(open(Path(yaml_file)).read())
         os.environ["POLLER_CLASS"] = settings["spec"]["class"]
         if settings["spec"].get("config"):
-            self._config = settings["spec"]["config"]
             os.environ["CONFIG"] = json.dumps(settings["spec"]["config"])
         if settings["spec"].get("secrets"):
-            self._secrets = settings["spec"]["secrets"]
             os.environ["SECRETS"] = json.dumps(settings["spec"]["secrets"])
-        return settings
 
     @property
     def las_user(self):
         return os.getenv("LAS_USER")
 
     @property
     def las_pwd(self):
         return os.getenv("LAS_PWD")
 
     @property
     def poller_class(self):
-        return self._settings["spec"]["class"]
+        return os.getenv("POLLER_CLASS")
 
     @property
     def config(self):
-        return self._config
+        return json.loads(os.getenv("CONFIG"))
 
     @property
     def secrets(self):
-        return self._secrets
+        return os.getenv("SECRETS")
 
 
 # # LAS Auth
 # LAS_USER = os.getenv("LAS_USER")
 # LAS_PWD = os.getenv("LAS_PWD")
 
 # # External Auth
```

## Comparing `lasutils-1.0.65.dist-info/METADATA` & `lasutils-1.0.67.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lasutils
-Version: 1.0.65
+Version: 1.0.67
 Summary: LAS utils
 Project-URL: Homepage, https://livearenasports.com/
 Author-email: Johan Gustavsson <johan.gustavsson@sportway.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

## Comparing `lasutils-1.0.65.dist-info/RECORD` & `lasutils-1.0.67.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 lasutils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lasutils/api_poller.py,sha256=SI5UN0akoY0wyEzkvjqW5X4rFexWyLgcMm8TgoQ_go8,14464
 lasutils/connector.py,sha256=p-mIyCm6LW7VhzUy_sgOV_W__2gCWwzNwfL4A_p1P0k,2191
 lasutils/deserializer.py,sha256=1_vh9iq_G5VFbgePd1doK6EMoblPw955WtsgWA6jvhY,2164
 lasutils/exceptions.py,sha256=Zhxtn9PUSiU6aDf5x-yxiWI7gpKWA9oYbrsrOJR_Dd0,112
-lasutils/helpers.py,sha256=40fo5BHBfQTDXsYgPuf4gjzP_xkp_y-086kCqscl49g,5132
+lasutils/helpers.py,sha256=JaCgW1EeHre23F9iuEWgzRjbIeY-zJp4v8OkIijgy5M,5147
 lasutils/keyvault.py,sha256=gS4MheMfHQ_nIkoCgEWn6vxqqF29k77nh9qH-74xZMY,2362
-lasutils/las_api.py,sha256=n-fVACb9Pnys7sjC-h8ylZPDWwzGSIDW2cWn8bDX6Ow,16707
+lasutils/las_api.py,sha256=zvyt5ODRiY_fEcb8s6W0n-jmfZDgp9H_HQNZDgZ1mt8,17042
 lasutils/my_ffmpeg.py,sha256=3w6_Zf_YWcH-f8xlP-uiB1UJYPtfJwfbQ-fyLjSyDQk,1082
 lasutils/serializer.py,sha256=WUy6wadA_JJhWCBXuz-mJFhJRh-S9UVD2baTVzVXMus,1588
-lasutils/settings.py,sha256=Tc3h8RrtvkwOKp6nKmTYYy5NOWWtdTI9LMDIWdu7hXY,1633
+lasutils/settings.py,sha256=o29dH0R8gKcpEXATunGIEsdMT3TSgbUjSbV5b7aevf8,1328
 lasutils/variable_parser.py,sha256=Mt02n0wIbSO3OZwFKnDDsraDO1qhz6bpfk78ZJ002fc,1025
-lasutils-1.0.65.dist-info/METADATA,sha256=NwDHcBkjeVMgbPyJv-v3ubaihswxXtiGgq-N_irkVII,650
-lasutils-1.0.65.dist-info/WHEEL,sha256=TJPnKdtrSue7xZ_AVGkp9YXcvDrobsjBds1du3Nx6dc,87
-lasutils-1.0.65.dist-info/RECORD,,
+lasutils-1.0.67.dist-info/METADATA,sha256=XQ8JjCWBTqUmBIzBHc-2m-8zhPpubddtMtbolalhKbM,650
+lasutils-1.0.67.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+lasutils-1.0.67.dist-info/RECORD,,
```

