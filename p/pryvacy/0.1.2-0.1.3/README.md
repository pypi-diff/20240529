# Comparing `tmp/pryvacy-0.1.2.tar.gz` & `tmp/pryvacy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pryvacy-0.1.2.tar", max compression
+gzip compressed data, was "pryvacy-0.1.3.tar", max compression
```

## Comparing `pryvacy-0.1.2.tar` & `pryvacy-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-05-29 05:18:42.280764 pryvacy-0.1.2/LICENSE
--rw-r--r--   0        0        0     1948 2024-05-29 14:59:45.808618 pryvacy-0.1.2/README.md
--rw-r--r--   0        0        0      134 2024-05-29 14:59:45.808618 pryvacy-0.1.2/pryvacy/__init__.py
--rw-r--r--   0        0        0      101 2024-05-29 14:59:45.808618 pryvacy-0.1.2/pryvacy/access_policy.py
--rw-r--r--   0        0        0      441 2024-05-29 14:59:45.808618 pryvacy-0.1.2/pryvacy/context.py
--rw-r--r--   0        0        0       39 2024-05-29 14:59:45.808618 pryvacy-0.1.2/pryvacy/decorators/__init__.py
--rw-r--r--   0        0        0      445 2024-05-29 14:59:45.808618 pryvacy-0.1.2/pryvacy/decorators/access_decorators/__init__.py
--rw-r--r--   0        0        0      649 2024-05-29 14:59:45.808618 pryvacy-0.1.2/pryvacy/decorators/pryvacy_decorator/__init__.py
--rw-r--r--   0        0        0     2568 2024-05-29 15:14:21.658544 pryvacy-0.1.2/pryvacy/decorators/pryvacy_decorator/instance_methods.py
--rw-r--r--   0        0        0      791 2024-05-29 14:59:45.808618 pryvacy-0.1.2/pryvacy/decorators/pryvacy_decorator/nested_classes.py
--rw-r--r--   0        0        0      364 2024-05-29 14:59:45.808618 pryvacy-0.1.2/pryvacy/decorators/utils.py
--rw-r--r--   0        0        0      394 2024-05-29 15:15:08.078540 pryvacy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2399 1970-01-01 00:00:00.000000 pryvacy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 05:18:42.280764 pryvacy-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1948 2024-05-29 14:59:45.808618 pryvacy-0.1.3/README.md
+-rw-r--r--   0        0        0      134 2024-05-29 14:59:45.808618 pryvacy-0.1.3/pryvacy/__init__.py
+-rw-r--r--   0        0        0      101 2024-05-29 14:59:45.808618 pryvacy-0.1.3/pryvacy/access_policy.py
+-rw-r--r--   0        0        0      381 2024-05-29 15:39:30.648423 pryvacy-0.1.3/pryvacy/context.py
+-rw-r--r--   0        0        0       39 2024-05-29 14:59:45.808618 pryvacy-0.1.3/pryvacy/decorators/__init__.py
+-rw-r--r--   0        0        0      445 2024-05-29 14:59:45.808618 pryvacy-0.1.3/pryvacy/decorators/access_decorators/__init__.py
+-rw-r--r--   0        0        0      649 2024-05-29 14:59:45.808618 pryvacy-0.1.3/pryvacy/decorators/pryvacy_decorator/__init__.py
+-rw-r--r--   0        0        0     2567 2024-05-29 16:03:54.388318 pryvacy-0.1.3/pryvacy/decorators/pryvacy_decorator/instance_methods.py
+-rw-r--r--   0        0        0      796 2024-05-29 16:00:05.598336 pryvacy-0.1.3/pryvacy/decorators/pryvacy_decorator/nested_classes.py
+-rw-r--r--   0        0        0      364 2024-05-29 14:59:45.808618 pryvacy-0.1.3/pryvacy/decorators/utils.py
+-rw-r--r--   0        0        0      394 2024-05-29 16:13:07.778275 pryvacy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2399 1970-01-01 00:00:00.000000 pryvacy-0.1.3/PKG-INFO
```

### Comparing `pryvacy-0.1.2/LICENSE` & `pryvacy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pryvacy-0.1.2/README.md` & `pryvacy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pryvacy-0.1.2/pryvacy/decorators/pryvacy_decorator/__init__.py` & `pryvacy-0.1.3/pryvacy/decorators/pryvacy_decorator/__init__.py`

 * *Files identical despite different names*

### Comparing `pryvacy-0.1.2/pryvacy/decorators/pryvacy_decorator/instance_methods.py` & `pryvacy-0.1.3/pryvacy/decorators/pryvacy_decorator/instance_methods.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,61 @@
 import inspect
 from typing import Type
 
 from pryvacy.access_policy import AccessPolicy
-from pryvacy.context import reset_cls_ctx, set_cls_ctx, get_current_class
+from pryvacy.context import pop_cls_ctx, push_cls_ctx, get_current_class
 from pryvacy.decorators.utils import get_access_policy 
 
 
 def init(cls: Type):
-    normal_methods = { name: method for name, method in inspect.getmembers(cls, inspect.isfunction) if not name.startswith("__") }
-    
+    normal_methods = { name: method for name, method in cls.__dict__.items() if not name.startswith("__") and inspect.isfunction(method) }
     for name, _method in normal_methods.items():
         match get_access_policy(_method):
             case AccessPolicy.PUBLIC:
                 def _local_public():
                     method = _method
                     def public_method(self, *args, **kwargs):
                         try:
-                            set_cls_ctx(cls)
+                            push_cls_ctx(cls)
                             return method(self, *args, **kwargs)
                         finally:
-                            reset_cls_ctx()
+                            pop_cls_ctx()
 
                     return public_method
 
                 setattr(cls, name, _local_public())
 
             case AccessPolicy.PRIVATE:
                 def _local_public():
                     method = _method
                     def private_method(self, *args, **kwargs):
                         current_class = get_current_class()
                         if not current_class or not (current_class == cls or cls.__dict__.get(current_class.__name__, None) == current_class):
                             raise Exception(f"'{name}' method of {cls.__name__} is marked as private")
 
                         try:
-                            set_cls_ctx(cls)
+                            push_cls_ctx(cls)
                             return method(self, *args, **kwargs)
                         finally:
-                            reset_cls_ctx()
+                            pop_cls_ctx()
 
                     return private_method
 
                 setattr(cls, name, _local_public())
 
             case AccessPolicy.PROTECTED:
                 def _local_protected():
                     method = _method
                     def protected_method(self, *args, **kwargs):
                         current_class = get_current_class()
                         if not current_class or not (issubclass(current_class, cls) or cls.__dict__.get(current_class.__name__, None) == current_class):
                             raise Exception(f"'{name}' method of {cls.__name__} is marked as protected")
 
                         try:
-                            set_cls_ctx(cls)
+                            push_cls_ctx(cls)
                             return method(self, *args, **kwargs)
                         finally:
-                            reset_cls_ctx()
+                            pop_cls_ctx()
 
                     return protected_method
 
                 setattr(cls, name, _local_protected())
```

### Comparing `pryvacy-0.1.2/pryvacy/decorators/pryvacy_decorator/nested_classes.py` & `pryvacy-0.1.3/pryvacy/decorators/pryvacy_decorator/nested_classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pryvacy.access_policy import AccessPolicy
 from pryvacy.decorators.utils import get_access_policy 
 
 
 def init(cls: Type):
     from pryvacy.decorators.pryvacy_decorator import pryvacy
 
-    nested_classes = { name: obj for name, obj in inspect.getmembers(cls, inspect.isclass) if obj.__module__ == cls.__module__ }
+    nested_classes = { name: obj for name, obj in cls.__dict__.items() if inspect.isclass(obj) and obj.__module__ == cls.__module__ }
 
     for name, nested_cls in nested_classes.items():
         match get_access_policy(nested_cls):
             case AccessPolicy.PUBLIC:
                 pryvacy(nested_cls)
             case AccessPolicy.PRIVATE:
                 raise NotImplemented("Can not annotate nested classes with @private yet")
```

### Comparing `pryvacy-0.1.2/PKG-INFO` & `pryvacy-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pryvacy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A set of access control descriptors for methods and nested classes
 Author: Huy-DNA
 Author-email: huydo862003@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

