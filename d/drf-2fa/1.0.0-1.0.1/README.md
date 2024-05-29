# Comparing `tmp/drf-2fa-1.0.0.tar.gz` & `tmp/drf-2fa-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-2fa-1.0.0.tar", last modified: Wed May 29 08:53:23 2024, max compression
+gzip compressed data, was "drf-2fa-1.0.1.tar", last modified: Wed May 29 09:18:29 2024, max compression
```

## Comparing `drf-2fa-1.0.0.tar` & `drf-2fa-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 08:53:23.028080 drf-2fa-1.0.0/
--rw-rw-rw-   0        0        0     1092 2024-05-28 18:07:59.000000 drf-2fa-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      982 2024-05-29 08:53:23.026742 drf-2fa-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      504 2024-05-28 20:27:24.000000 drf-2fa-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 08:53:22.974248 drf-2fa-1.0.0/drf_2fa/
--rw-rw-rw-   0        0        0        0 2024-04-01 11:36:42.000000 drf-2fa-1.0.0/drf_2fa/__init__.py
--rw-rw-rw-   0        0        0      468 2024-05-26 21:10:31.000000 drf-2fa-1.0.0/drf_2fa/admin.py
--rw-rw-rw-   0        0        0      220 2024-05-25 18:33:11.000000 drf-2fa-1.0.0/drf_2fa/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:53:23.022199 drf-2fa-1.0.0/drf_2fa/backends/
--rw-rw-rw-   0        0        0     2235 2024-05-26 18:26:16.000000 drf-2fa-1.0.0/drf_2fa/backends/__init__.py
--rw-rw-rw-   0        0        0     1447 2024-05-28 20:39:18.000000 drf-2fa-1.0.0/drf_2fa/backends/authenticator.py
--rw-rw-rw-   0        0        0      707 2024-05-26 18:22:12.000000 drf-2fa-1.0.0/drf_2fa/backends/email.py
--rw-rw-rw-   0        0        0     1243 2024-05-28 20:37:18.000000 drf-2fa-1.0.0/drf_2fa/backends/twilio.py
--rw-rw-rw-   0        0        0      678 2024-05-26 17:27:16.000000 drf-2fa-1.0.0/drf_2fa/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:53:23.025733 drf-2fa-1.0.0/drf_2fa/migrations/
--rw-rw-rw-   0        0        0     1403 2024-05-25 19:09:05.000000 drf-2fa-1.0.0/drf_2fa/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-04-01 11:36:42.000000 drf-2fa-1.0.0/drf_2fa/migrations/__init__.py
--rw-rw-rw-   0        0        0     2365 2024-05-26 21:10:31.000000 drf-2fa-1.0.0/drf_2fa/models.py
--rw-rw-rw-   0        0        0      319 2024-05-27 21:52:52.000000 drf-2fa-1.0.0/drf_2fa/serializers.py
--rw-rw-rw-   0        0        0     3746 2024-05-28 18:05:55.000000 drf-2fa-1.0.0/drf_2fa/settings.py
--rw-rw-rw-   0        0        0      428 2024-05-28 18:05:55.000000 drf-2fa-1.0.0/drf_2fa/signals.py
--rw-rw-rw-   0        0        0      307 2024-05-27 21:57:31.000000 drf-2fa-1.0.0/drf_2fa/urls.py
--rw-rw-rw-   0        0        0     3584 2024-05-28 18:05:55.000000 drf-2fa-1.0.0/drf_2fa/views.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:53:23.012689 drf-2fa-1.0.0/drf_2fa.egg-info/
--rw-rw-rw-   0        0        0      982 2024-05-29 08:53:22.000000 drf-2fa-1.0.0/drf_2fa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2024-05-29 08:53:22.000000 drf-2fa-1.0.0/drf_2fa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 08:53:22.000000 drf-2fa-1.0.0/drf_2fa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-29 08:53:22.000000 drf-2fa-1.0.0/drf_2fa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       62 2024-05-29 08:53:22.000000 drf-2fa-1.0.0/drf_2fa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 08:53:23.028080 drf-2fa-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1058 2024-05-28 18:17:49.000000 drf-2fa-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.393917 drf-2fa-1.0.1/
+-rw-rw-rw-   0        0        0     1092 2024-05-28 18:07:59.000000 drf-2fa-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      991 2024-05-29 09:18:29.392779 drf-2fa-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2024-05-28 20:27:24.000000 drf-2fa-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.366267 drf-2fa-1.0.1/drf_2fa/
+-rw-rw-rw-   0        0        0        0 2024-04-01 11:36:42.000000 drf-2fa-1.0.1/drf_2fa/__init__.py
+-rw-rw-rw-   0        0        0      468 2024-05-26 21:10:31.000000 drf-2fa-1.0.1/drf_2fa/admin.py
+-rw-rw-rw-   0        0        0      220 2024-05-25 18:33:11.000000 drf-2fa-1.0.1/drf_2fa/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.384668 drf-2fa-1.0.1/drf_2fa/backends/
+-rw-rw-rw-   0        0        0     2235 2024-05-26 18:26:16.000000 drf-2fa-1.0.1/drf_2fa/backends/__init__.py
+-rw-rw-rw-   0        0        0     1447 2024-05-28 20:39:18.000000 drf-2fa-1.0.1/drf_2fa/backends/authenticator.py
+-rw-rw-rw-   0        0        0      707 2024-05-26 18:22:12.000000 drf-2fa-1.0.1/drf_2fa/backends/email.py
+-rw-rw-rw-   0        0        0     1243 2024-05-28 20:37:18.000000 drf-2fa-1.0.1/drf_2fa/backends/twilio.py
+-rw-rw-rw-   0        0        0      678 2024-05-26 17:27:16.000000 drf-2fa-1.0.1/drf_2fa/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.386686 drf-2fa-1.0.1/drf_2fa/migrations/
+-rw-rw-rw-   0        0        0     1403 2024-05-25 19:09:05.000000 drf-2fa-1.0.1/drf_2fa/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 11:36:42.000000 drf-2fa-1.0.1/drf_2fa/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2365 2024-05-26 21:10:31.000000 drf-2fa-1.0.1/drf_2fa/models.py
+-rw-rw-rw-   0        0        0      319 2024-05-27 21:52:52.000000 drf-2fa-1.0.1/drf_2fa/serializers.py
+-rw-rw-rw-   0        0        0     3746 2024-05-28 18:05:55.000000 drf-2fa-1.0.1/drf_2fa/settings.py
+-rw-rw-rw-   0        0        0      428 2024-05-28 18:05:55.000000 drf-2fa-1.0.1/drf_2fa/signals.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.341514 drf-2fa-1.0.1/drf_2fa/templates/
+drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.343458 drf-2fa-1.0.1/drf_2fa/templates/drf_2fa/
+drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.389774 drf-2fa-1.0.1/drf_2fa/templates/drf_2fa/email/
+-rw-rw-rw-   0        0        0      615 2024-05-25 19:05:18.000000 drf-2fa-1.0.1/drf_2fa/templates/drf_2fa/email/message.html
+-rw-rw-rw-   0        0        0       50 2024-05-25 19:03:32.000000 drf-2fa-1.0.1/drf_2fa/templates/drf_2fa/email/subject.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.390774 drf-2fa-1.0.1/drf_2fa/templates/drf_2fa/sms/
+-rw-rw-rw-   0        0        0       29 2024-05-26 10:33:51.000000 drf-2fa-1.0.1/drf_2fa/templates/drf_2fa/sms/message.txt
+-rw-rw-rw-   0        0        0      307 2024-05-27 21:57:31.000000 drf-2fa-1.0.1/drf_2fa/urls.py
+-rw-rw-rw-   0        0        0     3584 2024-05-28 18:05:55.000000 drf-2fa-1.0.1/drf_2fa/views.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.380322 drf-2fa-1.0.1/drf_2fa.egg-info/
+-rw-rw-rw-   0        0        0      991 2024-05-29 09:18:29.000000 drf-2fa-1.0.1/drf_2fa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      651 2024-05-29 09:18:29.000000 drf-2fa-1.0.1/drf_2fa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 09:18:29.000000 drf-2fa-1.0.1/drf_2fa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-29 09:18:29.000000 drf-2fa-1.0.1/drf_2fa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 09:18:29.394834 drf-2fa-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1089 2024-05-29 09:18:12.000000 drf-2fa-1.0.1/setup.py
```

### Comparing `drf-2fa-1.0.0/LICENSE` & `drf-2fa-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.0/PKG-INFO` & `drf-2fa-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: drf-2fa
-Version: 1.0.0
-Summary: Integrate 2 factor authentication in your django rest api easily
+Version: 1.0.1
+Summary: Integrate 2 Factor Authentication in Your Django REST API project easily.
 Home-page: https://github.com/farhad0085/drf-2fa
 Author: Farhad Hossain
 Author-email: farhadhossain0085@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drf-2fa-1.0.0/drf_2fa/backends/__init__.py` & `drf-2fa-1.0.1/drf_2fa/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.0/drf_2fa/backends/authenticator.py` & `drf-2fa-1.0.1/drf_2fa/backends/authenticator.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.0/drf_2fa/backends/email.py` & `drf-2fa-1.0.1/drf_2fa/backends/email.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.0/drf_2fa/backends/twilio.py` & `drf-2fa-1.0.1/drf_2fa/backends/twilio.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.0/drf_2fa/exceptions.py` & `drf-2fa-1.0.1/drf_2fa/exceptions.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.0/drf_2fa/migrations/0001_initial.py` & `drf-2fa-1.0.1/drf_2fa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.0/drf_2fa/models.py` & `drf-2fa-1.0.1/drf_2fa/models.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.0/drf_2fa/settings.py` & `drf-2fa-1.0.1/drf_2fa/settings.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.0/drf_2fa/views.py` & `drf-2fa-1.0.1/drf_2fa/views.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.0/drf_2fa.egg-info/PKG-INFO` & `drf-2fa-1.0.1/drf_2fa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: drf-2fa
-Version: 1.0.0
-Summary: Integrate 2 factor authentication in your django rest api easily
+Version: 1.0.1
+Summary: Integrate 2 Factor Authentication in Your Django REST API project easily.
 Home-page: https://github.com/farhad0085/drf-2fa
 Author: Farhad Hossain
 Author-email: farhadhossain0085@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drf-2fa-1.0.0/drf_2fa.egg-info/SOURCES.txt` & `drf-2fa-1.0.1/drf_2fa.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 drf_2fa/settings.py
 drf_2fa/signals.py
 drf_2fa/urls.py
 drf_2fa/views.py
 drf_2fa.egg-info/PKG-INFO
 drf_2fa.egg-info/SOURCES.txt
 drf_2fa.egg-info/dependency_links.txt
-drf_2fa.egg-info/requires.txt
 drf_2fa.egg-info/top_level.txt
 drf_2fa/backends/__init__.py
 drf_2fa/backends/authenticator.py
 drf_2fa/backends/email.py
 drf_2fa/backends/twilio.py
 drf_2fa/migrations/0001_initial.py
-drf_2fa/migrations/__init__.py
+drf_2fa/migrations/__init__.py
+drf_2fa/templates/drf_2fa/email/message.html
+drf_2fa/templates/drf_2fa/email/subject.txt
+drf_2fa/templates/drf_2fa/sms/message.txt
```

### Comparing `drf-2fa-1.0.0/setup.py` & `drf-2fa-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 
 # The text of the README file
 README = (BASE_PATH / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="drf-2fa",
-    version="1.0.0",
-    description="Integrate 2 factor authentication in your django rest api easily",
+    version="1.0.1",
+    description="Integrate 2 Factor Authentication in Your Django REST API project easily.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/farhad0085/drf-2fa",
     author="Farhad Hossain",
     author_email="farhadhossain0085@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
     ],
-    packages=["drf_2fa", "drf_2fa/migrations", "drf_2fa/templates", "drf_2fa/backends"],
+    packages=["drf_2fa", "drf_2fa/migrations", "drf_2fa/backends"],
+    package_data={'drf_2fa': ['templates/**/**/*.*']},
     include_package_data=True,
-    install_requires=["django>=2.2"],
+    install_requires=[],
 )
 
 # build
 # python setup.py sdist bdist_wheel
 # upload to pypi
 # twine upload dist/*
```

