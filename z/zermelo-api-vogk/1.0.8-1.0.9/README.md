# Comparing `tmp/zermelo_api_vogk-1.0.8.tar.gz` & `tmp/zermelo_api_vogk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zermelo_api_vogk-1.0.8.tar", last modified: Thu May 23 22:15:36 2024, max compression
+gzip compressed data, was "zermelo_api_vogk-1.0.9.tar", last modified: Tue May 28 14:10:08 2024, max compression
```

## Comparing `zermelo_api_vogk-1.0.8.tar` & `zermelo_api_vogk-1.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 22:15:36.905723 zermelo_api_vogk-1.0.8/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1068 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.8/LICENSE
--rw-r--r--   0 klaas     (1000) klaas     (1000)     4065 2024-05-23 22:15:36.905723 zermelo_api_vogk-1.0.8/PKG-INFO
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3493 2024-05-23 22:15:35.000000 zermelo_api_vogk-1.0.8/README.md
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 22:15:36.889723 zermelo_api_vogk-1.0.8/app/
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 22:15:36.889723 zermelo_api_vogk-1.0.8/app/zermelo_api/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      567 2024-05-23 07:09:10.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/__init__.py
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 22:15:36.901723 zermelo_api_vogk-1.0.8/app/zermelo_api/src/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)        0 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/__init__.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3144 2024-05-23 08:08:40.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/appointments.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     4100 2024-05-23 07:09:10.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/branches.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1437 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/config.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      618 2024-05-17 10:07:35.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/credentials.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1556 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/groepen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      674 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/io_json.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1136 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/leerjaren.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     6132 2024-05-23 22:15:35.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/lesgroepen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      812 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/lokalen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      446 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/time_utils.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3786 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/users.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1806 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/vakdoclok.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     2291 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/vakken.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     5831 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/vaklessen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3657 2024-05-23 22:15:35.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/zermelo_api.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1523 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/zermelo_collection.py
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 22:15:36.905723 zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/
--rw-r--r--   0 klaas     (1000) klaas     (1000)     4065 2024-05-23 22:15:36.000000 zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/PKG-INFO
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      834 2024-05-23 22:15:36.000000 zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/SOURCES.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)        1 2024-05-23 22:15:36.000000 zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/dependency_links.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       15 2024-05-23 22:15:36.000000 zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/requires.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       12 2024-05-23 22:15:36.000000 zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/top_level.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       38 2024-05-23 22:15:36.905723 zermelo_api_vogk-1.0.8/setup.cfg
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      874 2024-05-23 22:15:35.000000 zermelo_api_vogk-1.0.8/setup.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-28 14:10:08.948022 zermelo_api_vogk-1.0.9/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1068 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.9/LICENSE
+-rw-r--r--   0 klaas     (1000) klaas     (1000)     4087 2024-05-28 14:10:08.948022 zermelo_api_vogk-1.0.9/PKG-INFO
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3515 2024-05-28 14:08:46.000000 zermelo_api_vogk-1.0.9/README.md
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-28 14:10:08.928021 zermelo_api_vogk-1.0.9/app/
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-28 14:10:08.932021 zermelo_api_vogk-1.0.9/app/zermelo_api/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      567 2024-05-23 07:09:10.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/__init__.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-28 14:10:08.944022 zermelo_api_vogk-1.0.9/app/zermelo_api/src/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)        0 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/__init__.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3144 2024-05-23 08:08:40.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/appointments.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     4177 2024-05-28 14:08:46.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/branches.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1437 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/config.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      618 2024-05-17 10:07:35.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/credentials.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1556 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/groepen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      674 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/io_json.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1136 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/leerjaren.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     6132 2024-05-23 22:15:35.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/lesgroepen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      812 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/lokalen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      446 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/time_utils.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3786 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/users.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1973 2024-05-28 14:08:46.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/vakdoclok.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     2291 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/vakken.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     5831 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/vaklessen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3657 2024-05-23 22:15:35.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/zermelo_api.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1523 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.9/app/zermelo_api/src/zermelo_collection.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-28 14:10:08.944022 zermelo_api_vogk-1.0.9/app/zermelo_api_vogk.egg-info/
+-rw-r--r--   0 klaas     (1000) klaas     (1000)     4087 2024-05-28 14:10:08.000000 zermelo_api_vogk-1.0.9/app/zermelo_api_vogk.egg-info/PKG-INFO
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      834 2024-05-28 14:10:08.000000 zermelo_api_vogk-1.0.9/app/zermelo_api_vogk.egg-info/SOURCES.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)        1 2024-05-28 14:10:08.000000 zermelo_api_vogk-1.0.9/app/zermelo_api_vogk.egg-info/dependency_links.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       15 2024-05-28 14:10:08.000000 zermelo_api_vogk-1.0.9/app/zermelo_api_vogk.egg-info/requires.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       12 2024-05-28 14:10:08.000000 zermelo_api_vogk-1.0.9/app/zermelo_api_vogk.egg-info/top_level.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       38 2024-05-28 14:10:08.948022 zermelo_api_vogk-1.0.9/setup.cfg
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      874 2024-05-28 14:08:46.000000 zermelo_api_vogk-1.0.9/setup.py
```

### Comparing `zermelo_api_vogk-1.0.8/LICENSE` & `zermelo_api_vogk-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/PKG-INFO` & `zermelo_api_vogk-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zermelo_api_vogk
-Version: 1.0.8
+Version: 1.0.9
 Summary: A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 Home-page: https://github.com/KlaasVogel/zermelo_api_vogk
 Author: Klaas Vogel
 Author-email: zermelo_api@klaasvogel.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
@@ -14,20 +14,21 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Provides-Extra: dev
 
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
-# V1.0.8
+# V1.0.9
  - async loading lesgroepen done
  - async loading appointments done
  - enabled packages in __init__
  - made generator for branches
  - bugfix: appointments, rooster
+ - enabled vakdocloks
 
 # V1.0.2
  - replacement of request for working with asyncio
  - first rough test if asyncio is working
  - TODO: refactor leerlingen (sort should be done later)
  - loading branches seems done.
  - Next check Lesgroepen en vakdocloks
```

### Comparing `zermelo_api_vogk-1.0.8/README.md` & `zermelo_api_vogk-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
-# V1.0.8
+# V1.0.9
  - async loading lesgroepen done
  - async loading appointments done
  - enabled packages in __init__
  - made generator for branches
  - bugfix: appointments, rooster
+ - enabled vakdocloks
 
 # V1.0.2
  - replacement of request for working with asyncio
  - first rough test if asyncio is working
  - TODO: refactor leerlingen (sort should be done later)
  - loading branches seems done.
  - Next check Lesgroepen en vakdocloks
```

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/__init__.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/__init__.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/appointments.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/appointments.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/branches.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/branches.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from .time_utils import get_date, get_year, datetime
 from .users import Leerlingen, Personeel
 from .leerjaren import Leerjaren
 from .groepen import Groepen
 from .lesgroepen import Lesgroepen
 from .vakken import Vakken
 from .lokalen import Lokalen
-
-# from .vakdoclok import get_vakdocloks, VakDocLoks
+from .vakdoclok import get_vakdocloks, VakDocLoks
 from dataclasses import dataclass, InitVar, field
 import asyncio
 import logging
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)
 
@@ -64,16 +63,18 @@
                 self.vakken,
                 self.groepen,
                 self.leerlingen,
                 self.personeel,
             )
         return False
 
-    # def get_vak_doc_loks(self, start: int, eind: int) -> VakDocLoks:
-    #     return get_vakdocloks(self.id, start, eind)
+    async def get_vak_doc_loks(self) -> VakDocLoks:
+        start = int(self.date.timestamp())
+        eind = start + 28 * 24 * 3600
+        return await get_vakdocloks(self.zermelo, self.id, start, eind)
 
 
 @dataclass
 class Branches(ZermeloCollection[Branch]):
     def __post_init__(self):
         super().__post_init__()
         self.type = Branch
```

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/config.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/config.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/credentials.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/credentials.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/groepen.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/groepen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/io_json.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/io_json.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/leerjaren.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/leerjaren.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/lesgroepen.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/lesgroepen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/lokalen.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/lokalen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/users.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/users.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/vakdoclok.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/vakdoclok.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-from .zermelo_api import ZermeloCollection
+from .zermelo_collection import ZermeloCollection, ZermeloAPI
 from dataclasses import dataclass, InitVar, field
 
 
 @dataclass
 class VakDocLokData:
     teachers: list[str]
     locationsOfBranch: list[int]  # lokalen
     choosableInDepartments: list[str]
 
 
-class DataVakDocLoks(ZermeloCollection, list[VakDocLokData]):
-    def __init__(self, id_branch: int, start: int, eind: int):
-        query = f"appointments?branchOfSchool={id_branch}&fields=locationsOfBranch,teachers,choosableInDepartments,&start={start}&end={eind}"
-        self.load_collection(query, VakDocLokData)
+@dataclass
+class DataVakDocLoks(ZermeloCollection[VakDocLokData]):
+    branch_id: InitVar[int] = 0
+    start: InitVar[int] = 0
+    eind: InitVar[int] = 0
+
+    def __post_init__(self, id_branch: int, start: int, eind: int):
+        self.query = f"appointments?branchOfSchool={id_branch}&fields=locationsOfBranch,teachers,choosableInDepartments,&start={start}&end={eind}"
+        self.type = VakDocLokData
 
 
 @dataclass
 class VakDocLok:
     id: int
     docenten: list[str] = field(default_factory=list)
     lokalen: list[int] = field(default_factory=list)
@@ -44,16 +49,17 @@
     def get(self, id: int) -> VakDocLok | bool:
         for vakdoclok in self:
             if vakdoclok.id == id:
                 return vakdoclok
         return False
 
 
-def get_vakdocloks(id_branch: int, start: int, eind: int):
-    vakdata = DataVakDocLoks(id_branch, start, eind)
+async def get_vakdocloks(zermelo: ZermeloAPI, id_branch: int, start: int, eind: int):
+    vakdata = DataVakDocLoks(zermelo, id_branch, start, eind)
+    await vakdata._init()
     vakdocloks = VakDocLoks()
     for data in vakdata:
         for id in data.choosableInDepartments:
             vakdoclok = vakdocloks.add(id)
             vakdoclok.add_docs(data.teachers)
             vakdoclok.add_loks(data.locationsOfBranch)
     return vakdocloks
```

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/vakken.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/vakken.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/vaklessen.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/vaklessen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/zermelo_api.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/zermelo_api.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api/src/zermelo_collection.py` & `zermelo_api_vogk-1.0.9/app/zermelo_api/src/zermelo_collection.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/PKG-INFO` & `zermelo_api_vogk-1.0.9/app/zermelo_api_vogk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zermelo_api_vogk
-Version: 1.0.8
+Version: 1.0.9
 Summary: A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 Home-page: https://github.com/KlaasVogel/zermelo_api_vogk
 Author: Klaas Vogel
 Author-email: zermelo_api@klaasvogel.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
@@ -14,20 +14,21 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Provides-Extra: dev
 
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
-# V1.0.8
+# V1.0.9
  - async loading lesgroepen done
  - async loading appointments done
  - enabled packages in __init__
  - made generator for branches
  - bugfix: appointments, rooster
+ - enabled vakdocloks
 
 # V1.0.2
  - replacement of request for working with asyncio
  - first rough test if asyncio is working
  - TODO: refactor leerlingen (sort should be done later)
  - loading branches seems done.
  - Next check Lesgroepen en vakdocloks
```

### Comparing `zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/SOURCES.txt` & `zermelo_api_vogk-1.0.9/app/zermelo_api_vogk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.8/setup.py` & `zermelo_api_vogk-1.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="zermelo_api_vogk",
-    version="1.0.8",
+    version="1.0.9",
     description="A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KlaasVogel/zermelo_api_vogk",
     author="Klaas Vogel",
```

