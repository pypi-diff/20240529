# Comparing `tmp/govuk-frontend-wtf-3.0.0.tar.gz` & `tmp/govuk_frontend_wtf-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govuk-frontend-wtf-3.0.0.tar", last modified: Tue Feb 13 14:28:53 2024, max compression
+gzip compressed data, was "govuk_frontend_wtf-3.1.0.tar", last modified: Wed May 29 13:12:44 2024, max compression
```

## Comparing `govuk-frontend-wtf-3.0.0.tar` & `govuk_frontend_wtf-3.1.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:28:53.324478 govuk-frontend-wtf-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-02-13 14:28:53.324478 govuk-frontend-wtf-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:28:53.320478 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/gov_form_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:28:53.324478 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/templates/button.html
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/templates/charactercount.html
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/templates/checkboxes.html
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/templates/date.html
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/templates/file-upload.html
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/templates/input.html
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/templates/radios.html
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/templates/select.html
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/templates/textarea.html
--rw-r--r--   0 runner    (1001) docker     (127)    10318 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/wtforms_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:28:53.324478 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-02-13 14:28:53.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-02-13 14:28:53.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 14:28:53.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-13 14:28:53.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-13 14:28:53.000000 govuk-frontend-wtf-3.0.0/govuk_frontend_wtf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-13 14:28:53.324478 govuk-frontend-wtf-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:28:53.324478 govuk-frontend-wtf-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-02-13 14:28:41.000000 govuk-frontend-wtf-3.0.0/tests/test_wtf_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:12:44.688125 govuk_frontend_wtf-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-29 13:12:44.688125 govuk_frontend_wtf-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:12:44.684125 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/gov_form_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:12:44.684125 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/templates/button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/templates/charactercount.html
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/templates/checkboxes.html
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/templates/date.html
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/templates/file-upload.html
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/templates/input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/templates/password.html
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/templates/radios.html
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/templates/select.html
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/templates/textarea.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/wtforms_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:12:44.684125 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-29 13:12:44.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-29 13:12:44.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:12:44.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 13:12:44.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 13:12:44.000000 govuk_frontend_wtf-3.1.0/govuk_frontend_wtf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-29 13:12:44.688125 govuk_frontend_wtf-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:12:44.684125 govuk_frontend_wtf-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-29 13:12:40.000000 govuk_frontend_wtf-3.1.0/tests/test_wtf_widgets.py
```

### Comparing `govuk-frontend-wtf-3.0.0/LICENSE` & `govuk_frontend_wtf-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `govuk-frontend-wtf-3.0.0/PKG-INFO` & `govuk_frontend_wtf-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-wtf
-Version: 3.0.0
+Version: 3.1.0
 Summary: GOV.UK Frontend WTForms Widgets
 Home-page: https://github.com/LandRegistry/govuk-frontend-wtf
 Author: Matt Shaw
 Author-email: matthew.shaw@landregistry.gov.uk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,15 +27,15 @@
 Requires-Dist: govuk-frontend-jinja>=3.0.0
 Requires-Dist: jinja2
 Requires-Dist: wtforms>=3.1.0
 
 # GOV.UK Frontend WTForms Widgets
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-wtf.svg)](https://pypi.org/project/govuk-frontend-wtf/)
-![govuk-frontend 5.1.0](https://img.shields.io/badge/govuk--frontend%20version-5.1.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 5.4.0](https://img.shields.io/badge/govuk--frontend%20version-5.4.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend WTForms is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository contains a set of [WTForms widgets](https://wtforms.readthedocs.io/en/2.3.x/widgets/) used to render [WTForm fields](https://wtforms.readthedocs.io/en/2.3.x/fields/) using [GOV.UK Frontend](https://design-system.service.gov.uk/) component styling. This is done using Jinja macros from the [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) port of the original GOV.UK Frontend Nunjucks macros. These are kept up-to-date with GOV.UK Frontend releases, are thoroughly tested and produce 100% equivalent markup.
 
 This approach also renders the associated error messages in the appropriate place, shows the error summary component at the top of the page and sets all related accessibility ARIA attributes. Adding the appropriate [widget](#widgets) to your existing form Python class, along with far simpler templates, makes it quick and easy to produce fully GOV.UK compliant forms.
```

### Comparing `govuk-frontend-wtf-3.0.0/README.md` & `govuk_frontend_wtf-3.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # GOV.UK Frontend WTForms Widgets
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-wtf.svg)](https://pypi.org/project/govuk-frontend-wtf/)
-![govuk-frontend 5.1.0](https://img.shields.io/badge/govuk--frontend%20version-5.1.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 5.4.0](https://img.shields.io/badge/govuk--frontend%20version-5.4.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend WTForms is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository contains a set of [WTForms widgets](https://wtforms.readthedocs.io/en/2.3.x/widgets/) used to render [WTForm fields](https://wtforms.readthedocs.io/en/2.3.x/fields/) using [GOV.UK Frontend](https://design-system.service.gov.uk/) component styling. This is done using Jinja macros from the [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) port of the original GOV.UK Frontend Nunjucks macros. These are kept up-to-date with GOV.UK Frontend releases, are thoroughly tested and produce 100% equivalent markup.
 
 This approach also renders the associated error messages in the appropriate place, shows the error summary component at the top of the page and sets all related accessibility ARIA attributes. Adding the appropriate [widget](#widgets) to your existing form Python class, along with far simpler templates, makes it quick and easy to produce fully GOV.UK compliant forms.
```

### Comparing `govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/gov_form_base.py` & `govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/gov_form_base.py`

 * *Files identical despite different names*

### Comparing `govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/main.py` & `govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/main.py`

 * *Files identical despite different names*

### Comparing `govuk-frontend-wtf-3.0.0/govuk_frontend_wtf/wtforms_widgets.py` & `govuk_frontend_wtf-3.1.0/govuk_frontend_wtf/wtforms_widgets.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,25 +33,21 @@
 
 class GovTextInput(GovInput, TextInput):
     """Render a single-line text input."""
 
     input_type = "text"
 
 
-class GovPasswordInput(GovInput, PasswordInput):
-    """Render a password input.
+class GovPasswordInput(GovFormBase, PasswordInput):
+    """Render a password input."""
 
-    For security purposes, this field will not reproduce the value on a form
-    submit by default. To have the value filled in, set `hide_value` to
-    `False`.
-    """
+    template = "govuk_frontend_wtf/password.html"
 
     def __call__(self, field, **kwargs):
-        if self.hide_value:
-            kwargs["value"] = ""
+        kwargs.setdefault("id", field.id)
         return super().__call__(field, **kwargs)
 
 
 class GovCheckboxesInput(GovIterableBase):
     """Multiple checkboxes, from a SelectMultipleField
 
     This widget type doesn't exist in WTForms - the recommendation
```

### Comparing `govuk-frontend-wtf-3.0.0/govuk_frontend_wtf.egg-info/PKG-INFO` & `govuk_frontend_wtf-3.1.0/govuk_frontend_wtf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-wtf
-Version: 3.0.0
+Version: 3.1.0
 Summary: GOV.UK Frontend WTForms Widgets
 Home-page: https://github.com/LandRegistry/govuk-frontend-wtf
 Author: Matt Shaw
 Author-email: matthew.shaw@landregistry.gov.uk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,15 +27,15 @@
 Requires-Dist: govuk-frontend-jinja>=3.0.0
 Requires-Dist: jinja2
 Requires-Dist: wtforms>=3.1.0
 
 # GOV.UK Frontend WTForms Widgets
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-wtf.svg)](https://pypi.org/project/govuk-frontend-wtf/)
-![govuk-frontend 5.1.0](https://img.shields.io/badge/govuk--frontend%20version-5.1.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 5.4.0](https://img.shields.io/badge/govuk--frontend%20version-5.4.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend WTForms is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository contains a set of [WTForms widgets](https://wtforms.readthedocs.io/en/2.3.x/widgets/) used to render [WTForm fields](https://wtforms.readthedocs.io/en/2.3.x/fields/) using [GOV.UK Frontend](https://design-system.service.gov.uk/) component styling. This is done using Jinja macros from the [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) port of the original GOV.UK Frontend Nunjucks macros. These are kept up-to-date with GOV.UK Frontend releases, are thoroughly tested and produce 100% equivalent markup.
 
 This approach also renders the associated error messages in the appropriate place, shows the error summary component at the top of the page and sets all related accessibility ARIA attributes. Adding the appropriate [widget](#widgets) to your existing form Python class, along with far simpler templates, makes it quick and easy to produce fully GOV.UK compliant forms.
```

### Comparing `govuk-frontend-wtf-3.0.0/govuk_frontend_wtf.egg-info/SOURCES.txt` & `govuk_frontend_wtf-3.1.0/govuk_frontend_wtf.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 govuk_frontend_wtf.egg-info/top_level.txt
 govuk_frontend_wtf/templates/button.html
 govuk_frontend_wtf/templates/charactercount.html
 govuk_frontend_wtf/templates/checkboxes.html
 govuk_frontend_wtf/templates/date.html
 govuk_frontend_wtf/templates/file-upload.html
 govuk_frontend_wtf/templates/input.html
+govuk_frontend_wtf/templates/password.html
 govuk_frontend_wtf/templates/radios.html
 govuk_frontend_wtf/templates/select.html
 govuk_frontend_wtf/templates/textarea.html
 tests/test_wtf_widgets.py
```

### Comparing `govuk-frontend-wtf-3.0.0/setup.py` & `govuk_frontend_wtf-3.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 templates = []
 directories = glob.glob("govuk_frontend_wtf/templates/*.html")
 for directory in directories:
     templates.append(os.path.relpath(os.path.dirname(directory), "govuk_frontend_wtf") + "/*.html")
 
 setuptools.setup(
     name="govuk-frontend-wtf",
-    version="3.0.0",
+    version="3.1.0",
     author="Matt Shaw",
     author_email="matthew.shaw@landregistry.gov.uk",
     description="GOV.UK Frontend WTForms Widgets",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LandRegistry/govuk-frontend-wtf",
     packages=setuptools.find_packages(exclude=["tests"]),
```

### Comparing `govuk-frontend-wtf-3.0.0/tests/test_wtf_widgets.py` & `govuk_frontend_wtf-3.1.0/tests/test_wtf_widgets.py`

 * *Files identical despite different names*

