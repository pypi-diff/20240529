# Comparing `tmp/askvideos-0.1.0.tar.gz` & `tmp/askvideos-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/askvideos-0.1.0.tar", last modified: Sat Mar  2 22:54:37 2024, max compression
+gzip compressed data, was "askvideos-0.1.1.tar", last modified: Wed May 29 01:07:32 2024, max compression
```

## Comparing `askvideos-0.1.0.tar` & `askvideos-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxr-xr-x   0 bhav       (501) staff       (20)        0 2024-03-02 22:54:37.735979 askvideos-0.1.0/
--rw-r--r--   0 bhav       (501) staff       (20)      643 2024-03-02 22:54:37.735753 askvideos-0.1.0/PKG-INFO
--rw-r--r--   0 bhav       (501) staff       (20)        0 2024-03-02 22:38:36.000000 askvideos-0.1.0/README.md
-drwxr-xr-x   0 bhav       (501) staff       (20)        0 2024-03-02 22:54:37.735549 askvideos-0.1.0/askvideos.egg-info/
--rw-r--r--   0 bhav       (501) staff       (20)      643 2024-03-02 22:54:37.000000 askvideos-0.1.0/askvideos.egg-info/PKG-INFO
--rw-r--r--   0 bhav       (501) staff       (20)      150 2024-03-02 22:54:37.000000 askvideos-0.1.0/askvideos.egg-info/SOURCES.txt
--rw-r--r--   0 bhav       (501) staff       (20)        1 2024-03-02 22:54:37.000000 askvideos-0.1.0/askvideos.egg-info/dependency_links.txt
--rw-r--r--   0 bhav       (501) staff       (20)        1 2024-03-02 22:54:37.000000 askvideos-0.1.0/askvideos.egg-info/top_level.txt
--rw-r--r--   0 bhav       (501) staff       (20)       38 2024-03-02 22:54:37.736022 askvideos-0.1.0/setup.cfg
--rw-r--r--   0 bhav       (501) staff       (20)     1810 2024-03-02 22:46:40.000000 askvideos-0.1.0/setup.py
+drwxrwxr-x   0 bhavashok  (1000) bhavashok  (1000)        0 2024-05-29 01:07:32.051195 askvideos-0.1.1/
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)     1050 2024-05-29 01:07:32.051195 askvideos-0.1.1/PKG-INFO
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)      790 2024-05-29 00:55:03.000000 askvideos-0.1.1/README.md
+drwxrwxr-x   0 bhavashok  (1000) bhavashok  (1000)        0 2024-05-29 01:07:32.051195 askvideos-0.1.1/askvideos.egg-info/
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)     1050 2024-05-29 01:07:31.000000 askvideos-0.1.1/askvideos.egg-info/PKG-INFO
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)      192 2024-05-29 01:07:32.000000 askvideos-0.1.1/askvideos.egg-info/SOURCES.txt
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)        1 2024-05-29 01:07:31.000000 askvideos-0.1.1/askvideos.egg-info/dependency_links.txt
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)        9 2024-05-29 01:07:31.000000 askvideos-0.1.1/askvideos.egg-info/requires.txt
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)        7 2024-05-29 01:07:31.000000 askvideos-0.1.1/askvideos.egg-info/top_level.txt
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)    11411 2024-05-29 00:43:29.000000 askvideos-0.1.1/client.py
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)       38 2024-05-29 01:07:32.051195 askvideos-0.1.1/setup.cfg
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)     1298 2024-05-29 01:05:46.000000 askvideos-0.1.1/setup.py
```

### Comparing `askvideos-0.1.0/setup.py` & `askvideos-0.1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='askvideos',  # Replace 'your_package_name' with the name of your package
-    version='0.1.0',  # Version number for your package
+    version='0.1.1',  # Version number for your package
     author='AskVideos',  # Your name or your organization's name
     author_email='askutubeai@gmail.com',  # Your email or your organization's contact email
     description='AskVideos python library',  # A brief description of your package
     long_description=open('README.md').read(),  # A long description from your README.md
     long_description_content_type='text/markdown',  # Specifies that the long description is in Markdown
-    url='https://github.com/AskYoutubeAI/AskVideos',  # URL to your package's repository
+    url='https://github.com/AskYoutubeAI/askvideos-py',  # URL to your package's repository
     #packages=find_packages(exclude=('tests', 'docs')),  # Automatically find all packages in your project
     install_requires=[
         # List your project's dependencies here.
         # They will be installed by pip when your package is installed.
         # Example: 'requests>=2.19.1'
-    ],
-    classifiers=[
-        # Trove classifiers
-        # Full list at https://pypi.org/classifiers/
-        'Development Status :: 3 - Alpha',  # Change as appropriate
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',  # Change as appropriate
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
+        "requests",
     ],
     python_requires='>=3.6',  # Minimum version requirement of Python
     #entry_points={
     #    'console_scripts': [
     #        # Entry points for console scripts
     #        # Example: 'your_script_name = your_package.module:function'
     #    ],
```

