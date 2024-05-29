# Comparing `tmp/desgld-0.1.4.tar.gz` & `tmp/desgld-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desgld-0.1.4.tar", last modified: Fri May  3 23:52:13 2024, max compression
+gzip compressed data, was "desgld-0.1.6.tar", last modified: Wed May 29 19:13:59 2024, max compression
```

## Comparing `desgld-0.1.4.tar` & `desgld-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 23:52:13.322524 desgld-0.1.4/
--rw-r--r--   0 macpc      (501) staff       (20)     1079 2024-04-29 20:32:35.000000 desgld-0.1.4/LICENSE
--rw-r--r--   0 macpc      (501) staff       (20)      773 2024-05-03 23:52:13.321979 desgld-0.1.4/PKG-INFO
--rw-r--r--   0 macpc      (501) staff       (20)      228 2024-04-29 22:08:43.000000 desgld-0.1.4/README.md
--rw-r--r--   0 macpc      (501) staff       (20)       79 2024-04-29 20:32:35.000000 desgld-0.1.4/pyproject.toml
--rw-r--r--   0 macpc      (501) staff       (20)       38 2024-05-03 23:52:13.322618 desgld-0.1.4/setup.cfg
--rw-r--r--   0 macpc      (501) staff       (20)      708 2024-05-03 23:49:12.000000 desgld-0.1.4/setup.py
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 23:52:13.317940 desgld-0.1.4/src/
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 23:52:13.319769 desgld-0.1.4/src/desgld/
--rw-r--r--   0 macpc      (501) staff       (20)      273 2024-04-29 20:32:35.000000 desgld-0.1.4/src/desgld/__init__.py
--rw-r--r--   0 macpc      (501) staff       (20)    11597 2024-04-29 21:40:38.000000 desgld-0.1.4/src/desgld/desgld_alg.py
--rw-r--r--   0 macpc      (501) staff       (20)     5454 2024-04-29 20:32:35.000000 desgld-0.1.4/src/desgld/evaluation.py
--rw-r--r--   0 macpc      (501) staff       (20)     8171 2024-05-03 23:50:01.000000 desgld-0.1.4/src/desgld/network.py
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 23:52:13.321160 desgld-0.1.4/src/desgld.egg-info/
--rw-r--r--   0 macpc      (501) staff       (20)      773 2024-05-03 23:52:13.000000 desgld-0.1.4/src/desgld.egg-info/PKG-INFO
--rw-r--r--   0 macpc      (501) staff       (20)      305 2024-05-03 23:52:13.000000 desgld-0.1.4/src/desgld.egg-info/SOURCES.txt
--rw-r--r--   0 macpc      (501) staff       (20)        1 2024-05-03 23:52:13.000000 desgld-0.1.4/src/desgld.egg-info/dependency_links.txt
--rw-r--r--   0 macpc      (501) staff       (20)       78 2024-05-03 23:52:13.000000 desgld-0.1.4/src/desgld.egg-info/requires.txt
--rw-r--r--   0 macpc      (501) staff       (20)        7 2024-05-03 23:52:13.000000 desgld-0.1.4/src/desgld.egg-info/top_level.txt
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-29 19:13:59.424188 desgld-0.1.6/
+-rw-r--r--   0 macpc      (501) staff       (20)     1079 2024-04-29 20:32:35.000000 desgld-0.1.6/LICENSE
+-rw-r--r--   0 macpc      (501) staff       (20)      772 2024-05-29 19:13:59.423737 desgld-0.1.6/PKG-INFO
+-rw-r--r--   0 macpc      (501) staff       (20)      228 2024-04-29 22:08:43.000000 desgld-0.1.6/README.md
+-rw-r--r--   0 macpc      (501) staff       (20)       79 2024-04-29 20:32:35.000000 desgld-0.1.6/pyproject.toml
+-rw-r--r--   0 macpc      (501) staff       (20)       38 2024-05-29 19:13:59.424278 desgld-0.1.6/setup.cfg
+-rw-r--r--   0 macpc      (501) staff       (20)      723 2024-05-29 19:12:02.000000 desgld-0.1.6/setup.py
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-29 19:13:59.418561 desgld-0.1.6/src/
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-29 19:13:59.421115 desgld-0.1.6/src/desgld/
+-rw-r--r--   0 macpc      (501) staff       (20)      273 2024-04-29 20:32:35.000000 desgld-0.1.6/src/desgld/__init__.py
+-rw-r--r--   0 macpc      (501) staff       (20)    11597 2024-05-29 19:09:43.000000 desgld-0.1.6/src/desgld/desgld_alg.py
+-rw-r--r--   0 macpc      (501) staff       (20)     5454 2024-05-29 19:10:07.000000 desgld-0.1.6/src/desgld/evaluation.py
+-rw-r--r--   0 macpc      (501) staff       (20)     8171 2024-05-29 19:10:29.000000 desgld-0.1.6/src/desgld/network.py
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-29 19:13:59.422926 desgld-0.1.6/src/desgld.egg-info/
+-rw-r--r--   0 macpc      (501) staff       (20)      772 2024-05-29 19:13:59.000000 desgld-0.1.6/src/desgld.egg-info/PKG-INFO
+-rw-r--r--   0 macpc      (501) staff       (20)      305 2024-05-29 19:13:59.000000 desgld-0.1.6/src/desgld.egg-info/SOURCES.txt
+-rw-r--r--   0 macpc      (501) staff       (20)        1 2024-05-29 19:13:59.000000 desgld-0.1.6/src/desgld.egg-info/dependency_links.txt
+-rw-r--r--   0 macpc      (501) staff       (20)       78 2024-05-29 19:13:59.000000 desgld-0.1.6/src/desgld.egg-info/requires.txt
+-rw-r--r--   0 macpc      (501) staff       (20)        7 2024-05-29 19:13:59.000000 desgld-0.1.6/src/desgld.egg-info/top_level.txt
```

### Comparing `desgld-0.1.4/LICENSE` & `desgld-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `desgld-0.1.4/PKG-INFO` & `desgld-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: desgld
-Version: 0.1.4
-Summary: Package for decentralized stochastic gradient descent
+Version: 0.1.6
+Summary: Decentralized stochastic gradient Langevin diffusion
 Home-page: https://github.com/mrislambd/desgld_package.git
 Author: Rafiq Islam
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
```

### Comparing `desgld-0.1.4/setup.py` & `desgld-0.1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,25 +4,28 @@
     "numpy",
     "scipy",
     "scikit-learn",
     "matplotlib",
     "tqdm",
 ]
 
+
 requirements_dev = ["black", "isort", "flake8", "pre-commit"]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="desgld",
-    version="0.1.4",
-    description="Package for decentralized stochastic gradient descent",
+    version="0.1.6",
+    description="Decentralized stochastic gradient Langevin diffusion",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrislambd/desgld_package.git",
     author="Rafiq Islam",
     packages=["desgld"],
     package_dir={"": "src"},
     install_requires=requirements,
-    extras_require={"dev": requirements_dev},
+    extras_require={
+        "dev": requirements_dev,
+    },
 )
```

### Comparing `desgld-0.1.4/src/desgld/desgld_alg.py` & `desgld-0.1.6/src/desgld/desgld_alg.py`

 * *Files identical despite different names*

### Comparing `desgld-0.1.4/src/desgld/evaluation.py` & `desgld-0.1.6/src/desgld/evaluation.py`

 * *Files identical despite different names*

### Comparing `desgld-0.1.4/src/desgld/network.py` & `desgld-0.1.6/src/desgld/network.py`

 * *Files identical despite different names*

### Comparing `desgld-0.1.4/src/desgld.egg-info/PKG-INFO` & `desgld-0.1.6/src/desgld.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: desgld
-Version: 0.1.4
-Summary: Package for decentralized stochastic gradient descent
+Version: 0.1.6
+Summary: Decentralized stochastic gradient Langevin diffusion
 Home-page: https://github.com/mrislambd/desgld_package.git
 Author: Rafiq Islam
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
```

