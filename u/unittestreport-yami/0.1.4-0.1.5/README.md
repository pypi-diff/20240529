# Comparing `tmp/unittestreport_yami-0.1.4.tar.gz` & `tmp/unittestreport_yami-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unittestreport_yami-0.1.4.tar", last modified: Wed May 22 09:32:51 2024, max compression
+gzip compressed data, was "unittestreport_yami-0.1.5.tar", last modified: Wed May 29 02:38:37 2024, max compression
```

## Comparing `unittestreport_yami-0.1.4.tar` & `unittestreport_yami-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 09:32:51.789163 unittestreport_yami-0.1.4/
--rw-rw-rw-   0        0        0     1091 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2111 2024-05-22 09:32:51.787164 unittestreport_yami-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1686 2024-05-22 03:00:51.000000 unittestreport_yami-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 09:32:51.789751 unittestreport_yami-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-05-22 09:32:24.000000 unittestreport_yami-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:32:51.732988 unittestreport_yami-0.1.4/unittestreport_yami/
--rw-rw-rw-   0        0        0      145 2024-05-22 02:31:24.000000 unittestreport_yami-0.1.4/unittestreport_yami/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:32:51.765563 unittestreport_yami-0.1.4/unittestreport_yami/core/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.4/unittestreport_yami/core/__init__.py
--rw-rw-rw-   0        0        0     2755 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.4/unittestreport_yami/core/dataDriver.py
--rw-rw-rw-   0        0        0    22987 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.4/unittestreport_yami/core/parameterized.py
--rw-rw-rw-   0        0        0     1009 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.4/unittestreport_yami/core/reRun.py
--rw-rw-rw-   0        0        0     4996 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.4/unittestreport_yami/core/resultPush.py
--rw-rw-rw-   0        0        0     2500 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.4/unittestreport_yami/core/sendEmail.py
--rw-rw-rw-   0        0        0     6999 2024-05-22 07:19:43.000000 unittestreport_yami-0.1.4/unittestreport_yami/core/testResult.py
--rw-rw-rw-   0        0        0    12886 2024-05-22 06:26:24.000000 unittestreport_yami-0.1.4/unittestreport_yami/core/testRunner.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:32:51.786008 unittestreport_yami-0.1.4/unittestreport_yami/templates/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.4/unittestreport_yami/templates/__init__.py
--rw-rw-rw-   0        0        0      318 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.4/unittestreport_yami/templates/dingtalk.md
--rw-rw-rw-   0        0        0    18656 2024-04-05 03:28:31.000000 unittestreport_yami-0.1.4/unittestreport_yami/templates/templates.html
--rw-rw-rw-   0        0        0     2464 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.4/unittestreport_yami/templates/templates03.html
--rw-rw-rw-   0        0        0    25462 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.4/unittestreport_yami/templates/templates2.html
--rw-rw-rw-   0        0        0   197083 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.4/unittestreport_yami/templates/templates3.html
-drwxrwxrwx   0        0        0        0 2024-05-22 09:32:51.752953 unittestreport_yami-0.1.4/unittestreport_yami.egg-info/
--rw-rw-rw-   0        0        0     2111 2024-05-22 09:32:51.000000 unittestreport_yami-0.1.4/unittestreport_yami.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      859 2024-05-22 09:32:51.000000 unittestreport_yami-0.1.4/unittestreport_yami.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 09:32:51.000000 unittestreport_yami-0.1.4/unittestreport_yami.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-22 09:32:51.000000 unittestreport_yami-0.1.4/unittestreport_yami.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-22 09:32:51.000000 unittestreport_yami-0.1.4/unittestreport_yami.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 02:38:37.118533 unittestreport_yami-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2111 2024-05-29 02:38:37.115537 unittestreport_yami-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1686 2024-05-22 03:00:51.000000 unittestreport_yami-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 02:38:37.119533 unittestreport_yami-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-05-29 02:38:08.000000 unittestreport_yami-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:38:37.026053 unittestreport_yami-0.1.5/unittestreport_yami/
+-rw-rw-rw-   0        0        0      190 2024-05-29 02:14:58.000000 unittestreport_yami-0.1.5/unittestreport_yami/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:38:37.098532 unittestreport_yami-0.1.5/unittestreport_yami/core/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/__init__.py
+-rw-rw-rw-   0        0        0     2755 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/dataDriver.py
+-rw-rw-rw-   0        0        0    22987 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/parameterized.py
+-rw-rw-rw-   0        0        0     1009 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/reRun.py
+-rw-rw-rw-   0        0        0     4996 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/resultPush.py
+-rw-rw-rw-   0        0        0     2500 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/sendEmail.py
+-rw-rw-rw-   0        0        0     7279 2024-05-29 02:23:45.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/testResult.py
+-rw-rw-rw-   0        0        0    12886 2024-05-29 01:16:12.000000 unittestreport_yami-0.1.5/unittestreport_yami/core/testRunner.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:38:37.111533 unittestreport_yami-0.1.5/unittestreport_yami/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.5/unittestreport_yami/templates/__init__.py
+-rw-rw-rw-   0        0        0      318 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/unittestreport_yami/templates/dingtalk.md
+-rw-rw-rw-   0        0        0    18656 2024-04-05 03:28:31.000000 unittestreport_yami-0.1.5/unittestreport_yami/templates/templates.html
+-rw-rw-rw-   0        0        0     2464 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/unittestreport_yami/templates/templates03.html
+-rw-rw-rw-   0        0        0    25462 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/unittestreport_yami/templates/templates2.html
+-rw-rw-rw-   0        0        0   197083 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.5/unittestreport_yami/templates/templates3.html
+drwxrwxrwx   0        0        0        0 2024-05-29 02:38:37.081533 unittestreport_yami-0.1.5/unittestreport_yami.egg-info/
+-rw-rw-rw-   0        0        0     2111 2024-05-29 02:38:36.000000 unittestreport_yami-0.1.5/unittestreport_yami.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      859 2024-05-29 02:38:36.000000 unittestreport_yami-0.1.5/unittestreport_yami.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 02:38:36.000000 unittestreport_yami-0.1.5/unittestreport_yami.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-29 02:38:36.000000 unittestreport_yami-0.1.5/unittestreport_yami.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-29 02:38:36.000000 unittestreport_yami-0.1.5/unittestreport_yami.egg-info/top_level.txt
```

### Comparing `unittestreport_yami-0.1.4/LICENSE` & `unittestreport_yami-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.4/PKG-INFO` & `unittestreport_yami-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittestreport_yami
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://github.com/EthanLiuInyami/UnitTestReport
 Author: Ethan
 Author-email: ethan.liu@yamibuy.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `unittestreport_yami-0.1.4/README.md` & `unittestreport_yami-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.4/setup.py` & `unittestreport_yami-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
     name="unittestreport_yami",
-    version="0.1.4",
+    version="0.1.5",
     author="Ethan",
     author_email="ethan.liu@yamibuy.com",
     url="https://github.com/EthanLiuInyami/UnitTestReport",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["Jinja2==3.1.2", "PyYAML==5.3.1", "requests==2.32.2"],
```

### Comparing `unittestreport_yami-0.1.4/unittestreport_yami/core/dataDriver.py` & `unittestreport_yami-0.1.5/unittestreport_yami/core/dataDriver.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.4/unittestreport_yami/core/parameterized.py` & `unittestreport_yami-0.1.5/unittestreport_yami/core/parameterized.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.4/unittestreport_yami/core/reRun.py` & `unittestreport_yami-0.1.5/unittestreport_yami/core/reRun.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.4/unittestreport_yami/core/resultPush.py` & `unittestreport_yami-0.1.5/unittestreport_yami/core/resultPush.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.4/unittestreport_yami/core/sendEmail.py` & `unittestreport_yami-0.1.5/unittestreport_yami/core/sendEmail.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.4/unittestreport_yami/core/testResult.py` & `unittestreport_yami-0.1.5/unittestreport_yami/core/testResult.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,24 @@
         self.fp.flush()
 
 
 stdout_redirector = OutputRedirector(sys.stdout)
 stderr_redirector = OutputRedirector(sys.stderr)
 
 
+def add_screenshot(test):
+    if type(getattr(test, "driver", "")).__name__ == "WebDriver":
+        try:
+            driver = getattr(test, "driver")
+            test.images.append(driver.get_screenshot_as_base64())
+        except Exception as e:
+            print(e)
+            driver.quit()
+
+
 class TestResult(unittest.TestResult):
     def __init__(self):
         super().__init__()
 
         self.fields = {
             "success": 0,
             "all": 0,
@@ -94,42 +104,43 @@
                 self.fields["skip"],
                 self.fields["success"],
             ]
         )
         self.fields["testClass"] = list(self.fields["testClass"])
 
     def addSuccess(self, test):
+        self._add_screen_shot_in_test(test)
         self.fields["success"] += 1
         test.state = "成功"
         sys.stdout.write("{}执行——>【通过】\n".format(test))
         logs = []
         output = self.complete_output()
         logs.append(output)
         test.run_info = logs
-        self._add_screen_shot_in_test(test)
 
     def addFailure(self, test, err):
+        self._add_screen_shot_in_test(test)
         super().addFailure(test, err)
         logs = []
         test.state = "失败"
         sys.stderr.write("{}执行——>【失败】\n".format(test))
         output = self.complete_output()
         logs.append(output)
         logs.extend(traceback.format_exception(*err))
         test.run_info = logs
-        self._add_screen_shot_in_test(test)
 
     def addSkip(self, test, reason):
         super().addSkip(test, reason)
         test.state = "跳过"
         sys.stdout.write("{}执行--【跳过Skip】\n".format(test))
         logs = [reason]
         test.run_info = logs
 
     def addError(self, test, err):
+        self._add_screen_shot_in_test(test)
         super().addError(test, err)
         test.state = "错误"
         sys.stderr.write("{}执行——>【错误Error】\n".format(test))
         logs = []
         logs.extend(traceback.format_exception(*err))
         test.run_info = logs
         if test.__class__.__qualname__ == "_ErrorHolder":
@@ -139,23 +150,23 @@
             test.method_name = res.group(1)
             test.method_doc = test.shortDescription()
             self.fields["results"].append(test)
             self.fields["testClass"].add(test.class_name)
         else:
             output = self.complete_output()
             logs.append(output)
-        self._add_screen_shot_in_test(test)
 
     def _add_screen_shot_in_test(self, test):
+        add_screenshot(test)
+        self._close_driver(test)
+
+    def _close_driver(self, test):
         if type(getattr(test, "driver", "")).__name__ == "WebDriver":
             driver = getattr(test, "driver")
-            try:
-                test.images.append(driver.get_screenshot_as_base64())
-            except BaseException as e:
-                print(e)
+            driver.quit()
 
 
 class ReRunResult(TestResult):
 
     def __init__(self, count, interval):
         super().__init__()
         self.count = count
```

### Comparing `unittestreport_yami-0.1.4/unittestreport_yami/core/testRunner.py` & `unittestreport_yami-0.1.5/unittestreport_yami/core/testRunner.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.4/unittestreport_yami/templates/templates.html` & `unittestreport_yami-0.1.5/unittestreport_yami/templates/templates.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.4/unittestreport_yami/templates/templates03.html` & `unittestreport_yami-0.1.5/unittestreport_yami/templates/templates03.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.4/unittestreport_yami/templates/templates2.html` & `unittestreport_yami-0.1.5/unittestreport_yami/templates/templates2.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.4/unittestreport_yami/templates/templates3.html` & `unittestreport_yami-0.1.5/unittestreport_yami/templates/templates3.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.4/unittestreport_yami.egg-info/PKG-INFO` & `unittestreport_yami-0.1.5/unittestreport_yami.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittestreport-yami
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://github.com/EthanLiuInyami/UnitTestReport
 Author: Ethan
 Author-email: ethan.liu@yamibuy.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `unittestreport_yami-0.1.4/unittestreport_yami.egg-info/SOURCES.txt` & `unittestreport_yami-0.1.5/unittestreport_yami.egg-info/SOURCES.txt`

 * *Files identical despite different names*

