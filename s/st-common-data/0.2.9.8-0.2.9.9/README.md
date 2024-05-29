# Comparing `tmp/st_common_data-0.2.9.8.tar.gz` & `tmp/st_common_data-0.2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_common_data-0.2.9.8.tar", last modified: Wed Apr  3 14:34:36 2024, max compression
+gzip compressed data, was "st_common_data-0.2.9.9.tar", last modified: Wed Apr 10 17:21:07 2024, max compression
```

## Comparing `st_common_data-0.2.9.8.tar` & `st_common_data-0.2.9.9.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-03 14:34:36.219991 st_common_data-0.2.9.8/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1073 2022-04-19 17:26:26.000000 st_common_data-0.2.9.8/LICENCE
--rw-r--r--   0 bayraktar  (1000) bayraktar  (1000)     1224 2024-04-03 14:34:36.219991 st_common_data-0.2.9.8/PKG-INFO
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      648 2024-01-03 16:21:08.000000 st_common_data-0.2.9.8/README.md
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      103 2022-04-19 17:26:26.000000 st_common_data-0.2.9.8/pyproject.toml
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      669 2024-04-03 14:34:36.219991 st_common_data-0.2.9.8/setup.cfg
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-03 14:34:36.215991 st_common_data-0.2.9.8/st_common_data/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      143 2024-04-03 14:34:31.000000 st_common_data-0.2.9.8/st_common_data/__init__.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-03 14:34:36.215991 st_common_data-0.2.9.8/st_common_data/auth/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      443 2023-04-11 10:31:33.000000 st_common_data-0.2.9.8/st_common_data/auth/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      118 2022-12-07 11:03:09.000000 st_common_data-0.2.9.8/st_common_data/auth/apps.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10938 2024-03-18 12:37:09.000000 st_common_data-0.2.9.8/st_common_data/auth/django_auth.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10009 2023-04-18 06:48:02.000000 st_common_data-0.2.9.8/st_common_data/auth/fastapi_auth.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      386 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/auth/serializers.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      278 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/auth/urls.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4086 2024-01-11 11:51:04.000000 st_common_data-0.2.9.8/st_common_data/auth/views.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    34092 2024-04-03 14:26:00.000000 st_common_data-0.2.9.8/st_common_data/datum.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      398 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/pagination.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-03 14:34:36.215991 st_common_data-0.2.9.8/st_common_data/trading_accounts/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/__init__.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-03 14:34:36.219991 st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4299 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0001_initial.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      652 2023-02-24 09:24:45.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      456 2023-03-22 00:17:46.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0003_tradingaccount_personal_status.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      539 2023-11-20 18:32:49.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0004_tradingaccount_platform.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      541 2024-03-12 13:41:45.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0005_tradingaccount_routing.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     3625 2024-03-12 13:41:45.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/models.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      214 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/serializers.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      200 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/urls.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4193 2022-12-07 11:03:09.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/views.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-03 14:34:36.219991 st_common_data-0.2.9.8/st_common_data/utils/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-07-21 20:22:31.000000 st_common_data-0.2.9.8/st_common_data/utils/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4885 2024-01-03 17:13:10.000000 st_common_data-0.2.9.8/st_common_data/utils/common.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-03 14:34:36.219991 st_common_data-0.2.9.8/st_common_data.egg-info/
--rw-r--r--   0 bayraktar  (1000) bayraktar  (1000)     1224 2024-04-03 14:34:36.000000 st_common_data-0.2.9.8/st_common_data.egg-info/PKG-INFO
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1197 2024-04-03 14:34:36.000000 st_common_data-0.2.9.8/st_common_data.egg-info/SOURCES.txt
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        1 2024-04-03 14:34:36.000000 st_common_data-0.2.9.8/st_common_data.egg-info/dependency_links.txt
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)       15 2024-04-03 14:34:36.000000 st_common_data-0.2.9.8/st_common_data.egg-info/top_level.txt
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-10 17:21:07.673167 st_common_data-0.2.9.9/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1073 2022-04-19 17:26:26.000000 st_common_data-0.2.9.9/LICENCE
+-rw-r--r--   0 bayraktar  (1000) bayraktar  (1000)     1224 2024-04-10 17:21:07.673167 st_common_data-0.2.9.9/PKG-INFO
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      648 2024-01-03 16:21:08.000000 st_common_data-0.2.9.9/README.md
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      103 2022-04-19 17:26:26.000000 st_common_data-0.2.9.9/pyproject.toml
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      669 2024-04-10 17:21:07.673167 st_common_data-0.2.9.9/setup.cfg
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-10 17:21:07.665167 st_common_data-0.2.9.9/st_common_data/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      143 2024-04-10 17:19:44.000000 st_common_data-0.2.9.9/st_common_data/__init__.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-10 17:21:07.669167 st_common_data-0.2.9.9/st_common_data/auth/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      443 2023-04-11 10:31:33.000000 st_common_data-0.2.9.9/st_common_data/auth/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      118 2022-12-07 11:03:09.000000 st_common_data-0.2.9.9/st_common_data/auth/apps.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10938 2024-03-18 12:37:09.000000 st_common_data-0.2.9.9/st_common_data/auth/django_auth.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10009 2023-04-18 06:48:02.000000 st_common_data-0.2.9.9/st_common_data/auth/fastapi_auth.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      386 2022-08-23 10:22:22.000000 st_common_data-0.2.9.9/st_common_data/auth/serializers.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      278 2022-08-23 10:22:22.000000 st_common_data-0.2.9.9/st_common_data/auth/urls.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4086 2024-01-11 11:51:04.000000 st_common_data-0.2.9.9/st_common_data/auth/views.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    34092 2024-04-03 14:26:00.000000 st_common_data-0.2.9.9/st_common_data/datum.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      398 2022-08-23 10:22:22.000000 st_common_data-0.2.9.9/st_common_data/pagination.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-10 17:21:07.669167 st_common_data-0.2.9.9/st_common_data/trading_accounts/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.9.9/st_common_data/trading_accounts/__init__.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-10 17:21:07.669167 st_common_data-0.2.9.9/st_common_data/trading_accounts/migrations/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4299 2022-08-23 10:22:22.000000 st_common_data-0.2.9.9/st_common_data/trading_accounts/migrations/0001_initial.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      652 2023-02-24 09:24:45.000000 st_common_data-0.2.9.9/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      456 2023-03-22 00:17:46.000000 st_common_data-0.2.9.9/st_common_data/trading_accounts/migrations/0003_tradingaccount_personal_status.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      539 2023-11-20 18:32:49.000000 st_common_data-0.2.9.9/st_common_data/trading_accounts/migrations/0004_tradingaccount_platform.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      581 2024-04-10 17:17:25.000000 st_common_data-0.2.9.9/st_common_data/trading_accounts/migrations/0005_tradingaccount_routing.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      452 2024-04-10 17:19:44.000000 st_common_data-0.2.9.9/st_common_data/trading_accounts/migrations/0006_tradingaccount_bp_active.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.9.9/st_common_data/trading_accounts/migrations/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     3809 2024-04-10 17:17:37.000000 st_common_data-0.2.9.9/st_common_data/trading_accounts/models.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      214 2022-08-23 10:22:22.000000 st_common_data-0.2.9.9/st_common_data/trading_accounts/serializers.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      200 2022-08-23 10:22:22.000000 st_common_data-0.2.9.9/st_common_data/trading_accounts/urls.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4193 2022-12-07 11:03:09.000000 st_common_data-0.2.9.9/st_common_data/trading_accounts/views.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-10 17:21:07.673167 st_common_data-0.2.9.9/st_common_data/utils/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-07-21 20:22:31.000000 st_common_data-0.2.9.9/st_common_data/utils/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4885 2024-01-03 17:13:10.000000 st_common_data-0.2.9.9/st_common_data/utils/common.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-10 17:21:07.673167 st_common_data-0.2.9.9/st_common_data.egg-info/
+-rw-r--r--   0 bayraktar  (1000) bayraktar  (1000)     1224 2024-04-10 17:21:07.000000 st_common_data-0.2.9.9/st_common_data.egg-info/PKG-INFO
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1273 2024-04-10 17:21:07.000000 st_common_data-0.2.9.9/st_common_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        1 2024-04-10 17:21:07.000000 st_common_data-0.2.9.9/st_common_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)       15 2024-04-10 17:21:07.000000 st_common_data-0.2.9.9/st_common_data.egg-info/top_level.txt
```

### Comparing `st_common_data-0.2.9.8/LICENCE` & `st_common_data-0.2.9.9/LICENCE`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.8/PKG-INFO` & `st_common_data-0.2.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st_common_data
-Version: 0.2.9.8
+Version: 0.2.9.9
 Summary: Data that is used in different ST projects
 Home-page: https://github.com/ivanovds/st_common_data
 Author: Daniil Ivanov
 Author-email: danil.98and@gmail.com
 Project-URL: Bug Tracker, https://github.com/ivanovds/st_common_data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `st_common_data-0.2.9.8/README.md` & `st_common_data-0.2.9.9/README.md`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.8/setup.cfg` & `st_common_data-0.2.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.8/st_common_data/auth/django_auth.py` & `st_common_data-0.2.9.9/st_common_data/auth/django_auth.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.8/st_common_data/auth/fastapi_auth.py` & `st_common_data-0.2.9.9/st_common_data/auth/fastapi_auth.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.8/st_common_data/auth/views.py` & `st_common_data-0.2.9.9/st_common_data/auth/views.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.8/st_common_data/datum.py` & `st_common_data-0.2.9.9/st_common_data/datum.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0001_initial.py` & `st_common_data-0.2.9.9/st_common_data/trading_accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py` & `st_common_data-0.2.9.9/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0004_tradingaccount_platform.py` & `st_common_data-0.2.9.9/st_common_data/trading_accounts/migrations/0004_tradingaccount_platform.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0005_tradingaccount_routing.py` & `st_common_data-0.2.9.9/st_common_data/trading_accounts/migrations/0005_tradingaccount_routing.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,10 +9,12 @@
         ('trading_accounts', '0004_tradingaccount_platform'),
     ]
 
     operations = [
         migrations.AddField(
             model_name='tradingaccount',
             name='routing',
-            field=models.PositiveSmallIntegerField(blank=True, choices=[(0, 'TRAFIX'), (1, 'LYNX'), (2, 'STERLING'), (3, 'EMULATOR')], default=None, null=True, verbose_name='Routing'),
+            field=models.PositiveSmallIntegerField(
+                choices=[(0, 'TRAFIX'), (1, 'LYNX'), (2, 'STERLING'), (3, 'EMULATOR'), (4, 'VELOCITY'), (5, 'NON_SET')],
+                default=5, verbose_name='Routing'),
         ),
     ]
```

### Comparing `st_common_data-0.2.9.8/st_common_data/trading_accounts/models.py` & `st_common_data-0.2.9.9/st_common_data/trading_accounts/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,20 +64,24 @@
         (TRADING_APP, 'TRADING_APP'),
     )
 
     TRAFIX = 0
     LYNX = 1
     STERLING = 2
     EMULATOR = 3
+    VELOCITY = 4
+    NON_SET = 5
 
     ROUTING_CHOICES = (
         (TRAFIX, 'TRAFIX'),
         (LYNX, 'LYNX'),
         (STERLING, 'STERLING'),
         (EMULATOR, 'EMULATOR'),
+        (VELOCITY, 'VELOCITY'),
+        (NON_SET, 'NON_SET'),
     )
 
     fid = models.IntegerField(
         unique=True,
         verbose_name='Foreign ID')
 
     user = models.ForeignKey(
@@ -119,16 +123,19 @@
     personal_status = models.BooleanField(
         default=False,
         verbose_name='Is personal account')
     platform = models.PositiveSmallIntegerField(
         null=True, blank=True, default=None,
         choices=PLATFORM_CHOICES, verbose_name='Platform')
     routing = models.PositiveSmallIntegerField(
-        null=True, blank=True, default=None,
+        default=NON_SET,
         choices=ROUTING_CHOICES, verbose_name='Routing')
+    bp_active = models.BooleanField(
+        default=False,
+        verbose_name='Does it have not zero BP')
 
     created_by = models.ForeignKey(
         UserModel, on_delete=models.PROTECT,
         null=True, blank=True, default=None,
         related_name='created_by_user',
         verbose_name='Created by')
     created = models.DateTimeField(
```

### Comparing `st_common_data-0.2.9.8/st_common_data/trading_accounts/views.py` & `st_common_data-0.2.9.9/st_common_data/trading_accounts/views.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.8/st_common_data/utils/common.py` & `st_common_data-0.2.9.9/st_common_data/utils/common.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.8/st_common_data.egg-info/PKG-INFO` & `st_common_data-0.2.9.9/st_common_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st_common_data
-Version: 0.2.9.8
+Version: 0.2.9.9
 Summary: Data that is used in different ST projects
 Home-page: https://github.com/ivanovds/st_common_data
 Author: Daniil Ivanov
 Author-email: danil.98and@gmail.com
 Project-URL: Bug Tracker, https://github.com/ivanovds/st_common_data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `st_common_data-0.2.9.8/st_common_data.egg-info/SOURCES.txt` & `st_common_data-0.2.9.9/st_common_data.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -22,10 +22,11 @@
 st_common_data/trading_accounts/urls.py
 st_common_data/trading_accounts/views.py
 st_common_data/trading_accounts/migrations/0001_initial.py
 st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py
 st_common_data/trading_accounts/migrations/0003_tradingaccount_personal_status.py
 st_common_data/trading_accounts/migrations/0004_tradingaccount_platform.py
 st_common_data/trading_accounts/migrations/0005_tradingaccount_routing.py
+st_common_data/trading_accounts/migrations/0006_tradingaccount_bp_active.py
 st_common_data/trading_accounts/migrations/__init__.py
 st_common_data/utils/__init__.py
 st_common_data/utils/common.py
```

