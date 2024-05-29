# Comparing `tmp/sanghyunjo-1.4.2.tar.gz` & `tmp/sanghyunjo-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sanghyunjo-1.4.2.tar", last modified: Tue May 28 15:17:55 2024, max compression
+gzip compressed data, was "dist\sanghyunjo-1.4.3.tar", last modified: Wed May 29 06:40:16 2024, max compression
```

## Comparing `sanghyunjo-1.4.2.tar` & `sanghyunjo-1.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 15:17:55.664555 sanghyunjo-1.4.2/
--rw-rw-rw-   0        0        0     1087 2024-05-16 07:32:54.000000 sanghyunjo-1.4.2/LICENSE
--rw-rw-rw-   0        0        0       53 2024-05-16 07:24:52.000000 sanghyunjo-1.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0      365 2024-05-28 15:17:55.662561 sanghyunjo-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-05-16 07:32:26.000000 sanghyunjo-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 15:17:55.642785 sanghyunjo-1.4.2/sanghyunjo/
--rw-rw-rw-   0        0        0      194 2024-05-28 15:16:56.000000 sanghyunjo-1.4.2/sanghyunjo/__init__.py
--rw-rw-rw-   0        0        0     9340 2024-05-28 15:17:36.000000 sanghyunjo-1.4.2/sanghyunjo/cv_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-28 15:17:55.660565 sanghyunjo-1.4.2/sanghyunjo/fonts/
--rw-rw-rw-   0        0        0    34888 2023-07-19 08:59:35.000000 sanghyunjo-1.4.2/sanghyunjo/fonts/Times New Roman MT Std.otf
--rw-rw-rw-   0        0        0      358 2024-05-20 07:08:56.000000 sanghyunjo-1.4.2/sanghyunjo/json_utils.py
--rw-rw-rw-   0        0        0     3115 2024-05-26 14:14:30.000000 sanghyunjo-1.4.2/sanghyunjo/misc.py
-drwxrwxrwx   0        0        0        0 2024-05-28 15:17:55.662561 sanghyunjo-1.4.2/sanghyunjo.egg-info/
--rw-rw-rw-   0        0        0      365 2024-05-28 15:17:55.000000 sanghyunjo-1.4.2/sanghyunjo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2024-05-28 15:17:55.000000 sanghyunjo-1.4.2/sanghyunjo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 15:17:55.000000 sanghyunjo-1.4.2/sanghyunjo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-16 07:28:15.000000 sanghyunjo-1.4.2/sanghyunjo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-28 15:17:55.000000 sanghyunjo-1.4.2/sanghyunjo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 15:17:55.664555 sanghyunjo-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      828 2024-05-20 07:09:32.000000 sanghyunjo-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 06:40:16.174271 sanghyunjo-1.4.3/
+-rw-rw-rw-   0        0        0     1087 2024-05-16 07:32:54.000000 sanghyunjo-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-05-16 07:24:52.000000 sanghyunjo-1.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      365 2024-05-29 06:40:16.173275 sanghyunjo-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-05-28 15:18:59.000000 sanghyunjo-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 06:40:16.151332 sanghyunjo-1.4.3/sanghyunjo/
+-rw-rw-rw-   0        0        0      194 2024-05-29 06:40:07.000000 sanghyunjo-1.4.3/sanghyunjo/__init__.py
+-rw-rw-rw-   0        0        0     9449 2024-05-29 06:39:32.000000 sanghyunjo-1.4.3/sanghyunjo/cv_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 06:40:16.171278 sanghyunjo-1.4.3/sanghyunjo/fonts/
+-rw-rw-rw-   0        0        0    34888 2023-07-19 08:59:35.000000 sanghyunjo-1.4.3/sanghyunjo/fonts/Times New Roman MT Std.otf
+-rw-rw-rw-   0        0        0      358 2024-05-20 07:08:56.000000 sanghyunjo-1.4.3/sanghyunjo/json_utils.py
+-rw-rw-rw-   0        0        0     3115 2024-05-26 14:14:30.000000 sanghyunjo-1.4.3/sanghyunjo/misc.py
+drwxrwxrwx   0        0        0        0 2024-05-29 06:40:16.172276 sanghyunjo-1.4.3/sanghyunjo.egg-info/
+-rw-rw-rw-   0        0        0      365 2024-05-29 06:40:15.000000 sanghyunjo-1.4.3/sanghyunjo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2024-05-29 06:40:16.000000 sanghyunjo-1.4.3/sanghyunjo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 06:40:15.000000 sanghyunjo-1.4.3/sanghyunjo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-16 07:28:15.000000 sanghyunjo-1.4.3/sanghyunjo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-29 06:40:15.000000 sanghyunjo-1.4.3/sanghyunjo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 06:40:16.174271 sanghyunjo-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      828 2024-05-20 07:09:32.000000 sanghyunjo-1.4.3/setup.py
```

### Comparing `sanghyunjo-1.4.2/LICENSE` & `sanghyunjo-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.4.2/README.md` & `sanghyunjo-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.4.2/sanghyunjo/cv_utils.py` & `sanghyunjo-1.4.3/sanghyunjo/cv_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,29 +37,37 @@
         elif event == cv2.EVENT_RBUTTONDOWN: self.rightdown(x, y)
         elif event == cv2.EVENT_RBUTTONUP: self.rightup(x, y)
         elif event == cv2.EVENT_MOUSEMOVE: self.move(x, y)
         elif event == cv2.EVENT_MOUSEWHEEL: 
             if flags > 0: self.wheelup()
             else: self.wheeldown()
 
-def read_image(path, mode='opencv', unicode=False, mask=False):
-    if mode == 'opencv': 
-        if unicode: 
-            return cv2.imdecode(
-                np.fromfile(path, dtype=np.uint8), 
-                cv2.IMREAD_UNCHANGED
-            )
-        else: 
-            return cv2.imread(path, cv2.IMREAD_UNCHANGED)
-    else: 
-        try: 
-            image = Image.open(path)
-            return image if mask else image.convert('RGB')
-        except FileNotFoundError: 
-            return None
+def read_image(path, mode='opencv', color=None):
+    color_dict = {
+        'opencv': {
+            'gray': cv2.IMREAD_GRAYSCALE,
+            'rgb': cv2.IMREAD_COLOR,
+            None: cv2.IMREAD_UNCHANGED,
+        },
+        'pillow': {
+            'gray': 'L',
+            'rgb': 'RGB',
+            None: None
+        }
+    }
+
+    try: 
+        if mode == 'opencv':
+            image = cv2.imdecode(np.fromfile(path, np.uint8), color_dict[color])
+        else:
+            image = Image.open(path).convert(color_dict[color])
+    except FileNotFoundError: 
+        image = None
+    
+    return image
 
 def write_image(path, image, palette=None):
     if palette is None: cv2.imwrite(path, image)
     else:
         image = Image.fromarray(image.astype(np.uint8)).convert('P')
         image.putpalette(palette)
         image.save(path)
```

### Comparing `sanghyunjo-1.4.2/sanghyunjo/fonts/Times New Roman MT Std.otf` & `sanghyunjo-1.4.3/sanghyunjo/fonts/Times New Roman MT Std.otf`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.4.2/sanghyunjo/misc.py` & `sanghyunjo-1.4.3/sanghyunjo/misc.py`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.4.2/setup.py` & `sanghyunjo-1.4.3/setup.py`

 * *Files identical despite different names*

