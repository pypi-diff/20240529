# Comparing `tmp/xenoslib-0.1.29.7.tar.gz` & `tmp/xenoslib-0.1.29.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.29.7.tar", last modified: Wed Jan 10 05:39:42 2024, max compression
+gzip compressed data, was "xenoslib-0.1.29.8.tar", last modified: Wed May 29 05:47:55 2024, max compression
```

## Comparing `xenoslib-0.1.29.7.tar` & `xenoslib-0.1.29.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 05:39:42.644944 xenoslib-0.1.29.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-10 05:39:42.644944 xenoslib-0.1.29.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-10 05:39:42.644944 xenoslib-0.1.29.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 05:39:42.644944 xenoslib-0.1.29.7/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-01-10 05:39:34.000000 xenoslib-0.1.29.7/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 05:39:42.644944 xenoslib-0.1.29.7/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-10 05:39:42.000000 xenoslib-0.1.29.7/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-01-10 05:39:42.000000 xenoslib-0.1.29.7/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 05:39:42.000000 xenoslib-0.1.29.7/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-10 05:39:42.000000 xenoslib-0.1.29.7/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-10 05:39:42.000000 xenoslib-0.1.29.7/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:47:55.147463 xenoslib-0.1.29.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-29 05:47:55.147463 xenoslib-0.1.29.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 05:47:55.147463 xenoslib-0.1.29.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:47:55.143463 xenoslib-0.1.29.8/xenoslib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      310 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/xenoslib/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-29 05:47:49.000000 xenoslib-0.1.29.8/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:47:55.147463 xenoslib-0.1.29.8/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-29 05:47:55.000000 xenoslib-0.1.29.8/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-29 05:47:55.000000 xenoslib-0.1.29.8/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 05:47:55.000000 xenoslib-0.1.29.8/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-29 05:47:55.000000 xenoslib-0.1.29.8/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 05:47:55.000000 xenoslib-0.1.29.8/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.29.7/LICENSE` & `xenoslib-0.1.29.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.7/PKG-INFO` & `xenoslib-0.1.29.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenoslib
-Version: 0.1.29.7
+Version: 0.1.29.8
 Summary: Xenos' common lib
 Home-page: https://github.com/XenosLu/xenoslib.git
 Author: Xenocider
 Author-email: xenos.lu@gmail.com
 License: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `xenoslib-0.1.29.7/README.md` & `xenoslib-0.1.29.8/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.7/setup.py` & `xenoslib-0.1.29.8/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.7/xenoslib/base.py` & `xenoslib-0.1.29.8/xenoslib/base.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.7/xenoslib/dev.py` & `xenoslib-0.1.29.8/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.7/xenoslib/extend.py` & `xenoslib-0.1.29.8/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.7/xenoslib/linux.py` & `xenoslib-0.1.29.8/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.7/xenoslib/mail.py` & `xenoslib-0.1.29.8/xenoslib/mail.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.7/xenoslib/mock.py` & `xenoslib-0.1.29.8/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.7/xenoslib/onedrive.py` & `xenoslib-0.1.29.8/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.7/xenoslib/win_trayicon.py` & `xenoslib-0.1.29.8/xenoslib/win_trayicon.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,31 +81,32 @@
 class MenuItemConsole(MenuItem):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.hconsole = win32console.GetConsoleWindow()
 
     def is_window_visible_not_minimized(self):
         """返回窗口是否可见且不处于最小化状态"""
-        # 判断窗口是否可见
         visible = win32gui.IsWindowVisible(self.hconsole)
-        # 判断窗口是否最小化
         minimized = win32gui.IsIconic(self.hconsole)
+        logger.debug(f"window visible: {visible}, window minimized: {minimized}")
         return visible and not minimized
 
     def action(self, show=None):
         if show is None:
-            # super().action()'
+            # super().action()
             self.checked = not self.is_window_visible_not_minimized()
             # logger.info(self.checked)
         else:
             self.checked = show
         win32gui.ShowWindow(self.hconsole, self.checked)
         if self.checked:
             try:
+                # win32gui.BringWindowToTop(self.hconsole)
                 win32gui.SetForegroundWindow(self.hconsole)
+                # ctypes.windll.user32.SetForegroundWindow(self.hconsole)
             except Exception as exc:
                 logger.debug(exc, exc_info=True)
 
     def remove_close_button_from_console(self):
         hmenu = win32gui.GetSystemMenu(self.hconsole, 0)
         if hmenu:
             win32gui.DeleteMenu(hmenu, win32con.SC_CLOSE, win32con.MF_BYCOMMAND)
@@ -117,15 +118,15 @@
     FIRST_ID = 1023
     WINDOW_CLASS_NAME = "PySysTrayIcon"
 
     def init_icon(self, iconpath=None):
         if not iconpath:
             python_path = os.path.dirname(os.path.abspath(sys.executable))
             iconpath = os.path.join(python_path, "DLLs", "pyd.ico")
-            logger.debug(iconpath)
+            logger.debug(f"Load icon from path: {iconpath}")
         if os.path.isfile(iconpath):
             hinst = win32gui.GetModuleHandle(None)
             icon_flags = win32con.LR_LOADFROMFILE | win32con.LR_DEFAULTSIZE
             hicon = win32gui.LoadImage(hinst, iconpath, win32con.IMAGE_ICON, 0, 0, icon_flags)
         else:
             logger.warning("Can't find icon file - using default.")
             hicon = win32gui.LoadIcon(0, win32con.IDI_APPLICATION)
```

### Comparing `xenoslib-0.1.29.7/xenoslib/windows.py` & `xenoslib-0.1.29.8/xenoslib/windows.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.7/xenoslib.egg-info/PKG-INFO` & `xenoslib-0.1.29.8/xenoslib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenoslib
-Version: 0.1.29.7
+Version: 0.1.29.8
 Summary: Xenos' common lib
 Home-page: https://github.com/XenosLu/xenoslib.git
 Author: Xenocider
 Author-email: xenos.lu@gmail.com
 License: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

