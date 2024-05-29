# Comparing `tmp/muttfuzz-0.8.5-py3-none-any.whl.zip` & `tmp/muttfuzz-0.8.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10141 bytes, number of entries: 8
+Zip file size: 10144 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     4944 b- defN 24-May-28 17:16 muttfuzz/fuzz.py
 -rw-r--r--  2.0 unx    11144 b- defN 24-May-28 18:05 muttfuzz/fuzzutil.py
--rw-r--r--  2.0 unx     5822 b- defN 24-May-29 03:35 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     6941 b- defN 24-May-29 03:38 muttfuzz-0.8.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-29 03:38 muttfuzz-0.8.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-29 03:38 muttfuzz-0.8.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-29 03:38 muttfuzz-0.8.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      623 b- defN 24-May-29 03:38 muttfuzz-0.8.5.dist-info/RECORD
-8 files, 29636 bytes uncompressed, 9057 bytes compressed:  69.4%
+-rw-r--r--  2.0 unx     5834 b- defN 24-May-29 03:39 muttfuzz/mutate.py
+-rw-r--r--  2.0 unx     6941 b- defN 24-May-29 03:40 muttfuzz-0.8.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-29 03:40 muttfuzz-0.8.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-29 03:40 muttfuzz-0.8.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-29 03:40 muttfuzz-0.8.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 24-May-29 03:40 muttfuzz-0.8.6.dist-info/RECORD
+8 files, 29648 bytes uncompressed, 9060 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.8.5.dist-info/METADATA
+Filename: muttfuzz-0.8.6.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.8.5.dist-info/WHEEL
+Filename: muttfuzz-0.8.6.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.8.5.dist-info/entry_points.txt
+Filename: muttfuzz-0.8.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.8.5.dist-info/top_level.txt
+Filename: muttfuzz-0.8.6.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.8.5.dist-info/RECORD
+Filename: muttfuzz-0.8.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/mutate.py

```diff
@@ -112,17 +112,17 @@
 def mutant_from(code, jumps, order=1):
     new_code = bytearray(code)
     reach_code = bytearray(code)
     for i in range(order): # allows higher-order mutants, though can undo mutations
         (loc, new_data) = pick_and_change(jumps)
         for offset in range(0, len(new_data)):
             if offset == 0:
-                reach_code[offset] = HALT[0]
+                reach_code[loc + offset] = HALT[0]
             else:
-                reach_code[offset] = NOP[0]
+                reach_code[loc + offset] = NOP[0]
             new_code[loc + offset] = new_data[offset]
     return (new_code, reach_code)
 
 def mutant(filename, order=1, avoid_mutating=[]):
     return mutant_from(get_code(filename), get_jumps(filename, avoid_mutating), order=order)
 
 def mutate_from(code, jumps, new_filename, order=1, reachability_filename=""):
```

## Comparing `muttfuzz-0.8.5.dist-info/METADATA` & `muttfuzz-0.8.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.8.5
+Version: 0.8.6
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

