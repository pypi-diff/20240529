# Comparing `tmp/holcstore-0.2.1.tar.gz` & `tmp/holcstore-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holcstore-0.2.1.tar", last modified: Thu May 23 15:37:24 2024, max compression
+gzip compressed data, was "holcstore-0.2.2.tar", last modified: Tue May 28 17:14:55 2024, max compression
```

## Comparing `holcstore-0.2.1.tar` & `holcstore-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:37:24.424799 holcstore-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-23 15:37:21.000000 holcstore-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-23 15:37:21.000000 holcstore-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-23 15:37:24.424799 holcstore-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-23 15:37:21.000000 holcstore-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:37:24.420799 holcstore-0.2.1/holcstore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:37:21.000000 holcstore-0.2.1/holcstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-23 15:37:21.000000 holcstore-0.2.1/holcstore/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-23 15:37:21.000000 holcstore-0.2.1/holcstore/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-23 15:37:21.000000 holcstore-0.2.1/holcstore/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-23 15:37:21.000000 holcstore-0.2.1/holcstore/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:37:24.424799 holcstore-0.2.1/holcstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-23 15:37:24.000000 holcstore-0.2.1/holcstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-23 15:37:24.000000 holcstore-0.2.1/holcstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:37:24.000000 holcstore-0.2.1/holcstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-23 15:37:24.000000 holcstore-0.2.1/holcstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 15:37:24.000000 holcstore-0.2.1/holcstore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:37:24.424799 holcstore-0.2.1/hostore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:37:24.424799 holcstore-0.2.1/hostore/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/migrations/0004_testdatastore_created_at.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/migrations/0005_alter_testdatastore_prm.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:37:24.424799 holcstore-0.2.1/hostore/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/utils/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 15:37:21.000000 holcstore-0.2.1/hostore/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-23 15:37:21.000000 holcstore-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-23 15:37:24.424799 holcstore-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 15:37:21.000000 holcstore-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:55.654345 holcstore-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-28 17:14:51.000000 holcstore-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-28 17:14:51.000000 holcstore-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-28 17:14:55.654345 holcstore-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-28 17:14:51.000000 holcstore-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:55.650345 holcstore-0.2.2/holcstore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:51.000000 holcstore-0.2.2/holcstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-28 17:14:51.000000 holcstore-0.2.2/holcstore/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-28 17:14:51.000000 holcstore-0.2.2/holcstore/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-28 17:14:51.000000 holcstore-0.2.2/holcstore/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-28 17:14:51.000000 holcstore-0.2.2/holcstore/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:55.654345 holcstore-0.2.2/holcstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-28 17:14:55.000000 holcstore-0.2.2/holcstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-28 17:14:55.000000 holcstore-0.2.2/holcstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:14:55.000000 holcstore-0.2.2/holcstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 17:14:55.000000 holcstore-0.2.2/holcstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 17:14:55.000000 holcstore-0.2.2/holcstore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:55.654345 holcstore-0.2.2/hostore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:55.654345 holcstore-0.2.2/hostore/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/migrations/0004_testdatastore_created_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/migrations/0005_alter_testdatastore_prm.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12247 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12663 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:55.654345 holcstore-0.2.2/hostore/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/utils/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 17:14:51.000000 holcstore-0.2.2/hostore/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 17:14:51.000000 holcstore-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-28 17:14:55.654345 holcstore-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 17:14:51.000000 holcstore-0.2.2/setup.py
```

### Comparing `holcstore-0.2.1/LICENSE` & `holcstore-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.1/PKG-INFO` & `holcstore-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holcstore
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Django App to use a simple load curve store
 Home-page: 
 Author: Jean-Pierre Lartigue
 Author-email: 
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `holcstore-0.2.1/README.rst` & `holcstore-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.1/holcstore/settings.py` & `holcstore-0.2.2/holcstore/settings.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.1/holcstore/urls.py` & `holcstore-0.2.2/holcstore/urls.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.1/holcstore.egg-info/PKG-INFO` & `holcstore-0.2.2/holcstore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holcstore
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Django App to use a simple load curve store
 Home-page: 
 Author: Jean-Pierre Lartigue
 Author-email: 
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `holcstore-0.2.1/holcstore.egg-info/SOURCES.txt` & `holcstore-0.2.2/holcstore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.1/hostore/migrations/0001_initial.py` & `holcstore-0.2.2/hostore/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.1/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py` & `holcstore-0.2.2/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.1/hostore/models.py` & `holcstore-0.2.2/hostore/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,14 +122,42 @@
         if len(entries) > 0 and combined_versions:
             ds_combined = ts_combine_first([e['data'] for e in entries])
             entries[0]['data'] = ds_combined
             return entries[0:1]
         return entries
 
     @classmethod
+    def get_lc_by_ids(cls, ids: List[int], client_id: int) -> List[Dict]:
+        """
+        Get the prm load curve
+        Args:
+            ids: List of ids
+            client_id: int, client's id
+        Returns:
+            List[Dict]
+        """
+        logger.info(f'Getting load curve with ids {ids} for client {client_id}')
+
+        qs = cls.objects.filter(id__in=ids, client_id=client_id)
+
+        entries = []
+        for entry in qs:
+            entry_dict = vars(entry)
+            reader = BufferReader(entry_dict['data'])
+            ds = pd.read_feather(reader)
+            if 'index' in ds.columns:
+                ds.set_index('index', inplace=True)
+            else:
+                logger.info(f'data is malformed, remove id {id}')
+                entry.delete()
+            entry_dict['data'] = ds.iloc[:, 0]
+            entries.append(entry_dict)
+        return entries
+
+    @classmethod
     def get_many_lc(cls, prms: [str], client_id: int, combined_versions=True, custom_filters=None) -> Dict[str, List[Dict]]:
         """
         Get many prms from cache
         Args:
             prms: list of prms
             client_id: int, client's id
             combined_versions: bool, if multiple versions exists we combine them (default True)
```

### Comparing `holcstore-0.2.1/hostore/tests.py` & `holcstore-0.2.2/hostore/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,26 @@
         self.assertEquals(len(data), 1)
         self.assertEquals(data[0]['version'], 0)
         # Vérifier que la combinaison donne la deuxième version
         pd.testing.assert_series_equal(data[0]['data'], self.test_data, check_names=False)
 
     # *******************************************************
 
+    def test_get_by_ids(self):
+        TestDataStore.clear_all(self.test_client_id)
+        # Test get_by_ids method
+        new_prm = 'new_test_prm'
+        TestDataStore.set_lc(prm=new_prm, value=self.test_data, client_id=self.test_client_id)
+
+        ids = TestDataStore.objects.all().values_list('id', flat=True)
+        data = TestDataStore.get_lc_by_ids(ids, self.test_client_id)
+
+        self.assertEquals(len(data), 1)
+        pd.testing.assert_series_equal(data[0]['data'], self.test_data, check_names=False)
+
     def test_clearing(self):
         TestDataStore.clear([self.test_prm], self.test_client_id)
         data_after_clear = TestDataStore.get_lc(self.test_prm, self.test_client_id)
         self.assertEqual(len(data_after_clear), 0)
 
     def test_clearing_version(self):
         TestDataStore.clear([self.test_prm_2], self.test_client_id, version=0)
```

### Comparing `holcstore-0.2.1/hostore/utils/timeseries.py` & `holcstore-0.2.2/hostore/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.2.1/setup.cfg` & `holcstore-0.2.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = holcstore
-version = 0.2.1
+version = 0.2.2
 description = A Django App to use a simple load curve store
 long_description = file: README.rst
 url = 
 author = Jean-Pierre Lartigue
 author_email = 
 license = BSD-3-Clause
 classifiers =
```

