# Comparing `tmp/django_lookbook-0.0.1.tar.gz` & `tmp/django_lookbook-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_lookbook-0.0.1.tar", max compression
+gzip compressed data, was "django_lookbook-0.0.2.tar", max compression
```

## Comparing `django_lookbook-0.0.1.tar` & `django_lookbook-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        9 2024-05-28 02:42:41.342461 django_lookbook-0.0.1/README.md
--rw-r--r--   0        0        0      659 2024-05-29 08:33:10.691211 django_lookbook-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-28 06:33:19.067612 django_lookbook-0.0.1/src/django_lookbook/__init__.py
--rw-r--r--   0        0        0       98 2024-05-28 06:31:27.795446 django_lookbook-0.0.1/src/django_lookbook/apps.py
--rw-r--r--   0        0        0      146 2024-03-28 02:17:08.521000 django_lookbook-0.0.1/src/django_lookbook/fields.py
--rw-r--r--   0        0        0    69287 2024-05-29 08:57:35.246686 django_lookbook-0.0.1/src/django_lookbook/static/lookbook/css/app.css
--rw-r--r--   0        0        0    20024 2024-05-29 08:57:35.248394 django_lookbook-0.0.1/src/django_lookbook/static/lookbook/css/app.css.map
--rw-r--r--   0        0        0  1192399 2024-05-29 08:57:35.247100 django_lookbook-0.0.1/src/django_lookbook/static/lookbook/js/app.js
--rw-r--r--   0        0        0      124 2024-05-29 08:57:35.247204 django_lookbook-0.0.1/src/django_lookbook/static/lookbook/js/app.js.LICENSE.txt
--rw-r--r--   0        0        0  3030414 2024-05-29 08:57:35.247992 django_lookbook-0.0.1/src/django_lookbook/static/lookbook/js/app.js.map
--rw-r--r--   0        0        0      742 2024-05-29 08:57:35.251057 django_lookbook-0.0.1/src/django_lookbook/static/lookbook/manifest.json
--rw-r--r--   0        0        0        0 2024-05-29 08:57:35.246301 django_lookbook-0.0.1/src/django_lookbook/static/lookbook/vendors/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-29 08:57:35.247453 django_lookbook-0.0.1/src/django_lookbook/static/lookbook/vendors/images/.gitkeep
--rw-r--r--   0        0        0   330309 2024-05-29 08:57:35.248333 django_lookbook-0.0.1/src/django_lookbook/static/lookbook/vendors/images/lucide-sprite.svg
--rw-r--r--   0        0        0   273404 2024-05-29 08:57:35.248134 django_lookbook-0.0.1/src/django_lookbook/static/lookbook/vendors/images/sample.jpg
--rw-r--r--   0        0        0   238213 2024-05-29 08:57:35.248571 django_lookbook-0.0.1/src/django_lookbook/static/lookbook/vendors/images/webpack.png
--rw-r--r--   0        0        0     1923 2024-05-29 03:28:35.924344 django_lookbook-0.0.1/src/django_lookbook/templates/django_lookbook/base.html
--rw-r--r--   0        0        0      857 2024-05-25 03:38:05.374000 django_lookbook-0.0.1/src/django_lookbook/templates/django_lookbook/fields/toggle_switch_widget.html
--rw-r--r--   0        0        0     2647 2024-05-29 03:29:10.626926 django_lookbook-0.0.1/src/django_lookbook/templates/django_lookbook/includes/sidebar_2_level.html
--rw-r--r--   0        0        0     4795 2024-05-29 03:29:10.631141 django_lookbook-0.0.1/src/django_lookbook/templates/django_lookbook/includes/sidebar_3_level.html
--rw-r--r--   0        0        0     1849 2024-05-29 03:29:10.623573 django_lookbook-0.0.1/src/django_lookbook/templates/django_lookbook/includes/sidebar_previews.html
--rw-r--r--   0        0        0     2663 2024-05-29 03:53:42.275278 django_lookbook-0.0.1/src/django_lookbook/templates/django_lookbook/index.html
--rw-r--r--   0        0        0     9751 2024-05-29 03:29:10.634921 django_lookbook-0.0.1/src/django_lookbook/templates/django_lookbook/inspect.html
--rw-r--r--   0        0        0      305 2024-05-29 02:55:07.292390 django_lookbook-0.0.1/src/django_lookbook/urls.py
--rw-r--r--   0        0        0      141 2024-03-28 02:17:08.522000 django_lookbook-0.0.1/src/django_lookbook/utils.py
--rw-r--r--   0        0        0     6405 2024-05-29 03:25:01.073894 django_lookbook-0.0.1/src/django_lookbook/views.py
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 django_lookbook-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        9 2024-05-29 09:19:02.228446 django_lookbook-0.0.2/README.md
+-rw-r--r--   0        0        0      659 2024-05-29 09:19:02.244446 django_lookbook-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 09:19:02.244446 django_lookbook-0.0.2/src/django_lookbook/__init__.py
+-rw-r--r--   0        0        0       98 2024-05-29 09:19:02.244446 django_lookbook-0.0.2/src/django_lookbook/apps.py
+-rw-r--r--   0        0        0      146 2024-05-29 09:19:02.244446 django_lookbook-0.0.2/src/django_lookbook/fields.py
+-rw-r--r--   0        0        0    69287 2024-05-29 09:19:02.244446 django_lookbook-0.0.2/src/django_lookbook/static/lookbook/css/app.css
+-rw-r--r--   0        0        0    20024 2024-05-29 09:19:02.244446 django_lookbook-0.0.2/src/django_lookbook/static/lookbook/css/app.css.map
+-rw-r--r--   0        0        0  1192399 2024-05-29 09:19:02.252446 django_lookbook-0.0.2/src/django_lookbook/static/lookbook/js/app.js
+-rw-r--r--   0        0        0      124 2024-05-29 09:19:02.252446 django_lookbook-0.0.2/src/django_lookbook/static/lookbook/js/app.js.LICENSE.txt
+-rw-r--r--   0        0        0  3030414 2024-05-29 09:19:02.264446 django_lookbook-0.0.2/src/django_lookbook/static/lookbook/js/app.js.map
+-rw-r--r--   0        0        0      742 2024-05-29 09:19:02.264446 django_lookbook-0.0.2/src/django_lookbook/static/lookbook/manifest.json
+-rw-r--r--   0        0        0        0 2024-05-29 09:19:02.264446 django_lookbook-0.0.2/src/django_lookbook/static/lookbook/vendors/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-29 09:19:02.264446 django_lookbook-0.0.2/src/django_lookbook/static/lookbook/vendors/images/.gitkeep
+-rw-r--r--   0        0        0   330309 2024-05-29 09:19:02.268446 django_lookbook-0.0.2/src/django_lookbook/static/lookbook/vendors/images/lucide-sprite.svg
+-rw-r--r--   0        0        0   273404 2024-05-29 09:19:02.268446 django_lookbook-0.0.2/src/django_lookbook/static/lookbook/vendors/images/sample.jpg
+-rw-r--r--   0        0        0   238213 2024-05-29 09:19:02.268446 django_lookbook-0.0.2/src/django_lookbook/static/lookbook/vendors/images/webpack.png
+-rw-r--r--   0        0        0     1923 2024-05-29 09:19:02.268446 django_lookbook-0.0.2/src/django_lookbook/templates/django_lookbook/base.html
+-rw-r--r--   0        0        0      857 2024-05-29 09:19:02.268446 django_lookbook-0.0.2/src/django_lookbook/templates/django_lookbook/fields/toggle_switch_widget.html
+-rw-r--r--   0        0        0     2647 2024-05-29 09:19:02.268446 django_lookbook-0.0.2/src/django_lookbook/templates/django_lookbook/includes/sidebar_2_level.html
+-rw-r--r--   0        0        0     4795 2024-05-29 09:19:02.268446 django_lookbook-0.0.2/src/django_lookbook/templates/django_lookbook/includes/sidebar_3_level.html
+-rw-r--r--   0        0        0     1849 2024-05-29 09:19:02.268446 django_lookbook-0.0.2/src/django_lookbook/templates/django_lookbook/includes/sidebar_previews.html
+-rw-r--r--   0        0        0     2663 2024-05-29 09:19:02.268446 django_lookbook-0.0.2/src/django_lookbook/templates/django_lookbook/index.html
+-rw-r--r--   0        0        0     9751 2024-05-29 09:19:02.268446 django_lookbook-0.0.2/src/django_lookbook/templates/django_lookbook/inspect.html
+-rw-r--r--   0        0        0      305 2024-05-29 09:19:02.268446 django_lookbook-0.0.2/src/django_lookbook/urls.py
+-rw-r--r--   0        0        0      141 2024-05-29 09:19:02.268446 django_lookbook-0.0.2/src/django_lookbook/utils.py
+-rw-r--r--   0        0        0     6405 2024-05-29 09:19:02.268446 django_lookbook-0.0.2/src/django_lookbook/views.py
+-rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 django_lookbook-0.0.2/PKG-INFO
```

### Comparing `django_lookbook-0.0.1/pyproject.toml` & `django_lookbook-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-lookbook"
-version = "0.0.1"
+version = "0.0.2"
 description = "UI development environment for Django"
 authors = ["Michael Yin <michaelyin@accordbox.com>"]
 license = "MIT"
 homepage = "https://github.com/rails-inspire-django/django-lookbook"
 readme = "README.md"
 packages = [{ include = "django_lookbook", from = "src" }]
```

### Comparing `django_lookbook-0.0.1/src/django_lookbook/static/lookbook/css/app.css` & `django_lookbook-0.0.2/src/django_lookbook/static/lookbook/css/app.css`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/static/lookbook/css/app.css.map` & `django_lookbook-0.0.2/src/django_lookbook/static/lookbook/css/app.css.map`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/static/lookbook/js/app.js` & `django_lookbook-0.0.2/src/django_lookbook/static/lookbook/js/app.js`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/static/lookbook/js/app.js.map` & `django_lookbook-0.0.2/src/django_lookbook/static/lookbook/js/app.js.map`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/static/lookbook/manifest.json` & `django_lookbook-0.0.2/src/django_lookbook/static/lookbook/manifest.json`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/static/lookbook/vendors/images/lucide-sprite.svg` & `django_lookbook-0.0.2/src/django_lookbook/static/lookbook/vendors/images/lucide-sprite.svg`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/static/lookbook/vendors/images/sample.jpg` & `django_lookbook-0.0.2/src/django_lookbook/static/lookbook/vendors/images/sample.jpg`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/static/lookbook/vendors/images/webpack.png` & `django_lookbook-0.0.2/src/django_lookbook/static/lookbook/vendors/images/webpack.png`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/templates/django_lookbook/base.html` & `django_lookbook-0.0.2/src/django_lookbook/templates/django_lookbook/base.html`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/templates/django_lookbook/fields/toggle_switch_widget.html` & `django_lookbook-0.0.2/src/django_lookbook/templates/django_lookbook/fields/toggle_switch_widget.html`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/templates/django_lookbook/includes/sidebar_2_level.html` & `django_lookbook-0.0.2/src/django_lookbook/templates/django_lookbook/includes/sidebar_2_level.html`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/templates/django_lookbook/includes/sidebar_3_level.html` & `django_lookbook-0.0.2/src/django_lookbook/templates/django_lookbook/includes/sidebar_3_level.html`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/templates/django_lookbook/includes/sidebar_previews.html` & `django_lookbook-0.0.2/src/django_lookbook/templates/django_lookbook/includes/sidebar_previews.html`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/templates/django_lookbook/index.html` & `django_lookbook-0.0.2/src/django_lookbook/templates/django_lookbook/index.html`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/templates/django_lookbook/inspect.html` & `django_lookbook-0.0.2/src/django_lookbook/templates/django_lookbook/inspect.html`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/src/django_lookbook/views.py` & `django_lookbook-0.0.2/src/django_lookbook/views.py`

 * *Files identical despite different names*

### Comparing `django_lookbook-0.0.1/PKG-INFO` & `django_lookbook-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lookbook
-Version: 0.0.1
+Version: 0.0.2
 Summary: UI development environment for Django
 Home-page: https://github.com/rails-inspire-django/django-lookbook
 License: MIT
 Author: Michael Yin
 Author-email: michaelyin@accordbox.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

