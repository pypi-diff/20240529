# Comparing `tmp/url_remote-0.0.96.tar.gz` & `tmp/url_remote-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "url_remote-0.0.96.tar", last modified: Thu May 23 17:03:01 2024, max compression
+gzip compressed data, was "url_remote-0.0.97.tar", last modified: Wed May 29 14:04:06 2024, max compression
```

## Comparing `url_remote-0.0.96.tar` & `url_remote-0.0.97.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:03:01.177111 url_remote-0.0.96/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-23 17:03:01.177111 url_remote-0.0.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-23 17:02:50.000000 url_remote-0.0.96/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-23 17:02:50.000000 url_remote-0.0.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:03:01.177111 url_remote-0.0.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-23 17:02:50.000000 url_remote-0.0.96/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:03:01.173111 url_remote-0.0.96/url_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:03:01.177111 url_remote-0.0.96/url_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:02:50.000000 url_remote-0.0.96/url_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-23 17:02:50.000000 url_remote-0.0.96/url_remote/src/action_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-23 17:02:50.000000 url_remote-0.0.96/url_remote/src/api_version_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-23 17:02:50.000000 url_remote-0.0.96/url_remote/src/authentiction_api_version_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-23 17:02:50.000000 url_remote-0.0.96/url_remote/src/brand_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-23 17:02:50.000000 url_remote-0.0.96/url_remote/src/component_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 17:02:50.000000 url_remote-0.0.96/url_remote/src/entity_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-23 17:02:50.000000 url_remote-0.0.96/url_remote/src/environment_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9051 2024-05-23 17:02:50.000000 url_remote-0.0.96/url_remote/src/our_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-23 17:02:50.000000 url_remote-0.0.96/url_remote/src/url_circlez.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:03:01.177111 url_remote-0.0.96/url_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-23 17:03:01.000000 url_remote-0.0.96/url_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-23 17:03:01.000000 url_remote-0.0.96/url_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:03:01.000000 url_remote-0.0.96/url_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 17:03:01.000000 url_remote-0.0.96/url_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:04:06.639021 url_remote-0.0.97/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-29 14:04:06.639021 url_remote-0.0.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-29 14:03:53.000000 url_remote-0.0.97/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-29 14:03:59.000000 url_remote-0.0.97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:04:06.639021 url_remote-0.0.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-29 14:03:53.000000 url_remote-0.0.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:04:06.635021 url_remote-0.0.97/url_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:04:06.639021 url_remote-0.0.97/url_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/action_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/api_version_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/authentiction_api_version_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/brand_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/component_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/entity_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/environment_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/our_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/url_circlez.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:04:06.639021 url_remote-0.0.97/url_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-29 14:04:06.000000 url_remote-0.0.97/url_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-29 14:04:06.000000 url_remote-0.0.97/url_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:04:06.000000 url_remote-0.0.97/url_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 14:04:06.000000 url_remote-0.0.97/url_remote.egg-info/top_level.txt
```

### Comparing `url_remote-0.0.96/README.md` & `url_remote-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.96/setup.py` & `url_remote-0.0.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "url-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.96',  # https://pypi.org/project/url-remote
+    version='0.0.97',  # https://pypi.org/project/url-remote
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="URL Local",
```

### Comparing `url_remote-0.0.96/url_remote/src/action_name_enum.py` & `url_remote-0.0.97/url_remote/src/action_name_enum.py`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.96/url_remote/src/api_version_dicts.py` & `url_remote-0.0.97/url_remote/src/api_version_dicts.py`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.96/url_remote/src/component_name_enum.py` & `url_remote-0.0.97/url_remote/src/component_name_enum.py`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.96/url_remote/src/our_url.py` & `url_remote-0.0.97/url_remote/src/our_url.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         'logger.play1.circ.zone': 'fsujmjyfal.execute-api.us-east-1.amazonaws.com',
         # 'event.play1.circ.zone': 'p89mpsr5m1.execute-api.us-east-1.amazonaws.com',
         # 'event.play1.circ.zone': 'x8ql0j9cwf.execute-api.us-east-1.amazonaws.com',
         'event.play1.circ.zone': '2iclscptqh.execute-api.us-east-1.amazonaws.com',
         'event.dvlp1.circ.zone': 'wbq5liyk63.execute-api.us-east-1.amazonaws.com',
         'storage.play1.circ.zone': 'wbq5liyk63.execute-api.us-east-1.amazonaws.com',  # TODO update
         'storage.dvlp1.circ.zone': 'wbq5liyk63.execute-api.us-east-1.amazonaws.com',  # TODO update
-        'smartlink.play1.circ.zone': 'wagdetw4hk.execute-api.us-east-1.amazonaws.com/dev',
-        'smartlink.dvlp1.circ.zone': '6cqasxkwcl.execute-api.us-east-1.amazonaws.com/dev',
+        'smartlink.play1.circ.zone': 'ezt1n60if7.execute-api.us-east-1.amazonaws.com',
+        'smartlink.dvlp1.circ.zone': 'u5ohxnpxug.execute-api.us-east-1.amazonaws.com',
         'dialogWorkflow.play1.circ.zone': 'g91pb4afb1.execute-api.us-east-1.amazonaws.com/dev',
         'dialogWorkflow.dvlp1.circ.zone': 'xoonx24zbg.execute-api.us-east-1.amazonaws.com/dev',
         # 'websocket.dvlp1.circ.zone': 'ws://23.22.217.199:8080',
         # 'websocket.play1.circ.zone': 'ws://23.22.217.199:8080',
     }
 
     @staticmethod
```

### Comparing `url_remote-0.0.96/url_remote.egg-info/SOURCES.txt` & `url_remote-0.0.97/url_remote.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,11 +7,12 @@
 url_remote.egg-info/top_level.txt
 url_remote/src/__init__.py
 url_remote/src/action_name_enum.py
 url_remote/src/api_version_dicts.py
 url_remote/src/authentiction_api_version_dict.py
 url_remote/src/brand_name_enum.py
 url_remote/src/component_name_enum.py
+url_remote/src/domain.py
 url_remote/src/entity_name_enum.py
 url_remote/src/environment_name_enum.py
 url_remote/src/our_url.py
 url_remote/src/url_circlez.py
```

