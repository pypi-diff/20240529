# Comparing `tmp/happylife-1.0.1.tar.gz` & `tmp/happylife-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happylife-1.0.1.tar", last modified: Tue May 28 07:47:30 2024, max compression
+gzip compressed data, was "happylife-1.1.0.tar", last modified: Wed May 29 04:07:26 2024, max compression
```

## Comparing `happylife-1.0.1.tar` & `happylife-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 07:47:30.080402 happylife-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-28 07:47:30.079429 happylife-1.0.1/HappyLife.egg-info/
--rw-rw-rw-   0        0        0     2246 2024-05-28 07:47:30.000000 happylife-1.0.1/HappyLife.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-05-28 07:47:30.000000 happylife-1.0.1/HappyLife.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 07:47:30.000000 happylife-1.0.1/HappyLife.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-28 07:47:30.000000 happylife-1.0.1/HappyLife.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       66 2024-05-28 07:47:30.000000 happylife-1.0.1/HappyLife.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-28 07:47:30.000000 happylife-1.0.1/HappyLife.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2246 2024-05-28 07:47:30.080402 happylife-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1767 2024-05-28 07:24:25.000000 happylife-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 07:47:30.078454 happylife-1.0.1/auto/
--rw-rw-rw-   0        0        0    29674 2024-05-28 07:47:01.000000 happylife-1.0.1/auto/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-28 07:47:30.080402 happylife-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-28 07:44:37.000000 happylife-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:07:26.771318 happylife-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-29 04:07:26.770344 happylife-1.1.0/HappyLife.egg-info/
+-rw-rw-rw-   0        0        0     2838 2024-05-29 04:07:26.000000 happylife-1.1.0/HappyLife.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-05-29 04:07:26.000000 happylife-1.1.0/HappyLife.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 04:07:26.000000 happylife-1.1.0/HappyLife.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-29 04:07:26.000000 happylife-1.1.0/HappyLife.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       66 2024-05-29 04:07:26.000000 happylife-1.1.0/HappyLife.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-29 04:07:26.000000 happylife-1.1.0/HappyLife.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2838 2024-05-29 04:07:26.771318 happylife-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2346 2024-05-29 04:01:04.000000 happylife-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 04:07:26.769370 happylife-1.1.0/auto/
+-rw-rw-rw-   0        0        0    30806 2024-05-29 03:55:45.000000 happylife-1.1.0/auto/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 04:07:26.771318 happylife-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-28 07:44:37.000000 happylife-1.1.0/setup.py
```

### Comparing `happylife-1.0.1/auto/__init__.py` & `happylife-1.1.0/auto/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0.1'
+__version__ = '1.1.0'
 from PIL import ImageGrab
 from PIL import Image
 from contextlib import contextmanager
 from ctypes import windll
 import collections, ctypes, sys, cv2, numpy, time, win32gui, win32ui, win32con, win32api, win32print
 
 def get_scaling():
@@ -257,34 +257,42 @@
     def img_click(self,bind,img,wait=0.3,grayscale=True,confidence=0.9):
         '''
         後臺點擊匹配到的圖片,
         img_click(圖片,點擊後等待X秒,是否使用灰階,相似度)
         bw = Bw('夜神模擬器')
         img_click(bw,'1.png')
         '''
-        search_img = img_center_point2(img, bind, confidence=confidence, grayscale=grayscale)
-        if search_img:
-            x,y = img_center_point2(img, bind, confidence=confidence, grayscale=grayscale)
-            self.x = x; self.y = y
-            win32api.SendMessage(self.hwnd, win32con.WM_LBUTTONDOWN, 1, ((int(self.y/self.display_zoom)) << 16 | (int(self.x//self.display_zoom))))
-            win32api.SendMessage(self.hwnd, win32con.WM_LBUTTONUP, 0, ((int(self.y/self.display_zoom)) << 16 | (int(self.x//self.display_zoom))))
-            time.sleep(wait)
-
+        try:
+            print(f"嘗試點擊圖像: {img}")
+            search_img = img_center_point2(img, bind, confidence=confidence, grayscale=grayscale)
+            if search_img:
+                x,y = search_img
+                self.x = x; self.y = y
+                time.sleep(wait)
+                win32api.SendMessage(self.hwnd, win32con.WM_LBUTTONDOWN, 1, ((int(self.y/self.display_zoom)) << 16 | (int(self.x//self.display_zoom))))
+                win32api.SendMessage(self.hwnd, win32con.WM_LBUTTONUP, 0, ((int(self.y/self.display_zoom)) << 16 | (int(self.x//self.display_zoom))))
+                print(f"點擊位置: ({x}, {y})")
+                return True
+        except ImageNotFoundException as e:
+            print(f"未找到圖像: {img}. 錯誤: {e}")
+        return False
+    
     def img_drag(self, bind, img, img2, delay=0.3, grayscale=True):
         '''
         拖拽圖片,滑鼠從圖片1座標拖拽到圖片2座標
         bw = Bw('夜神模擬器')
         img_drag(bw,'1.png','2.png')
         '''
         search_img = img_center_point2(img, bind, confidence=0.9, grayscale=grayscale)
         if search_img:
             x,y = img_center_point2(img, bind, confidence=0.9, grayscale=grayscale)
             x2,y2 = img_center_point2(img2, bind, confidence=0.9, grayscale=grayscale)
             self.x = x; self.y = y
             self.x2 = x2; self.y2 = y2
+            time.sleep(0.3)
             win32api.SendMessage(self.hwnd, win32con.WM_LBUTTONDOWN, 1, ((int(self.y/self.display_zoom)) << 16 | (int(self.x//self.display_zoom))))
             time.sleep(delay)
             win32api.SendMessage(self.hwnd, win32con.WM_LBUTTONUP, 0, ((int(self.y2/self.display_zoom)) << 16 | (int(self.x2//self.display_zoom))))
 
 
 # 前臺操作        
 class Fd:
@@ -421,38 +429,61 @@
 
     def img_click(img, wait=0.3,grayscale=True):
         '''
         前臺點擊匹配到的圖片,
         img_click(圖片,點擊後等待X秒,是否使用灰階)
         img_click('1.png',0.5,True)
         '''
-        search_img = img_center_point(img, confidence=0.9, grayscale=grayscale)
-        if search_img:
-            x,y = img_center_point(img, confidence=0.9, grayscale=grayscale)
-            win32api.SetCursorPos([x,y])
-            win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP | win32con.MOUSEEVENTF_LEFTDOWN, 0, 0, 0, 0)
-            time.sleep(wait)
+        try:
+            print(f"嘗試點擊圖像: {img}")
+            search_img = img_center_point(img, confidence=0.9, grayscale=grayscale)
+            if search_img:
+                x,y = search_img
+                time.sleep(wait)
+                win32api.SetCursorPos([x,y])
+                win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP | win32con.MOUSEEVENTF_LEFTDOWN, 0, 0, 0, 0)
+                print(f"點擊位置: ({x}, {y})")
+                return True
+        except ImageNotFoundException as e:
+            print(f"未找到圖像: {img}. 錯誤: {e}")
+        return False
     
     def img_drag(img, img2, delay=0.3, grayscale=True):
         '''
         拖拽圖片,滑鼠從圖片1座標拖拽到圖片2座標
         img_drag('1.png','2.png')
         '''
         search_img = img_center_point(img, confidence=0.9, grayscale=grayscale)
         if search_img:
             x,y = img_center_point(img, confidence=0.9, grayscale=grayscale)
             x2,y2 = img_center_point(img2, confidence=0.9, grayscale=grayscale)
+            time.sleep(0.3)
             win32api.SetCursorPos([x,y])
             win32api.mouse_event(win32con.MOUSEEVENTF_LEFTDOWN, 0, 0, 0, 0)
             time.sleep(delay)
             win32api.SetCursorPos([x2,y2])
             time.sleep(delay)
             win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP, 0, 0, 0, 0)
 
-
+# 執行任務
+def perform_task(task_function, *args, **kwargs):
+    task_completed = False
+    while not task_completed:
+        print(f'執行任務 {task_function.__name__}')
+        if task_function(*args, **kwargs):
+            task_completed = True
+            print(f"任務 {task_function.__name__} 完成")
+        else:
+            print(f"任務 {task_function.__name__} 失敗，重試中...")
+            time.sleep(1)  # 等待一段時間後重試
+
+# 依序執行任務
+def execute_tasks_in_sequence(tasks):
+    for task in tasks:
+        perform_task(*task)
         
 # 圖色識別
 # 函式來自 pyscreeze , https://github.com/asweigart/pyscreeze
 
 unicode = str # 在 Python 3 上,所有 isinstance(spam, (str, unicode)) 調用都將與 Python 2 一樣工作
 USE_IMAGE_NOT_FOUND_EXCEPTION = False
 GRAYSCALE_DEFAULT = False
```

### Comparing `happylife-1.0.1/setup.py` & `happylife-1.1.0/setup.py`

 * *Files identical despite different names*

