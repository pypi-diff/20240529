# Comparing `tmp/wagtail-mailchimp-integration-0.0.9.tar.gz` & `tmp/wagtail_mailchimp_integration-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-mailchimp-integration-0.0.9.tar", last modified: Thu Feb 29 09:36:20 2024, max compression
+gzip compressed data, was "wagtail_mailchimp_integration-0.1.0.tar", last modified: Wed May 29 11:45:58 2024, max compression
```

## Comparing `wagtail-mailchimp-integration-0.0.9.tar` & `wagtail_mailchimp_integration-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:36:20.071790 wagtail-mailchimp-integration-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-02-29 09:36:20.071790 wagtail-mailchimp-integration-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-29 09:36:20.071790 wagtail-mailchimp-integration-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:36:20.071790 wagtail-mailchimp-integration-0.0.9/wagtail_mailchimp_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-02-29 09:36:20.000000 wagtail-mailchimp-integration-0.0.9/wagtail_mailchimp_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-29 09:36:20.000000 wagtail-mailchimp-integration-0.0.9/wagtail_mailchimp_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 09:36:20.000000 wagtail-mailchimp-integration-0.0.9/wagtail_mailchimp_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-29 09:36:20.000000 wagtail-mailchimp-integration-0.0.9/wagtail_mailchimp_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 09:36:20.000000 wagtail-mailchimp-integration-0.0.9/wagtail_mailchimp_integration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:36:20.071790 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    10374 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:36:20.071790 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:36:20.067790 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:36:20.071790 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/templates/wagtailmailchimp/
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:36:20.071790 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/templates/wagtailmailchimp/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-02-29 09:36:12.000000 wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:45:58.501863 wagtail_mailchimp_integration-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-29 11:45:58.497863 wagtail_mailchimp_integration-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-29 11:45:58.501863 wagtail_mailchimp_integration-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:45:58.497863 wagtail_mailchimp_integration-0.1.0/wagtail_mailchimp_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-29 11:45:58.000000 wagtail_mailchimp_integration-0.1.0/wagtail_mailchimp_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-29 11:45:58.000000 wagtail_mailchimp_integration-0.1.0/wagtail_mailchimp_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:45:58.000000 wagtail_mailchimp_integration-0.1.0/wagtail_mailchimp_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-29 11:45:58.000000 wagtail_mailchimp_integration-0.1.0/wagtail_mailchimp_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 11:45:58.000000 wagtail_mailchimp_integration-0.1.0/wagtail_mailchimp_integration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:45:58.497863 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10374 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:45:58.497863 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:45:58.493863 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:45:58.497863 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/templates/wagtailmailchimp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:45:58.497863 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/templates/wagtailmailchimp/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/templates/wagtailmailchimp/widgets/audience_select_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-29 11:45:52.000000 wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/widgets.py
```

### Comparing `wagtail-mailchimp-integration-0.0.9/LICENSE` & `wagtail_mailchimp_integration-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.9/PKG-INFO` & `wagtail_mailchimp_integration-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wagtail-mailchimp-integration
-Version: 0.0.9
-Summary: Integration of Mailchimp Email Marketing in Wagtail Projects.
+Version: 0.1.0
+Summary: Integration of Mailchimp Email Marketing in Wagtail Form Builder Pages.
 Home-page: https://github.com/wmo-raf/wagtail-mailchimp-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `wagtail-mailchimp-integration-0.0.9/README.md` & `wagtail_mailchimp_integration-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.9/setup.cfg` & `wagtail_mailchimp_integration-0.1.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = wagtail-mailchimp-integration
-version = 0.0.9
-description = Integration of Mailchimp Email Marketing in Wagtail Projects.
+version = 0.1.0
+description = Integration of Mailchimp Email Marketing in Wagtail Form Builder Pages.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/wagtail-mailchimp-integration
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
 classifiers =
```

### Comparing `wagtail-mailchimp-integration-0.0.9/wagtail_mailchimp_integration.egg-info/PKG-INFO` & `wagtail_mailchimp_integration-0.1.0/wagtail_mailchimp_integration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wagtail-mailchimp-integration
-Version: 0.0.9
-Summary: Integration of Mailchimp Email Marketing in Wagtail Projects.
+Version: 0.1.0
+Summary: Integration of Mailchimp Email Marketing in Wagtail Form Builder Pages.
 Home-page: https://github.com/wmo-raf/wagtail-mailchimp-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `wagtail-mailchimp-integration-0.0.9/wagtail_mailchimp_integration.egg-info/SOURCES.txt` & `wagtail_mailchimp_integration-0.1.0/wagtail_mailchimp_integration.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 wagtail_mailchimp_integration.egg-info/dependency_links.txt
 wagtail_mailchimp_integration.egg-info/requires.txt
 wagtail_mailchimp_integration.egg-info/top_level.txt
 wagtailmailchimp/__init__.py
 wagtailmailchimp/admin.py
 wagtailmailchimp/api.py
 wagtailmailchimp/apps.py
+wagtailmailchimp/errors.py
 wagtailmailchimp/forms.py
 wagtailmailchimp/models.py
 wagtailmailchimp/tests.py
 wagtailmailchimp/views.py
 wagtailmailchimp/wagtail_hooks.py
 wagtailmailchimp/widgets.py
 wagtailmailchimp/migrations/0001_initial.py
 wagtailmailchimp/migrations/__init__.py
 wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html
+wagtailmailchimp/templates/wagtailmailchimp/widgets/audience_select_widget.html
 wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html
```

### Comparing `wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/api.py` & `wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,14 @@
 from django.core.cache import cache
 from mailchimp3 import MailChimp
 
 
 class MailchimpApi:
     def __init__(self, api_key):
-        self.client = None
-        self.is_active = False
-
-        self.init_api(api_key)
-
-    def init_api(self, api_key):
-        try:
-            self.client = MailChimp(mc_api=api_key)
-            self.is_active = True
-        except Exception as e:
-            return None
+        self.client = MailChimp(mc_api=api_key)
 
     def get_lists(self, fields='lists.id,lists.name'):
         cache_key = f"get-lists-{fields}"
         lists = cache.get(cache_key)
 
         if lists is None:
             try:
@@ -112,7 +102,10 @@
 
             categories.append(interest_category)
 
         return categories
 
     def add_user_to_list(self, list_id, data):
         return self.client.lists.members.create(list_id=list_id, data=data)
+
+    def ping(self):
+        return self.client.ping.get()
```

### Comparing `wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/forms.py` & `wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/migrations/0001_initial.py` & `wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/models.py` & `wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import json
 
 from django.contrib import messages
+from django.core.exceptions import ValidationError
 from django.db import models
 from django.forms import BooleanField
 from django.template import Context, Template
 from django.utils.translation import gettext_lazy as _
 from mailchimp3.mailchimpclient import MailChimpError
 from wagtail.admin.panels import FieldPanel, FieldRowPanel, MultiFieldPanel
 from wagtail.contrib.forms.models import AbstractForm
 from wagtail.contrib.settings.models import BaseSiteSetting
 from wagtail.contrib.settings.registry import register_setting
 
 from .api import MailchimpApi
-from .widgets import MailchimpSubscriberOptinWidget, MailchimpAudienceListWidget
+from .widgets import MailchimpSubscriberOptinWidget, MailchimpAudienceSelectWidget
 
 
 @register_setting
 class MailchimpSettings(BaseSiteSetting):
     api_key = models.CharField(verbose_name=_("Mailchimp API Key"), max_length=50, blank=True, null=True,
                                help_text=_("Mailchimp API Key "))
     default_audience_id = models.CharField(verbose_name=_("Default Mailchimp Audience Id"), max_length=100, blank=True,
@@ -24,14 +25,27 @@
                                            help_text=_("Default Mailchimp Audience Id"))
 
     panels = [
         FieldPanel("api_key"),
         FieldPanel("default_audience_id"),
     ]
 
+    def clean_fields(self, exclude=None):
+        super().clean()
+
+        if not self.api_key:
+            return
+
+        try:
+            # Check if the API key is valid
+            api = MailchimpApi(self.api_key)
+            api.ping()
+        except Exception as e:
+            raise ValidationError({'api_key': str(e)})
+
 
 class AbstractMailChimpPage(models.Model):
     """
     Abstract MailChimp page definition.
     """
     list_id = models.CharField(_('MailChimp Audience'), max_length=50,
                                help_text=_('Select MailChimp Audience to use for this form'))
@@ -61,15 +75,15 @@
 
         view = MailChimpView.as_view(page_instance=self)
         return view(request)
 
     content_panels = [
         MultiFieldPanel([
             FieldRowPanel([
-                FieldPanel('list_id', widget=MailchimpAudienceListWidget),
+                FieldPanel('list_id', widget=MailchimpAudienceSelectWidget),
                 FieldPanel('double_optin'),
             ], classname='label-above'),
         ], (_('MailChimp Settings'))),
         FieldPanel('thank_you_text')
     ]
 
 
@@ -86,42 +100,51 @@
     merge_fields_mapping = models.TextField(blank=True, null=True)
     interest_categories = models.TextField(blank=True, null=True)
 
     mailing_list_checkbox_label = models.CharField(max_length=200, blank=True,
                                                    verbose_name=_("Mailing list checkbox label"))
 
     integration_panels = [
-        FieldPanel("audience_list_id", widget=MailchimpAudienceListWidget),
+        FieldPanel("audience_list_id", widget=MailchimpAudienceSelectWidget),
     ]
 
     is_mailchimp_integration = True
 
     def remove_mailchimp_field(self, form):
         form.fields.pop(self.mailchimp_field_name, None)
         return form.cleaned_data.pop(self.mailchimp_field_name, None)
 
     def serve(self, request, *args, **kwargs):
         # We need to access the request later on in integration operation
         self.request = request
 
         return super(AbstractMailchimpIntegrationForm, self).serve(request, *args, **kwargs)
 
+    def should_perform_mailchimp_integration_operation(self, request, form):
+        # override this method to add custom logic to determine if the
+        # mailchimp integration operation should be performed
+        return True
+
+    def show_page_listing_mailchimp_integration_button(self):
+        # override this method to add custom logic to determine if the
+        # mailchimp integration button should be shown in the page listing
+        return True
+
     def process_form_submission(self, form):
         self.remove_mailchimp_field(form)
 
         form_submission = super(AbstractMailchimpIntegrationForm, self).process_form_submission(form)
 
         if self.request:
             try:
-
                 form_data = dict(form.data)
                 user_checked_sub = bool(form_data.get(self.mailchimp_field_name, False))
                 user_selected_interests = form_data.get(self.mailchimp_interests_field_name, None)
 
-                if user_checked_sub:
+                if user_checked_sub and self.should_perform_mailchimp_integration_operation(self.request, form):
                     self.mailchimp_integration_operation(self, form=form, request=self.request,
                                                          user_selected_interests=user_selected_interests)
             except Exception as e:
                 pass
 
         return form_submission
```

### Comparing `wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html` & `wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html` & `wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/views.py` & `wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         Returns list of MailChimp grouping dictionaries.
 
         :rtype: dict.
         """
 
         api = self.get_api()
 
-        if self.interest_categories is None and api.is_active:
+        if self.interest_categories is None:
             list_id = self.page_instance.list_id
 
             interest_categories = api.get_interest_categories_for_list(list_id=list_id)
 
             categories = []
 
             for category in interest_categories:
@@ -129,15 +129,15 @@
         Returns list of MailChimp merge fields dictionaries.
 
         :rtype: dict.
         """
 
         api = self.get_api()
 
-        if self.merge_fields is None and api.is_active:
+        if self.merge_fields is None:
             self.merge_fields = api.get_merge_fields_for_list(self.page_instance.list_id)
 
         # If we don't have any merge variables to build a form from,
         # raise an HTTP 404 error.
         if not self.merge_fields:
             raise Http404
 
@@ -149,15 +149,14 @@
 
         :param form_class: name of the form class to use.
         :rtype: MailChimpForm.
         """
 
         merge_fields = self.get_merge_fields()
         interest_categories = self.get_interest_categories()
-
         return MailChimpForm(merge_fields, interest_categories, **self.get_form_kwargs())
 
     def get_template_names(self):
         """
         Returns list of available template names.
 
         :rtype: list.
@@ -192,15 +191,15 @@
             interests_payload[interest] = True
 
         error_traceback = None
 
         context = {'page': self.page_instance, 'self': self.page_instance}
 
         # Must have an email address.
-        if api.is_active and 'EMAIL' in clean_merge_fields:
+        if 'EMAIL' in clean_merge_fields:
             data = {
                 'email_address': clean_merge_fields.pop('EMAIL'),
                 'merge_fields': clean_merge_fields,
                 'status': status,
             }
 
             if interests_payload:
@@ -220,15 +219,15 @@
                                 "form": self.get_form(),
                             })
                             return self.render_to_response(context)
 
             except Exception as e:
                 error_traceback = e
         else:
-            if not api.is_active:
+            if not api:
                 error_traceback = "MAILCHIMP API not active"
             else:
                 error_traceback = "No email in fields"
 
         if error_traceback:
             mail_admins("Error adding user to mailing list", str(error_traceback), fail_silently=True)
```

### Comparing `wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/wagtail_hooks.py` & `wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/wagtail_hooks.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,14 @@
         path('mailchimp-integration/<int:page_id>', mailchimp_integration_view, name="mailchimp_integration_view"),
     ]
 
 
 @hooks.register('register_page_listing_buttons')
 def page_listing_buttons(page, page_perms, next_url=None):
     if hasattr(page, "is_mailchimp_integration") and hasattr(page, "audience_list_id"):
-        if page.audience_list_id:
+        if page.audience_list_id and page.show_page_listing_mailchimp_integration_button():
             url = reverse("mailchimp_integration_view", args=[page.pk, ])
             yield wagtail_admin_widgets.PageListingButton(
                 "Mailchimp Integration",
                 url,
-                priority=50
+                priority=60
             )
```

### Comparing `wagtail-mailchimp-integration-0.0.9/wagtailmailchimp/widgets.py` & `wagtail_mailchimp_integration-0.1.0/wagtailmailchimp/widgets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from django.db.utils import ProgrammingError
 from django.forms.widgets import Input, Select
 from wagtail.models import Site
+from django.utils.translation import gettext as _
 
 from .api import MailchimpApi
+from .errors import MailchimpApiError
 
 
 class CustomSelect(Select):
     def create_option(self, *args, **kwargs):
         option = super().create_option(*args, **kwargs)
         if not option.get('value'):
             option['attrs']['disabled'] = True
@@ -28,33 +30,51 @@
         ctx = super(MailchimpSubscriberOptinWidget, self).get_context(name, value, attrs)
         ctx['widget']['interest_categories'] = self.interest_categories
         ctx['widget']['label'] = self.label
         ctx['widget']['interests_field_name'] = self.interests_field_name
         return ctx
 
 
-class MailchimpAudienceListWidget(Select):
-    def __init__(self, attrs=None, choices=()):
-        super().__init__(attrs, choices)
+class MailchimpAudienceSelectWidget(Input):
+    template_name = 'wagtailmailchimp/widgets/audience_select_widget.html'
 
-        audience_lists = self.get_mailchimp_audience_lists()
-        audience_choices = [("", "-- None --")]
+    def get_context(self, name, value, attrs):
+        ctx = super().get_context(name, value, attrs)
+        mailchimp_error = None
+
+        audiences = []
 
-        for audience in audience_lists:
-            audience_choices.append([audience.get("id"), audience.get("name")])
+        try:
+            audiences = self.get_mailchimp_audience_lists()
+        except MailchimpApiError as e:
+            mailchimp_error = e.message
+        except Exception as e:
+            mailchimp_error = _("Error obtaining Mailchimp audiences. Please make sure the Mailchimp API "
+                                "key in Mailchimp Settings is correct")
+
+        ctx["widget"].update({
+            "value": value,
+            "mailchimp_error": mailchimp_error,
+            "audiences": audiences,
+            "no_audiences_message": _("No Mailchimp audiences found. Please create one on Mailchimp and try again.")
+        })
 
-        self.choices = audience_choices
+        return ctx
 
     def get_mailchimp_audience_lists(self):
         from .models import MailchimpSettings
 
         # catch error where 'wagtailcore_site' relation is not migrated to db yet
         try:
             current_site = Site.objects.get(is_default_site=True)
         except ProgrammingError:
             return []
 
         mc_settings = MailchimpSettings.for_site(current_site)
+
+        if not mc_settings.api_key:
+            raise MailchimpApiError("Mailchimp API key is not set")
+
         mailchimp = MailchimpApi(api_key=mc_settings.api_key)
         lists = mailchimp.get_lists()
 
         return lists
```

