# Comparing `tmp/fairness_checker-0.0.1.tar.gz` & `tmp/fairness_checker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fairness_checker-0.0.1.tar", last modified: Thu May 23 21:37:34 2024, max compression
+gzip compressed data, was "dist/fairness_checker-0.0.2.tar", last modified: Wed May 29 18:17:37 2024, max compression
```

## Comparing `fairness_checker-0.0.1.tar` & `fairness_checker-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-05-23 21:37:34.000000 fairness_checker-0.0.1/
--rw-r--r--   0 rexyuan    (501) staff       (20)     1211 2024-05-23 21:16:19.000000 fairness_checker-0.0.1/LICENSE
--rw-r--r--   0 rexyuan    (501) staff       (20)      477 2024-05-23 21:37:34.000000 fairness_checker-0.0.1/PKG-INFO
--rw-r--r--   0 rexyuan    (501) staff       (20)       12 2024-05-23 21:19:13.000000 fairness_checker-0.0.1/README.md
--rw-r--r--   0 rexyuan    (501) staff       (20)       38 2024-05-23 21:37:34.000000 fairness_checker-0.0.1/setup.cfg
--rw-r--r--   0 rexyuan    (501) staff       (20)      497 2024-05-23 21:16:52.000000 fairness_checker-0.0.1/setup.py
-drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-05-23 21:37:34.000000 fairness_checker-0.0.1/src/
-drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-05-23 21:37:34.000000 fairness_checker-0.0.1/src/fairness_checker/
--rw-r--r--   0 rexyuan    (501) staff       (20)       20 2024-05-23 20:38:54.000000 fairness_checker-0.0.1/src/fairness_checker/__init__.py
--rw-r--r--   0 rexyuan    (501) staff       (20)    59726 2024-05-23 20:52:31.000000 fairness_checker-0.0.1/src/fairness_checker/main.py
-drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-05-23 21:37:34.000000 fairness_checker-0.0.1/src/fairness_checker.egg-info/
--rw-r--r--   0 rexyuan    (501) staff       (20)      477 2024-05-23 21:37:34.000000 fairness_checker-0.0.1/src/fairness_checker.egg-info/PKG-INFO
--rw-r--r--   0 rexyuan    (501) staff       (20)      264 2024-05-23 21:37:34.000000 fairness_checker-0.0.1/src/fairness_checker.egg-info/SOURCES.txt
--rw-r--r--   0 rexyuan    (501) staff       (20)        1 2024-05-23 21:37:34.000000 fairness_checker-0.0.1/src/fairness_checker.egg-info/dependency_links.txt
--rw-r--r--   0 rexyuan    (501) staff       (20)       17 2024-05-23 21:37:34.000000 fairness_checker-0.0.1/src/fairness_checker.egg-info/top_level.txt
+drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/
+-rw-r--r--   0 rexyuan    (501) staff       (20)     1211 2024-05-23 21:16:19.000000 fairness_checker-0.0.2/LICENSE
+-rw-r--r--   0 rexyuan    (501) staff       (20)      477 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/PKG-INFO
+-rw-r--r--   0 rexyuan    (501) staff       (20)       12 2024-05-23 21:19:13.000000 fairness_checker-0.0.2/README.md
+-rw-r--r--   0 rexyuan    (501) staff       (20)       38 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/setup.cfg
+-rw-r--r--   0 rexyuan    (501) staff       (20)      497 2024-05-29 18:17:00.000000 fairness_checker-0.0.2/setup.py
+drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/src/
+drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/src/fairness_checker/
+-rw-r--r--   0 rexyuan    (501) staff       (20)       20 2024-05-23 20:38:54.000000 fairness_checker-0.0.2/src/fairness_checker/__init__.py
+-rw-r--r--   0 rexyuan    (501) staff       (20)    59726 2024-05-29 18:10:29.000000 fairness_checker-0.0.2/src/fairness_checker/main.py
+drwxr-xr-x   0 rexyuan    (501) staff       (20)        0 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/src/fairness_checker.egg-info/
+-rw-r--r--   0 rexyuan    (501) staff       (20)      477 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/src/fairness_checker.egg-info/PKG-INFO
+-rw-r--r--   0 rexyuan    (501) staff       (20)      264 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/src/fairness_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 rexyuan    (501) staff       (20)        1 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/src/fairness_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 rexyuan    (501) staff       (20)       17 2024-05-29 18:17:37.000000 fairness_checker-0.0.2/src/fairness_checker.egg-info/top_level.txt
```

### Comparing `fairness_checker-0.0.1/LICENSE` & `fairness_checker-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fairness_checker-0.0.1/src/fairness_checker/main.py` & `fairness_checker-0.0.2/src/fairness_checker/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,16 +291,16 @@
 
         return measure < ratio
 
     def equal_calibration(self,
                           ratio: float,
                           model: object,
                           privileged_predicate: Callable[[csv_row], bool],
-                          score_predicate_h: Callable[..., Callable[[csv_row], bool]],
-                          score_arg: Tuple[Any, ...],
+                          calib_predicate_h: Callable[..., Callable[[csv_row], bool]],
+                          calib_arg: Tuple[Any, ...],
                           truth_predicate: Callable[[csv_row], bool]) -> bool:
         """
         Evaluates the equal calibration of the model's predictions between privileged and unprivileged groups.
 
         Parameters:
         ratio (float): The fairness threshold ratio.
         model (object): The predictive model object.
@@ -316,18 +316,18 @@
         unprivileged = list(filter(lambda row: not privileged_predicate(row), self.reader))
 
         with self.csv_file_written('privileged.csv', privileged):
             with self.csv_file_written('unprivileged.csv', unprivileged):
                 privileged_Y_pred = model.predict('privileged.csv')
                 unprivileged_Y_pred = model.predict('unprivileged.csv')
 
-        score_predicate = score_predicate_h(*score_arg)
+        calib_predicate = calib_predicate_h(*calib_arg)
 
-        privileged_score = list(filter(lambda row_Y: score_predicate(row_Y[1]), zip(privileged, privileged_Y_pred)))
-        unprivileged_score = list(filter(lambda row_Y: score_predicate(row_Y[1]), zip(unprivileged, unprivileged_Y_pred)))
+        privileged_score = list(filter(lambda row_Y: calib_predicate(row_Y[1]), zip(privileged, privileged_Y_pred)))
+        unprivileged_score = list(filter(lambda row_Y: calib_predicate(row_Y[1]), zip(unprivileged, unprivileged_Y_pred)))
 
         privileged_score = list(map(lambda row_Y: row_Y[0], privileged_score))
         unprivileged_score = list(map(lambda row_Y: row_Y[0], unprivileged_score))
 
         privileged_positive_truth = list(filter(lambda row: truth_predicate(row), privileged_score))
         unprivileged_positive_truth = list(filter(lambda row: truth_predicate(row), unprivileged_score))
 
@@ -815,33 +815,33 @@
         print_stats('predictive parity', measure, ratio)
 
         return measure < ratio
 
     def equal_calibration(self,
                           ratio: float,
                           privileged_predicate: Callable[[csv_row], bool],
-                          score_predicate_h: Callable[..., Callable[[csv_row], bool]],
-                          score_arg: Tuple[Any, ...],
+                          calib_predicate_h: Callable[..., Callable[[csv_row], bool]],
+                          calib_arg: Tuple[Any, ...],
                           truth_predicate: Callable[[csv_row], bool]) -> bool:
         """
         Evaluates the equal calibration of the model's predictions between privileged and unprivileged groups.
 
         Parameters:
         ratio (float): The fairness threshold ratio.
         privileged_predicate (Callable[[csv_row], bool]): A function that determines whether a data point is privileged or not.
         positive_predicate (Callable[[csv_row], bool]): A function that determines whether the model's prediction is positive.
         truth_predicate: Callable[[csv_row], bool]: A function that determines a data point's ground truth.
 
         Returns:
         bool: If the input model satisfies the required fairness threshold ratio.
         """
-        score_predicate = score_predicate_h(*score_arg)
+        calib_predicate = calib_predicate_h(*calib_arg)
 
-        privileged_score = list(filter(lambda row: privileged_predicate(row) and score_predicate(row), self.reader))
-        unprivileged_score = list(filter(lambda row: not privileged_predicate(row) and score_predicate(row), self.reader))
+        privileged_score = list(filter(lambda row: privileged_predicate(row) and calib_predicate(row), self.reader))
+        unprivileged_score = list(filter(lambda row: not privileged_predicate(row) and calib_predicate(row), self.reader))
 
         privileged_positive_truth = list(filter(lambda row: truth_predicate(row), privileged_score))
         unprivileged_positive_truth = list(filter(lambda row: truth_predicate(row), unprivileged_score))
 
         privileged_positive_truth_percentage = len(privileged_positive_truth) / len(privileged_score)
         unprivileged_positive_truth_percentage = len(unprivileged_positive_truth) / len(unprivileged_score)
         measure = abs(privileged_positive_truth_percentage - unprivileged_positive_truth_percentage)
```

