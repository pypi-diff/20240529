# Comparing `tmp/omigo_core-0.6.3.tar.gz` & `tmp/omigo_core-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omigo_core-0.6.3.tar", last modified: Mon Jan 29 22:23:29 2024, max compression
+gzip compressed data, was "omigo_core-0.6.4.tar", last modified: Wed May 29 18:41:34 2024, max compression
```

## Comparing `omigo_core-0.6.3.tar` & `omigo_core-0.6.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:29.500756 omigo_core-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-01-29 22:23:29.500756 omigo_core-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:13.000000 omigo_core-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-29 22:23:13.000000 omigo_core-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-01-29 22:23:29.500756 omigo_core-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:29.492756 omigo_core-0.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:29.496756 omigo_core-0.6.3/src/omigo_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:13.000000 omigo_core-0.6.3/src/omigo_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-01-29 22:23:13.000000 omigo_core-0.6.3/src/omigo_core/etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-01-29 22:23:13.000000 omigo_core-0.6.3/src/omigo_core/file_io_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-01-29 22:23:13.000000 omigo_core-0.6.3/src/omigo_core/file_paths_data_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-29 22:23:13.000000 omigo_core-0.6.3/src/omigo_core/file_paths_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-01-29 22:23:13.000000 omigo_core-0.6.3/src/omigo_core/file_paths_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-01-29 22:23:13.000000 omigo_core-0.6.3/src/omigo_core/funclib.py
--rw-r--r--   0 runner    (1001) docker     (127)    25498 2024-01-29 22:23:13.000000 omigo_core-0.6.3/src/omigo_core/graph_traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-01-29 22:23:13.000000 omigo_core-0.6.3/src/omigo_core/local_fs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    14465 2024-01-29 22:23:13.000000 omigo_core-0.6.3/src/omigo_core/s3_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-01-29 22:23:13.000000 omigo_core-0.6.3/src/omigo_core/s3io_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)   216599 2024-01-29 22:23:13.000000 omigo_core-0.6.3/src/omigo_core/tsv.py
--rw-r--r--   0 runner    (1001) docker     (127)    28453 2024-01-29 22:23:13.000000 omigo_core-0.6.3/src/omigo_core/tsvutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18980 2024-01-29 22:23:13.000000 omigo_core-0.6.3/src/omigo_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:29.500756 omigo_core-0.6.3/src/omigo_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-01-29 22:23:29.000000 omigo_core-0.6.3/src/omigo_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-01-29 22:23:29.000000 omigo_core-0.6.3/src/omigo_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 22:23:29.000000 omigo_core-0.6.3/src/omigo_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-29 22:23:29.000000 omigo_core-0.6.3/src/omigo_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-29 22:23:29.000000 omigo_core-0.6.3/src/omigo_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:23:29.500756 omigo_core-0.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-01-29 22:23:13.000000 omigo_core-0.6.3/test/test_tsv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:34.723882 omigo_core-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-29 18:41:34.723882 omigo_core-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:25.000000 omigo_core-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 18:41:25.000000 omigo_core-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-29 18:41:34.723882 omigo_core-0.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:34.719882 omigo_core-0.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:34.723882 omigo_core-0.6.4/src/omigo_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:25.000000 omigo_core-0.6.4/src/omigo_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-05-29 18:41:25.000000 omigo_core-0.6.4/src/omigo_core/etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-29 18:41:25.000000 omigo_core-0.6.4/src/omigo_core/file_io_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-29 18:41:25.000000 omigo_core-0.6.4/src/omigo_core/file_paths_data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-29 18:41:25.000000 omigo_core-0.6.4/src/omigo_core/file_paths_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-05-29 18:41:25.000000 omigo_core-0.6.4/src/omigo_core/file_paths_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16702 2024-05-29 18:41:25.000000 omigo_core-0.6.4/src/omigo_core/funclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25498 2024-05-29 18:41:25.000000 omigo_core-0.6.4/src/omigo_core/graph_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-29 18:41:25.000000 omigo_core-0.6.4/src/omigo_core/local_fs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15031 2024-05-29 18:41:25.000000 omigo_core-0.6.4/src/omigo_core/s3_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17177 2024-05-29 18:41:25.000000 omigo_core-0.6.4/src/omigo_core/s3io_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)   216599 2024-05-29 18:41:25.000000 omigo_core-0.6.4/src/omigo_core/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28787 2024-05-29 18:41:25.000000 omigo_core-0.6.4/src/omigo_core/tsvutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19157 2024-05-29 18:41:25.000000 omigo_core-0.6.4/src/omigo_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:34.723882 omigo_core-0.6.4/src/omigo_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-29 18:41:34.000000 omigo_core-0.6.4/src/omigo_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-29 18:41:34.000000 omigo_core-0.6.4/src/omigo_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:41:34.000000 omigo_core-0.6.4/src/omigo_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-29 18:41:34.000000 omigo_core-0.6.4/src/omigo_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 18:41:34.000000 omigo_core-0.6.4/src/omigo_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:41:34.723882 omigo_core-0.6.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-29 18:41:25.000000 omigo_core-0.6.4/test/test_tsv.py
```

### Comparing `omigo_core-0.6.3/PKG-INFO` & `omigo_core-0.6.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo_core
-Version: 0.6.3
+Version: 0.6.4
 Summary: Data Analytics Library for Python
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omigo_core-0.6.3/setup.cfg` & `omigo_core-0.6.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = omigo_core
-version = 0.6.3
+version = 0.6.4
 author = amit jaiswal
 author_email = amit.jaiswal@gmail.com
 description = Data Analytics Library for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrowdStrike/omigo-data-analytics
 project_urls =
```

### Comparing `omigo_core-0.6.3/src/omigo_core/etl.py` & `omigo_core-0.6.4/src/omigo_core/etl.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.6.3/src/omigo_core/file_io_wrapper.py` & `omigo_core-0.6.4/src/omigo_core/file_io_wrapper.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.6.3/src/omigo_core/file_paths_data_reader.py` & `omigo_core-0.6.4/src/omigo_core/file_paths_data_reader.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.6.3/src/omigo_core/file_paths_reader.py` & `omigo_core-0.6.4/src/omigo_core/file_paths_reader.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.6.3/src/omigo_core/file_paths_util.py` & `omigo_core-0.6.4/src/omigo_core/file_paths_util.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.6.3/src/omigo_core/funclib.py` & `omigo_core-0.6.4/src/omigo_core/funclib.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,20 @@
 
 def mean(vs):
     vs = list([float(v) for v in vs])
     return statistics.mean(vs)
 
 def std_dev(vs):
     vs = list([float(v) for v in vs])
+
+    # adding check for atleast 2 elements before calling the statistics package
+    if (len(vs) < 2):
+        return 0
+
+    # return
     return statistics.stdev(vs)
 
 def mkstr(vs):
     vs2 = list(filter(lambda t: len(t.strip()) > 0, [str(x) for x in vs]))
     return ",".join(vs2)
 
 def sorted_mkstr(vs):
```

### Comparing `omigo_core-0.6.3/src/omigo_core/graph_traversal.py` & `omigo_core-0.6.4/src/omigo_core/graph_traversal.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.6.3/src/omigo_core/local_fs_wrapper.py` & `omigo_core-0.6.4/src/omigo_core/local_fs_wrapper.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.6.3/src/omigo_core/s3_wrapper.py` & `omigo_core-0.6.4/src/omigo_core/s3_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -236,20 +236,22 @@
         yield from response.get('Contents', [])
         if not response.get('IsTruncated'):  # At the end of the list?
             break
         continuation_token = response.get('NextContinuationToken')
 
 # FIXME: This method is implemented using reverse engineering. Not so reliable
 # TODO: ignore_if_missing should be FALSE by default
+# FIXME: the prefix in aws s3 list command are hurting
 def get_directory_listing(path, filter_func = None, ignore_if_missing = False, skip_exist_check = False, s3_region = None, aws_profile = None):
     s3_region, aws_profile = resolve_region_profile(s3_region, aws_profile)
     s3 = get_s3_client_cache(s3_region = s3_region, aws_profile = aws_profile)
 
     # split the path
     bucket_name, object_key = utils.split_s3_path(path)
+    # utils.info("get_directory_listing: bucket_name: {}, object_key: {}".format(bucket_name, object_key))
 
     filenames = []
     # validation
     if (check_path_exists(path, s3_region = s3_region, aws_profile = aws_profile) == False):
         if (ignore_if_missing == False):
             raise Exception("Directory does not exist: " + path)
         else:
@@ -266,14 +268,22 @@
         # utils.debug("Response: {}".format(dir_content))
         filename = dir_content['Key']
 
         # check if the directory listing was done on leaf node in which case ignore
         if (object_key == filename):
             continue
 
+        # check if there was a prefix match to a parallel directory or key at the same level. in that case ignore
+        if (filename.startswith(object_key)):
+            filename_remaining = filename[len(object_key):]
+
+            # check for valid prefix to a parallel directory
+            if (len(filename_remaining) > 0 and filename_remaining.startswith("/") == False):
+                continue
+
         # extract the key for remaining
         extracted_key = filename[len(object_key) + 1:]
         # utils.debug("extracted_key: {}".format(extracted_key))
 
         # this had directory as child
         parts = extracted_key.split("/")
         base_filename = None
@@ -289,15 +299,15 @@
 
         # collect all the paths found
         if (base_filename is not None):
             # extract the last part and then prepend the bucket and object key to construct full path
             filenames.append(path + "/" + base_filename)
 
     # print the number of object_keys found
-    utils.trace("Number of entries found in directory listing: {}: {}".format(path, count))
+    # utils.trace("Number of entries found in directory listing: {}: {}".format(path, count))
 
     # dedup
     filenames = sorted(list(set(filenames)))
 
     # valid files as boto does a prefix search
     if (skip_exist_check == False):
         filenames = list(filter(lambda t: check_path_exists(t, s3_region = s3_region, aws_profile = aws_profile), filenames))
```

### Comparing `omigo_core-0.6.3/src/omigo_core/s3io_wrapper.py` & `omigo_core-0.6.4/src/omigo_core/s3io_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         index = len(path)
         result1 = list(filter(lambda t: include_reserved_files == True or t.endswith("/" + RESERVED_HIDDEN_FILE) == False, listings))
         result2 = list(map(lambda t: t[index + 1:], result1))
 
         # return
         return result2
 
-    # TODO: this is a wait method and confusing
+    # TODO: this is a wait method and confusing. FIXME: The aws prefix way of listing is hurting
     def ls(self, path, include_reserved_files = False, wait_sec = DEFAULT_WAIT_SEC, attempts = DEFAULT_ATTEMPTS, skip_exist_check = False):
         path = self.__normalize_path__(path)
 
         # go into a wait loop for s3 to sync if the path is missing
         if (self.dir_exists(path) == False and attempts > 0):
             utils.info("ls: path: {} doesnt exist. waiting for {} seconds. attempts: {}".format(path, wait_sec, attempts))
             time.sleep(wait_sec)
```

### Comparing `omigo_core-0.6.3/src/omigo_core/tsv.py` & `omigo_core-0.6.4/src/omigo_core/tsv.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.6.3/src/omigo_core/tsvutils.py` & `omigo_core-0.6.4/src/omigo_core/tsvutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -386,16 +386,27 @@
 
     return tsv.TSV(header, data)
 
 def load_from_array_of_map(map_arr):
     # take a union of all keys
     keys = {}
 
-    # iterate over all maps
+    # copy map array and remove any white spaces
+    map_arr2 = []
     for mp in map_arr:
+        mp2 = {}
+        for k in mp.keys():
+            k2 = utils.replace_spl_white_spaces_with_space(k)
+            v2 = utils.replace_spl_white_spaces_with_space(mp[k])
+            mp2[k2] = v2
+
+        map_arr2.append(mp2)
+
+    # iterate over all maps
+    for mp in map_arr2:
         for k in mp.keys():
             keys[k] = 1
 
     # sort the keys alphabetically
     sorted_keys = sorted(list(set(keys.keys())))
 
     # create header
@@ -404,21 +415,21 @@
     header_map = {}
     for i in range(len(header_fields)):
         h = header_fields[i]
         header_map[h] = i
 
     data = []
     # create data
-    for mp in map_arr:
+    for mp in map_arr2:
         fields = []
         for k in header_fields:
             v = ""
             if (k in mp.keys()):
                 # read as string and replace any newline or tab characters
-                v = utils.strip_spl_white_spaces(mp[k])
+                v = utils.replace_spl_white_spaces_with_space(mp[k])
 
             # append
             fields.append(v)
 
         # create line
         line = "\t".join(fields)
         data.append(line)
```

### Comparing `omigo_core-0.6.3/src/omigo_core/utils.py` & `omigo_core-0.6.4/src/omigo_core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,15 +413,20 @@
 
     # print error
     error(msg)
 
     # raise exception
     raise Exception(msg)
 
+# Deprecated
 def strip_spl_white_spaces(v):
+    warn_once("Deprecated: use replace_spl_white_spaces_with_space")
+    return replace_spl_white_spaces_with_space(v)
+
+def replace_spl_white_spaces_with_space(v):
     # check None
     if (v is None):
         return None
 
     # return
     return str(v).replace("\t", " ").replace("\n", " ").replace("\v", " ").replace("\r", " ")
```

### Comparing `omigo_core-0.6.3/src/omigo_core.egg-info/PKG-INFO` & `omigo_core-0.6.4/src/omigo_core.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo_core
-Version: 0.6.3
+Version: 0.6.4
 Summary: Data Analytics Library for Python
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omigo_core-0.6.3/src/omigo_core.egg-info/SOURCES.txt` & `omigo_core-0.6.4/src/omigo_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

