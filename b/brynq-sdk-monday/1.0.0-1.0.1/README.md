# Comparing `tmp/brynq_sdk_monday-1.0.0.tar.gz` & `tmp/brynq_sdk_monday-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brynq_sdk_monday-1.0.0.tar", last modified: Tue May  7 13:31:41 2024, max compression
+gzip compressed data, was "dist/brynq_sdk_monday-1.0.1.tar", last modified: Wed May 29 13:54:12 2024, max compression
```

## Comparing `brynq_sdk_monday-1.0.0.tar` & `brynq_sdk_monday-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:31:41.000000 brynq_sdk_monday-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      248 2024-05-07 13:31:41.000000 brynq_sdk_monday-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:31:41.000000 brynq_sdk_monday-1.0.0/brynq_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:31:41.000000 brynq_sdk_monday-1.0.0/brynq_sdk/monday/
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-07 13:31:23.000000 brynq_sdk_monday-1.0.0/brynq_sdk/monday/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12275 2024-05-07 13:31:23.000000 brynq_sdk_monday-1.0.0/brynq_sdk/monday/extract_monday.py
--rw-rw-rw-   0 root         (0) root         (0)     4298 2024-05-07 13:31:23.000000 brynq_sdk_monday-1.0.0/brynq_sdk/monday/extract_tracket.py
--rw-rw-rw-   0 root         (0) root         (0)     5877 2024-05-07 13:31:23.000000 brynq_sdk_monday-1.0.0/brynq_sdk/monday/upload_tracket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:31:41.000000 brynq_sdk_monday-1.0.0/brynq_sdk_monday.egg-info/
--rw-r--r--   0 root         (0) root         (0)      248 2024-05-07 13:31:40.000000 brynq_sdk_monday-1.0.0/brynq_sdk_monday.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-07 13:31:40.000000 brynq_sdk_monday-1.0.0/brynq_sdk_monday.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 13:31:40.000000 brynq_sdk_monday-1.0.0/brynq_sdk_monday.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 13:31:40.000000 brynq_sdk_monday-1.0.0/brynq_sdk_monday.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-07 13:31:40.000000 brynq_sdk_monday-1.0.0/brynq_sdk_monday.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-07 13:31:40.000000 brynq_sdk_monday-1.0.0/brynq_sdk_monday.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 13:31:41.000000 brynq_sdk_monday-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-07 13:31:23.000000 brynq_sdk_monday-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:54:12.000000 brynq_sdk_monday-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      248 2024-05-29 13:54:12.000000 brynq_sdk_monday-1.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:54:12.000000 brynq_sdk_monday-1.0.1/brynq_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:54:12.000000 brynq_sdk_monday-1.0.1/brynq_sdk/monday/
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-29 13:53:55.000000 brynq_sdk_monday-1.0.1/brynq_sdk/monday/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12322 2024-05-29 13:53:55.000000 brynq_sdk_monday-1.0.1/brynq_sdk/monday/extract_monday.py
+-rw-rw-rw-   0 root         (0) root         (0)     4298 2024-05-29 13:53:55.000000 brynq_sdk_monday-1.0.1/brynq_sdk/monday/extract_tracket.py
+-rw-rw-rw-   0 root         (0) root         (0)     5877 2024-05-29 13:53:55.000000 brynq_sdk_monday-1.0.1/brynq_sdk/monday/upload_tracket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:54:12.000000 brynq_sdk_monday-1.0.1/brynq_sdk_monday.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      248 2024-05-29 13:54:12.000000 brynq_sdk_monday-1.0.1/brynq_sdk_monday.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-29 13:54:12.000000 brynq_sdk_monday-1.0.1/brynq_sdk_monday.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 13:54:12.000000 brynq_sdk_monday-1.0.1/brynq_sdk_monday.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 13:54:12.000000 brynq_sdk_monday-1.0.1/brynq_sdk_monday.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-29 13:54:12.000000 brynq_sdk_monday-1.0.1/brynq_sdk_monday.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-29 13:54:12.000000 brynq_sdk_monday-1.0.1/brynq_sdk_monday.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 13:54:12.000000 brynq_sdk_monday-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-29 13:53:55.000000 brynq_sdk_monday-1.0.1/setup.py
```

### Comparing `brynq_sdk_monday-1.0.0/brynq_sdk/monday/extract_monday.py` & `brynq_sdk_monday-1.0.1/brynq_sdk/monday/extract_monday.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,20 +132,20 @@
             return response
 
     def get_column_values(self, item_ids: list):
         """
         :param item_ids: all the items where you want to get the column values from
         """
         # Chunk in lists of 50 items since monday.com doesn't accept requests longer than 50 items
-        items_list = (item_ids[pos:pos + 49] for pos in range(0, len(item_ids), 49))
+        items_list = (item_ids[pos:pos + 25] for pos in range(0, len(item_ids), 25))
         all_data = []
 
         for chunk in items_list:
             payload = {
-                "query": f"query {{items (ids: {chunk} exclude_nonactive: false) {{id name updated_at column_values {{ column {{ title }} id text }} }} }}"
+                "query": f"query {{items (ids: {chunk} exclude_nonactive: false) {{id name updated_at column_values {{ column {{ title }} id text value }} }} }}"
             }
             payload = json.dumps(payload)
             if self.debug:
                 print(payload)
             response = requests.request("POST", self.endpoint, headers=self.headers, data=payload)
             if self.debug:
                 print(response.json())
@@ -157,15 +157,15 @@
             for item in data['items']:
                 row = {}
                 row['item_id'] = item['id']
                 row['item'] = item['name']
                 row['updated_at'] = item['updated_at']
                 for col in item['column_values']:
                     title = col['column']['title']
-                    text = col['text']
+                    text = col['value'] if col['text'] == None else col['text']
                     row[title] = text
                 flat_data.append(row)
             all_data.extend(flat_data)
         df = pd.DataFrame(all_data)
         return df
 
     def get_items(self,
```

### Comparing `brynq_sdk_monday-1.0.0/brynq_sdk/monday/extract_tracket.py` & `brynq_sdk_monday-1.0.1/brynq_sdk/monday/extract_tracket.py`

 * *Files identical despite different names*

### Comparing `brynq_sdk_monday-1.0.0/brynq_sdk/monday/upload_tracket.py` & `brynq_sdk_monday-1.0.1/brynq_sdk/monday/upload_tracket.py`

 * *Files identical despite different names*

