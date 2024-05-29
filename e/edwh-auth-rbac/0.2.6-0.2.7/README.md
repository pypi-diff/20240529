# Comparing `tmp/edwh_auth_rbac-0.2.6.tar.gz` & `tmp/edwh_auth_rbac-0.2.7.tar.gz`

## Comparing `edwh_auth_rbac-0.2.6.tar` & `edwh_auth_rbac-0.2.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/CHANGELOG.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/.gitignore
--rw-r--r--   0        0        0     9928 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/class_index.html
--rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/coverage_html_cb_da166b87.js
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/favicon_32_cb_58284776.png
--rw-r--r--   0        0        0    36693 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/function_index.html
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/keybd_closed_cb_ce680311.png
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/status.json
--rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/style_cb_8e611ae1.css
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/z_438b44bce6437be6___init___py.html
--rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/z_438b44bce6437be6_helpers_py.html
--rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/z_438b44bce6437be6_migrations_py.html
--rw-r--r--   0        0        0   109622 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/z_438b44bce6437be6_model_py.html
--rw-r--r--   0        0        0    61317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/z_438b44bce6437be6_rbac_py.html
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/z_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0    59418 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/htmlcov/z_a44f0ac069e85531_test_rbac_py.html
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/src/edwh_auth_rbac/__init__.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/src/edwh_auth_rbac/helpers.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/src/edwh_auth_rbac/migrations.py
--rw-r--r--   0        0        0    13788 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/src/edwh_auth_rbac/model.py
--rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/src/edwh_auth_rbac/rbac.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/tests/test_migrate.py
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/tests/test_rbac.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/.gitignore
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/README.md
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/CHANGELOG.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/.gitignore
+-rw-r--r--   0        0        0     9928 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/class_index.html
+-rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/coverage_html_cb_da166b87.js
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/favicon_32_cb_58284776.png
+-rw-r--r--   0        0        0    36693 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/function_index.html
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/keybd_closed_cb_ce680311.png
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/status.json
+-rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/style_cb_8e611ae1.css
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6___init___py.html
+-rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_helpers_py.html
+-rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_migrations_py.html
+-rw-r--r--   0        0        0   109622 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_model_py.html
+-rw-r--r--   0        0        0    61317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_rbac_py.html
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/z_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0    59418 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/z_a44f0ac069e85531_test_rbac_py.html
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/helpers.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/migrations.py
+-rw-r--r--   0        0        0    14285 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/model.py
+-rw-r--r--   0        0        0     8098 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/rbac.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/tests/__init__.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/tests/test_migrate.py
+-rw-r--r--   0        0        0     7070 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/tests/test_rbac.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/.gitignore
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/README.md
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/PKG-INFO
```

### Comparing `edwh_auth_rbac-0.2.6/CHANGELOG.md` & `edwh_auth_rbac-0.2.7/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.2.7 (2024-05-29)
+
+### Fix
+
+* Don't autocommit within this library; raise errors from validate_ result ([`b203e46`](https://github.com/educationwarehouse/edwh-auth-rbac/commit/b203e46380e3b0338375c5cbd978fcf6eec5c561))
+
 ## v0.2.6 (2024-05-29)
 
 ### Fix
 
 * Make ruff happier ([`22b12e0`](https://github.com/educationwarehouse/edwh-auth-rbac/commit/22b12e03d0556be64990544cfc16ef2fdc46f73a))
 * You can provide a custom gid to add_identity/add_item and password is optional for items ([`986175b`](https://github.com/educationwarehouse/edwh-auth-rbac/commit/986175b7be37aec8559c5d2130082533be15e31f))
```

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/class_index.html` & `edwh_auth_rbac-0.2.7/htmlcov/class_index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/coverage_html_cb_da166b87.js` & `edwh_auth_rbac-0.2.7/htmlcov/coverage_html_cb_da166b87.js`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/favicon_32_cb_58284776.png` & `edwh_auth_rbac-0.2.7/htmlcov/favicon_32_cb_58284776.png`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/function_index.html` & `edwh_auth_rbac-0.2.7/htmlcov/function_index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/index.html` & `edwh_auth_rbac-0.2.7/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/keybd_closed_cb_ce680311.png` & `edwh_auth_rbac-0.2.7/htmlcov/keybd_closed_cb_ce680311.png`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/status.json` & `edwh_auth_rbac-0.2.7/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/style_cb_8e611ae1.css` & `edwh_auth_rbac-0.2.7/htmlcov/style_cb_8e611ae1.css`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/z_438b44bce6437be6___init___py.html` & `edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6___init___py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/z_438b44bce6437be6_helpers_py.html` & `edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_helpers_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/z_438b44bce6437be6_migrations_py.html` & `edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_migrations_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/z_438b44bce6437be6_model_py.html` & `edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_model_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/z_438b44bce6437be6_rbac_py.html` & `edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_rbac_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/z_a44f0ac069e85531___init___py.html` & `edwh_auth_rbac-0.2.7/htmlcov/z_a44f0ac069e85531___init___py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/htmlcov/z_a44f0ac069e85531_test_rbac_py.html` & `edwh_auth_rbac-0.2.7/htmlcov/z_a44f0ac069e85531_test_rbac_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/src/edwh_auth_rbac/migrations.py` & `edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/migrations.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/src/edwh_auth_rbac/model.py` & `edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,40 +212,44 @@
     object_type: Optional[ObjectTypes] = None,
 ) -> str:
     """paramaters name and firstname are equal."""
     email = email.lower().strip()
     if object_type is None:
         raise ValueError("object_type parameter expected")
     object_id = gid or uuid.uuid4()
-    db.identity.validate_and_insert(
+    result = db.identity.validate_and_insert(
         object_id=object_id,
         object_type=object_type,
         email=email,
         firstname=name or firstname or None,
         fullname=fullname,
         encoded_password=Password.encode(password) if password else None,
     )
-    db.commit()
+
+    if e := result.get("errors"):
+        raise ValueError(e)
+
+    # db.commit()
     for key in member_of:
         group_id = key_lookup(db, key, "group")
         if get_group(db, group_id):
             # check each group if it exists.
             add_membership(db, identity_key=object_id, group_key=group_id)
-    db.commit()
+    # db.commit()
     return str(object_id)
 
 
 def add_group(db: DAL, email: str, name: str, member_of: list[IdentityKey]):
     return add_identity(db, email, member_of, name=name, object_type="group")
 
 
 def remove_identity(db: DAL, object_id: IdentityKey):
     removed = db(db.identity.object_id == object_id).delete()
     # todo: remove permissions and group memberships
-    db.commit()
+    # db.commit()
     return removed > 0
 
 
 def get_identity(db: DAL, key: IdentityKey | None, object_type: Optional[ObjectTypes] = None) -> Identity | None:
     """
     :param db: dal db connection
     :param key: can be the email, id, or object_id
@@ -301,28 +305,30 @@
         raise ValueError(f"invalid identity_oid key: {identity_key}")
     group = get_group(db, group_key)
     if not group:
         raise ValueError(f"invalid group key: {group_key}")
     query = db.membership.subject == identity_oid
     query &= db.membership.member_of == group.object_id
     if db(query).count() == 0:
-        db.membership.validate_and_insert(
+        result = db.membership.validate_and_insert(
             subject=identity_oid,
             member_of=group.object_id,
         )
-    db.commit()
+        if e := result.get("errors"):
+            raise ValueError(e)
+    # db.commit()
 
 
 def remove_membership(db: DAL, identity_key: IdentityKey, group_key: IdentityKey) -> int:
     identity = get_identity(db, identity_key)
     group = get_group(db, group_key)
     query = db.membership.subject == identity.object_id
     query &= db.membership.member_of == group.object_id
     deleted = db(query).delete()
-    db.commit()
+    # db.commit()
     return deleted
 
 
 def get_memberships(db: DAL, object_id: IdentityKey, bare: bool = True):
     query = db.recursive_memberships.root == object_id
     fields = [db.recursive_memberships.object_id, db.recursive_memberships.object_type] if bare else []
     return db(query).select(*fields)
@@ -350,22 +356,24 @@
         print(
             "{privilege} permission already granted to {user_or_group_key} on {target_oid} @ {starts} ".format(
                 **locals()
             )
         )
         # print(db._lastsql)
         return
-    db.permission.validate_and_insert(
+    result = db.permission.validate_and_insert(
         privilege=privilege,
         identity_object_id=identity_oid,
         target_object_id=target_oid,
         starts=starts,
         ends=ends,
     )
-    db.commit()
+    if e := result.get("errors"):
+        raise ValueError(e)
+    # db.commit()
 
 
 def remove_permission(
     db: DAL, identity_key: IdentityKey, target_oid: IdentityKey, privilege: str, when: When | None = DEFAULT
 ) -> bool:
     identity_oid = key_lookup(db, identity_key)
     if when is DEFAULT:
@@ -376,15 +384,15 @@
     permission = db.permission
     query = permission.identity_object_id == identity_oid
     query &= permission.target_object_id == target_oid
     query &= permission.privilege == privilege
     query &= permission.starts <= when
     query &= permission.ends >= when
     result = db(query).delete() > 0
-    db.commit()
+    # db.commit()
     # print(db._lastsql)
     return result
 
 
 def with_alias(db: DAL, source: Table, alias: str) -> Table:
     other = copy.copy(source)
     other["ALL"] = SQLALL(other)
@@ -424,8 +432,19 @@
     query = left.root == root_oid
     query &= right.root == target_oid
     query &= permission.identity_object_id == left.object_id
     query &= permission.target_object_id == right.object_id
     query &= permission.privilege == privilege
     query &= permission.starts <= when
     query &= permission.ends >= when
+
+    if row := db(permission).select().first():
+        identity = db.identity(object_id=row.identity_object_id)
+        target = db.identity(object_id=row.target_object_id)
+
+        print(
+            row,
+            identity,
+            target,
+        )
+
     return db(query).count() > 0
```

### Comparing `edwh_auth_rbac-0.2.6/src/edwh_auth_rbac/rbac.py` & `edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/rbac.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         user.update_record(
             email=email.lower().strip() if email else user.email,
             firstname=name if name else firstname if firstname else user.firstname,
             lastname=lastname if lastname else user.lastname,
             fullname=fullname if fullname else user.fullname,
             password=Password.encode(password) if password else user.encoded_password,
         )
-        self.db.commit()
+        # self.# db.commit()
 
     def get_user(self, key: IdentityKey, return_memberhips: bool = False) -> UserDict:
         rec = model.get_user(self.db, key)
         result: UserDict = dict(
             object_id=rec.object_id,
             email=rec.email,
             firstname=rec.firstname,
```

### Comparing `edwh_auth_rbac-0.2.6/tests/test_migrate.py` & `edwh_auth_rbac-0.2.7/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/tests/test_rbac.py` & `edwh_auth_rbac-0.2.7/tests/test_rbac.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 @pytest.fixture(scope="module")
 def database(tmpdir):
     class Database:
         def __enter__(self):
             self.db = DAL("sqlite://auth_rbac.sqlite", folder=tmpdir)
 
-            settings = dict(allowed_types=["user", "group"], migrate=True)
+            settings = dict(allowed_types=["user", "group", "item"], migrate=True)
 
             define_auth_rbac_model(self.db, settings)
             rbac_views(self.db)
             return self.db
 
         def __exit__(self, exc_type, exc_value, traceback):
             self.db.close()
@@ -141,7 +141,21 @@
             store[name] = rbac.add_user("article_" + name + "@test.nl", name, "subarticle", "", [])["object_id"]
             rbac.add_membership(store[name], store.subarticles)
         assert rbac.has_permission(store.nested_admin, store.s, "read") is True
 
     def test_removing_a_nested_group(self, rbac, store):
         rbac.remove_membership(store.nested_admin, store.subadmins)
         assert rbac.has_permission(store.nested_admin, store.s, "read") is False
+
+    def test_permission_flow(self, rbac):
+        users = rbac.add_group("users@internal", "Users", [])
+        items = rbac.add_group("items@internal", "Items", [])
+        user = rbac.add_user("test@example", "Test", "Test Example", "secure", [users])
+        item_gid = str(uuid.uuid4())
+
+        item = rbac.add_item(f"@{item_gid}", item_gid, [items], gid=item_gid)
+
+        assert item["object_id"] == item_gid
+
+        rbac.add_permission(users, item_gid, "read")
+
+        assert rbac.has_permission(user, item_gid, "read")
```

### Comparing `edwh_auth_rbac-0.2.6/pyproject.toml` & `edwh_auth_rbac-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.6/PKG-INFO` & `edwh_auth_rbac-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: edwh-auth-rbac
-Version: 0.2.6
+Version: 0.2.7
 Summary: Recursive Memberships and Permissions for the Education Warehouse Authentication System
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-auth-rbac#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-auth-rbac/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-auth-rbac
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 Keywords: edwh,omgeving,whitelabel
```

