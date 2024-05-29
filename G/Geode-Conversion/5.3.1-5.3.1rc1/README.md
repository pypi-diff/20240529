# Comparing `tmp/Geode_Conversion-5.3.1-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/Geode_Conversion-5.3.1rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1626085 bytes, number of entries: 8
--rw-r--r--  2.0 unx       67 b- defN 24-May-29 05:16 geode_conversion/__init__.py
--rw-r--r--  2.0 unx      172 b- defN 24-May-29 05:16 geode_conversion/model.py
--rwxr-xr-x  2.0 unx   167512 b- defN 24-May-29 05:16 geode_conversion/lib64/geode_conversion_py_model.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx  3602416 b- defN 24-May-29 05:16 geode_conversion/lib64/libGeode-Conversion_model.so
--rw-r--r--  2.0 unx     1931 b- defN 24-May-29 05:16 Geode_Conversion-5.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx      103 b- defN 24-May-29 05:16 Geode_Conversion-5.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-May-29 05:16 Geode_Conversion-5.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      748 b- defN 24-May-29 05:16 Geode_Conversion-5.3.1.dist-info/RECORD
-8 files, 3772966 bytes uncompressed, 1624761 bytes compressed:  57.0%
+Zip file size: 1649040 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      171 b- defN 24-May-24 13:26 geode_conversion/__init__.py
+-rw-rw-rw-  2.0 fat      178 b- defN 24-May-24 13:26 geode_conversion/model.py
+-rw-rw-rw-  2.0 fat  4083200 b- defN 24-May-24 13:27 geode_conversion/bin/Geode-Conversion_model.dll
+-rw-rw-rw-  2.0 fat   148480 b- defN 24-May-24 13:27 geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1996 b- defN 24-May-24 13:27 Geode_Conversion-5.3.1rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-24 13:27 Geode_Conversion-5.3.1rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 24-May-24 13:27 Geode_Conversion-5.3.1rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      743 b- defN 24-May-24 13:27 Geode_Conversion-5.3.1rc1.dist-info/RECORD
+8 files, 4234885 bytes uncompressed, 1647728 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: geode_conversion/__init__.py
 Comment: 
 
 Filename: geode_conversion/model.py
 Comment: 
 
-Filename: geode_conversion/lib64/geode_conversion_py_model.cpython-39-x86_64-linux-gnu.so
+Filename: geode_conversion/bin/Geode-Conversion_model.dll
 Comment: 
 
-Filename: geode_conversion/lib64/libGeode-Conversion_model.so
+Filename: geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Conversion-5.3.1.dist-info/METADATA
+Filename: Geode_Conversion-5.3.1rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Conversion-5.3.1.dist-info/WHEEL
+Filename: Geode_Conversion-5.3.1rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Conversion-5.3.1.dist-info/top_level.txt
+Filename: Geode_Conversion-5.3.1rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Conversion-5.3.1.dist-info/RECORD
+Filename: Geode_Conversion-5.3.1rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_conversion/__init__.py

```diff
@@ -1,3 +1,6 @@
-## Copyright (c) 2019 - 2024 Geode-solutions
-
-from .model import *
+## Copyright (c) 2019 - 2024 Geode-solutions
+
+import os, pathlib
+os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
+
+from .model import *
```

## geode_conversion/model.py

```diff
@@ -1,8 +1,8 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-
-from .lib64.geode_conversion_py_model import *
-ConversionModelLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+
+from .bin.geode_conversion_py_model import *
+ConversionModelLibrary.initialize()
```

