# Comparing `tmp/treasury-0.8.tar.gz` & `tmp/treasury-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treasury-0.8.tar", last modified: Tue Feb  7 15:29:47 2023, max compression
+gzip compressed data, was "treasury-0.9.tar", last modified: Mon Mar  6 08:21:30 2023, max compression
```

## Comparing `treasury-0.8.tar` & `treasury-0.9.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 kiranr    (1000) kiranr    (1000)        0 2023-02-07 15:29:47.854617 treasury-0.8/
--rw-r--r--   0 kiranr    (1000) kiranr    (1000)       84 2022-12-28 16:31:58.000000 treasury-0.8/MANIFEST.in
--rw-r--r--   0 kiranr    (1000) kiranr    (1000)     3475 2023-02-07 15:29:47.854617 treasury-0.8/PKG-INFO
--rw-r--r--   0 kiranr    (1000) kiranr    (1000)     2305 2023-01-18 17:35:41.000000 treasury-0.8/README.md
--rw-r--r--   0 kiranr    (1000) kiranr    (1000)       67 2022-12-28 16:31:58.000000 treasury-0.8/dev.txt
--rw-r--r--   0 kiranr    (1000) kiranr    (1000)       38 2023-02-07 15:29:47.854617 treasury-0.8/setup.cfg
--rw-r--r--   0 kiranr    (1000) kiranr    (1000)     2550 2023-01-18 17:35:41.000000 treasury-0.8/setup.py
-drwxr-xr-x   0 kiranr    (1000) kiranr    (1000)        0 2023-02-07 15:29:47.854617 treasury-0.8/treasury/
--rw-r--r--   0 kiranr    (1000) kiranr    (1000)        0 2022-12-28 16:31:58.000000 treasury-0.8/treasury/__init__.py
--rw-r--r--   0 kiranr    (1000) kiranr    (1000)    16019 2023-02-03 19:47:36.000000 treasury-0.8/treasury/api.py
--rw-r--r--   0 kiranr    (1000) kiranr    (1000)        3 2023-02-07 15:29:33.000000 treasury-0.8/treasury/version.txt
-drwxr-xr-x   0 kiranr    (1000) kiranr    (1000)        0 2023-02-07 15:29:47.854617 treasury-0.8/treasury.egg-info/
--rw-r--r--   0 kiranr    (1000) kiranr    (1000)     3475 2023-02-07 15:29:47.000000 treasury-0.8/treasury.egg-info/PKG-INFO
--rw-r--r--   0 kiranr    (1000) kiranr    (1000)      255 2023-02-07 15:29:47.000000 treasury-0.8/treasury.egg-info/SOURCES.txt
--rw-r--r--   0 kiranr    (1000) kiranr    (1000)        1 2023-02-07 15:29:47.000000 treasury-0.8/treasury.egg-info/dependency_links.txt
--rw-r--r--   0 kiranr    (1000) kiranr    (1000)      158 2023-02-07 15:29:47.000000 treasury-0.8/treasury.egg-info/requires.txt
--rw-r--r--   0 kiranr    (1000) kiranr    (1000)        9 2023-02-07 15:29:47.000000 treasury-0.8/treasury.egg-info/top_level.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-03-06 08:21:30.784065 treasury-0.9/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       96 2023-03-05 07:16:45.000000 treasury-0.9/MANIFEST.in
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3519 2023-03-06 08:21:30.784065 treasury-0.9/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2305 2023-01-18 14:51:40.000000 treasury-0.9/README.md
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        8 2023-03-05 04:59:21.000000 treasury-0.9/airflow.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       81 2023-02-23 00:09:49.000000 treasury-0.9/dev.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2023-03-06 08:21:30.784065 treasury-0.9/setup.cfg
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2731 2023-03-05 05:00:03.000000 treasury-0.9/setup.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-03-06 08:21:30.784065 treasury-0.9/treasury/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2022-07-28 05:37:53.000000 treasury-0.9/treasury/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-03-06 08:21:30.784065 treasury-0.9/treasury/airflow/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1072 2023-03-05 17:46:08.000000 treasury-0.9/treasury/airflow/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4683 2023-03-06 06:24:21.000000 treasury-0.9/treasury/airflow/hooks.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2527 2023-03-06 05:43:58.000000 treasury-0.9/treasury/airflow/operators.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)    15327 2023-03-06 06:29:09.000000 treasury-0.9/treasury/api.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        3 2023-03-06 08:21:26.000000 treasury-0.9/treasury/version.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-03-06 08:21:30.784065 treasury-0.9/treasury.egg-info/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3519 2023-03-06 08:21:30.000000 treasury-0.9/treasury.egg-info/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      387 2023-03-06 08:21:30.000000 treasury-0.9/treasury.egg-info/SOURCES.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-03-06 08:21:30.000000 treasury-0.9/treasury.egg-info/dependency_links.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       77 2023-03-06 08:21:30.000000 treasury-0.9/treasury.egg-info/entry_points.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      205 2023-03-06 08:21:30.000000 treasury-0.9/treasury.egg-info/requires.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        9 2023-03-06 08:21:30.000000 treasury-0.9/treasury.egg-info/top_level.txt
```

### Comparing `treasury-0.8/PKG-INFO` & `treasury-0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treasury
-Version: 0.8
+Version: 0.9
 Summary: treasury
 Home-page: https://bitbucket.org/dbuy/treasury
 Author: dev
 Author-email: developers@directbuy.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -23,14 +23,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: airflow
+Provides-Extra: all
 
 # treasury
 
 a simple api client for interacting with sfcc using waddle as its secrets 
 manager.  named after a group of goldfinches.  pax avium.
 
 ### key config elements
```

### Comparing `treasury-0.8/README.md` & `treasury-0.9/README.md`

 * *Files identical despite different names*

### Comparing `treasury-0.8/setup.py` & `treasury-0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Frankenstein long_description: version-specific changelog note + README
 with open('README.md') as f:
     long_description = f.read()
 
 extras = {}
 all_extras = set()
-for x in [ 'dev' ]:
+for x in [ 'dev', 'airflow', ]:
     filename = f'{x}.txt'
     with open(filename, 'r') as f:
         st = f.read()
     rg = st.split()
     extras[x] = rg
     if x != 'dev':
         all_extras |= set(rg)
@@ -42,14 +42,15 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='dev',
     author_email='developers@directbuy.com',
     url='https://bitbucket.org/dbuy/treasury',
     packages=[
         'treasury',
+        'treasury.airflow',
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: BSD License',
@@ -75,8 +76,13 @@
         'pytz',
         'requests',
         'urllib3',
         'requests_oauthlib',
         'deceit>=0.4'
     ],
     extras_require=extras,
-)
+    entry_points={
+        'apache_airflow_provider': [
+            'provider_info = treasury.airflow:get_provider_info',
+        ],
+    },
+)
```

### Comparing `treasury-0.8/treasury/api.py` & `treasury-0.9/treasury/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                        we created the api client record
         :password (str):  the password that we set when we created the api client
                        record.  It can be reset using account manager.
         :organization_id (str):  this value can be seen from Administration >
                               Salesforce Commerce API Settings (in the
                               admin console)
     """
-    def __init__(self, conf,
+    def __init__(self, conf=None,
                  base_url=None, site_id=None, scopes=None,
                  client_id=None, password=None, organization_id=None,
                  webdav_prefix=None, default_time_zone=None,
                  timeout=300, **kwargs):
         """
         :param str which: specifies which config to load from waddle
         :param int timeout: specify -1 to wait indefinitely for a response
@@ -71,23 +71,21 @@
         self.site_id = site_id or conf.site_id
         self.scopes = scopes or conf.scopes
         self.conf = conf
         self.client_id = client_id or conf.client_id
         self.password = password or conf.password
         self.organization_id = organization_id or conf.organization_id
         self.default_time_zone = default_time_zone or timezone('PST8PDT')
-        self.webdav_prefix = webdav_prefix or conf.webdav_prefix
+        self.webdav_prefix = webdav_prefix
+        if not self.webdav_prefix and conf:
+            self.webdav_prefix = conf.webdav_prefix
         self.token_expires_at = datetime.now(utc)
-        self.page_size = conf.page_size
-        self.read_columns = conf.read_columns
-        self.column_alias = conf.column_alias
-        self.columns_order = conf.columns_order
         adapter = RetryAdapter(max_retries=5)
         self.session = OAuth2Session(client=BackendApplicationClient(
-            client_id=conf.client_id,
+            client_id=self.client_id,
             scope=self.scope),
             auto_refresh_url='https://account.demandware.com/dwsso/oauth2/access_token')
         self.session.mount('https://', adapter)
         self.base_orders_url = (
             f'checkout/orders/v1'
             f'/organizations/{self.organization_id}'
         )
@@ -101,15 +99,14 @@
         )
 
         self.base_catalog_url = (
             f'product/catalogs/v1'
             f'/organizations/{self.organization_id}/catalogs'
         )
 
-
     @property
     def json_headers(self):
         return {
             'content-type': 'application/json',
         }
 
     @property
@@ -131,26 +128,21 @@
             scope=self.scope)
         expires_at = self.session.token['expires_at']
         self.token_expires_at = datetime.fromtimestamp(expires_at, utc)
         self.token_expires_at -= timedelta(minutes=5)
 
     def send(self, method, route, params=None, form_data=None, json_data=None,
              raw=False, **kwargs):
-        parse_response = not raw
         h = kwargs.pop('headers', None)
         headers = {}
         headers.update(self.json_headers)
         headers.update(h or {})
         response = super().send(
             method=method, route=route, params=params, form_data=form_data,
-            json_data=json_data, raw=True, headers=headers, **kwargs)
-        if parse_response:
-            result = self.handle_response(response)
-            if result:
-                return result
+            json_data=json_data, raw=raw, headers=headers, **kwargs)
         return response
 
     @property
     def expired(self):
         return self.now() >= self.token_expires_at
 
     def presend(self, request: PreparedRequest):
@@ -333,18 +325,15 @@
                 break
             params['offset'] = count
             product_data = self.post(url, json_data=params)
 
         # loop through the list of products to get required data
         products = []
         for index, variant in enumerate(list_products):
-            row = {}
-            result = self.product(variant)
-            for count, key in enumerate(self.read_columns):
-                row[self.column_alias[count]] = self.get_val_from_str(key, json.loads(json.dumps(result)))
+            row = self.product(variant)
             products.append(row)
         return products
 
     def get_zone_info(self, **kwargs):
         url = f'{self.base_cdn_url}/zones/info'
         response = self.get(url, **kwargs)
         return response
@@ -407,17 +396,7 @@
             json_data = {
                 'type': type_,
                 'action': action,
                 'values': values,
             }
             return self.post(url, json_data)
         return None
-
-    def get_val_from_str(self, string, dct):
-        keys = string.split('.')
-        v = dct
-        for key in keys:
-            if key in v:
-                v = v[key]
-            else:
-                return ''
-        return v
```

### Comparing `treasury-0.8/treasury.egg-info/PKG-INFO` & `treasury-0.9/treasury.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treasury
-Version: 0.8
+Version: 0.9
 Summary: treasury
 Home-page: https://bitbucket.org/dbuy/treasury
 Author: dev
 Author-email: developers@directbuy.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -23,14 +23,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: airflow
+Provides-Extra: all
 
 # treasury
 
 a simple api client for interacting with sfcc using waddle as its secrets 
 manager.  named after a group of goldfinches.  pax avium.
 
 ### key config elements
```

