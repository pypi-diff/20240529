# Comparing `tmp/gpt-repository-loader-0.9.0.tar.gz` & `tmp/gpt-repository-loader-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-repository-loader-0.9.0.tar", last modified: Thu May 16 17:53:09 2024, max compression
+gzip compressed data, was "gpt-repository-loader-0.9.1.tar", last modified: Wed May 29 03:35:46 2024, max compression
```

## Comparing `gpt-repository-loader-0.9.0.tar` & `gpt-repository-loader-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-16 17:53:09.172155 gpt-repository-loader-0.9.0/
--rw-r--r--   0 harshwork   (502) staff       (20)     1066 2023-03-17 08:40:06.000000 gpt-repository-loader-0.9.0/LICENSE
--rw-r--r--   0 harshwork   (502) staff       (20)     3313 2024-05-16 17:53:09.171867 gpt-repository-loader-0.9.0/PKG-INFO
--rw-r--r--   0 harshwork   (502) staff       (20)     2517 2023-03-23 06:58:13.000000 gpt-repository-loader-0.9.0/README.md
-drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-16 17:53:09.170168 gpt-repository-loader-0.9.0/gpt_repository_loader/
--rw-r--r--   0 harshwork   (502) staff       (20)      100 2023-03-21 06:32:35.000000 gpt-repository-loader-0.9.0/gpt_repository_loader/__init__.py
--rwxr-xr-x   0 harshwork   (502) staff       (20)     4337 2024-05-16 17:46:08.000000 gpt-repository-loader-0.9.0/gpt_repository_loader/gpt_repository_loader.py
-drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-16 17:53:09.171566 gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/
--rw-r--r--   0 harshwork   (502) staff       (20)     3313 2024-05-16 17:53:09.000000 gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/PKG-INFO
--rw-r--r--   0 harshwork   (502) staff       (20)      379 2024-05-16 17:53:09.000000 gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/SOURCES.txt
--rw-r--r--   0 harshwork   (502) staff       (20)        1 2024-05-16 17:53:09.000000 gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/dependency_links.txt
--rw-r--r--   0 harshwork   (502) staff       (20)       69 2024-05-16 17:53:09.000000 gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/entry_points.txt
--rw-r--r--   0 harshwork   (502) staff       (20)       10 2024-05-16 17:53:09.000000 gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/requires.txt
--rw-r--r--   0 harshwork   (502) staff       (20)       22 2024-05-16 17:53:09.000000 gpt-repository-loader-0.9.0/gpt_repository_loader.egg-info/top_level.txt
--rw-r--r--   0 harshwork   (502) staff       (20)       38 2024-05-16 17:53:09.172209 gpt-repository-loader-0.9.0/setup.cfg
--rwxr-xr-x   0 harshwork   (502) staff       (20)     1176 2024-05-16 17:49:31.000000 gpt-repository-loader-0.9.0/setup.py
+drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-29 03:35:46.223846 gpt-repository-loader-0.9.1/
+-rw-r--r--   0 harshwork   (502) staff       (20)     1066 2023-03-17 08:40:06.000000 gpt-repository-loader-0.9.1/LICENSE
+-rw-r--r--   0 harshwork   (502) staff       (20)     1368 2024-05-29 03:35:46.223586 gpt-repository-loader-0.9.1/PKG-INFO
+-rw-r--r--   0 harshwork   (502) staff       (20)      572 2024-05-21 05:51:26.000000 gpt-repository-loader-0.9.1/README.md
+drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-29 03:35:46.222077 gpt-repository-loader-0.9.1/gpt_repository_loader/
+-rw-r--r--   0 harshwork   (502) staff       (20)      100 2023-03-21 06:32:35.000000 gpt-repository-loader-0.9.1/gpt_repository_loader/__init__.py
+-rwxr-xr-x   0 harshwork   (502) staff       (20)     4358 2024-05-21 05:52:23.000000 gpt-repository-loader-0.9.1/gpt_repository_loader/gpt_repository_loader.py
+drwxr-xr-x   0 harshwork   (502) staff       (20)        0 2024-05-29 03:35:46.223325 gpt-repository-loader-0.9.1/gpt_repository_loader.egg-info/
+-rw-r--r--   0 harshwork   (502) staff       (20)     1368 2024-05-29 03:35:46.000000 gpt-repository-loader-0.9.1/gpt_repository_loader.egg-info/PKG-INFO
+-rw-r--r--   0 harshwork   (502) staff       (20)      379 2024-05-29 03:35:46.000000 gpt-repository-loader-0.9.1/gpt_repository_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)        1 2024-05-29 03:35:46.000000 gpt-repository-loader-0.9.1/gpt_repository_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)       69 2024-05-29 03:35:46.000000 gpt-repository-loader-0.9.1/gpt_repository_loader.egg-info/entry_points.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)       10 2024-05-29 03:35:46.000000 gpt-repository-loader-0.9.1/gpt_repository_loader.egg-info/requires.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)       22 2024-05-29 03:35:46.000000 gpt-repository-loader-0.9.1/gpt_repository_loader.egg-info/top_level.txt
+-rw-r--r--   0 harshwork   (502) staff       (20)       38 2024-05-29 03:35:46.223901 gpt-repository-loader-0.9.1/setup.cfg
+-rwxr-xr-x   0 harshwork   (502) staff       (20)     1176 2024-05-29 03:35:43.000000 gpt-repository-loader-0.9.1/setup.py
```

### Comparing `gpt-repository-loader-0.9.0/LICENSE` & `gpt-repository-loader-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-repository-loader-0.9.0/gpt_repository_loader/gpt_repository_loader.py` & `gpt-repository-loader-0.9.1/gpt_repository_loader/gpt_repository_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         with open(ignore_file_path, 'r') as ignore_file:
             for line in ignore_file:
                 line = line.strip()
                 if not line or line.startswith("#"):
                     continue
                 ignore_list.append(line)
 
-    default_ignore_list = ['dist', 'dist/','dist/*','sdist', 'sdist/','sdist/*' '.git/', '/.git/', '.git', '.git/*', '.gptignore', '.gitignore', 'node_modules', 'node_modules/*', '__pycache__', '__pycache__/*']
+    default_ignore_list = ['dist', 'dist/','dist/*','sdist', 'sdist/','sdist/*' '.git/', '/.git/', '.git', '.git/*', '.gptignore', '.gitignore', 'node_modules', 'node_modules/*', '__pycache__', '__pycache__/*', 'package-lock.json']
     ignore_list += default_ignore_list
 
     return ignore_list
 
 def process_repository(repo_path, ignore_list, output_stream):
     git_files = subprocess.check_output(["git", "ls-files"], cwd=repo_path, universal_newlines=True).splitlines()
```

### Comparing `gpt-repository-loader-0.9.0/setup.py` & `gpt-repository-loader-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gpt-repository-loader",
-    version="0.9.0",
+    version="0.9.1",
     author="Felvin",
     author_email="team@felvin.com",
     description="A utility to convert a Git repository into a text representation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/felvin-search/gpt-repository-loader",
     packages=find_packages(),
```

