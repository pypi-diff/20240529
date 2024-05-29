# Comparing `tmp/muttfuzz-0.8.6-py3-none-any.whl.zip` & `tmp/muttfuzz-0.8.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10144 bytes, number of entries: 8
+Zip file size: 10172 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     4944 b- defN 24-May-28 17:16 muttfuzz/fuzz.py
 -rw-r--r--  2.0 unx    11144 b- defN 24-May-28 18:05 muttfuzz/fuzzutil.py
--rw-r--r--  2.0 unx     5834 b- defN 24-May-29 03:39 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     6941 b- defN 24-May-29 03:40 muttfuzz-0.8.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-29 03:40 muttfuzz-0.8.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-29 03:40 muttfuzz-0.8.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-29 03:40 muttfuzz-0.8.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      623 b- defN 24-May-29 03:40 muttfuzz-0.8.6.dist-info/RECORD
-8 files, 29648 bytes uncompressed, 9060 bytes compressed:  69.4%
+-rw-r--r--  2.0 unx     5958 b- defN 24-May-29 04:19 muttfuzz/mutate.py
+-rw-r--r--  2.0 unx     6941 b- defN 24-May-29 04:19 muttfuzz-0.8.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-29 04:19 muttfuzz-0.8.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-29 04:19 muttfuzz-0.8.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-29 04:19 muttfuzz-0.8.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 24-May-29 04:19 muttfuzz-0.8.7.dist-info/RECORD
+8 files, 29772 bytes uncompressed, 9088 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.8.6.dist-info/METADATA
+Filename: muttfuzz-0.8.7.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.8.6.dist-info/WHEEL
+Filename: muttfuzz-0.8.7.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.8.6.dist-info/entry_points.txt
+Filename: muttfuzz-0.8.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.8.6.dist-info/top_level.txt
+Filename: muttfuzz-0.8.7.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.8.6.dist-info/RECORD
+Filename: muttfuzz-0.8.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/mutate.py

```diff
@@ -99,14 +99,16 @@
     print("ORIGINAL CODE:", jumps[loc][3])
     if changed in SHORT_NAMES:
         print("CHANGING TO", SHORT_NAMES[changed])
     elif changed in NEAR_NAMES:
         print("CHANGING TO", NEAR_NAMES[changed])
     else:
         print("CHANGING TO NOPS")
+    if len(changed) < len(jumps[loc][1]):
+        changed = changed + jumps[loc][1][len(jumps[loc][1]) - len(changed) - 1:]
     return (loc, changed)
 
 def get_code(filename):
     with open(filename, "rb") as f:
         return bytearray(f.read())
 
 def mutant_from(code, jumps, order=1):
```

## Comparing `muttfuzz-0.8.6.dist-info/METADATA` & `muttfuzz-0.8.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.8.6
+Version: 0.8.7
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.8.6.dist-info/RECORD` & `muttfuzz-0.8.7.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 muttfuzz/fuzz.py,sha256=cis3_IqePjHxFGhsi7RXmHdpYVrZqxeJ3TUyZ_HJ4x8,4944
 muttfuzz/fuzzutil.py,sha256=VjLJn_oVDg7eAMbYYxNC0zA_b4ECIS4H06K57trIw8Y,11144
-muttfuzz/mutate.py,sha256=AJzLg8FgS55d2MiLvFwL31vTfGmkZhrSIxAk-WLUUhA,5834
-muttfuzz-0.8.6.dist-info/METADATA,sha256=rCveeEti48E6uUvo43M1xShoHET2BSto1aAjZBpqZec,6941
-muttfuzz-0.8.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.8.6.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.8.6.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.8.6.dist-info/RECORD,,
+muttfuzz/mutate.py,sha256=Q9197L2-e9aXyopHwjWWHi9VqKGlPIREu7YyVoIgW4c,5958
+muttfuzz-0.8.7.dist-info/METADATA,sha256=73V-OBXaDbwlhm71JC9OcWJjiwWsAY65T7uex7SxZEA,6941
+muttfuzz-0.8.7.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.8.7.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.8.7.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.8.7.dist-info/RECORD,,
```

