# Comparing `tmp/package-tea-one-1.0.0.tar.gz` & `tmp/package-tea-one-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/package-tea-one-1.0.0.tar", last modified: Mon Mar  4 03:00:54 2024, max compression
+gzip compressed data, was "dist/package-tea-one-1.0.1.tar", last modified: Wed May 29 07:44:51 2024, max compression
```

## Comparing `package-tea-one-1.0.0.tar` & `package-tea-one-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 03:00:54.770412 package-tea-one-1.0.0/
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1141 2024-03-04 03:00:54.769860 package-tea-one-1.0.0/PKG-INFO
--rw-r--r--   0 xiaofeng   (502) staff       (20)      155 2024-03-04 02:45:56.000000 package-tea-one-1.0.0/README.rst
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 03:00:54.766008 package-tea-one-1.0.0/package-tea-one/
--rw-r--r--   0 xiaofeng   (502) staff       (20)      126 2024-03-04 02:49:10.000000 package-tea-one-1.0.0/package-tea-one/__init__.py
--rw-r--r--   0 xiaofeng   (502) staff       (20)      505 2024-03-04 02:45:56.000000 package-tea-one-1.0.0/package-tea-one/main.py
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 03:00:54.769411 package-tea-one-1.0.0/package_tea_one.egg-info/
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1141 2024-03-04 03:00:54.000000 package-tea-one-1.0.0/package_tea_one.egg-info/PKG-INFO
--rw-r--r--   0 xiaofeng   (502) staff       (20)      265 2024-03-04 03:00:54.000000 package-tea-one-1.0.0/package_tea_one.egg-info/SOURCES.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)        1 2024-03-04 03:00:54.000000 package-tea-one-1.0.0/package_tea_one.egg-info/dependency_links.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       52 2024-03-04 03:00:54.000000 package-tea-one-1.0.0/package_tea_one.egg-info/requires.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       16 2024-03-04 03:00:54.000000 package-tea-one-1.0.0/package_tea_one.egg-info/top_level.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       38 2024-03-04 03:00:54.770491 package-tea-one-1.0.0/setup.cfg
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1458 2024-03-04 03:00:38.000000 package-tea-one-1.0.0/setup.py
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-29 07:44:51.000000 package-tea-one-1.0.1/
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1159 2024-05-29 07:44:51.000000 package-tea-one-1.0.1/PKG-INFO
+-rw-r--r--   0 xf.shen    (502) staff       (20)      148 2024-05-29 07:43:35.000000 package-tea-one-1.0.1/README.rst
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-29 07:44:51.000000 package-tea-one-1.0.1/package-tea-one/
+-rw-r--r--   0 xf.shen    (502) staff       (20)      126 2024-05-29 07:36:48.000000 package-tea-one-1.0.1/package-tea-one/__init__.py
+-rw-r--r--   0 xf.shen    (502) staff       (20)      505 2024-05-29 07:36:48.000000 package-tea-one-1.0.1/package-tea-one/main.py
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-29 07:44:51.000000 package-tea-one-1.0.1/package_tea_one.egg-info/
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1159 2024-05-29 07:44:51.000000 package-tea-one-1.0.1/package_tea_one.egg-info/PKG-INFO
+-rw-r--r--   0 xf.shen    (502) staff       (20)      265 2024-05-29 07:44:51.000000 package-tea-one-1.0.1/package_tea_one.egg-info/SOURCES.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)        1 2024-05-29 07:44:51.000000 package-tea-one-1.0.1/package_tea_one.egg-info/dependency_links.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       49 2024-05-29 07:44:51.000000 package-tea-one-1.0.1/package_tea_one.egg-info/requires.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       16 2024-05-29 07:44:51.000000 package-tea-one-1.0.1/package_tea_one.egg-info/top_level.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       38 2024-05-29 07:44:51.000000 package-tea-one-1.0.1/setup.cfg
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1445 2024-05-29 07:43:39.000000 package-tea-one-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `package-tea-one-1.0.0/setup.py` & `package-tea-one-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 from setuptools import find_packages
 
 with open("README.rst", "r") as f:
   long_description = f.read()
 
 
 setup(name='package-tea-one',  # 包名
-      version='1.0.0',  # 版本号
-      description='small package just example',
+      version='1.0.1',  # 版本号
+      description='example for pypi',
       long_description=long_description,
       author='hanyan_news',
       author_email='hanyan0572@gmail.com',
       url='https://github.com/hanyan007/package-tea-one.git',
-      install_requires=["package-tea-hanyan==1.0.3", "restful-dnspod-log==1.0.1"],
+      install_requires=["package-tea-one==1.0.0", "restful-dnspod-log==1.0.1"],
       project_urls={  # Optional
         "Source": 'https://github.com/hanyan007/package-tea-one.git',
       },
       license='BSD License',
       packages=find_packages(),
       platforms=["all"],
       classifiers=[
```

