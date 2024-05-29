# Comparing `tmp/spacecan-2.2.0.tar.gz` & `tmp/spacecan-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacecan-2.2.0.tar", last modified: Wed Mar 27 01:04:42 2024, max compression
+gzip compressed data, was "spacecan-2.3.0.tar", last modified: Wed May 29 21:33:57 2024, max compression
```

## Comparing `spacecan-2.2.0.tar` & `spacecan-2.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 01:04:42.122113 spacecan-2.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1066 2024-03-27 01:04:29.000000 spacecan-2.2.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1233 2024-03-27 01:04:42.122113 spacecan-2.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      970 2024-03-27 01:04:29.000000 spacecan-2.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-03-27 01:04:29.000000 spacecan-2.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-27 01:04:42.122113 spacecan-2.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 01:04:42.114113 spacecan-2.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 01:04:42.116113 spacecan-2.2.0/src/spacecan/
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5010 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 01:04:42.119113 spacecan-2.2.0/src/spacecan/primitives/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/primitives/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/primitives/can_frame.py
--rw-rw-rw-   0 root         (0) root         (0)     2845 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/primitives/heartbeat.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/primitives/network.py
--rw-rw-rw-   0 root         (0) root         (0)     1402 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/primitives/packet.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/primitives/sync.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/primitives/timer.py
--rw-rw-rw-   0 root         (0) root         (0)     4875 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/responder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 01:04:42.121112 spacecan-2.2.0/src/spacecan/services/
--rw-rw-rw-   0 root         (0) root         (0)     1855 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/services/ST01_request_verification.py
--rw-rw-rw-   0 root         (0) root         (0)     8196 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/services/ST03_housekeeping.py
--rw-rw-rw-   0 root         (0) root         (0)     5457 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/services/ST08_function_management.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/services/ST17_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5219 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/services/ST20_parameter_management.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3675 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/services/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 01:04:42.121112 spacecan-2.2.0/src/spacecan/transport/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/transport/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1249 2024-03-27 01:04:29.000000 spacecan-2.2.0/src/spacecan/transport/socketcan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 01:04:42.122113 spacecan-2.2.0/src/spacecan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1233 2024-03-27 01:04:42.000000 spacecan-2.2.0/src/spacecan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      953 2024-03-27 01:04:42.000000 spacecan-2.2.0/src/spacecan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 01:04:42.000000 spacecan-2.2.0/src/spacecan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-27 01:04:42.000000 spacecan-2.2.0/src/spacecan.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-27 01:04:42.000000 spacecan-2.2.0/src/spacecan.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 01:04:42.121112 spacecan-2.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-03-27 01:04:29.000000 spacecan-2.2.0/tests/test_basic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:33:57.506615 spacecan-2.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2024-05-29 21:33:45.000000 spacecan-2.3.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-05-29 21:33:57.506615 spacecan-2.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      970 2024-05-29 21:33:45.000000 spacecan-2.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-29 21:33:45.000000 spacecan-2.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 21:33:57.506615 spacecan-2.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:33:57.499615 spacecan-2.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:33:57.501615 spacecan-2.3.0/src/spacecan/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5010 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:33:57.503615 spacecan-2.3.0/src/spacecan/primitives/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/primitives/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/primitives/can_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/primitives/heartbeat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/primitives/network.py
+-rw-rw-rw-   0 root         (0) root         (0)     1402 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/primitives/packet.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/primitives/sync.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/primitives/timer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4875 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/responder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:33:57.505615 spacecan-2.3.0/src/spacecan/services/
+-rw-rw-rw-   0 root         (0) root         (0)     1958 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/services/ST01_request_verification.py
+-rw-rw-rw-   0 root         (0) root         (0)     8396 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/services/ST03_housekeeping.py
+-rw-rw-rw-   0 root         (0) root         (0)     6126 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/services/ST08_function_management.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/services/ST17_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5388 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/services/ST20_parameter_management.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3675 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/services/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:33:57.505615 spacecan-2.3.0/src/spacecan/transport/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/transport/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1249 2024-05-29 21:33:45.000000 spacecan-2.3.0/src/spacecan/transport/socketcan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:33:57.506615 spacecan-2.3.0/src/spacecan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-05-29 21:33:57.000000 spacecan-2.3.0/src/spacecan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      953 2024-05-29 21:33:57.000000 spacecan-2.3.0/src/spacecan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 21:33:57.000000 spacecan-2.3.0/src/spacecan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-29 21:33:57.000000 spacecan-2.3.0/src/spacecan.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-29 21:33:57.000000 spacecan-2.3.0/src/spacecan.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:33:57.506615 spacecan-2.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-29 21:33:45.000000 spacecan-2.3.0/tests/test_basic.py
```

### Comparing `spacecan-2.2.0/LICENSE.txt` & `spacecan-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spacecan-2.2.0/PKG-INFO` & `spacecan-2.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacecan
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python implementation of SpaceCAN protocol
 Author-email: LibreCube <info@librecube.org>
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: python-can
```

### Comparing `spacecan-2.2.0/README.md` & `spacecan-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `spacecan-2.2.0/src/spacecan/controller.py` & `spacecan-2.3.0/src/spacecan/controller.py`

 * *Files identical despite different names*

### Comparing `spacecan-2.2.0/src/spacecan/primitives/can_frame.py` & `spacecan-2.3.0/src/spacecan/primitives/can_frame.py`

 * *Files identical despite different names*

### Comparing `spacecan-2.2.0/src/spacecan/primitives/heartbeat.py` & `spacecan-2.3.0/src/spacecan/primitives/heartbeat.py`

 * *Files identical despite different names*

### Comparing `spacecan-2.2.0/src/spacecan/primitives/network.py` & `spacecan-2.3.0/src/spacecan/primitives/network.py`

 * *Files identical despite different names*

### Comparing `spacecan-2.2.0/src/spacecan/primitives/packet.py` & `spacecan-2.3.0/src/spacecan/primitives/packet.py`

 * *Files identical despite different names*

### Comparing `spacecan-2.2.0/src/spacecan/primitives/sync.py` & `spacecan-2.3.0/src/spacecan/primitives/sync.py`

 * *Files identical despite different names*

### Comparing `spacecan-2.2.0/src/spacecan/responder.py` & `spacecan-2.3.0/src/spacecan/responder.py`

 * *Files identical despite different names*

### Comparing `spacecan-2.2.0/src/spacecan/services/ST01_request_verification.py` & `spacecan-2.3.0/src/spacecan/services/ST01_request_verification.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,36 +5,42 @@
     def __init__(self, parent):
         self.parent = parent
 
     def process(self, service, subtype, data, node_id):
         case = (service, subtype)
         source_packet = data[0], data[1]
 
+        self.received_report(node_id, case, source_packet)
+
         if case == (1, 1):
             self.received_success_acceptance_report(node_id, source_packet)
         elif case == (1, 2):
             self.received_fail_acceptance_report(node_id, source_packet)
         elif case == (1, 7):
-            self.received_success_completion_execution_report(node_id, source_packet)
+            self.received_success_completion_report(node_id, source_packet)
         elif case == (1, 8):
-            self.received_fail_completion_execution_report(node_id, source_packet)
+            self.received_fail_completion_report(node_id, source_packet)
+
+    def received_report(self, node_id, case, source_packet):
+        # to be overwritten
+        pass
 
     def received_success_acceptance_report(self, node_id, source_packet):
         # to be overwritten
         pass
 
     def received_fail_acceptance_report(self, node_id, source_packet):
         # to be overwritten
         pass
 
-    def received_success_completion_execution_report(self, node_id, source_packet):
+    def received_success_completion_report(self, node_id, source_packet):
         # to be overwritten
         pass
 
-    def received_fail_completion_execution_report(self, node_id, source_packet):
+    def received_fail_completion_report(self, node_id, source_packet):
         # to be overwritten
         pass
 
 
 class RequestVerificationServiceResponder:
     def __init__(self, parent):
         self.parent = parent
@@ -44,12 +50,12 @@
 
     def send_success_acceptance_report(self, source_packet):
         self.parent.send(Packet([1, 1] + source_packet))
 
     def send_fail_acceptance_report(self, source_packet):
         self.parent.send(Packet([1, 2] + source_packet))
 
-    def send_success_completion_execution_report(self, source_packet):
+    def send_success_completion_report(self, source_packet):
         self.parent.send(Packet([1, 7] + source_packet))
 
-    def send_fail_completion_execution_report(self, source_packet):
+    def send_fail_completion_report(self, source_packet):
         self.parent.send(Packet([1, 8] + source_packet))
```

### Comparing `spacecan-2.2.0/src/spacecan/services/ST03_housekeeping.py` & `spacecan-2.3.0/src/spacecan/services/ST03_housekeeping.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             for report_id in report_ids:
                 report = self.get_housekeeping_report(report_id)
                 report.enabled = True
 
             self._update_housekeeping_timer()
 
             # send success completion report
-            self.parent.request_verification.send_success_completion_execution_report(
+            self.parent.request_verification.send_success_completion_report(
                 [service, subtype]
             )
 
         # disable periodic housekeeping report
         elif case == (3, 6):
             report_ids = self._extract_report_ids(data)
             if report_ids is None:
@@ -174,15 +174,15 @@
             for report_id in report_ids:
                 report = self.get_housekeeping_report(report_id)
                 report.enabled = False
 
             self._update_housekeeping_timer()
 
             # send success completion report
-            self.parent.request_verification.send_success_completion_execution_report(
+            self.parent.request_verification.send_success_completion_report(
                 [service, subtype]
             )
 
         elif case == (3, 27):
             report_ids = self._extract_report_ids(data)
             if report_ids is None:
                 # send fail acceptance report
@@ -196,21 +196,28 @@
                 [service, subtype]
             )
 
             for report_id in report_ids:
                 self.send_housekeeping_report(report_id)
 
             # send success completion report
-            self.parent.request_verification.send_success_completion_execution_report(
+            self.parent.request_verification.send_success_completion_report(
+                [service, subtype]
+            )
+        else:
+            # send fail acceptance report
+            self.parent.request_verification.send_fail_acceptance_report(
                 [service, subtype]
             )
 
     def _extract_report_ids(self, data):
         try:
             n = data.pop(0)
+            if n == 0:
+                return None
             report_ids = list(x for x in data)
             if n != len(report_ids):
                 raise ValueError
             for report_id in report_ids:
                 if report_id not in self.housekeeping_reports:
                     raise ValueError
         except (IndexError, ValueError):
```

### Comparing `spacecan-2.2.0/src/spacecan/services/ST08_function_management.py` & `spacecan-2.3.0/src/spacecan/services/ST08_function_management.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,17 +122,29 @@
 
             if len(data) > 0:
                 n = data.pop(0)
 
             arguments = []
             for _, argument in sorted(function.arguments.items()):
                 size = argument.get_encoded_size()
-                argument_id = data.pop(0)
+                try:
+                    argument_id = data.pop(0)
+                except IndexError:
+                    # send fail acceptance report
+                    self.parent.request_verification.send_fail_acceptance_report(
+                        [service, subtype]
+                    )
+                    return
                 if argument_id != argument.argument_id:
-                    raise ValueError("Arguments order not correct")
+                    # raise ValueError("Arguments order not correct")
+                    # send fail acceptance report
+                    self.parent.request_verification.send_fail_acceptance_report(
+                        [service, subtype]
+                    )
+                    return
                 encoded_value = data[:size]
                 data = data[size:]
                 value = argument.decode(encoded_value)
                 arguments.append(value)
 
             if len(arguments) > 0 and n != len(arguments):
                 # send fail acceptance report
@@ -144,19 +156,24 @@
             # send success acceptance report
             self.parent.request_verification.send_success_acceptance_report(
                 [service, subtype]
             )
 
             if self.perform_function(function_id, arguments) is False:
                 # send fail completion report
-                self.parent.request_verification.send_fail_completion_execution_report(
+                self.parent.request_verification.send_fail_completion_report(
                     [service, subtype]
                 )
             else:
                 # send success completion report
-                self.parent.request_verification.send_success_completion_execution_report(
+                self.parent.request_verification.send_success_completion_report(
                     [service, subtype]
                 )
+        else:
+            # send fail acceptance report
+            self.parent.request_verification.send_fail_acceptance_report(
+                [service, subtype]
+            )
 
     def perform_function(self, function_id, arguments):
         # to be overwritten
         return True
```

### Comparing `spacecan-2.2.0/src/spacecan/services/ST17_test.py` & `spacecan-2.3.0/src/spacecan/services/ST17_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                 [service, subtype]
             )
 
             # reply with (17, 2)
             self.send_connection_test_report()
 
             # send success completion report
-            self.parent.request_verification.send_success_completion_execution_report(
+            self.parent.request_verification.send_success_completion_report(
                 [service, subtype]
             )
 
         elif case == (17, 3):
             apid = int.from_bytes(data)
 
             # send success acceptance report
@@ -63,22 +63,27 @@
             result = self.received_application_connection_test(apid)
 
             if result is True:
                 # reply with (17, 4)
                 self.send_application_connection_test_report(apid)
 
                 # send success completion report
-                self.parent.request_verification.send_success_completion_execution_report(
+                self.parent.request_verification.send_success_completion_report(
                     [service, subtype]
                 )
             else:
                 # send fail completion report
-                self.parent.request_verification.send_fail_completion_execution_report(
+                self.parent.request_verification.send_fail_completion_report(
                     [service, subtype]
                 )
+        else:
+            # send fail acceptance report
+            self.parent.request_verification.send_fail_acceptance_report(
+                [service, subtype]
+            )
 
     def send_connection_test_report(self):
         self.parent.send(Packet([17, 2]))
 
     def send_application_connection_test_report(self, apid):
         self.parent.send(Packet([17, 4] + [apid]))
```

### Comparing `spacecan-2.2.0/src/spacecan/services/ST20_parameter_management.py` & `spacecan-2.3.0/src/spacecan/services/ST20_parameter_management.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,15 +125,20 @@
                 [service, subtype]
             )
 
             # reply with (20, 2)
             self.send_parameter_value_report(parameter_ids)
 
             # send success completion report
-            self.parent.request_verification.send_success_completion_execution_report(
+            self.parent.request_verification.send_success_completion_report(
+                [service, subtype]
+            )
+        else:
+            # send fail acceptance report
+            self.parent.request_verification.send_fail_acceptance_report(
                 [service, subtype]
             )
 
     def _extract_parameter_ids(self, data):
         try:
             n = data.pop(0)
             parameter_ids = list(data)
```

### Comparing `spacecan-2.2.0/src/spacecan/services/core.py` & `spacecan-2.3.0/src/spacecan/services/core.py`

 * *Files identical despite different names*

### Comparing `spacecan-2.2.0/src/spacecan/transport/socketcan.py` & `spacecan-2.3.0/src/spacecan/transport/socketcan.py`

 * *Files identical despite different names*

### Comparing `spacecan-2.2.0/src/spacecan.egg-info/PKG-INFO` & `spacecan-2.3.0/src/spacecan.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacecan
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python implementation of SpaceCAN protocol
 Author-email: LibreCube <info@librecube.org>
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: python-can
```

### Comparing `spacecan-2.2.0/src/spacecan.egg-info/SOURCES.txt` & `spacecan-2.3.0/src/spacecan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

