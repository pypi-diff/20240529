# Comparing `tmp/flask_openapi3_swagger-5.17.13.tar.gz` & `tmp/flask_openapi3_swagger-5.17.14.tar.gz`

## Comparing `flask_openapi3_swagger-5.17.13.tar` & `flask_openapi3_swagger-5.17.14.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.13/flask_openapi3_swagger/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.13/flask_openapi3_swagger/__version__.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.13/flask_openapi3_swagger/plugins.py
--rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.13/flask_openapi3_swagger/templates/__init__.py
--rw-r--r--   0        0        0   152071 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.13/flask_openapi3_swagger/templates/swagger/css/swagger-ui.css
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.13/flask_openapi3_swagger/templates/swagger/images/swagger.svg
--rw-r--r--   0        0        0  1452758 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.13/flask_openapi3_swagger/templates/swagger/js/swagger-ui-bundle.js
--rw-r--r--   0        0        0   230293 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.13/flask_openapi3_swagger/templates/swagger/js/swagger-ui-standalone-preset.js
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.13/.gitignore
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.13/pyproject.toml
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.13/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.14/flask_openapi3_swagger/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.14/flask_openapi3_swagger/__version__.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.14/flask_openapi3_swagger/plugins.py
+-rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.14/flask_openapi3_swagger/templates/__init__.py
+-rw-r--r--   0        0        0   152071 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.14/flask_openapi3_swagger/templates/swagger/css/swagger-ui.css
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.14/flask_openapi3_swagger/templates/swagger/images/swagger.svg
+-rw-r--r--   0        0        0  1452753 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.14/flask_openapi3_swagger/templates/swagger/js/swagger-ui-bundle.js
+-rw-r--r--   0        0        0   230293 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.14/flask_openapi3_swagger/templates/swagger/js/swagger-ui-standalone-preset.js
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.14/.gitignore
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.14/pyproject.toml
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 flask_openapi3_swagger-5.17.14/PKG-INFO
```

### Comparing `flask_openapi3_swagger-5.17.13/flask_openapi3_swagger/plugins.py` & `flask_openapi3_swagger-5.17.14/flask_openapi3_swagger/plugins.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3_swagger-5.17.13/flask_openapi3_swagger/templates/__init__.py` & `flask_openapi3_swagger-5.17.14/flask_openapi3_swagger/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3_swagger-5.17.13/flask_openapi3_swagger/templates/swagger/css/swagger-ui.css` & `flask_openapi3_swagger-5.17.14/flask_openapi3_swagger/templates/swagger/css/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask_openapi3_swagger-5.17.13/flask_openapi3_swagger/templates/swagger/images/swagger.svg` & `flask_openapi3_swagger-5.17.14/flask_openapi3_swagger/templates/swagger/images/swagger.svg`

 * *Files identical despite different names*

### Comparing `flask_openapi3_swagger-5.17.13/flask_openapi3_swagger/templates/swagger/js/swagger-ui-bundle.js` & `flask_openapi3_swagger-5.17.14/flask_openapi3_swagger/templates/swagger/js/swagger-ui-bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -26629,17 +26629,15 @@
             getMapDispatchToProps(o) {
                 return s => We()({}, this.getWrappedAndBoundActions(s), this.getFn(), o)
             }
         }
 
         function combinePlugins(o, s) {
             return isObject(o) && !isArray(o) ? Qe()({}, o) : isFunc(o) ? combinePlugins(o(s), s) : isArray(o) ? o.map((o => combinePlugins(o, s))).reduce(systemExtend, {
-                components: {
-                    ...s.getComponents()
-                }
+                components: s.getComponents()
             }) : {}
         }
 
         function callAfterLoad(o, s, {
             hasLoaded: i
         } = {}) {
             let u = i;
@@ -47927,18 +47925,18 @@
             versions_after_load = () => {
                 const {
                     GIT_DIRTY: o,
                     GIT_COMMIT: s,
                     PACKAGE_VERSION: i,
                     BUILD_TIME: u
                 } = {
-                    PACKAGE_VERSION: "5.17.13",
-                    GIT_COMMIT: "g31b35fdc",
+                    PACKAGE_VERSION: "5.17.14",
+                    GIT_COMMIT: "g8aa52920",
                     GIT_DIRTY: !0,
-                    BUILD_TIME: "Mon, 27 May 2024 11:44:43 GMT"
+                    BUILD_TIME: "Tue, 28 May 2024 05:23:41 GMT"
                 };
                 at.versions = at.versions || {}, at.versions.swaggerUI = {
                     version: i,
                     gitRevision: s,
                     gitDirty: o,
                     buildTimestamp: u
                 }
```

### Comparing `flask_openapi3_swagger-5.17.13/flask_openapi3_swagger/templates/swagger/js/swagger-ui-standalone-preset.js` & `flask_openapi3_swagger-5.17.14/flask_openapi3_swagger/templates/swagger/js/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask_openapi3_swagger-5.17.13/.gitignore` & `flask_openapi3_swagger-5.17.14/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_openapi3_swagger-5.17.13/pyproject.toml` & `flask_openapi3_swagger-5.17.14/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_openapi3_swagger-5.17.13/PKG-INFO` & `flask_openapi3_swagger-5.17.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flask-openapi3-swagger
-Version: 5.17.13
+Version: 5.17.14
 Summary: Provide Swagger UI for flask-openapi3.
 Project-URL: Homepage, https://github.com/luolingchun/flask-openapi3-plugins/tree/master/flask-openapi3-swagger
 Project-URL: Documentation, https://luolingchun.github.io/flask-openapi3/latest/Usage/UI_Templates/
 Maintainer-email: llc <luolingchun@outlook.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

