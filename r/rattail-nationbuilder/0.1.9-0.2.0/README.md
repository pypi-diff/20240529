# Comparing `tmp/rattail-nationbuilder-0.1.9.tar.gz` & `tmp/rattail_nationbuilder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rattail-nationbuilder-0.1.9.tar", last modified: Wed Sep 13 01:52:43 2023, max compression
+gzip compressed data, was "rattail_nationbuilder-0.2.0.tar", last modified: Wed May 29 15:15:05 2024, max compression
```

## Comparing `rattail-nationbuilder-0.1.9.tar` & `rattail_nationbuilder-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-13 01:52:43.434260 rattail-nationbuilder-0.1.9/
--rw-r--r--   0 lance     (1000) lance     (1000)     1140 2023-09-13 01:52:21.000000 rattail-nationbuilder-0.1.9/CHANGELOG.md
--rw-r--r--   0 lance     (1000) lance     (1000)       83 2023-09-12 23:55:16.000000 rattail-nationbuilder-0.1.9/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     1005 2023-09-13 01:52:43.434260 rattail-nationbuilder-0.1.9/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      290 2023-05-05 18:32:20.000000 rattail-nationbuilder-0.1.9/README.md
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-13 01:52:43.434260 rattail-nationbuilder-0.1.9/rattail_nationbuilder/
--rw-r--r--   0 lance     (1000) lance     (1000)     1013 2023-05-05 19:43:26.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-09-13 01:52:24.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1246 2023-09-12 19:52:47.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/commands.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1592 2023-09-12 21:15:43.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/config.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-13 01:52:43.434260 rattail-nationbuilder-0.1.9/rattail_nationbuilder/db/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2023-09-12 19:32:53.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/db/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-13 01:52:43.434260 rattail-nationbuilder-0.1.9/rattail_nationbuilder/db/alembic/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-13 01:52:43.434260 rattail-nationbuilder-0.1.9/rattail_nationbuilder/db/alembic/versions/
--rw-r--r--   0 lance     (1000) lance     (1000)     6092 2023-09-12 23:11:13.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/db/alembic/versions/1e17031c4b3e_first_cache_tables.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4806 2023-09-13 01:23:53.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/db/alembic/versions/c3cb75afcae2_add_donations_cache_table.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-13 01:52:43.434260 rattail-nationbuilder-0.1.9/rattail_nationbuilder/db/model/
--rw-r--r--   0 lance     (1000) lance     (1000)     1064 2023-09-13 00:30:29.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/db/model/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4685 2023-09-13 01:48:57.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/db/model/nationbuilder.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-13 01:52:43.434260 rattail-nationbuilder-0.1.9/rattail_nationbuilder/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)      996 2023-09-12 19:37:07.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/importing/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1363 2023-09-13 00:32:11.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/importing/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5497 2023-09-13 01:52:01.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/importing/nationbuilder.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1648 2023-09-13 00:32:25.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/importing/versions.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-13 01:52:43.434260 rattail-nationbuilder-0.1.9/rattail_nationbuilder/nationbuilder/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2023-05-05 19:45:56.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/nationbuilder/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1088 2023-09-12 20:48:51.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/nationbuilder/util.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6628 2023-09-12 20:31:10.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder/nationbuilder/webapi.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-13 01:52:43.434260 rattail-nationbuilder-0.1.9/rattail_nationbuilder.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     1005 2023-09-13 01:52:43.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)     1064 2023-09-13 01:52:43.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-09-13 01:52:43.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      338 2023-09-13 01:52:43.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder.egg-info/entry_points.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        8 2023-09-13 01:52:43.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       22 2023-09-13 01:52:43.000000 rattail-nationbuilder-0.1.9/rattail_nationbuilder.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)     1160 2023-09-13 01:52:43.434260 rattail-nationbuilder-0.1.9/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     1017 2023-05-17 12:01:08.000000 rattail-nationbuilder-0.1.9/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:15:05.172639 rattail_nationbuilder-0.2.0/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1663 2024-05-29 15:14:11.000000 rattail_nationbuilder-0.2.0/CHANGELOG.md
+-rw-r--r--   0 lance     (1000) lance     (1000)       83 2023-09-12 23:55:16.000000 rattail_nationbuilder-0.2.0/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     1005 2024-05-29 15:15:05.172639 rattail_nationbuilder-0.2.0/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      290 2023-05-05 18:32:20.000000 rattail_nationbuilder-0.2.0/README.md
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:15:05.172639 rattail_nationbuilder-0.2.0/rattail_nationbuilder/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1013 2023-05-05 19:43:26.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2024-05-29 15:14:03.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1970 2023-09-14 18:21:04.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/app.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1880 2024-05-17 01:12:28.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/commands.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1592 2023-09-12 21:15:43.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/config.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:15:05.172639 rattail_nationbuilder-0.2.0/rattail_nationbuilder/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2023-09-12 19:32:53.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/db/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:15:05.172639 rattail_nationbuilder-0.2.0/rattail_nationbuilder/db/alembic/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:15:05.172639 rattail_nationbuilder-0.2.0/rattail_nationbuilder/db/alembic/versions/
+-rw-r--r--   0 lance     (1000) lance     (1000)     6092 2023-09-12 23:11:13.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/db/alembic/versions/1e17031c4b3e_first_cache_tables.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      805 2023-09-13 14:13:52.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/db/alembic/versions/7fc3dee0e9c5_fix_nullable.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4806 2023-09-13 01:23:53.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/db/alembic/versions/c3cb75afcae2_add_donations_cache_table.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:15:05.172639 rattail_nationbuilder-0.2.0/rattail_nationbuilder/db/model/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1064 2023-09-13 00:30:29.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/db/model/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4673 2023-09-13 14:12:16.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/db/model/nationbuilder.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:15:05.172639 rattail_nationbuilder-0.2.0/rattail_nationbuilder/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)      996 2023-09-12 19:37:07.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/importing/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1363 2023-09-13 00:32:11.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/importing/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5628 2023-10-16 16:08:22.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/importing/nationbuilder.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1648 2023-09-13 00:32:25.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/importing/versions.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:15:05.172639 rattail_nationbuilder-0.2.0/rattail_nationbuilder/nationbuilder/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2023-05-05 19:45:56.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/nationbuilder/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1325 2023-09-14 18:14:23.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/nationbuilder/util.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6794 2023-10-16 16:11:54.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder/nationbuilder/webapi.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:15:05.172639 rattail_nationbuilder-0.2.0/rattail_nationbuilder.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1005 2024-05-29 15:15:05.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)     1164 2024-05-29 15:15:05.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-05-29 15:15:05.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      514 2024-05-29 15:15:05.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder.egg-info/entry_points.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        8 2024-05-29 15:15:05.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       22 2024-05-29 15:15:05.000000 rattail_nationbuilder-0.2.0/rattail_nationbuilder.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1338 2024-05-29 15:15:05.172639 rattail_nationbuilder-0.2.0/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     1017 2023-05-17 12:01:08.000000 rattail_nationbuilder-0.2.0/setup.py
```

### Comparing `rattail-nationbuilder-0.1.9/CHANGELOG.md` & `rattail_nationbuilder-0.2.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,38 @@
 
 # Changelog
 All notable changes to rattail-nationbuilder will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.2.0] - 2024-05-29
+### Changed
+- Migrate all commands to use `typer`.
+
+## [0.1.14] - 2023-12-01
+### Changed
+- Update subcommand entry point group names, per wuttjamaican.
+
+## [0.1.13] - 2023-09-16
+### Changed
+- Limit page size to 100, for fetching Person records from NB API.
+
+## [0.1.12] - 2023-09-15
+### Changed
+- Add rattail provider for NationBuilder integration.
+
+## [0.1.11] - 2023-09-13
+### Changed
+- Fix schema inconsistencies.
+
+## [0.1.10] - 2023-09-12
+### Changed
+- Assume null if NB person tags are empty.
+
 ## [0.1.9] - 2023-09-12
 ### Changed
 - Add cache table, importer for NationBuilder donations.
 
 ## [0.1.8] - 2023-09-12
 ### Changed
 - Fix manifest again..omg.
```

### Comparing `rattail-nationbuilder-0.1.9/PKG-INFO` & `rattail_nationbuilder-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-nationbuilder
-Version: 0.1.9
+Version: 0.2.0
 Summary: Rattail integration package for NationBuilder
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder/__init__.py` & `rattail_nationbuilder-0.2.0/rattail_nationbuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder/commands.py` & `rattail_nationbuilder-0.2.0/rattail_nationbuilder/importing/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,20 +17,11 @@
 #  details.
 #
 #  You should have received a copy of the GNU General Public License along with
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
-rattail-nationbuilder commands
+rattail-nationbuilder importing
 """
 
-from rattail import commands
-
-
-class ImportNationBuilder(commands.ImportSubcommand):
-    """
-    Import data for NationBuilder => Rattail
-    """
-    name = 'import-nationbuilder'
-    description = __doc__.strip()
-    handler_key = 'to_rattail.from_nationbuilder.import'
+from . import model
```

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder/config.py` & `rattail_nationbuilder-0.2.0/rattail_nationbuilder/config.py`

 * *Files identical despite different names*

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder/db/alembic/versions/1e17031c4b3e_first_cache_tables.py` & `rattail_nationbuilder-0.2.0/rattail_nationbuilder/db/alembic/versions/1e17031c4b3e_first_cache_tables.py`

 * *Files identical despite different names*

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder/db/alembic/versions/c3cb75afcae2_add_donations_cache_table.py` & `rattail_nationbuilder-0.2.0/rattail_nationbuilder/db/alembic/versions/c3cb75afcae2_add_donations_cache_table.py`

 * *Files identical despite different names*

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder/db/model/__init__.py` & `rattail_nationbuilder-0.2.0/rattail_nationbuilder/db/model/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder/db/model/nationbuilder.py` & `rattail_nationbuilder-0.2.0/rattail_nationbuilder/db/model/nationbuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     model_title_plural = "NationBuilder People"
 
     uuid = model.uuid_column()
 
     id = sa.Column(sa.Integer(), nullable=False)
     signup_type = sa.Column(sa.Integer(), nullable=True)
     external_id = sa.Column(sa.String(length=50), nullable=True)
-    tags = sa.Column(sa.String(length=255), nullable=True)
+    tags = sa.Column(sa.Text(), nullable=True)
     first_name = sa.Column(sa.String(length=100), nullable=True)
     middle_name = sa.Column(sa.String(length=100), nullable=True)
     last_name = sa.Column(sa.String(length=100), nullable=True)
     email = sa.Column(sa.String(length=255), nullable=True)
     email_opt_in = sa.Column(sa.Boolean(), nullable=True)
     mobile = sa.Column(sa.String(length=50), nullable=True)
     mobile_opt_in = sa.Column(sa.Boolean(), nullable=True)
```

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder/importing/__init__.py` & `rattail_nationbuilder-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,11 +17,13 @@
 #  details.
 #
 #  You should have received a copy of the GNU General Public License along with
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
-rattail-nationbuilder importing
+rattail-nationbuilder setup script
 """
 
-from . import model
+from setuptools import setup
+
+setup()
```

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder/importing/model.py` & `rattail_nationbuilder-0.2.0/rattail_nationbuilder/importing/model.py`

 * *Files identical despite different names*

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder/importing/nationbuilder.py` & `rattail_nationbuilder-0.2.0/rattail_nationbuilder/importing/nationbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,16 @@
         'primary_image_url_ssl',
         'signup_type',
         'tags',
         'updated_at',
     ] + primary_address_fields
 
     def get_host_objects(self):
-        return self.nationbuilder.get_people(page_size=500)
+        return self.nationbuilder.get_people(page_size=100,
+                                             progress=self.progress)
 
     def normalize_host_object(self, person):
 
         # nb. some fields may not be present in person dict
         data = dict([(field, person.get(field))
                      for field in self.fields])
         if data:
@@ -115,14 +116,16 @@
             for field in ('created_at', 'updated_at'):
                 data[field] = self.normalize_timestamp(data[field])
 
             if 'tags' in self.fields:
                 tags = data['tags']
                 if tags:
                     data['tags'] = self.config.make_list_string(tags)
+                else:
+                    data['tags'] = None
 
             if self.fields_active(self.primary_address_fields):
                 address = person.get('primary_address')
                 if address:
                     data.update({
                         'primary_address_address1': address['address1'],
                         'primary_address_address2': address['address2'],
```

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder/importing/versions.py` & `rattail_nationbuilder-0.2.0/rattail_nationbuilder/importing/versions.py`

 * *Files identical despite different names*

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder/nationbuilder/util.py` & `rattail_nationbuilder-0.2.0/rattail_nationbuilder/nationbuilder/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,12 +20,18 @@
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
 NationBuilder utils
 """
 
+import warnings
+
 
 def get_nationbuilder_url(config):
-    url = config.get('nationbuilder', 'url')
-    if url:
-        return url.rstrip('/')
+    warnings.warn("get_nationbuilder_url() function is deprecated; "
+                  "please use nationbuilder_handler.get_url() instead",
+                  DeprecationWarning, stacklevel=2)
+
+    app = config.get_app()
+    nationbuilder = app.get_nationbuilder_handler()
+    return nationbuilder.get_url()
```

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder/nationbuilder/webapi.py` & `rattail_nationbuilder-0.2.0/rattail_nationbuilder/nationbuilder/webapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,14 +91,18 @@
 
     def get_people(self, page_size=10, max_pages=None, progress=None, **kwargs):
         """
         Retrieve all Person records.
 
         https://apiexplorer.nationbuilder.com/nationbuilder#People
         """
+        # nb. found this limit in practice, but it is not documented?!
+        if page_size > 100:
+            raise ValueError("page_size cannot be more than 100")
+
         response = self.get('/api/v1/people/count')
         count = response.json()['people_count']
         pages = count // page_size
         if count % page_size:
             pages += 1
 
         url = {'next': '/api/v1/people?limit={}'.format(page_size)}
```

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder.egg-info/PKG-INFO` & `rattail_nationbuilder-0.2.0/rattail_nationbuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-nationbuilder
-Version: 0.1.9
+Version: 0.2.0
 Summary: Rattail integration package for NationBuilder
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rattail-nationbuilder-0.1.9/rattail_nationbuilder.egg-info/SOURCES.txt` & `rattail_nationbuilder-0.2.0/rattail_nationbuilder.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 CHANGELOG.md
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 rattail_nationbuilder/__init__.py
 rattail_nationbuilder/_version.py
+rattail_nationbuilder/app.py
 rattail_nationbuilder/commands.py
 rattail_nationbuilder/config.py
 rattail_nationbuilder.egg-info/PKG-INFO
 rattail_nationbuilder.egg-info/SOURCES.txt
 rattail_nationbuilder.egg-info/dependency_links.txt
 rattail_nationbuilder.egg-info/entry_points.txt
 rattail_nationbuilder.egg-info/requires.txt
 rattail_nationbuilder.egg-info/top_level.txt
 rattail_nationbuilder/db/__init__.py
 rattail_nationbuilder/db/alembic/versions/1e17031c4b3e_first_cache_tables.py
+rattail_nationbuilder/db/alembic/versions/7fc3dee0e9c5_fix_nullable.py
 rattail_nationbuilder/db/alembic/versions/c3cb75afcae2_add_donations_cache_table.py
 rattail_nationbuilder/db/model/__init__.py
 rattail_nationbuilder/db/model/nationbuilder.py
 rattail_nationbuilder/importing/__init__.py
 rattail_nationbuilder/importing/model.py
 rattail_nationbuilder/importing/nationbuilder.py
 rattail_nationbuilder/importing/versions.py
```

