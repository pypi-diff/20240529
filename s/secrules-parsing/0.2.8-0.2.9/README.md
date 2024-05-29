# Comparing `tmp/secrules_parsing-0.2.8.tar.gz` & `tmp/secrules_parsing-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrules_parsing-0.2.8.tar", max compression
+gzip compressed data, was "secrules_parsing-0.2.9.tar", max compression
```

## Comparing `secrules_parsing-0.2.8.tar` & `secrules_parsing-0.2.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-04-10 20:35:22.470623 secrules_parsing-0.2.8/LICENSE
--rw-r--r--   0        0        0     4926 2024-04-10 20:35:22.470623 secrules_parsing-0.2.8/README.md
--rw-r--r--   0        0        0     1223 2024-04-10 20:35:36.918624 secrules_parsing-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       76 2024-04-10 20:35:22.474623 secrules_parsing-0.2.8/src/secrules_parsing/__init__.py
--rw-r--r--   0        0        0     2655 2024-04-10 20:35:22.474623 secrules_parsing-0.2.8/src/secrules_parsing/cli.py
--rw-r--r--   0        0        0        0 2024-04-10 20:35:22.474623 secrules_parsing-0.2.8/src/secrules_parsing/model/__init__.py
--rw-r--r--   0        0        0    11744 2024-04-10 20:35:22.474623 secrules_parsing-0.2.8/src/secrules_parsing/model/secrules.tx
--rwxr-xr-x   0        0        0     3564 2024-04-10 20:35:22.474623 secrules_parsing-0.2.8/src/secrules_parsing/parser.py
--rw-r--r--   0        0        0      291 2024-04-10 20:35:22.474623 secrules_parsing-0.2.8/src/secrules_parsing/resources.py
--rw-r--r--   0        0        0     6122 1970-01-01 00:00:00.000000 secrules_parsing-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-11 06:57:39.291994 secrules_parsing-0.2.9/LICENSE
+-rw-r--r--   0        0        0     4926 2024-04-11 06:57:39.291994 secrules_parsing-0.2.9/README.md
+-rw-r--r--   0        0        0     1223 2024-04-11 06:57:54.252136 secrules_parsing-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0       76 2024-04-11 06:57:39.291994 secrules_parsing-0.2.9/src/secrules_parsing/__init__.py
+-rw-r--r--   0        0        0     2655 2024-04-11 06:57:39.291994 secrules_parsing-0.2.9/src/secrules_parsing/cli.py
+-rw-r--r--   0        0        0        0 2024-04-11 06:57:39.291994 secrules_parsing-0.2.9/src/secrules_parsing/model/__init__.py
+-rw-r--r--   0        0        0    11744 2024-04-11 06:57:39.291994 secrules_parsing-0.2.9/src/secrules_parsing/model/secrules.tx
+-rwxr-xr-x   0        0        0     3564 2024-04-11 06:57:39.291994 secrules_parsing-0.2.9/src/secrules_parsing/parser.py
+-rw-r--r--   0        0        0      291 2024-04-11 06:57:39.291994 secrules_parsing-0.2.9/src/secrules_parsing/resources.py
+-rw-r--r--   0        0        0     6122 1970-01-01 00:00:00.000000 secrules_parsing-0.2.9/PKG-INFO
```

### Comparing `secrules_parsing-0.2.8/LICENSE` & `secrules_parsing-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `secrules_parsing-0.2.8/README.md` & `secrules_parsing-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `secrules_parsing-0.2.8/pyproject.toml` & `secrules_parsing-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secrules-parsing"
-version = "v0.2.8"
+version = "v0.2.9"
 description = "ModSecurity DSL Parser package using textX"
 authors = [
     "Felipe Zipitria <felipe.zipitria@owasp.org>"
 ]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/coreruleset/secrules_parsing"
```

### Comparing `secrules_parsing-0.2.8/src/secrules_parsing/cli.py` & `secrules_parsing-0.2.9/src/secrules_parsing/cli.py`

 * *Files identical despite different names*

### Comparing `secrules_parsing-0.2.8/src/secrules_parsing/model/secrules.tx` & `secrules_parsing-0.2.9/src/secrules_parsing/model/secrules.tx`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     'FILES_TMP_CONTENT' | 'HIGHEST_SEVERITY' | 'INBOUND_DATA_ERROR' | 'MATCHED_VAR_NAME' |
     'MODSEC_BUILD' | 'MULTIPART_CRLF_LF_LINES' | 'MULTIPART_FILENAME' | 'MULTIPART_NAME' |
     'MULTIPART_STRICT_ERROR' | 'MULTIPART_UNMATCHED_BOUNDARY' | 'OUTBOUND_DATA_ERROR' | 
     'PATH_INFO' | 'PERF_ALL' | 'PERF_COMBINED' | 'PERF_GC' | 'PERF_LOGGING' | 'PERF_PHASE1' |
     'PERF_PHASE2' | 'PERF_PHASE3' | 'PERF_PHASE4' | 'PERF_PHASE5' | 'PERF_SREAD' | 'PERF_SWRITE' |
     'QUERY_STRING' | 'REMOTE_ADDR' | 'REMOTE_HOST' | 'REMOTE_PORT' | 'REMOTE_USER' |
     'REQBODY_ERROR' | 'REQBODY_ERROR_MSG' | 'REQBODY_PROCESSOR' | 'REQUEST_BASENAME' |
-    'REQUEST_BODY' | 'REQUEST_BODY_LENGTH' | 'REQUEST_FILENAME' | 'REQUEST_LINE' |
+    'REQUEST_BODY_LENGTH' | 'REQUEST_BODY' | 'REQUEST_FILENAME' | 'REQUEST_LINE' |
     'REQUEST_METHOD' | 'REQUEST_PROTOCOL' | 'REQUEST_URI_RAW' |'REQUEST_URI' |
     'RESPONSE_BODY' | 'RESPONSE_CONTENT_LENGTH' | 'RESPONSE_CONTENT_TYPE' |
     'RESPONSE_PROTOCOL' | 'RESPONSE_STATUS' | 'RULE' | 'SCRIPT_BASENAME' | 'SCRIPT_FILENAME' |
     'SCRIPT_GID' | 'SCRIPT_GROUPNAME' | 'SCRIPT_MODE' | 'SCRIPT_UID' | 'SCRIPT_USERNAME' |
     'SDBM_DELETE_ERROR' | 'SERVER_ADDR' | 'SERVER_NAME' | 'SERVER_PORT' | 'SESSION' | 'SESSIONID' |
     'STATUS_LINE' | 'STREAM_INPUT_BODY' | 'STREAM_OUTPUT_BODY' | 'TIME' | 'TIME_DAY' | 'TIME_EPOCH' |
     'TIME_HOUR' | 'TIME_MIN' | 'TIME_MON' | 'TIME_SEC' | 'TIME_WDAY' | 'TIME_YEAR' | 'UNIQUE_ID' |
```

### Comparing `secrules_parsing-0.2.8/src/secrules_parsing/parser.py` & `secrules_parsing-0.2.9/src/secrules_parsing/parser.py`

 * *Files identical despite different names*

### Comparing `secrules_parsing-0.2.8/PKG-INFO` & `secrules_parsing-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrules-parsing
-Version: 0.2.8
+Version: 0.2.9
 Summary: ModSecurity DSL Parser package using textX
 Home-page: https://github.com/coreruleset/secrules_parsing
 License: Apache-2.0
 Keywords: secrule,modsecurity,parser,textX
 Author: Felipe Zipitria
 Author-email: felipe.zipitria@owasp.org
 Requires-Python: >=3.7,<4.0
```

