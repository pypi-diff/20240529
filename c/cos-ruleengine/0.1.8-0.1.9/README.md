# Comparing `tmp/cos-ruleengine-0.1.8.tar.gz` & `tmp/cos-ruleengine-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cos-ruleengine-0.1.8.tar", last modified: Mon Aug 28 03:05:49 2023, max compression
+gzip compressed data, was "cos-ruleengine-0.1.9.tar", last modified: Mon Sep  4 12:12:56 2023, max compression
```

## Comparing `cos-ruleengine-0.1.8.tar` & `cos-ruleengine-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 03:05:49.223643 cos-ruleengine-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (999)      101 2023-08-28 03:05:49.223643 cos-ruleengine-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)       13 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 03:05:49.223643 cos-ruleengine-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      803 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 03:05:49.219643 cos-ruleengine-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 03:05:49.223643 cos-ruleengine-0.1.8/src/cos_ruleengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)      101 2023-08-28 03:05:49.000000 cos-ruleengine-0.1.8/src/cos_ruleengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      718 2023-08-28 03:05:49.000000 cos-ruleengine-0.1.8/src/cos_ruleengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 03:05:49.000000 cos-ruleengine-0.1.8/src/cos_ruleengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      108 2023-08-28 03:05:49.000000 cos-ruleengine-0.1.8/src/cos_ruleengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       17 2023-08-28 03:05:49.000000 cos-ruleengine-0.1.8/src/cos_ruleengine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 03:05:49.223643 cos-ruleengine-0.1.8/src/ruleengine/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/ruleengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 03:05:49.223643 cos-ruleengine-0.1.8/src/ruleengine/dsl/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/ruleengine/dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      122 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/ruleengine/dsl/actions.py
--rw-r--r--   0 runner    (1001) docker     (999)     3143 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/ruleengine/dsl/base_conditions.py
--rw-r--r--   0 runner    (1001) docker     (999)     3172 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/ruleengine/dsl/condition.py
--rw-r--r--   0 runner    (1001) docker     (999)     1435 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/ruleengine/dsl/log_conditions.py
--rw-r--r--   0 runner    (1001) docker     (999)     3519 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/ruleengine/dsl/sequence_conditions.py
--rw-r--r--   0 runner    (1001) docker     (999)     1592 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/ruleengine/dsl/validator.py
--rw-r--r--   0 runner    (1001) docker     (999)      796 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/ruleengine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 03:05:49.223643 cos-ruleengine-0.1.8/src/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 03:05:49.223643 cos-ruleengine-0.1.8/src/tests/dsl/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/tests/dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5107 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/tests/dsl/test_base_conditions.py
--rw-r--r--   0 runner    (1001) docker     (999)     2449 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/tests/dsl/test_log_conditions.py
--rw-r--r--   0 runner    (1001) docker     (999)     4106 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/tests/dsl/test_sequence_conditions.py
--rw-r--r--   0 runner    (1001) docker     (999)     1314 2023-08-28 03:05:34.000000 cos-ruleengine-0.1.8/src/tests/dsl/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 12:12:56.375377 cos-ruleengine-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (999)      101 2023-09-04 12:12:56.375377 cos-ruleengine-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)       13 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-04 12:12:56.375377 cos-ruleengine-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)      803 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 12:12:56.371377 cos-ruleengine-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 12:12:56.371377 cos-ruleengine-0.1.9/src/cos_ruleengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      101 2023-09-04 12:12:56.000000 cos-ruleengine-0.1.9/src/cos_ruleengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      974 2023-09-04 12:12:56.000000 cos-ruleengine-0.1.9/src/cos_ruleengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-04 12:12:56.000000 cos-ruleengine-0.1.9/src/cos_ruleengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      108 2023-09-04 12:12:56.000000 cos-ruleengine-0.1.9/src/cos_ruleengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       17 2023-09-04 12:12:56.000000 cos-ruleengine-0.1.9/src/cos_ruleengine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 12:12:56.371377 cos-ruleengine-0.1.9/src/ruleengine/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 12:12:56.375377 cos-ruleengine-0.1.9/src/ruleengine/dsl/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      122 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/dsl/action.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3143 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/dsl/base_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3172 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/dsl/condition.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1435 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/dsl/log_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5321 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/dsl/sequence_conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 12:12:56.375377 cos-ruleengine-0.1.9/src/ruleengine/dsl/validation/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/dsl/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      602 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/dsl/validation/ast.py
+-rw-r--r--   0 runner    (1001) docker     (999)      445 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/dsl/validation/fake_actions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3573 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/dsl/validation/main.py
+-rw-r--r--   0 runner    (1001) docker     (999)      399 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/dsl/validation/validation_result.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1648 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/dsl/validation/validator.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1787 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/dsl/validator.py
+-rw-r--r--   0 runner    (1001) docker     (999)      795 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/ruleengine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 12:12:56.375377 cos-ruleengine-0.1.9/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 12:12:56.375377 cos-ruleengine-0.1.9/src/tests/dsl/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/tests/dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5106 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/tests/dsl/test_base_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2448 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/tests/dsl/test_log_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4788 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/tests/dsl/test_sequence_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1314 2023-09-04 12:12:43.000000 cos-ruleengine-0.1.9/src/tests/dsl/test_validator.py
```

### Comparing `cos-ruleengine-0.1.8/setup.py` & `cos-ruleengine-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `cos-ruleengine-0.1.8/src/cos_ruleengine.egg-info/SOURCES.txt` & `cos-ruleengine-0.1.9/src/cos_ruleengine.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -4,19 +4,25 @@
 src/cos_ruleengine.egg-info/SOURCES.txt
 src/cos_ruleengine.egg-info/dependency_links.txt
 src/cos_ruleengine.egg-info/requires.txt
 src/cos_ruleengine.egg-info/top_level.txt
 src/ruleengine/__init__.py
 src/ruleengine/engine.py
 src/ruleengine/dsl/__init__.py
-src/ruleengine/dsl/actions.py
+src/ruleengine/dsl/action.py
 src/ruleengine/dsl/base_conditions.py
 src/ruleengine/dsl/condition.py
 src/ruleengine/dsl/log_conditions.py
 src/ruleengine/dsl/sequence_conditions.py
 src/ruleengine/dsl/validator.py
+src/ruleengine/dsl/validation/__init__.py
+src/ruleengine/dsl/validation/ast.py
+src/ruleengine/dsl/validation/fake_actions.py
+src/ruleengine/dsl/validation/main.py
+src/ruleengine/dsl/validation/validation_result.py
+src/ruleengine/dsl/validation/validator.py
 src/tests/__init__.py
 src/tests/dsl/__init__.py
 src/tests/dsl/test_base_conditions.py
 src/tests/dsl/test_log_conditions.py
 src/tests/dsl/test_sequence_conditions.py
 src/tests/dsl/test_validator.py
```

### Comparing `cos-ruleengine-0.1.8/src/ruleengine/dsl/base_conditions.py` & `cos-ruleengine-0.1.9/src/ruleengine/dsl/base_conditions.py`

 * *Files identical despite different names*

### Comparing `cos-ruleengine-0.1.8/src/ruleengine/dsl/condition.py` & `cos-ruleengine-0.1.9/src/ruleengine/dsl/condition.py`

 * *Files identical despite different names*

### Comparing `cos-ruleengine-0.1.8/src/ruleengine/dsl/log_conditions.py` & `cos-ruleengine-0.1.9/src/ruleengine/dsl/log_conditions.py`

 * *Files identical despite different names*

### Comparing `cos-ruleengine-0.1.8/src/ruleengine/dsl/validator.py` & `cos-ruleengine-0.1.9/src/ruleengine/dsl/validation/validator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,53 @@
 import inspect
 from ruleengine.dsl import base_conditions, log_conditions, sequence_conditions
+from ruleengine.dsl.condition import Condition
+from ruleengine.dsl.action import Action
+from .validation_result import ValidationResult, ValidationErrorType
+from .ast import validate_expression
+from . import fake_actions
 
 base_dsl_values = dict(
     inspect.getmembers(base_conditions)
     + inspect.getmembers(log_conditions)
     + inspect.getmembers(sequence_conditions)
 )
 
-
-def upload(
-    before=10,
-    title="",
-    description="",
-    labels=[],
-    extra_files=[],
-):
-    pass
-
-
-def create_moment(
-    title,
-    description="",
-    timestamp=0,
-    duration=1,
-    create_task=False,
-    assign_to=None,
-):
-    pass
-
-
 actions_dsl_values = {
-    "upload": upload,
-    "create_moment": create_moment,
+    **dict(inspect.getmembers(fake_actions)),
     **base_dsl_values,
 }
 
 
 def validate_condition(cond_str):
-    # TODO: Very much not safe. Condition strings are user supplied, and we need
-    # to sanitize the fuck out of it before doing eval.
-    return eval(cond_str, base_dsl_values)
+    return _do_validate(
+        cond_str, base_dsl_values, Condition, ValidationErrorType.NOT_CONDITION
+    )
 
 
 def validate_action(action_str):
-    # TODO: Very much not safe. Condition strings are user supplied, and we need
-    # to sanitize the fuck out of it before doing eval.
-    return eval(action_str, actions_dsl_values)
+    return _do_validate(
+        action_str, actions_dsl_values, Action, ValidationErrorType.NOT_ACTION
+    )
 
 
-if __name__ == "__main__":
-    import argparse
-
-    parser = argparse.ArgumentParser(description="Validate condition or action strings")
-    parser.add_argument(
-        "mode",
-        help="What we're validating, action or condition",
-        choices=["action", "condition"],
-    )
-    parser.add_argument("content", help="Content string to be validated")
-    args = parser.parse_args()
+def _do_validate(expr_str, injected_values, expected_class, class_expectation_error):
+    if not expr_str.strip():
+        return ValidationResult(False, ValidationErrorType.EMPTY)
+
+    expr_res = validate_expression(expr_str, injected_values)
+    if not expr_res.success:
+        return expr_res
+
+    try:
+        result = eval(expr_str, injected_values)
+    except TypeError as e:
+        return ValidationResult(False, ValidationErrorType.TYPE, {"message": str(e)})
+    except Exception as e:
+        return ValidationResult(False, ValidationErrorType.UNKNOWN, {"message": str(e)})
+
+    if not isinstance(result, expected_class):
+        return ValidationResult(
+            False, class_expectation_error, {"actual": type(result).__name__}
+        )
 
-    match args.mode:
-        case "action":
-            validate_action(args.content)
-        case "condition":
-            validate_condition(args.content)
+    return ValidationResult(True)
```

### Comparing `cos-ruleengine-0.1.8/src/ruleengine/engine.py` & `cos-ruleengine-0.1.9/src/ruleengine/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .dsl.actions import Action
+from .dsl.action import Action
 from .dsl.condition import Condition
 
 
 class Rule:
     def __init__(self, condition, action):
         assert isinstance(condition, Condition)
         assert isinstance(action, Action)
```

### Comparing `cos-ruleengine-0.1.8/src/tests/dsl/test_base_conditions.py` & `cos-ruleengine-0.1.9/src/tests/dsl/test_base_conditions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from collections import namedtuple
 
-from ruleengine.dsl.actions import Action
+from ruleengine.dsl.action import Action
 from ruleengine.dsl.base_conditions import *
 from ruleengine.engine import Engine, Rule
 
 MockDataItem = namedtuple("MockDataItem", "topic msg ts msgtype")
 MockMessage = namedtuple("MockMessage", "int_value str_value")
 
 simple_sequence = [
```

### Comparing `cos-ruleengine-0.1.8/src/tests/dsl/test_log_conditions.py` & `cos-ruleengine-0.1.9/src/tests/dsl/test_log_conditions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from collections import namedtuple
 
-from ruleengine.dsl.actions import Action
+from ruleengine.dsl.action import Action
 from ruleengine.dsl.base_conditions import *
 from ruleengine.dsl.log_conditions import *
 from ruleengine.engine import Engine, Rule
 
 MockDataItem = namedtuple("MockDataItem", "topic msg ts msgtype")
 MockMessage = namedtuple("MockMessage", "int_value str_value")
 RosMockMessage = namedtuple("RosMockMessage", "msg level")
```

### Comparing `cos-ruleengine-0.1.8/src/tests/dsl/test_sequence_conditions.py` & `cos-ruleengine-0.1.9/src/tests/dsl/test_sequence_conditions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from collections import namedtuple
 
-from ruleengine.dsl.actions import Action
+from ruleengine.dsl.action import Action
 from ruleengine.dsl.base_conditions import *
-from ruleengine.dsl.sequence_conditions import repeated, sequential, sustained
+from ruleengine.dsl.sequence_conditions import *
 from ruleengine.engine import Engine, Rule
 
 MockDataItem = namedtuple("MockDataItem", "topic msg ts")
 MockMessage = namedtuple("MockMessage", "int_value str_value")
 
 simple_sequence = [
     MockDataItem("t1", MockMessage(1, "hello"), 0),
@@ -21,14 +21,15 @@
     MockDataItem("t2", MockMessage(5, "world"), 4),
     MockDataItem("t2", MockMessage(5, "world"), 4),
     MockDataItem("t2", MockMessage(4, "hello"), 5),
     MockDataItem("t2", MockMessage(4, "hello"), 6),
     MockDataItem("t2", MockMessage(4, "hello"), 7),
     MockDataItem("t2", MockMessage(4, "hello"), 7),
     MockDataItem("t2", MockMessage(4, "hello"), 9),
+    MockDataItem("t3", MockMessage(4, "single"), 9),
 ]
 
 
 class CollectAction(Action):
     def __init__(self):
         self.collector = []
 
@@ -36,14 +37,18 @@
         self.collector.append((item, scope))
 
 
 def get_start_times(res):
     return [i[1]["start_time"] for i in res]
 
 
+def get_trigger_times(res):
+    return [i[0].ts for i in res]
+
+
 class SequenceConditionTest(unittest.TestCase):
     def test_sustained_sequence(self):
         result = self.__run_test(sustained(always, msg.str_value == "hello", 2))
         self.assertEqual(get_start_times(result), [0, 5])
 
         result = self.__run_test(sustained(always, msg.str_value == "hello", 6))
         self.assertEqual(get_start_times(result), [])
@@ -96,17 +101,31 @@
         result = self.__run_test(repeated(always, 2, 5))
         self.assertEqual(get_start_times(result), [0])
 
         result = self.__run_test(repeated(topic_is("t2"), 2, 5))
         self.assertEqual(get_start_times(result), [1])
 
         result = self.__run_test(repeated(topic_is("t2"), 5, 5))
-        self.assertEqual(get_start_times(result), [4])
+        self.assertEqual(get_start_times(result), [1])
 
         result = self.__run_test(repeated(topic_is("t2"), 2, 0.5))
         self.assertEqual(get_start_times(result), [1, 3, 4, 7])
 
+    def test_debounce(self):
+        result = self.__run_test(debounce(msg.str_value == "hello", 3))
+        self.assertEqual(get_trigger_times(result), [0])
+
+        result = self.__run_test(debounce(msg.str_value == "hello", 1.5))
+        self.assertEqual(get_trigger_times(result), [0, 5, 9])
+
+        result = self.__run_test(debounce(msg.str_value == "single", 3))
+        self.assertEqual(get_trigger_times(result), [9])
+
+    def test_throttle(self):
+        result = self.__run_test(throttle(msg.str_value == "hello", 3))
+        self.assertEqual(get_trigger_times(result), [0, 3, 6, 9])
+
     @staticmethod
     def __run_test(condition):
         action = CollectAction()
         Engine([Rule(condition, action)], simple_sequence).run()
         return action.collector
```

### Comparing `cos-ruleengine-0.1.8/src/tests/dsl/test_validator.py` & `cos-ruleengine-0.1.9/src/tests/dsl/test_validator.py`

 * *Files identical despite different names*

