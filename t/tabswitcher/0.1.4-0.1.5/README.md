# Comparing `tmp/tabswitcher-0.1.4.tar.gz` & `tmp/tabswitcher-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabswitcher-0.1.4.tar", last modified: Tue May 28 13:52:39 2024, max compression
+gzip compressed data, was "tabswitcher-0.1.5.tar", last modified: Wed May 29 17:27:58 2024, max compression
```

## Comparing `tabswitcher-0.1.4.tar` & `tabswitcher-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:52:39.954684 tabswitcher-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-28 13:52:39.954684 tabswitcher-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:52:39.954684 tabswitcher-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:52:39.950684 tabswitcher-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:52:39.950684 tabswitcher-0.1.4/src/tabswitcher/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/NetworkImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/SearchInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/TabList.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/VisibilityChecker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:52:39.954684 tabswitcher-0.1.4/src/tabswitcher/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/assets/Icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/assets/install.bat
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/assets/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/assets/sans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/assets/searchIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/assets/tabswitcher_service.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/brotab.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/focusWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/fuzzySearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/loadBookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/logTabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 13:52:33.000000 tabswitcher-0.1.4/src/tabswitcher/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:52:39.954684 tabswitcher-0.1.4/tabswitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-28 13:52:39.000000 tabswitcher-0.1.4/tabswitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-28 13:52:39.000000 tabswitcher-0.1.4/tabswitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:52:39.000000 tabswitcher-0.1.4/tabswitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 13:52:39.000000 tabswitcher-0.1.4/tabswitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-28 13:52:39.000000 tabswitcher-0.1.4/tabswitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 13:52:39.000000 tabswitcher-0.1.4/tabswitcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:27:58.322837 tabswitcher-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-29 17:27:58.322837 tabswitcher-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:27:58.322837 tabswitcher-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:27:58.314837 tabswitcher-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:27:58.318837 tabswitcher-0.1.5/src/tabswitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/NetworkImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/SearchInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/TabList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/VisibilityChecker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:27:58.322837 tabswitcher-0.1.5/src/tabswitcher/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/assets/Icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/assets/install.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/assets/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/assets/sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/assets/searchIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/assets/tabswitcher_service.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/brotab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/focusWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/fuzzySearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/loadBookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/logTabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:27:58.322837 tabswitcher-0.1.5/tabswitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-29 17:27:58.000000 tabswitcher-0.1.5/tabswitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-29 17:27:58.000000 tabswitcher-0.1.5/tabswitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:27:58.000000 tabswitcher-0.1.5/tabswitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-29 17:27:58.000000 tabswitcher-0.1.5/tabswitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-29 17:27:58.000000 tabswitcher-0.1.5/tabswitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 17:27:58.000000 tabswitcher-0.1.5/tabswitcher.egg-info/top_level.txt
```

### Comparing `tabswitcher-0.1.4/LICENCE` & `tabswitcher-0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/PKG-INFO` & `tabswitcher-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
@@ -21,15 +21,15 @@
 Requires-Dist: chardet<4
 Requires-Dist: werkzeug<3.0
 Requires-Dist: psutil==5.9.4
 Requires-Dist: fuzzywuzzy
 Requires-Dist: PyQt5
 Requires-Dist: schedule
 Requires-Dist: brotab
-Requires-Dist: pynput
+Requires-Dist: pynput; platform_system == "Windows"
 Requires-Dist: pywin32; platform_system == "Windows"
 
 # TabSwitcher
 
 TabSwitcher is a simple window for switching between tabs in a browser. It uses the [brotab](https://github.com/balta2ar/brotab) CLI and browser extensions as a foundation.
 
 ## Requirements
```

### Comparing `tabswitcher-0.1.4/README.md` & `tabswitcher-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/setup.py` & `tabswitcher-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tabswitcher',
-    version='0.1.4',
+    version='0.1.5',
     packages=['tabswitcher'],
     package_dir={'tabswitcher': 'src/tabswitcher'},
     package_data={'tabswitcher': ['assets/*']},
     description="A tool for efficient browser tab switching outside the browser",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='YukiGasai',
@@ -34,11 +34,11 @@
         'chardet<4',
         'werkzeug<3.0', # werkzeug 3.0 breaks flask and by extension brotab
         'psutil==5.9.4', # psutil is the first version that supports the wheels for multiple python versions
         'fuzzywuzzy',
         'PyQt5',
         'schedule',
         'brotab',
-        'pynput',
+        'pynput;platform_system=="Windows"',
         'pywin32;platform_system=="Windows"',
     ],
 )
```

### Comparing `tabswitcher-0.1.4/src/tabswitcher/NetworkImage.py` & `tabswitcher-0.1.5/src/tabswitcher/NetworkImage.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/SearchInput.py` & `tabswitcher-0.1.5/src/tabswitcher/SearchInput.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/Settings.py` & `tabswitcher-0.1.5/src/tabswitcher/Settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         }
         self.config['Functions'] = {
             'UseFzf': 'False',
             'EnableTabLogging': 'True',
             'TabLoggingInterval': '1',
             'TabLoggingMax': '10',
             'TabLoggingFile': 'tabHistory.pkl',
+            'LoadBookmarks': True
         }
         with open(self.config_file, 'w') as configfile:
             self.config.write(configfile)
 
     def load_settings(self):
         self.config.read(self.config_file)
 
@@ -51,8 +52,12 @@
         return self.config.getint('Functions', 'TabLoggingInterval')
     
     def get_tab_logging_max(self):
         return self.config.getint('Functions', 'TabLoggingMax')
     
     def get_tab_logging_file(self):
         return self.config.get('Functions', 'TabLoggingFile')
+    
+    def get_load_bookmarks(self):
+        return self.config.getboolean('Functions', 'LoadBookmarks')
+
```

### Comparing `tabswitcher-0.1.4/src/tabswitcher/Tab.py` & `tabswitcher-0.1.5/src/tabswitcher/Tab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/TabList.py` & `tabswitcher-0.1.5/src/tabswitcher/TabList.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/VisibilityChecker.py` & `tabswitcher-0.1.5/src/tabswitcher/VisibilityChecker.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/__main__.py` & `tabswitcher-0.1.5/src/tabswitcher/__main__.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/actions.py` & `tabswitcher-0.1.5/src/tabswitcher/actions.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/assets/Icon.ico` & `tabswitcher-0.1.5/src/tabswitcher/assets/Icon.ico`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/assets/install.bat` & `tabswitcher-0.1.5/src/tabswitcher/assets/install.bat`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/assets/sans.ttf` & `tabswitcher-0.1.5/src/tabswitcher/assets/sans.ttf`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/assets/tabswitcher_service.xml` & `tabswitcher-0.1.5/src/tabswitcher/assets/tabswitcher_service.xml`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/brotab.py` & `tabswitcher-0.1.5/src/tabswitcher/brotab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/colors.py` & `tabswitcher-0.1.5/src/tabswitcher/colors.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/focusWindow.py` & `tabswitcher-0.1.5/src/tabswitcher/focusWindow.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/fuzzySearch.py` & `tabswitcher-0.1.5/src/tabswitcher/fuzzySearch.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/loadBookmarks.py` & `tabswitcher-0.1.5/src/tabswitcher/loadBookmarks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 import sqlite3
 import json
 import os
 
+from tabswitcher.Settings import Settings
+
+settings = Settings()
+
 def load_chrome_bookmarks():
 
     # Path to the Chrome bookmarks file
     bookmarks_file = os.path.expanduser("~/AppData/Local/Google/Chrome/User Data/Default/Bookmarks")
 
     if not os.path.exists(bookmarks_file):
         return []
 
     # Load the bookmarks file
-    with open(bookmarks_file, 'r') as f:
+    with open(bookmarks_file, 'r', encoding='utf-8') as f:
         bookmarks_data = json.load(f)
 
     # Initialize an empty list to store the bookmarks
     bookmarks = []
-
     # Recursive function to extract bookmarks from the nested structure
     def extract_bookmarks(node):
-        if 'children' in node:
-            for child in node['children']:
-                extract_bookmarks(child)
-        elif node['type'] == 'url':
-            bookmarks.append((node['name'], node['url']))
+        for child in node:
+            if not isinstance(child, dict):
+                continue
+            if 'type' in child:
+                if child['type'] == 'folder':
+                    for subChild in child['children']:
+                        extract_bookmarks(subChild)
+                elif child['type'] == 'url':
+                    bookmarks.append((child.get('name', ''), child.get('url', '')))
 
     # Extract bookmarks from the root node
-    extract_bookmarks(bookmarks_data['roots'])
+    if 'roots' in bookmarks_data:
+        for subnode in bookmarks_data['roots'].values():
+            if 'children' in subnode:
+                extract_bookmarks(subnode['children'])
 
     return bookmarks
 
 
 def load_firefox_bookmark():
 
     # Path to the Firefox profiles directory
@@ -75,10 +85,14 @@
 
     # Close the 
     # connection
     conn.close()
     return bookmarks
 
 def load_bookmarks():
+
+    if not settings.get_load_bookmarks():
+        return []
+    
     chrome_bookmarks = load_chrome_bookmarks()
     firefox_bookmarks = load_firefox_bookmark()
     return chrome_bookmarks + firefox_bookmarks
```

### Comparing `tabswitcher-0.1.4/src/tabswitcher/logTabs.py` & `tabswitcher-0.1.5/src/tabswitcher/logTabs.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/src/tabswitcher/shortcuts.py` & `tabswitcher-0.1.5/src/tabswitcher/shortcuts.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.4/tabswitcher.egg-info/PKG-INFO` & `tabswitcher-0.1.5/tabswitcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
@@ -21,15 +21,15 @@
 Requires-Dist: chardet<4
 Requires-Dist: werkzeug<3.0
 Requires-Dist: psutil==5.9.4
 Requires-Dist: fuzzywuzzy
 Requires-Dist: PyQt5
 Requires-Dist: schedule
 Requires-Dist: brotab
-Requires-Dist: pynput
+Requires-Dist: pynput; platform_system == "Windows"
 Requires-Dist: pywin32; platform_system == "Windows"
 
 # TabSwitcher
 
 TabSwitcher is a simple window for switching between tabs in a browser. It uses the [brotab](https://github.com/balta2ar/brotab) CLI and browser extensions as a foundation.
 
 ## Requirements
```

### Comparing `tabswitcher-0.1.4/tabswitcher.egg-info/SOURCES.txt` & `tabswitcher-0.1.5/tabswitcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

