# Comparing `tmp/django_firebird-2.2.2.tar.gz` & `tmp/django-firebird-2.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_firebird-2.2.2.tar", last modified: Wed May 29 14:35:15 2024, max compression
+gzip compressed data, was "dist/django-firebird-2.2a1.tar", last modified: Fri Jun 19 19:12:05 2020, max compression
```

## Comparing `django_firebird-2.2.2.tar` & `django-firebird-2.2a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 maxi      (1000) maxi      (1000)        0 2024-05-29 14:35:15.848064 django_firebird-2.2.2/
--rw-r--r--   0 maxi      (1000) maxi      (1000)     1553 2020-03-12 13:32:25.000000 django_firebird-2.2.2/LICENSE
--rw-r--r--   0 maxi      (1000) maxi      (1000)       35 2020-03-12 13:32:25.000000 django_firebird-2.2.2/MANIFEST.in
--rw-r--r--   0 maxi      (1000) maxi      (1000)     3753 2024-05-29 14:35:15.848064 django_firebird-2.2.2/PKG-INFO
--rw-rw-r--   0 maxi      (1000) maxi      (1000)     2852 2024-05-29 12:49:32.000000 django_firebird-2.2.2/README.rst
-drwxrwxr-x   0 maxi      (1000) maxi      (1000)        0 2024-05-29 14:35:15.848064 django_firebird-2.2.2/django_firebird.egg-info/
--rw-r--r--   0 maxi      (1000) maxi      (1000)     3753 2024-05-29 14:35:15.000000 django_firebird-2.2.2/django_firebird.egg-info/PKG-INFO
--rw-rw-r--   0 maxi      (1000) maxi      (1000)      498 2024-05-29 14:35:15.000000 django_firebird-2.2.2/django_firebird.egg-info/SOURCES.txt
--rw-rw-r--   0 maxi      (1000) maxi      (1000)        1 2024-05-29 14:35:15.000000 django_firebird-2.2.2/django_firebird.egg-info/dependency_links.txt
--rw-rw-r--   0 maxi      (1000) maxi      (1000)        1 2024-05-29 14:35:15.000000 django_firebird-2.2.2/django_firebird.egg-info/not-zip-safe
--rw-rw-r--   0 maxi      (1000) maxi      (1000)        9 2024-05-29 14:35:15.000000 django_firebird-2.2.2/django_firebird.egg-info/top_level.txt
-drwxrwxr-x   0 maxi      (1000) maxi      (1000)        0 2024-05-29 14:35:15.848064 django_firebird-2.2.2/firebird/
--rw-rw-r--   0 maxi      (1000) maxi      (1000)      137 2024-05-29 13:01:28.000000 django_firebird-2.2.2/firebird/__init__.py
--rw-rw-r--   0 maxi      (1000) maxi      (1000)    27001 2024-05-29 12:49:32.000000 django_firebird-2.2.2/firebird/base.py
--rw-rw-r--   0 maxi      (1000) maxi      (1000)      998 2024-05-29 12:49:32.000000 django_firebird-2.2.2/firebird/client.py
--rw-rw-r--   0 maxi      (1000) maxi      (1000)     1965 2022-04-26 00:08:14.000000 django_firebird-2.2.2/firebird/compiler.py
--rw-rw-r--   0 maxi      (1000) maxi      (1000)     5281 2024-05-29 12:49:32.000000 django_firebird-2.2.2/firebird/creation.py
--rw-rw-r--   0 maxi      (1000) maxi      (1000)     1267 2024-05-29 12:49:32.000000 django_firebird-2.2.2/firebird/expressions.py
--rw-rw-r--   0 maxi      (1000) maxi      (1000)     3022 2024-05-29 12:49:32.000000 django_firebird-2.2.2/firebird/features.py
--rw-rw-r--   0 maxi      (1000) maxi      (1000)    14858 2024-05-29 12:56:11.000000 django_firebird-2.2.2/firebird/introspection.py
--rw-rw-r--   0 maxi      (1000) maxi      (1000)    24735 2024-05-29 12:49:32.000000 django_firebird-2.2.2/firebird/operations.py
--rw-rw-r--   0 maxi      (1000) maxi      (1000)    42595 2024-05-29 13:00:15.000000 django_firebird-2.2.2/firebird/schema.py
--rw-rw-r--   0 maxi      (1000) maxi      (1000)      131 2022-04-26 00:08:14.000000 django_firebird-2.2.2/firebird/validation.py
--rw-rw-r--   0 maxi      (1000) maxi      (1000)     1317 2022-04-26 00:08:14.000000 django_firebird-2.2.2/firebird/version.py
--rw-rw-r--   0 maxi      (1000) maxi      (1000)       96 2024-05-29 14:35:15.848064 django_firebird-2.2.2/setup.cfg
--rw-rw-r--   0 maxi      (1000) maxi      (1000)     1514 2024-05-29 12:49:32.000000 django_firebird-2.2.2/setup.py
+drwxr-xr-x   0 maxi      (1000) maxi      (1000)        0 2020-06-19 19:12:05.000000 django-firebird-2.2a1/
+drwxr-xr-x   0 maxi      (1000) maxi      (1000)        0 2020-06-19 19:12:05.000000 django-firebird-2.2a1/django_firebird.egg-info/
+-rw-r--r--   0 maxi      (1000) maxi      (1000)        1 2020-06-19 19:12:04.000000 django-firebird-2.2a1/django_firebird.egg-info/dependency_links.txt
+-rw-r--r--   0 maxi      (1000) maxi      (1000)        1 2020-06-19 19:12:04.000000 django-firebird-2.2a1/django_firebird.egg-info/not-zip-safe
+-rw-r--r--   0 maxi      (1000) maxi      (1000)        9 2020-06-19 19:12:04.000000 django-firebird-2.2a1/django_firebird.egg-info/top_level.txt
+-rw-r--r--   0 maxi      (1000) maxi      (1000)     4666 2020-06-19 19:12:04.000000 django-firebird-2.2a1/django_firebird.egg-info/PKG-INFO
+-rw-r--r--   0 maxi      (1000) maxi      (1000)      498 2020-06-19 19:12:04.000000 django-firebird-2.2a1/django_firebird.egg-info/SOURCES.txt
+-rw-r--r--   0 maxi      (1000) maxi      (1000)       35 2020-03-12 13:32:25.000000 django-firebird-2.2a1/MANIFEST.in
+-rw-r--r--   0 maxi      (1000) maxi      (1000)     1553 2020-03-12 13:32:25.000000 django-firebird-2.2a1/LICENSE
+-rw-r--r--   0 maxi      (1000) maxi      (1000)     1464 2020-06-19 18:58:36.000000 django-firebird-2.2a1/setup.py
+-rw-r--r--   0 maxi      (1000) maxi      (1000)     4666 2020-06-19 19:12:05.000000 django-firebird-2.2a1/PKG-INFO
+-rw-r--r--   0 maxi      (1000) maxi      (1000)     2983 2020-06-19 19:07:47.000000 django-firebird-2.2a1/README.rst
+drwxr-xr-x   0 maxi      (1000) maxi      (1000)        0 2020-06-19 19:12:05.000000 django-firebird-2.2a1/firebird/
+-rw-r--r--   0 maxi      (1000) maxi      (1000)     5281 2020-06-19 17:35:34.000000 django-firebird-2.2a1/firebird/creation.py
+-rw-r--r--   0 maxi      (1000) maxi      (1000)    27001 2020-06-19 17:35:34.000000 django-firebird-2.2a1/firebird/base.py
+-rw-r--r--   0 maxi      (1000) maxi      (1000)      998 2020-03-12 13:32:25.000000 django-firebird-2.2a1/firebird/client.py
+-rw-r--r--   0 maxi      (1000) maxi      (1000)      131 2020-03-12 13:32:25.000000 django-firebird-2.2a1/firebird/validation.py
+-rw-r--r--   0 maxi      (1000) maxi      (1000)     3022 2020-06-19 17:35:34.000000 django-firebird-2.2a1/firebird/features.py
+-rw-r--r--   0 maxi      (1000) maxi      (1000)     1317 2020-03-12 13:32:25.000000 django-firebird-2.2a1/firebird/version.py
+-rw-r--r--   0 maxi      (1000) maxi      (1000)    42033 2020-06-19 17:35:34.000000 django-firebird-2.2a1/firebird/schema.py
+-rw-r--r--   0 maxi      (1000) maxi      (1000)    14091 2020-06-19 17:35:34.000000 django-firebird-2.2a1/firebird/introspection.py
+-rw-r--r--   0 maxi      (1000) maxi      (1000)     1965 2020-03-12 13:32:25.000000 django-firebird-2.2a1/firebird/compiler.py
+-rw-r--r--   0 maxi      (1000) maxi      (1000)     1267 2020-03-12 13:32:25.000000 django-firebird-2.2a1/firebird/expressions.py
+-rw-r--r--   0 maxi      (1000) maxi      (1000)    24614 2020-06-19 17:35:34.000000 django-firebird-2.2a1/firebird/operations.py
+-rw-r--r--   0 maxi      (1000) maxi      (1000)      137 2020-06-19 18:58:36.000000 django-firebird-2.2a1/firebird/__init__.py
+-rw-r--r--   0 maxi      (1000) maxi      (1000)       96 2020-06-19 19:12:05.000000 django-firebird-2.2a1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `django_firebird-2.2.2/LICENSE` & `django-firebird-2.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_firebird-2.2.2/README.rst` & `django-firebird-2.2a1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 ===============
 django-firebird
 ===============
 
 .. image:: https://img.shields.io/pypi/v/django-firebird.svg
     :target: https://pypi.python.org/pypi/django-firebird
 
+.. image:: https://caniusepython3.com/project/django-firebird.svg
+    :target: https://caniusepython3.com/project/django-firebird
+
 
 Firebird SQL backend for django
 -------------------------------
 
 **Repo Note**:
 The ``master`` branch is an *in development* version of django-firebird. This may be substantially different from the latest
 `release of django-firebird`_
@@ -49,33 +52,33 @@
 
 **Manual Installation**
 
 Instructions for Ubuntu/Debian
 I assume you have installed django from source with python setup.py install
 
 
-    cd /usr/local/lib/python3.8/dist-packages
+    cd /usr/local/lib/python2.7/dist-packages
 
     sudo git clone git://github.com/maxirobaina/django-firebird.git
 
     sudo ln -s django-firebird/firebird firebird
 
-    cd /usr/local/lib/python3.8/dist-packages/django/db/backends
+    cd /usr/local/lib/python2.7/dist-packages/django/db/backends
 
-    sudo ln -s /usr/local/lib/python3.8/dist-packages/django-firebird/firebird
+    sudo ln -s /usr/local/lib/python2.7/dist-packages/django-firebird/firebird
 
 Configuration
 -------------
 
 Modify your setting.py ::
 
     DATABASES = {
         'default': {
             'ENGINE' : 'firebird',
-            'NAME' : '/var/lib/firebird/3.0/data/django_firebird.fdb', # Path to database or db alias
+            'NAME' : '/var/lib/firebird/2.5/data/django_firebird.fdb', # Path to database or db alias
             'USER' : 'SYSDBA',           # Your db user
             'PASSWORD' : '*****',    # db user password
             'HOST' : '127.0.0.1',        # Your host machine
             'PORT' : '3050',             # If is empty, use default 3050
             #'OPTIONS' : {'charset':'ISO8859_1'}
         }
     }
```

### Comparing `django_firebird-2.2.2/firebird/base.py` & `django-firebird-2.2a1/firebird/base.py`

 * *Files identical despite different names*

### Comparing `django_firebird-2.2.2/firebird/client.py` & `django-firebird-2.2a1/firebird/client.py`

 * *Files identical despite different names*

### Comparing `django_firebird-2.2.2/firebird/compiler.py` & `django-firebird-2.2a1/firebird/compiler.py`

 * *Files identical despite different names*

### Comparing `django_firebird-2.2.2/firebird/creation.py` & `django-firebird-2.2a1/firebird/creation.py`

 * *Files identical despite different names*

### Comparing `django_firebird-2.2.2/firebird/expressions.py` & `django-firebird-2.2a1/firebird/expressions.py`

 * *Files identical despite different names*

### Comparing `django_firebird-2.2.2/firebird/features.py` & `django-firebird-2.2a1/firebird/features.py`

 * *Files identical despite different names*

### Comparing `django_firebird-2.2.2/firebird/introspection.py` & `django-firebird-2.2a1/firebird/introspection.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,20 +182,20 @@
             )
 
             # This query retrieves each field name and index type on the given table.
             tbl_name = "'%s'" % table_name.upper()
             cursor.execute("""
             SELECT
               LOWER(s.RDB$FIELD_NAME) AS field_name,
-
+    
               LOWER(case
                 when rc.RDB$CONSTRAINT_TYPE is not null then rc.RDB$CONSTRAINT_TYPE
                 else 'INDEX'
               end) AS constraint_type
-
+    
             FROM RDB$INDEX_SEGMENTS s
             LEFT JOIN RDB$INDICES i ON i.RDB$INDEX_NAME = s.RDB$INDEX_NAME
             LEFT JOIN RDB$RELATION_CONSTRAINTS rc ON rc.RDB$INDEX_NAME = s.RDB$INDEX_NAME
             WHERE i.RDB$RELATION_NAME = %s
             AND i.RDB$SEGMENT_COUNT = 1
             ORDER BY s.RDB$FIELD_POSITION
             """ % (tbl_name,))
@@ -246,15 +246,15 @@
             else 'INDEX'
           end AS constraint_type,
 
           case
             when s.RDB$FIELD_NAME is not null then s.RDB$FIELD_NAME
             else ''
           end AS field_name,
-
+          
           i2.RDB$RELATION_NAME AS references_table,
           s2.RDB$FIELD_NAME AS references_field,
           i.RDB$UNIQUE_FLAG,
           i.RDB$INDEX_TYPE,
           i.RDB$EXPRESSION_SOURCE as expression_source
         FROM RDB$INDEX_SEGMENTS s
         FULL JOIN RDB$INDICES i ON i.RDB$INDEX_NAME = s.RDB$INDEX_NAME
@@ -325,27 +325,12 @@
             where i.rdb$relation_name = %s
             and s.rdb$field_name = %s
             and rc.rdb$constraint_type is null
             order by s.rdb$field_position """ % (table, field,))
 
         return [index_name[0].strip() for index_name in cursor.fetchall()]
 
-    def _get_check_constraints(self, cursor, table_name, field_name):
-        table = "'%s'" % table_name.upper()
-        field = "'%s'" % field_name.upper()
-        cursor.execute("""
-            select distinct rc.rdb$constraint_name as check_constraint_name
-            from rdb$relation_constraints rc
-            join rdb$check_constraints cc on rc.rdb$constraint_name = cc.rdb$constraint_name
-            join rdb$triggers c on cc.rdb$trigger_name = c.rdb$trigger_name
-            join rdb$relation_fields rf on rc.rdb$relation_name = rf.rdb$relation_name
-            where rc.rdb$relation_name = %s
-            and rf.rdb$field_name = %s
-            and rc.rdb$constraint_type = 'CHECK'
-        """ % (table, field,))
-        return [cn[0].strip() for cn in cursor.fetchall()]
-
     def _name_to_index(self, cursor, table_name):
         """Return a dictionary of {field_name: field_index} for the given table.
            Indexes are 0-based.
         """
         return dict([(d[0], i) for i, d in enumerate(self.get_table_description(cursor, table_name))])
```

### Comparing `django_firebird-2.2.2/firebird/operations.py` & `django-firebird-2.2a1/firebird/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,33 +288,27 @@
                 value = force_text(value, encoding=db_charset, errors='replace')
             else:
                 value = force_text(value)
         return value
 
     def convert_binaryfield_value(self, value, expression, connection, context):
         if value is not None:
-            try:
-              value = force_bytes(value.read())
-            except:
-              value = force_bytes(value)
+            value = force_bytes(value)
         return value
 
     def convert_booleanfield_value(self, value, expression, connection, context):
         if value in (0, 1):
             value = bool(value)
         return value
 
     def convert_decimalfield_value(self, value, expression, connection, context):
         field = expression.field
 
         val = utils.format_number(value, field.max_digits, field.decimal_places)
-
-        if val is not None:
-            value = decimal.Decimal(val)
-
+        value = decimal.Decimal.from_float(float(val))
         return value
 
     def convert_ipfield_value(self, value, expression, connection, context):
         if value is not None:
             value = value.strip()
         return value
 
@@ -461,15 +455,15 @@
                     column_name = self.quote_name(f.column)
                     sequence_name = self.get_sequence_name(model._meta.db_table)
                     output.append(reset_value_sql % {'sequence_name': sequence_name,
                                                      'column_name': column_name,
                                                      'table_name': table_name})
                     break
             for f in model._meta.many_to_many:
-                if not f.remote_field.through:
+                if not f.rel.through:
                     table_name = self.quote_name(f.m2m_db_table())
                     column_name = self.quote_name(f.column)
                     sequence_name = get_autoinc_sequence_name(self, f.m2m_db_table())
                     output.append(reset_value_sql % {'sequence_name': sequence_name,
                                                      'column_name': column_name,
                                                      'table_name': table_name})
         return output
@@ -506,15 +500,15 @@
                     column_name = self.quote_name(f.column)
                     sequence_name = get_autoinc_sequence_name(self, model._meta.db_table)
                     procedure_name = get_reset_procedure_name(self, model._meta.db_table)
                     output.append(procedure_sql % locals())
                     procedures.append(procedure_name)
                     break
             for f in model._meta.many_to_many:
-                if not f.remote_field.through:
+                if not f.rel.through:
                     table_name = self.quote_name(f.m2m_db_table())
                     column_name = self.quote_name(f.column)
                     sequence_name = get_autoinc_sequence_name(self, f.m2m_db_table())
                     procedure_name = get_reset_procedure_name(self, f.m2m_db_table())
                     output.append(procedure_sql % locals())
                     procedures.append(procedure_name)
         for procedure in procedures:
```

### Comparing `django_firebird-2.2.2/firebird/schema.py` & `django-firebird-2.2a1/firebird/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     sql_create_hash_index = "CREATE INDEX %(name)s ON %(table)s computed by(hash(%(columns)s))"
     sql_create_unique_hash_index = "CREATE UNIQUE INDEX %(name)s ON %(table)s computed by(hash(%(columns)s))"
 
     def _alter_column_set_null(self, table_name, column_name, is_null):
         engine_ver = str(self.connection.connection.engine_version).split('.')
         if engine_ver and len(engine_ver) > 0 and int(engine_ver[0]) >= 3:
             sql = """
-                ALTER TABLE \"%(table_name)s\"
-                ALTER \"%(column)s\"
+                ALTER TABLE \"%(table_name)s\" 
+                ALTER \"%(column)s\" 
                 %(null_flag)s NOT NULL
             """
             null_flag = 'DROP' if is_null else 'SET'
         else:
             sql = """
                 UPDATE RDB$RELATION_FIELDS SET RDB$NULL_FLAG = %(null_flag)s
                 WHERE RDB$FIELD_NAME = '%(column)s'
@@ -233,20 +233,14 @@
         return create_index
 
     def _get_field_indexes(self, model, field):
         with self.connection.cursor() as cursor:
             indexes = self.connection.introspection._get_field_indexes(cursor, model._meta.db_table, field.column)
         return indexes
 
-    def _get_field_check_constraints(self, model, field):
-        with self.connection.cursor() as cursor:
-            db_table = model._meta.db_table
-            checks = self.connection.introspection._get_check_constraints(cursor, db_table, field.column)
-        return checks
-
     def remove_field(self, model, field):
         # If remove a AutoField, we need remove all related stuff
         # if isinstance(field, AutoField):
         if field.get_internal_type() in ("AutoField", "BigAutoField"):
             tbl = model._meta.db_table
             trg_name = self.connection.ops.get_sequence_trigger_name(tbl)
             self.execute('DROP TRIGGER %s' % trg_name)
@@ -254,19 +248,14 @@
             self.execute('DROP SEQUENCE %s' % seq_name)
 
         # If 'field' is a ForeingKey and It has defined extra indexes, delete that indexes (Github issue #70)
         for index_name in self._get_field_indexes(model, field):
             sql = self._delete_constraint_sql(self.sql_delete_index, model, index_name)
             self.execute(sql)
 
-        # If field has check constraint, then remove it first
-        for check_constraint_name in self._get_field_check_constraints(model, field):
-            sql = self._delete_constraint_sql(self.sql_delete_constraint, model, check_constraint_name)
-            self.execute(sql)
-
         super(DatabaseSchemaEditor, self).remove_field(model, field)
 
     def _alter_column_type_sql(self, table, old_field, new_field, new_type):
         # The Firebird does not support direct type change to BLOB,
         # therefore this action is divided into 4 stages.
         # Change through temp column.
         alter_blob_actions = []
@@ -882,8 +871,8 @@
             with TransactionContext(self.connection.connection.trans()) as tr:
                 try:
                     cur = tr.cursor()
                     cur.execute(str(sql), params)
                 except Exception as e:
                     raise e
         else:
-            super(DatabaseSchemaEditor, self).execute(sql, params)
+            super(DatabaseSchemaEditor, self).execute(sql, params)
```

### Comparing `django_firebird-2.2.2/firebird/version.py` & `django-firebird-2.2a1/firebird/version.py`

 * *Files identical despite different names*

### Comparing `django_firebird-2.2.2/setup.py` & `django-firebird-2.2a1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,25 +20,24 @@
     long_description=__doc__,
     license='BSD',
     author='Maximiliano Robaina',
     author_email='maxirobaina@gmail.com',
     url='https://github.com/maxirobaina/django-firebird',
     packages=find_packages(),
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
+        'Development Status :: 3 - Alpha',
         'Environment :: Web Environment',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
+        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Database',
         'Topic :: Internet :: WWW/HTTP',
     ],
     zip_safe=False,
     install_requires=[],
 )
```

