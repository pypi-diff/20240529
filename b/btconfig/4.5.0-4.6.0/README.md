# Comparing `tmp/btconfig-4.5.0.tar.gz` & `tmp/btconfig-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btconfig-4.5.0.tar", last modified: Wed Jul 19 23:50:24 2023, max compression
+gzip compressed data, was "btconfig-4.6.0.tar", last modified: Wed May 29 20:55:18 2024, max compression
```

## Comparing `btconfig-4.5.0.tar` & `btconfig-4.6.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-19 23:50:24.567035 btconfig-4.5.0/
--rw-r--r--   0 etejeda    (501) staff       (20)     1311 2023-01-09 20:02:16.000000 btconfig-4.5.0/.gitignore
--rw-r--r--   0 etejeda    (501) staff       (20)      175 2023-01-09 20:02:16.000000 btconfig-4.5.0/AUTHORS.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     1097 2023-01-09 20:02:16.000000 btconfig-4.5.0/LICENSE
--rw-r--r--   0 etejeda    (501) staff       (20)      344 2023-01-09 20:02:16.000000 btconfig-4.5.0/MANIFEST.in
--rw-r--r--   0 etejeda    (501) staff       (20)     3796 2023-07-19 23:50:24.567333 btconfig-4.5.0/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     3132 2023-05-11 11:53:49.000000 btconfig-4.5.0/README.md
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-19 23:50:24.555460 btconfig-4.5.0/btconfig/
--rw-r--r--   0 etejeda    (501) staff       (20)     1267 2023-05-11 11:55:36.000000 btconfig-4.5.0/btconfig/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     3788 2023-05-14 18:16:20.000000 btconfig-4.5.0/btconfig/configloader.py
--rw-r--r--   0 etejeda    (501) staff       (20)     3217 2023-07-18 23:18:47.000000 btconfig-4.5.0/btconfig/configutils.py
--rw-r--r--   0 etejeda    (501) staff       (20)      897 2023-06-09 20:13:17.000000 btconfig-4.5.0/btconfig/logger.py
--rw-r--r--   0 etejeda    (501) staff       (20)     4695 2023-07-19 22:26:14.000000 btconfig-4.5.0/btconfig/superconf.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-19 23:50:24.559449 btconfig-4.5.0/btconfig.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)     3796 2023-07-19 23:50:24.000000 btconfig-4.5.0/btconfig.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      604 2023-07-19 23:50:24.000000 btconfig-4.5.0/btconfig.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-07-19 23:50:24.000000 btconfig-4.5.0/btconfig.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-15 01:07:02.000000 btconfig-4.5.0/btconfig.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)       78 2023-07-19 23:50:24.000000 btconfig-4.5.0/btconfig.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        9 2023-07-19 23:50:24.000000 btconfig-4.5.0/btconfig.egg-info/top_level.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-19 23:50:24.566449 btconfig-4.5.0/examples/
--rw-r--r--   0 etejeda    (501) staff       (20)     3045 2023-05-11 11:53:23.000000 btconfig-4.5.0/examples/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)      157 2023-05-11 11:53:25.000000 btconfig-4.5.0/examples/example1.py
--rw-r--r--   0 etejeda    (501) staff       (20)      170 2023-05-11 11:53:22.000000 btconfig-4.5.0/examples/example2.py
--rw-r--r--   0 etejeda    (501) staff       (20)      160 2023-05-11 11:53:23.000000 btconfig-4.5.0/examples/example3.py
--rw-r--r--   0 etejeda    (501) staff       (20)      189 2023-05-11 11:53:24.000000 btconfig-4.5.0/examples/example4.py
--rw-r--r--   0 etejeda    (501) staff       (20)       54 2023-01-09 20:02:16.000000 btconfig-4.5.0/examples/myconfig1.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      234 2023-01-09 20:02:16.000000 btconfig-4.5.0/examples/myconfig2.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      435 2023-01-09 20:02:16.000000 btconfig-4.5.0/examples/myconfig3.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      208 2023-01-09 20:02:16.000000 btconfig-4.5.0/examples/myconfig4.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-01-09 20:02:16.000000 btconfig-4.5.0/requirements.txt
--rw-r--r--   0 etejeda    (501) staff       (20)     1074 2023-07-19 23:50:24.568519 btconfig-4.5.0/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)       36 2023-01-09 20:02:16.000000 btconfig-4.5.0/setup.py
--rw-r--r--   0 etejeda    (501) staff       (20)      248 2023-05-11 11:54:41.000000 btconfig-4.5.0/test.py
--rw-r--r--   0 etejeda    (501) staff       (20)      315 2023-01-09 20:02:16.000000 btconfig-4.5.0/tox.ini
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-29 20:55:18.283119 btconfig-4.6.0/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1311 2023-01-09 20:02:16.000000 btconfig-4.6.0/.gitignore
+-rw-r--r--   0 etejeda    (501) staff       (20)      175 2023-01-09 20:02:16.000000 btconfig-4.6.0/AUTHORS.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     1097 2023-01-09 20:02:16.000000 btconfig-4.6.0/LICENSE
+-rw-r--r--   0 etejeda    (501) staff       (20)      344 2023-01-09 20:02:16.000000 btconfig-4.6.0/MANIFEST.in
+-rw-r--r--   0 etejeda    (501) staff       (20)     3796 2024-05-29 20:55:18.283764 btconfig-4.6.0/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     3132 2023-05-11 11:53:49.000000 btconfig-4.6.0/README.md
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-29 20:55:18.272467 btconfig-4.6.0/btconfig/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1342 2024-05-29 19:13:15.000000 btconfig-4.6.0/btconfig/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     3944 2024-05-29 19:13:15.000000 btconfig-4.6.0/btconfig/configloader.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     3217 2023-07-18 23:18:47.000000 btconfig-4.6.0/btconfig/configutils.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      897 2023-06-09 20:13:17.000000 btconfig-4.6.0/btconfig/logger.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     4695 2023-07-19 22:26:14.000000 btconfig-4.6.0/btconfig/superconf.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-29 20:55:18.275649 btconfig-4.6.0/btconfig.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3796 2024-05-29 20:55:17.000000 btconfig-4.6.0/btconfig.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)      604 2024-05-29 20:55:18.000000 btconfig-4.6.0/btconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2024-05-29 20:55:17.000000 btconfig-4.6.0/btconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-15 01:07:02.000000 btconfig-4.6.0/btconfig.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)       78 2024-05-29 20:55:17.000000 btconfig-4.6.0/btconfig.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        9 2024-05-29 20:55:17.000000 btconfig-4.6.0/btconfig.egg-info/top_level.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-29 20:55:18.282177 btconfig-4.6.0/examples/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3045 2023-05-11 11:53:23.000000 btconfig-4.6.0/examples/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)      157 2023-05-11 11:53:25.000000 btconfig-4.6.0/examples/example1.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      170 2023-05-11 11:53:22.000000 btconfig-4.6.0/examples/example2.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      160 2023-05-11 11:53:23.000000 btconfig-4.6.0/examples/example3.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      189 2023-05-11 11:53:24.000000 btconfig-4.6.0/examples/example4.py
+-rw-r--r--   0 etejeda    (501) staff       (20)       54 2023-01-09 20:02:16.000000 btconfig-4.6.0/examples/myconfig1.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      234 2023-01-09 20:02:16.000000 btconfig-4.6.0/examples/myconfig2.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      435 2023-01-09 20:02:16.000000 btconfig-4.6.0/examples/myconfig3.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      208 2023-01-09 20:02:16.000000 btconfig-4.6.0/examples/myconfig4.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-01-09 20:02:16.000000 btconfig-4.6.0/requirements.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)     1074 2024-05-29 20:55:18.288091 btconfig-4.6.0/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)       36 2023-01-09 20:02:16.000000 btconfig-4.6.0/setup.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      248 2023-05-11 11:54:41.000000 btconfig-4.6.0/test.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      315 2023-01-09 20:02:16.000000 btconfig-4.6.0/tox.ini
```

### Comparing `btconfig-4.5.0/.gitignore` & `btconfig-4.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `btconfig-4.5.0/LICENSE` & `btconfig-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `btconfig-4.5.0/PKG-INFO` & `btconfig-4.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btconfig
-Version: 4.5.0
+Version: 4.6.0
 Summary: Module for reading configuration files
 Home-page: https://github.com/berttejeda/bert.config
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btconfig-4.5.0/README.md` & `btconfig-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `btconfig-4.5.0/btconfig/__init__.py` & `btconfig-4.6.0/btconfig/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,8 +24,9 @@
     self.failfast = kwargs.get('failfast',False)
     self.data_key = kwargs.get('data_key')
     self.templatized = kwargs.get('templatized')
     self.config_file_auth_username = kwargs.get('auth_username')
     self.config_file_auth_password = kwargs.get('auth_password')
     self.configs_already_processed = []
     self.default_value = kwargs.get('default_value', {})
+    self.warn_if_config_not_found = kwargs.get('warn_if_config_not_found')
```

### Comparing `btconfig-4.5.0/btconfig/configloader.py` & `btconfig-4.6.0/btconfig/configloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,11 +98,14 @@
             if self.failfast:
                 self.logger.error(
                     "Aborting due to invalid or not found \
                     config(s) [%s]" % ','.join(config_file_uris)
                 )
                 sys.exit(1)
             else:
-                logger.debug('No settings could be derived, using defaults')
+                if self.warn_if_config_not_found:
+                    logger.warn('No settings could be derived, using defaults')
+                else:
+                    logger.debug('No settings could be derived, using defaults')
                 config_data = self.default_value
 
         return config_data
```

### Comparing `btconfig-4.5.0/btconfig/configutils.py` & `btconfig-4.6.0/btconfig/configutils.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.5.0/btconfig/logger.py` & `btconfig-4.6.0/btconfig/logger.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.5.0/btconfig/superconf.py` & `btconfig-4.6.0/btconfig/superconf.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.5.0/btconfig.egg-info/PKG-INFO` & `btconfig-4.6.0/btconfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btconfig
-Version: 4.5.0
+Version: 4.6.0
 Summary: Module for reading configuration files
 Home-page: https://github.com/berttejeda/bert.config
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btconfig-4.5.0/btconfig.egg-info/SOURCES.txt` & `btconfig-4.6.0/btconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `btconfig-4.5.0/examples/README.md` & `btconfig-4.6.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `btconfig-4.5.0/setup.cfg` & `btconfig-4.6.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = btconfig
 author = Engelbert Tejeda
 author_email = berttejeda@gmail.com
 description = Module for reading configuration files
-version = 4.5.0
+version = 4.6.0
 url = https://github.com/berttejeda/bert.config
 keywords = 
 	yaml
 	configuration
 	config
 	file
 	python
```

