# Comparing `tmp/jyhelper-1.2.4.tar.gz` & `tmp/jyhelper-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jyhelper-1.2.4.tar", last modified: Thu May 23 02:48:26 2024, max compression
+gzip compressed data, was "jyhelper-1.2.5.tar", last modified: Wed May 29 09:38:53 2024, max compression
```

## Comparing `jyhelper-1.2.4.tar` & `jyhelper-1.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 02:48:26.827283 jyhelper-1.2.4/
--rw-rw-rw-   0        0        0     1130 2024-05-23 02:48:26.826283 jyhelper-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      820 2023-11-17 09:46:48.000000 jyhelper-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 02:48:26.800707 jyhelper-1.2.4/jyhelper/
--rw-rw-rw-   0        0        0      385 2023-11-17 06:00:40.000000 jyhelper-1.2.4/jyhelper/__init__.py
--rw-rw-rw-   0        0        0     4455 2024-01-30 07:23:11.000000 jyhelper-1.2.4/jyhelper/common.py
--rw-rw-rw-   0        0        0    15771 2024-05-23 02:43:07.000000 jyhelper-1.2.4/jyhelper/db.py
--rw-rw-rw-   0        0        0     5284 2024-01-05 03:38:54.000000 jyhelper-1.2.4/jyhelper/feishuRobot.py
--rw-rw-rw-   0        0        0     1888 2024-05-21 03:10:31.000000 jyhelper-1.2.4/jyhelper/file.py
--rw-rw-rw-   0        0        0     4651 2024-04-30 03:17:37.000000 jyhelper-1.2.4/jyhelper/timeHelper.py
-drwxrwxrwx   0        0        0        0 2024-05-23 02:48:26.824055 jyhelper-1.2.4/jyhelper.egg-info/
--rw-rw-rw-   0        0        0     1130 2024-05-23 02:48:26.000000 jyhelper-1.2.4/jyhelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2024-05-23 02:48:26.000000 jyhelper-1.2.4/jyhelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 02:48:26.000000 jyhelper-1.2.4/jyhelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-23 02:48:26.000000 jyhelper-1.2.4/jyhelper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 02:48:26.000000 jyhelper-1.2.4/jyhelper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 02:48:26.827283 jyhelper-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      718 2024-05-23 02:47:35.000000 jyhelper-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:38:53.767338 jyhelper-1.2.5/
+-rw-rw-rw-   0        0        0     1130 2024-05-29 09:38:53.767338 jyhelper-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      820 2023-11-17 09:46:48.000000 jyhelper-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 09:38:53.748576 jyhelper-1.2.5/jyhelper/
+-rw-rw-rw-   0        0        0      385 2023-11-17 06:00:40.000000 jyhelper-1.2.5/jyhelper/__init__.py
+-rw-rw-rw-   0        0        0     4455 2024-01-30 07:23:11.000000 jyhelper-1.2.5/jyhelper/common.py
+-rw-rw-rw-   0        0        0    15771 2024-05-23 02:43:07.000000 jyhelper-1.2.5/jyhelper/db.py
+-rw-rw-rw-   0        0        0     5284 2024-01-05 03:38:54.000000 jyhelper-1.2.5/jyhelper/feishuRobot.py
+-rw-rw-rw-   0        0        0     1888 2024-05-21 03:10:31.000000 jyhelper-1.2.5/jyhelper/file.py
+-rw-rw-rw-   0        0        0     4752 2024-05-29 09:37:08.000000 jyhelper-1.2.5/jyhelper/timeHelper.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:38:53.763927 jyhelper-1.2.5/jyhelper.egg-info/
+-rw-rw-rw-   0        0        0     1130 2024-05-29 09:38:53.000000 jyhelper-1.2.5/jyhelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-05-29 09:38:53.000000 jyhelper-1.2.5/jyhelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 09:38:53.000000 jyhelper-1.2.5/jyhelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-29 09:38:53.000000 jyhelper-1.2.5/jyhelper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 09:38:53.000000 jyhelper-1.2.5/jyhelper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 09:38:53.768338 jyhelper-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      718 2024-05-29 09:37:29.000000 jyhelper-1.2.5/setup.py
```

### Comparing `jyhelper-1.2.4/PKG-INFO` & `jyhelper-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jyhelper
-Version: 1.2.4
+Version: 1.2.5
 Summary: 各种实用、常用的小函数、类
 Home-page: https://pypi.org/project/jyhelper/
 Author: JY
 Author-email: your-email@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.0
```

### Comparing `jyhelper-1.2.4/README.md` & `jyhelper-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.4/jyhelper/common.py` & `jyhelper-1.2.5/jyhelper/common.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.4/jyhelper/db.py` & `jyhelper-1.2.5/jyhelper/db.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.4/jyhelper/feishuRobot.py` & `jyhelper-1.2.5/jyhelper/feishuRobot.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.4/jyhelper/file.py` & `jyhelper-1.2.5/jyhelper/file.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.4/jyhelper/timeHelper.py` & `jyhelper-1.2.5/jyhelper/timeHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,12 +127,17 @@
     def checkIsDate(date):
         try:
             time.strptime(date, '%Y-%m-%d %H:%M:%S')
             return True
         except ValueError:
             return False
 
+    @staticmethod
+    def sleep(seconds):
+        time.sleep(seconds)
+
 
 if __name__ == '__main__':
     day = '2023-11-12'
     print(timeHelper.getWeekFirstDay(day=day), timeHelper.getWeekEndDay(day=day))
+    timeHelper.sleep(10)
     print(timeHelper.getWeekJi(day))
```

### Comparing `jyhelper-1.2.4/jyhelper.egg-info/PKG-INFO` & `jyhelper-1.2.5/jyhelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jyhelper
-Version: 1.2.4
+Version: 1.2.5
 Summary: 各种实用、常用的小函数、类
 Home-page: https://pypi.org/project/jyhelper/
 Author: JY
 Author-email: your-email@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.0
```

### Comparing `jyhelper-1.2.4/setup.py` & `jyhelper-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Time : 2023/11/08 18:38 
 # @Author : JY
 
 from setuptools import setup
 
 setup(
     name='jyhelper',
-    version='1.2.4',
+    version='1.2.5',
     packages=['jyhelper'],
     install_requires=[
         'pymysql',
         'requests'
     ],
     description='各种实用、常用的小函数、类',
     long_description=open('README.md',encoding='utf-8').read(),  # 详细描述，通常从 README.md 中读取
```

