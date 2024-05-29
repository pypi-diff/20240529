# Comparing `tmp/image_center-2024.5.24.tar.gz` & `tmp/image_center-2024.5.29.tar.gz`

## Comparing `image_center-2024.5.24.tar` & `image_center-2024.5.29.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    17398 2020-02-02 00:00:00.000000 image_center-2024.5.24/image_center/__init__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 image_center-2024.5.24/image_center/__version__.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 image_center-2024.5.24/image_center/conf.py
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 image_center-2024.5.24/image_center/server.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 image_center-2024.5.24/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 image_center-2024.5.24/LICENSE
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 image_center-2024.5.24/README.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 image_center-2024.5.24/pyproject.toml
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 image_center-2024.5.24/PKG-INFO
+-rw-r--r--   0        0        0    17548 2020-02-02 00:00:00.000000 image_center-2024.5.29/image_center/__init__.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 image_center-2024.5.29/image_center/__version__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 image_center-2024.5.29/image_center/conf.py
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 image_center-2024.5.29/image_center/server.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 image_center-2024.5.29/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 image_center-2024.5.29/LICENSE
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 image_center-2024.5.29/README.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 image_center-2024.5.29/pyproject.toml
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 image_center-2024.5.29/PKG-INFO
```

### Comparing `image_center-2024.5.24/image_center/__init__.py` & `image_center-2024.5.29/image_center/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     def __init__(self, *name):
         """
         通过模板资源未匹配到对应元素
         :param name: 命令
         """
         err = f"通过图片资源, 未在屏幕上匹配到元素"
-        template = [f"{i}.png" for i in name]
+        template = [f"{i}" for i in name]
         BaseException.__init__(self, err, *template)
 
 
 class TemplatePictureNotExist(BaseException):
     """图片资源，文件不存在"""
 
     def __init__(self, name):
@@ -91,23 +91,26 @@
             rate = float(setting.IMAGE_RATE)
         screen = setting.SCREEN_CACHE
 
         if not picture_abspath:
             if screen_bbox:
                 screen = cls.save_temporary_picture(*screen_bbox) + ".png"
             else:
-                if setting.IS_X11:
-                    try:
-                        pyscreenshot.grab().save(screen)
-                    except easyprocess.EasyProcessError:
-                        ...
-                elif setting.IS_WAYLAND:
-                    screen = os.popen(cls.wayland_screen_dbus).read().strip("\n")
+                if setting.IS_LINUX:
+                    if setting.IS_X11:
+                        try:
+                            pyscreenshot.grab().save(screen)
+                        except easyprocess.EasyProcessError:
+                            ...
+                    else:
+                        # setting.IS_WAYLAND
+                        screen = os.popen(cls.wayland_screen_dbus).read().strip("\n")
                 else:
-                    #for windows and macos
+                    # setting.IS_WINDOWS or setting.IS_MACOS:
+                    # for windows and macos
                     pyscreenshot.grab().save(screen)
 
         else:
             screen = picture_abspath
 
         # 如果传入的image_path参数不带文件后缀名，就根据文件类型判断文件是否存在，存在则将后缀类型（'.png','.jpg','.jpeg'）加上
         if not image_path.endswith(('.png', '.jpg', '.jpeg')):
```

### Comparing `image_center-2024.5.24/image_center/conf.py` & `image_center-2024.5.29/image_center/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,71 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
 
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 
 # SPDX-License-Identifier: Apache Software License
+import enum
 import os
 import platform
 import tempfile
+from os import popen
+
+
+@enum.unique
+class DisplayServer(enum.Enum):
+    wayland = "wayland"
+    x11 = "x11"
+
+
+@enum.unique
+class PlatForm(enum.Enum):
+    win = "Windows"
+    linux = "Linux"
+    macos = "Darwin"
+
 
 class _Setting:
-    PIC_PATH = ""
-    IMAGE_RATE = 0.9
-    SCREEN_CACHE = "/tmp/screen.png"
-    # Win default path——C:\\Users\\xxxx\\AppData\\Local\\Temp
-    # Linux_MacOS default path——/tmp/screen.png
-    SCREEN_CACHE = os.path.join(tempfile.gettempdir(), 'screen.png')  # /tmp/screen.png
-    TMPDIR = "/tmp/tmpdir"
-    # IMAGE_MATCH_NUMBER = 1
-    # IMAGE_MATCH_WAIT_TIME = 1
+    """配置模块"""
 
-    # RPC config
-    SERVER_IP = ""
+    SERVER_IP = "127.0.0.1"
     PORT = 8889
-    NETWORK_RETRY =1
+    NETWORK_RETRY = 1
     PAUSE = 1
     TIMEOUT = 5
     MAX_MATCH_NUMBER = 100
 
+    IS_LINUX = False
+    IS_WINDOWS = False
+    IS_MACOS = False
 
+    PIC_PATH = ""
+    IMAGE_RATE = 0.9
+    # Win default path——C:\\Users\\xxxx\\AppData\\Local\\Temp
+    # Linux_MacOS default path——/tmp/screen.png
+    SCREEN_CACHE = os.path.join(tempfile.gettempdir(), 'screen.png')
+    TMPDIR = os.path.join(tempfile.gettempdir(), 'tmpdir')
+    # IMAGE_MATCH_NUMBER = 1
+    # IMAGE_MATCH_WAIT_TIME = 1
 
-    if platform.system() == "Linux":
+    if platform.system() == PlatForm.win.value:
+        # windows
+        IS_WINDOWS = True
+    elif platform.system() == PlatForm.macos.value:
+        # MacOS
+        IS_MACOS = True
+    elif platform.system() == PlatForm.linux.value:
+        # Linux
+        IS_LINUX = True
         # 显示服务器
-        DISPLAY_SERVER = os.popen(
-            "cat ~/.xsession-errors | grep XDG_SESSION_TYPE | head -n 1"
-        ).read().split("=")[-1].strip("\n")
-
-        class DisplayServer:
-            wayland = "wayland"
-            x11 = "x11"
-
-        IS_X11 = (DISPLAY_SERVER == DisplayServer.x11)
-        IS_WAYLAND = (DISPLAY_SERVER == DisplayServer.wayland)
-    elif platform.system() == "Darwin":
-        IS_X11 = False
-        IS_WAYLAND = False
-    elif platform.system() == "Windows":
-        IS_X11 = False
-        IS_WAYLAND = False
+        DISPLAY_SERVER = (
+                             popen("cat ~/.xsession-errors | grep XDG_SESSION_TYPE | head -n 1")
+                             .read()
+                             .split("=")[-1]
+                             .strip("\n")
+                         ) or ("x11" if popen("ps -ef | grep -v grep | grep kwin_x11").read() else "wayland")
+
+        IS_X11 = DISPLAY_SERVER == DisplayServer.x11.value
+        IS_WAYLAND = DISPLAY_SERVER == DisplayServer.wayland.value
+
 
 setting = _Setting()
```

### Comparing `image_center-2024.5.24/image_center/server.py` & `image_center-2024.5.29/image_center/server.py`

 * *Files identical despite different names*

### Comparing `image_center-2024.5.24/.gitignore` & `image_center-2024.5.29/.gitignore`

 * *Files identical despite different names*

### Comparing `image_center-2024.5.24/LICENSE` & `image_center-2024.5.29/LICENSE`

 * *Files identical despite different names*

### Comparing `image_center-2024.5.24/README.md` & `image_center-2024.5.29/README.md`

 * *Files identical despite different names*

### Comparing `image_center-2024.5.24/pyproject.toml` & `image_center-2024.5.29/pyproject.toml`

 * *Files identical despite different names*

### Comparing `image_center-2024.5.24/PKG-INFO` & `image_center-2024.5.29/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-center
-Version: 2024.5.24
+Version: 2024.5.29
 Summary: image-center
 Project-URL: Source, https://github.com/linuxdeepin/image-center
 Project-URL: Documentation, https://linuxdeepin.github.io/image-center
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: image-center Version: 2024.5.24 Summary: image-
+Metadata-Version: 2.1 Name: image-center Version: 2024.5.29 Summary: image-
 center Project-URL: Source, https://github.com/linuxdeepin/image-center
 Project-URL: Documentation, https://linuxdeepin.github.io/image-center Author-
 email: mikigo <1964191531@qq.com> License-File: LICENSE Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Requires-Python:
 >=3.6 Requires-Dist: pillow Requires-Dist: pyscreenshot Provides-Extra: doc
 Requires-Dist: mkdocs-material; extra == 'doc' Provides-Extra: test Requires-
```

