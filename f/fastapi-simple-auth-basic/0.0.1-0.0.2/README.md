# Comparing `tmp/fastapi_simple_auth_basic-0.0.1.tar.gz` & `tmp/fastapi_simple_auth_basic-0.0.2.tar.gz`

## Comparing `fastapi_simple_auth_basic-0.0.1.tar` & `fastapi_simple_auth_basic-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/__init__.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/statics/css/styles.css
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/statics/images/github-mark.svg
--rw-r--r--   0        0        0    10931 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/statics/js/simpleauth.js
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/afterlogin.html
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/base.html
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/login.html
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/profile.html
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/recover.html
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/recover_code.html
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/register.html
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/verify-email.html
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/email/change-email.html
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/email/confirm-email.html
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/email/recover.html
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/LICENSE
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/README.md
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/__init__.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/statics/css/styles.css
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/statics/images/github-mark.svg
+-rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/statics/js/simpleauth.js
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/afterlogin.html
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/base.html
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/login.html
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/profile.html
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/recover.html
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/recover_code.html
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/register.html
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/verify-email.html
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/email/change-email.html
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/email/confirm-email.html
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/email/recover.html
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/LICENSE
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/README.md
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 fastapi_simple_auth_basic-0.0.2/PKG-INFO
```

### Comparing `fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/statics/css/styles.css` & `fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/statics/css/styles.css`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/statics/images/github-mark.svg` & `fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/statics/images/github-mark.svg`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/statics/js/simpleauth.js` & `fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/statics/js/simpleauth.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -130,15 +130,15 @@
             },
             body: JSON.stringify(payload)
         })
         .then(async r => {
             switch (r.status) {
                 case 200:
                     var result = await r.json();
-                    open_modal_ok("Login successful", function() {
+                    open_modal_ok("Verification successful", function() {
                         window.location.replace(result['url']);
                     });
                     break;
                 case 400:
                     open_modal_close(await r.text());
                     break;
                 default:
@@ -363,25 +363,26 @@
         })
         .then(r => {
             response = r.clone();
             return r.json();
         })
         .then(async r => {
             // console.log("FIN", r, response.status, response)
-            if (response.status != 200) {
-                var text = await response.text()
-                open_modal_close(text)
-            } else {
-                if (r.status == 'OK') {
-                    console.log("redirect to", r.redirect);
+
+            switch (response.status) {
+                case 200:
                     window.location = r.redirect;
-                } else {
-                    console.log("status not OK:", r)
-                }
+                    break;
+                case 400:
+                    open_modal_close(r.detail);
+                    break;
+                default:
+                    open_modal_close("Something went wrong. Please try again later.")
             }
+
         })
         .catch(e => console.log("ERROR", e))
 }
 
 function init_hooks() {
     var hooks = {
         'fastapi-simple-auth-register-btn': reg_btn_onclick,
@@ -392,15 +393,15 @@
         'fastapi-simple-auth-chpass-btn': chpass_btn_onclick,
         'fastapi-simple-auth-send-recover-btn': send_recover_btn_onclick,
         'fastapi-simple-auth-recover-btn': recover_btn_onclick,
     }
     for (let el_id in hooks) {
         var btn = document.getElementById(el_id);
         if (btn) {
-            console.log("hook", el_id, btn)
+            // console.log("hook", el_id, btn)
             btn.onclick = hooks[el_id]
         }
     }
 
 }
 
 function init_page() {
```

### Comparing `fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/base.html` & `fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/base.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/login.html` & `fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/login.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/profile.html` & `fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/profile.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/recover.html` & `fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/recover.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/recover_code.html` & `fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/recover_code.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/register.html` & `fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/register.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth_basic-0.0.1/fastapi_simple_auth_basic/templates/verify-email.html` & `fastapi_simple_auth_basic-0.0.2/fastapi_simple_auth_basic/templates/verify-email.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth_basic-0.0.1/.gitignore` & `fastapi_simple_auth_basic-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth_basic-0.0.1/LICENSE` & `fastapi_simple_auth_basic-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth_basic-0.0.1/pyproject.toml` & `fastapi_simple_auth_basic-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi-simple-auth-basic"
 # dynamic = ["version"]
-version = "0.0.1"
+version = "0.0.2"
 description = 'FastAPI simple authentication (basic theme)'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Yaroslav Polyakov", email = "yaroslaff@gmail.com" },
```

### Comparing `fastapi_simple_auth_basic-0.0.1/PKG-INFO` & `fastapi_simple_auth_basic-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fastapi-simple-auth-basic
-Version: 0.0.1
+Version: 0.0.2
 Summary: FastAPI simple authentication (basic theme)
 Project-URL: Documentation, https://github.com/yaroslaff/fastapi-simple-auth#readme
 Project-URL: Issues, https://github.com/yaroslaff/fastapi-simple-auth/issues
 Project-URL: Source, https://github.com/yaroslaff/fastapi-simple-auth
 Author-email: Yaroslav Polyakov <yaroslaff@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

