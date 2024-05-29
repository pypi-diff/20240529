# Comparing `tmp/rov_db_access-1.0.5.tar.gz` & `tmp/rov_db_access-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rov_db_access-1.0.5.tar", max compression
+gzip compressed data, was "rov_db_access-1.0.6.tar", max compression
```

## Comparing `rov_db_access-1.0.5.tar` & `rov_db_access-1.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0        0 2024-01-29 18:44:26.776172 rov_db_access-1.0.5/README.md
--rw-r--r--   0        0        0      561 2024-05-27 22:00:30.596269 rov_db_access-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-20 20:01:43.946199 rov_db_access-1.0.5/rov_db_access/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 18:50:41.475751 rov_db_access-1.0.5/rov_db_access/authentication/__init__.py
--rw-r--r--   0        0        0     2332 2024-05-20 20:01:43.946696 rov_db_access-1.0.5/rov_db_access/authentication/models.py
--rw-r--r--   0        0        0     1195 2024-05-20 13:50:20.917781 rov_db_access-1.0.5/rov_db_access/authentication/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.917823 rov_db_access-1.0.5/rov_db_access/config/__init__.py
--rw-r--r--   0        0        0     2069 2024-05-15 15:24:19.907085 rov_db_access-1.0.5/rov_db_access/config/db_utils.py
--rw-r--r--   0        0        0      983 2024-05-20 20:01:43.947272 rov_db_access-1.0.5/rov_db_access/config/settings.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.918355 rov_db_access-1.0.5/rov_db_access/geodata/__init__.py
--rw-r--r--   0        0        0     1966 2024-05-20 13:50:20.918452 rov_db_access-1.0.5/rov_db_access/geodata/models.py
--rw-r--r--   0        0        0        0 2024-05-08 18:50:41.476424 rov_db_access-1.0.5/rov_db_access/gis/__init__.py
--rw-r--r--   0        0        0     8313 2024-05-28 22:12:46.563385 rov_db_access-1.0.5/rov_db_access/gis/models.py
--rw-r--r--   0        0        0       78 2024-05-20 13:50:20.918762 rov_db_access-1.0.5/rov_db_access/gis/test.py
--rw-r--r--   0        0        0    35748 2024-05-28 23:04:21.434811 rov_db_access-1.0.5/rov_db_access/gis/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.919463 rov_db_access-1.0.5/rov_db_access/ine/__init__.py
--rw-r--r--   0        0        0      850 2024-05-20 13:50:20.919583 rov_db_access-1.0.5/rov_db_access/ine/models.py
--rw-r--r--   0        0        0     2298 2024-05-20 13:50:20.919670 rov_db_access-1.0.5/rov_db_access/ine/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.919752 rov_db_access-1.0.5/rov_db_access/label_studio/__init__.py
--rw-r--r--   0        0        0     9115 2024-05-20 13:50:20.919967 rov_db_access-1.0.5/rov_db_access/label_studio/models.py
--rw-r--r--   0        0        0     7153 2024-05-20 13:50:20.920121 rov_db_access-1.0.5/rov_db_access/label_studio/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.920191 rov_db_access-1.0.5/rov_db_access/landing/__init__.py
--rw-r--r--   0        0        0     2124 2024-05-20 13:50:20.920282 rov_db_access-1.0.5/rov_db_access/landing/models.py
--rw-r--r--   0        0        0     5890 2024-05-20 13:50:20.920415 rov_db_access-1.0.5/rov_db_access/landing/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.920480 rov_db_access-1.0.5/rov_db_access/risks/__init__.py
--rw-r--r--   0        0        0     1176 2024-05-20 13:50:20.920564 rov_db_access-1.0.5/rov_db_access/risks/models.py
--rw-r--r--   0        0        0     6554 2024-05-27 19:05:01.933210 rov_db_access-1.0.5/rov_db_access/risks/worker.py
--rw-r--r--   0        0        0        0 2024-05-08 18:50:41.476890 rov_db_access-1.0.5/rov_db_access/sentinel/__init__.py
--rw-r--r--   0        0        0      412 2024-05-08 18:50:41.477041 rov_db_access-1.0.5/rov_db_access/sentinel/models.py
--rw-r--r--   0        0        0     5878 2024-05-20 13:50:20.921035 rov_db_access-1.0.5/rov_db_access/sentinel/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.921067 rov_db_access-1.0.5/rov_db_access/utils/__init__.py
--rw-r--r--   0        0        0     5317 2024-05-20 20:01:43.948847 rov_db_access-1.0.5/rov_db_access/utils/geoserver_utils.py
--rw-r--r--   0        0        0     2078 2024-05-20 20:01:43.949178 rov_db_access-1.0.5/rov_db_access/utils/s3_utils.py
--rw-r--r--   0        0        0     1120 2024-05-20 13:50:20.921348 rov_db_access-1.0.5/rov_db_access/utils/utils.py
--rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 rov_db_access-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-29 18:44:26.776172 rov_db_access-1.0.6/README.md
+-rw-r--r--   0        0        0      561 2024-05-29 15:21:47.087624 rov_db_access-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-20 20:01:43.946199 rov_db_access-1.0.6/rov_db_access/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:50:41.475751 rov_db_access-1.0.6/rov_db_access/authentication/__init__.py
+-rw-r--r--   0        0        0     2332 2024-05-20 20:01:43.946696 rov_db_access-1.0.6/rov_db_access/authentication/models.py
+-rw-r--r--   0        0        0     1195 2024-05-20 13:50:20.917781 rov_db_access-1.0.6/rov_db_access/authentication/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.917823 rov_db_access-1.0.6/rov_db_access/config/__init__.py
+-rw-r--r--   0        0        0     2069 2024-05-15 15:24:19.907085 rov_db_access-1.0.6/rov_db_access/config/db_utils.py
+-rw-r--r--   0        0        0      983 2024-05-20 20:01:43.947272 rov_db_access-1.0.6/rov_db_access/config/settings.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.918355 rov_db_access-1.0.6/rov_db_access/geodata/__init__.py
+-rw-r--r--   0        0        0     1966 2024-05-20 13:50:20.918452 rov_db_access-1.0.6/rov_db_access/geodata/models.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:50:41.476424 rov_db_access-1.0.6/rov_db_access/gis/__init__.py
+-rw-r--r--   0        0        0     8313 2024-05-28 22:12:46.563385 rov_db_access-1.0.6/rov_db_access/gis/models.py
+-rw-r--r--   0        0        0       78 2024-05-20 13:50:20.918762 rov_db_access-1.0.6/rov_db_access/gis/test.py
+-rw-r--r--   0        0        0    36021 2024-05-29 15:21:38.081120 rov_db_access-1.0.6/rov_db_access/gis/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.919463 rov_db_access-1.0.6/rov_db_access/ine/__init__.py
+-rw-r--r--   0        0        0      850 2024-05-20 13:50:20.919583 rov_db_access-1.0.6/rov_db_access/ine/models.py
+-rw-r--r--   0        0        0     2298 2024-05-20 13:50:20.919670 rov_db_access-1.0.6/rov_db_access/ine/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.919752 rov_db_access-1.0.6/rov_db_access/label_studio/__init__.py
+-rw-r--r--   0        0        0     9115 2024-05-20 13:50:20.919967 rov_db_access-1.0.6/rov_db_access/label_studio/models.py
+-rw-r--r--   0        0        0     7153 2024-05-20 13:50:20.920121 rov_db_access-1.0.6/rov_db_access/label_studio/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.920191 rov_db_access-1.0.6/rov_db_access/landing/__init__.py
+-rw-r--r--   0        0        0     2124 2024-05-20 13:50:20.920282 rov_db_access-1.0.6/rov_db_access/landing/models.py
+-rw-r--r--   0        0        0     5890 2024-05-20 13:50:20.920415 rov_db_access-1.0.6/rov_db_access/landing/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.920480 rov_db_access-1.0.6/rov_db_access/risks/__init__.py
+-rw-r--r--   0        0        0     1176 2024-05-20 13:50:20.920564 rov_db_access-1.0.6/rov_db_access/risks/models.py
+-rw-r--r--   0        0        0     6554 2024-05-27 19:05:01.933210 rov_db_access-1.0.6/rov_db_access/risks/worker.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:50:41.476890 rov_db_access-1.0.6/rov_db_access/sentinel/__init__.py
+-rw-r--r--   0        0        0      412 2024-05-08 18:50:41.477041 rov_db_access-1.0.6/rov_db_access/sentinel/models.py
+-rw-r--r--   0        0        0     5878 2024-05-20 13:50:20.921035 rov_db_access-1.0.6/rov_db_access/sentinel/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.921067 rov_db_access-1.0.6/rov_db_access/utils/__init__.py
+-rw-r--r--   0        0        0     5317 2024-05-20 20:01:43.948847 rov_db_access-1.0.6/rov_db_access/utils/geoserver_utils.py
+-rw-r--r--   0        0        0     2078 2024-05-20 20:01:43.949178 rov_db_access-1.0.6/rov_db_access/utils/s3_utils.py
+-rw-r--r--   0        0        0     1120 2024-05-20 13:50:20.921348 rov_db_access-1.0.6/rov_db_access/utils/utils.py
+-rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 rov_db_access-1.0.6/PKG-INFO
```

### Comparing `rov_db_access-1.0.5/pyproject.toml` & `rov_db_access-1.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rov-db-access"
-version = "1.0.5"
+version = "1.0.6"
 description = ""
 authors = ["Pablo Cano <pablo.cano@rovisen.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 geoalchemy2 = "^0.14.2"
```

### Comparing `rov_db_access-1.0.5/rov_db_access/authentication/models.py` & `rov_db_access-1.0.6/rov_db_access/authentication/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/authentication/worker.py` & `rov_db_access-1.0.6/rov_db_access/authentication/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/config/db_utils.py` & `rov_db_access-1.0.6/rov_db_access/config/db_utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/config/settings.py` & `rov_db_access-1.0.6/rov_db_access/config/settings.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/geodata/models.py` & `rov_db_access-1.0.6/rov_db_access/geodata/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/gis/models.py` & `rov_db_access-1.0.6/rov_db_access/gis/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/gis/worker.py` & `rov_db_access-1.0.6/rov_db_access/gis/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -682,26 +682,26 @@
                 bbox=bbox,
                 user_id=user.id,
                 organization_id=user.organization_id
             )
             session.add(new_image)
             session.commit()
             return new_image
-        
+
     def add_run_data_output(self, run_id, data=None):
         with Session(self.engine) as session:
             output = session.scalar(select(Run.output).where(Run.id == run_id))
             if output is None:
                 print(f'Corrupted run with id {run_id}')
             else:
                 output.data = data
                 output.status = "ready"
                 session.commit()
 
-    def add_results_raster(self, run_data_id, object_key, data=None, bbox=None):
+    def add_raster_results(self, run_data_id, object_key, data=None, bbox=None):
         with Session(self.engine) as session:
             new_result = ResultsRaster(
                 url=object_key,
                 data=data,
                 bbox=bbox,
                 run_data_id=run_data_id,
             )
@@ -838,23 +838,25 @@
 
         Args:
             run_id: The id of the run
             bbox: The bbox of the raster
             files_path: The path where the files are located
             runtime: The runtime of the run
             raster_name: The name of the raster file
+            preview_name: The name of the preview file (i.e: thumbnail.png)
             file_names: Array with the names of additional files to upload
             data: additional data to store in the results raster table
         """
         assert isinstance(run_id, int), 'Invalid run_id!'
         assert bbox is None or isinstance(bbox, str), 'Invalid bbox!'
         assert isinstance(runtime, (int, float)), 'Invalid runtime!'
         runtime = int(runtime)
         assert isinstance(files_path, str), 'Invalid files_path!'
         assert raster_name is None or isinstance(raster_name, str), 'Invalid raster_name!'
+        assert preview_name is None or isinstance(preview_name, str), 'Invalid preview_name!'
         assert isinstance(file_names, list), 'Invalid file_names!'
         assert data is None or isinstance(data, dict), 'Invalid data!'
 
         assert raster_name is not None or len(file_names) != 0, 'No files to upload!'
 
         with Session(self.engine) as session:
             # actual function
@@ -883,25 +885,27 @@
 
             if raster_name is not None:
                 print(f'Uploading raster file: {raster_name}')
                 object_key = bucket_base_directory + raster_name
                 file_path = os.path.join(files_path, raster_name)
                 s3_client.upload_file(file_path, object_key)
                 print(f'File uploaded to S3 with key: {object_key}')
-                self.add_results_raster(run_id, object_key, data, bbox)
+                self.add_raster_results(run_id, object_key, data, bbox)
 
-            # update run status
-            # when all runs of a process are finished, an SQL trigger will update the process status
-            run.status = 'finished'
-            run.finished_at = func.now()
-            #run.bbox = bbox
-            run.output.data = {
+            # update RunData status and data
+            run_data_data = {
                 'bbox': bbox,
                 'preview': bucket_base_directory + preview_name
             }
+            self.add_run_data_output(run_id=run_id, data=run_data_data)
+
+            # update Run status
+            # when all runs of a process are finished, an SQL trigger will update the process status
+            run.status = 'finished'
+            run.finished_at = func.now()
 
             # SQL trigger will update the process runtime
             run.runtime = runtime
             # run.filepath = bucket_base_directory
             session.commit()
 
             return True
@@ -910,26 +914,26 @@
         with Session(self.engine) as session:
             query_runs = (
                 select(Run.id)
                 .where(Run.inference_model_id == model_id)
                 .where(Run.status == 'queued')
                 .order_by(Run.id)
             )
-            runs = session.scalars(query_runs)
-            if runs is None:
+            runs = session.scalars(query_runs).all()
+            if runs is None or len(runs) == 0:
                 return []
             else:
                 print(f'Queued runs found!: {len(runs)} results')
                 return runs
 
     def load_run_input(self, run_id: str):
         with Session(self.engine) as session:
             query = select(Run.input).where(Run.id == run_id)
             input = session.scalar(query)
-            if input == None:
+            if input is None:
                 print('Run with corrupted Input data')
             else:
                 return {
                     "status": input.status,
                     "data": input.data,
                     "type": input.type,
                 }
```

### Comparing `rov_db_access-1.0.5/rov_db_access/ine/models.py` & `rov_db_access-1.0.6/rov_db_access/ine/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/ine/worker.py` & `rov_db_access-1.0.6/rov_db_access/ine/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/label_studio/models.py` & `rov_db_access-1.0.6/rov_db_access/label_studio/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/label_studio/worker.py` & `rov_db_access-1.0.6/rov_db_access/label_studio/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/landing/models.py` & `rov_db_access-1.0.6/rov_db_access/landing/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/landing/worker.py` & `rov_db_access-1.0.6/rov_db_access/landing/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/risks/models.py` & `rov_db_access-1.0.6/rov_db_access/risks/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/risks/worker.py` & `rov_db_access-1.0.6/rov_db_access/risks/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/sentinel/worker.py` & `rov_db_access-1.0.6/rov_db_access/sentinel/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/utils/geoserver_utils.py` & `rov_db_access-1.0.6/rov_db_access/utils/geoserver_utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/utils/s3_utils.py` & `rov_db_access-1.0.6/rov_db_access/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/rov_db_access/utils/utils.py` & `rov_db_access-1.0.6/rov_db_access/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.5/PKG-INFO` & `rov_db_access-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rov-db-access
-Version: 1.0.5
+Version: 1.0.6
 Summary: 
 Author: Pablo Cano
 Author-email: pablo.cano@rovisen.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

