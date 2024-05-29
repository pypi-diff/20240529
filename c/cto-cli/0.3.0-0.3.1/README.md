# Comparing `tmp/cto_cli-0.3.0.tar.gz` & `tmp/cto_cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cto_cli-0.3.0.tar", max compression
+gzip compressed data, was "cto_cli-0.3.1.tar", max compression
```

## Comparing `cto_cli-0.3.0.tar` & `cto_cli-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-05-29 09:42:10.999284 cto_cli-0.3.0/LICENSE
--rw-r--r--   0        0        0      233 2024-05-29 09:42:10.999284 cto_cli-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/api/__init__.py
--rw-r--r--   0        0        0     8748 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/api/connector.py
--rw-r--r--   0        0        0        0 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/commands/__init__.py
--rw-r--r--   0        0        0     4043 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/commands/config.py
--rw-r--r--   0        0        0     2046 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/commands/users.py
--rw-r--r--   0        0        0        0 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/local/__init__.py
--rw-r--r--   0        0        0      451 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/local/commands.py
--rw-r--r--   0        0        0     7333 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/local/files.py
--rw-r--r--   0        0        0     7384 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/local/operations.py
--rw-r--r--   0        0        0     3266 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/local/settings.py
--rw-r--r--   0        0        0     1832 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/local/validators.py
--rw-r--r--   0        0        0     3779 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/ecs/main.py
--rw-r--r--   0        0        0      652 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/main.py
--rw-r--r--   0        0        0      213 2024-05-29 09:42:10.999284 cto_cli-0.3.0/cto_cli/utils/errors.py
--rw-r--r--   0        0        0     1580 2024-05-29 09:42:11.931291 cto_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 cto_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 13:25:43.860944 cto_cli-0.3.1/LICENSE
+-rw-r--r--   0        0        0      233 2024-05-29 13:25:43.860944 cto_cli-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/ecs/api/__init__.py
+-rw-r--r--   0        0        0     8800 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/ecs/api/connector.py
+-rw-r--r--   0        0        0        0 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/ecs/commands/__init__.py
+-rw-r--r--   0        0        0     4043 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/ecs/commands/config.py
+-rw-r--r--   0        0        0     2110 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/ecs/commands/users.py
+-rw-r--r--   0        0        0        0 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/ecs/local/__init__.py
+-rw-r--r--   0        0        0      451 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/ecs/local/commands.py
+-rw-r--r--   0        0        0     7333 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/ecs/local/files.py
+-rw-r--r--   0        0        0     7384 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/ecs/local/operations.py
+-rw-r--r--   0        0        0     3266 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/ecs/local/settings.py
+-rw-r--r--   0        0        0     1832 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/ecs/local/validators.py
+-rw-r--r--   0        0        0     3779 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/ecs/main.py
+-rw-r--r--   0        0        0      652 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/main.py
+-rw-r--r--   0        0        0      213 2024-05-29 13:25:43.860944 cto_cli-0.3.1/cto_cli/utils/errors.py
+-rw-r--r--   0        0        0     1580 2024-05-29 13:25:44.784944 cto_cli-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 cto_cli-0.3.1/PKG-INFO
```

### Comparing `cto_cli-0.3.0/LICENSE` & `cto_cli-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.0/cto_cli/ecs/api/connector.py` & `cto_cli-0.3.1/cto_cli/ecs/api/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,26 +103,28 @@
 
     # USERS
     def create_user(
         self,
         username: str,
         given_name: str,
         family_name: str,
+        email: str,
         admin: bool = False,
         return_as_dict: bool = False,
         read_secrets: bool = False,
         edit_strategies: bool = False,
     ) -> dict | None:
         response = self._make_request(
             'post',
             'users',
             json={
                 'username': username,
                 'given_name': given_name,
                 'family_name': family_name,
+                'email': email,
                 'admin': admin,
                 **({'read_secrets': read_secrets} if admin is False else {}),
                 **({'edit_strategies': edit_strategies} if admin is False else {}),
             },
             headers=self._headers,
         )
         self._handle_response(response)
```

### Comparing `cto_cli-0.3.0/cto_cli/ecs/commands/config.py` & `cto_cli-0.3.1/cto_cli/ecs/commands/config.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.0/cto_cli/ecs/commands/users.py` & `cto_cli-0.3.1/cto_cli/ecs/commands/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,22 +22,24 @@
 
 
 @app.command(name='create')
 def create(
     username: Annotated[str, typer.Option()],
     given_name: Annotated[str, typer.Option()],
     family_name: Annotated[str, typer.Option()],
+    email: Annotated[str, typer.Option()],
     admin: bool = False,
     read_secrets: bool = False,
     edit_strategies: bool = False,
 ):
     APIConnector().create_user(
         username=username,
         given_name=given_name,
         family_name=family_name,
+        email=email,
         admin=admin,
         read_secrets=read_secrets,
         edit_strategies=edit_strategies,
     )
 
 
 class UserAuthOptions(Enum):
```

### Comparing `cto_cli-0.3.0/cto_cli/ecs/local/files.py` & `cto_cli-0.3.1/cto_cli/ecs/local/files.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.0/cto_cli/ecs/local/operations.py` & `cto_cli-0.3.1/cto_cli/ecs/local/operations.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.0/cto_cli/ecs/local/settings.py` & `cto_cli-0.3.1/cto_cli/ecs/local/settings.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.0/cto_cli/ecs/local/validators.py` & `cto_cli-0.3.1/cto_cli/ecs/local/validators.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.0/cto_cli/ecs/main.py` & `cto_cli-0.3.1/cto_cli/ecs/main.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.0/cto_cli/main.py` & `cto_cli-0.3.1/cto_cli/main.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.3.0/pyproject.toml` & `cto_cli-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cto-cli"
-version = "0.3.0"
+version = "0.3.1"
 description = "The CTO cli"
 authors = ["CTO <support@cloudtechnologyoffice.com>"]
 readme = "README.md"
 homepage = "https://doc.cloudtechnologyoffice.com/ecs/latest"
 repository = "https://github.com/Cloud-Technology-Office/cto-cli"
 license = "Apache-2.0"
```

### Comparing `cto_cli-0.3.0/PKG-INFO` & `cto_cli-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cto-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: The CTO cli
 Home-page: https://doc.cloudtechnologyoffice.com/ecs/latest
 License: Apache-2.0
 Author: CTO
 Author-email: support@cloudtechnologyoffice.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

