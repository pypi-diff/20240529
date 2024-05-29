# Comparing `tmp/tabswitcher-0.1.5.tar.gz` & `tmp/tabswitcher-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabswitcher-0.1.5.tar", last modified: Wed May 29 17:27:58 2024, max compression
+gzip compressed data, was "tabswitcher-0.1.7.tar", last modified: Wed May 29 19:52:57 2024, max compression
```

## Comparing `tabswitcher-0.1.5.tar` & `tabswitcher-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:27:58.322837 tabswitcher-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-29 17:27:58.322837 tabswitcher-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:27:58.322837 tabswitcher-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:27:58.314837 tabswitcher-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:27:58.318837 tabswitcher-0.1.5/src/tabswitcher/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/NetworkImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/SearchInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/TabList.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/VisibilityChecker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:27:58.322837 tabswitcher-0.1.5/src/tabswitcher/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/assets/Icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/assets/install.bat
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/assets/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/assets/sans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/assets/searchIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/assets/tabswitcher_service.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/brotab.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/focusWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/fuzzySearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/loadBookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/logTabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 17:27:54.000000 tabswitcher-0.1.5/src/tabswitcher/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:27:58.322837 tabswitcher-0.1.5/tabswitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-29 17:27:58.000000 tabswitcher-0.1.5/tabswitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-29 17:27:58.000000 tabswitcher-0.1.5/tabswitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:27:58.000000 tabswitcher-0.1.5/tabswitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-29 17:27:58.000000 tabswitcher-0.1.5/tabswitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-29 17:27:58.000000 tabswitcher-0.1.5/tabswitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 17:27:58.000000 tabswitcher-0.1.5/tabswitcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:52:57.876142 tabswitcher-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-29 19:52:57.876142 tabswitcher-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:52:57.876142 tabswitcher-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:52:57.868142 tabswitcher-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:52:57.872142 tabswitcher-0.1.7/src/tabswitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/NetworkImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/SearchInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/TabList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/VisibilityChecker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:52:57.876142 tabswitcher-0.1.7/src/tabswitcher/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/assets/Icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/assets/install.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/assets/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/assets/sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/assets/searchIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/assets/tabswitcher_service.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/brotab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/focusWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/fuzzySearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/loadBookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/logTabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:52:57.876142 tabswitcher-0.1.7/tabswitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-29 19:52:57.000000 tabswitcher-0.1.7/tabswitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-29 19:52:57.000000 tabswitcher-0.1.7/tabswitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:52:57.000000 tabswitcher-0.1.7/tabswitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-29 19:52:57.000000 tabswitcher-0.1.7/tabswitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-29 19:52:57.000000 tabswitcher-0.1.7/tabswitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 19:52:57.000000 tabswitcher-0.1.7/tabswitcher.egg-info/top_level.txt
```

### Comparing `tabswitcher-0.1.5/LICENCE` & `tabswitcher-0.1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/PKG-INFO` & `tabswitcher-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.1.5
+Version: 0.1.7
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
@@ -23,14 +23,15 @@
 Requires-Dist: psutil==5.9.4
 Requires-Dist: fuzzywuzzy
 Requires-Dist: PyQt5
 Requires-Dist: schedule
 Requires-Dist: brotab
 Requires-Dist: pynput; platform_system == "Windows"
 Requires-Dist: pywin32; platform_system == "Windows"
+Requires-Dist: keyboard; platform_system == "Windows"
 
 # TabSwitcher
 
 TabSwitcher is a simple window for switching between tabs in a browser. It uses the [brotab](https://github.com/balta2ar/brotab) CLI and browser extensions as a foundation.
 
 ## Requirements
```

### Comparing `tabswitcher-0.1.5/README.md` & `tabswitcher-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/setup.py` & `tabswitcher-0.1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tabswitcher',
-    version='0.1.5',
+    version='0.1.7',
     packages=['tabswitcher'],
     package_dir={'tabswitcher': 'src/tabswitcher'},
     package_data={'tabswitcher': ['assets/*']},
     description="A tool for efficient browser tab switching outside the browser",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='YukiGasai',
@@ -36,9 +36,10 @@
         'psutil==5.9.4', # psutil is the first version that supports the wheels for multiple python versions
         'fuzzywuzzy',
         'PyQt5',
         'schedule',
         'brotab',
         'pynput;platform_system=="Windows"',
         'pywin32;platform_system=="Windows"',
+        'keyboard;platform_system=="Windows"'
     ],
 )
```

### Comparing `tabswitcher-0.1.5/src/tabswitcher/NetworkImage.py` & `tabswitcher-0.1.7/src/tabswitcher/NetworkImage.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/src/tabswitcher/SearchInput.py` & `tabswitcher-0.1.7/src/tabswitcher/SearchInput.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/src/tabswitcher/Tab.py` & `tabswitcher-0.1.7/src/tabswitcher/Tab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/src/tabswitcher/TabList.py` & `tabswitcher-0.1.7/src/tabswitcher/TabList.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/src/tabswitcher/VisibilityChecker.py` & `tabswitcher-0.1.7/src/tabswitcher/VisibilityChecker.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/src/tabswitcher/__main__.py` & `tabswitcher-0.1.7/src/tabswitcher/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from tabswitcher.actions import activate_tab, open_settings, openFirstGoogleResult, searchGoogeInNewTab
 from tabswitcher.loadBookmarks import load_bookmarks
 from tabswitcher.shortcuts import setup_shortcuts
 
 from .SearchInput import SearchInput
 from .Settings import Settings
 from .TabList import TabList
-from .brotab import delete_tab, get_tabs, seach_tab
+from .brotab import delete_tab, get_tabs, print_recent_tabs, seach_tab
 from .colors import getBackgroundColor, getPlaceholderColor, getWindowBackgroundColor
 from .fuzzySearch import fuzzy_search_cmd, fuzzy_search_py
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 settings = Settings()
 
 config_dir = os.path.expanduser('~/.tabswitcher')
@@ -292,35 +292,14 @@
         elif input_text.startswith("#"):
             self.info_label.setText("No bookmarks found.")
         else:
             self.info_label.setText("No matches found.")
 
         self.info_label.show()
         self.list.hide()
-        
-
-
-def print_recent_tabs(index):
-    try:
-        with open(tab_history_path, 'rb') as f:
-            tab_ids = pickle.load(f)
-            if index:
-                print(tab_ids[int(index)])
-                exit(0)
-            for tab_id in tab_ids:
-                print(tab_id)
-            exit(0)
-            
-    except FileNotFoundError:
-        print("File not found: " + tab_history_path, file=sys.stderr)
-        exit(1)
-    except ValueError:
-        print("Invalid index: " + index, file=sys.stderr)
-        exit(1)
-    
 
 
 def open_tabswitcher():
     app = QApplication(sys.argv)
     window = MainWindow()
     window.show()
     window.activateWindow()
```

### Comparing `tabswitcher-0.1.5/src/tabswitcher/actions.py` & `tabswitcher-0.1.7/src/tabswitcher/actions.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/src/tabswitcher/assets/Icon.ico` & `tabswitcher-0.1.7/src/tabswitcher/assets/Icon.ico`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/src/tabswitcher/assets/install.bat` & `tabswitcher-0.1.7/src/tabswitcher/assets/install.bat`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/src/tabswitcher/assets/sans.ttf` & `tabswitcher-0.1.7/src/tabswitcher/assets/sans.ttf`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/src/tabswitcher/assets/tabswitcher_service.xml` & `tabswitcher-0.1.7/src/tabswitcher/assets/tabswitcher_service.xml`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/src/tabswitcher/brotab.py` & `tabswitcher-0.1.7/src/tabswitcher/brotab.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 import os
 import pickle
 import subprocess
+import sys
 import chardet
 
 from PyQt5.QtCore import Qt
 from PyQt5.QtGui import QGuiApplication
 
 from tabswitcher.focusWindow import focus_window
 
@@ -50,34 +51,42 @@
             tab = Tab(id, title, url, manager)
             tabs[title] = tab
         
         return tabs
     except:
         return {}
 
-def switch_tab(tab_id, tab_title=None):
+def activate_tab(tab_id, focus):
     url = get_url()
 
+    command = ['bt']
+
+    if url is not None:
+        command.append('--target')
+        command.append(url)
+
+    command.append('activate')
+    command.append(tab_id)
+
+    if focus:
+        command.append('--focused')
+
+    subprocess.call(command)
+
+def switch_tab(tab_id, tab_title=None):
+    
+
     app = QGuiApplication.instance()
     modifiers = app.queryKeyboardModifiers()
 
-    if modifiers & Qt.ShiftModifier:
-        if url is None:
-            subprocess.call(['bt', 'activate', tab_id, '--focused'])
-        else:
-            subprocess.call(['bt', '--target', url, 'activate', tab_id, '--focused'])
-        if tab_title is not None:
-            print("FOCUS THIS " + tab_title)
-            focus_window(tab_title)
-
+    if modifiers & Qt.ShiftModifier and tab_title is not None:
+        activate_tab(tab_id, True)
+        focus_window(tab_title)
     else:
-        if url is None:
-            subprocess.call(['bt', 'activate', tab_id])
-        else:
-            subprocess.call(['bt', '--target', url, 'activate', tab_id])
+        activate_tab(tab_id, False)
 
 
 def delete_tab(tab_id):
     url = get_url()
     if url is None:
         subprocess.call(['bt', 'close', tab_id])
     else:
@@ -126,8 +135,43 @@
             return None
         data = lines[0].split('\t')
         if (len(data) == 5):
             return data[0]
         return None
     except:
         return None
+    
+def get_recent_tabs(index=None):
+    try:
+        with open(tab_history_path, 'rb') as f:
+            tab_ids = pickle.load(f)
+            if index:
+                index = int(index)
+                if index < len(tab_ids):
+                    return tab_ids[index]
+                else:
+                    return None
+            return tab_ids
+            
+    except FileNotFoundError:
+        print("File not found: " + tab_history_path, file=sys.stderr)
+        exit(1)
+    except ValueError:
+        print("Invalid index: " + index, file=sys.stderr)
+        exit(1)
+
+def print_recent_tabs(index=None):
+    try:
+        tabs = get_recent_tabs(index)
+        if isinstance(tabs, list):
+            for tab in tabs:
+                print(tab)
+        else:
+            print(tabs)
+            
+    except FileNotFoundError:
+        print("File not found: " + tab_history_path, file=sys.stderr)
+        exit(1)
+    except ValueError:
+        print("Invalid index: " + index, file=sys.stderr)
+        exit(1)
```

### Comparing `tabswitcher-0.1.5/src/tabswitcher/colors.py` & `tabswitcher-0.1.7/src/tabswitcher/colors.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/src/tabswitcher/focusWindow.py` & `tabswitcher-0.1.7/src/tabswitcher/focusWindow.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/src/tabswitcher/fuzzySearch.py` & `tabswitcher-0.1.7/src/tabswitcher/fuzzySearch.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/src/tabswitcher/loadBookmarks.py` & `tabswitcher-0.1.7/src/tabswitcher/loadBookmarks.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/src/tabswitcher/shortcuts.py` & `tabswitcher-0.1.7/src/tabswitcher/shortcuts.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.5/tabswitcher.egg-info/PKG-INFO` & `tabswitcher-0.1.7/tabswitcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.1.5
+Version: 0.1.7
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
@@ -23,14 +23,15 @@
 Requires-Dist: psutil==5.9.4
 Requires-Dist: fuzzywuzzy
 Requires-Dist: PyQt5
 Requires-Dist: schedule
 Requires-Dist: brotab
 Requires-Dist: pynput; platform_system == "Windows"
 Requires-Dist: pywin32; platform_system == "Windows"
+Requires-Dist: keyboard; platform_system == "Windows"
 
 # TabSwitcher
 
 TabSwitcher is a simple window for switching between tabs in a browser. It uses the [brotab](https://github.com/balta2ar/brotab) CLI and browser extensions as a foundation.
 
 ## Requirements
```

### Comparing `tabswitcher-0.1.5/tabswitcher.egg-info/SOURCES.txt` & `tabswitcher-0.1.7/tabswitcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

