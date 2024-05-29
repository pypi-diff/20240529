# Comparing `tmp/aind_data_transfer_models-0.3.0.tar.gz` & `tmp/aind_data_transfer_models-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_data_transfer_models-0.3.0.tar", last modified: Sat May 18 00:10:59 2024, max compression
+gzip compressed data, was "aind_data_transfer_models-0.4.0.tar", last modified: Wed May 29 01:02:21 2024, max compression
```

## Comparing `aind_data_transfer_models-0.3.0.tar` & `aind_data_transfer_models-0.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.296639 aind_data_transfer_models-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.288639 aind_data_transfer_models-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.292639 aind_data_transfer_models-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.292639 aind_data_transfer_models-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-18 00:10:59.296639 aind_data_transfer_models-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.292639 aind_data_transfer_models-0.3.0/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.292639 aind_data_transfer_models-0.3.0/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.292639 aind_data_transfer_models-0.3.0/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 00:10:59.296639 aind_data_transfer_models-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.288639 aind_data_transfer_models-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.292639 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.296639 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-18 00:10:59.000000 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-18 00:10:59.000000 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 00:10:59.000000 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-18 00:10:59.000000 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-18 00:10:59.000000 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.292639 aind_data_transfer_models-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:02:21.628874 aind_data_transfer_models-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:02:21.624874 aind_data_transfer_models-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:02:21.624874 aind_data_transfer_models-0.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:02:21.624874 aind_data_transfer_models-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-29 01:02:21.628874 aind_data_transfer_models-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:02:21.624874 aind_data_transfer_models-0.4.0/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:02:21.624874 aind_data_transfer_models-0.4.0/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:02:21.628874 aind_data_transfer_models-0.4.0/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 01:02:21.628874 aind_data_transfer_models-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:02:21.624874 aind_data_transfer_models-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:02:21.628874 aind_data_transfer_models-0.4.0/src/aind_data_transfer_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-29 01:02:08.000000 aind_data_transfer_models-0.4.0/src/aind_data_transfer_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/src/aind_data_transfer_models/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:02:21.628874 aind_data_transfer_models-0.4.0/src/aind_data_transfer_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-29 01:02:21.000000 aind_data_transfer_models-0.4.0/src/aind_data_transfer_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-29 01:02:21.000000 aind_data_transfer_models-0.4.0/src/aind_data_transfer_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 01:02:21.000000 aind_data_transfer_models-0.4.0/src/aind_data_transfer_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-29 01:02:21.000000 aind_data_transfer_models-0.4.0/src/aind_data_transfer_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 01:02:21.000000 aind_data_transfer_models-0.4.0/src/aind_data_transfer_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:02:21.628874 aind_data_transfer_models-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-05-29 01:02:07.000000 aind_data_transfer_models-0.4.0/tests/test_core.py
```

### Comparing `aind_data_transfer_models-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_data_transfer_models-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_data_transfer_models-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/.github/ISSUE_TEMPLATE/user-story.md` & `aind_data_transfer_models-0.4.0/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/.github/workflows/tag_and_publish.yml` & `aind_data_transfer_models-0.4.0/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/.github/workflows/test_and_lint.yml` & `aind_data_transfer_models-0.4.0/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/.gitignore` & `aind_data_transfer_models-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/LICENSE` & `aind_data_transfer_models-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/PKG-INFO` & `aind_data_transfer_models-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-data-transfer-models
-Version: 0.3.0
+Version: 0.4.0
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_data_transfer_models-0.3.0/README.md` & `aind_data_transfer_models-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/doc_template/Makefile` & `aind_data_transfer_models-0.4.0/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/doc_template/make.bat` & `aind_data_transfer_models-0.4.0/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/doc_template/source/_static/dark-logo.svg` & `aind_data_transfer_models-0.4.0/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/doc_template/source/_static/favicon.ico` & `aind_data_transfer_models-0.4.0/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/doc_template/source/_static/light-logo.svg` & `aind_data_transfer_models-0.4.0/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/doc_template/source/conf.py` & `aind_data_transfer_models-0.4.0/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/pyproject.toml` & `aind_data_transfer_models-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/src/aind_data_transfer_models/core.py` & `aind_data_transfer_models-0.4.0/src/aind_data_transfer_models/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from pydantic import (
     ConfigDict,
     EmailStr,
     Field,
     ValidationInfo,
     computed_field,
     field_validator,
+    model_validator,
 )
 from pydantic_settings import BaseSettings
 
 
 class EmailNotificationType(str, Enum):
     """Types of email notifications a user can select"""
 
@@ -110,29 +111,42 @@
         else:
             return False
 
 
 class BasicUploadJobConfigs(BaseSettings):
     """Configuration for the basic upload job"""
 
-    # Allow users to pass in extra fields
-    model_config = ConfigDict(extra="allow", use_enum_values=True)
+    model_config = ConfigDict(use_enum_values=True)
 
     # Need some way to extract abbreviations. Maybe a public method can be
     # added to the Platform class
     _PLATFORM_MAP: ClassVar = {
         p().abbreviation.upper(): p().abbreviation for p in Platform._ALL
     }
     _DATETIME_PATTERN1: ClassVar = re.compile(
         r"^\d{4}-\d{2}-\d{2}[ |T]\d{2}:\d{2}:\d{2}$"
     )
     _DATETIME_PATTERN2: ClassVar = re.compile(
         r"^\d{1,2}/\d{1,2}/\d{4} \d{1,2}:\d{2}:\d{2} [APap][Mm]$"
     )
 
+    user_email: Optional[EmailStr] = Field(
+        default=None,
+        description=(
+            "Optional email address to receive job status notifications"
+        ),
+    )
+
+    email_notification_types: Optional[Set[EmailNotificationType]] = Field(
+        default=None,
+        description=(
+            "Types of job statuses to receive email notifications about"
+        ),
+    )
+
     project_name: str = Field(
         ..., description="Name of project", title="Project Name"
     )
     process_capsule_id: Optional[str] = Field(
         None,
         description="Use custom codeocean capsule or pipeline id",
         title="Process Capsule ID",
@@ -243,22 +257,41 @@
             return datetime_val
 
 
 class SubmitJobRequest(BaseSettings):
     """Main request that will be sent to the backend. Bundles jobs into a list
     and allows a user to add an email address to receive notifications."""
 
+    model_config = ConfigDict(use_enum_values=True)
+
     user_email: Optional[EmailStr] = Field(
         default=None,
         description=(
             "Optional email address to receive job status notifications"
         ),
     )
     email_notification_types: Set[EmailNotificationType] = Field(
         default={EmailNotificationType.FAIL},
         description=(
             "Types of job statuses to receive email notifications about"
         ),
     )
     upload_jobs: List[BasicUploadJobConfigs] = Field(
-        ..., description="List of upload jobs to process"
+        ...,
+        description="List of upload jobs to process. Max of 1000 at a time.",
+        min_items=1,
+        max_items=1000,
     )
+
+    @model_validator(mode="after")
+    def propagate_email_settings(self):
+        """Propagate email settings from global to individual jobs"""
+        global_email_user = self.user_email
+        global_email_notification_types = self.email_notification_types
+        for upload_job in self.upload_jobs:
+            if global_email_user is not None and upload_job.user_email is None:
+                upload_job.user_email = global_email_user
+            if upload_job.email_notification_types is None:
+                upload_job.email_notification_types = (
+                    global_email_notification_types
+                )
+        return self
```

### Comparing `aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/PKG-INFO` & `aind_data_transfer_models-0.4.0/src/aind_data_transfer_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-data-transfer-models
-Version: 0.3.0
+Version: 0.4.0
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/SOURCES.txt` & `aind_data_transfer_models-0.4.0/src/aind_data_transfer_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.3.0/tests/test_core.py` & `aind_data_transfer_models-0.4.0/tests/test_core.py`

 * *Files 17% similar despite different names*

```diff
@@ -157,15 +157,15 @@
                 acq_datetime="2020/05/23T09:05:03",
                 **self.base_configs,
             )
         error_msg = json.loads(e.exception.json())[0]["msg"]
         self.assertTrue("Value error, Incorrect datetime format" in error_msg)
 
     def test_parse_platform_string(self):
-        """Tests that an error is raised if an unknown platform is used"""
+        """Tests platform can be parsed from string"""
 
         base_configs = self.example_configs.model_dump(
             exclude={
                 "platform": True,
                 "s3_prefix": True,
                 "modalities": {"__all__": {"output_folder_name"}},
             }
@@ -206,61 +206,128 @@
                 ),
             ],
             subject_id="123456",
             acq_datetime=datetime(2020, 10, 13, 13, 10, 10),
         )
         cls.example_upload_config = example_upload_config
 
+    def test_min_items(self):
+        """Tests error is raised if no job list is empty"""
+
+        with self.assertRaises(ValidationError) as e:
+            SubmitJobRequest(upload_jobs=[])
+        expected_message = (
+            "List should have at least 1 item after validation, not 0"
+        )
+        actual_message = json.loads(e.exception.json())[0]["msg"]
+        self.assertEqual(1, len(json.loads(e.exception.json())))
+        self.assertEqual(expected_message, actual_message)
+
+    def test_max_items(self):
+        """Tests error is raised if job list is greater than maximum allowed"""
+
+        upload_job = BasicUploadJobConfigs(
+            **self.example_upload_config.model_dump(round_trip=True)
+        )
+
+        with self.assertRaises(ValidationError) as e:
+            SubmitJobRequest(upload_jobs=[upload_job for _ in range(0, 1001)])
+        expected_message = (
+            "List should have at most 1000 items after validation, not 1001"
+        )
+        actual_message = json.loads(e.exception.json())[0]["msg"]
+        self.assertEqual(1, len(json.loads(e.exception.json())))
+        self.assertEqual(expected_message, actual_message)
+
     def test_default_settings(self):
         """Tests defaults are set correctly."""
 
-        job_settings = SubmitJobRequest(
-            upload_jobs=[self.example_upload_config]
+        upload_job = BasicUploadJobConfigs(
+            **self.example_upload_config.model_dump(round_trip=True)
         )
+
+        job_settings = SubmitJobRequest(upload_jobs=[upload_job])
         self.assertIsNone(job_settings.user_email)
         self.assertEqual(
             {EmailNotificationType.FAIL}, job_settings.email_notification_types
         )
-        self.assertEqual(
-            [self.example_upload_config], job_settings.upload_jobs
-        )
 
     def test_non_default_settings(self):
         """Tests user can modify the settings."""
+        upload_job_configs = self.example_upload_config.model_dump(
+            round_trip=True
+        )
 
         job_settings = SubmitJobRequest(
             user_email="abc@acme.com",
             email_notification_types={
                 EmailNotificationType.BEGIN,
                 EmailNotificationType.FAIL,
             },
-            upload_jobs=[self.example_upload_config],
+            upload_jobs=[BasicUploadJobConfigs(**upload_job_configs)],
         )
         self.assertEqual("abc@acme.com", job_settings.user_email)
         self.assertEqual(
             {EmailNotificationType.BEGIN, EmailNotificationType.FAIL},
             job_settings.email_notification_types,
         )
-        self.assertEqual(
-            [self.example_upload_config], job_settings.upload_jobs
-        )
 
     def test_email_validation(self):
         """Tests user can not input invalid email address."""
 
+        upload_job_configs = self.example_upload_config.model_dump(
+            round_trip=True
+        )
         with self.assertRaises(ValidationError) as e:
             SubmitJobRequest(
                 user_email="some user",
-                upload_jobs=[self.example_upload_config],
+                upload_jobs=[BasicUploadJobConfigs(**upload_job_configs)],
             )
         expected_error_message = (
             "value is not a valid email address:"
             " The email address is not valid. It must have exactly one @-sign."
         )
         actual_error_message = json.loads(e.exception.json())[0]["msg"]
         # Check only 1 validation error is raised
         self.assertEqual(1, len(json.loads(e.exception.json())))
         self.assertEqual(expected_error_message, actual_error_message)
 
+    def test_propagate_email_settings(self):
+        """Tests global email settings is propagated to individual jobs."""
+
+        example_job_configs = self.example_upload_config.model_dump(
+            exclude={"user_email", "email_notification_types"}, round_trip=True
+        )
+        new_job = BasicUploadJobConfigs(
+            user_email="xyz@acme.org",
+            email_notification_types=[EmailNotificationType.ALL],
+            **example_job_configs,
+        )
+        job_settings = SubmitJobRequest(
+            user_email="abc@acme.org",
+            email_notification_types={
+                EmailNotificationType.BEGIN,
+                EmailNotificationType.FAIL,
+            },
+            upload_jobs=[
+                new_job,
+                BasicUploadJobConfigs(**example_job_configs),
+            ],
+        )
+
+        self.assertEqual(
+            "xyz@acme.org", job_settings.upload_jobs[0].user_email
+        )
+        self.assertEqual(
+            "abc@acme.org", job_settings.upload_jobs[1].user_email
+        )
+        self.assertEqual(
+            {"all"}, job_settings.upload_jobs[0].email_notification_types
+        )
+        self.assertEqual(
+            {"begin", "fail"},
+            job_settings.upload_jobs[1].email_notification_types,
+        )
+
 
 if __name__ == "__main__":
     unittest.main()
```

