# Comparing `tmp/muttfuzz-0.8.2-py3-none-any.whl.zip` & `tmp/muttfuzz-0.8.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10036 bytes, number of entries: 8
+Zip file size: 10126 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     4944 b- defN 24-May-28 17:16 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx    11128 b- defN 24-May-28 17:49 muttfuzz/fuzzutil.py
+-rw-r--r--  2.0 unx    11144 b- defN 24-May-28 18:05 muttfuzz/fuzzutil.py
 -rw-r--r--  2.0 unx     5721 b- defN 24-May-28 10:34 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     6714 b- defN 24-May-28 17:49 muttfuzz-0.8.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 17:49 muttfuzz-0.8.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-28 17:49 muttfuzz-0.8.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-28 17:49 muttfuzz-0.8.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      623 b- defN 24-May-28 17:49 muttfuzz-0.8.2.dist-info/RECORD
-8 files, 29292 bytes uncompressed, 8952 bytes compressed:  69.4%
+-rw-r--r--  2.0 unx     6941 b- defN 24-May-28 18:05 muttfuzz-0.8.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 18:05 muttfuzz-0.8.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-28 18:05 muttfuzz-0.8.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-28 18:05 muttfuzz-0.8.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 24-May-28 18:05 muttfuzz-0.8.3.dist-info/RECORD
+8 files, 29535 bytes uncompressed, 9042 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.8.2.dist-info/METADATA
+Filename: muttfuzz-0.8.3.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.8.2.dist-info/WHEEL
+Filename: muttfuzz-0.8.3.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.8.2.dist-info/entry_points.txt
+Filename: muttfuzz-0.8.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.8.2.dist-info/top_level.txt
+Filename: muttfuzz-0.8.3.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.8.2.dist-info/RECORD
+Filename: muttfuzz-0.8.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzzutil.py

```diff
@@ -121,15 +121,15 @@
                 r = silent_run_with_timeout(reachability_check_cmd, reachability_check_timeout)
                 restore_executable(executable, executable_code)
                 if r == 0:
                     print("MUTANT IS NOT REACHABLE (RETURN CODE 0)")
                     mutant_ok = False
                 else:
                     reachability_hits += 1.0
-                print ("RUNNING COVERAGE ESTIMATE OVER", int(mutants_run), "MUTANTS:",
+                print ("RUNNING COVERAGE ESTIMATE OVER", int(reachability_checks), "MUTANTS:",
                        str(round((reachability_hits / reachability_checks) * 100.0, 2)) + "%")
             if mutant_ok:
                 os.rename("/tmp/new_executable", executable)
                 subprocess.check_call(['chmod', '+x', executable])
                 if prune_mutant_cmd != "":
                     print("PRUNING MUTANT...")
                     r = silent_run_with_timeout(prune_mutant_cmd, prune_mutant_timeout)
@@ -164,15 +164,15 @@
         restore_executable(executable, executable_code)
         silent_run_with_timeout(fuzzer_cmd, budget - (time.time() - start_fuzz))
         print("COMPLETED ALL FUZZING AFTER", round(time.time() - start_fuzz, 2), "SECONDS")
         if status_cmd != "":
             print("FINAL STATUS:")
             subprocess.call(status_cmd, shell=True)
         if reachability_check_cmd != "":
-            print ("FINAL COVERAGE ESTIMATE OVER", int(mutants_run), "MUTANTS:",
+            print ("FINAL COVERAGE ESTIMATE OVER", int(reachability_checks), "MUTANTS:",
                    str(round((reachability_hits / reachability_checks) * 100.0, 2)) + "%")
         if score:
             print ("FINAL MUTATION SCORE OVER", int(mutants_run), "MUTANTS:",
                     str(round((mutants_killed / mutants_run) * 100.0, 2)) + "%")
             print ("NOTE:  MUTANTS MAY BE REDUNDANT")
     finally:
         # always restore the original binary!
```

## Comparing `muttfuzz-0.8.2.dist-info/METADATA` & `muttfuzz-0.8.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.8.2
+Version: 0.8.3
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
@@ -67,15 +67,15 @@
 
 **A**: For more information on that, and on the source-based version of this idea, see [our paper in submission to ACM TOSEM, the final version of our FUZZING'22 registered report](https://github.com/agroce/fuzzing22report/blob/master/tosem/currentdraft.pdf).  Long story short, we speculate that some mutants remove common barriers to fuzzing, and/or allow fuzzing to find branches "non-chronologically."
 
 **Q**: Hey, you said I could use MuttFuzz to estimate a mutation score?
 
 **A**: Yes, just use a fuzzing command that does nothing but check a mutant for detection (something like the commands used for reachability and pruning) that returns non-zero on detected mutants, and add the `--score` option.  Note that MuttFuzz uses a peculiar and biased set of mutation operators, and may score the same mutant multiple times, so take this value with a grain of salt.  You can also have the fuzzing command do some actual fuzzing, and then check for detection after the fuzzing.
 
-Note that reachability and pruning work as usual here.  Pruning will seldom be needed, but there may be some notion of invalid mutants you want to use.  Reachability lets you compute  a score over mutants the corpus actually executes, which is usually more informative than including mutants not even executed.  The distinction is between "mutation score" and "covered mutation score" (see [this paper](https://agroce.github.io/issre23.pdf)).  Note that MuttFuzz, when a reachability check is included, always shows a running and final total of estimated coverage of mutants.
+Note that reachability and pruning work as usual here.  Pruning will seldom be needed, but there may be some notion of invalid mutants you want to use.  Reachability lets you compute  a score over mutants the corpus actually executes, which is usually more informative than including mutants not even executed.  The distinction is between "mutation score" and "covered mutation score" (see [this paper](https://agroce.github.io/issre23.pdf)).  Note that MuttFuzz, when a reachability check is included, always shows a running and final total of estimated coverage of mutants.  In principle a mutation score estimate could be produced from the prune checks during fuzzing campaigns, but the fact that fuzzing (we hope) changes the power of the corpus will make this total unstable and hard to interpret.
 
 **Q**: Why "MuttFuzz"?
 
 **A**: When I (Alex) created the repo, I made a typo, but I liked it.  Certainly memorable compared to "mutfuzz" for "mutant fuzzer".
 
 -------------------------------
```

## Comparing `muttfuzz-0.8.2.dist-info/RECORD` & `muttfuzz-0.8.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 muttfuzz/fuzz.py,sha256=cis3_IqePjHxFGhsi7RXmHdpYVrZqxeJ3TUyZ_HJ4x8,4944
-muttfuzz/fuzzutil.py,sha256=S7PaiD8Wxgxd614JftRmmbVFyzc87NROn034kpl3ERA,11128
+muttfuzz/fuzzutil.py,sha256=VjLJn_oVDg7eAMbYYxNC0zA_b4ECIS4H06K57trIw8Y,11144
 muttfuzz/mutate.py,sha256=EUFlHVAhzW9FSBuaNz-nHtcp_CgGgQCOyLyzQEyHPxQ,5721
-muttfuzz-0.8.2.dist-info/METADATA,sha256=aEfh2WNwnpmv7KHqXW8lDiaoJol0fpOaYQ0sylNdJn0,6714
-muttfuzz-0.8.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.8.2.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.8.2.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.8.2.dist-info/RECORD,,
+muttfuzz-0.8.3.dist-info/METADATA,sha256=zC25uQuiSvtTZnfRuIa898k1bEpc4BqoYbYbY5kdMzI,6941
+muttfuzz-0.8.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.8.3.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.8.3.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.8.3.dist-info/RECORD,,
```

