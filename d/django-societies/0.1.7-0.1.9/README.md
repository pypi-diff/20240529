# Comparing `tmp/django-societies-0.1.7.tar.gz` & `tmp/django-societies-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-societies-0.1.7.tar", last modified: Sun Apr 21 14:54:12 2024, max compression
+gzip compressed data, was "django-societies-0.1.9.tar", last modified: Tue May 28 05:16:39 2024, max compression
```

## Comparing `django-societies-0.1.7.tar` & `django-societies-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-04-21 14:54:12.286090 django-societies-0.1.7/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    35149 2023-12-14 11:32:43.000000 django-societies-0.1.7/LICENSE
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       60 2023-12-14 11:32:43.000000 django-societies-0.1.7/MANIFEST.in
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1604 2024-04-21 14:54:12.286090 django-societies-0.1.7/PKG-INFO
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      517 2023-12-14 11:32:43.000000 django-societies-0.1.7/README.rst
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-04-21 14:54:12.286090 django-societies-0.1.7/django_societies.egg-info/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1604 2024-04-21 14:54:12.000000 django-societies-0.1.7/django_societies.egg-info/PKG-INFO
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      434 2024-04-21 14:54:12.000000 django-societies-0.1.7/django_societies.egg-info/SOURCES.txt
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        1 2024-04-21 14:54:12.000000 django-societies-0.1.7/django_societies.egg-info/dependency_links.txt
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       12 2024-04-21 14:54:12.000000 django-societies-0.1.7/django_societies.egg-info/requires.txt
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       10 2024-04-21 14:54:12.000000 django-societies-0.1.7/django_societies.egg-info/top_level.txt
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       90 2023-12-14 11:32:43.000000 django-societies-0.1.7/pyproject.toml
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1059 2024-04-21 14:54:12.287090 django-societies-0.1.7/setup.cfg
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       38 2023-12-14 11:32:43.000000 django-societies-0.1.7/setup.py
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-04-21 14:54:12.285090 django-societies-0.1.7/societies/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        0 2023-12-14 11:32:43.000000 django-societies-0.1.7/societies/__init__.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       63 2023-12-14 11:32:43.000000 django-societies-0.1.7/societies/admin.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      150 2023-12-14 11:32:43.000000 django-societies-0.1.7/societies/apps.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    10049 2024-03-05 17:13:35.000000 django-societies-0.1.7/societies/choices.py
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-04-21 14:54:12.286090 django-societies-0.1.7/societies/migrations/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        0 2023-12-14 11:32:43.000000 django-societies-0.1.7/societies/migrations/__init__.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     4659 2024-04-21 14:52:24.000000 django-societies-0.1.7/societies/models.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       60 2023-12-14 11:32:43.000000 django-societies-0.1.7/societies/tests.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       63 2023-12-14 11:32:43.000000 django-societies-0.1.7/societies/views.py
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-05-28 05:16:39.987645 django-societies-0.1.9/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    35149 2023-12-14 11:32:43.000000 django-societies-0.1.9/LICENSE
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       60 2023-12-14 11:32:43.000000 django-societies-0.1.9/MANIFEST.in
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1604 2024-05-28 05:16:39.987645 django-societies-0.1.9/PKG-INFO
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      517 2023-12-14 11:32:43.000000 django-societies-0.1.9/README.rst
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-05-28 05:16:39.986645 django-societies-0.1.9/django_societies.egg-info/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1604 2024-05-28 05:16:39.000000 django-societies-0.1.9/django_societies.egg-info/PKG-INFO
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      434 2024-05-28 05:16:39.000000 django-societies-0.1.9/django_societies.egg-info/SOURCES.txt
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        1 2024-05-28 05:16:39.000000 django-societies-0.1.9/django_societies.egg-info/dependency_links.txt
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       12 2024-05-28 05:16:39.000000 django-societies-0.1.9/django_societies.egg-info/requires.txt
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       10 2024-05-28 05:16:39.000000 django-societies-0.1.9/django_societies.egg-info/top_level.txt
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       90 2023-12-14 11:32:43.000000 django-societies-0.1.9/pyproject.toml
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1059 2024-05-28 05:16:39.987645 django-societies-0.1.9/setup.cfg
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       38 2023-12-14 11:32:43.000000 django-societies-0.1.9/setup.py
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-05-28 05:16:39.986645 django-societies-0.1.9/societies/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        0 2023-12-14 11:32:43.000000 django-societies-0.1.9/societies/__init__.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       63 2023-12-14 11:32:43.000000 django-societies-0.1.9/societies/admin.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      150 2023-12-14 11:32:43.000000 django-societies-0.1.9/societies/apps.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    10088 2024-05-28 05:15:24.000000 django-societies-0.1.9/societies/choices.py
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-05-28 05:16:39.986645 django-societies-0.1.9/societies/migrations/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        0 2023-12-14 11:32:43.000000 django-societies-0.1.9/societies/migrations/__init__.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     5611 2024-05-27 21:42:32.000000 django-societies-0.1.9/societies/models.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       60 2023-12-14 11:32:43.000000 django-societies-0.1.9/societies/tests.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       63 2023-12-14 11:32:43.000000 django-societies-0.1.9/societies/views.py
```

### Comparing `django-societies-0.1.7/LICENSE` & `django-societies-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-societies-0.1.7/PKG-INFO` & `django-societies-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-societies
-Version: 0.1.7
+Version: 0.1.9
 Summary: A Django module that provides a collection of abstract models for handling data associated with people, groups, organizations, places, events and means of communication.
 Home-page: https://www.schemefusion.com/
 Author: Onyeibo Oku
 Author-email: onyeibo@schemefusion.com
 License: GPLv3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-societies-0.1.7/README.rst` & `django-societies-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-societies-0.1.7/django_societies.egg-info/PKG-INFO` & `django-societies-0.1.9/django_societies.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-societies
-Version: 0.1.7
+Version: 0.1.9
 Summary: A Django module that provides a collection of abstract models for handling data associated with people, groups, organizations, places, events and means of communication.
 Home-page: https://www.schemefusion.com/
 Author: Onyeibo Oku
 Author-email: onyeibo@schemefusion.com
 License: GPLv3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-societies-0.1.7/setup.cfg` & `django-societies-0.1.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-societies
-version = 0.1.7
+version = 0.1.9
 description = A Django module that provides a collection of abstract models for handling data associated with people, groups, organizations, places, events and means of communication.
 long_description = file: README.rst
 url = https://www.schemefusion.com/
 author = Onyeibo Oku
 author_email = onyeibo@schemefusion.com
 license = GPLv3
 classifiers =
```

### Comparing `django-societies-0.1.7/societies/choices.py` & `django-societies-0.1.9/societies/choices.py`

 * *Files 2% similar despite different names*

```diff
@@ -391,33 +391,35 @@
     (2, "Female"),
 ]
 
 TIES = [
     (0, "Unspecified"),
     (1, "Father"),
     (2, "Mother"),
-    (3, "Sister"),
-    (4, "Brother"),
+    (3, "Brother"),
+    (4, "Sister"),
     (5, "Cousin"),
-    (6, "Niece"),
-    (7, "Nephew"),
-    (8, "Aunt"),
-    (9, "Uncle"),
+    (6, "Nephew"),
+    (7, "Niece"),
+    (8, "Uncle"),
+    (9, "Aunt"),
     (10, "Parent"),
     (11, "Father-in-Law"),
     (12, "Mother-in-Law"),
-    (13, "Sister-in-Law"),
-    (14, "Brother-in-Law"),
-    (15, "Employer"),
-    (16, "Spouse"),
-    (17, "Son"),
-    (18, "Daughter"),
-    (19, "Pastor"),
-    (20, "Priest"),
-    (21, "Non-Profit Organization"),
-    (22, "Son-in-Law"),
-    (23, "Daughter-in-Law"),
-    (24, "Local Ordinary"),
-    (25, "Self"),
-    (26, "Corporate Sponsor"),
-    (27, "Group Sponsor"),
+    (13, "Son-in-Law"),
+    (14, "Daughter-in-Law"),
+    (15, "Brother-in-Law"),
+    (16, "Sister-in-Law"),
+    (17, "Husband"),
+    (18, "Wife"),
+    (19, "Spouse"),
+    (20, "Son"),
+    (21, "Daughter"),
+    (22, "Self"),
+    (23, "Pastor"),
+    (24, "Priest"),
+    (25, "Local Ordinary"),
+    (26, "Employer"),
+    (27, "Non-Profit Organization"),
+    (28, "Corporate Sponsor"),
+    (29, "Group Sponsor"),
 ]
```

### Comparing `django-societies-0.1.7/societies/models.py` & `django-societies-0.1.9/societies/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,14 +22,44 @@
     class Meta:
         """Meta class for this Model"""
 
         abstract = True
         managed = True
 
 
+class MinimalPersonContact(models.Model):
+    """Essentials for Contacting a Person"""
+
+    address = models.CharField(max_length=255)
+    closest_landmark =  models.CharField(blank=True, null=True, max_length=255)
+    first_name = models.CharField(max_length=255)
+    last_name = models.CharField(max_length=255)
+    middle_name = models.CharField(blank=True, null=True, max_length=255)
+    phone = models.CharField(max_length=255)
+
+    def __str__(self):
+        """Print String for this Model"""
+
+        return self.last_name
+
+    @property
+    def name(self): 
+        """Return the fullname of this Person""" 
+        
+        prefix = self.prefix if self.prefix else ""
+        middle_name = self.middle_name if self.middle_name else ""
+        return f"{prefix} {self.last_name}, {self.first_name} {middle_name}" 
+
+    class Meta:
+        """Meta class for this Model"""
+
+        abstract = True
+        managed = True
+
+
 class Email(models.Model):
     """A Person's Email Address"""
 
     email = models.EmailField(max_length=255, blank=True, null=True)
     typefk = models.IntegerField(default=1, choices=choices.LOCATION_TYPES)
 
     class Meta:
@@ -38,15 +68,15 @@
         abstract = True
         managed = True
 
 
 class Event(models.Model):
     """An event in a Person's Life"""
 
-    authority = models.CharField(max_length=255)
+    authority = models.CharField(blank=True, null=True, max_length=255)
     end_date = models.DateField(blank=True, null=True)
     note = models.CharField(max_length=255, blank=True, null=True)
     proof = models.IntegerField(
         default=0,
         choices=choices.EVENT_PROOFS
     )
     reference = models.CharField(max_length=255, blank=True, null=True)
```

