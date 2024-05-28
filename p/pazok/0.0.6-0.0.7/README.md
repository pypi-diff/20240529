# Comparing `tmp/pazok-0.0.6.tar.gz` & `tmp/pazok-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pazok-0.0.6.tar", last modified: Sat May 25 00:41:05 2024, max compression
+gzip compressed data, was "pazok-0.0.7.tar", last modified: Tue May 28 17:56:25 2024, max compression
```

## Comparing `pazok-0.0.6.tar` & `pazok-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 00:41:05.667894 pazok-0.0.6/
--rw-rw-rw-   0        0        0       29 2024-05-23 23:30:01.000000 pazok-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     1166 2024-05-25 00:41:05.665360 pazok-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-05-23 23:29:46.000000 pazok-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 00:41:05.639570 pazok-0.0.6/pazok/
--rw-rw-rw-   0        0        0      745 2024-05-25 00:14:14.000000 pazok-0.0.6/pazok/__init__.py
--rw-rw-rw-   0        0        0    44346 2024-05-25 00:40:09.000000 pazok-0.0.6/pazok/pazok.py
-drwxrwxrwx   0        0        0        0 2024-05-25 00:41:05.663368 pazok-0.0.6/pazok.egg-info/
--rw-rw-rw-   0        0        0     1166 2024-05-25 00:41:05.000000 pazok-0.0.6/pazok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-05-25 00:41:05.000000 pazok-0.0.6/pazok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 00:41:05.000000 pazok-0.0.6/pazok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-25 00:41:05.000000 pazok-0.0.6/pazok.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-25 00:41:05.000000 pazok-0.0.6/pazok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 00:41:05.667894 pazok-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      605 2024-05-25 00:40:33.000000 pazok-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:56:25.551854 pazok-0.0.7/
+-rw-rw-rw-   0        0        0       29 2024-05-23 23:30:01.000000 pazok-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     1166 2024-05-28 17:56:25.548861 pazok-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-05-23 23:29:46.000000 pazok-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 17:56:25.526933 pazok-0.0.7/pazok/
+-rw-rw-rw-   0        0        0      745 2024-05-28 17:55:36.000000 pazok-0.0.7/pazok/__init__.py
+-rw-rw-rw-   0        0        0    44869 2024-05-28 17:55:32.000000 pazok-0.0.7/pazok/pazok.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:56:25.547845 pazok-0.0.7/pazok.egg-info/
+-rw-rw-rw-   0        0        0     1166 2024-05-28 17:56:25.000000 pazok-0.0.7/pazok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2024-05-28 17:56:25.000000 pazok-0.0.7/pazok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 17:56:25.000000 pazok-0.0.7/pazok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-28 17:56:25.000000 pazok-0.0.7/pazok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-28 17:56:25.000000 pazok-0.0.7/pazok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 17:56:25.551854 pazok-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      605 2024-05-28 17:55:57.000000 pazok-0.0.7/setup.py
```

### Comparing `pazok-0.0.6/PKG-INFO` & `pazok-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pazok
-Version: 0.0.6
+Version: 0.0.7
 Summary: A short description of my package
 Author: b_azo
 Author-email: husseun.selt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pazok Version: 0.0.6 Summary: A short description
+Metadata-Version: 2.1 Name: pazok Version: 0.0.7 Summary: A short description
 of my package Author: b_azo Author-email: husseun.selt@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
 Dist: requests
                               ************ ppaazzookk ************
 ### What is pazok? It is a python library that contains a set of ready-made
```

### Comparing `pazok-0.0.6/README.md` & `pazok-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pazok-0.0.6/pazok/__init__.py` & `pazok-0.0.7/pazok/__init__.py`

 * *Files identical despite different names*

### Comparing `pazok-0.0.6/pazok/pazok.py` & `pazok-0.0.7/pazok/pazok.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     from urllib.parse import unquote, urlparse
     import pyperclip
     from rich.console import Console
     from rich.syntax import Syntax
     from PIL import Image
     from fake_useragent import UserAgent
     from colorama import init, Fore, Back, Style
-
+    from asciimatics.renderers import ImageFile
 except:
     os.system("pip install argparse")
     os.system("pip install json")
     os.system("pip install locale")
     os.system("pip install re")
     os.system("pip install shlex")
     os.system("pip install collections")
@@ -35,15 +35,15 @@
     os.system("pip install python-cfonts")
     os.system("pip install pyTelegramBotAPI")
     os.system("pip install colorama")
     os.system("pip install requests")
     os.system("pip install threading")
     os.system("pip install random")
     os.system("pip install time")
-    
+    os.system("pip install asciimatics")
 
 #- - - - - - - - - - - - - - -- - - - - - -- - - - - #
 #لوكو
 def logo():
     o = "\u001b[38;5;208m"  # برتقالي
     e = "\u001b[38;5;242m"  # رمادي داكن
     logo=f"""
@@ -523,35 +523,45 @@
 #print(pazok.name_halo())
 
 
 #- - - - - - - - - - - - - - -- - - - - - -- - - - - #
 
 #تخويل الصور الى نقاط
 
-def picture(image_path, height=20):
-    import os
+def picture(image_path, height=None, style=None):
+    
     from PIL import Image, ImageOps
     from picharsso import new_drawer
+    from asciimatics.renderers import ImageFile
+    import io
     
-    pkg = ["picharsso"]
-    for lib in pkg:
-        try:
-            __import__(lib)
-            pass
-        except ImportError:
-            print(" جاري تثبيت المكاتب ،⬇️")
-            os.system(f"pip install {lib}")
-
     try:
         image = Image.open(image_path)
-        image = ImageOps.invert(image)
-        drawer = new_drawer("braille", height=height)
-        return drawer(image)
+        if image.mode != "RGB":
+            image = image.convert("RGB")
+        inverted_image = ImageOps.invert(image)
+        
+        if style == 1:
+            drawer = new_drawer("braille", height=height)
+            return drawer(inverted_image)
+        
+        elif style == 2:
+            with io.BytesIO() as output:
+                inverted_image.save(output, format="PNG")
+                output.seek(0)
+                renderer = ImageFile(output, height=height)
+                ascii_art = str(renderer)
+            return ascii_art    
+        else:
+            raise ValueError("النمط غير مدعوم. يرجى اختيار 1 أو 2.")   
     except FileNotFoundError:
         print("المسار غير صحيح:", image_path)
+    except Exception as e:
+        print("حدث خطأ:", e)
+
 
 #x="/storage/emulated/0/DCIM/100PINT/المنشورات/dbb76dbc7436ebe6defa7cd206103780.jpg"
 #z=30
 
 #jj=pazok.picture(x,z)
 #print(jj)
```

### Comparing `pazok-0.0.6/pazok.egg-info/PKG-INFO` & `pazok-0.0.7/pazok.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pazok
-Version: 0.0.6
+Version: 0.0.7
 Summary: A short description of my package
 Author: b_azo
 Author-email: husseun.selt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pazok Version: 0.0.6 Summary: A short description
+Metadata-Version: 2.1 Name: pazok Version: 0.0.7 Summary: A short description
 of my package Author: b_azo Author-email: husseun.selt@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
 Dist: requests
                               ************ ppaazzookk ************
 ### What is pazok? It is a python library that contains a set of ready-made
```

### Comparing `pazok-0.0.6/setup.py` & `pazok-0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pazok',
-    version='0.0.6',
+    version='0.0.7',
     author='b_azo',
     author_email='husseun.selt@gmail.com',
     description='A short description of my package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

