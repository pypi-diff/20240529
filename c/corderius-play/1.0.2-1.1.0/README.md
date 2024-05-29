# Comparing `tmp/corderius_play-1.0.2.tar.gz` & `tmp/corderius_play-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corderius_play-1.0.2.tar", last modified: Sat May 25 10:12:57 2024, max compression
+gzip compressed data, was "corderius_play-1.1.0.tar", last modified: Wed May 29 10:46:24 2024, max compression
```

## Comparing `corderius_play-1.0.2.tar` & `corderius_play-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:12:57.237918 corderius_play-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-25 10:12:53.000000 corderius_play-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-25 10:12:53.000000 corderius_play-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    30827 2024-05-25 10:12:57.233918 corderius_play-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30269 2024-05-25 10:12:53.000000 corderius_play-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:12:57.233918 corderius_play-1.0.2/corderius_play.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    30827 2024-05-25 10:12:57.000000 corderius_play-1.0.2/corderius_play.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-25 10:12:57.000000 corderius_play-1.0.2/corderius_play.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 10:12:57.000000 corderius_play-1.0.2/corderius_play.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-25 10:12:57.000000 corderius_play-1.0.2/corderius_play.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-25 10:12:57.000000 corderius_play-1.0.2/corderius_play.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    76062 2024-05-25 10:12:53.000000 corderius_play-1.0.2/example.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:12:57.233918 corderius_play-1.0.2/play/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/all_sprites.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/async_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/blank_image.png
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/clamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/color.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:12:57.233918 corderius_play-1.0.2/play/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/keypress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:12:57.233918 corderius_play-1.0.2/play/objects/
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/objects/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/objects/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (127)    11459 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/objects/sprite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/objects/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:12:57.233918 corderius_play-1.0.2/play/physics/
--rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18690 2024-05-25 10:12:53.000000 corderius_play-1.0.2/play/play.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-25 10:12:53.000000 corderius_play-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 10:12:57.237918 corderius_play-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-25 10:12:53.000000 corderius_play-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:46:24.443354 corderius_play-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-29 10:46:20.000000 corderius_play-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-29 10:46:20.000000 corderius_play-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    30827 2024-05-29 10:46:24.443354 corderius_play-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30269 2024-05-29 10:46:20.000000 corderius_play-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:46:24.443354 corderius_play-1.1.0/corderius_play.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30827 2024-05-29 10:46:24.000000 corderius_play-1.1.0/corderius_play.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-29 10:46:24.000000 corderius_play-1.1.0/corderius_play.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:46:24.000000 corderius_play-1.1.0/corderius_play.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-29 10:46:24.000000 corderius_play-1.1.0/corderius_play.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 10:46:24.000000 corderius_play-1.1.0/corderius_play.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76062 2024-05-29 10:46:20.000000 corderius_play-1.1.0/example.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:46:24.439354 corderius_play-1.1.0/play/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/all_sprites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/async_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/blank_image.png
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/clamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:46:24.443354 corderius_play-1.1.0/play/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/keypress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:46:24.443354 corderius_play-1.1.0/play/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/objects/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/objects/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/objects/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/objects/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:46:24.443354 corderius_play-1.1.0/play/physics/
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-29 10:46:20.000000 corderius_play-1.1.0/play/play.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-29 10:46:20.000000 corderius_play-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-29 10:46:20.000000 corderius_play-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:46:24.443354 corderius_play-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-29 10:46:20.000000 corderius_play-1.1.0/setup.py
```

### Comparing `corderius_play-1.0.2/LICENSE` & `corderius_play-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corderius_play-1.0.2/PKG-INFO` & `corderius_play-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corderius-play
-Version: 1.0.2
+Version: 1.1.0
 Summary: The easiest way to make games and media projects in Python.
 Home-page: https://github.com/Corderius-College-Amersfoort/play
 Author: koen1711
 Author-email: koenvurk1711@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `corderius_play-1.0.2/README.md` & `corderius_play-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `corderius_play-1.0.2/corderius_play.egg-info/PKG-INFO` & `corderius_play-1.1.0/corderius_play.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corderius-play
-Version: 1.0.2
+Version: 1.1.0
 Summary: The easiest way to make games and media projects in Python.
 Home-page: https://github.com/Corderius-College-Amersfoort/play
 Author: koen1711
 Author-email: koenvurk1711@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `corderius_play-1.0.2/corderius_play.egg-info/SOURCES.txt` & `corderius_play-1.1.0/corderius_play.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 example.gif
+pyproject.toml
 requirements.txt
 setup.py
 corderius_play.egg-info/PKG-INFO
 corderius_play.egg-info/SOURCES.txt
 corderius_play.egg-info/dependency_links.txt
 corderius_play.egg-info/requires.txt
 corderius_play.egg-info/top_level.txt
```

### Comparing `corderius_play-1.0.2/example.gif` & `corderius_play-1.1.0/example.gif`

 * *Files identical despite different names*

### Comparing `corderius_play-1.0.2/play/async_helpers.py` & `corderius_play-1.1.0/play/async_helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,38 @@
+"""This module contains code to help with async functions."""
+
 import asyncio as _asyncio
 import warnings as _warnings
 from .exceptions import Oops
 
+
 def _raise_on_await_warning(func):
     """
     If someone doesn't put 'await' before functions that require 'await'
     like play.timer() or play.animate(), raise an exception.
     """
 
-    async def f(*args, **kwargs):
-        with _warnings.catch_warnings(record=True) as w:
+    async def raise_on_warning(*args, **kwargs):
+        with _warnings.catch_warnings(record=True) as warnings:
             await func(*args, **kwargs)
-            for warning in w:
-                str_message = warning.message.args[0]  # e.g. "coroutine 'timer' was never awaited"
-                if 'was never awaited' in str_message:
+            for warning in warnings:
+                str_message = warning.message.args[
+                    0
+                ]  # e.g. "coroutine 'timer' was never awaited"
+                if "was never awaited" in str_message:
                     unawaited_function_name = str_message.split("'")[1]
+
                     raise Oops(
-                        f"""Looks like you forgot to put "await" before play.{unawaited_function_name} on line {warning.lineno} of file {warning.filename}.
-To fix this, just add the word 'await' before play.{unawaited_function_name} on line {warning.lineno} of file {warning.filename} in the function {func.__name__}.""")
-                else:
-                    print(warning.message)
+                        f"""Looks like you forgot to put "await" before play.{unawaited_function_name} on line {warning.lineno} of file {warning.filename}.""" + # pylint: disable=line-too-long
+"""To fix this, just add the word 'await' before play.{unawaited_function_name} on line {warning.lineno} of file {warning.filename} in the function {func.__name__}.""" # pylint: disable=line-too-long
+                        # pylint: enable=line-too-long
+                    )
+                print(warning.message)
 
-    return f
+    return raise_on_warning
 
 
 def _make_async(func):
     """
     Turn a non-async function into an async function.
     Used mainly in decorators like @repeat_forever.
     """
@@ -33,8 +40,8 @@
         # if it's already async just return it
         return _raise_on_await_warning(func)
 
     @_raise_on_await_warning
     async def async_func(*args, **kwargs):
         return func(*args, **kwargs)
 
-    return async_func
+    return async_func
```

### Comparing `corderius_play-1.0.2/play/blank_image.png` & `corderius_play-1.1.0/play/blank_image.png`

 * *Files identical despite different names*

### Comparing `corderius_play-1.0.2/play/objects/box.py` & `corderius_play-1.1.0/play/objects/box.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,29 @@
+"""This module contains the Box class, which represents a box in the game."""
+
 import pygame
 from .sprite import Sprite
 from ..all_sprites import all_sprites
 from ..color import color_name_to_rgb as _color_name_to_rgb
 
 
 class Box(Sprite):
-    def __init__(self, color='black', x=0, y=0, width=100, height=200, border_color='light blue', border_width=0,
-                 transparency=100, size=100, angle=0):
+    def __init__( # pylint: disable=too-many-arguments
+        self,
+        color="black",
+        x=0,
+        y=0,
+        width=100,
+        height=200,
+        border_color="light blue",
+        border_width=0,
+        transparency=100,
+        size=100,
+        angle=0,
+    ):
         super().__init__(x, y, size, angle, transparency)
         self._x = x
         self._y = y
         self._width = width
         self._height = height
         self._color = color
         self._border_color = border_color
@@ -26,23 +39,32 @@
         self._when_clicked_callbacks = []
 
         self._compute_primary_surface()
 
         all_sprites.append(self)
 
     def _compute_primary_surface(self):
-        self._primary_pygame_surface = pygame.Surface((self._width, self._height), pygame.SRCALPHA)
+        self._primary_pygame_surface = pygame.Surface(
+            (self._width, self._height), pygame.SRCALPHA # pylint: disable=no-member
+        )
 
         if self._border_width and self._border_color:
             # draw border rectangle
             self._primary_pygame_surface.fill(_color_name_to_rgb(self._border_color))
             # draw fill rectangle over border rectangle at the proper position
-            pygame.draw.rect(self._primary_pygame_surface, _color_name_to_rgb(self._color), (
-            self._border_width, self._border_width, self._width - 2 * self._border_width,
-            self._height - 2 * self.border_width))
+            pygame.draw.rect(
+                self._primary_pygame_surface,
+                _color_name_to_rgb(self._color),
+                (
+                    self._border_width,
+                    self._border_width,
+                    self._width - 2 * self._border_width,
+                    self._height - 2 * self.border_width,
+                ),
+            )
 
         else:
             self._primary_pygame_surface.fill(_color_name_to_rgb(self._color))
 
         self._should_recompute_primary_surface = False
         self._compute_secondary_surface(force=True)
 
@@ -93,15 +115,41 @@
 
     @border_width.setter
     def border_width(self, _border_width):
         self._border_width = _border_width
         self._should_recompute_primary_surface = True
 
     def clone(self):
-        return self.__class__(color=self.color, width=self.width, height=self.height, border_color=self.border_color,
-                              border_width=self.border_width, **self._common_properties())
-
-
-def new_box(color='black', x=0, y=0, width=100, height=200, border_color='light blue', border_width=0, angle=0,
-            transparency=100, size=100):
-    return Box(color=color, x=x, y=y, width=width, height=height, border_color=border_color, border_width=border_width,
-               angle=angle, transparency=transparency, size=size)
+        return self.__class__(
+            color=self.color,
+            width=self.width,
+            height=self.height,
+            border_color=self.border_color,
+            border_width=self.border_width,
+            **self._common_properties()
+        )
+
+
+def new_box( # pylint: disable=too-many-arguments
+    color="black",
+    x=0,
+    y=0,
+    width=100,
+    height=200,
+    border_color="light blue",
+    border_width=0,
+    angle=0,
+    transparency=100,
+    size=100,
+):
+    return Box(
+        color=color,
+        x=x,
+        y=y,
+        width=width,
+        height=height,
+        border_color=border_color,
+        border_width=border_width,
+        angle=angle,
+        transparency=transparency,
+        size=size,
+    )
```

### Comparing `corderius_play-1.0.2/play/objects/line.py` & `corderius_play-1.1.0/play/objects/line.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,42 @@
+"""This module contains the Line class, which is a subclass of Sprite. It is used to create lines in the game window."""
+
+import math as _math
+
 import pygame
 from .sprite import Sprite
 from ..all_sprites import all_sprites
-import math as _math
 
 
 class Line(Sprite):
-    def __init__(self, color='black', x=0, y=0, length=None, angle=None, thickness=1, x1=None, y1=None,
-                 transparency=100, size=100):
+    def __init__( # pylint: disable=too-many-arguments
+        self,
+        color="black",
+        x=0,
+        y=0,
+        length=None,
+        angle=None,
+        thickness=1,
+        x1=None,
+        y1=None,
+        transparency=100,
+        size=100,
+    ):
         super().__init__(x, y, size, angle, transparency)
         self._x = x
         self._y = y
         self._color = color
         self._thickness = thickness
 
         # can set either (length, angle) or (x1,y1), otherwise a default is used
-        if length != None and angle != None:
+        if length is not None and angle is not None:
             self._length = length
             self._angle = angle
             self._x1, self._y1 = self._calc_endpoint()
-        elif x1 != None and y1 != None:
+        elif x1 is not None and y1 is not None:
             self._x1 = x1
             self._y1 = y1
             self._length, self._angle = self._calc_length_angle()
         else:
             # default values
             self._length = length or 100
             self._angle = angle or 0
@@ -37,44 +51,44 @@
         self._when_clicked_callbacks = []
 
         self._compute_primary_surface()
 
         all_sprites.append(self)
 
     def clone(self):
-        return self.__class__(color=self.color, length=self.length, thickness=self.thickness,
-                              **self._common_properties())
+        return self.__class__(
+            color=self.color,
+            length=self.length,
+            thickness=self.thickness,
+            **self._common_properties()
+        )
 
     def _compute_primary_surface(self):
         # Make a surface that just contains the line and no white-space around the line.
         # If line isn't horizontal, this surface will be drawn rotated.
         width = self.length
         height = self.thickness + 1
 
-        self._primary_pygame_surface = pygame.Surface((width, height), pygame.SRCALPHA)
+        self._primary_pygame_surface = pygame.Surface((width, height), pygame.SRCALPHA) # pylint: disable=no-member
         # self._primary_pygame_surface.set_colorkey((255,255,255, 255)) # set background to transparent
 
-        # # @hack
-        # if self.thickness == 1:
-        #     pygame.draw.aaline(self._primary_pygame_surface, _color_name_to_rgb(self.color), (0,1), (width,1), True)
-        # else:
-        #     pygame.draw.line(self._primary_pygame_surface, _color_name_to_rgb(self.color), (0,_math.floor(height/2)), (width,_math.floor(height/2)), self.thickness)
-
         # line is actually drawn in _game_loop because coordinates work different
 
         self._should_recompute_primary_surface = False
         self._compute_secondary_surface(force=True)
 
     def _compute_secondary_surface(self, force=False):
-        self._secondary_pygame_surface = self._primary_pygame_surface.copy()
+        self._secondary_pygame_surface = self._primary_pygame_surface.copy() # pylint: disable=attribute-defined-outside-init
 
         if force or self._transparency != 100:
-            self._secondary_pygame_surface.set_alpha(round((self._transparency / 100.) * 255))
+            self._secondary_pygame_surface.set_alpha(
+                round((self._transparency / 100.0) * 255)
+            )
 
-        self._should_recompute_secondary_surface = False
+        self._should_recompute_secondary_surface = False # pylint: disable=attribute-defined-outside-init
 
     ##### color #####
     @property
     def color(self):
         return self._color
 
     @color.setter
@@ -90,15 +104,18 @@
     @thickness.setter
     def thickness(self, _thickness):
         self._thickness = _thickness
         self._should_recompute_primary_surface = True
 
     def _calc_endpoint(self):
         radians = _math.radians(self._angle)
-        return self._length * _math.cos(radians) + self.x, self._length * _math.sin(radians) + self.y
+        return (
+            self._length * _math.cos(radians) + self.x,
+            self._length * _math.sin(radians) + self.y,
+        )
 
     ##### length #####
     @property
     def length(self):
         return self._length
 
     @length.setter
@@ -120,15 +137,15 @@
             self.physics._pymunk_body.angle = _math.radians(_angle)
 
     def _calc_length_angle(self):
         dx = self.x1 - self.x
         dy = self.y1 - self.y
 
         # TODO: this doesn't work at all
-        return _math.sqrt(dx ** 2 + dy ** 2), _math.degrees(_math.atan2(dy, dx))
+        return _math.sqrt(dx**2 + dy**2), _math.degrees(_math.atan2(dy, dx))
 
     ##### x1 #####
     @property
     def x1(self):
         return self._x1
 
     @x1.setter
@@ -145,11 +162,31 @@
     @y1.setter
     def y1(self, _y1):
         self._angle = _y1
         self._length, self._angle = self._calc_length_angle()
         self._should_recompute_primary_surface = True
 
 
-def new_line(color='black', x=0, y=0, length=None, angle=None, thickness=1, x1=None, y1=None, transparency=100,
-             size=100):
-    return Line(color=color, x=x, y=y, length=length, angle=angle, thickness=thickness, x1=x1, y1=y1,
-                transparency=transparency, size=size)
+def new_line( # pylint: disable=too-many-arguments
+    color="black",
+    x=0,
+    y=0,
+    length=None,
+    angle=None,
+    thickness=1,
+    x1=None,
+    y1=None,
+    transparency=100,
+    size=100,
+):
+    return Line(
+        color=color,
+        x=x,
+        y=y,
+        length=length,
+        angle=angle,
+        thickness=thickness,
+        x1=x1,
+        y1=y1,
+        transparency=transparency,
+        size=size,
+    )
```

### Comparing `corderius_play-1.0.2/play/objects/sprite.py` & `corderius_play-1.1.0/play/objects/sprite.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,45 @@
-from ..all_sprites import all_sprites
-import pygame
-from ..exceptions import Oops, Hmm
-import os as _os
+"""This module contains the base sprite class for all objects in the game."""
+
 import math as _math
+import warnings as _warnings
+import os as _os
 import pymunk as _pymunk
+import pygame
+
+from ..all_sprites import all_sprites
+from ..exceptions import Oops, Hmm
 from ..physics import physics_space, _Physics
-import warnings as _warnings
 from ..clamp import _clamp
 from ..io import screen
 from ..async_helpers import _make_async
 
 
 def _sprite_touching_sprite(a, b):
     # todo: custom code for circle, line, rotated rectangley sprites
     # use physics engine if both sprites have physics on
     # if a.physics and b.physics:
-    if a.left >= b.right or a.right <= b.left or a.top <= b.bottom or a.bottom >= b.top: return False
+    if a.left >= b.right or a.right <= b.left or a.top <= b.bottom or a.bottom >= b.top:
+        return False
     return True
 
 
-def _point_touching_sprite(point, sprite):
+def point_touching_sprite(point, sprite):
     # todo: custom code for circle, line, rotated rectangley sprites
-    return sprite.left <= point.x <= sprite.right and sprite.bottom <= point.y <= sprite.top
+    return (
+        sprite.left <= point.x <= sprite.right
+        and sprite.bottom <= point.y <= sprite.top
+    )
 
 
-class Sprite(object):
-    def __init__(self, image=None, x=0, y=0, size=100, angle=0, transparency=100):
-        self._image = image or _os.path.join(_os.path.split(__file__)[0], 'blank_image.png')
+class Sprite(): # pylint: disable=attribute-defined-outside-init, too-many-public-methods
+    def __init__(self, image=None, x=0, y=0, size=100, angle=0, transparency=100): # pylint: disable=too-many-arguments
+        self._image = image or _os.path.join(
+            _os.path.split(__file__)[0], "blank_image.png"
+        )
         self._x = x
         self._y = y
         self._angle = angle
         self._size = size
         self._transparency = transparency
 
         self.physics = None
@@ -42,18 +51,22 @@
         self._when_clicked_callbacks = []
 
         all_sprites.append(self)
 
     def _compute_primary_surface(self):
         try:
             self._primary_pygame_surface = pygame.image.load(_os.path.join(self._image))
-        except pygame.error as exc:
-            raise Oops(f"""We couldn't find the image file you provided named "{self._image}".
-If the file is in a folder, make sure you add the folder name, too.""") from exc
-        self._primary_pygame_surface.set_colorkey((255, 255, 255, 255))  # set background to transparent
+        except pygame.error as exc: # pylint: disable=no-member
+            raise Oops(
+                f"""We couldn't find the image file you provided named "{self._image}".
+If the file is in a folder, make sure you add the folder name, too."""
+            ) from exc
+        self._primary_pygame_surface.set_colorkey(
+            (255, 255, 255, 255)
+        )  # set background to transparent
 
         self._should_recompute_primary_surface = False
 
         # always recompute secondary surface if the primary surface changes
         self._compute_secondary_surface(force=True)
 
     def _compute_secondary_surface(self, force=False):
@@ -61,32 +74,40 @@
         self._secondary_pygame_surface = self._primary_pygame_surface.copy()
 
         # transparency
         if self._transparency != 100 or force:
             try:
                 # for text and images with transparent pixels
                 array = pygame.surfarray.pixels_alpha(self._secondary_pygame_surface)
-                array[:, :] = (array[:, :] * (self._transparency / 100.)).astype(
-                    array.dtype)  # modify surface pixels in-place
+                array[:, :] = (array[:, :] * (self._transparency / 100.0)).astype(
+                    array.dtype
+                )  # modify surface pixels in-place
                 del array  # I think pixels are written when array leaves memory, so delete it explicitly here
-            except Exception as e:
+            except Exception: # pylint: disable=broad-except
                 # this works for images without alpha pixels in them
-                self._secondary_pygame_surface.set_alpha(round((self._transparency / 100.) * 255))
+                self._secondary_pygame_surface.set_alpha(
+                    round((self._transparency / 100.0) * 255)
+                )
 
         # scale
         if (self.size != 100) or force:
-            ratio = self.size / 100.
+            ratio = self.size / 100.0
             self._secondary_pygame_surface = pygame.transform.scale(
                 self._secondary_pygame_surface,
-                (round(self._secondary_pygame_surface.get_width() * ratio),  # width
-                 round(self._secondary_pygame_surface.get_height() * ratio)))  # height
+                (
+                    round(self._secondary_pygame_surface.get_width() * ratio),  # width
+                    round(self._secondary_pygame_surface.get_height() * ratio),
+                ),
+            )  # height
 
         # rotate
         if (self.angle != 0) or force:
-            self._secondary_pygame_surface = pygame.transform.rotate(self._secondary_pygame_surface, self._angle)
+            self._secondary_pygame_surface = pygame.transform.rotate(
+                self._secondary_pygame_surface, self._angle
+            )
 
         self._should_recompute_secondary_surface = False
 
     @property
     def is_clicked(self):
         return self._is_clicked
 
@@ -106,15 +127,18 @@
     def x(self, _x):
         prev_x = self._x
         self._x = _x
         if self.physics:
             self.physics._pymunk_body.position = self._x, self._y
             if prev_x != _x:
                 # setting velocity makes the simulation more realistic usually
-                self.physics._pymunk_body.velocity = _x - prev_x, self.physics._pymunk_body.velocity.y
+                self.physics._pymunk_body.velocity = (
+                    _x - prev_x,
+                    self.physics._pymunk_body.velocity.y,
+                )
             if self.physics._pymunk_body.body_type == _pymunk.Body.STATIC:
                 physics_space.reindex_static()
 
     @property
     def y(self):
         return self._y
 
@@ -122,31 +146,39 @@
     def y(self, _y):
         prev_y = self._y
         self._y = _y
         if self.physics:
             self.physics._pymunk_body.position = self._x, self._y
             if prev_y != _y:
                 # setting velocity makes the simulation more realistic usually
-                self.physics._pymunk_body.velocity = self.physics._pymunk_body.velocity.x, _y - prev_y
+                self.physics._pymunk_body.velocity = (
+                    self.physics._pymunk_body.velocity.x,
+                    _y - prev_y,
+                )
             if self.physics._pymunk_body.body_type == _pymunk.Body.STATIC:
                 physics_space.reindex_static()
 
     @property
     def transparency(self):
         return self._transparency
 
     @transparency.setter
     def transparency(self, alpha):
         if not isinstance(alpha, float) and not isinstance(alpha, int):
-            raise Oops(f"""Looks like you're trying to set {self}'s transparency to '{alpha}', which isn't a number.
+            raise Oops(
+                f"""Looks like you're trying to set {self}'s transparency to '{alpha}', which isn't a number.
 Try looking in your code for where you're setting transparency for {self} and change it a number.
-""")
+"""
+            )
         if alpha > 100 or alpha < 0:
-            _warnings.warn(f"""The transparency setting for {self} is being set to {alpha} and it should be between 0 and 100.
-You might want to look in your code where you're setting transparency and make sure it's between 0 and 100.  """, Hmm)
+            _warnings.warn(
+                f"""The transparency setting for {self} is being set to {alpha} and it should be between 0 and 100.
+You might want to look in your code where you're setting transparency and make sure it's between 0 and 100.  """,
+                Hmm,
+            )
 
         self._transparency = _clamp(alpha, 0, 100)
         self._should_recompute_secondary_surface = True
 
     @property
     def image(self):
         return self._image
@@ -203,63 +235,62 @@
         return not self._is_hidden
 
     @is_shown.setter
     def is_shown(self, show):
         self._is_hidden = not show
 
     def is_touching(self, sprite_or_point):
-        rect = self._secondary_pygame_surface.get_rect()
+        self._secondary_pygame_surface.get_rect()
         if isinstance(sprite_or_point, Sprite):
             return _sprite_touching_sprite(sprite_or_point, self)
-        else:
-            return _point_touching_sprite(sprite_or_point, self)
+        return point_touching_sprite(sprite_or_point, self)
 
     def point_towards(self, x, y=None):
         try:
             x, y = x.x, x.y
         except AttributeError:
-            x, y = x, y
+            pass
         self.angle = _math.degrees(_math.atan2(y - self.y, x - self.x))
 
     def go_to(self, x=None, y=None):
         """
         Example:
 
             # text will follow around the mouse
             text = play.new_text('yay')
 
             @play.repeat_forever
             async def do():
                 text.go_to(play.mouse)
         """
-        assert (not x is None)
+        assert not x is None
 
         try:
             # users can call e.g. sprite.go_to(play.mouse), so x will be an object with x and y
             self.x = x.x
             self.y = x.y
         except AttributeError:
             self.x = x
             self.y = y
 
     def distance_to(self, x, y=None):
-        assert (not x is None)
+        assert not x is None
 
         try:
             # x can either be a number or a sprite. If it's a sprite:
             x1 = x.x
             y1 = x.y
         except AttributeError:
             x1 = x
             y1 = y
 
         dx = self.x - x1
         dy = self.y - y1
 
-        return _math.sqrt(dx ** 2 + dy ** 2)
+        return _math.sqrt(dx**2 + dy**2)
 
     def remove(self):
         if self.physics:
             self.physics._remove()
         all_sprites.remove(self)
 
     @property
@@ -299,18 +330,26 @@
         return self.y - self.height / 2
 
     @bottom.setter
     def bottom(self, y):
         self.y = y + self.height / 2
 
     def _pygame_x(self):
-        return self.x + (screen.width / 2.) - (self._secondary_pygame_surface.get_width() / 2.)
+        return (
+            self.x
+            + (screen.width / 2.0)
+            - (self._secondary_pygame_surface.get_width() / 2.0)
+        )
 
     def _pygame_y(self):
-        return (screen.height / 2.) - self.y - (self._secondary_pygame_surface.get_height() / 2.)
+        return (
+            (screen.height / 2.0)
+            - self.y
+            - (self._secondary_pygame_surface.get_height() / 2.0)
+        )
 
     # @decorator
     def when_clicked(self, callback, call_with_sprite=False):
         async_callback = _make_async(callback)
 
         async def wrapper():
             wrapper.is_running = True
@@ -322,15 +361,21 @@
 
         wrapper.is_running = False
         self._when_clicked_callbacks.append(wrapper)
         return wrapper
 
     def _common_properties(self):
         # used with inheritance to clone
-        return {'x': self.x, 'y': self.y, 'size': self.size, 'transparency': self.transparency, 'angle': self.angle}
+        return {
+            "x": self.x,
+            "y": self.y,
+            "size": self.size,
+            "transparency": self.transparency,
+            "angle": self.angle,
+        }
 
     def clone(self):
         # TODO: make work with physics
         return self.__class__(image=self.image, **self._common_properties())
 
     # def __getattr__(self, key):
     #     # TODO: use physics as a proxy object so users can do e.g. sprite.x_speed
@@ -341,16 +386,25 @@
 
     # def __setattr__(self, name, value):
     #     if not self.physics:
     #         return setattr(self, name, value)
     #     elif self.physics and name in :
     #         return setattr(self.physics, name, value)
 
-    def start_physics(self, can_move=True, stable=False, x_speed=0, y_speed=0, obeys_gravity=True, bounciness=1.0,
-                      mass=10, friction=0.1):
+    def start_physics( # pylint: disable=too-many-arguments
+        self,
+        can_move=True,
+        stable=False,
+        x_speed=0,
+        y_speed=0,
+        obeys_gravity=True,
+        bounciness=1.0,
+        mass=10,
+        friction=0.1,
+    ):
         if not self.physics:
             self.physics = _Physics(
                 self,
                 can_move,
                 stable,
                 x_speed,
                 y_speed,
```

### Comparing `corderius_play-1.0.2/play/objects/text.py` & `corderius_play-1.1.0/play/objects/text.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,38 @@
+"""This module contains the Text class, which is used to create text objects in the game."""
+import warnings as _warnings
 import pygame
 from .sprite import Sprite
 from ..all_sprites import all_sprites
 from ..exceptions import Hmm
-import warnings as _warnings
 from ..color import color_name_to_rgb as _color_name_to_rgb
 
 
 class Text(Sprite):
-    def __init__(self, words='hi :)', x=0, y=0, font=None, font_size=50, color='black', angle=0, transparency=100,
-                 size=100):
+    def __init__( # pylint: disable=too-many-arguments
+        self,
+        words="hi :)",
+        x=0,
+        y=0,
+        font=None,
+        font_size=50,
+        color="black",
+        angle=0,
+        transparency=100,
+        size=100,
+    ):
         self._font = font
         self._font_size = font_size
         self._words = words
         self._color = color
         super().__init__(x, y, size, angle, transparency)
 
         self._x = x
         self._y = y
 
-
-
         self._size = size
         self._angle = angle
         self.transparency = transparency
 
         self._is_clicked = False
         self._is_hidden = False
         self.physics = None
@@ -31,27 +40,36 @@
         self._compute_primary_surface()
 
         self._when_clicked_callbacks = []
 
         all_sprites.append(self)
 
     def clone(self):
-        return self.__class__(words=self.words, font=self.font, font_size=self.font_size, color=self.color,
-                              **self._common_properties())
+        return self.__class__(
+            words=self.words,
+            font=self.font,
+            font_size=self.font_size,
+            color=self.color,
+            **self._common_properties(),
+        )
 
     def _compute_primary_surface(self):
         try:
             self._pygame_font = pygame.font.Font(self._font, self._font_size)
-        except:
-            _warnings.warn(f"""We couldn't find the font file '{self._font}'. We'll use the default font instead for now.
-To fix this, either set the font to None, or make sure you have a font file (usually called something like Arial.ttf) in your project folder.\n""",
-                           Hmm)
+        except: # pylint: disable=bare-except
+            _warnings.warn(
+                f"""We couldn't find the font file '{self._font}'. We'll use the default font instead for now.""" + # pylint: disable=line-too-long
+"""To fix this, either set the font to None, or make sure you have a font file (usually called something like Arial.ttf) in your project folder.\n""", # pylint: disable=line-too-long
+                Hmm,
+            )
             self._pygame_font = pygame.font.Font(None, self._font_size)
 
-        self._primary_pygame_surface = self._pygame_font.render(self._words, True, _color_name_to_rgb(self._color))
+        self._primary_pygame_surface = self._pygame_font.render(
+            self._words, True, _color_name_to_rgb(self._color)
+        )
         self._should_recompute_primary_surface = False
 
         self._compute_secondary_surface(force=True)
 
     @property
     def words(self):
         return self._words
@@ -85,10 +103,29 @@
 
     @color.setter
     def color(self, color_):
         self._color = color_
         self._should_recompute_primary_surface = True
 
 
-def new_text(words='hi :)', x=0, y=0, font=None, font_size=50, color='black', angle=0, transparency=100, size=100):
-    return Text(words=words, x=x, y=y, font=font, font_size=font_size, color=color, angle=angle,
-                transparency=transparency, size=size)
+def new_text( # pylint: disable=too-many-arguments
+    words="hi :)",
+    x=0,
+    y=0,
+    font=None,
+    font_size=50,
+    color="black",
+    angle=0,
+    transparency=100,
+    size=100,
+):
+    return Text(
+        words=words,
+        x=x,
+        y=y,
+        font=font,
+        font_size=font_size,
+        color=color,
+        angle=angle,
+        transparency=transparency,
+        size=size,
+    )
```

### Comparing `corderius_play-1.0.2/play/physics/__init__.py` & `corderius_play-1.1.0/play/physics/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,30 @@
-import pymunk as _pymunk
+"""This handles the physics of the game."""
+
 import math as _math
+import pymunk as _pymunk
 from ..clamp import _clamp
 
 _SPEED_MULTIPLIER = 10
 
 
-class _Physics(object):
+class _Physics():
 
-    def __init__(self, sprite, can_move, stable, x_speed, y_speed, obeys_gravity, bounciness, mass, friction):
+    def __init__( # pylint: disable=too-many-arguments
+            self,
+            sprite,
+            can_move,
+            stable,
+            x_speed,
+            y_speed,
+            obeys_gravity,
+            bounciness,
+            mass,
+            friction,
+    ):
         """
 
         Examples of objects with the different parameters:
 
             Blocks that can be knocked over (the default):
                 can_move = True
                 stable = False
@@ -36,73 +49,98 @@
         self._obeys_gravity = obeys_gravity
         self._bounciness = bounciness
         self._mass = mass
         self._friction = friction
 
         self._make_pymunk()
 
-    def _make_pymunk(self):
+    def _make_pymunk(self): # pylint: disable=too-many-branches
         mass = self.mass if self.can_move else 0
 
         # non-moving line shapes are platforms and it's easier to take care of them less-generically
         if not self.can_move and self.sprite.__class__ == "Line":
             self._pymunk_body = physics_space.static_body.copy()
-            self._pymunk_shape = _pymunk.Segment(self._pymunk_body, (self.sprite.x, self.sprite.y),
-                                                 (self.sprite.x1, self.sprite.y1), self.sprite.thickness)
+            self._pymunk_shape = _pymunk.Segment(
+                self._pymunk_body,
+                (self.sprite.x, self.sprite.y),
+                (self.sprite.x1, self.sprite.y1),
+                self.sprite.thickness,
+            )
         else:
             if self.stable:
-                moment = _pymunk.inf
+                moment = float("inf")
             elif self.sprite.__class__ == "Circle":
                 moment = _pymunk.moment_for_circle(mass, 0, self.sprite.radius, (0, 0))
             elif self.sprite.__class__ == "Line":
-                moment = _pymunk.moment_for_box(mass, (self.sprite.length, self.sprite.thickness))
+                moment = _pymunk.moment_for_box(
+                    mass, (self.sprite.length, self.sprite.thickness)
+                )
             else:
-                moment = _pymunk.moment_for_box(mass, (self.sprite.width, self.sprite.height))
+                moment = _pymunk.moment_for_box(
+                    mass, (self.sprite.width, self.sprite.height)
+                )
 
             if self.can_move and not self.stable:
                 body_type = _pymunk.Body.DYNAMIC
             elif self.can_move and self.stable:
                 if self.obeys_gravity or physics_space.gravity == 0:
                     body_type = _pymunk.Body.DYNAMIC
                 else:
                     body_type = _pymunk.Body.KINEMATIC
             else:
                 body_type = _pymunk.Body.STATIC
             self._pymunk_body = _pymunk.Body(mass, moment, body_type=body_type)
 
             if self.sprite.__class__ == "Line":
-                self._pymunk_body.position = self.sprite.x + (self.sprite.x1 - self.sprite.x) / 2, self.sprite.y + (
-                        self.sprite.y1 - self.sprite.y) / 2
+                self._pymunk_body.position = (
+                    self.sprite.x + (self.sprite.x1 - self.sprite.x) / 2,
+                    self.sprite.y + (self.sprite.y1 - self.sprite.y) / 2,
+                )
             else:
                 self._pymunk_body.position = self.sprite.x, self.sprite.y
 
             self._pymunk_body.angle = _math.radians(self.sprite.angle)
 
             if self.can_move:
                 self._pymunk_body.velocity = (self._x_speed, self._y_speed)
 
             if not self.obeys_gravity:
-                self._pymunk_body.velocity_func = lambda body, gravity, damping, dt: None
+                self._pymunk_body.velocity_func = (
+                    lambda body, gravity, damping, dt: None
+                )
 
             if self.sprite.__class__ == "Circle":
-                self._pymunk_shape = _pymunk.Circle(self._pymunk_body, self.sprite.radius, (0, 0))
+                self._pymunk_shape = _pymunk.Circle(
+                    self._pymunk_body, self.sprite.radius, (0, 0)
+                )
             elif self.sprite.__class__ == "Line":
-                self._pymunk_shape = _pymunk.Segment(self._pymunk_body, (self.sprite.x, self.sprite.y),
-                                                     (self.sprite.x1, self.sprite.y1), self.sprite.thickness)
+                self._pymunk_shape = _pymunk.Segment(
+                    self._pymunk_body,
+                    (self.sprite.x, self.sprite.y),
+                    (self.sprite.x1, self.sprite.y1),
+                    self.sprite.thickness,
+                )
             else:
-                self._pymunk_shape = _pymunk.Poly.create_box(self._pymunk_body, (self.sprite.width, self.sprite.height))
+                self._pymunk_shape = _pymunk.Poly.create_box(
+                    self._pymunk_body, (self.sprite.width, self.sprite.height)
+                )
 
-        self._pymunk_shape.elasticity = _clamp(self.bounciness, 0, .99)
+        self._pymunk_shape.elasticity = _clamp(self.bounciness, 0, 0.99)
         self._pymunk_shape.friction = self._friction
         physics_space.add(self._pymunk_body, self._pymunk_shape)
 
     def clone(self, sprite):
         # TODO: finish filling out params
-        return self.__class__(sprite=sprite, can_move=self.can_move, x_speed=self.x_speed,
-                              y_speed=self.y_speed, obeys_gravity=self.obeys_gravity)
+        return self.__class__( # pylint: disable=no-value-for-parameter
+            sprite=sprite,
+            can_move=self.can_move,
+            x_speed=self.x_speed,
+            y_speed=self.y_speed,
+            obeys_gravity=self.obeys_gravity,
+        )
 
     def pause(self):
         self._remove()
 
     def unpause(self):
         if not self._pymunk_body and not self._pymunk_shape:
             physics_space.add(self._pymunk_body, self._pymunk_shape)
@@ -146,15 +184,15 @@
     @property
     def bounciness(self):
         return self._bounciness
 
     @bounciness.setter
     def bounciness(self, _bounciness):
         self._bounciness = _bounciness
-        self._pymunk_shape.elasticity = _clamp(self._bounciness, 0, .99)
+        self._pymunk_shape.elasticity = _clamp(self._bounciness, 0, 0.99)
 
     @property
     def stable(self):
         return self._stable
 
     @stable.setter
     def stable(self, _stable):
@@ -182,34 +220,36 @@
         self._obeys_gravity = _obeys_gravity
         if _obeys_gravity:
             self._pymunk_body.velocity_func = _pymunk.Body.update_velocity
         else:
             self._pymunk_body.velocity_func = lambda body, gravity, damping, dt: None
 
 
-class _Gravity(object):
+class _Gravity(): # pylint: disable=too-few-public-methods
     # TODO: make this default to vertical if horizontal is 0?
     vertical = -100 * _SPEED_MULTIPLIER
     horizontal = 0
 
 
-gravity = _Gravity()
+GRAVITY = _Gravity()
 physics_space = _pymunk.Space()
 physics_space.sleep_time_threshold = 0.5
-physics_space.idle_speed_threshold = 0  # pymunk estimates good threshold based on gravity
-physics_space.gravity = gravity.horizontal, gravity.vertical
+physics_space.idle_speed_threshold = (
+    0  # pymunk estimates good threshold based on gravity
+)
+physics_space.gravity = GRAVITY.horizontal, GRAVITY.vertical
 
 
 def set_gravity(vertical=-100, horizontal=None):
-    global gravity
-    gravity.vertical = vertical * _SPEED_MULTIPLIER
-    if horizontal != None:
-        gravity.horizontal = horizontal * _SPEED_MULTIPLIER
+    global GRAVITY # pylint: disable=global-variable-not-assigned
+    GRAVITY.vertical = vertical * _SPEED_MULTIPLIER
+    if horizontal is not None:
+        GRAVITY.horizontal = horizontal * _SPEED_MULTIPLIER
 
-    physics_space.gravity = gravity.horizontal, gravity.vertical
+    physics_space.gravity = GRAVITY.horizontal, GRAVITY.vertical
 
 
 _NUM_SIMULATION_STEPS = 3
 
 
 def simulate_physics():
     # more steps means more accurate simulation, but more processing time
```

### Comparing `corderius_play-1.0.2/play/play.py` & `corderius_play-1.1.0/play/play.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,40 @@
+"""The main source file of the play library."""
+
 import logging as _logging
-import warnings as _warnings
-from .async_helpers import _make_async
-import pygame
+import math as _math
+import random as _random
+import asyncio as _asyncio
 
-pygame.init()
+import pygame
 import pygame.gfxdraw
 
-import asyncio as _asyncio
-import random as _random
+from .async_helpers import _make_async
+
 
-from .keypress import \
-    pygame_key_to_name as _pygame_key_to_name  # don't pollute user-facing namespace with library internals
 from .color import color_name_to_rgb as _color_name_to_rgb
-from .exceptions import Oops, Hmm
-import math as _math
-from .io import screen
+
+from .io import screen, PYGAME_DISPLAY
 from .physics import simulate_physics
 from .all_sprites import all_sprites
 from .objects import Line
-from .objects.sprite import _point_touching_sprite
+from .objects.sprite import point_touching_sprite
+
+pygame.init() # pylint: disable=no-member
+
+# pylint: disable=wrong-import-position
+from .keypress import (
+    pygame_key_to_name as _pygame_key_to_name, _loop, _keys_pressed_this_frame, _keys_released_this_frame,
+    _keys_to_skip, _pressed_keys, _keypress_callbacks, _keyrelease_callbacks,
+)  # don't pollute user-facing namespace with library internals
 
 # _pygame_display = pygame.display.set_mode((screen_width, screen_height), pygame.DOUBLEBUF | pygame.OPENGL)
-_pygame_display = pygame.display.set_mode((screen.width, screen.height), pygame.DOUBLEBUF)
-pygame.display.set_caption("Python Play")
 
 
-class _Mouse(object):
+class _Mouse():
     def __init__(self):
         self.x = 0
         self.y = 0
         self._is_clicked = False
         self._when_clicked_callbacks = []
         self._when_click_released_callbacks = []
 
@@ -39,15 +44,15 @@
         #    if play.mouse.is_clicked: # <-- forgetting parentheses causes bad behavior
         #        ...
         # and is_clicked is a method (they forgot the parens), then it will always
         # return True. Better to eliminate the need for parens.
         return self._is_clicked
 
     def is_touching(self, other):
-        return _point_touching_sprite(self, other)
+        return point_touching_sprite(self, other)
 
     # @decorator
     def when_clicked(self, func):
         async_callback = _make_async(func)
 
         async def wrapper():
             await async_callback()
@@ -62,96 +67,94 @@
         async def wrapper():
             await async_callback()
 
         self._when_click_released_callbacks.append(wrapper)
         return wrapper
 
     def distance_to(self, x=None, y=None):
-        assert (not x is None)
+        assert x is not None
 
         try:
             # x can either by a number or a sprite. If it's a sprite:
             x = x.x
             y = x.y
         except AttributeError:
-            x = x
-            y = y
+            pass
 
         dx = self.x - x
         dy = self.y - y
 
-        return _math.sqrt(dx ** 2 + dy ** 2)
+        return _math.sqrt(dx**2 + dy**2)
 
 
 # @decorator
 def when_mouse_clicked(func):
     return mouse.when_clicked(func)
 
 
 # @decorator
 def when_click_released(func):
     return mouse.when_click_released(func)
 
 
 mouse = _Mouse()
 
-_debug = True
+_DEBUG = True
 
 
 def debug(on_or_off):
-    global _debug
-    if on_or_off == 'on':
-        _debug = True
-    elif on_or_off == 'off':
-        _debug = False
+    global _DEBUG
+    if on_or_off == "on":
+        _DEBUG = True
+    elif on_or_off == "off":
+        _DEBUG = False
 
 
-backdrop = (255, 255, 255)
+BACKDROP = (255, 255, 255)
 
 
 def set_backdrop(color_or_image_name):
-    global backdrop
+    global BACKDROP
 
     # I chose to make set_backdrop a function so that we can give
     # good error messages at the call site if a color isn't recognized.
     # If we didn't have a function and just set backdrop like this:
     #
     #       play.backdrop = 'gbluereen'
     #
     # then any errors resulting from that statement would appear somewhere
     # deep in this library instead of in the user code.
 
     # this line will raise a useful exception
     _color_name_to_rgb(color_or_image_name)
 
-    backdrop = color_or_image_name
+    BACKDROP = color_or_image_name
 
 
 def random_number(lowest=0, highest=100):
     # if user supplies whole numbers, return whole numbers
-    if type(lowest) == int and type(highest) == int:
+    if isinstance(lowest, int) and isinstance(highest, int):
         return _random.randint(lowest, highest)
-    else:
-        # if user supplied any floats, return decimals
-        return round(_random.uniform(lowest, highest), 2)
+    # if user supplied any floats, return decimals
+    return round(_random.uniform(lowest, highest), 2)
 
 
 def random_color():
-    return (random_number(0, 255), random_number(0, 255), random_number(0, 255))
+    return random_number(0, 255), random_number(0, 255), random_number(0, 255)
 
 
-class _Position(object):
+class _Position():
     def __init__(self, x, y):
         self.x = x
         self.y = y
 
     def __getitem__(self, indices):
         if indices == 0:
             return self.x
-        elif indices == 1:
+        if indices == 1:
             return self.y
         raise IndexError()
 
     def __iter__(self):
         yield self.x
         yield self.y
 
@@ -175,194 +178,89 @@
         sprite.y = position.y
 
     or equivalently:
         sprite.go_to(play.random_position())
     """
     return _Position(
         random_number(screen.left, screen.right),
-        random_number(screen.bottom, screen.top)
+        random_number(screen.bottom, screen.top),
     )
 
 
 # @decorator
 def when_sprite_clicked(*sprites):
     def wrapper(func):
         for sprite in sprites:
             sprite.when_clicked(func, call_with_sprite=True)
         return func
 
     return wrapper
 
 
-pygame.key.set_repeat(200, 16)
-_pressed_keys = {}
-_keypress_callbacks = []
-_keyrelease_callbacks = []
-
-
-# @decorator
-def when_any_key_pressed(func):
-    if not callable(func):
-        raise Oops("""@play.when_any_key_pressed doesn't use a list of keys. Try just this instead:
-
-@play.when_any_key_pressed
-async def do(key):
-    print("This key was pressed!", key)
-""")
-    async_callback = _make_async(func)
-
-    async def wrapper(*args, **kwargs):
-        wrapper.is_running = True
-        await async_callback(*args, **kwargs)
-        wrapper.is_running = False
-
-    wrapper.keys = None
-    wrapper.is_running = False
-    _keypress_callbacks.append(wrapper)
-    return wrapper
-
-
-# @decorator
-def when_key_pressed(*keys):
-    def decorator(func):
-        async_callback = _make_async(func)
-
-        async def wrapper(*args, **kwargs):
-            wrapper.is_running = True
-            await async_callback(*args, **kwargs)
-            wrapper.is_running = False
-
-        wrapper.keys = keys
-        wrapper.is_running = False
-        _keypress_callbacks.append(wrapper)
-        return wrapper
-
-    return decorator
-
-
-# @decorator
-def when_any_key_released(func):
-    if not callable(func):
-        raise Oops("""@play.when_any_key_released doesn't use a list of keys. Try just this instead:
-
-@play.when_any_key_released
-async def do(key):
-    print("This key was released!", key)
-""")
-    async_callback = _make_async(func)
-
-    async def wrapper(*args, **kwargs):
-        wrapper.is_running = True
-        await async_callback(*args, **kwargs)
-        wrapper.is_running = False
-
-    wrapper.keys = None
-    wrapper.is_running = False
-    _keyrelease_callbacks.append(wrapper)
-    return wrapper
-
-
-# @decorator
-def when_key_released(*keys):
-    def decorator(func):
-        async_callback = _make_async(func)
-
-        async def wrapper(*args, **kwargs):
-            wrapper.is_running = True
-            await async_callback(*args, **kwargs)
-            wrapper.is_running = False
-
-        wrapper.keys = keys
-        wrapper.is_running = False
-        _keyrelease_callbacks.append(wrapper)
-        return wrapper
-
-    return decorator
-
-
-def key_is_pressed(*keys):
-    """
-    Returns True if any of the given keys are pressed.
-
-    Example:
-
-        @play.repeat_forever
-        async def do():
-            if play.key_is_pressed('up', 'w'):
-                print('up or w pressed')
-    """
-    # Called this function key_is_pressed instead of is_key_pressed so it will
-    # sound more english-like with if-statements:
-    #
-    #   if play.key_is_pressed('w', 'up'): ...
-
-    for key in keys:
-        if key in _pressed_keys.values():
-            return True
-    return False
-
-
-_loop = _asyncio.get_event_loop()
-_loop.set_debug(False)
-
-_keys_pressed_this_frame = []
-_keys_released_this_frame = []
-_keys_to_skip = (pygame.K_MODE,)
-pygame.event.set_allowed(
-    [pygame.QUIT, pygame.KEYDOWN, pygame.KEYUP, pygame.MOUSEBUTTONDOWN, pygame.MOUSEBUTTONUP, pygame.MOUSEMOTION])
 _clock = pygame.time.Clock()
 
 
+# pylint: disable=too-many-branches, too-many-statements
 def _game_loop():
     _keys_pressed_this_frame.clear()  # do this instead of `_keys_pressed_this_frame = []` to save a tiny bit of memory
     _keys_released_this_frame.clear()
     click_happened_this_frame = False
     click_release_happened_this_frame = False
 
     _clock.tick(60)
     for event in pygame.event.get():
-        if event.type == pygame.QUIT or (
-                event.type == pygame.KEYDOWN and event.key == pygame.K_q and (
-                pygame.key.get_mods() & pygame.KMOD_META or pygame.key.get_mods() & pygame.KMOD_CTRL
-        )):
+        if event.type == pygame.QUIT or ( # pylint: disable=no-member
+            event.type == pygame.KEYDOWN # pylint: disable=no-member
+            and event.key == pygame.K_q # pylint: disable=no-member
+            and (
+                pygame.key.get_mods() & pygame.KMOD_META # pylint: disable=no-member
+                or pygame.key.get_mods() & pygame.KMOD_CTRL # pylint: disable=no-member
+            )
+        ):
             # quitting by clicking window's close button or pressing ctrl+q / command+q
             _loop.stop()
             return False
-        if event.type == pygame.MOUSEBUTTONDOWN:
+        if event.type == pygame.MOUSEBUTTONDOWN: # pylint: disable=no-member
             click_happened_this_frame = True
             mouse._is_clicked = True
-        if event.type == pygame.MOUSEBUTTONUP:
+        if event.type == pygame.MOUSEBUTTONUP: # pylint: disable=no-member
             click_release_happened_this_frame = True
             mouse._is_clicked = False
-        if event.type == pygame.MOUSEMOTION:
-            mouse.x, mouse.y = (event.pos[0] - screen.width / 2.), (screen.height / 2. - event.pos[1])
-        if event.type == pygame.KEYDOWN:
-            if not (event.key in _keys_to_skip):
+        if event.type == pygame.MOUSEMOTION: # pylint: disable=no-member
+            mouse.x, mouse.y = (event.pos[0] - screen.width / 2.0), (
+                screen.height / 2.0 - event.pos[1]
+            )
+        if event.type == pygame.KEYDOWN: # pylint: disable=no-member
+            if event.key not in _keys_to_skip:
                 name = _pygame_key_to_name(event)
                 _pressed_keys[event.key] = name
                 _keys_pressed_this_frame.append(name)
-        if event.type == pygame.KEYUP:
+        if event.type == pygame.KEYUP: # pylint: disable=no-member
             if not (event.key in _keys_to_skip) and event.key in _pressed_keys:
                 _keys_released_this_frame.append(_pressed_keys[event.key])
                 del _pressed_keys[event.key]
 
     ############################################################
     # @when_any_key_pressed and @when_key_pressed callbacks
     ############################################################
     for key in _keys_pressed_this_frame:
         for callback in _keypress_callbacks:
-            if not callback.is_running and (callback.keys is None or key in callback.keys):
+            if not callback.is_running and (
+                callback.keys is None or key in callback.keys
+            ):
                 _loop.create_task(callback(key))
 
     ############################################################
     # @when_any_key_released and @when_key_released callbacks
     ############################################################
     for key in _keys_released_this_frame:
         for callback in _keyrelease_callbacks:
-            if not callback.is_running and (callback.keys is None or key in callback.keys):
+            if not callback.is_running and (
+                callback.keys is None or key in callback.keys
+            ):
                 _loop.create_task(callback(key))
 
     ####################################
     # @mouse.when_clicked callbacks
     ####################################
     if click_happened_this_frame and mouse._when_clicked_callbacks:
         for callback in mouse._when_clicked_callbacks:
@@ -396,15 +294,15 @@
     # 6.  run mouse/click callbacks (make sure more than one isn't running at a time)
     # 7.  run keyboard callbacks (make sure more than one isn't running at a time)
     # 8.  run when_touched callbacks
     # 9.  render background
     # 10. render sprites (with correct z-order)
     # 11. call event loop again
 
-    _pygame_display.fill(_color_name_to_rgb(backdrop))
+    PYGAME_DISPLAY.fill(_color_name_to_rgb(BACKDROP))
 
     # BACKGROUND COLOR
     # note: cannot use screen.fill((1, 1, 1)) because pygame's screen
     #       does not support fill() on OpenGL surfaces
     # gl.glClearColor(_background_color[0], _background_color[1], _background_color[2], 1)
     # gl.glClear(gl.GL_COLOR_BUFFER_BIT)
 
@@ -425,68 +323,90 @@
             if isinstance(sprite, Line):
                 sprite._x = body.position.x - (sprite.length / 2) * _math.cos(angle)
                 sprite._y = body.position.y - (sprite.length / 2) * _math.sin(angle)
                 sprite._x1 = body.position.x + (sprite.length / 2) * _math.cos(angle)
                 sprite._y1 = body.position.y + (sprite.length / 2) * _math.sin(angle)
                 # sprite._length, sprite._angle = sprite._calc_length_angle()
             else:
-                if str(body.position.x) != 'nan':  # this condition can happen when changing sprite.physics.can_move
+                if (
+                    str(body.position.x) != "nan"
+                ):  # this condition can happen when changing sprite.physics.can_move
                     sprite._x = body.position.x
-                if str(body.position.y) != 'nan':
+                if str(body.position.y) != "nan":
                     sprite._y = body.position.y
 
-            sprite.angle = angle  # needs to be .angle, not ._angle so surface gets recalculated
+            sprite.angle = (
+                angle  # needs to be .angle, not ._angle so surface gets recalculated
+            )
             sprite.physics._x_speed, sprite.physics._y_speed = body.velocity
 
         #################################
         # @sprite.when_clicked events
         #################################
-        if mouse.is_clicked and not type(sprite) == Line:
-            if _point_touching_sprite(mouse, sprite):
+        if mouse.is_clicked and not isinstance(sprite, Line):
+            if point_touching_sprite(mouse, sprite) and click_happened_this_frame:
                 # only run sprite clicks on the frame the mouse was clicked
-                if click_happened_this_frame:
-                    sprite._is_clicked = True
-                    for callback in sprite._when_clicked_callbacks:
-                        if not callback.is_running:
-                            _loop.create_task(callback())
+                sprite._is_clicked = True
+                for callback in sprite._when_clicked_callbacks:
+                    if not callback.is_running:
+                        _loop.create_task(callback())
 
         # do sprite image transforms (re-rendering images/fonts, scaling, rotating, etc)
 
         # we put it in the event loop instead of just recomputing immediately because if we do it
         # synchronously then the data and rendered image may get out of sync
         if sprite._should_recompute_primary_surface:
             # recomputing primary surface also recomputes secondary surface
             _loop.call_soon(sprite._compute_primary_surface)
         elif sprite._should_recompute_secondary_surface:
             _loop.call_soon(sprite._compute_secondary_surface)
 
-        if type(sprite) == Line:
+        if isinstance(sprite, Line):
             # @hack: Line-drawing code should probably be in the line._compute_primary_surface function
             # but the coordinates work different for lines than other sprites.
 
             # x = screen.width/2 + sprite.x
             # y = screen.height/2 - sprite.y - sprite.thickness
             # _pygame_display.blit(sprite._secondary_pygame_surface, (x,y) )
 
-            x = screen.width / 2 + sprite.x
-            y = screen.height / 2 - sprite.y
-            x1 = screen.width / 2 + sprite.x1
-            y1 = screen.height / 2 - sprite.y1
+            x = screen.width / 2 + sprite.x # pylint: disable=invalid-name
+            y = screen.height / 2 - sprite.y # pylint: disable=invalid-name
+            x_1 = screen.width / 2 + sprite.x1
+            y_1 = screen.height / 2 - sprite.y1
             if sprite.thickness == 1:
-                pygame.draw.aaline(_pygame_display, _color_name_to_rgb(sprite.color), (x, y), (x1, y1), True)
+                pygame.draw.aaline(
+                    PYGAME_DISPLAY,
+                    _color_name_to_rgb(sprite.color),
+                    (x, y),
+                    (x_1, y_1),
+                    True,
+                )
             else:
-                pygame.draw.line(_pygame_display, _color_name_to_rgb(sprite.color), (x, y), (x1, y1), sprite.thickness)
+                pygame.draw.line(
+                    PYGAME_DISPLAY,
+                    _color_name_to_rgb(sprite.color),
+                    (x, y),
+                    (x_1, y_1),
+                    sprite.thickness,
+                )
         else:
-            _pygame_display.blit(sprite._secondary_pygame_surface, (sprite._pygame_x(), sprite._pygame_y()))
+
+            PYGAME_DISPLAY.blit(
+                sprite._secondary_pygame_surface,
+                (sprite._pygame_x(), sprite._pygame_y()),
+            )
 
     pygame.display.flip()
     _loop.call_soon(_game_loop)
     return True
 
 
+# pylint: enable=too-many-branches, too-many-statements
+
+
 async def timer(seconds=1.0):
     """
     Wait a number of seconds. Used with the await keyword like this:
 
     @play.repeat_forever
     async def do():
         await play.timer(seconds=2)
@@ -564,15 +484,15 @@
 
     _when_program_starts_callbacks.append(wrapper)
     return func
 
 
 def repeat(number_of_times):
     """
-    Repeat a set of commands a certain number of times. 
+    Repeat a set of commands a certain number of times.
 
     Equivalent to `range(1, number_of_times+1)`.
 
     Used like this:
 
     @play.repeat_forever
     async def do():
@@ -592,8 +512,8 @@
         _loop.create_task(func())
 
     _loop.call_soon(_game_loop)
     try:
         _loop.run_forever()
     finally:
         _logging.getLogger("asyncio").setLevel(_logging.CRITICAL)
-        pygame.quit()
+        pygame.quit()  # pylint: disable=no-member
```

### Comparing `corderius_play-1.0.2/setup.py` & `corderius_play-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="corderius-play",
-    version="1.0.2",
+    version="1.1.0",
     description="The easiest way to make games and media projects in Python.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Corderius-College-Amersfoort/play",
     author="koen1711",
     author_email="koenvurk1711@gmail.com",
     license="MIT",
```

