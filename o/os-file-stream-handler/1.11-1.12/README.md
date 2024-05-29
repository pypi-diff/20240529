# Comparing `tmp/os_file_stream_handler-1.11.tar.gz` & `tmp/os_file_stream_handler-1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os_file_stream_handler-1.11.tar", last modified: Thu Nov 24 09:05:33 2022, max compression
+gzip compressed data, was "os_file_stream_handler-1.12.tar", last modified: Wed May 29 07:30:18 2024, max compression
```

## Comparing `os_file_stream_handler-1.11.tar` & `os_file_stream_handler-1.12.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2022-11-24 09:05:33.172071 os_file_stream_handler-1.11/
--rw-r--r--   0 ozshabbat   (501) staff       (20)     1065 2019-06-20 10:31:16.000000 os_file_stream_handler-1.11/LICENSE.txt
--rw-r--r--   0 ozshabbat   (501) staff       (20)      804 2022-11-24 09:05:33.172130 os_file_stream_handler-1.11/PKG-INFO
--rw-r--r--   0 ozshabbat   (501) staff       (20)     6214 2021-02-07 14:01:45.000000 os_file_stream_handler-1.11/README.md
-drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2022-11-24 09:05:33.171580 os_file_stream_handler-1.11/os_file_stream_handler/
--rw-r--r--   0 ozshabbat   (501) staff       (20)     8438 2022-11-24 09:05:14.000000 os_file_stream_handler-1.11/os_file_stream_handler/file_stream_handler.py
--rw-r--r--   0 ozshabbat   (501) staff       (20)       61 2021-02-07 14:00:44.000000 os_file_stream_handler-1.11/os_file_stream_handler/test.py
-drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2022-11-24 09:05:33.171986 os_file_stream_handler-1.11/os_file_stream_handler.egg-info/
--rw-r--r--   0 ozshabbat   (501) staff       (20)      804 2022-11-24 09:05:32.000000 os_file_stream_handler-1.11/os_file_stream_handler.egg-info/PKG-INFO
--rw-r--r--   0 ozshabbat   (501) staff       (20)      301 2022-11-24 09:05:33.000000 os_file_stream_handler-1.11/os_file_stream_handler.egg-info/SOURCES.txt
--rw-r--r--   0 ozshabbat   (501) staff       (20)        1 2022-11-24 09:05:32.000000 os_file_stream_handler-1.11/os_file_stream_handler.egg-info/dependency_links.txt
--rw-r--r--   0 ozshabbat   (501) staff       (20)       23 2022-11-24 09:05:33.000000 os_file_stream_handler-1.11/os_file_stream_handler.egg-info/top_level.txt
--rw-r--r--   0 ozshabbat   (501) staff       (20)       38 2022-11-24 09:05:33.172398 os_file_stream_handler-1.11/setup.cfg
--rw-r--r--   0 ozshabbat   (501) staff       (20)     1576 2022-11-24 09:05:24.000000 os_file_stream_handler-1.11/setup.py
+drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2024-05-29 07:30:18.529569 os_file_stream_handler-1.12/
+-rw-r--r--   0 ozshabbat   (501) staff       (20)     1065 2019-06-20 10:31:16.000000 os_file_stream_handler-1.12/LICENSE.txt
+-rw-r--r--   0 ozshabbat   (501) staff       (20)      776 2024-05-29 07:30:18.529512 os_file_stream_handler-1.12/PKG-INFO
+-rw-r--r--   0 ozshabbat   (501) staff       (20)     6214 2021-02-07 14:01:45.000000 os_file_stream_handler-1.12/README.md
+drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2024-05-29 07:30:18.528679 os_file_stream_handler-1.12/os_file_stream_handler/
+-rw-r--r--   0 ozshabbat   (501) staff       (20)     9343 2024-05-29 07:24:53.000000 os_file_stream_handler-1.12/os_file_stream_handler/file_stream_handler.py
+-rw-r--r--   0 ozshabbat   (501) staff       (20)       61 2021-02-07 14:00:44.000000 os_file_stream_handler-1.12/os_file_stream_handler/test.py
+drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2024-05-29 07:30:18.529355 os_file_stream_handler-1.12/os_file_stream_handler.egg-info/
+-rw-r--r--   0 ozshabbat   (501) staff       (20)      776 2024-05-29 07:30:18.000000 os_file_stream_handler-1.12/os_file_stream_handler.egg-info/PKG-INFO
+-rw-r--r--   0 ozshabbat   (501) staff       (20)      301 2024-05-29 07:30:18.000000 os_file_stream_handler-1.12/os_file_stream_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 ozshabbat   (501) staff       (20)        1 2024-05-29 07:30:18.000000 os_file_stream_handler-1.12/os_file_stream_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 ozshabbat   (501) staff       (20)       23 2024-05-29 07:30:18.000000 os_file_stream_handler-1.12/os_file_stream_handler.egg-info/top_level.txt
+-rw-r--r--   0 ozshabbat   (501) staff       (20)       38 2024-05-29 07:30:18.529725 os_file_stream_handler-1.12/setup.cfg
+-rw-r--r--   0 ozshabbat   (501) staff       (20)     1576 2024-05-29 07:25:11.000000 os_file_stream_handler-1.12/setup.py
```

### Comparing `os_file_stream_handler-1.11/LICENSE.txt` & `os_file_stream_handler-1.12/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `os_file_stream_handler-1.11/PKG-INFO` & `os_file_stream_handler-1.12/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: os_file_stream_handler
-Version: 1.11
+Version: 1.12
 Summary: py file stream handling tools for os
 Home-page: https://github.com/osfunapps/os-file-stream-handler-py
 Author: Oz Shabat
 Author-email: support@os-apps.com
 License: MIT
 Keywords: python,osfunapps,files,tools,utils,stream
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `os_file_stream_handler-1.11/README.md` & `os_file_stream_handler-1.12/README.md`

 * *Files identical despite different names*

### Comparing `os_file_stream_handler-1.11/os_file_stream_handler/file_stream_handler.py` & `os_file_stream_handler-1.12/os_file_stream_handler/file_stream_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -229,14 +229,42 @@
                     text_to_return.append(lines[i])
                 return text_to_return
             else:
                 text_to_return.append(lines[i])
     return None
 
 
+# will uncomment a line. For example:
+# uncommentLineInFile("#", "pod 'google-cast-sdk-no-bluetooth'", os.path.join(finals.PROJECT_PATH, 'Podfile'))
+def uncomment_line_in_file(comment_sign, line_to_uncomment, file_path):
+    try:
+        with open(file_path, 'r') as file:
+            lines = file.readlines()
+
+        line_changed = False
+        new_lines = []
+        for line in lines:
+            stripped_line = line.lstrip()
+            if stripped_line.startswith(comment_sign + line_to_uncomment):
+                new_lines.append(line.replace(comment_sign, '', 1))
+                line_changed = True
+            else:
+                new_lines.append(line)
+
+        if line_changed:
+            with open(file_path, 'w') as file:
+                file.writelines(new_lines)
+
+        return line_changed
+
+    except Exception as e:
+        print(f"An error occurred: {e}")
+        return False
+
+
 def clear_text_from_last(lines, text):
     for i in reversed(range(0, len(lines))):
         found = False
         if text in lines[i]:
             found = True
         lines.pop(-1)
         if found:
```

### Comparing `os_file_stream_handler-1.11/os_file_stream_handler.egg-info/PKG-INFO` & `os_file_stream_handler-1.12/os_file_stream_handler.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: os-file-stream-handler
-Version: 1.11
+Version: 1.12
 Summary: py file stream handling tools for os
 Home-page: https://github.com/osfunapps/os-file-stream-handler-py
 Author: Oz Shabat
 Author-email: support@os-apps.com
 License: MIT
 Keywords: python,osfunapps,files,tools,utils,stream
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `os_file_stream_handler-1.11/setup.py` & `os_file_stream_handler-1.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='os_file_stream_handler',  # How you named your package folder (MyLib)
     packages=['os_file_stream_handler'],  # Choose the same as "name"
-    version='1.11',  # Start with a small number and increase it with every change you make
+    version='1.12',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='py file stream handling tools for os',  # Give a short description about your library
     author='Oz Shabat',  # Type in your name
     author_email='support@os-apps.com',  # Type in your E-Mail
     url='https://github.com/osfunapps/os-file-stream-handler-py',  # Provide either the link to your github or to your website
     keywords=['python', 'osfunapps', 'files', 'tools', 'utils', 'stream'],  # Keywords that define your package best
     install_requires=[],
```

