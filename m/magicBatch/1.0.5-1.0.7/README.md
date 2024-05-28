# Comparing `tmp/magicBatch-1.0.5.tar.gz` & `tmp/magicBatch-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicBatch-1.0.5.tar", last modified: Mon Apr  1 01:23:22 2024, max compression
+gzip compressed data, was "magicBatch-1.0.7.tar", last modified: Tue May 28 22:52:42 2024, max compression
```

## Comparing `magicBatch-1.0.5.tar` & `magicBatch-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kbrulois   (501) staff       (20)        0 2024-04-01 01:23:22.436915 magicBatch-1.0.5/
--rw-r--r--   0 kbrulois   (501) staff       (20)      454 2024-04-01 01:23:22.436802 magicBatch-1.0.5/PKG-INFO
--rw-r--r--   0 kbrulois   (501) staff       (20)      652 2021-11-23 23:22:44.000000 magicBatch-1.0.5/README.txt
--rw-r--r--   0 kbrulois   (501) staff       (20)       79 2024-04-01 01:23:22.437157 magicBatch-1.0.5/setup.cfg
--rwxrwxrwx   0 kbrulois   (501) staff       (20)      799 2024-04-01 01:23:01.000000 magicBatch-1.0.5/setup.py
-drwxr-xr-x   0 kbrulois   (501) staff       (20)        0 2024-04-01 01:23:22.434215 magicBatch-1.0.5/src/
-drwxr-xr-x   0 kbrulois   (501) staff       (20)        0 2024-04-01 01:23:22.435067 magicBatch-1.0.5/src/magicBatch/
--rwxr-xr--   0 kbrulois   (501) staff       (20)     3130 2022-03-16 23:00:22.000000 magicBatch-1.0.5/src/magicBatch/MAGIC.py
--rw-r--r--   0 kbrulois   (501) staff       (20)     8566 2024-04-01 01:19:08.000000 magicBatch-1.0.5/src/magicBatch/MAGIC_core.py
--rw-rw-r--   0 kbrulois   (501) staff       (20)       68 2021-12-02 19:03:02.000000 magicBatch-1.0.5/src/magicBatch/__init__.py
-drwxr-xr-x   0 kbrulois   (501) staff       (20)        0 2024-04-01 01:23:22.436293 magicBatch-1.0.5/src/magicBatch.egg-info/
--rw-r--r--   0 kbrulois   (501) staff       (20)      454 2024-04-01 01:23:22.000000 magicBatch-1.0.5/src/magicBatch.egg-info/PKG-INFO
--rw-r--r--   0 kbrulois   (501) staff       (20)      298 2024-04-01 01:23:22.000000 magicBatch-1.0.5/src/magicBatch.egg-info/SOURCES.txt
--rw-r--r--   0 kbrulois   (501) staff       (20)        1 2024-04-01 01:23:22.000000 magicBatch-1.0.5/src/magicBatch.egg-info/dependency_links.txt
--rw-r--r--   0 kbrulois   (501) staff       (20)       80 2024-04-01 01:23:22.000000 magicBatch-1.0.5/src/magicBatch.egg-info/requires.txt
--rw-r--r--   0 kbrulois   (501) staff       (20)       11 2024-04-01 01:23:22.000000 magicBatch-1.0.5/src/magicBatch.egg-info/top_level.txt
+drwxr-xr-x   0 kbrulois   (501) staff       (20)        0 2024-05-28 22:52:42.345390 magicBatch-1.0.7/
+-rw-r--r--   0 kbrulois   (501) staff       (20)      454 2024-05-28 22:52:42.345311 magicBatch-1.0.7/PKG-INFO
+-rw-r--r--   0 kbrulois   (501) staff       (20)      652 2021-11-23 23:22:44.000000 magicBatch-1.0.7/README.txt
+-rw-r--r--   0 kbrulois   (501) staff       (20)       79 2024-05-28 22:52:42.345645 magicBatch-1.0.7/setup.cfg
+-rwxrwxrwx   0 kbrulois   (501) staff       (20)      799 2024-05-28 22:50:40.000000 magicBatch-1.0.7/setup.py
+drwxr-xr-x   0 kbrulois   (501) staff       (20)        0 2024-05-28 22:52:42.342635 magicBatch-1.0.7/src/
+drwxr-xr-x   0 kbrulois   (501) staff       (20)        0 2024-05-28 22:52:42.343738 magicBatch-1.0.7/src/magicBatch/
+-rwxr-xr--   0 kbrulois   (501) staff       (20)     3130 2022-03-16 23:00:22.000000 magicBatch-1.0.7/src/magicBatch/MAGIC.py
+-rw-r--r--   0 kbrulois   (501) staff       (20)     8569 2024-05-28 22:45:42.000000 magicBatch-1.0.7/src/magicBatch/MAGIC_core.py
+-rw-rw-r--   0 kbrulois   (501) staff       (20)       68 2021-12-02 19:03:02.000000 magicBatch-1.0.7/src/magicBatch/__init__.py
+drwxr-xr-x   0 kbrulois   (501) staff       (20)        0 2024-05-28 22:52:42.345027 magicBatch-1.0.7/src/magicBatch.egg-info/
+-rw-r--r--   0 kbrulois   (501) staff       (20)      454 2024-05-28 22:52:42.000000 magicBatch-1.0.7/src/magicBatch.egg-info/PKG-INFO
+-rw-r--r--   0 kbrulois   (501) staff       (20)      298 2024-05-28 22:52:42.000000 magicBatch-1.0.7/src/magicBatch.egg-info/SOURCES.txt
+-rw-r--r--   0 kbrulois   (501) staff       (20)        1 2024-05-28 22:52:42.000000 magicBatch-1.0.7/src/magicBatch.egg-info/dependency_links.txt
+-rw-r--r--   0 kbrulois   (501) staff       (20)       80 2024-05-28 22:52:42.000000 magicBatch-1.0.7/src/magicBatch.egg-info/requires.txt
+-rw-r--r--   0 kbrulois   (501) staff       (20)       11 2024-05-28 22:52:42.000000 magicBatch-1.0.7/src/magicBatch.egg-info/top_level.txt
```

### Comparing `magicBatch-1.0.5/README.txt` & `magicBatch-1.0.7/README.txt`

 * *Files identical despite different names*

### Comparing `magicBatch-1.0.5/setup.py` & `magicBatch-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import shutil
 from warnings import warn
 from distutils.core import setup
 
 
 setup(name='magicBatch',
-      version='1.0.5',
+      version='1.0.7',
       description='MAGICbatch',
       author='Kevin Brulois',
       author_email='kevin.brulois@gmail.com',
       package_dir={'': 'src'},
       packages=['magicBatch'],
       url='https://github.com/kbrulois/magicBatch',
       download_url='https://github.com/kbrulois/magicBatch/archive/refs/tags/v1.0.0.tar.gz',
```

### Comparing `magicBatch-1.0.5/src/magicBatch/MAGIC.py` & `magicBatch-1.0.7/src/magicBatch/MAGIC.py`

 * *Files identical despite different names*

### Comparing `magicBatch-1.0.5/src/magicBatch/MAGIC_core.py` & `magicBatch-1.0.7/src/magicBatch/MAGIC_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,27 +55,25 @@
         L = L.todense()
         if(isinstance(t, str)):
             t_param = t.split('_')
             t_param = [int(i) for i in t_param]
         data_new = multi_t_fast_impute(data, L = L, t = t_param, rescale_percent = rescale_percent, rescale_method = rescale_method)
         
     if csv_i != None:
-        data_new = dt.cbind(data_new)
+        data_new = dt.cbind([dt.Frame(i) for i in data_new])
         data_new.to_csv(csv_i)
     else:
         return(data_new)
 
 def run_pca(data, n_components=100, random=True):
-
-    solver = 'randomized'
-    if random != True:
-        solver = 'full'
-
-    pca = PCA(n_components=n_components, svd_solver=solver)
-    return pca.fit_transform(data)
+	solver = 'randomized'
+	if random != True:
+		solver = 'full'
+	pca = PCA(n_components=n_components, svd_solver=solver)
+	return pca.fit_transform(data)
 
 def multi_t_fast_impute(data, L, t, rescale_percent = 0, rescale_method = 'adaptive'):
 
     t_max = max(t)
 	
     if t_max >= 2: 
         L2 = np.matmul(L, L)
```

