# Comparing `tmp/hsr_pic_parcer-1.0.2.tar.gz` & `tmp/hsr_pic_parcer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsr_pic_parcer-1.0.2.tar", last modified: Sun Apr 21 14:13:19 2024, max compression
+gzip compressed data, was "hsr_pic_parcer-1.0.3.tar", last modified: Wed May 29 09:08:28 2024, max compression
```

## Comparing `hsr_pic_parcer-1.0.2.tar` & `hsr_pic_parcer-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-21 14:13:19.033725 hsr_pic_parcer-1.0.2/
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1068 2024-02-22 20:53:45.000000 hsr_pic_parcer-1.0.2/LICENCE.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)     2571 2024-04-21 14:13:19.032725 hsr_pic_parcer-1.0.2/PKG-INFO
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1963 2024-04-21 14:11:00.000000 hsr_pic_parcer-1.0.2/README.md
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-21 14:13:19.031725 hsr_pic_parcer-1.0.2/hsr_pic_parcer.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)     2571 2024-04-21 14:13:18.000000 hsr_pic_parcer-1.0.2/hsr_pic_parcer.egg-info/PKG-INFO
--rw-r--r--   0 ivan      (1000) ivan      (1000)      454 2024-04-21 14:13:18.000000 hsr_pic_parcer-1.0.2/hsr_pic_parcer.egg-info/SOURCES.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)        1 2024-04-21 14:13:18.000000 hsr_pic_parcer-1.0.2/hsr_pic_parcer.egg-info/dependency_links.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)       40 2024-04-21 14:13:18.000000 hsr_pic_parcer-1.0.2/hsr_pic_parcer.egg-info/requires.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)       15 2024-04-21 14:13:18.000000 hsr_pic_parcer-1.0.2/hsr_pic_parcer.egg-info/top_level.txt
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-21 14:13:19.032725 hsr_pic_parcer-1.0.2/hsr_pic_parser/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      363 2024-04-21 14:03:29.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/__init__.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      332 2024-04-17 22:00:21.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/character_picture.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)       47 2024-02-22 20:53:45.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/cut_url.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-17 22:00:21.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/get_cone.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      933 2024-02-28 22:09:16.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/get_picture_info.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      187 2024-04-17 22:00:21.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/get_relic.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      173 2024-04-17 22:00:21.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/picture_url.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      842 2024-04-21 14:03:29.000000 hsr_pic_parcer-1.0.2/hsr_pic_parser/prydwen.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)       38 2024-04-21 14:13:19.033725 hsr_pic_parcer-1.0.2/setup.cfg
--rw-r--r--   0 ivan      (1000) ivan      (1000)      866 2024-04-21 14:13:13.000000 hsr_pic_parcer-1.0.2/setup.py
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-29 09:08:28.977181 hsr_pic_parcer-1.0.3/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1068 2024-02-22 20:53:45.000000 hsr_pic_parcer-1.0.3/LICENCE.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     2648 2024-05-29 09:08:28.976181 hsr_pic_parcer-1.0.3/PKG-INFO
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1970 2024-05-29 09:05:22.000000 hsr_pic_parcer-1.0.3/README.md
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-29 09:08:28.975181 hsr_pic_parcer-1.0.3/hsr_pic_parcer.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     2648 2024-05-29 09:08:28.000000 hsr_pic_parcer-1.0.3/hsr_pic_parcer.egg-info/PKG-INFO
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      454 2024-05-29 09:08:28.000000 hsr_pic_parcer-1.0.3/hsr_pic_parcer.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)        1 2024-05-29 09:08:28.000000 hsr_pic_parcer-1.0.3/hsr_pic_parcer.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       40 2024-05-29 09:08:28.000000 hsr_pic_parcer-1.0.3/hsr_pic_parcer.egg-info/requires.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       15 2024-05-29 09:08:28.000000 hsr_pic_parcer-1.0.3/hsr_pic_parcer.egg-info/top_level.txt
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-29 09:08:28.975181 hsr_pic_parcer-1.0.3/hsr_pic_parser/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      363 2024-04-21 14:03:29.000000 hsr_pic_parcer-1.0.3/hsr_pic_parser/__init__.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      332 2024-04-17 22:00:21.000000 hsr_pic_parcer-1.0.3/hsr_pic_parser/character_picture.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       47 2024-02-22 20:53:45.000000 hsr_pic_parcer-1.0.3/hsr_pic_parser/cut_url.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-17 22:00:21.000000 hsr_pic_parcer-1.0.3/hsr_pic_parser/get_cone.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      933 2024-02-28 22:09:16.000000 hsr_pic_parcer-1.0.3/hsr_pic_parser/get_picture_info.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      187 2024-04-17 22:00:21.000000 hsr_pic_parcer-1.0.3/hsr_pic_parser/get_relic.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      173 2024-04-17 22:00:21.000000 hsr_pic_parcer-1.0.3/hsr_pic_parser/picture_url.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      845 2024-05-29 09:08:13.000000 hsr_pic_parcer-1.0.3/hsr_pic_parser/prydwen.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       38 2024-05-29 09:08:28.977181 hsr_pic_parcer-1.0.3/setup.cfg
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      866 2024-05-29 09:03:55.000000 hsr_pic_parcer-1.0.3/setup.py
```

### Comparing `hsr_pic_parcer-1.0.2/LICENCE.txt` & `hsr_pic_parcer-1.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `hsr_pic_parcer-1.0.2/PKG-INFO` & `hsr_pic_parcer-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: hsr_pic_parcer
-Version: 1.0.2
+Version: 1.0.3
 Summary: parser to get images from hsr mana
 Home-page: https://github.com/vano979797/hsr_pic_parser
 Author: vano979797
 Author-email: vano979797@gmail.com
 Project-URL: Documentation, https://github.com/vano979797/hsr_pic_parser/blob/4a0309d617f93c56714fe206753119f690109219/README.md
 Keywords: python parse hsr
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
+Requires-Dist: requests>=2.25.1
+Requires-Dist: beautifulsoup4>=4.12.3
 
 # hsr_pic_parser
 
 ## Introduction
 
 This is a Python library for getting pictures of characters, light cones, relics and planetaries with names from [starrail.mana](https://starrail.mana.wiki/).
 
@@ -66,14 +68,14 @@
 def save_image_as_png(image_data, output_file_path):
     with open(output_file_path, "wb") as png_file:
         png_file.write(image_data)
 
 save_image_as_png(picture, f"${name}.png")
 ```
 
-You can get the name and the picture of the charater from prydwen [prydwen.gg](https://www.prydwen.gg/star-rail/characters/).
+You can get the name and the picture of the charater from prydwen [prydwen.gg](https://www.prydwen.gg/star-rail/characters/) by URL.
 
 ```python
 from hsr_pic_parser import get_character_prydwen
 
 picture, name = get_character_prydwen('argenti')
 ```
```

### Comparing `hsr_pic_parcer-1.0.2/README.md` & `hsr_pic_parcer-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,14 @@
 def save_image_as_png(image_data, output_file_path):
     with open(output_file_path, "wb") as png_file:
         png_file.write(image_data)
 
 save_image_as_png(picture, f"${name}.png")
 ```
 
-You can get the name and the picture of the charater from prydwen [prydwen.gg](https://www.prydwen.gg/star-rail/characters/).
+You can get the name and the picture of the charater from prydwen [prydwen.gg](https://www.prydwen.gg/star-rail/characters/) by URL.
 
 ```python
 from hsr_pic_parser import get_character_prydwen
 
 picture, name = get_character_prydwen('argenti')
 ```
```

### Comparing `hsr_pic_parcer-1.0.2/hsr_pic_parcer.egg-info/PKG-INFO` & `hsr_pic_parcer-1.0.3/hsr_pic_parcer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
-Name: hsr-pic-parcer
-Version: 1.0.2
+Name: hsr_pic_parcer
+Version: 1.0.3
 Summary: parser to get images from hsr mana
 Home-page: https://github.com/vano979797/hsr_pic_parser
 Author: vano979797
 Author-email: vano979797@gmail.com
 Project-URL: Documentation, https://github.com/vano979797/hsr_pic_parser/blob/4a0309d617f93c56714fe206753119f690109219/README.md
 Keywords: python parse hsr
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
+Requires-Dist: requests>=2.25.1
+Requires-Dist: beautifulsoup4>=4.12.3
 
 # hsr_pic_parser
 
 ## Introduction
 
 This is a Python library for getting pictures of characters, light cones, relics and planetaries with names from [starrail.mana](https://starrail.mana.wiki/).
 
@@ -66,14 +68,14 @@
 def save_image_as_png(image_data, output_file_path):
     with open(output_file_path, "wb") as png_file:
         png_file.write(image_data)
 
 save_image_as_png(picture, f"${name}.png")
 ```
 
-You can get the name and the picture of the charater from prydwen [prydwen.gg](https://www.prydwen.gg/star-rail/characters/).
+You can get the name and the picture of the charater from prydwen [prydwen.gg](https://www.prydwen.gg/star-rail/characters/) by URL.
 
 ```python
 from hsr_pic_parser import get_character_prydwen
 
 picture, name = get_character_prydwen('argenti')
 ```
```

### Comparing `hsr_pic_parcer-1.0.2/hsr_pic_parser/get_picture_info.py` & `hsr_pic_parcer-1.0.3/hsr_pic_parser/get_picture_info.py`

 * *Files identical despite different names*

### Comparing `hsr_pic_parcer-1.0.2/hsr_pic_parser/prydwen.py` & `hsr_pic_parcer-1.0.3/hsr_pic_parser/prydwen.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from bs4 import BeautifulSoup
 import requests
 
 
 def get_character_prydwen(name):
-    response = requests.get('https://www.prydwen.gg/star-rail/characters')
+    response = requests.get('https://www.prydwen.gg/star-rail/characters' + '/' + name)
 
     if response.status_code == 200:
         html_content = response.content
         soup = BeautifulSoup(html_content, 'html.parser')
 
         pictures = soup.find_all('img')
         for picture in pictures:
-            if picture['alt'].lower() == name.lower():
+            if picture['alt'] == "Character":
                 pic_url = "https://www.prydwen.gg"+ picture['data-src']
                 maybe_pic = requests.get(pic_url)
                 if maybe_pic.status_code == 200:
                     return maybe_pic.content, name
                 else:
                     print('Error loading the image:', maybe_pic.status_code)
     elif response.status_code == 500:
-        print('Error loading the page:', response.status_code)
+        print('Error loading the page:', response.status_code)
```

### Comparing `hsr_pic_parcer-1.0.2/setup.py` & `hsr_pic_parcer-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='hsr_pic_parcer',
-  version='1.0.2',
+  version='1.0.3',
   author='vano979797',
   author_email='vano979797@gmail.com',
   description='parser to get images from hsr mana',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/vano979797/hsr_pic_parser',
   packages=find_packages(),
```

