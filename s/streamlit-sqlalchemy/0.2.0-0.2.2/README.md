# Comparing `tmp/streamlit_sqlalchemy-0.2.0.tar.gz` & `tmp/streamlit_sqlalchemy-0.2.2.tar.gz`

## Comparing `streamlit_sqlalchemy-0.2.0.tar` & `streamlit_sqlalchemy-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/CONTRIBUTING
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/.streamlit/secrets.toml
--rw-r--r--   0        0        0    20991 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/assets/crud_create.png
--rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/assets/crud_update.png
--rw-r--r--   0        0        0  4919016 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/assets/streamlit-example-2023-12-31-16-12-91.gif
--rw-r--r--   0        0        0  3628434 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/assets/streamlit-example-2023-12-31-16-12-91.webm
--rw-r--r--   0        0        0  3360669 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/assets/streamlit-example-2024-01-06-13-01-36.gif
--rw-r--r--   0        0        0  2426792 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/assets/streamlit-example-2024-01-06-13-01-36.webm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/examples/__init__.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/examples/example.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/examples/example2.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/examples/models.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/src/streamlit_sqlalchemy/__init__.py
--rw-r--r--   0        0        0    21418 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/src/streamlit_sqlalchemy/mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/tests/objects.py
--rw-r--r--   0        0        0     8939 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/tests/streamlit_sqlalchemy/test_mixin.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/tests/streamlit_sqlalchemy/mixin/create_form.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/tests/streamlit_sqlalchemy/mixin/create_form_advanced.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/tests/streamlit_sqlalchemy/mixin/delete_button.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/tests/streamlit_sqlalchemy/mixin/delete_form.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/tests/streamlit_sqlalchemy/mixin/edit_button.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/tests/streamlit_sqlalchemy/mixin/update_form.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/tests/streamlit_sqlalchemy/mixin/update_form_except_m2o.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/tests/streamlit_sqlalchemy/mixin/update_select_form.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/LICENSE
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/README.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/CONTRIBUTING
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/.streamlit/secrets.toml
+-rw-r--r--   0        0        0    20991 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/assets/crud_create.png
+-rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/assets/crud_update.png
+-rw-r--r--   0        0        0  4919016 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/assets/streamlit-example-2023-12-31-16-12-91.gif
+-rw-r--r--   0        0        0  3628434 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/assets/streamlit-example-2023-12-31-16-12-91.webm
+-rw-r--r--   0        0        0  3360669 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/assets/streamlit-example-2024-01-06-13-01-36.gif
+-rw-r--r--   0        0        0  2426792 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/assets/streamlit-example-2024-01-06-13-01-36.webm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/examples/__init__.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/examples/example.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/examples/example2.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/examples/models.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/src/streamlit_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    21791 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/src/streamlit_sqlalchemy/mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/tests/objects.py
+-rw-r--r--   0        0        0     8939 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/tests/streamlit_sqlalchemy/test_mixin.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/tests/streamlit_sqlalchemy/mixin/create_form.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/tests/streamlit_sqlalchemy/mixin/create_form_advanced.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/tests/streamlit_sqlalchemy/mixin/delete_button.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/tests/streamlit_sqlalchemy/mixin/delete_form.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/tests/streamlit_sqlalchemy/mixin/edit_button.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/tests/streamlit_sqlalchemy/mixin/update_form.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/tests/streamlit_sqlalchemy/mixin/update_form_except_m2o.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/tests/streamlit_sqlalchemy/mixin/update_select_form.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/LICENSE
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/README.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.2/PKG-INFO
```

### Comparing `streamlit_sqlalchemy-0.2.0/CONTRIBUTING` & `streamlit_sqlalchemy-0.2.2/CONTRIBUTING`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/.github/workflows/python-publish.yml` & `streamlit_sqlalchemy-0.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/assets/crud_create.png` & `streamlit_sqlalchemy-0.2.2/assets/crud_create.png`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/assets/crud_update.png` & `streamlit_sqlalchemy-0.2.2/assets/crud_update.png`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/assets/streamlit-example-2023-12-31-16-12-91.gif` & `streamlit_sqlalchemy-0.2.2/assets/streamlit-example-2023-12-31-16-12-91.gif`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/assets/streamlit-example-2023-12-31-16-12-91.webm` & `streamlit_sqlalchemy-0.2.2/assets/streamlit-example-2023-12-31-16-12-91.webm`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/assets/streamlit-example-2024-01-06-13-01-36.gif` & `streamlit_sqlalchemy-0.2.2/assets/streamlit-example-2024-01-06-13-01-36.gif`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/assets/streamlit-example-2024-01-06-13-01-36.webm` & `streamlit_sqlalchemy-0.2.2/assets/streamlit-example-2024-01-06-13-01-36.webm`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/examples/example.py` & `streamlit_sqlalchemy-0.2.2/examples/example.py`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/examples/example2.py` & `streamlit_sqlalchemy-0.2.2/examples/example2.py`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/examples/models.py` & `streamlit_sqlalchemy-0.2.2/examples/models.py`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/src/streamlit_sqlalchemy/mixin.py` & `streamlit_sqlalchemy-0.2.2/src/streamlit_sqlalchemy/mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,17 @@
         with conn.session as session:
             query = (
                 session.query(cls).order_by(_st_order_by(cls)).filter_by(**filter_by)
             )
             return query.all()
 
     @classmethod
-    def st_create_form(cls, defaults: Optional[dict] = None, *, border: bool = False):
+    def st_create_form(
+        cls, defaults: Optional[dict] = None, *, border: bool = False
+    ) -> bool:
         """
         Renders a form to create a new object of this class.
 
         :param defaults: A dictionary of default values for the form.
         :param border: Whether or not to display a border around the form.
 
         Example:
@@ -195,14 +197,16 @@
                     if any(
                         hasattr(kwargs[field], sql_field)
                         for sql_field in ["foreign_keys", "_sa_instance_state"]
                     ):
                         kwargs[field] = kwargs[field].id
                 cls._st_create(**kwargs)
 
+        return submitted
+
     @classmethod
     def st_update_select_form(
         cls,
         filter_by: Optional[dict] = None,
         except_columns: Optional[list] = None,
         *,
         border: bool = False,
@@ -332,96 +336,104 @@
                     index = next(choices.index(c) for c in choices if c.id == value)
 
                 return st.selectbox(
                     label,
                     index=index,
                     options=choices,
                     format_func=_st_repr,
+                    help=column.doc,
                 )
 
             return selectbox
 
         if isinstance(column.type, SqlInteger):
             default = get_default_value(column, default=0)
 
             def number_input(label, value=None):
                 value = value if value is not None else default
-                return st.number_input(label, value=value, step=1)
+                return st.number_input(label, value=value, step=1, help=column.doc)
 
             return number_input
 
         if isinstance(column.type, Float):
             default = get_default_value(column, default=0.0)
 
             def float_input(label, value=None):
                 value = value if value is not None else default
-                return st.number_input(label, value=value, step=0.1)
+                return st.number_input(label, value=value, step=0.1, help=column.doc)
 
             return float_input
 
         if isinstance(column.type, Boolean):
             default = get_default_value(column)
 
             def boolean_select(label, value=None):
                 options = [True, False]
                 selected = value if value is not None else default
                 index = options.index(selected) if selected is not None else None
-                return st.selectbox(label, options=[True, False], index=index)
+                return st.selectbox(
+                    label, options=[True, False], index=index, help=column.doc
+                )
 
             return boolean_select
 
         if isinstance(column.type, DateTime):
             default = get_default_value(column, default=datetime.now())
 
             def datetime_input(label, value=None):
                 value = value if value is not None else default
                 value_date = value.date()
                 value_time = value.time().replace(minute=0, second=0, microsecond=0)
 
                 selected_date = st.date_input(label, value=value_date)
                 selected_time = st.time_input(
-                    label, value=value_time, label_visibility="collapsed"
+                    label,
+                    value=value_time,
+                    label_visibility="collapsed",
+                    help=column.doc,
                 )
 
                 assert isinstance(selected_date, date)
                 return datetime.combine(selected_date, selected_time)
 
             return datetime_input
 
         if isinstance(column.type, Date):
             default = get_default_value(column, default=date.today())
 
             def date_input(label, value=None):
                 value = value if value is not None else default
-                return st.date_input(label, value=value)
+                return st.date_input(label, value=value, help=column.doc)
 
             return date_input
 
         if isinstance(column.type, Time):
             default = get_default_value(column, default=datetime.now().time())
 
             def time_input(label, value=None):
                 value = value if value is not None else default
-                value = value.replace(minute=0, second=0, microsecond=0)
+                value = value.replace(
+                    minute=0, second=0, microsecond=0, help=column.doc
+                )
                 return st.time_input(label, value=value)
 
             return time_input
 
         default = get_default_value(column, default="")
         if isinstance(column.type, Text):
 
             def text_area(label, value=None):
                 value = value if value is not None else default
-                return st.text_area(label, value=value)
+                return st.text_area(label, value=value, help=column.doc)
 
             return text_area
 
         def text_input(label, value=None):
             value = value if value is not None else default
-            return st.text_input(label, value=value)
+            return st.text_input(label, value=value, help=column.doc)
 
         return text_input
 
     @classmethod
     def _st_get_class_by_tablename(cls, tablename: str):
         """
         Returns the class for the given tablename.
@@ -508,22 +520,22 @@
             label,
             on_click=_update,
             kwargs=values,
             key=f"edit_{self.__class__.__name__}_{self.id}_{unique_hash}",
             **kwargs,
         )
 
-    def st_delete_button(self, label: str = "Delete", **kwargs):
+    def st_delete_button(self, label: str = "Delete", **kwargs) -> bool:
         """
         Renders a button to delete this object.
 
         :param label: The label for the button.
         :param kwargs: Additional keyword arguments to pass to the button.
         """
-        st.button(
+        return st.button(
             label=label,
             on_click=self._st_session_delete,
             key=f"delete_{self.__class__.__name__}_{self.id}",
             **kwargs,
         )
 
     def st_update_form(
```

### Comparing `streamlit_sqlalchemy-0.2.0/tests/objects.py` & `streamlit_sqlalchemy-0.2.2/tests/objects.py`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/tests/streamlit_sqlalchemy/test_mixin.py` & `streamlit_sqlalchemy-0.2.2/tests/streamlit_sqlalchemy/test_mixin.py`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/LICENSE` & `streamlit_sqlalchemy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/README.md` & `streamlit_sqlalchemy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.0/pyproject.toml` & `streamlit_sqlalchemy-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "streamlit-sqlalchemy"
-version = "0.2.0"
+version = "0.2.2"
 authors = [{ name = "artygo8", email = "arthurgossuin@gmail.com" }]
 description = "Some templating for streamlit and sqlalchemy"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python :: 3",
```

### Comparing `streamlit_sqlalchemy-0.2.0/PKG-INFO` & `streamlit_sqlalchemy-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: streamlit-sqlalchemy
-Version: 0.2.0
+Version: 0.2.2
 Summary: Some templating for streamlit and sqlalchemy
 Project-URL: Homepage, https://github.com/artygo8/streamlit-sqlalchemy
 Project-URL: Issues, https://github.com/artygo8/streamlit-sqlalchemy/issues
 Author-email: artygo8 <arthurgossuin@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: database,sql,sqlalchemy,streamlit,templating
```

