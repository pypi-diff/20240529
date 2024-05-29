# Comparing `tmp/Peliqan-1.6.3.tar.gz` & `tmp/Peliqan-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Peliqan-1.6.3.tar", last modified: Wed May 22 06:39:44 2024, max compression
+gzip compressed data, was "Peliqan-1.7.0.tar", last modified: Wed May 29 07:24:54 2024, max compression
```

## Comparing `Peliqan-1.6.3.tar` & `Peliqan-1.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-22 06:39:44.590258 Peliqan-1.6.3/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-22 06:39:44.590105 Peliqan-1.6.3/PKG-INFO
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-22 06:39:44.585207 Peliqan-1.6.3/Peliqan.egg-info/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-22 06:39:44.000000 Peliqan-1.6.3/Peliqan.egg-info/PKG-INFO
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      437 2024-05-22 06:39:44.000000 Peliqan-1.6.3/Peliqan.egg-info/SOURCES.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2024-05-22 06:39:44.000000 Peliqan-1.6.3/Peliqan.egg-info/dependency_links.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2024-05-22 06:39:44.000000 Peliqan-1.6.3/Peliqan.egg-info/requires.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2024-05-22 06:39:44.000000 Peliqan-1.6.3/Peliqan.egg-info/top_level.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-08-02 11:35:09.000000 Peliqan-1.6.3/README.md
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-22 06:39:44.587417 Peliqan-1.6.3/peliqan/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      872 2024-05-22 06:37:04.000000 Peliqan-1.6.3/peliqan/__init__.py
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-22 06:39:44.589634 Peliqan-1.6.3/peliqan/client/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      421 2024-05-13 13:01:35.000000 Peliqan-1.6.3/peliqan/client/__init__.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    17466 2024-05-22 06:06:57.000000 Peliqan-1.6.3/peliqan/client/backend_service.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1743 2024-05-20 14:08:33.000000 Peliqan-1.6.3/peliqan/client/base.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    10806 2024-05-22 06:06:57.000000 Peliqan-1.6.3/peliqan/client/dbclient.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      928 2024-05-13 13:01:35.000000 Peliqan-1.6.3/peliqan/client/sftpclient.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     4549 2024-05-13 13:01:35.000000 Peliqan-1.6.3/peliqan/client/writeback.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    29172 2024-05-22 06:06:57.000000 Peliqan-1.6.3/peliqan/core.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      393 2024-05-10 06:48:15.000000 Peliqan-1.6.3/peliqan/exceptions.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    20342 2024-03-21 07:17:47.000000 Peliqan-1.6.3/peliqan/local_test.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1118 2024-05-20 14:08:33.000000 Peliqan-1.6.3/peliqan/utils.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2024-05-22 06:39:44.590318 Peliqan-1.6.3/setup.cfg
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1371 2024-05-10 06:48:22.000000 Peliqan-1.6.3/setup.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-29 07:24:54.341915 Peliqan-1.7.0/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-29 07:24:54.341761 Peliqan-1.7.0/PKG-INFO
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-29 07:24:54.334356 Peliqan-1.7.0/Peliqan.egg-info/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-29 07:24:54.000000 Peliqan-1.7.0/Peliqan.egg-info/PKG-INFO
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      437 2024-05-29 07:24:54.000000 Peliqan-1.7.0/Peliqan.egg-info/SOURCES.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2024-05-29 07:24:54.000000 Peliqan-1.7.0/Peliqan.egg-info/dependency_links.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2024-05-29 07:24:54.000000 Peliqan-1.7.0/Peliqan.egg-info/requires.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2024-05-29 07:24:54.000000 Peliqan-1.7.0/Peliqan.egg-info/top_level.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-08-02 11:35:09.000000 Peliqan-1.7.0/README.md
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-29 07:24:54.338492 Peliqan-1.7.0/peliqan/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      872 2024-05-29 07:07:44.000000 Peliqan-1.7.0/peliqan/__init__.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-29 07:24:54.341338 Peliqan-1.7.0/peliqan/client/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      421 2024-05-13 13:01:35.000000 Peliqan-1.7.0/peliqan/client/__init__.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    20269 2024-05-28 11:39:58.000000 Peliqan-1.7.0/peliqan/client/backend_service.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1743 2024-05-20 14:08:33.000000 Peliqan-1.7.0/peliqan/client/base.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    11515 2024-05-28 13:06:11.000000 Peliqan-1.7.0/peliqan/client/dbclient.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      928 2024-05-13 13:01:35.000000 Peliqan-1.7.0/peliqan/client/sftpclient.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     4549 2024-05-13 13:01:35.000000 Peliqan-1.7.0/peliqan/client/writeback.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    33371 2024-05-29 06:20:55.000000 Peliqan-1.7.0/peliqan/core.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      393 2024-05-10 06:48:15.000000 Peliqan-1.7.0/peliqan/exceptions.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    20342 2024-03-21 07:17:47.000000 Peliqan-1.7.0/peliqan/local_test.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1118 2024-05-20 14:08:33.000000 Peliqan-1.7.0/peliqan/utils.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2024-05-29 07:24:54.341988 Peliqan-1.7.0/setup.cfg
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1371 2024-05-10 06:48:22.000000 Peliqan-1.7.0/setup.py
```

### Comparing `Peliqan-1.6.3/PKG-INFO` & `Peliqan-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 1.6.3
+Version: 1.7.0
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-1.6.3/Peliqan.egg-info/PKG-INFO` & `Peliqan-1.7.0/Peliqan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 1.6.3
+Version: 1.7.0
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-1.6.3/README.md` & `Peliqan-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.3/peliqan/__init__.py` & `Peliqan-1.7.0/peliqan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.6.3"
+__version__ = "1.7.0"
 __author__ = 'Peliqan.io'
 __credits__ = 'Peliqan.io'
 
 __all__ = [
     "Peliqan",
     "BasePeliqanClient"
 ]
```

### Comparing `Peliqan-1.6.3/peliqan/client/backend_service.py` & `Peliqan-1.7.0/peliqan/client/backend_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -351,46 +351,122 @@
             "change_id": change_id,
             "writeback_status": writeback_status
         }
 
         response_dict = self.call_backend("patch", url, json=data)
         return response_dict
 
+    def list_servers(self):
+        url = f"{self.BACKEND_URL}/api/servers/"
+        response_dict = self.call_backend("get", url)
+        return response_dict
+
     def list_databases(self):
-        url = f"{self.BACKEND_URL}/api/applications"
+        url = f"{self.BACKEND_URL}/api/applications/"
         response_dict = self.call_backend("get", url)
         return response_dict
 
     def get_table(self, table_id):
         url = f"{self.BACKEND_URL}/api/database/tables/{table_id}/"
         response_dict = self.call_backend("get", url)
         return response_dict
 
-    def update_table(self, table_id, name=None, query=None, settings=None):
+    def create_query(
+        self,
+        name,
+        query,
+        database_id=None,
+        schema_id=None,
+        run_on_peliqan_trino=empty,
+        materialize=empty
+    ):
+        url = f"{self.BACKEND_URL}/api/database/tables/create-sql-query/"
+        if schema_id and not database_id:
+            response = self.get_schema(schema_id)
+            database_id = response['database']
+
+        if database_id:
+            url = f"{self.BACKEND_URL}/api/database/tables/database/{database_id}/"
+
+        data = {
+            'table_type': 'query',
+            'schema_id': schema_id,
+            'name': name,
+            'query': query
+        }
+
+        response_dict = self.call_backend("post", url, json=data)
+
+        if run_on_peliqan_trino is True or materialize is True:
+            response_dict = self.update_table(
+                response_dict['id'],
+                run_on_peliqan_trino=run_on_peliqan_trino,
+                materialize=materialize,
+            )
+
+        return response_dict
+
+    def update_table(
+        self,
+        table_id,
+        name=None,
+        query=None,
+        settings=None,
+        materialize=empty,
+        run_on_peliqan_trino=empty
+    ):
         url = f"{self.BACKEND_URL}/api/database/tables/%s/" % table_id
         data = {}
+
         if name:
-            data["name"] = name
+            data['name'] = name
+
         if query:
-            data["query"] = query
+            data['query'] = query
+
+        if run_on_peliqan_trino != empty:
+            data['run_on_peliqan_trino'] = run_on_peliqan_trino
+
+        if not settings:
+            settings = {}
+
+        if materialize != empty:
+            settings['materialize_settings'] = {
+                'materialize': materialize
+            }
+
         if settings:
-            data["settings"] = settings
+            data['settings'] = settings
+
         response_dict = self.call_backend("patch", url, json=data)
         return response_dict
 
-    def update_database_metadata(self, id, description=None, tags=None):
-        url = f"{self.BACKEND_URL}/api/applications/%s/data-catalog/" % id
+    def update_database_metadata(self, database_id, description=None, tags=None):
+        url = f"{self.BACKEND_URL}/api/applications/%s/data-catalog/" % database_id
         data = {}
         if description:
             data["description"] = description
         if tags:
             data["tags"] = tags
         response_dict = self.call_backend("patch", url, json=data)
         return response_dict
 
+    def get_schema(self, schema_id):
+        url = f"{self.BACKEND_URL}/api/database/schemas/%s/" % schema_id
+        response_dict = self.call_backend("get", url)
+        return response_dict
+
+    def update_schema(self, schema_id, name):
+        url = f"{self.BACKEND_URL}/api/database/schemas/%s/" % schema_id
+        data = {}
+        if name:
+            data["schema_name"] = name
+        response_dict = self.call_backend("patch", url, json=data)
+        return response_dict
+
     def update_table_metadata(self, table_id, description=None, tags=None, primary_field_id=None):
         url = f"{self.BACKEND_URL}/api/database/tables/%s/details/" % table_id
         data = {}
         if description:
             data["description"] = description
         if tags:
             data["tags"] = tags
@@ -428,15 +504,15 @@
 
         data = {k: v for k, v in kwargs.items() if v is not empty}
         return self.call_backend("patch", url, json=data)
 
     def create_interface(self, group_id, **kwargs):
         url = f"{self.BACKEND_URL}/api/interfaces/{group_id}/"
 
-        data = {k: v for k, v in kwargs.items() if v is not empty}
+        data = {k: v for k, v in kwargs.items() if v is not None}
         return self.call_backend("post", url, json=data)
 
     def get_interface_state(self, interface_id):
         data = self.get_interface(interface_id)
         return data.get('state', '')
 
     def set_interface_state(self, interface_id, state):
@@ -453,7 +529,24 @@
 
     def get_pipeline_runs(self, connection_id=None, page=1, per_page=10):
         if connection_id:
             url = f"{self.BACKEND_URL}/api/servers/{connection_id}/runs/?page={page}&per_page={per_page}"
         else:
             url = f"{self.BACKEND_URL}/api/pipeline_runs/?page={page}&per_page={per_page}"
         return self.call_backend("get", url)
+
+    def get_interface_runs(self, interface_id=None, page=1, per_page=10):
+        url = f"{self.BACKEND_URL}/api/interface_runs/?interface_id={interface_id}&page={page}&per_page={per_page}"
+        return self.call_backend("GET", url)
+
+    def send_connection_invite(self, recipient, subject, message, confirmation_recipient, server_type):
+        data = {
+            'recipient': recipient,
+            'subject': subject,
+            'message': message,
+            'confirmationRecipient': confirmation_recipient,
+            'serverType': server_type,
+        }
+
+        url = f"{self.BACKEND_URL}/api/servers/invite/"
+
+        return self.call_backend("POST", url, expected_status_code=204, json=data)
```

### Comparing `Peliqan-1.6.3/peliqan/client/base.py` & `Peliqan-1.7.0/peliqan/client/base.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.3/peliqan/client/dbclient.py` & `Peliqan-1.7.0/peliqan/client/dbclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,22 @@
             "action": action,
             "kwargs": kwargs
         }
 
         url = f"{self.BACKEND_URL}/api/proxy/db/"
         return self.call_backend('post', url, json=payload)
 
+    def create_schema(self, db_name, schema_name):
+        response = self.db_via_proxy(db_name, schema_name, None, None, 'create_schema')
+        return response
+
+    def create_table(self, db_name, schema_name, table_name, fields=None, pk=None):
+        response = self.db_via_proxy(db_name, schema_name, table_name, pk, 'create_table', fields=fields)
+        return response
+
     def insert(self, db_name, schema_name, table_name, *args, **kwargs):
         # allow using both keyword arguments or a dict as argument:
         # pq.insert("my_db", "my_table", name='John', city='NY') or pq.insert("my_db", "my_table", contact_obj)
         kwargs = self.args_to_kwargs(args, kwargs)
         response = self.db_via_proxy(db_name, schema_name, table_name, None, 'insert', **kwargs)
         return response
 
@@ -185,14 +193,20 @@
         response = self.db_via_proxy(db_name, schema_name, table_name, pk, 'write_records', **kwargs)
         return response
 
 
 class PeliqanTrinoDBClient(DBClient):
     is_trino = True
 
+    def create_schema(self, db_name, schema_name):
+        raise OperationNotSupported("'create_schema' operation is not support by Peliqan Trino")
+
+    def create_table(self, db_name, schema_name, table_name, fields=None, pk=None):
+        raise OperationNotSupported("'create_table' operation is not support by Peliqan Trino")
+
     def insert(self, db_name, schema_name, table_name, *args, **kwargs):
         raise OperationNotSupported("'insert' operation is not support by Peliqan Trino")
 
     def update(self, db_name, schema_name, table_name, pk=empty, *args, **kwargs):
         raise OperationNotSupported("'update' operation is not support by Peliqan Trino")
 
     def upsert(self, db_name, schema_name, table_name, pk=empty, *args, **kwargs):
```

### Comparing `Peliqan-1.6.3/peliqan/client/sftpclient.py` & `Peliqan-1.7.0/peliqan/client/sftpclient.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.3/peliqan/client/writeback.py` & `Peliqan-1.7.0/peliqan/client/writeback.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.3/peliqan/core.py` & `Peliqan-1.7.0/peliqan/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -183,51 +183,57 @@
                     'detail': 'The sync task has completed.',
                     'syncing': False
                 }
 
             time.sleep(interval)
             count += 1
 
+    def _refresh_connection(self, base_url, connection_id, connection_name, is_async):
+        response = self.__service_client__.refresh_resource(
+            resource_type='connection',
+            refresh_baseurl=base_url,
+            resource_name=connection_name,
+            resource_id=connection_id
+        )
+
+        if not is_async:
+            response = self._retry_get_resource_status(
+                lambda: self.get_refresh_connection_status(
+                    connection_name=connection_name,
+                    connection_id=connection_id,
+                    task_id=response.get('task_id'))
+            )
+
+        return response
+
     def run_pipeline(self, connection_name=None, connection_id=None, tables=None, is_async=True):
-        return self.refresh_connection(
-            connection_name,
-            connection_id,
-            tables,
-            is_async,
-            only_pipelines=True
+        if not isinstance(tables, (list, tuple, type(None))):
+            tables = [tables]
+
+        tables = ','.join(table for table in tables) if tables else ""
+        pipeline = "true"
+
+        base_url = (
+            f"{self.BACKEND_URL}/api/servers/%s/syncdb/?pipeline={pipeline}&tables={tables}"
         )
 
+        return self._refresh_connection(base_url, connection_id, connection_name, is_async)
+
     def refresh_connection(
         self,
         connection_name=None,
         connection_id=None,
-        tables=None,
         is_async=True,
-        only_pipelines=False
     ):
-        if not isinstance(tables, (list, tuple, type(None))):
-            tables = [tables]
-
-        tables = ','.join(table for table in tables) if tables else ""
-
-        pipeline = "true" if only_pipelines else "false"
 
         base_url = (
-            f"{self.BACKEND_URL}/api/servers/%s/syncdb/?pipeline={pipeline}&tables={tables}"
+            f"{self.BACKEND_URL}/api/servers/%s/syncdb/"
         )
-        response = self.__service_client__.refresh_resource(resource_type='connection', refresh_baseurl=base_url,
-                                                            resource_name=connection_name, resource_id=connection_id)
 
-        if not is_async:
-            response = self._retry_get_resource_status(
-                lambda: self.get_refresh_connection_status(connection_name=connection_name, connection_id=connection_id,
-                                                           task_id=response.get('task_id'))
-            )
-
-        return response
+        return self._refresh_connection(base_url, connection_id, connection_name, is_async)
 
     def refresh_database(self, connection_name=None, database_name=None, database_id=None, is_async=True):
         base_url = f"{self.BACKEND_URL}/api/applications/%s/syncdb/"
         response = self.__service_client__.refresh_resource(resource_type='database', refresh_baseurl=base_url,
                                                             resource_name=database_name, resource_id=database_id,
                                                             connection_name=connection_name)
 
@@ -425,27 +431,43 @@
         try:
             change_id = int(change_id)
         except ValueError:
             raise PeliqanClientException("change_id must be a valid integer")
 
         return self.__service_client__.update_writeback_status(table_id, change_id, writeback_status)
 
+    def list_connections(self):
+        """
+        Returns a list of servers in the account.
+
+        :return: list of databases
+        """
+        return self.__service_client__.list_servers()
+
     def list_databases(self):
         """
         Returns a list of all databases in the account including tables and fields in tables.
 
         :return: list of databases
         """
         return self.__service_client__.list_databases()
 
+    def get_schema(self, schema_id):
+        """
+        Returns all meta-data for a schema.
+
+        :return: schema meta-data
+        """
+        return self.__service_client__.get_schema(schema_id)
+
     def get_table(self, table_id):
         """
-            Returns all meta-data for a table including fields.
+        Returns all meta-data for a table including fields.
 
-            :return: list of databases
+        :return: table meta-data
         """
         return self.__service_client__.get_table(table_id)
 
     def update_field(self, field_id, description=None, tags=None):
         """
         Updates a field (column).
 
@@ -453,44 +475,74 @@
         :param description: optional, string, description of the field (data catalog metadata)
         :param tags: optional, array of strings, tags assigned to the field (data catalog metadata)
         :return: result of update
         """
 
         return self.__service_client__.update_field_metadata(field_id, description, tags)
 
-    def update_table(self, table_id, name=None, query=None, primary_field_id=None,
-                     settings=None,
-                     description=None, tags=None):
+    def update_table(
+        self,
+        table_id,
+        name=None,
+        query=None,
+        primary_field_id=None,
+        settings=None,
+        description=None,
+        tags=None,
+        run_on_peliqan_trino=empty,
+        materialize=empty
+    ):
         """
         Updates a table.
 
         :param table_id: required, integer, id of the table to update
         :param name: optional, string, new name of the table
         :param query: optional, string, new SQL query for tables of type 'query'
         :param primary_field_id: optional, integer, primary key field id for this table, i.e. the field id in Peliqan.
         See, table details page in Peliqan to get the primary_field_id for a table.
         :param settings: optional, string (json), settings of the table
         :param description: optional, string, description of the table (data catalog metadata)
         :param tags: optional, array of strings, tags assigned to the table (data catalog metadata)
+        :param run_on_peliqan_trino: optional, boolean, whether the query should run on the native engine or trino engine.
+        :param materialize: optional, boolean,  whether the query should be materialized as a table into a database.
+
         :return: result of update
         """
 
         update_result_dict = {}
         update_metadata_result_dict = {}
         if name or query or settings:
-            update_result_dict = self.__service_client__.update_table(table_id, name, query, settings)
+            update_result_dict = self.__service_client__.update_table(
+                table_id,
+                name,
+                query,
+                settings,
+                run_on_peliqan_trino,
+                materialize
+            )
         if description or tags or primary_field_id:
             update_metadata_result_dict = self.__service_client__.update_table_metadata(
                 table_id,
                 description,
                 tags,
                 primary_field_id
             )
         return {**update_result_dict, **update_metadata_result_dict}
 
+    def update_schema(self, schema_id, name):
+        """
+        Updates a schema.
+
+        :param schema_id: required, integer, id of the schema to update
+        :param name: required, new name of the schema
+        :return: result of update
+        """
+
+        return self.__service_client__.update_schema(schema_id, name)
+
     def update_database(self, database_id, description=None, tags=None):
         """
         Updates a database.
 
         :param database_id: required, integer, id of the database to update
         :param description: optional, string, description of the database (data catalog metadata)
         :param tags: optional, array of strings, tags assigned to the database (data catalog metadata)
@@ -547,31 +599,49 @@
             raw_script=raw_script,
             settings=settings,
             state=state,
             flow=flow,
             editor=editor
         )
 
-    def add_script(self, group_id, name=empty, script_type=empty, run_mode=empty):
+    def add_script(self, group_id, name, run_mode='STREAMLIT', script_type='streamlit'):
         """
 
         :param group_id: The group the script will belong to.
         :param name: The name of the new script.
         :param script_type: An enum value that decides the type of script. Options: [streamlit]
         :param run_mode:  An enum value that decides whether the script will be triggered by an API or a streamlit app.
-        Options: [STREAMLIT, API]
+        Options: [STREAMLIT, API, SHELL]
         :return:
         """
         return self.__service_client__.create_interface(
             group_id,
             name=name,
             type=script_type,
             run_mode=run_mode
         )
 
+    def add_query_table(
+        self,
+        name,
+        query,
+        database_id=None,
+        schema_id=None,
+        run_on_peliqan_trino=empty,
+        materialize=empty,
+    ):
+        return self.__service_client__.create_query(
+            name=name,
+            query=query,
+            database_id=database_id,
+            schema_id=schema_id,
+            run_on_peliqan_trino=run_on_peliqan_trino,
+            materialize=materialize
+        )
+
     def generate_sql_union(self, table_ids, sources=None):
         """
         Generates an SQL UNION query for the given tables.
         All columns of all tables will be added to the UNION query.
         If a column does not exist in one of the tables, it will be added with a null value.
         Optionally, a "source" column can be added to indicate from which table each row originated.
 
@@ -675,7 +745,83 @@
 
         :param connection_id: integer, id of the source connection.
         :param page: integer, the page number to fetch.
         :param per_page: integer, the number of results per page.
         :return: list of pipeline runs
         """
         return self.__service_client__.get_pipeline_runs(connection_id, page, per_page)
+
+    def get_script_runs(self, script_id=None, page=1, per_page=10):
+        return self.__service_client__.get_interface_runs(script_id, page, per_page)
+
+    def send_connection_invite(
+        self,
+        recipient,
+        subject,
+        message,
+        confirmation_recipient,
+        server_type
+    ):
+
+        return self.__service_client__.send_connection_invite(
+            recipient,
+            subject,
+            message,
+            confirmation_recipient,
+            server_type
+        )
+
+    def get_or_create_schema(self, database_id, schema_name):
+        try:
+            url = f"{self.BACKEND_URL}/api/database/schemas/database/{database_id}/"
+            response = self.__service_client__.call_backend("POST", url, json={'schema_name': schema_name})
+        except PeliqanClientException as e:
+            if 'ERROR_SCHEMA_ALREADY_EXISTS' not in str(e):
+                raise
+            response = self.__service_client__.find_schema(database_id=database_id, schema_name=schema_name)
+            schema_id = response.get('schema_id')
+            if schema_id:
+                response = self.get_schema(schema_id)
+
+        return response
+
+    def get_or_create_query_table(
+        self,
+        name,
+        query,
+        database_id=None,
+        schema_id=None,
+        run_on_peliqan_trino=empty,
+        materialize=empty
+    ):
+        try:
+            response = self.__service_client__.find_table_or_field(
+                database_id=database_id,
+                schema_id=schema_id,
+                table_name=name
+            )
+
+            table_id = response.get('table_id')
+            if table_id:
+                response = self.get_table(table_id)
+
+        except PeliqanClientException as e:
+            if 'ERROR_TABLE_DOES_NOT_EXIST' not in str(e):
+                raise
+
+            response = self.add_query_table(
+                name,
+                query,
+                database_id=database_id,
+                schema_id=schema_id,
+                run_on_peliqan_trino=run_on_peliqan_trino,
+                materialize=materialize,
+            )
+
+        return response
+
+    def discover_object_schema(self, records):
+        if not isinstance(records, (list, tuple)):
+            records = [records]
+
+        url = f"{self.BACKEND_URL}/api/database/resource/json-schema/"
+        return self.__service_client__.call_backend("POST", url, json={'records': records})
```

### Comparing `Peliqan-1.6.3/peliqan/local_test.py` & `Peliqan-1.7.0/peliqan/local_test.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.3/peliqan/utils.py` & `Peliqan-1.7.0/peliqan/utils.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.3/setup.py` & `Peliqan-1.7.0/setup.py`

 * *Files identical despite different names*

