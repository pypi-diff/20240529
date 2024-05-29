# Comparing `tmp/pyexclient-1.0.3-py3-none-any.whl.zip` & `tmp/pyexclient-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 70130 bytes, number of entries: 8
--rw-r--r--  2.0 unx       46 b- defN 24-May-24 15:46 pyexclient/__init__.py
--rw-r--r--  2.0 unx      497 b- defN 24-May-24 15:46 pyexclient/_version.py
--rw-r--r--  2.0 unx   970764 b- defN 24-May-24 15:46 pyexclient/workbench.py
--rw-r--r--  2.0 unx     1321 b- defN 24-May-24 15:46 pyexclient-1.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3511 b- defN 24-May-24 15:46 pyexclient-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 15:46 pyexclient-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-24 15:46 pyexclient-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      638 b- defN 24-May-24 15:46 pyexclient-1.0.3.dist-info/RECORD
-8 files, 976880 bytes uncompressed, 69018 bytes compressed:  92.9%
+Zip file size: 70129 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       46 b- defN 24-May-28 20:49 pyexclient/__init__.py
+-rw-r--r--  2.0 unx      497 b- defN 24-May-28 20:49 pyexclient/_version.py
+-rw-r--r--  2.0 unx   970764 b- defN 24-May-28 20:49 pyexclient/workbench.py
+-rw-r--r--  2.0 unx     1321 b- defN 24-May-28 20:49 pyexclient-1.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3511 b- defN 24-May-28 20:49 pyexclient-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 20:49 pyexclient-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-28 20:49 pyexclient-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      638 b- defN 24-May-28 20:49 pyexclient-1.0.4.dist-info/RECORD
+8 files, 976880 bytes uncompressed, 69017 bytes compressed:  92.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: pyexclient/_version.py
 Comment: 
 
 Filename: pyexclient/workbench.py
 Comment: 
 
-Filename: pyexclient-1.0.3.dist-info/LICENSE
+Filename: pyexclient-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: pyexclient-1.0.3.dist-info/METADATA
+Filename: pyexclient-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: pyexclient-1.0.3.dist-info/WHEEL
+Filename: pyexclient-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: pyexclient-1.0.3.dist-info/top_level.txt
+Filename: pyexclient-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pyexclient-1.0.3.dist-info/RECORD
+Filename: pyexclient-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyexclient/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-05-24T11:35:03-0400",
+ "date": "2024-05-28T16:45:30-0400",
  "dirty": false,
  "error": null,
- "full-revisionid": "359b502a23c7eb8abbfc0cac8549e1281936ed03",
- "version": "1.0.3"
+ "full-revisionid": "fb63c544caa28076bb07336fbc09e9c24a0725f4",
+ "version": "1.0.4"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## Comparing `pyexclient-1.0.3.dist-info/LICENSE` & `pyexclient-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyexclient-1.0.3.dist-info/METADATA` & `pyexclient-1.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyexclient
-Version: 1.0.3
+Version: 1.0.4
 Summary: Expel Workbench Client
 Home-page: https://github.com/expel-io/pyexclient
 Author: Expel Inc.
 License: BSD
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyexclient Version: 1.0.3 Summary: Expel Workbench
+Metadata-Version: 2.1 Name: pyexclient Version: 1.0.4 Summary: Expel Workbench
 Client Home-page: https://github.com/expel-io/pyexclient Author: Expel Inc.
 License: BSD Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
                              ******** PPyyeexxcclliieenntt ********
                    A Python client for the Expel Workbench.
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
```

