# Comparing `tmp/eip712_clearsign-2.0.0rc2.tar.gz` & `tmp/eip712_clearsign-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eip712_clearsign-2.0.0rc2.tar", last modified: Mon May 27 08:20:54 2024, max compression
+gzip compressed data, was "eip712_clearsign-2.0.0rc3.tar", last modified: Wed May 29 12:21:45 2024, max compression
```

## Comparing `eip712_clearsign-2.0.0rc2.tar` & `eip712_clearsign-2.0.0rc3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 08:20:54.118771 eip712_clearsign-2.0.0rc2/
--rw-r--r--   0 runner    (1001) runner    (1001)     1063 2024-05-27 08:20:01.000000 eip712_clearsign-2.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) runner    (1001)     2432 2024-05-27 08:20:54.118771 eip712_clearsign-2.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)     1968 2024-05-27 08:20:01.000000 eip712_clearsign-2.0.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 08:20:54.118771 eip712_clearsign-2.0.0rc2/eip712/
--rw-r--r--   0 runner    (1001) runner    (1001)    10263 2024-05-27 08:20:01.000000 eip712_clearsign-2.0.0rc2/eip712/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 08:20:54.118771 eip712_clearsign-2.0.0rc2/eip712_clearsign.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     2432 2024-05-27 08:20:54.000000 eip712_clearsign-2.0.0rc2/eip712_clearsign.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      265 2024-05-27 08:20:54.000000 eip712_clearsign-2.0.0rc2/eip712_clearsign.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-05-27 08:20:54.000000 eip712_clearsign-2.0.0rc2/eip712_clearsign.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-05-27 08:20:54.000000 eip712_clearsign-2.0.0rc2/eip712_clearsign.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        7 2024-05-27 08:20:54.000000 eip712_clearsign-2.0.0rc2/eip712_clearsign.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-05-27 08:20:54.118771 eip712_clearsign-2.0.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)      720 2024-05-27 08:20:01.000000 eip712_clearsign-2.0.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 08:20:54.118771 eip712_clearsign-2.0.0rc2/tests/
--rw-r--r--   0 runner    (1001) runner    (1001)    15343 2024-05-27 08:20:01.000000 eip712_clearsign-2.0.0rc2/tests/test_eip712.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-29 12:21:45.347486 eip712_clearsign-2.0.0rc3/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1063 2024-05-29 12:20:58.000000 eip712_clearsign-2.0.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)     2432 2024-05-29 12:21:45.347486 eip712_clearsign-2.0.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2024-05-29 12:20:58.000000 eip712_clearsign-2.0.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-29 12:21:45.343486 eip712_clearsign-2.0.0rc3/eip712/
+-rw-r--r--   0 runner    (1001) runner    (1001)    10365 2024-05-29 12:20:58.000000 eip712_clearsign-2.0.0rc3/eip712/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-29 12:21:45.347486 eip712_clearsign-2.0.0rc3/eip712_clearsign.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     2432 2024-05-29 12:21:45.000000 eip712_clearsign-2.0.0rc3/eip712_clearsign.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      265 2024-05-29 12:21:45.000000 eip712_clearsign-2.0.0rc3/eip712_clearsign.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-05-29 12:21:45.000000 eip712_clearsign-2.0.0rc3/eip712_clearsign.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-05-29 12:21:45.000000 eip712_clearsign-2.0.0rc3/eip712_clearsign.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        7 2024-05-29 12:21:45.000000 eip712_clearsign-2.0.0rc3/eip712_clearsign.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-05-29 12:21:45.347486 eip712_clearsign-2.0.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)      720 2024-05-29 12:20:58.000000 eip712_clearsign-2.0.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-29 12:21:45.347486 eip712_clearsign-2.0.0rc3/tests/
+-rw-r--r--   0 runner    (1001) runner    (1001)    15343 2024-05-29 12:20:58.000000 eip712_clearsign-2.0.0rc3/tests/test_eip712.py
```

### Comparing `eip712_clearsign-2.0.0rc2/LICENSE` & `eip712_clearsign-2.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `eip712_clearsign-2.0.0rc2/PKG-INFO` & `eip712_clearsign-2.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eip712-clearsign
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: Parse eip712 clear sign descriptors
 Home-page: https://github.com/LedgerHQ/python-eip712
 Author: Ledger
 Author-email: hello@ledger.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eip712_clearsign-2.0.0rc2/README.md` & `eip712_clearsign-2.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `eip712_clearsign-2.0.0rc2/eip712/__init__.py` & `eip712_clearsign-2.0.0rc3/eip712/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,48 +91,41 @@
 
 
 @dataclass
 class EIP712AmountJoinTokenFieldMapper(EIP712FieldMapper):
     TYPE_PREFIX: ClassVar[int] = 11
     format: ClassVar[EIP712Format] = EIP712Format.TOKEN
 
-    coin_ref: Optional[int]
+    coin_ref: int
 
     def additional_hash(self, version: EIP712Version) -> str:
         if version == EIP712Version.V1:
             return super().additional_hash(version)
         else:
-            coin_ref_hash = (
-                self.coin_ref.to_bytes(1, byteorder="big").hex()
-                if self.coin_ref is not None
-                else ""
+            return (
+                f"{self.field_path.encode('utf-8').hex()}"
+                f"{self.coin_ref.to_bytes(1, byteorder='big').hex()}"
             )
-            return f"{self.field_path.encode('utf-8').hex()}" f"{coin_ref_hash}"
 
 
 @dataclass
 class EIP712AmountJoinValueFieldMapper(EIP712FieldMapper):
     TYPE_PREFIX: ClassVar[int] = 22
     format: ClassVar[EIP712Format] = EIP712Format.AMOUNT
 
-    coin_ref: Optional[int]
+    coin_ref: int
 
     def additional_hash(self, version: EIP712Version) -> str:
         if version == EIP712Version.V1:
             return super().additional_hash(version)
         else:
-            coin_ref_hash = (
-                self.coin_ref.to_bytes(1, byteorder="big").hex()
-                if self.coin_ref is not None
-                else ""
-            )
             return (
                 f"{self.field_path.encode('utf-8').hex()}"
                 f"{self.display_name_hash}"
-                f"{coin_ref_hash}"
+                f"{self.coin_ref.to_bytes(1, byteorder='big').hex()}"
             )
 
 
 @dataclass
 class EIP712DatetimeFieldMapper(EIP712FieldMapper):
     TYPE_PREFIX: ClassVar[int] = 33
     format: ClassVar[EIP712Format] = EIP712Format.DATETIME
@@ -156,22 +149,30 @@
     assetPath: Optional[str] = None
     format: Optional[EIP712Format] = None
     coinRef: Optional[int] = None
 
     def mapper(self, **mapper_data) -> EIP712FieldMapper:
         match self.format:
             case EIP712Format.TOKEN:
+                if self.coinRef is None:
+                    raise ValueError(
+                        f"EIP712 amount token field should have coin_ref: {self}"
+                    )
                 return EIP712AmountJoinTokenFieldMapper(
                     field_path=self.path,
                     display_name=self.label,
                     coin_ref=self.coinRef,
                     **mapper_data,
                 )
 
             case EIP712Format.AMOUNT:
+                if self.coinRef is None:
+                    raise ValueError(
+                        f"EIP712 amount value should have coin_ref: {self}"
+                    )
                 return EIP712AmountJoinValueFieldMapper(
                     field_path=self.path,
                     display_name=self.label,
                     coin_ref=self.coinRef,
                     **mapper_data,
                 )
```

### Comparing `eip712_clearsign-2.0.0rc2/eip712_clearsign.egg-info/PKG-INFO` & `eip712_clearsign-2.0.0rc3/eip712_clearsign.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eip712-clearsign
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: Parse eip712 clear sign descriptors
 Home-page: https://github.com/LedgerHQ/python-eip712
 Author: Ledger
 Author-email: hello@ledger.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eip712_clearsign-2.0.0rc2/setup.py` & `eip712_clearsign-2.0.0rc3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="eip712-clearsign",
-    version="2.0.0rc2",
+    version="2.0.0rc3",
     url="https://github.com/LedgerHQ/python-eip712",
     author="Ledger",
     author_email="hello@ledger.com",
     description="Parse eip712 clear sign descriptors",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["pydantic"],
```

### Comparing `eip712_clearsign-2.0.0rc2/tests/test_eip712.py` & `eip712_clearsign-2.0.0rc3/tests/test_eip712.py`

 * *Files identical despite different names*

