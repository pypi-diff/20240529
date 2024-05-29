# Comparing `tmp/clear_skies_twilio-0.9.0.tar.gz` & `tmp/clear_skies_twilio-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear_skies_twilio-0.9.0.tar", max compression
+gzip compressed data, was "clear_skies_twilio-0.9.1.tar", max compression
```

## Comparing `clear_skies_twilio-0.9.0.tar` & `clear_skies_twilio-0.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2024-04-24 18:59:41.490848 clear_skies_twilio-0.9.0/LICENSE
--rw-r--r--   0        0        0     3094 2024-04-25 11:28:16.271795 clear_skies_twilio-0.9.0/README.md
--rw-r--r--   0        0        0      728 2024-04-25 16:54:52.571843 clear_skies_twilio-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       26 2024-04-25 17:17:30.135273 clear_skies_twilio-0.9.0/src/clearskies_twilio/__init__.py
--rw-r--r--   0        0        0      488 2024-04-25 17:17:42.948174 clear_skies_twilio-0.9.0/src/clearskies_twilio/actions/__init__.py
--rw-r--r--   0        0        0     5420 2024-04-25 17:28:21.715236 clear_skies_twilio-0.9.0/src/clearskies_twilio/actions/sms.py
--rw-r--r--   0        0        0     2449 2024-04-25 17:30:51.592030 clear_skies_twilio-0.9.0/src/clearskies_twilio/actions/sms_test.py
--rw-r--r--   0        0        0      428 2024-04-25 11:19:19.744591 clear_skies_twilio-0.9.0/src/clearskies_twilio/di/__init__.py
--rw-r--r--   0        0        0     2298 2024-04-25 16:54:12.429959 clear_skies_twilio-0.9.0/src/clearskies_twilio/di/twilio.py
--rw-r--r--   0        0        0     3763 1970-01-01 00:00:00.000000 clear_skies_twilio-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-24 18:59:41.490848 clear_skies_twilio-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3094 2024-04-25 11:28:16.271795 clear_skies_twilio-0.9.1/README.md
+-rw-r--r--   0        0        0      728 2024-05-29 11:36:56.441938 clear_skies_twilio-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       26 2024-04-25 17:17:30.135273 clear_skies_twilio-0.9.1/src/clearskies_twilio/__init__.py
+-rw-r--r--   0        0        0      488 2024-04-25 17:17:42.948174 clear_skies_twilio-0.9.1/src/clearskies_twilio/actions/__init__.py
+-rw-r--r--   0        0        0     4879 2024-05-29 11:36:37.709880 clear_skies_twilio-0.9.1/src/clearskies_twilio/actions/sms.py
+-rw-r--r--   0        0        0     2449 2024-04-25 17:30:51.592030 clear_skies_twilio-0.9.1/src/clearskies_twilio/actions/sms_test.py
+-rw-r--r--   0        0        0      428 2024-04-25 11:19:19.744591 clear_skies_twilio-0.9.1/src/clearskies_twilio/di/__init__.py
+-rw-r--r--   0        0        0     2298 2024-04-25 16:54:12.429959 clear_skies_twilio-0.9.1/src/clearskies_twilio/di/twilio.py
+-rw-r--r--   0        0        0     3763 1970-01-01 00:00:00.000000 clear_skies_twilio-0.9.1/PKG-INFO
```

### Comparing `clear_skies_twilio-0.9.0/LICENSE` & `clear_skies_twilio-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clear_skies_twilio-0.9.0/README.md` & `clear_skies_twilio-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `clear_skies_twilio-0.9.0/pyproject.toml` & `clear_skies_twilio-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "clear-skies-twilio"
-version = "0.9.0"
+version = "0.9.1"
 description = "clearskies bindings for working with Twilio"
 authors = [
     "Conor Mancone <cmancone@gmail.com>",
 ]
 repository = "https://github.com/cmancone/clearskies-twilio"
 license = "MIT"
 readme = "./README.md"
```

### Comparing `clear_skies_twilio-0.9.0/src/clearskies_twilio/actions/sms.py` & `clear_skies_twilio-0.9.1/src/clearskies_twilio/actions/sms.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     def __call__(self, model: clearskies.Model) -> None:
         """Send a notification as configured."""
         if self.when and not self.di.call_function(self.when, model=model):
             return
 
         from_number = self._resolve_number(self.from_number, "from_number", model)
         to_number = self._resolve_number(self.to_number, "to_number", model)
+        if not from_number or not to_number:
+            return
         message = self._resolve_message(self.message, model)
         self.twilio.messages.create(**{
             "to":to_number,
             "from":from_number,
             "body":message,
         })
 
@@ -65,23 +67,23 @@
 
         Note that the actual phone numbers may not be in the correct format expected by twilio.
         """
         model_label = model.id_column_name + ": " + model.get(model.id_column_name)
         if callable(number):
             number = self.di.call_function(number, model=model)
             if not number:
-                raise ValueError(f"Error with clearskies.twilio.actions.sms: I executed the callable attached to '{label}' but it returned a non-value.  The callable must return a phone number as a string.  In case this helps, you can provide a callable to 'when' and have it return false in csaes where you don't want a message sent.")
+                return None
             if not isinstance(number, str):
                 raise ValueError(f"Error with clearskies_twilio.actions.sms: I executed the callable attached to '{label}' but it did not return a string.  The callable must return a phone number as a string.")
         else:
             # do we have a column name?
             if number in model.columns():
                 number = model.get(number)
             if not number:
-                raise ValueError(f"Error with clearskies.twilio.actions.sms: I fetched a column called '{label}' for model {model_label}, hoping for a phone number, but I got back a non-value.  In case this helps, you can provide a callable to 'when' and have it return false in csaes where you don't want a message sent.")
+                return None
             if not isinstance(number, str):
                 raise ValueError(f"Error with clearskies_twilio.actions.sms: I fetched a column called '{label}' for model {model_label}, hoping for a phone number, but it returned a non-string.  The column must return a phone number as a string.")
 
 
         # now make sure we have a twilio friendly number
         number = re.sub(r"\D", "", number)
         if not number:
```

### Comparing `clear_skies_twilio-0.9.0/src/clearskies_twilio/actions/sms_test.py` & `clear_skies_twilio-0.9.1/src/clearskies_twilio/actions/sms_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_twilio-0.9.0/src/clearskies_twilio/di/twilio.py` & `clear_skies_twilio-0.9.1/src/clearskies_twilio/di/twilio.py`

 * *Files identical despite different names*

### Comparing `clear_skies_twilio-0.9.0/PKG-INFO` & `clear_skies_twilio-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-twilio
-Version: 0.9.0
+Version: 0.9.1
 Summary: clearskies bindings for working with Twilio
 Home-page: https://github.com/cmancone/clearskies-twilio
 License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

