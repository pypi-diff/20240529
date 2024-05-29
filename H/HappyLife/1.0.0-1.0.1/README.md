# Comparing `tmp/happylife-1.0.0.tar.gz` & `tmp/happylife-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happylife-1.0.0.tar", last modified: Tue May 28 04:10:38 2024, max compression
+gzip compressed data, was "happylife-1.0.1.tar", last modified: Tue May 28 07:47:30 2024, max compression
```

## Comparing `happylife-1.0.0.tar` & `happylife-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 04:10:38.929414 happylife-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-28 04:10:38.929414 happylife-1.0.0/HappyLife.egg-info/
--rw-rw-rw-   0        0        0      376 2024-05-28 04:10:38.000000 happylife-1.0.0/HappyLife.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-05-28 04:10:38.000000 happylife-1.0.0/HappyLife.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 04:10:38.000000 happylife-1.0.0/HappyLife.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-28 04:10:38.000000 happylife-1.0.0/HappyLife.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       65 2024-05-28 04:10:38.000000 happylife-1.0.0/HappyLife.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-28 04:10:38.000000 happylife-1.0.0/HappyLife.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      376 2024-05-28 04:10:38.929414 happylife-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-28 04:10:38.929414 happylife-1.0.0/auto/
--rw-rw-rw-   0        0        0    29543 2024-05-28 03:39:48.000000 happylife-1.0.0/auto/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-28 04:10:38.929414 happylife-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      888 2024-05-28 04:09:27.000000 happylife-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:47:30.080402 happylife-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-05-28 07:47:30.079429 happylife-1.0.1/HappyLife.egg-info/
+-rw-rw-rw-   0        0        0     2246 2024-05-28 07:47:30.000000 happylife-1.0.1/HappyLife.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-05-28 07:47:30.000000 happylife-1.0.1/HappyLife.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 07:47:30.000000 happylife-1.0.1/HappyLife.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-28 07:47:30.000000 happylife-1.0.1/HappyLife.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       66 2024-05-28 07:47:30.000000 happylife-1.0.1/HappyLife.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-28 07:47:30.000000 happylife-1.0.1/HappyLife.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2246 2024-05-28 07:47:30.080402 happylife-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1767 2024-05-28 07:24:25.000000 happylife-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 07:47:30.078454 happylife-1.0.1/auto/
+-rw-rw-rw-   0        0        0    29674 2024-05-28 07:47:01.000000 happylife-1.0.1/auto/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-28 07:47:30.080402 happylife-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-28 07:44:37.000000 happylife-1.0.1/setup.py
```

### Comparing `happylife-1.0.0/auto/__init__.py` & `happylife-1.0.1/auto/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 from PIL import ImageGrab
 from PIL import Image
 from contextlib import contextmanager
 from ctypes import windll
 import collections, ctypes, sys, cv2, numpy, time, win32gui, win32ui, win32con, win32api, win32print
 
 def get_scaling():
@@ -41,18 +41,19 @@
         self.hwnd = hwnd_child_list[child_list_number]
 
     def window_locate(self):
         '''窗口定位,返回窗口左上角和右下角的坐標'''
         self.left, self.top, self.right, self.bottom = win32gui.GetWindowRect(self.hwnd)
         return self.left, self.top, self.right, self.bottom
         
-    def lclick(self,x,y):
+    def lclick(self,x,y,second=0.1):
         '''後臺滑鼠左鍵單擊指定座標,lclick(55,110)'''
-        self.x = x; self.y = y
+        self.x = x; self.y = y; self.second = second
         win32api.SendMessage(self.hwnd, win32con.WM_LBUTTONDOWN, 1, ((int(self.y/self.display_zoom)) << 16 | (int(self.x//self.display_zoom))))
+        time.sleep(self.second)
         win32api.SendMessage(self.hwnd, win32con.WM_LBUTTONUP, 0, ((int(self.y/self.display_zoom)) << 16 | (int(self.x//self.display_zoom))))
 
     def lclick2(self,x,y):
         '''後臺滑鼠左鍵雙擊指定座標,lclick2(55,110)'''
         self.x = x; self.y = y
         win32api.SendMessage(self.hwnd, win32con.WM_LBUTTONDOWN, 1, ((self.y) << 16 | (self.x)))
         win32api.SendMessage(self.hwnd, win32con.WM_LBUTTONUP, 0, ((self.y) << 16 | (self.x)))
@@ -253,28 +254,30 @@
         #cv2.waitKey()
         #cv2.destroyAllWindows()
 
     def img_click(self,bind,img,wait=0.3,grayscale=True,confidence=0.9):
         '''
         後臺點擊匹配到的圖片,
         img_click(圖片,點擊後等待X秒,是否使用灰階,相似度)
-        img_click('1.png',0.5,True,0.9)
+        bw = Bw('夜神模擬器')
+        img_click(bw,'1.png')
         '''
         search_img = img_center_point2(img, bind, confidence=confidence, grayscale=grayscale)
         if search_img:
             x,y = img_center_point2(img, bind, confidence=confidence, grayscale=grayscale)
             self.x = x; self.y = y
             win32api.SendMessage(self.hwnd, win32con.WM_LBUTTONDOWN, 1, ((int(self.y/self.display_zoom)) << 16 | (int(self.x//self.display_zoom))))
             win32api.SendMessage(self.hwnd, win32con.WM_LBUTTONUP, 0, ((int(self.y/self.display_zoom)) << 16 | (int(self.x//self.display_zoom))))
             time.sleep(wait)
 
     def img_drag(self, bind, img, img2, delay=0.3, grayscale=True):
         '''
         拖拽圖片,滑鼠從圖片1座標拖拽到圖片2座標
-        img_drag('1.png','2.png')
+        bw = Bw('夜神模擬器')
+        img_drag(bw,'1.png','2.png')
         '''
         search_img = img_center_point2(img, bind, confidence=0.9, grayscale=grayscale)
         if search_img:
             x,y = img_center_point2(img, bind, confidence=0.9, grayscale=grayscale)
             x2,y2 = img_center_point2(img2, bind, confidence=0.9, grayscale=grayscale)
             self.x = x; self.y = y
             self.x2 = x2; self.y2 = y2
```

