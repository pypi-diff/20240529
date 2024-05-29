# Comparing `tmp/rezka_api_sdk-0.0.1.post2.tar.gz` & `tmp/rezka_api_sdk-0.0.1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rezka_api_sdk-0.0.1.post2.tar", last modified: Tue Feb 27 18:33:52 2024, max compression
+gzip compressed data, was "rezka_api_sdk-0.0.1.post3.tar", last modified: Wed May 29 19:48:20 2024, max compression
```

## Comparing `rezka_api_sdk-0.0.1.post2.tar` & `rezka_api_sdk-0.0.1.post3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-02-27 18:33:52.647210 rezka_api_sdk-0.0.1.post2/
--rw-rw-rw-   0        0        0     2283 2024-02-27 18:33:52.645206 rezka_api_sdk-0.0.1.post2/PKG-INFO
--rw-rw-rw-   0        0        0     1681 2024-02-27 15:36:00.000000 rezka_api_sdk-0.0.1.post2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-27 18:33:52.626202 rezka_api_sdk-0.0.1.post2/rezka_api_sdk/
--rw-rw-rw-   0        0        0      167 2024-02-27 15:22:40.000000 rezka_api_sdk-0.0.1.post2/rezka_api_sdk/__init__.py
--rw-rw-rw-   0        0        0       81 2024-02-27 15:33:23.000000 rezka_api_sdk-0.0.1.post2/rezka_api_sdk/constants.py
--rw-rw-rw-   0        0        0      475 2024-02-26 15:36:14.000000 rezka_api_sdk-0.0.1.post2/rezka_api_sdk/enums.py
--rw-rw-rw-   0        0        0      391 2024-02-26 16:00:56.000000 rezka_api_sdk-0.0.1.post2/rezka_api_sdk/exceptions.py
--rw-rw-rw-   0        0        0     1407 2024-02-27 15:26:32.000000 rezka_api_sdk-0.0.1.post2/rezka_api_sdk/models.py
--rw-rw-rw-   0        0        0     4120 2024-02-27 18:27:50.000000 rezka_api_sdk-0.0.1.post2/rezka_api_sdk/rezka_api.py
--rw-rw-rw-   0        0        0        0 2024-02-27 14:36:30.000000 rezka_api_sdk-0.0.1.post2/rezka_api_sdk/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-27 18:33:52.645206 rezka_api_sdk-0.0.1.post2/rezka_api_sdk.egg-info/
--rw-rw-rw-   0        0        0     2283 2024-02-27 18:33:52.000000 rezka_api_sdk-0.0.1.post2/rezka_api_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2024-02-27 18:33:52.000000 rezka_api_sdk-0.0.1.post2/rezka_api_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-27 18:33:52.000000 rezka_api_sdk-0.0.1.post2/rezka_api_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-02-27 18:33:52.000000 rezka_api_sdk-0.0.1.post2/rezka_api_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-02-27 18:33:52.000000 rezka_api_sdk-0.0.1.post2/rezka_api_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-27 18:33:52.647210 rezka_api_sdk-0.0.1.post2/setup.cfg
--rw-rw-rw-   0        0        0     1594 2024-02-26 17:32:11.000000 rezka_api_sdk-0.0.1.post2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:48:20.794864 rezka_api_sdk-0.0.1.post3/
+-rw-rw-rw-   0        0        0     2283 2024-05-29 19:48:20.792869 rezka_api_sdk-0.0.1.post3/PKG-INFO
+-rw-rw-rw-   0        0        0     1681 2024-02-27 15:36:02.000000 rezka_api_sdk-0.0.1.post3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 19:48:20.783894 rezka_api_sdk-0.0.1.post3/rezka_api_sdk/
+-rw-rw-rw-   0        0        0      167 2024-05-28 21:29:54.000000 rezka_api_sdk-0.0.1.post3/rezka_api_sdk/__init__.py
+-rw-rw-rw-   0        0        0       81 2024-02-27 15:33:24.000000 rezka_api_sdk-0.0.1.post3/rezka_api_sdk/constants.py
+-rw-rw-rw-   0        0        0      475 2024-02-26 15:36:16.000000 rezka_api_sdk-0.0.1.post3/rezka_api_sdk/enums.py
+-rw-rw-rw-   0        0        0      391 2024-02-26 16:00:58.000000 rezka_api_sdk-0.0.1.post3/rezka_api_sdk/exceptions.py
+-rw-rw-rw-   0        0        0     1454 2024-05-28 21:29:29.000000 rezka_api_sdk-0.0.1.post3/rezka_api_sdk/models.py
+-rw-rw-rw-   0        0        0     4120 2024-02-27 18:27:52.000000 rezka_api_sdk-0.0.1.post3/rezka_api_sdk/rezka_api.py
+-rw-rw-rw-   0        0        0        0 2024-02-27 14:36:32.000000 rezka_api_sdk-0.0.1.post3/rezka_api_sdk/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:48:20.792869 rezka_api_sdk-0.0.1.post3/rezka_api_sdk.egg-info/
+-rw-rw-rw-   0        0        0     2283 2024-05-29 19:48:20.000000 rezka_api_sdk-0.0.1.post3/rezka_api_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2024-05-29 19:48:20.000000 rezka_api_sdk-0.0.1.post3/rezka_api_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 19:48:20.000000 rezka_api_sdk-0.0.1.post3/rezka_api_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-29 19:48:20.000000 rezka_api_sdk-0.0.1.post3/rezka_api_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-29 19:48:20.000000 rezka_api_sdk-0.0.1.post3/rezka_api_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 19:48:20.794864 rezka_api_sdk-0.0.1.post3/setup.cfg
+-rw-rw-rw-   0        0        0     1594 2024-02-26 17:32:12.000000 rezka_api_sdk-0.0.1.post3/setup.py
```

### Comparing `rezka_api_sdk-0.0.1.post2/PKG-INFO` & `rezka_api_sdk-0.0.1.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rezka_api_sdk
-Version: 0.0.1.post2
+Version: 0.0.1.post3
 Summary: It is a library that allows you to interact with unofficial HDRezka API
 Home-page: https://github.com/arynyklas/rezka_api_sdk
 Author: Aryn Yklas
 Author-email: arynyklas@gmail.com
 Keywords: rezka,hdrezka,films,series
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rezka_api_sdk-0.0.1.post2/README.md` & `rezka_api_sdk-0.0.1.post3/README.md`

 * *Files identical despite different names*

### Comparing `rezka_api_sdk-0.0.1.post2/rezka_api_sdk/models.py` & `rezka_api_sdk-0.0.1.post3/rezka_api_sdk/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,8 +58,9 @@
 
 
 class DirectURLsModel(BaseModel):
     seasons: dict[str, str] | None
     episodes: dict[str, dict[str, str]] | None
     urls: dict[str, str] | None
     subtitles: dict[str, str] | None
+    subtitle_languages: dict[str, str] | None
     is_film: bool
```

### Comparing `rezka_api_sdk-0.0.1.post2/rezka_api_sdk/rezka_api.py` & `rezka_api_sdk-0.0.1.post3/rezka_api_sdk/rezka_api.py`

 * *Files identical despite different names*

### Comparing `rezka_api_sdk-0.0.1.post2/rezka_api_sdk.egg-info/PKG-INFO` & `rezka_api_sdk-0.0.1.post3/rezka_api_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rezka_api_sdk
-Version: 0.0.1.post2
+Name: rezka-api-sdk
+Version: 0.0.1.post3
 Summary: It is a library that allows you to interact with unofficial HDRezka API
 Home-page: https://github.com/arynyklas/rezka_api_sdk
 Author: Aryn Yklas
 Author-email: arynyklas@gmail.com
 Keywords: rezka,hdrezka,films,series
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rezka_api_sdk-0.0.1.post2/setup.py` & `rezka_api_sdk-0.0.1.post3/setup.py`

 * *Files identical despite different names*

