# Comparing `tmp/drf-2fa-1.0.1.tar.gz` & `tmp/drf-2fa-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-2fa-1.0.1.tar", last modified: Wed May 29 09:18:29 2024, max compression
+gzip compressed data, was "drf-2fa-1.0.2.tar", last modified: Wed May 29 10:59:25 2024, max compression
```

## Comparing `drf-2fa-1.0.1.tar` & `drf-2fa-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.393917 drf-2fa-1.0.1/
--rw-rw-rw-   0        0        0     1092 2024-05-28 18:07:59.000000 drf-2fa-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      991 2024-05-29 09:18:29.392779 drf-2fa-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      504 2024-05-28 20:27:24.000000 drf-2fa-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.366267 drf-2fa-1.0.1/drf_2fa/
--rw-rw-rw-   0        0        0        0 2024-04-01 11:36:42.000000 drf-2fa-1.0.1/drf_2fa/__init__.py
--rw-rw-rw-   0        0        0      468 2024-05-26 21:10:31.000000 drf-2fa-1.0.1/drf_2fa/admin.py
--rw-rw-rw-   0        0        0      220 2024-05-25 18:33:11.000000 drf-2fa-1.0.1/drf_2fa/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.384668 drf-2fa-1.0.1/drf_2fa/backends/
--rw-rw-rw-   0        0        0     2235 2024-05-26 18:26:16.000000 drf-2fa-1.0.1/drf_2fa/backends/__init__.py
--rw-rw-rw-   0        0        0     1447 2024-05-28 20:39:18.000000 drf-2fa-1.0.1/drf_2fa/backends/authenticator.py
--rw-rw-rw-   0        0        0      707 2024-05-26 18:22:12.000000 drf-2fa-1.0.1/drf_2fa/backends/email.py
--rw-rw-rw-   0        0        0     1243 2024-05-28 20:37:18.000000 drf-2fa-1.0.1/drf_2fa/backends/twilio.py
--rw-rw-rw-   0        0        0      678 2024-05-26 17:27:16.000000 drf-2fa-1.0.1/drf_2fa/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.386686 drf-2fa-1.0.1/drf_2fa/migrations/
--rw-rw-rw-   0        0        0     1403 2024-05-25 19:09:05.000000 drf-2fa-1.0.1/drf_2fa/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-04-01 11:36:42.000000 drf-2fa-1.0.1/drf_2fa/migrations/__init__.py
--rw-rw-rw-   0        0        0     2365 2024-05-26 21:10:31.000000 drf-2fa-1.0.1/drf_2fa/models.py
--rw-rw-rw-   0        0        0      319 2024-05-27 21:52:52.000000 drf-2fa-1.0.1/drf_2fa/serializers.py
--rw-rw-rw-   0        0        0     3746 2024-05-28 18:05:55.000000 drf-2fa-1.0.1/drf_2fa/settings.py
--rw-rw-rw-   0        0        0      428 2024-05-28 18:05:55.000000 drf-2fa-1.0.1/drf_2fa/signals.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.341514 drf-2fa-1.0.1/drf_2fa/templates/
-drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.343458 drf-2fa-1.0.1/drf_2fa/templates/drf_2fa/
-drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.389774 drf-2fa-1.0.1/drf_2fa/templates/drf_2fa/email/
--rw-rw-rw-   0        0        0      615 2024-05-25 19:05:18.000000 drf-2fa-1.0.1/drf_2fa/templates/drf_2fa/email/message.html
--rw-rw-rw-   0        0        0       50 2024-05-25 19:03:32.000000 drf-2fa-1.0.1/drf_2fa/templates/drf_2fa/email/subject.txt
-drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.390774 drf-2fa-1.0.1/drf_2fa/templates/drf_2fa/sms/
--rw-rw-rw-   0        0        0       29 2024-05-26 10:33:51.000000 drf-2fa-1.0.1/drf_2fa/templates/drf_2fa/sms/message.txt
--rw-rw-rw-   0        0        0      307 2024-05-27 21:57:31.000000 drf-2fa-1.0.1/drf_2fa/urls.py
--rw-rw-rw-   0        0        0     3584 2024-05-28 18:05:55.000000 drf-2fa-1.0.1/drf_2fa/views.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:18:29.380322 drf-2fa-1.0.1/drf_2fa.egg-info/
--rw-rw-rw-   0        0        0      991 2024-05-29 09:18:29.000000 drf-2fa-1.0.1/drf_2fa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      651 2024-05-29 09:18:29.000000 drf-2fa-1.0.1/drf_2fa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 09:18:29.000000 drf-2fa-1.0.1/drf_2fa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-29 09:18:29.000000 drf-2fa-1.0.1/drf_2fa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 09:18:29.394834 drf-2fa-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1089 2024-05-29 09:18:12.000000 drf-2fa-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.118488 drf-2fa-1.0.2/
+-rw-rw-rw-   0        0        0     1092 2024-05-28 18:07:59.000000 drf-2fa-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1303 2024-05-29 10:59:25.117483 drf-2fa-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      816 2024-05-29 10:28:10.000000 drf-2fa-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.092133 drf-2fa-1.0.2/drf_2fa/
+-rw-rw-rw-   0        0        0        0 2024-04-01 11:36:42.000000 drf-2fa-1.0.2/drf_2fa/__init__.py
+-rw-rw-rw-   0        0        0      468 2024-05-26 21:10:31.000000 drf-2fa-1.0.2/drf_2fa/admin.py
+-rw-rw-rw-   0        0        0      220 2024-05-25 18:33:11.000000 drf-2fa-1.0.2/drf_2fa/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.109981 drf-2fa-1.0.2/drf_2fa/backends/
+-rw-rw-rw-   0        0        0     2235 2024-05-26 18:26:16.000000 drf-2fa-1.0.2/drf_2fa/backends/__init__.py
+-rw-rw-rw-   0        0        0     1447 2024-05-28 20:39:18.000000 drf-2fa-1.0.2/drf_2fa/backends/authenticator.py
+-rw-rw-rw-   0        0        0      707 2024-05-26 18:22:12.000000 drf-2fa-1.0.2/drf_2fa/backends/email.py
+-rw-rw-rw-   0        0        0     1328 2024-05-29 10:00:19.000000 drf-2fa-1.0.2/drf_2fa/backends/twilio.py
+-rw-rw-rw-   0        0        0      678 2024-05-26 17:27:16.000000 drf-2fa-1.0.2/drf_2fa/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.111012 drf-2fa-1.0.2/drf_2fa/migrations/
+-rw-rw-rw-   0        0        0     1403 2024-05-25 19:09:05.000000 drf-2fa-1.0.2/drf_2fa/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 11:36:42.000000 drf-2fa-1.0.2/drf_2fa/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2365 2024-05-26 21:10:31.000000 drf-2fa-1.0.2/drf_2fa/models.py
+-rw-rw-rw-   0        0        0      319 2024-05-27 21:52:52.000000 drf-2fa-1.0.2/drf_2fa/serializers.py
+-rw-rw-rw-   0        0        0     3746 2024-05-28 18:05:55.000000 drf-2fa-1.0.2/drf_2fa/settings.py
+-rw-rw-rw-   0        0        0      428 2024-05-28 18:05:55.000000 drf-2fa-1.0.2/drf_2fa/signals.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.074010 drf-2fa-1.0.2/drf_2fa/templates/
+drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.075024 drf-2fa-1.0.2/drf_2fa/templates/drf_2fa/
+drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.114457 drf-2fa-1.0.2/drf_2fa/templates/drf_2fa/email/
+-rw-rw-rw-   0        0        0      615 2024-05-25 19:05:18.000000 drf-2fa-1.0.2/drf_2fa/templates/drf_2fa/email/message.html
+-rw-rw-rw-   0        0        0       50 2024-05-25 19:03:32.000000 drf-2fa-1.0.2/drf_2fa/templates/drf_2fa/email/subject.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.116482 drf-2fa-1.0.2/drf_2fa/templates/drf_2fa/sms/
+-rw-rw-rw-   0        0        0       29 2024-05-26 10:33:51.000000 drf-2fa-1.0.2/drf_2fa/templates/drf_2fa/sms/message.txt
+-rw-rw-rw-   0        0        0      307 2024-05-27 21:57:31.000000 drf-2fa-1.0.2/drf_2fa/urls.py
+-rw-rw-rw-   0        0        0     3584 2024-05-28 18:05:55.000000 drf-2fa-1.0.2/drf_2fa/views.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.105278 drf-2fa-1.0.2/drf_2fa.egg-info/
+-rw-rw-rw-   0        0        0     1303 2024-05-29 10:59:24.000000 drf-2fa-1.0.2/drf_2fa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      681 2024-05-29 10:59:25.000000 drf-2fa-1.0.2/drf_2fa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 10:59:24.000000 drf-2fa-1.0.2/drf_2fa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-29 10:59:24.000000 drf-2fa-1.0.2/drf_2fa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       44 2024-05-29 10:59:24.000000 drf-2fa-1.0.2/drf_2fa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 10:59:25.118488 drf-2fa-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1187 2024-05-29 10:59:12.000000 drf-2fa-1.0.2/setup.py
```

### Comparing `drf-2fa-1.0.1/LICENSE` & `drf-2fa-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.1/drf_2fa/backends/__init__.py` & `drf-2fa-1.0.2/drf_2fa/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.1/drf_2fa/backends/authenticator.py` & `drf-2fa-1.0.2/drf_2fa/backends/authenticator.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.1/drf_2fa/backends/email.py` & `drf-2fa-1.0.2/drf_2fa/backends/email.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.1/drf_2fa/backends/twilio.py` & `drf-2fa-1.0.2/drf_2fa/backends/twilio.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,16 @@
         try:
             client = Client(self.settings.TWILIO_ACCOUNT_SID, self.settings.TWILIO_AUTH_TOKEN)
         except Exception as e:
             raise SMSClientCouldNotCreate(e)
         return client
     
     def get_receiver_phone_number(self, user):
+        """Phone number returned from this method will receive OTP sms"""
+        
         try:
             return getattr(user, self.settings.PHONE_NUMBER_FIELD)
         except:
             raise InvalidPhoneNumberField
 
     def send_otp(self, user):
         client = self.get_twilio_client()
```

### Comparing `drf-2fa-1.0.1/drf_2fa/exceptions.py` & `drf-2fa-1.0.2/drf_2fa/exceptions.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.1/drf_2fa/migrations/0001_initial.py` & `drf-2fa-1.0.2/drf_2fa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.1/drf_2fa/models.py` & `drf-2fa-1.0.2/drf_2fa/models.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.1/drf_2fa/settings.py` & `drf-2fa-1.0.2/drf_2fa/settings.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.1/drf_2fa/templates/drf_2fa/email/message.html` & `drf-2fa-1.0.2/drf_2fa/templates/drf_2fa/email/message.html`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.1/drf_2fa/views.py` & `drf-2fa-1.0.2/drf_2fa/views.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.1/drf_2fa.egg-info/SOURCES.txt` & `drf-2fa-1.0.2/drf_2fa.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 drf_2fa/settings.py
 drf_2fa/signals.py
 drf_2fa/urls.py
 drf_2fa/views.py
 drf_2fa.egg-info/PKG-INFO
 drf_2fa.egg-info/SOURCES.txt
 drf_2fa.egg-info/dependency_links.txt
+drf_2fa.egg-info/requires.txt
 drf_2fa.egg-info/top_level.txt
 drf_2fa/backends/__init__.py
 drf_2fa/backends/authenticator.py
 drf_2fa/backends/email.py
 drf_2fa/backends/twilio.py
 drf_2fa/migrations/0001_initial.py
 drf_2fa/migrations/__init__.py
```

### Comparing `drf-2fa-1.0.1/setup.py` & `drf-2fa-1.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (BASE_PATH / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="drf-2fa",
-    version="1.0.1",
+    version="1.0.2",
     description="Integrate 2 Factor Authentication in Your Django REST API project easily.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/farhad0085/drf-2fa",
     author="Farhad Hossain",
     author_email="farhadhossain0085@gmail.com",
     license="MIT",
@@ -22,14 +22,15 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
     ],
     packages=["drf_2fa", "drf_2fa/migrations", "drf_2fa/backends"],
     package_data={'drf_2fa': ['templates/**/**/*.*']},
     include_package_data=True,
-    install_requires=[],
+    install_requires=["qrcode==7.4.2", "django>=2.2", "djangorestframework>=3.14"],
 )
 
 # build
+# update version name before building
 # python setup.py sdist bdist_wheel
 # upload to pypi
 # twine upload dist/*
```

