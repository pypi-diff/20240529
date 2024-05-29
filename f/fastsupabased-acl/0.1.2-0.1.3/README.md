# Comparing `tmp/fastsupabased_acl-0.1.2.tar.gz` & `tmp/fastsupabased_acl-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastsupabased_acl-0.1.2.tar", max compression
+gzip compressed data, was "fastsupabased_acl-0.1.3.tar", max compression
```

## Comparing `fastsupabased_acl-0.1.2.tar` & `fastsupabased_acl-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      783 2024-05-28 15:17:26.542425 fastsupabased_acl-0.1.2/README.md
--rw-r--r--   0        0        0      925 2024-05-28 15:17:26.542425 fastsupabased_acl-0.1.2/fastsupabased_acl/__init__.py
--rw-r--r--   0        0        0      402 2024-05-28 15:17:26.542425 fastsupabased_acl-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 fastsupabased_acl-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      783 2024-05-29 21:22:38.565591 fastsupabased_acl-0.1.3/README.md
+-rw-r--r--   0        0        0      929 2024-05-29 21:22:38.565591 fastsupabased_acl-0.1.3/fastsupabased_acl/__init__.py
+-rw-r--r--   0        0        0      402 2024-05-29 21:22:38.565591 fastsupabased_acl-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 fastsupabased_acl-0.1.3/PKG-INFO
```

### Comparing `fastsupabased_acl-0.1.2/README.md` & `fastsupabased_acl-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fastsupabased_acl-0.1.2/fastsupabased_acl/__init__.py` & `fastsupabased_acl-0.1.3/fastsupabased_acl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,11 +21,11 @@
 
 
 class FastSupabasedACL:
     def __init__(self, role: List[str] = ["authenticated"]):
         self.role = role
 
     def __call__(self, user = Depends(token_auth)):
-        if self.role != user.user.role:
+        if self.role not in user.user.role:
             raise HTTPException(status_code=403, detail="Unauthorized")
 
         return user
```

### Comparing `fastsupabased_acl-0.1.2/PKG-INFO` & `fastsupabased_acl-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsupabased-acl
-Version: 0.1.2
+Version: 0.1.3
 Summary: FastAPI Dependency for Supabase-based ACL using Supabase Roles
 Author: Vinicius Mesel
 Author-email: 4984147+vmesel@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

