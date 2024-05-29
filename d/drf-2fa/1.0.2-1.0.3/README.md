# Comparing `tmp/drf-2fa-1.0.2.tar.gz` & `tmp/drf-2fa-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-2fa-1.0.2.tar", last modified: Wed May 29 10:59:25 2024, max compression
+gzip compressed data, was "drf-2fa-1.0.3.tar", last modified: Wed May 29 11:38:14 2024, max compression
```

## Comparing `drf-2fa-1.0.2.tar` & `drf-2fa-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.118488 drf-2fa-1.0.2/
--rw-rw-rw-   0        0        0     1092 2024-05-28 18:07:59.000000 drf-2fa-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1303 2024-05-29 10:59:25.117483 drf-2fa-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      816 2024-05-29 10:28:10.000000 drf-2fa-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.092133 drf-2fa-1.0.2/drf_2fa/
--rw-rw-rw-   0        0        0        0 2024-04-01 11:36:42.000000 drf-2fa-1.0.2/drf_2fa/__init__.py
--rw-rw-rw-   0        0        0      468 2024-05-26 21:10:31.000000 drf-2fa-1.0.2/drf_2fa/admin.py
--rw-rw-rw-   0        0        0      220 2024-05-25 18:33:11.000000 drf-2fa-1.0.2/drf_2fa/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.109981 drf-2fa-1.0.2/drf_2fa/backends/
--rw-rw-rw-   0        0        0     2235 2024-05-26 18:26:16.000000 drf-2fa-1.0.2/drf_2fa/backends/__init__.py
--rw-rw-rw-   0        0        0     1447 2024-05-28 20:39:18.000000 drf-2fa-1.0.2/drf_2fa/backends/authenticator.py
--rw-rw-rw-   0        0        0      707 2024-05-26 18:22:12.000000 drf-2fa-1.0.2/drf_2fa/backends/email.py
--rw-rw-rw-   0        0        0     1328 2024-05-29 10:00:19.000000 drf-2fa-1.0.2/drf_2fa/backends/twilio.py
--rw-rw-rw-   0        0        0      678 2024-05-26 17:27:16.000000 drf-2fa-1.0.2/drf_2fa/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.111012 drf-2fa-1.0.2/drf_2fa/migrations/
--rw-rw-rw-   0        0        0     1403 2024-05-25 19:09:05.000000 drf-2fa-1.0.2/drf_2fa/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-04-01 11:36:42.000000 drf-2fa-1.0.2/drf_2fa/migrations/__init__.py
--rw-rw-rw-   0        0        0     2365 2024-05-26 21:10:31.000000 drf-2fa-1.0.2/drf_2fa/models.py
--rw-rw-rw-   0        0        0      319 2024-05-27 21:52:52.000000 drf-2fa-1.0.2/drf_2fa/serializers.py
--rw-rw-rw-   0        0        0     3746 2024-05-28 18:05:55.000000 drf-2fa-1.0.2/drf_2fa/settings.py
--rw-rw-rw-   0        0        0      428 2024-05-28 18:05:55.000000 drf-2fa-1.0.2/drf_2fa/signals.py
-drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.074010 drf-2fa-1.0.2/drf_2fa/templates/
-drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.075024 drf-2fa-1.0.2/drf_2fa/templates/drf_2fa/
-drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.114457 drf-2fa-1.0.2/drf_2fa/templates/drf_2fa/email/
--rw-rw-rw-   0        0        0      615 2024-05-25 19:05:18.000000 drf-2fa-1.0.2/drf_2fa/templates/drf_2fa/email/message.html
--rw-rw-rw-   0        0        0       50 2024-05-25 19:03:32.000000 drf-2fa-1.0.2/drf_2fa/templates/drf_2fa/email/subject.txt
-drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.116482 drf-2fa-1.0.2/drf_2fa/templates/drf_2fa/sms/
--rw-rw-rw-   0        0        0       29 2024-05-26 10:33:51.000000 drf-2fa-1.0.2/drf_2fa/templates/drf_2fa/sms/message.txt
--rw-rw-rw-   0        0        0      307 2024-05-27 21:57:31.000000 drf-2fa-1.0.2/drf_2fa/urls.py
--rw-rw-rw-   0        0        0     3584 2024-05-28 18:05:55.000000 drf-2fa-1.0.2/drf_2fa/views.py
-drwxrwxrwx   0        0        0        0 2024-05-29 10:59:25.105278 drf-2fa-1.0.2/drf_2fa.egg-info/
--rw-rw-rw-   0        0        0     1303 2024-05-29 10:59:24.000000 drf-2fa-1.0.2/drf_2fa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      681 2024-05-29 10:59:25.000000 drf-2fa-1.0.2/drf_2fa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 10:59:24.000000 drf-2fa-1.0.2/drf_2fa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-29 10:59:24.000000 drf-2fa-1.0.2/drf_2fa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       44 2024-05-29 10:59:24.000000 drf-2fa-1.0.2/drf_2fa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 10:59:25.118488 drf-2fa-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1187 2024-05-29 10:59:12.000000 drf-2fa-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:38:14.666442 drf-2fa-1.0.3/
+-rw-rw-rw-   0        0        0     1092 2024-05-28 18:07:59.000000 drf-2fa-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1303 2024-05-29 11:38:14.665388 drf-2fa-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      816 2024-05-29 10:28:10.000000 drf-2fa-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 11:38:14.641255 drf-2fa-1.0.3/drf_2fa/
+-rw-rw-rw-   0        0        0        0 2024-04-01 11:36:42.000000 drf-2fa-1.0.3/drf_2fa/__init__.py
+-rw-rw-rw-   0        0        0      468 2024-05-26 21:10:31.000000 drf-2fa-1.0.3/drf_2fa/admin.py
+-rw-rw-rw-   0        0        0      220 2024-05-25 18:33:11.000000 drf-2fa-1.0.3/drf_2fa/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:38:14.657835 drf-2fa-1.0.3/drf_2fa/backends/
+-rw-rw-rw-   0        0        0     2235 2024-05-26 18:26:16.000000 drf-2fa-1.0.3/drf_2fa/backends/__init__.py
+-rw-rw-rw-   0        0        0     1447 2024-05-28 20:39:18.000000 drf-2fa-1.0.3/drf_2fa/backends/authenticator.py
+-rw-rw-rw-   0        0        0      707 2024-05-26 18:22:12.000000 drf-2fa-1.0.3/drf_2fa/backends/email.py
+-rw-rw-rw-   0        0        0     1328 2024-05-29 10:00:19.000000 drf-2fa-1.0.3/drf_2fa/backends/twilio.py
+-rw-rw-rw-   0        0        0      678 2024-05-26 17:27:16.000000 drf-2fa-1.0.3/drf_2fa/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:38:14.661005 drf-2fa-1.0.3/drf_2fa/migrations/
+-rw-rw-rw-   0        0        0     1403 2024-05-25 19:09:05.000000 drf-2fa-1.0.3/drf_2fa/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 11:36:42.000000 drf-2fa-1.0.3/drf_2fa/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2389 2024-05-29 11:28:36.000000 drf-2fa-1.0.3/drf_2fa/models.py
+-rw-rw-rw-   0        0        0      319 2024-05-27 21:52:52.000000 drf-2fa-1.0.3/drf_2fa/serializers.py
+-rw-rw-rw-   0        0        0     3746 2024-05-28 18:05:55.000000 drf-2fa-1.0.3/drf_2fa/settings.py
+-rw-rw-rw-   0        0        0      428 2024-05-28 18:05:55.000000 drf-2fa-1.0.3/drf_2fa/signals.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:38:14.610480 drf-2fa-1.0.3/drf_2fa/templates/
+drwxrwxrwx   0        0        0        0 2024-05-29 11:38:14.611028 drf-2fa-1.0.3/drf_2fa/templates/drf_2fa/
+drwxrwxrwx   0        0        0        0 2024-05-29 11:38:14.663214 drf-2fa-1.0.3/drf_2fa/templates/drf_2fa/email/
+-rw-rw-rw-   0        0        0      615 2024-05-25 19:05:18.000000 drf-2fa-1.0.3/drf_2fa/templates/drf_2fa/email/message.html
+-rw-rw-rw-   0        0        0       50 2024-05-25 19:03:32.000000 drf-2fa-1.0.3/drf_2fa/templates/drf_2fa/email/subject.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 11:38:14.664379 drf-2fa-1.0.3/drf_2fa/templates/drf_2fa/sms/
+-rw-rw-rw-   0        0        0       29 2024-05-26 10:33:51.000000 drf-2fa-1.0.3/drf_2fa/templates/drf_2fa/sms/message.txt
+-rw-rw-rw-   0        0        0      307 2024-05-27 21:57:31.000000 drf-2fa-1.0.3/drf_2fa/urls.py
+-rw-rw-rw-   0        0        0     3776 2024-05-29 11:25:35.000000 drf-2fa-1.0.3/drf_2fa/views.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:38:14.653594 drf-2fa-1.0.3/drf_2fa.egg-info/
+-rw-rw-rw-   0        0        0     1303 2024-05-29 11:38:14.000000 drf-2fa-1.0.3/drf_2fa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      681 2024-05-29 11:38:14.000000 drf-2fa-1.0.3/drf_2fa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:38:14.000000 drf-2fa-1.0.3/drf_2fa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-29 11:38:14.000000 drf-2fa-1.0.3/drf_2fa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       44 2024-05-29 11:38:14.000000 drf-2fa-1.0.3/drf_2fa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:38:14.666442 drf-2fa-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1187 2024-05-29 11:35:20.000000 drf-2fa-1.0.3/setup.py
```

### Comparing `drf-2fa-1.0.2/LICENSE` & `drf-2fa-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.2/PKG-INFO` & `drf-2fa-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-2fa
-Version: 1.0.2
+Version: 1.0.3
 Summary: Integrate 2 Factor Authentication in Your Django REST API project easily.
 Home-page: https://github.com/farhad0085/drf-2fa
 Author: Farhad Hossain
 Author-email: farhadhossain0085@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `drf-2fa-1.0.2/README.md` & `drf-2fa-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.2/drf_2fa/backends/__init__.py` & `drf-2fa-1.0.3/drf_2fa/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.2/drf_2fa/backends/authenticator.py` & `drf-2fa-1.0.3/drf_2fa/backends/authenticator.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.2/drf_2fa/backends/email.py` & `drf-2fa-1.0.3/drf_2fa/backends/email.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.2/drf_2fa/backends/twilio.py` & `drf-2fa-1.0.3/drf_2fa/backends/twilio.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.2/drf_2fa/exceptions.py` & `drf-2fa-1.0.3/drf_2fa/exceptions.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.2/drf_2fa/migrations/0001_initial.py` & `drf-2fa-1.0.3/drf_2fa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.2/drf_2fa/models.py` & `drf-2fa-1.0.3/drf_2fa/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,13 +56,13 @@
             return False
         expiration_time = otp_obj.created_at + otp_expire
         return timezone.now() > expiration_time
 
     @classmethod
     def is_valid(cls, user, otp_code):
         # check if otp is valid, and not expired
-        otp_obj = cls.objects.filter(user=user, otp_code=otp_code).first()
+        otp_obj = cls.objects.filter(user=user, otp_code=otp_code).order_by('-created_at').first()
 
         if not otp_obj:
             return False, None
         
         return not cls.is_expired(otp_obj), otp_obj
```

### Comparing `drf-2fa-1.0.2/drf_2fa/settings.py` & `drf-2fa-1.0.3/drf_2fa/settings.py`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.2/drf_2fa/templates/drf_2fa/email/message.html` & `drf-2fa-1.0.3/drf_2fa/templates/drf_2fa/email/message.html`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.2/drf_2fa/views.py` & `drf-2fa-1.0.3/drf_2fa/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,14 +64,22 @@
     serializer_class = LoginSerializer
 
     def get_serializer(self):
         return self.serializer_class
 
     def get_is_2fa_required(self, user):
         return True
+    
+    def get_api_token(self, user):
+        """
+        Generate an api key and send it to the user
+        It can be JWT/Token based on your DRF integration
+        """
+        token, _ = Token.objects.get_or_create(user=user)
+        return token.key
 
     def post(self, request, format=None):
         data = request.data
         serializer = self.get_serializer()(data=data)
 
         serializer.is_valid(raise_exception=True)
         username = serializer.data["username"]
@@ -93,10 +101,9 @@
             otp_required_signal.send(sender=request, user=user)
             return Response({
                 "message": "2FA authentication is required",
                 "user_id": user.id,
                 "is_2fa_required": is_2fa_required
             })
         else:
-            # Generate a auth code and send it to the user
-            token, _ = Token.objects.get_or_create(user=user)
-            return Response({"message": "Login Successfully!", "api_token": token.key})
+            api_token = self.get_api_token(user)
+            return Response({"message": "Login Successfully!", "api_token": api_token})
```

### Comparing `drf-2fa-1.0.2/drf_2fa.egg-info/PKG-INFO` & `drf-2fa-1.0.3/drf_2fa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-2fa
-Version: 1.0.2
+Version: 1.0.3
 Summary: Integrate 2 Factor Authentication in Your Django REST API project easily.
 Home-page: https://github.com/farhad0085/drf-2fa
 Author: Farhad Hossain
 Author-email: farhadhossain0085@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `drf-2fa-1.0.2/drf_2fa.egg-info/SOURCES.txt` & `drf-2fa-1.0.3/drf_2fa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-2fa-1.0.2/setup.py` & `drf-2fa-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (BASE_PATH / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="drf-2fa",
-    version="1.0.2",
+    version="1.0.3",
     description="Integrate 2 Factor Authentication in Your Django REST API project easily.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/farhad0085/drf-2fa",
     author="Farhad Hossain",
     author_email="farhadhossain0085@gmail.com",
     license="MIT",
```

