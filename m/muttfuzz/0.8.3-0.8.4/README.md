# Comparing `tmp/muttfuzz-0.8.3-py3-none-any.whl.zip` & `tmp/muttfuzz-0.8.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10126 bytes, number of entries: 8
+Zip file size: 10140 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     4944 b- defN 24-May-28 17:16 muttfuzz/fuzz.py
 -rw-r--r--  2.0 unx    11144 b- defN 24-May-28 18:05 muttfuzz/fuzzutil.py
--rw-r--r--  2.0 unx     5721 b- defN 24-May-28 10:34 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     6941 b- defN 24-May-28 18:05 muttfuzz-0.8.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 18:05 muttfuzz-0.8.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-28 18:05 muttfuzz-0.8.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-28 18:05 muttfuzz-0.8.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      623 b- defN 24-May-28 18:05 muttfuzz-0.8.3.dist-info/RECORD
-8 files, 29535 bytes uncompressed, 9042 bytes compressed:  69.4%
+-rw-r--r--  2.0 unx     5822 b- defN 24-May-29 03:35 muttfuzz/mutate.py
+-rw-r--r--  2.0 unx     6941 b- defN 24-May-29 03:35 muttfuzz-0.8.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-29 03:35 muttfuzz-0.8.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-29 03:35 muttfuzz-0.8.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-29 03:35 muttfuzz-0.8.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 24-May-29 03:35 muttfuzz-0.8.4.dist-info/RECORD
+8 files, 29636 bytes uncompressed, 9056 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.8.3.dist-info/METADATA
+Filename: muttfuzz-0.8.4.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.8.3.dist-info/WHEEL
+Filename: muttfuzz-0.8.4.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.8.3.dist-info/entry_points.txt
+Filename: muttfuzz-0.8.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.8.3.dist-info/top_level.txt
+Filename: muttfuzz-0.8.4.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.8.3.dist-info/RECORD
+Filename: muttfuzz-0.8.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/mutate.py

```diff
@@ -110,16 +110,19 @@
         return bytearray(f.read())
 
 def mutant_from(code, jumps, order=1):
     new_code = bytearray(code)
     reach_code = bytearray(code)
     for i in range(order): # allows higher-order mutants, though can undo mutations
         (loc, new_data) = pick_and_change(jumps)
-        reach_code[loc] = HALT[0]
         for offset in range(0, len(new_data)):
+            if offset == 0:
+                reach_code[offset] = HALT[0]
+            else:
+                reach_code[offset] = NOP[0]
             new_code[loc + offset] = new_data[offset]
     return (new_code, reach_code)
 
 def mutant(filename, order=1, avoid_mutating=[]):
     return mutant_from(get_code(filename), get_jumps(filename, avoid_mutating), order=order)
 
 def mutate_from(code, jumps, new_filename, order=1, reachability_filename=""):
```

## Comparing `muttfuzz-0.8.3.dist-info/METADATA` & `muttfuzz-0.8.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.8.3
+Version: 0.8.4
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.8.3.dist-info/RECORD` & `muttfuzz-0.8.4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 muttfuzz/fuzz.py,sha256=cis3_IqePjHxFGhsi7RXmHdpYVrZqxeJ3TUyZ_HJ4x8,4944
 muttfuzz/fuzzutil.py,sha256=VjLJn_oVDg7eAMbYYxNC0zA_b4ECIS4H06K57trIw8Y,11144
-muttfuzz/mutate.py,sha256=EUFlHVAhzW9FSBuaNz-nHtcp_CgGgQCOyLyzQEyHPxQ,5721
-muttfuzz-0.8.3.dist-info/METADATA,sha256=zC25uQuiSvtTZnfRuIa898k1bEpc4BqoYbYbY5kdMzI,6941
-muttfuzz-0.8.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.8.3.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.8.3.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.8.3.dist-info/RECORD,,
+muttfuzz/mutate.py,sha256=EFD-_8jCLcUUEiLt6zyy59mu95If4_tG7fnzcv0gOIA,5822
+muttfuzz-0.8.4.dist-info/METADATA,sha256=spMfD29L68WLmlVHgv94NkTJBNTJhNfoM53QcGqO4yw,6941
+muttfuzz-0.8.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.8.4.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.8.4.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.8.4.dist-info/RECORD,,
```

