# Comparing `tmp/ethiack-job-manager-1.0.1rc1.tar.gz` & `tmp/ethiack_job_manager-1.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethiack-job-manager-1.0.1rc1.tar", last modified: Mon Mar 18 14:28:43 2024, max compression
+gzip compressed data, was "ethiack_job_manager-1.0.2rc1.tar", last modified: Wed May 29 11:52:20 2024, max compression
```

## Comparing `ethiack-job-manager-1.0.1rc1.tar` & `ethiack_job_manager-1.0.2rc1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 14:28:43.960513 ethiack-job-manager-1.0.1rc1/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-03-18 14:27:58.000000 ethiack-job-manager-1.0.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7292 2024-03-18 14:28:43.960513 ethiack-job-manager-1.0.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4577 2024-03-18 14:27:58.000000 ethiack-job-manager-1.0.1rc1/README.PYPI.md
--rw-r--r--   0 root         (0) root         (0)     4857 2024-03-18 14:27:58.000000 ethiack-job-manager-1.0.1rc1/README.md
--rw-r--r--   0 root         (0) root         (0)     1772 2024-03-18 14:27:58.000000 ethiack-job-manager-1.0.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-18 14:28:43.960513 ethiack-job-manager-1.0.1rc1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 14:28:43.952512 ethiack-job-manager-1.0.1rc1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 14:28:43.956513 ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager/
--rw-r--r--   0 root         (0) root         (0)     1369 2024-03-18 14:27:58.000000 ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8334 2024-03-18 14:27:58.000000 ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager/cli.py
--rw-r--r--   0 root         (0) root         (0)    13651 2024-03-18 14:27:58.000000 ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager/manager.py
--rw-r--r--   0 root         (0) root         (0)     1122 2024-03-18 14:27:58.000000 ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager/types.py
--rw-r--r--   0 root         (0) root         (0)      450 2024-03-18 14:27:58.000000 ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 14:28:43.960513 ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7292 2024-03-18 14:28:43.000000 ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-03-18 14:28:43.000000 ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 14:28:43.000000 ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2024-03-18 14:28:43.000000 ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      186 2024-03-18 14:28:43.000000 ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-03-18 14:28:43.000000 ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:52:20.104826 ethiack_job_manager-1.0.2rc1/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-29 11:51:58.000000 ethiack_job_manager-1.0.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7292 2024-05-29 11:52:20.104826 ethiack_job_manager-1.0.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4577 2024-05-29 11:51:58.000000 ethiack_job_manager-1.0.2rc1/README.PYPI.md
+-rw-r--r--   0 root         (0) root         (0)     4857 2024-05-29 11:51:58.000000 ethiack_job_manager-1.0.2rc1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-05-29 11:51:58.000000 ethiack_job_manager-1.0.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 11:52:20.104826 ethiack_job_manager-1.0.2rc1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:52:20.100825 ethiack_job_manager-1.0.2rc1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:52:20.100825 ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager/
+-rw-r--r--   0 root         (0) root         (0)     1369 2024-05-29 11:51:58.000000 ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8334 2024-05-29 11:51:58.000000 ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager/cli.py
+-rw-r--r--   0 root         (0) root         (0)    13836 2024-05-29 11:51:58.000000 ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager/manager.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2024-05-29 11:51:58.000000 ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager/types.py
+-rw-r--r--   0 root         (0) root         (0)      450 2024-05-29 11:51:58.000000 ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:52:20.104826 ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7292 2024-05-29 11:52:20.000000 ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-29 11:52:20.000000 ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 11:52:20.000000 ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2024-05-29 11:52:20.000000 ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      186 2024-05-29 11:52:20.000000 ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-29 11:52:20.000000 ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager.egg-info/top_level.txt
```

### Comparing `ethiack-job-manager-1.0.1rc1/LICENSE` & `ethiack_job_manager-1.0.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ethiack-job-manager-1.0.1rc1/PKG-INFO` & `ethiack_job_manager-1.0.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethiack-job-manager
-Version: 1.0.1rc1
+Version: 1.0.2rc1
 Summary: Python package for managing jobs using Ethiack's Public API
 Author-email: Ethiack <hello@ethiack.com>
 License:     MIT License
         
             Copyright (c) Ethiack, Lda.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ethiack-job-manager-1.0.1rc1/README.PYPI.md` & `ethiack_job_manager-1.0.2rc1/README.PYPI.md`

 * *Files identical despite different names*

### Comparing `ethiack-job-manager-1.0.1rc1/README.md` & `ethiack_job_manager-1.0.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `ethiack-job-manager-1.0.1rc1/pyproject.toml` & `ethiack_job_manager-1.0.2rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name =  "ethiack-job-manager"
 authors = [
     {name = "Ethiack", email = "hello@ethiack.com"},
 ]
 description = "Python package for managing jobs using Ethiack's Public API"
 dynamic = ["readme"]
 license = {file = "LICENSE"}
-version = "1.0.1rc1"
+version = "1.0.2rc1"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```

### Comparing `ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager/__init__.py` & `ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager/cli.py` & `ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager/cli.py`

 * *Files identical despite different names*

### Comparing `ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager/manager.py` & `ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,17 +185,20 @@
 
 class CancelJobResponse(pydantic.BaseModel):
     """Response from the cancel job endpoint."""
 
     success: bool
     """Whether the job was successfully cancelled."""
 
-    message: str
+    message: str = pydantic.Field(alias="description")
     """Message from the API."""
 
+    class Config:
+        populate_by_name = True
+
 
 def cancel_job(uuid: str, echo: bool = False) -> CancelJobResponse:
     """Cancel a queued or running job.
 
     Args:
         uuid (str): UUID of the job.
         echo (bool, optional): Echo the response using click. Defaults to False.
@@ -299,17 +302,20 @@
 
 class JobSuccessResponse(pydantic.BaseModel):
     """Response from the job success endpoint."""
 
     success: bool | None = None
     """Whether the job was successful."""
 
-    message: str | None = None
+    message: str | None = pydantic.Field(default=None, alias="description")
     """Message from the API."""
 
+    class Config:
+        populate_by_name = True
+
 
 def get_job_success(uuid: str,
                     severity: str,
                     echo: bool = False,
                     fail: bool = True) -> JobSuccessResponse:
     """Retrieve the success of a job.
```

### Comparing `ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager/types.py` & `ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Types for the Ethiack Job Manager."""
+
 import datetime
+from typing import Annotated
 
 import pydantic
 
-__all__ = ["Service", "Finding", "Job", "JobFindings"]
+from ethiack_job_manager import utils
 
-from typing import Annotated
 
-from ethiack_job_manager import utils
+__all__ = ["Service", "Finding", "Job", "JobFindings"]
+
 
 Url = Annotated[pydantic.AnyUrl,
                 pydantic.AfterValidator(lambda x: str(x).rstrip('/'))]
 
 
 class Service(pydantic.BaseModel):
     """Service model"""
```

### Comparing `ethiack-job-manager-1.0.1rc1/src/ethiack_job_manager.egg-info/PKG-INFO` & `ethiack_job_manager-1.0.2rc1/src/ethiack_job_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethiack-job-manager
-Version: 1.0.1rc1
+Version: 1.0.2rc1
 Summary: Python package for managing jobs using Ethiack's Public API
 Author-email: Ethiack <hello@ethiack.com>
 License:     MIT License
         
             Copyright (c) Ethiack, Lda.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
```

