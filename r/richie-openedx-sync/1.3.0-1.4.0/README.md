# Comparing `tmp/richie_openedx_sync-1.3.0.tar.gz` & `tmp/richie_openedx_sync-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richie_openedx_sync-1.3.0.tar", last modified: Thu Apr 18 13:47:52 2024, max compression
+gzip compressed data, was "richie_openedx_sync-1.4.0.tar", last modified: Wed May 29 10:47:38 2024, max compression
```

## Comparing `richie_openedx_sync-1.3.0.tar` & `richie_openedx_sync-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:52.969602 richie_openedx_sync-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-18 13:47:52.965602 richie_openedx_sync-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:52.965602 richie_openedx_sync-1.3.0/richie_openedx_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:52.965602 richie_openedx_sync-1.3.0/richie_openedx_sync/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:52.965602 richie_openedx_sync-1.3.0/richie_openedx_sync/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/management/commands/sync_courses_to_richie.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:52.965602 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-18 13:47:52.000000 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 13:47:52.000000 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:47:52.000000 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-18 13:47:52.000000 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:47:52.000000 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 13:47:52.000000 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-18 13:47:52.000000 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:47:52.969602 richie_openedx_sync-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:47:38.481957 richie_openedx_sync-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-29 10:47:34.000000 richie_openedx_sync-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 10:47:34.000000 richie_openedx_sync-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-29 10:47:38.481957 richie_openedx_sync-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-29 10:47:34.000000 richie_openedx_sync-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:47:38.481957 richie_openedx_sync-1.4.0/richie_openedx_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-29 10:47:34.000000 richie_openedx_sync-1.4.0/richie_openedx_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 10:47:34.000000 richie_openedx_sync-1.4.0/richie_openedx_sync/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:47:38.481957 richie_openedx_sync-1.4.0/richie_openedx_sync/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:47:34.000000 richie_openedx_sync-1.4.0/richie_openedx_sync/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:47:38.481957 richie_openedx_sync-1.4.0/richie_openedx_sync/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:47:34.000000 richie_openedx_sync-1.4.0/richie_openedx_sync/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-29 10:47:34.000000 richie_openedx_sync-1.4.0/richie_openedx_sync/management/commands/sync_courses_to_richie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-29 10:47:34.000000 richie_openedx_sync-1.4.0/richie_openedx_sync/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-29 10:47:34.000000 richie_openedx_sync-1.4.0/richie_openedx_sync/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-29 10:47:34.000000 richie_openedx_sync-1.4.0/richie_openedx_sync/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:47:38.481957 richie_openedx_sync-1.4.0/richie_openedx_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-29 10:47:38.000000 richie_openedx_sync-1.4.0/richie_openedx_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-29 10:47:38.000000 richie_openedx_sync-1.4.0/richie_openedx_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:47:38.000000 richie_openedx_sync-1.4.0/richie_openedx_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 10:47:38.000000 richie_openedx_sync-1.4.0/richie_openedx_sync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:47:38.000000 richie_openedx_sync-1.4.0/richie_openedx_sync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-29 10:47:38.000000 richie_openedx_sync-1.4.0/richie_openedx_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:47:38.481957 richie_openedx_sync-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-29 10:47:34.000000 richie_openedx_sync-1.4.0/setup.py
```

### Comparing `richie_openedx_sync-1.3.0/LICENSE` & `richie_openedx_sync-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `richie_openedx_sync-1.3.0/PKG-INFO` & `richie_openedx_sync-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richie-openedx-sync
-Version: 1.3.0
+Version: 1.4.0
 Summary: Richie Open edX Synchronization application
 Home-page: https://github.com/fccn/richie-openedx-sync
 Author: FCT|FCCN NAU
 Author-email: info@nau.edu.pt
 License: AGPL 3.0
 Keywords: Django,Open edX,MOOC,Richie
 Platform: any
@@ -13,18 +13,14 @@
 Classifier: Framework :: Django :: 2.2
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: edx-celeryutils
-Requires-Dist: requests
-Requires-Dist: celery
-Requires-Dist: django-celery
 
 # Richie Open edX Synchronization application
 
 ## Overview
 
 The aim of this Django application is to synchronize the Open edX courses to the Richie marketing site.
 Whenever a course schedule or details are updated on Studio a hook is run that sends the updated information to Richie.
```

### Comparing `richie_openedx_sync-1.3.0/README.md` & `richie_openedx_sync-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `richie_openedx_sync-1.3.0/richie_openedx_sync/apps.py` & `richie_openedx_sync-1.4.0/richie_openedx_sync/apps.py`

 * *Files identical despite different names*

### Comparing `richie_openedx_sync-1.3.0/richie_openedx_sync/management/commands/sync_courses_to_richie.py` & `richie_openedx_sync-1.4.0/richie_openedx_sync/management/commands/sync_courses_to_richie.py`

 * *Files identical despite different names*

### Comparing `richie_openedx_sync-1.3.0/richie_openedx_sync/signals.py` & `richie_openedx_sync-1.4.0/richie_openedx_sync/signals.py`

 * *Files identical despite different names*

### Comparing `richie_openedx_sync-1.3.0/richie_openedx_sync/tasks.py` & `richie_openedx_sync-1.4.0/richie_openedx_sync/tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,105 +31,95 @@
     log.debug("Entering richie update course on publish")
 
     course_id = kwargs["course_id"]
     course_key = CourseKey.from_string(course_id)
     course = modulestore().get_course(course_key)
 
     if not course:
-        raise ValueError(
-            "No course found with the course_id '{}'".format(course_id))
+        raise ValueError("No course found with the course_id '{}'".format(course_id))
 
     org = course_key.org
-    edxapp_domain = configuration_helpers.get_value_for_org(
+
+    hooks = configuration_helpers.get_value_for_org(
+        org,
+        "RICHIE_OPENEDX_SYNC_COURSE_HOOKS",
+        getattr(settings, "RICHIE_OPENEDX_SYNC_COURSE_HOOKS"),
+    )
+    if len(hooks) == 0:
+        log.info("No richie course hook found for organization '%s'. Please configure the "
+            "'RICHIE_OPENEDX_SYNC_COURSE_HOOKS' setting or as site configuration", org)
+        return {}
+
+    lms_domain = configuration_helpers.get_value_for_org(
         org, "LMS_BASE", settings.LMS_BASE
     )
     course_start = course.start and course.start.isoformat()
     course_end = course.end and course.end.isoformat()
     enrollment_start = course.enrollment_start and course.enrollment_start.isoformat()
     enrollment_end = course.enrollment_end and course.enrollment_end.isoformat()
 
     # Enrollment start date should fallback to course start date, by default Open edX uses the
     # course start date for the enrollment start date when the enrollment start date isn't defined.
     enrollment_start = enrollment_start or course_start
 
-    data = {
-        "resource_link": "https://{:s}/courses/{!s}/info".format(
-            edxapp_domain, course_key
-        ),
-        "start": course_start,
-        "end": course_end,
-        "enrollment_start": enrollment_start,
-        "enrollment_end": enrollment_end,
-        "languages": [course.language or settings.LANGUAGE_CODE],
-        "enrollment_count": CourseEnrollment.objects.filter(
-            course_id=course_id
-        ).count(),
-        "catalog_visibility": course.catalog_visibility,
-    }
-
-    hooks = configuration_helpers.get_value_for_org(
-        org,
-        "RICHIE_OPENEDX_SYNC_COURSE_HOOKS",
-        getattr(settings, "RICHIE_OPENEDX_SYNC_COURSE_HOOKS", []),
-    )
-    if not hooks:
-        msg = (
-            "No richie course hook found for organization '{}'. Please configure the "
-            "'RICHIE_OPENEDX_SYNC_COURSE_HOOKS' setting or as site configuration"
-        ).format(org)
-        log.info(msg)
-        return {}
-
-    log_requests = configuration_helpers.get_value_for_org(
-        org,
-        "RICHIE_OPENEDX_SYNC_LOG_REQUESTS",
-        getattr(settings, "RICHIE_OPENEDX_SYNC_LOG_REQUESTS", False),
-    )
+    enrollment_count = None
 
     result = {}
 
     for hook in hooks:
+        # calculate enrollment count just once per hook
+        if not enrollment_count:
+            enrollment_count = CourseEnrollment.objects.filter(
+                course_id=course_id
+            ).count()
+
+        resource_link = hook.get(
+            "resource_link_template", "https://{lms_domain}/courses/{course_id}/info"
+        ).format(lms_domain=lms_domain, course_id=str(course_id))
+
+        data = {
+            "resource_link": resource_link,
+            "start": course_start,
+            "end": course_end,
+            "enrollment_start": enrollment_start,
+            "enrollment_end": enrollment_end,
+            "languages": [course.language or settings.LANGUAGE_CODE],
+            "enrollment_count": enrollment_count,
+            "catalog_visibility": course.catalog_visibility,
+        }
+
         signature = hmac.new(
             hook["secret"].encode("utf-8"),
             msg=json.dumps(data).encode("utf-8"),
             digestmod=hashlib.sha256,
         ).hexdigest()
 
-        richie_url = hook.get("url")
+        richie_url = str(hook.get("url"))
         timeout = int(hook.get("timeout", 20))
 
         try:
+            log.info("Sending to Richie %s the data %s", richie_url, str(data))
             response = requests.post(
                 richie_url,
                 json=data,
-                headers={
-                    "Authorization": "SIG-HMAC-SHA256 {:s}".format(signature)},
+                headers={"Authorization": "SIG-HMAC-SHA256 {signature}".format(signature=signature)},
                 timeout=timeout,
             )
             response.raise_for_status()
             result[richie_url] = True
-            if log_requests:
-                status_code = response.status_code
-                msg = "Synchronized the course {} to richie site {} it returned the HTTP status code {}".format(
-                    course_key, richie_url, status_code
-                )
-                log.info(msg)
-                log.info(response.content)
+
+            log.info("Synchronized the course %s to richie site %s it returned the HTTP status code %d response content: %s".format(
+                course_id, richie_url, response.status_code, response.content
+            ))
         except requests.exceptions.HTTPError as e:
-            status_code = response.status_code
-            msg = "Error synchronizing course {} to richie site {} it returned the HTTP status code {}".format(
-                course_key, richie_url, status_code
+            log.warning("Error synchronizing course %s to richie site %s it returned the HTTP status code %d with response content of %s",
+                course_id, richie_url, response.status_code, response.content
             )
             log.warning(e, exc_info=True)
-            log.warning(msg)
-            log.warning(response.content)
             result[richie_url] = False
 
         except requests.exceptions.RequestException as e:
-            msg = "Error synchronizing course {} to richie site {}".format(
-                course_key, richie_url
-            )
+            log.warning("Error synchronizing course %s to richie site %s", course_id, richie_url)
             log.warning(e, exc_info=True)
-            log.warning(msg)
             result[richie_url] = False
 
     return result
```

### Comparing `richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/PKG-INFO` & `richie_openedx_sync-1.4.0/richie_openedx_sync.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richie-openedx-sync
-Version: 1.3.0
+Version: 1.4.0
 Summary: Richie Open edX Synchronization application
 Home-page: https://github.com/fccn/richie-openedx-sync
 Author: FCT|FCCN NAU
 Author-email: info@nau.edu.pt
 License: AGPL 3.0
 Keywords: Django,Open edX,MOOC,Richie
 Platform: any
@@ -13,18 +13,14 @@
 Classifier: Framework :: Django :: 2.2
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: edx-celeryutils
-Requires-Dist: requests
-Requires-Dist: celery
-Requires-Dist: django-celery
 
 # Richie Open edX Synchronization application
 
 ## Overview
 
 The aim of this Django application is to synchronize the Open edX courses to the Richie marketing site.
 Whenever a course schedule or details are updated on Studio a hook is run that sends the updated information to Richie.
```

### Comparing `richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/SOURCES.txt` & `richie_openedx_sync-1.4.0/richie_openedx_sync.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 richie_openedx_sync/signals.py
 richie_openedx_sync/tasks.py
 richie_openedx_sync.egg-info/PKG-INFO
 richie_openedx_sync.egg-info/SOURCES.txt
 richie_openedx_sync.egg-info/dependency_links.txt
 richie_openedx_sync.egg-info/entry_points.txt
 richie_openedx_sync.egg-info/not-zip-safe
-richie_openedx_sync.egg-info/requires.txt
 richie_openedx_sync.egg-info/top_level.txt
 richie_openedx_sync/management/__init__.py
 richie_openedx_sync/management/commands/__init__.py
 richie_openedx_sync/management/commands/sync_courses_to_richie.py
```

### Comparing `richie_openedx_sync-1.3.0/setup.py` & `richie_openedx_sync-1.4.0/setup.py`

 * *Files identical despite different names*

