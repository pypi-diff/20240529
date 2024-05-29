# Comparing `tmp/maptekomf_maptek-1.0.3-py3-none-any.whl.zip` & `tmp/maptekomf_maptek-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 26275 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      137 b- defN 23-Dec-13 01:26 maptekomf/maptek/__init__.py
--rw-rw-rw-  2.0 fat      685 b- defN 23-Dec-13 01:26 maptekomf/maptek/__main__.py
--rw-rw-rw-  2.0 fat    11466 b- defN 23-Dec-13 01:26 maptekomf/maptek/cli.py
--rw-rw-rw-  2.0 fat    32443 b- defN 23-Dec-13 01:26 maptekomf/maptek/exporter.py
--rw-rw-rw-  2.0 fat    35680 b- defN 23-Dec-13 01:26 maptekomf/maptek/importer.py
--rw-rw-rw-  2.0 fat    12503 b- defN 23-Dec-13 01:26 maptekomf/maptek/workflow.py
--rw-rw-rw-  2.0 fat     8228 b- defN 23-Dec-13 01:29 maptekomf_maptek-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Dec-13 01:29 maptekomf_maptek-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Dec-13 01:29 maptekomf_maptek-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      841 b- defN 23-Dec-13 01:29 maptekomf_maptek-1.0.3.dist-info/RECORD
-10 files, 102085 bytes uncompressed, 24839 bytes compressed:  75.7%
+Zip file size: 26274 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      137 b- defN 21-Dec-03 02:12 maptekomf/maptek/__init__.py
+-rw-rw-rw-  2.0 fat      685 b- defN 21-Dec-03 02:12 maptekomf/maptek/__main__.py
+-rw-rw-rw-  2.0 fat    11466 b- defN 23-Sep-05 06:14 maptekomf/maptek/cli.py
+-rw-rw-rw-  2.0 fat    32443 b- defN 23-Oct-24 02:36 maptekomf/maptek/exporter.py
+-rw-rw-rw-  2.0 fat    35680 b- defN 24-Mar-15 06:08 maptekomf/maptek/importer.py
+-rw-rw-rw-  2.0 fat    12503 b- defN 22-Jan-19 07:18 maptekomf/maptek/workflow.py
+-rw-rw-rw-  2.0 fat     8229 b- defN 24-May-29 07:47 maptekomf_maptek-1.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-29 07:47 maptekomf_maptek-1.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-29 07:47 maptekomf_maptek-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      841 b- defN 24-May-29 07:47 maptekomf_maptek-1.0.4.dist-info/RECORD
+10 files, 102086 bytes uncompressed, 24838 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: maptekomf/maptek/importer.py
 Comment: 
 
 Filename: maptekomf/maptek/workflow.py
 Comment: 
 
-Filename: maptekomf_maptek-1.0.3.dist-info/METADATA
+Filename: maptekomf_maptek-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: maptekomf_maptek-1.0.3.dist-info/WHEEL
+Filename: maptekomf_maptek-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: maptekomf_maptek-1.0.3.dist-info/top_level.txt
+Filename: maptekomf_maptek-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: maptekomf_maptek-1.0.3.dist-info/RECORD
+Filename: maptekomf_maptek-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `maptekomf_maptek-1.0.3.dist-info/METADATA` & `maptekomf_maptek-1.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maptekomf-maptek
-Version: 1.0.3
+Version: 1.0.4
 Summary: Provides interoperability between Maptek SDK and OMF.
 Author-email: Maptek <support@maptek.com.au>
 License: Maptek End User Licence Agreement
 Project-URL: Homepage, https://www.maptek.com
 Project-URL: Documentation, https://help.maptek.com/mapteksdk/
 Project-URL: Support, https://www.maptek.com/support/index.html
 Keywords: mining,data,interchange
@@ -15,18 +15,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: <3.12,>=3.7
+Requires-Python: <3.13,>=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: mapteksdk (<1.7.0,>=1.2.0)
-Requires-Dist: pillow (<9.5.0,>=7.0.0)
+Requires-Dist: mapteksdk (<2.0.0,>=1.2.0)
+Requires-Dist: pillow (<10.1.0,>=7.0.0)
 Requires-Dist: omf (==1.0.1)
 
 # maptekomf.maptek
 Provides support for inter-operability with the Open Mining Format (OMF) and
 Maptek applications which share an underlying infrastructure. This includes
 BlastLogic, PointStudio and Vulcan GeologyCore.
```

## Comparing `maptekomf_maptek-1.0.3.dist-info/RECORD` & `maptekomf_maptek-1.0.4.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 maptekomf/maptek/__init__.py,sha256=8EBHB8-muabUuDM8NhTweBqCLV51lKpREEaMpywLVPA,137
 maptekomf/maptek/__main__.py,sha256=rvdQTc-MaaS34rpKqL-bxm8GTCRj4MUOgPJx_hRqR04,685
 maptekomf/maptek/cli.py,sha256=Aiy8TCOFc-I2xZDCB96M9twVhtVmbOu8okSV83fHxkI,11466
 maptekomf/maptek/exporter.py,sha256=GBKRaSaMFAYh54-374WK4lrDvWHbL_55bq75Sbx7Ktc,32443
 maptekomf/maptek/importer.py,sha256=nd-4vlc3VTy9SJaCIa45rm1nDTAgcWRCV-dqyjxhaXo,35680
 maptekomf/maptek/workflow.py,sha256=oq3b_Zl-Cl0sjjToI5L20dk7giLnvtWumcRck7vVFY0,12503
-maptekomf_maptek-1.0.3.dist-info/METADATA,sha256=I6sxQ13d0B82iFmAJgsDVdlXujq7gLIGxU_TK45LLMk,8228
-maptekomf_maptek-1.0.3.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-maptekomf_maptek-1.0.3.dist-info/top_level.txt,sha256=WNPeIkzJeh7MSORka5BhN3ojoZ86dO3MgmuciTAPdW0,10
-maptekomf_maptek-1.0.3.dist-info/RECORD,,
+maptekomf_maptek-1.0.4.dist-info/METADATA,sha256=i8J-aKWBA4xIk5pNXofIQr8RHgACMQqJ2cTCvpMAr6Q,8229
+maptekomf_maptek-1.0.4.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+maptekomf_maptek-1.0.4.dist-info/top_level.txt,sha256=WNPeIkzJeh7MSORka5BhN3ojoZ86dO3MgmuciTAPdW0,10
+maptekomf_maptek-1.0.4.dist-info/RECORD,,
```

