# Comparing `tmp/pryvacy-0.1.0.tar.gz` & `tmp/pryvacy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pryvacy-0.1.0.tar", max compression
+gzip compressed data, was "pryvacy-0.1.1.tar", max compression
```

## Comparing `pryvacy-0.1.0.tar` & `pryvacy-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-05-29 05:18:42.280764 pryvacy-0.1.0/LICENSE
--rw-r--r--   0        0        0      503 2024-05-29 13:31:34.009014 pryvacy-0.1.0/README.md
--rw-r--r--   0        0        0      130 2024-05-29 13:39:09.638978 pryvacy-0.1.0/pryvacy/__init__.py
--rw-r--r--   0        0        0      101 2024-05-29 12:23:56.909325 pryvacy-0.1.0/pryvacy/access_policy.py
--rw-r--r--   0        0        0      441 2024-05-29 11:58:51.859440 pryvacy-0.1.0/pryvacy/context.py
--rw-r--r--   0        0        0       38 2024-05-29 12:36:03.369269 pryvacy-0.1.0/pryvacy/decorators/__init__.py
--rw-r--r--   0        0        0      443 2024-05-29 12:37:37.069260 pryvacy-0.1.0/pryvacy/decorators/access_decorators/__init__.py
--rw-r--r--   0        0        0      642 2024-05-29 13:08:24.269119 pryvacy-0.1.0/pryvacy/decorators/pyvacy_decorator/__init__.py
--rw-r--r--   0        0        0     2695 2024-05-29 13:25:50.009048 pryvacy-0.1.0/pryvacy/decorators/pyvacy_decorator/instance_methods.py
--rw-r--r--   0        0        0      785 2024-05-29 13:28:18.809035 pryvacy-0.1.0/pryvacy/decorators/pyvacy_decorator/nested_classes.py
--rw-r--r--   0        0        0      363 2024-05-29 13:05:26.419132 pryvacy-0.1.0/pryvacy/decorators/utils.py
--rw-r--r--   0        0        0      394 2024-05-29 14:38:18.738710 pryvacy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 pryvacy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 05:18:42.280764 pryvacy-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1948 2024-05-29 14:59:45.808618 pryvacy-0.1.1/README.md
+-rw-r--r--   0        0        0      134 2024-05-29 14:59:45.808618 pryvacy-0.1.1/pryvacy/__init__.py
+-rw-r--r--   0        0        0      101 2024-05-29 14:59:45.808618 pryvacy-0.1.1/pryvacy/access_policy.py
+-rw-r--r--   0        0        0      441 2024-05-29 14:59:45.808618 pryvacy-0.1.1/pryvacy/context.py
+-rw-r--r--   0        0        0       39 2024-05-29 14:59:45.808618 pryvacy-0.1.1/pryvacy/decorators/__init__.py
+-rw-r--r--   0        0        0      445 2024-05-29 14:59:45.808618 pryvacy-0.1.1/pryvacy/decorators/access_decorators/__init__.py
+-rw-r--r--   0        0        0      649 2024-05-29 14:59:45.808618 pryvacy-0.1.1/pryvacy/decorators/pryvacy_decorator/__init__.py
+-rw-r--r--   0        0        0     2698 2024-05-29 14:59:45.808618 pryvacy-0.1.1/pryvacy/decorators/pryvacy_decorator/instance_methods.py
+-rw-r--r--   0        0        0      791 2024-05-29 14:59:45.808618 pryvacy-0.1.1/pryvacy/decorators/pryvacy_decorator/nested_classes.py
+-rw-r--r--   0        0        0      364 2024-05-29 14:59:45.808618 pryvacy-0.1.1/pryvacy/decorators/utils.py
+-rw-r--r--   0        0        0      394 2024-05-29 14:59:45.808618 pryvacy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2399 1970-01-01 00:00:00.000000 pryvacy-0.1.1/PKG-INFO
```

### Comparing `pryvacy-0.1.0/LICENSE` & `pryvacy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pryvacy-0.1.0/pryvacy/decorators/pyvacy_decorator/__init__.py` & `pryvacy-0.1.1/pryvacy/decorators/pryvacy_decorator/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Type, TypeVar
 
-from pyvacy.decorators.pyvacy_decorator import instance_methods
-from pyvacy.decorators.pyvacy_decorator import nested_classes
+from pryvacy.decorators.pryvacy_decorator import instance_methods
+from pryvacy.decorators.pryvacy_decorator import nested_classes
 
 
 T = TypeVar('T')
-def pyvacy(cls: Type[T]) -> Type[T]:
-    if "@@_pyvacified" in pyvacy.__dict__:
+def pryvacy(cls: Type[T]) -> Type[T]:
+    if "@@_pyvacified" in pryvacy.__dict__:
         return cls
     setattr(cls, "@@_pyvacified", ())
 
     instance_methods.init(cls)
     nested_classes.init(cls)
     
     old_init_subclass = cls.__init_subclass__
     @classmethod
     def init_subclass_wrapper(cls, **kwargs):
-        pyvacy(cls)
+        pryvacy(cls)
         return old_init_subclass(**kwargs)
 
     setattr(cls, "__init_subclass__", init_subclass_wrapper)
         
     return cls
```

### Comparing `pryvacy-0.1.0/pryvacy/decorators/pyvacy_decorator/instance_methods.py` & `pryvacy-0.1.1/pryvacy/decorators/pryvacy_decorator/instance_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 from typing import Type
 
-from pyvacy.access_policy import AccessPolicy
-from pyvacy.context import reset_cls_ctx, set_cls_ctx, get_current_class
-from pyvacy.decorators.utils import get_access_policy 
+from pryvacy.access_policy import AccessPolicy
+from pryvacy.context import reset_cls_ctx, set_cls_ctx, get_current_class
+from pryvacy.decorators.utils import get_access_policy 
 
 
 def init(cls: Type):
     normal_methods = { name: method for name, method in inspect.getmembers(cls, inspect.isfunction) if not name.startswith("__") }
     
     for name, _method in normal_methods.items():
         match get_access_policy(_method):
```

### Comparing `pryvacy-0.1.0/pryvacy/decorators/pyvacy_decorator/nested_classes.py` & `pryvacy-0.1.1/pryvacy/decorators/pryvacy_decorator/nested_classes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import inspect
 from typing import Type
 
-from pyvacy.access_policy import AccessPolicy
-from pyvacy.decorators.utils import get_access_policy 
+from pryvacy.access_policy import AccessPolicy
+from pryvacy.decorators.utils import get_access_policy 
 
 
 def init(cls: Type):
-    from pyvacy.decorators.pyvacy_decorator import pyvacy
+    from pryvacy.decorators.pryvacy_decorator import pryvacy
 
     nested_classes = { name: obj for name, obj in inspect.getmembers(cls, inspect.isclass) if obj.__module__ == cls.__module__ }
 
     for name, nested_cls in nested_classes.items():
         match get_access_policy(nested_cls):
             case AccessPolicy.PUBLIC:
-                pyvacy(nested_cls)
+                pryvacy(nested_cls)
             case AccessPolicy.PRIVATE:
                 raise NotImplemented("Can not annotate nested classes with @private yet")
             case AccessPolicy.PROTECTED:
                 raise NotImplemented("Can not annotate nested classes with @protected yet")
```

