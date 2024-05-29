# Comparing `tmp/tap-taboola-0.2.1.tar.gz` & `tmp/tap_taboola-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-taboola-0.2.1.tar", last modified: Tue Apr 30 20:31:45 2019, max compression
+gzip compressed data, was "tap_taboola-0.3.1.tar", last modified: Wed May 29 12:24:24 2024, max compression
```

## Comparing `tap-taboola-0.2.1.tar` & `tap_taboola-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4940 2018-11-09 20:03:04.000000 tap-taboola-0.2.1/tap_taboola/schemas.py
--rwxrwxr-x   0 vagrant   (1000) vagrant   (1000)    10933 2019-04-30 20:30:45.000000 tap-taboola-0.2.1/tap_taboola/__init__.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola.egg-info/dependency_links.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       76 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       74 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola.egg-info/entry_points.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      277 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       12 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola.egg-info/top_level.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      312 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      643 2019-04-30 20:31:00.000000 tap-taboola-0.2.1/setup.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      312 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       38 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/setup.cfg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1991 2018-11-09 20:03:04.000000 tap-taboola-0.2.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 12:24:24.243445 tap_taboola-0.3.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32386 2024-05-23 12:08:52.000000 tap_taboola-0.3.1/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      487 2024-05-29 12:24:24.243445 tap_taboola-0.3.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1991 2024-05-23 12:08:52.000000 tap_taboola-0.3.1/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-29 12:24:24.243445 tap_taboola-0.3.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      747 2024-05-29 12:23:52.000000 tap_taboola-0.3.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 12:24:24.243445 tap_taboola-0.3.1/tap_taboola/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    11130 2024-05-29 12:03:59.000000 tap_taboola-0.3.1/tap_taboola/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5220 2024-05-23 12:08:52.000000 tap_taboola-0.3.1/tap_taboola/schemas.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-29 12:24:24.243445 tap_taboola-0.3.1/tap_taboola.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      487 2024-05-29 12:24:24.000000 tap_taboola-0.3.1/tap_taboola.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2024-05-29 12:24:24.000000 tap_taboola-0.3.1/tap_taboola.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-29 12:24:24.000000 tap_taboola-0.3.1/tap_taboola.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2024-05-29 12:24:24.000000 tap_taboola-0.3.1/tap_taboola.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2024-05-29 12:24:24.000000 tap_taboola-0.3.1/tap_taboola.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2024-05-29 12:24:24.000000 tap_taboola-0.3.1/tap_taboola.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tap-taboola-0.2.1/tap_taboola/schemas.py` & `tap_taboola-0.3.1/tap_taboola/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,14 +125,18 @@
             'format': 'date',
             'description': 'The start date for this campaign.',
         },
         'impressions': {
             'type': 'integer',
             'description': 'Total number of impressions',
         },
+        'campaign_name': {
+            'type': ['string', 'null'],
+            'description': 'Human-readable campaign name',
+        },
         'ctr': {
             'type': 'number',
             'description': 'CTR, calculated as clicks/impressions',
         },
         'clicks': {
             'type': 'integer',
             'description': 'Total number of clicks',
@@ -158,13 +162,17 @@
             'type': 'number',
             'description': 'CPA, calculated as spend/actions',
         },
         'spent': {
             'type': 'number',
             'description': 'Total spent amount',
         },
+        'conversions_value': {
+            'type': ['number', 'null'],
+            'description': 'Total revenue from conversions',
+        },
         'currency': {
             'type': 'string',
             'description': 'ISO4217 currency code for columns of type money',
         }
     }
 }
```

### Comparing `tap-taboola-0.2.1/tap_taboola/__init__.py` & `tap_taboola-0.3.1/tap_taboola/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         url,
         headers={'Content-Type': 'application/x-www-form-urlencoded',
                  'Accept': 'application/json'},
         params=params)
 
     LOGGER.info("Got response code: {}".format(response.status_code))
 
+    result = {}
     if response.status_code == 200:
         LOGGER.info("Got an access token.")
         result = {"token": response.json().get('access_token', None)}
     elif response.status_code >= 400 and response.status_code < 500:
         result = {k: response.json().get(k) for k in ('error','error_description')}
 
     return result
@@ -86,14 +87,15 @@
         url,
         headers={'Content-Type': 'application/x-www-form-urlencoded',
                  'Accept': 'application/json'},
         params=params)
 
     LOGGER.info("Got response code: {}".format(response.status_code))
 
+    result = {}
     if response.status_code == 200:
         LOGGER.info("Got an access token.")
         result = {"token": response.json().get('access_token', None)}
     elif response.status_code >= 400 and response.status_code < 500:
         result = {k: response.json().get(k) for k in ('error','error_description')}
 
     return result
@@ -128,14 +130,16 @@
         'cpa_conversion_rate': float(campaign_performance.get(
             'cpa_conversion_rate', 0.0)),
         'spent': float(campaign_performance.get('spent', 0.0)),
         'date': str(datetime.datetime.strptime(
             campaign_performance.get('date'),
             '%Y-%m-%d %H:%M:%S.%f'
         ).date()),
+        'campaign_name': str(campaign_performance.get('campaign_name', '')),
+        'conversions_value': float(campaign_performance.get('conversions_value', 0.0)),
     }
 
 def fetch_campaign_performance(config, state, access_token, account_id):
     url = ('{}/backstage/api/1.0/{}/reports/campaign-summary/dimensions/campaign_day_breakdown' #pylint: disable=line-too-long
            .format(BASE_URL, account_id))
 
     params = {
```

### Comparing `tap-taboola-0.2.1/setup.py` & `tap_taboola-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-taboola',
-      version='0.2.1',
+      version='0.3.1',
       description='Singer.io tap for extracting data from the Taboola API',
       author='Fishtown Analytics',
       url='http://www.singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_taboola'],
       install_requires=[
-          'singer-python==5.0.4',
-          'backoff==1.3.2',
-          'requests==2.20.0',
+          'singer-python==5.13.0',
+          'backoff==1.8.0',
+          'requests==2.31.0',
           'python-dateutil==2.6.0'
       ],
+      extras_require={
+        "dev": [
+            "pylint",
+            "ipdb",
+        ]
+        },
       entry_points='''
           [console_scripts]
           tap-taboola=tap_taboola:main
       ''',
       packages=['tap_taboola']
 )
```

### Comparing `tap-taboola-0.2.1/README.md` & `tap_taboola-0.3.1/README.md`

 * *Files identical despite different names*

