# Comparing `tmp/django-sass-processor-1.4.tar.gz` & `tmp/django_sass_processor-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sass-processor-1.4.tar", last modified: Tue Dec 12 10:27:48 2023, max compression
+gzip compressed data, was "django_sass_processor-1.4.1.tar", last modified: Wed May 29 13:59:50 2024, max compression
```

## Comparing `django-sass-processor-1.4.tar` & `django_sass_processor-1.4.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 10:27:48.442618 django-sass-processor-1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2023-12-12 10:27:39.000000 django-sass-processor-1.4/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-12 10:27:39.000000 django-sass-processor-1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19088 2023-12-12 10:27:48.442618 django-sass-processor-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17873 2023-12-12 10:27:39.000000 django-sass-processor-1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 10:27:48.438618 django-sass-processor-1.4/django_sass_processor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19088 2023-12-12 10:27:48.000000 django-sass-processor-1.4/django_sass_processor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-12-12 10:27:48.000000 django-sass-processor-1.4/django_sass_processor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 10:27:48.000000 django-sass-processor-1.4/django_sass_processor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 10:27:48.000000 django-sass-processor-1.4/django_sass_processor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-12 10:27:48.000000 django-sass-processor-1.4/django_sass_processor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-12 10:27:48.000000 django-sass-processor-1.4/django_sass_processor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 10:27:48.438618 django-sass-processor-1.4/sass_processor/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-12-12 10:27:39.000000 django-sass-processor-1.4/sass_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-12-12 10:27:39.000000 django-sass-processor-1.4/sass_processor/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2023-12-12 10:27:39.000000 django-sass-processor-1.4/sass_processor/finders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 10:27:48.438618 django-sass-processor-1.4/sass_processor/jinja2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 10:27:39.000000 django-sass-processor-1.4/sass_processor/jinja2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-12 10:27:39.000000 django-sass-processor-1.4/sass_processor/jinja2/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 10:27:48.438618 django-sass-processor-1.4/sass_processor/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 10:27:39.000000 django-sass-processor-1.4/sass_processor/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 10:27:48.438618 django-sass-processor-1.4/sass_processor/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 10:27:39.000000 django-sass-processor-1.4/sass_processor/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14194 2023-12-12 10:27:39.000000 django-sass-processor-1.4/sass_processor/management/commands/compilescss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2023-12-12 10:27:39.000000 django-sass-processor-1.4/sass_processor/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-12-12 10:27:39.000000 django-sass-processor-1.4/sass_processor/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 10:27:48.438618 django-sass-processor-1.4/sass_processor/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 10:27:39.000000 django-sass-processor-1.4/sass_processor/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-12-12 10:27:39.000000 django-sass-processor-1.4/sass_processor/templatetags/sass_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-12-12 10:27:39.000000 django-sass-processor-1.4/sass_processor/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-12-12 10:27:39.000000 django-sass-processor-1.4/sass_processor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-12 10:27:48.442618 django-sass-processor-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-12 10:27:39.000000 django-sass-processor-1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 10:27:48.438618 django-sass-processor-1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-12 10:27:39.000000 django-sass-processor-1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-12 10:27:39.000000 django-sass-processor-1.4/tests/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2023-12-12 10:27:39.000000 django-sass-processor-1.4/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2023-12-12 10:27:39.000000 django-sass-processor-1.4/tests/test_sass_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:59:50.680028 django_sass_processor-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18912 2024-05-29 13:59:50.680028 django_sass_processor-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17695 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:59:50.680028 django_sass_processor-1.4.1/django_sass_processor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18912 2024-05-29 13:59:50.000000 django_sass_processor-1.4.1/django_sass_processor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-29 13:59:50.000000 django_sass_processor-1.4.1/django_sass_processor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:59:50.000000 django_sass_processor-1.4.1/django_sass_processor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:59:50.000000 django_sass_processor-1.4.1/django_sass_processor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-29 13:59:50.000000 django_sass_processor-1.4.1/django_sass_processor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 13:59:50.000000 django_sass_processor-1.4.1/django_sass_processor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:59:50.676028 django_sass_processor-1.4.1/sass_processor/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/sass_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/sass_processor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/sass_processor/finders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:59:50.676028 django_sass_processor-1.4.1/sass_processor/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/sass_processor/jinja2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/sass_processor/jinja2/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:59:50.676028 django_sass_processor-1.4.1/sass_processor/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/sass_processor/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:59:50.676028 django_sass_processor-1.4.1/sass_processor/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/sass_processor/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14219 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/sass_processor/management/commands/compilescss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/sass_processor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/sass_processor/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:59:50.676028 django_sass_processor-1.4.1/sass_processor/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/sass_processor/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/sass_processor/templatetags/sass_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/sass_processor/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/sass_processor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-29 13:59:50.680028 django_sass_processor-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:59:50.676028 django_sass_processor-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/tests/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-29 13:59:47.000000 django_sass_processor-1.4.1/tests/test_sass_processor.py
```

### Comparing `django-sass-processor-1.4/LICENSE-MIT` & `django_sass_processor-1.4.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `django-sass-processor-1.4/PKG-INFO` & `django_sass_processor-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sass-processor
-Version: 1.4
+Version: 1.4.1
 Summary: SASS processor to compile SCSS files into *.css, while rendering, or offline.
 Home-page: https://github.com/jrief/django-sass-processor
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: django,sass
 Classifier: Development Status :: 5 - Production/Stable
@@ -516,13 +516,7 @@
 
 ```shell
 python -m pip install --upgrade pip
 pip install Django
 pip install -r tests/requirements.txt
 python -m pytest tests
 ```
-
-
-## Third Party Documentation
-
-Brian wrote a nice artice on
-[how to easily use SASS/SCSS with Django](https://engineertodeveloper.com/how-to-easily-use-sass-scss-with-django/).
```

### Comparing `django-sass-processor-1.4/README.md` & `django_sass_processor-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -486,13 +486,7 @@
 
 ```shell
 python -m pip install --upgrade pip
 pip install Django
 pip install -r tests/requirements.txt
 python -m pytest tests
 ```
-
-
-## Third Party Documentation
-
-Brian wrote a nice artice on
-[how to easily use SASS/SCSS with Django](https://engineertodeveloper.com/how-to-easily-use-sass-scss-with-django/).
```

### Comparing `django-sass-processor-1.4/django_sass_processor.egg-info/PKG-INFO` & `django_sass_processor-1.4.1/django_sass_processor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sass-processor
-Version: 1.4
+Version: 1.4.1
 Summary: SASS processor to compile SCSS files into *.css, while rendering, or offline.
 Home-page: https://github.com/jrief/django-sass-processor
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: django,sass
 Classifier: Development Status :: 5 - Production/Stable
@@ -516,13 +516,7 @@
 
 ```shell
 python -m pip install --upgrade pip
 pip install Django
 pip install -r tests/requirements.txt
 python -m pytest tests
 ```
-
-
-## Third Party Documentation
-
-Brian wrote a nice artice on
-[how to easily use SASS/SCSS with Django](https://engineertodeveloper.com/how-to-easily-use-sass-scss-with-django/).
```

### Comparing `django-sass-processor-1.4/django_sass_processor.egg-info/SOURCES.txt` & `django_sass_processor-1.4.1/django_sass_processor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-sass-processor-1.4/sass_processor/__init__.py` & `django_sass_processor-1.4.1/sass_processor/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 10. bump the version, append ".dev0" to __version__
 11. Add a new heading to README.md / Changelog, named "<next-version>.dev"
 12. git add sass_processor/__init__.py README.md
 12. git commit -m 'Start with <version>'
 13. git push
 """
 
-__version__ = '1.4'
+__version__ = '1.4.1'
```

### Comparing `django-sass-processor-1.4/sass_processor/apps.py` & `django_sass_processor-1.4.1/sass_processor/apps.py`

 * *Files identical despite different names*

### Comparing `django-sass-processor-1.4/sass_processor/finders.py` & `django_sass_processor-1.4.1/sass_processor/finders.py`

 * *Files identical despite different names*

### Comparing `django-sass-processor-1.4/sass_processor/jinja2/ext.py` & `django_sass_processor-1.4.1/sass_processor/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `django-sass-processor-1.4/sass_processor/management/commands/compilescss.py` & `django_sass_processor-1.4.1/sass_processor/management/commands/compilescss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 
 import ast
 from importlib import import_module
 import sass
 from compressor.exceptions import TemplateDoesNotExist, TemplateSyntaxError
+from pathlib import Path
 
 from django.apps import apps
 from django.conf import settings
 from django.core.files.base import ContentFile
 from django.core.management.base import BaseCommand, CommandError
 from django.template import engines
 from django.template.base import Origin
@@ -196,15 +197,15 @@
 
     def parse_source(self, filename):
         """
         Extract the statements from the given file, look for function calls
         `sass_processor(scss_file)` and compile the filename into CSS.
         """
         callvisitor = FuncCallVisitor('sass_processor')
-        tree = ast.parse(open(filename, 'rb').read())
+        tree = ast.parse(Path(filename).read_bytes())
         callvisitor.visit(tree)
         for sass_fileurl in callvisitor.sass_files:
             sass_filename = find_file(sass_fileurl)
             if not sass_filename or sass_filename in self.processed_files:
                 continue
             if self.delete_files:
                 self.delete_file(sass_filename, sass_fileurl)
```

### Comparing `django-sass-processor-1.4/sass_processor/processor.py` & `django_sass_processor-1.4.1/sass_processor/processor.py`

 * *Files identical despite different names*

### Comparing `django-sass-processor-1.4/sass_processor/storage.py` & `django_sass_processor-1.4.1/sass_processor/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django import VERSION
 from django.conf import settings
 from django.contrib.staticfiles.finders import get_finders
-from django.core.files.storage import FileSystemStorage, get_storage_class
+from django.core.files.storage import FileSystemStorage
 from django.utils.functional import LazyObject
 from django.utils.module_loading import import_string
 
 
 class SassFileStorage(LazyObject):
     def _setup(self):
         version_parts = VERSION[:2]
@@ -13,14 +13,15 @@
             staticfiles_storage_backend = settings.STORAGES.get("staticfiles", {}).get("BACKEND")
             sass_processor_storage = settings.STORAGES.get("sass_processor", {})
 
             storage_path = sass_processor_storage.get("BACKEND") or staticfiles_storage_backend
             storage_options = sass_processor_storage.get("OPTIONS") or {}
             storage_class = import_string(storage_path)
         else:
+            from django.core.files.storage import get_storage_class
             staticfiles_storage_backend = settings.STATICFILES_STORAGE
             storage_path = getattr(settings, 'SASS_PROCESSOR_STORAGE', staticfiles_storage_backend)
             storage_options = getattr(settings, 'SASS_PROCESSOR_STORAGE_OPTIONS', {})
             storage_class = get_storage_class(storage_path)
 
             storage_options["ROOT"] = getattr(settings, 'SASS_PROCESSOR_ROOT', settings.STATIC_ROOT)
```

### Comparing `django-sass-processor-1.4/sass_processor/templatetags/sass_tags.py` & `django_sass_processor-1.4.1/sass_processor/templatetags/sass_tags.py`

 * *Files identical despite different names*

### Comparing `django-sass-processor-1.4/sass_processor/utils.py` & `django_sass_processor-1.4.1/sass_processor/utils.py`

 * *Files identical despite different names*

### Comparing `django-sass-processor-1.4/setup.cfg` & `django_sass_processor-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-sass-processor-1.4/tests/settings.py` & `django_sass_processor-1.4.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-sass-processor-1.4/tests/test_sass_processor.py` & `django_sass_processor-1.4.1/tests/test_sass_processor.py`

 * *Files identical despite different names*

