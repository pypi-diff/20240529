# Comparing `tmp/pgpyui-0.1.0.tar.gz` & `tmp/pgpyui-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgpyui-0.1.0.tar", last modified: Mon Apr 29 08:26:28 2024, max compression
+gzip compressed data, was "pgpyui-0.1.1.tar", last modified: Wed May 29 16:38:09 2024, max compression
```

## Comparing `pgpyui-0.1.0.tar` & `pgpyui-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 08:26:28.399788 pgpyui-0.1.0/
--rw-rw-rw-   0        0        0     4251 2024-04-29 08:26:28.398789 pgpyui-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3673 2024-04-29 08:24:38.000000 pgpyui-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 08:26:28.391792 pgpyui-0.1.0/pgpyui/
--rw-rw-rw-   0        0        0      149 2024-04-29 08:09:03.000000 pgpyui-0.1.0/pgpyui/__init__.py
--rw-rw-rw-   0        0        0     2379 2024-04-29 08:20:11.000000 pgpyui-0.1.0/pgpyui/button.py
--rw-rw-rw-   0        0        0     2451 2024-04-28 11:31:24.000000 pgpyui-0.1.0/pgpyui/checkbox.py
--rw-rw-rw-   0        0        0     2183 2024-04-28 12:59:30.000000 pgpyui-0.1.0/pgpyui/radio.py
--rw-rw-rw-   0        0        0     2608 2024-04-28 11:21:59.000000 pgpyui-0.1.0/pgpyui/slider.py
--rw-rw-rw-   0        0        0     6072 2024-04-28 11:21:52.000000 pgpyui-0.1.0/pgpyui/textarea.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:26:28.397789 pgpyui-0.1.0/pgpyui.egg-info/
--rw-rw-rw-   0        0        0     4251 2024-04-29 08:26:28.000000 pgpyui-0.1.0/pgpyui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-04-29 08:26:28.000000 pgpyui-0.1.0/pgpyui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 08:26:28.000000 pgpyui-0.1.0/pgpyui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-29 08:26:28.000000 pgpyui-0.1.0/pgpyui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-29 08:26:28.000000 pgpyui-0.1.0/pgpyui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 08:26:28.400789 pgpyui-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      822 2024-04-29 08:07:12.000000 pgpyui-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:38:09.325643 pgpyui-0.1.1/
+-rw-rw-rw-   0        0        0     4241 2024-05-29 16:38:09.325643 pgpyui-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3663 2024-05-29 15:50:09.000000 pgpyui-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 16:38:09.318643 pgpyui-0.1.1/pgpyui/
+-rw-rw-rw-   0        0        0      146 2024-05-29 16:22:07.000000 pgpyui-0.1.1/pgpyui/__init__.py
+-rw-rw-rw-   0        0        0     2379 2024-05-29 16:06:12.000000 pgpyui-0.1.1/pgpyui/button.py
+-rw-rw-rw-   0        0        0     2670 2024-05-29 16:00:18.000000 pgpyui-0.1.1/pgpyui/checkbox.py
+-rw-rw-rw-   0        0        0     2403 2024-05-29 16:00:21.000000 pgpyui-0.1.1/pgpyui/radio.py
+-rw-rw-rw-   0        0        0     2849 2024-05-29 16:01:50.000000 pgpyui-0.1.1/pgpyui/slider.py
+-rw-rw-rw-   0        0        0     5462 2024-05-29 16:06:01.000000 pgpyui-0.1.1/pgpyui/textarea.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:38:09.324643 pgpyui-0.1.1/pgpyui.egg-info/
+-rw-rw-rw-   0        0        0     4241 2024-05-29 16:38:09.000000 pgpyui-0.1.1/pgpyui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-05-29 16:38:09.000000 pgpyui-0.1.1/pgpyui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 16:38:09.000000 pgpyui-0.1.1/pgpyui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-29 16:38:09.000000 pgpyui-0.1.1/pgpyui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-29 16:38:09.000000 pgpyui-0.1.1/pgpyui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 16:38:09.326644 pgpyui-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      822 2024-05-29 16:37:40.000000 pgpyui-0.1.1/setup.py
```

### Comparing `pgpyui-0.1.0/PKG-INFO` & `pgpyui-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pgpyui
-Version: 0.1.0
+Version: 0.1.1
 Summary: The package is an add-on for Pygame to create a user interface on the screen.
 Home-page: https://pypi.org/project/pgpyui/
 Author: Memdved
 Author-email: mixail.vilyukov@icloud.com
 Project-URL: GitHub, https://github.com/Memdved
 Keywords: ui gui pgpyui pygame
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
 
-# pgpyui 0.1.0
+# pgpyui 0.1.1
 
 pgpyui is an add-on module for pygame to create a user interface.
 
 ## Installation
 
 ```
 pip install pgpyui
@@ -32,15 +32,15 @@
 ```python
 from pgpyui import button
 import pygame
 ```
 
 Creating a button
 ```python
-button = button.Button((100, 100), (200, 100), "Some text", lambda: func(), sprites=["sprites/sprite1.png", "sprites/sprite2.png"])
+button = button.Button((100, 100), (200, 100), "Some text", func, sprites=["sprites/sprite1.png", "sprites/sprite2.png"])
 ```
 
 Event handling
 ```python
 button.check_events(event)
 ```
```

### Comparing `pgpyui-0.1.0/README.md` & `pgpyui-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pgpyui 0.1.0
+# pgpyui 0.1.1
 
 pgpyui is an add-on module for pygame to create a user interface.
 
 ## Installation
 
 ```
 pip install pgpyui
@@ -16,15 +16,15 @@
 ```python
 from pgpyui import button
 import pygame
 ```
 
 Creating a button
 ```python
-button = button.Button((100, 100), (200, 100), "Some text", lambda: func(), sprites=["sprites/sprite1.png", "sprites/sprite2.png"])
+button = button.Button((100, 100), (200, 100), "Some text", func, sprites=["sprites/sprite1.png", "sprites/sprite2.png"])
 ```
 
 Event handling
 ```python
 button.check_events(event)
 ```
```

### Comparing `pgpyui-0.1.0/pgpyui/button.py` & `pgpyui-0.1.1/pgpyui/button.py`

 * *Files identical despite different names*

### Comparing `pgpyui-0.1.0/pgpyui/checkbox.py` & `pgpyui-0.1.1/pgpyui/checkbox.py`

 * *Files 23% similar despite different names*

```diff
@@ -32,28 +32,34 @@
 
         self.__bg_color: tuple[int, int, int] = color
 
         self.__text_surface: pygame.Surface = pygame.font.SysFont("Arial", size[1]).render(
             "√", True, color
         )
 
-    def check_events(self, event: pygame.event.Event):
+    def check_events(self, event: pygame.event.Event) -> None:
+        """
+        Method for checking events.
+        """
         if event.type == pygame.MOUSEBUTTONDOWN:
             if event.button == 1:
                 num_box = 0
                 for box in self.__boxes:
                     if box.collidepoint(pygame.mouse.get_pos()):
                         if self.__indx[num_box] == 0:
                             self.__indx[num_box] = 1
                         else:
                             self.__indx[num_box] = 0
                     
                     num_box += 1
 
     def draw(self, window) -> None:
+        """
+        Method for drawing checkbox.
+        """
         num_box = 0
         if self.__is_sprite:
             for box in self.__boxes:
                 window.blit(self.__sprites[self.__indx[num_box]], (box.x, box.y))
                 num_box += 1
         else:
             for box in self.__boxes:
@@ -65,8 +71,12 @@
                 )   
                 pygame.draw.rect(window, self.__bg_color, box, 2)
                 if self.__indx[num_box]:
                     window.blit(self.__text_surface, text_rectangle)
                 num_box += 1
 
     def data_return(self) -> list[int]:
+        """
+        Method to return list of push buttons.
+        """
+        
         return self.__indx
```

### Comparing `pgpyui-0.1.0/pgpyui/radio.py` & `pgpyui-0.1.1/pgpyui/radio.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,18 @@
 
         self.__radio_buttons: list = [Circle(radius, (position[0], position[1] + (count * step)), self.__bg_color) for count in range(num_rb)]
 
         self.__indx: list = [0 for _ in range(num_rb)]
 
         self.__bg_color: tuple[int, int, int] = color
 
-    def check_events(self, event: pygame.event.Event):
+    def check_events(self, event: pygame.event.Event) -> None:
+        """
+        Method for checking events.
+        """
         if event.type == pygame.MOUSEBUTTONDOWN:
             if event.button == 1:
                 num_radio = 0
                 for circle in self.__radio_buttons:
                     mouse_pos = pygame.mouse.get_pos()
 
                     circle_pos = circle.pos
@@ -55,20 +58,27 @@
                     if (delta_x ** 2 + delta_y ** 2) ** 0.5 <= circle.r:
                         self.__indx = [0 for _ in range(self.__num_rb)]
                         self.__indx[num_radio] = 1
 
                     num_radio += 1
 
     def draw(self, window) -> None:
+        """
+        Method for draw radio-button.
+        """
         num_radio = 0
         for rd_bt in self.__radio_buttons:
             rd_bt.show(window)
 
             if self.__indx[num_radio]:
                 rd_bt.push = True
             else:
                 rd_bt.push = False
 
             num_radio += 1
 
     def data_return(self) -> list[int]:
+        """
+        Method to return list of push buttons.
+        """
+        
         return self.__indx
```

### Comparing `pgpyui-0.1.0/pgpyui/slider.py` & `pgpyui-0.1.1/pgpyui/slider.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,39 +36,50 @@
             self.__finish = (self.__start[0] + len, self.__start[1])
         else:
             self.__line_pos = ((self.__rectangle.centerx, self.__rectangle.centery), (self.__rectangle.centerx, self.__rectangle.centery + self.__len))
             self.__line_rect = pygame.Rect(*position, size_block[0], self.__len)
             self.__finish = (self.__start[0], self.__start[1] + len)
         
     
-    def __move(self):
+    def __move(self) -> None:
         x, y = pygame.mouse.get_pos()
         if self.__is_push:
             if self.__line_rect.collidepoint(x, y):
                 if not self.__orientation:
                     self.__rectangle.x = x
                 else:
                     self.__rectangle.y = y
         
-    def draw(self, window):
+    def draw(self, window) -> None:
+        """
+        Method for drawing slider.
+        """
+        
         pygame.draw.line(window, (255, 255, 255), self.__line_pos[0], self.__line_pos[1], 5)
         pygame.draw.rect(window, (255, 255, 255), self.__rectangle)
             
 
-    def check_events(self, event: pygame.event.Event):
+    def check_events(self, event: pygame.event.Event) -> None:
+        """
+        Method for checking events.
+        """
         if event.type == pygame.MOUSEBUTTONDOWN:
             if event.button == 1:
                 self.__is_push = True
         if event.type == pygame.MOUSEBUTTONUP:
             if event.button == 1:
                 self.__is_push = False
         
         self.__move()
 
-    def data_return(self):
+    def data_return(self) -> int:
+        """
+        Method for return progress of slider.
+        """
+
         progress: int
         if not self.__orientation:
             progress = int(round(self.__rectangle.centerx / self.__finish[0], 2) * 100)
         else:
             progress = int(round(self.__rectangle.centery / self.__finish[1], 2) * 100)
 
         return progress
```

### Comparing `pgpyui-0.1.0/pgpyui.egg-info/PKG-INFO` & `pgpyui-0.1.1/pgpyui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pgpyui
-Version: 0.1.0
+Version: 0.1.1
 Summary: The package is an add-on for Pygame to create a user interface on the screen.
 Home-page: https://pypi.org/project/pgpyui/
 Author: Memdved
 Author-email: mixail.vilyukov@icloud.com
 Project-URL: GitHub, https://github.com/Memdved
 Keywords: ui gui pgpyui pygame
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
 
-# pgpyui 0.1.0
+# pgpyui 0.1.1
 
 pgpyui is an add-on module for pygame to create a user interface.
 
 ## Installation
 
 ```
 pip install pgpyui
@@ -32,15 +32,15 @@
 ```python
 from pgpyui import button
 import pygame
 ```
 
 Creating a button
 ```python
-button = button.Button((100, 100), (200, 100), "Some text", lambda: func(), sprites=["sprites/sprite1.png", "sprites/sprite2.png"])
+button = button.Button((100, 100), (200, 100), "Some text", func, sprites=["sprites/sprite1.png", "sprites/sprite2.png"])
 ```
 
 Event handling
 ```python
 button.check_events(event)
 ```
```

### Comparing `pgpyui-0.1.0/setup.py` & `pgpyui-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='pgpyui',
-  version='0.1.0',
+  version='0.1.1',
   author='Memdved',
   author_email='mixail.vilyukov@icloud.com',
   description='The package is an add-on for Pygame to create a user interface on the screen.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://pypi.org/project/pgpyui/',
   packages=find_packages(),
```

