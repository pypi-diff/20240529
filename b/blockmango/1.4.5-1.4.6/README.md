# Comparing `tmp/blockmango-1.4.5.tar.gz` & `tmp/blockmango-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.4.5.tar", last modified: Tue May 28 20:22:04 2024, max compression
+gzip compressed data, was "blockmango-1.4.6.tar", last modified: Tue May 28 23:58:53 2024, max compression
```

## Comparing `blockmango-1.4.5.tar` & `blockmango-1.4.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-28 20:22:04.902259 blockmango-1.4.5/
--rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.5/LICENSE.md
--rw-------   0 userland  (2000) userland  (2000)     1716 2024-05-28 20:22:04.902259 blockmango-1.4.5/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      834 2024-05-16 17:43:12.000000 blockmango-1.4.5/README.md
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-28 20:22:04.882259 blockmango-1.4.5/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      200 2024-05-17 15:51:17.000000 blockmango-1.4.5/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     4177 2024-05-28 20:15:07.000000 blockmango-1.4.5/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)     1336 2024-05-28 20:16:13.000000 blockmango-1.4.5/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)     2231 2024-05-28 20:15:48.000000 blockmango-1.4.5/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     3520 2024-05-28 20:20:04.000000 blockmango-1.4.5/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     1225 2024-05-28 20:20:42.000000 blockmango-1.4.5/blockmango/http.py
--rw-------   0 userland  (2000) userland  (2000)     2105 2024-05-28 20:19:37.000000 blockmango-1.4.5/blockmango/user.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-28 20:22:04.898259 blockmango-1.4.5/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)     1716 2024-05-28 20:22:04.000000 blockmango-1.4.5/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      349 2024-05-28 20:22:04.000000 blockmango-1.4.5/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-28 20:22:04.000000 blockmango-1.4.5/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-28 20:22:04.000000 blockmango-1.4.5/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-28 20:22:04.000000 blockmango-1.4.5/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-28 20:22:04.902259 blockmango-1.4.5/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)     1091 2024-05-28 20:14:26.000000 blockmango-1.4.5/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-28 23:58:53.412850 blockmango-1.4.6/
+-rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.6/LICENSE.md
+-rw-------   0 userland  (2000) userland  (2000)    14576 2024-05-28 23:58:53.412850 blockmango-1.4.6/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      571 2024-05-28 23:52:58.000000 blockmango-1.4.6/README.md
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-28 23:58:53.396849 blockmango-1.4.6/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      200 2024-05-17 15:51:17.000000 blockmango-1.4.6/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     4177 2024-05-28 20:15:07.000000 blockmango-1.4.6/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)     1336 2024-05-28 20:16:13.000000 blockmango-1.4.6/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)     2231 2024-05-28 20:15:48.000000 blockmango-1.4.6/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     3520 2024-05-28 20:20:04.000000 blockmango-1.4.6/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     1225 2024-05-28 20:20:42.000000 blockmango-1.4.6/blockmango/http.py
+-rw-------   0 userland  (2000) userland  (2000)     2105 2024-05-28 20:19:37.000000 blockmango-1.4.6/blockmango/user.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-28 23:58:53.408849 blockmango-1.4.6/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)    14576 2024-05-28 23:58:53.000000 blockmango-1.4.6/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      349 2024-05-28 23:58:53.000000 blockmango-1.4.6/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-28 23:58:53.000000 blockmango-1.4.6/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-28 23:58:53.000000 blockmango-1.4.6/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-28 23:58:53.000000 blockmango-1.4.6/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-28 23:58:53.412850 blockmango-1.4.6/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)     1888 2024-05-28 23:57:45.000000 blockmango-1.4.6/setup.py
```

### Comparing `blockmango-1.4.5/LICENSE.md` & `blockmango-1.4.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.5/blockmango/clan.py` & `blockmango-1.4.6/blockmango/clan.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.5/blockmango/decoration.py` & `blockmango-1.4.6/blockmango/decoration.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.5/blockmango/friends.py` & `blockmango-1.4.6/blockmango/friends.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.5/blockmango/groupchat.py` & `blockmango-1.4.6/blockmango/groupchat.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.5/blockmango/http.py` & `blockmango-1.4.6/blockmango/http.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.5/blockmango/user.py` & `blockmango-1.4.6/blockmango/user.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.5/setup.py` & `blockmango-1.4.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,35 @@
 from setuptools import setup
+import os
 
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
+def read_md_files(filenames):
+    content = ""
+    for filename in filenames:
+        if filename == "README.md":
+            with open(filename, "r", encoding="utf-8") as file:
+                content += file.read() + "\n\n"
+        else:
+            with open(os.path.join("docs", filename), "r", encoding="utf-8") as file:
+                content += file.read() + "\n\n"
+    return content
+
+markdown_files = [
+    "README.md",
+    "friends.md",
+    "groupchat.md",
+    "user.md",
+    "clan.md",
+    "decoration.md"
+]
+
+long_description = read_md_files(markdown_files)
 
 setup(
     name='blockmango',
-    version='1.4.5',
+    version='1.4.6',
     author='Dark',
     author_email='darkness0777@proton.me',
     description='Blockman Go API package',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/darkkpy/blockmango',
     packages=['blockmango'],
@@ -24,8 +44,15 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
+    project_urls={
+        'Documentation': 'https://github.com/darkkpy/blockmango/tree/main/docs',
+        'Source': 'https://github.com/darkkpy/blockmango',
+        'Tracker': 'https://github.com/darkkpy/blockmango/issues',
+    },
+    keywords='blockmango blockman go api wrapper',
+    license='MIT',
 )
```

