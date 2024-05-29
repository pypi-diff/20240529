# Comparing `tmp/django_img_optimizer-1.2.tar.gz` & `tmp/django_img_optimizer-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_img_optimizer-1.2.tar", last modified: Wed Apr 24 05:46:28 2024, max compression
+gzip compressed data, was "django_img_optimizer-1.3.tar", last modified: Wed May 29 03:17:39 2024, max compression
```

## Comparing `django_img_optimizer-1.2.tar` & `django_img_optimizer-1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/django_img_optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/django_img_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/django_img_optimizer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/django_img_optimizer/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/django_img_optimizer/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/django_img_optimizer/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/django_img_optimizer/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/django_img_optimizer/management/commands/optimize_images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/django_img_optimizer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/django_img_optimizer/templatetags/image_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/django_img_optimizer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/django_img_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-24 05:46:28.000000 django_img_optimizer-1.2/django_img_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-24 05:46:28.000000 django_img_optimizer-1.2/django_img_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 05:46:28.000000 django_img_optimizer-1.2/django_img_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 05:46:28.000000 django_img_optimizer-1.2/django_img_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 05:46:28.000000 django_img_optimizer-1.2/django_img_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:46:28.484740 django_img_optimizer-1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-24 05:46:19.000000 django_img_optimizer-1.2/tests/test_build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:17:39.815988 django_img_optimizer-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 03:17:30.000000 django_img_optimizer-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-29 03:17:39.815988 django_img_optimizer-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-29 03:17:30.000000 django_img_optimizer-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:17:39.815988 django_img_optimizer-1.3/django_img_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:17:30.000000 django_img_optimizer-1.3/django_img_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-29 03:17:30.000000 django_img_optimizer-1.3/django_img_optimizer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:17:39.815988 django_img_optimizer-1.3/django_img_optimizer/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:17:30.000000 django_img_optimizer-1.3/django_img_optimizer/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:17:39.815988 django_img_optimizer-1.3/django_img_optimizer/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:17:30.000000 django_img_optimizer-1.3/django_img_optimizer/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-29 03:17:30.000000 django_img_optimizer-1.3/django_img_optimizer/management/commands/optimize_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:17:39.815988 django_img_optimizer-1.3/django_img_optimizer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-29 03:17:30.000000 django_img_optimizer-1.3/django_img_optimizer/templatetags/image_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-29 03:17:30.000000 django_img_optimizer-1.3/django_img_optimizer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:17:39.815988 django_img_optimizer-1.3/django_img_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-29 03:17:39.000000 django_img_optimizer-1.3/django_img_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-29 03:17:39.000000 django_img_optimizer-1.3/django_img_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:17:39.000000 django_img_optimizer-1.3/django_img_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 03:17:39.000000 django_img_optimizer-1.3/django_img_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 03:17:39.000000 django_img_optimizer-1.3/django_img_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-29 03:17:30.000000 django_img_optimizer-1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 03:17:39.815988 django_img_optimizer-1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:17:39.815988 django_img_optimizer-1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-29 03:17:30.000000 django_img_optimizer-1.3/tests/test_build.py
```

### Comparing `django_img_optimizer-1.2/LICENSE` & `django_img_optimizer-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_img_optimizer-1.2/PKG-INFO` & `django_img_optimizer-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-img-optimizer
-Version: 1.2
+Version: 1.3
 Summary: Image optimizer for Django.
 Author: Peter Stavrou
 License: MIT
 Project-URL: Homepage, https://github.com/peterstavrou/django-img-optimizer
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pillow>=10.2.0
 
 # Django Image Optimizer
 
-[![pytest](https://github.com/peterstavrou/django-img-optimizer/actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-img-optimizer/actions) &nbsp; [![pypi](https://img.shields.io/badge/dynamic/toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)](https://pypi.org/project/django-img-optimizer/1.2/)  &nbsp; [![mit-license](https://img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/django-img-optimizer/blob/main/LICENSE)
+[![pytest](https://github.com/peterstavrou/django-img-optimizer/actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-img-optimizer/actions) &nbsp; [![pypi](https://img.shields.io/badge/dynamic/toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)](https://pypi.org/project/django-img-optimizer/1.3/)  &nbsp; [![mit-license](https://img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/django-img-optimizer/blob/main/LICENSE)
 
 Django Image Optimizer converts images to WebP format while allowing you to specify the quality of the image. Optimized images that are larger than their originals are automatically deleted.
 
 ## Installation
     pip install django-img-optimizer
 
 ## Configuration
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: django-img-optimizer Version: 1.2 Summary: Image
+Metadata-Version: 2.1 Name: django-img-optimizer Version: 1.3 Summary: Image
 optimizer for Django. Author: Peter Stavrou License: MIT Project-URL: Homepage,
 https://github.com/peterstavrou/django-img-optimizer Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pillow>=10.2.0 # Django Image
 Optimizer [![pytest](https://github.com/peterstavrou/django-img-optimizer/
 actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-
 img-optimizer/actions)   [![pypi](https://img.shields.io/badge/dynamic/
 toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/
 main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)]
-(https://pypi.org/project/django-img-optimizer/1.2/)   [![mit-license](https://
+(https://pypi.org/project/django-img-optimizer/1.3/)   [![mit-license](https://
 img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/
 django-img-optimizer/blob/main/LICENSE) Django Image Optimizer converts images
 to WebP format while allowing you to specify the quality of the image.
 Optimized images that are larger than their originals are automatically
 deleted. ## Installation pip install django-img-optimizer ## Configuration Add
 django_img_optimizer to `INSTALLED_APPS` in your projects `settings.py` file:
 ``` INSTALLED_APPS = [ ... 'django_img_optimizer', ... ] ``` Set
```

### Comparing `django_img_optimizer-1.2/README.md` & `django_img_optimizer-1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Django Image Optimizer
 
-[![pytest](https://github.com/peterstavrou/django-img-optimizer/actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-img-optimizer/actions) &nbsp; [![pypi](https://img.shields.io/badge/dynamic/toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)](https://pypi.org/project/django-img-optimizer/1.2/)  &nbsp; [![mit-license](https://img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/django-img-optimizer/blob/main/LICENSE)
+[![pytest](https://github.com/peterstavrou/django-img-optimizer/actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-img-optimizer/actions) &nbsp; [![pypi](https://img.shields.io/badge/dynamic/toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)](https://pypi.org/project/django-img-optimizer/1.3/)  &nbsp; [![mit-license](https://img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/django-img-optimizer/blob/main/LICENSE)
 
 Django Image Optimizer converts images to WebP format while allowing you to specify the quality of the image. Optimized images that are larger than their originals are automatically deleted.
 
 ## Installation
     pip install django-img-optimizer
 
 ## Configuration
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # Django Image Optimizer [![pytest](https://github.com/peterstavrou/django-img-
 optimizer/actions/workflows/build.yml/badge.svg)](https://github.com/
 peterstavrou/django-img-optimizer/actions)   [![pypi](https://img.shields.io/
 badge/dynamic/toml?url=https://raw.githubusercontent.com/peterstavrou/django-
 img-optimizer/main/
 pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)](https://
-pypi.org/project/django-img-optimizer/1.2/)   [![mit-license](https://
+pypi.org/project/django-img-optimizer/1.3/)   [![mit-license](https://
 img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/
 django-img-optimizer/blob/main/LICENSE) Django Image Optimizer converts images
 to WebP format while allowing you to specify the quality of the image.
 Optimized images that are larger than their originals are automatically
 deleted. ## Installation pip install django-img-optimizer ## Configuration Add
 django_img_optimizer to `INSTALLED_APPS` in your projects `settings.py` file:
 ``` INSTALLED_APPS = [ ... 'django_img_optimizer', ... ] ``` Set
```

### Comparing `django_img_optimizer-1.2/django_img_optimizer/management/commands/optimize_images.py` & `django_img_optimizer-1.3/django_img_optimizer/management/commands/optimize_images.py`

 * *Files identical despite different names*

### Comparing `django_img_optimizer-1.2/django_img_optimizer/templatetags/image_optimizer.py` & `django_img_optimizer-1.3/django_img_optimizer/templatetags/image_optimizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     Args:
         *args: Variable number of arguments representing the attributes for the image tag.
     """
     attributes = ' '.join(args)
 
     # Get src attribute value
     match_src = re.search(r'src="([^"]+)"', attributes)
-    # print(match_src)
-    # print('************')
     relative_image_path = match_src.group(1) if match_src.group(1) is not None else "src could not be found"
 
     # Get django static path
     image_static_src = static(relative_image_path)
 
     # Replace src in attributes with django static src
     attributes_output = re.sub(r'(src=")([^"]+)(")(?=\s|>)', fr'\g<1>{image_static_src}\g<3>', attributes)
```

### Comparing `django_img_optimizer-1.2/django_img_optimizer/utils.py` & `django_img_optimizer-1.3/django_img_optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `django_img_optimizer-1.2/django_img_optimizer.egg-info/PKG-INFO` & `django_img_optimizer-1.3/django_img_optimizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-img-optimizer
-Version: 1.2
+Version: 1.3
 Summary: Image optimizer for Django.
 Author: Peter Stavrou
 License: MIT
 Project-URL: Homepage, https://github.com/peterstavrou/django-img-optimizer
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pillow>=10.2.0
 
 # Django Image Optimizer
 
-[![pytest](https://github.com/peterstavrou/django-img-optimizer/actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-img-optimizer/actions) &nbsp; [![pypi](https://img.shields.io/badge/dynamic/toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)](https://pypi.org/project/django-img-optimizer/1.2/)  &nbsp; [![mit-license](https://img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/django-img-optimizer/blob/main/LICENSE)
+[![pytest](https://github.com/peterstavrou/django-img-optimizer/actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-img-optimizer/actions) &nbsp; [![pypi](https://img.shields.io/badge/dynamic/toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)](https://pypi.org/project/django-img-optimizer/1.3/)  &nbsp; [![mit-license](https://img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/django-img-optimizer/blob/main/LICENSE)
 
 Django Image Optimizer converts images to WebP format while allowing you to specify the quality of the image. Optimized images that are larger than their originals are automatically deleted.
 
 ## Installation
     pip install django-img-optimizer
 
 ## Configuration
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: django-img-optimizer Version: 1.2 Summary: Image
+Metadata-Version: 2.1 Name: django-img-optimizer Version: 1.3 Summary: Image
 optimizer for Django. Author: Peter Stavrou License: MIT Project-URL: Homepage,
 https://github.com/peterstavrou/django-img-optimizer Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pillow>=10.2.0 # Django Image
 Optimizer [![pytest](https://github.com/peterstavrou/django-img-optimizer/
 actions/workflows/build.yml/badge.svg)](https://github.com/peterstavrou/django-
 img-optimizer/actions)   [![pypi](https://img.shields.io/badge/dynamic/
 toml?url=https://raw.githubusercontent.com/peterstavrou/django-img-optimizer/
 main/pyproject.toml&prefix=v&query=project.version&label=pypi&color=blue)]
-(https://pypi.org/project/django-img-optimizer/1.2/)   [![mit-license](https://
+(https://pypi.org/project/django-img-optimizer/1.3/)   [![mit-license](https://
 img.shields.io/badge/license-MIT-9d9d9d)](https://github.com/peterstavrou/
 django-img-optimizer/blob/main/LICENSE) Django Image Optimizer converts images
 to WebP format while allowing you to specify the quality of the image.
 Optimized images that are larger than their originals are automatically
 deleted. ## Installation pip install django-img-optimizer ## Configuration Add
 django_img_optimizer to `INSTALLED_APPS` in your projects `settings.py` file:
 ``` INSTALLED_APPS = [ ... 'django_img_optimizer', ... ] ``` Set
```

### Comparing `django_img_optimizer-1.2/django_img_optimizer.egg-info/SOURCES.txt` & `django_img_optimizer-1.3/django_img_optimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_img_optimizer-1.2/tests/test_build.py` & `django_img_optimizer-1.3/tests/test_build.py`

 * *Files identical despite different names*

