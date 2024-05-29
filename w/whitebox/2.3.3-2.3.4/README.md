# Comparing `tmp/whitebox-2.3.3.tar.gz` & `tmp/whitebox-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitebox-2.3.3.tar", last modified: Fri May 24 01:10:31 2024, max compression
+gzip compressed data, was "whitebox-2.3.4.tar", last modified: Wed May 29 13:13:48 2024, max compression
```

## Comparing `whitebox-2.3.3.tar` & `whitebox-2.3.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:10:31.869992 whitebox-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-24 01:10:19.000000 whitebox-2.3.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-24 01:10:19.000000 whitebox-2.3.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 01:10:19.000000 whitebox-2.3.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-24 01:10:19.000000 whitebox-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-24 01:10:19.000000 whitebox-2.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-05-24 01:10:31.869992 whitebox-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-05-24 01:10:19.000000 whitebox-2.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:10:31.865992 whitebox-2.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-24 01:10:19.000000 whitebox-2.3.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 01:10:19.000000 whitebox-2.3.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-05-24 01:10:19.000000 whitebox-2.3.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 01:10:19.000000 whitebox-2.3.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 01:10:19.000000 whitebox-2.3.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-24 01:10:19.000000 whitebox-2.3.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-24 01:10:19.000000 whitebox-2.3.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-24 01:10:19.000000 whitebox-2.3.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 01:10:19.000000 whitebox-2.3.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-24 01:10:19.000000 whitebox-2.3.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-24 01:10:31.869992 whitebox-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-24 01:10:19.000000 whitebox-2.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:10:31.865992 whitebox-2.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-24 01:10:19.000000 whitebox-2.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-24 01:10:19.000000 whitebox-2.3.3/tests/test_whitebox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:10:31.865992 whitebox-2.3.3/whitebox/
--rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-05-24 01:10:19.000000 whitebox-2.3.3/whitebox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-24 01:10:19.000000 whitebox-2.3.3/whitebox/automation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-05-24 01:10:19.000000 whitebox-2.3.3/whitebox/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-05-24 01:10:19.000000 whitebox-2.3.3/whitebox/download_wbt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2605 2024-05-24 01:10:19.000000 whitebox-2.3.3/whitebox/example.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-24 01:10:19.000000 whitebox-2.3.3/whitebox/whitebox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-05-24 01:10:19.000000 whitebox-2.3.3/whitebox/whitebox_example.py
--rw-r--r--   0 runner    (1001) docker     (127)   503856 2024-05-24 01:10:19.000000 whitebox-2.3.3/whitebox/whitebox_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:10:31.869992 whitebox-2.3.3/whitebox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-05-24 01:10:31.000000 whitebox-2.3.3/whitebox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-24 01:10:31.000000 whitebox-2.3.3/whitebox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:10:31.000000 whitebox-2.3.3/whitebox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 01:10:31.000000 whitebox-2.3.3/whitebox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:10:31.000000 whitebox-2.3.3/whitebox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 01:10:31.000000 whitebox-2.3.3/whitebox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 01:10:31.000000 whitebox-2.3.3/whitebox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:13:48.544858 whitebox-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 13:13:40.000000 whitebox-2.3.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-29 13:13:40.000000 whitebox-2.3.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-29 13:13:40.000000 whitebox-2.3.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 13:13:40.000000 whitebox-2.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-29 13:13:40.000000 whitebox-2.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-29 13:13:48.544858 whitebox-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10112 2024-05-29 13:13:40.000000 whitebox-2.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:13:48.540858 whitebox-2.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-29 13:13:40.000000 whitebox-2.3.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 13:13:40.000000 whitebox-2.3.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-05-29 13:13:40.000000 whitebox-2.3.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-29 13:13:40.000000 whitebox-2.3.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 13:13:40.000000 whitebox-2.3.4/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-29 13:13:40.000000 whitebox-2.3.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-29 13:13:40.000000 whitebox-2.3.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-29 13:13:40.000000 whitebox-2.3.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 13:13:40.000000 whitebox-2.3.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-29 13:13:40.000000 whitebox-2.3.4/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-29 13:13:48.544858 whitebox-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-29 13:13:40.000000 whitebox-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:13:48.540858 whitebox-2.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 13:13:40.000000 whitebox-2.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-29 13:13:40.000000 whitebox-2.3.4/tests/test_whitebox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:13:48.544858 whitebox-2.3.4/whitebox/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-05-29 13:13:40.000000 whitebox-2.3.4/whitebox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-29 13:13:40.000000 whitebox-2.3.4/whitebox/automation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-05-29 13:13:40.000000 whitebox-2.3.4/whitebox/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-05-29 13:13:40.000000 whitebox-2.3.4/whitebox/download_wbt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2605 2024-05-29 13:13:40.000000 whitebox-2.3.4/whitebox/example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-29 13:13:40.000000 whitebox-2.3.4/whitebox/whitebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-05-29 13:13:40.000000 whitebox-2.3.4/whitebox/whitebox_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)   504197 2024-05-29 13:13:40.000000 whitebox-2.3.4/whitebox/whitebox_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:13:48.544858 whitebox-2.3.4/whitebox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-29 13:13:48.000000 whitebox-2.3.4/whitebox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 13:13:48.000000 whitebox-2.3.4/whitebox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:13:48.000000 whitebox-2.3.4/whitebox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-29 13:13:48.000000 whitebox-2.3.4/whitebox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:13:48.000000 whitebox-2.3.4/whitebox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 13:13:48.000000 whitebox-2.3.4/whitebox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 13:13:48.000000 whitebox-2.3.4/whitebox.egg-info/top_level.txt
```

### Comparing `whitebox-2.3.3/CONTRIBUTING.rst` & `whitebox-2.3.4/CONTRIBUTING.rst`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Types of Contributions
 ----------------------
 
 Report Bugs
 ~~~~~~~~~~~
 
-Report bugs at https://github.com/opengeos/whitebox/issues.
+Report bugs at https://github.com/opengeos/whitebox-python/issues.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
@@ -41,15 +41,15 @@
 whitebox could always use more documentation, whether as part of the
 official whitebox docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
-The best way to send feedback is to file an issue at https://github.com/opengeos/whitebox/issues.
+The best way to send feedback is to file an issue at https://github.com/opengeos/whitebox-python/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
```

### Comparing `whitebox-2.3.3/LICENSE` & `whitebox-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whitebox-2.3.3/PKG-INFO` & `whitebox-2.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: whitebox
-Version: 2.3.3
+Version: 2.3.4
 Summary: An advanced geospatial data analysis platform 
-Home-page: https://github.com/opengeos/whitebox
+Home-page: https://github.com/opengeos/whitebox-python
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: whitebox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -244,15 +244,15 @@
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-.. _example.py: https://github.com/opengeos/whitebox/blob/master/whitebox/example.py
+.. _example.py: https://github.com/opengeos/whitebox-python/blob/master/whitebox/example.py
 .. _WhiteboxTools: https://github.com/jblindsay/whitebox-tools
 .. _webpage: https://jblindsay.github.io/ghrg/index.html
 .. _jblindsay: https://github.com/jblindsay
 .. _`Geomorphometry and Hydrogeomatics Research Group`: https://jblindsay.github.io/ghrg/index.html
 .. _`conda user guide`: https://conda.io/docs/user-guide/install/index.html
 .. _`managing Python environment`: https://conda.io/docs/user-guide/tasks/manage-environments.html
 .. _`WhiteboxTools Usage`: https://github.com/jblindsay/whitebox-tools#3-usage
```

### Comparing `whitebox-2.3.3/README.rst` & `whitebox-2.3.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-.. _example.py: https://github.com/opengeos/whitebox/blob/master/whitebox/example.py
+.. _example.py: https://github.com/opengeos/whitebox-python/blob/master/whitebox/example.py
 .. _WhiteboxTools: https://github.com/jblindsay/whitebox-tools
 .. _webpage: https://jblindsay.github.io/ghrg/index.html
 .. _jblindsay: https://github.com/jblindsay
 .. _`Geomorphometry and Hydrogeomatics Research Group`: https://jblindsay.github.io/ghrg/index.html
 .. _`conda user guide`: https://conda.io/docs/user-guide/install/index.html
 .. _`managing Python environment`: https://conda.io/docs/user-guide/tasks/manage-environments.html
 .. _`WhiteboxTools Usage`: https://github.com/jblindsay/whitebox-tools#3-usage
```

### Comparing `whitebox-2.3.3/docs/Makefile` & `whitebox-2.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `whitebox-2.3.3/docs/conf.py` & `whitebox-2.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `whitebox-2.3.3/docs/installation.rst` & `whitebox-2.3.4/docs/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 
     $ git clone git://github.com/opengeos/whitebox
 
 Or download the `tarball`_:
 
 .. code-block:: console
 
-    $ curl  -OL https://github.com/opengeos/whitebox/tarball/master
+    $ curl  -OL https://github.com/opengeos/whitebox-python/tarball/master
 
 Once you have a copy of the source, you can install it with:
 
 .. code-block:: console
 
     $ python setup.py install
 
 
 .. _Github repo: https://github.com/opengeos/whitebox
-.. _tarball: https://github.com/opengeos/whitebox/tarball/master
+.. _tarball: https://github.com/opengeos/whitebox-python/tarball/master
```

### Comparing `whitebox-2.3.3/docs/make.bat` & `whitebox-2.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `whitebox-2.3.3/docs/usage.rst` & `whitebox-2.3.4/docs/usage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     wbt.verbose = False
     wbt.feature_preserving_denoise("DEM.tif", "smoothed.tif", filter=9)
     wbt.breach_depressions("smoothed.tif", "breached.tif")
     wbt.d_inf_flow_accumulation("breached.tif", "flow_accum.tif")
 
 Check the example.py_ for more details.
 
-.. _example.py: https://github.com/opengeos/whitebox/blob/master/whitebox/example.py
+.. _example.py: https://github.com/opengeos/whitebox-python/blob/master/whitebox/example.py
```

### Comparing `whitebox-2.3.3/setup.py` & `whitebox-2.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-with open('README.rst') as readme_file:
+with open("README.rst") as readme_file:
     readme = readme_file.read()
 
-with open('HISTORY.rst') as history_file:
+with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
 requirements = [
-    'Click>=6.0',
+    "Click>=6.0",
 ]
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
     author="Qiusheng Wu",
-    author_email='giswqs@gmail.com',
+    author_email="giswqs@gmail.com",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
     ],
     description="An advanced geospatial data analysis platform ",
     entry_points={
-        'console_scripts': [
-            'whitebox=whitebox.cli:main',
+        "console_scripts": [
+            "whitebox=whitebox.cli:main",
         ],
     },
     install_requires=requirements,
     license="MIT license",
-    long_description=readme + '\n\n' + history,
+    long_description=readme + "\n\n" + history,
     include_package_data=True,
-    keywords='whitebox',
-    name='whitebox',
-    packages=find_packages(include=['whitebox']),
+    keywords="whitebox",
+    name="whitebox",
+    packages=find_packages(include=["whitebox"]),
     setup_requires=setup_requirements,
-    test_suite='tests',
+    test_suite="tests",
     tests_require=test_requirements,
-    url='https://github.com/opengeos/whitebox',
-    version='2.3.3',
+    url="https://github.com/opengeos/whitebox-python",
+    version="2.3.4",
     zip_safe=False,
 )
```

### Comparing `whitebox-2.3.3/tests/test_whitebox.py` & `whitebox-2.3.4/tests/test_whitebox.py`

 * *Files identical despite different names*

### Comparing `whitebox-2.3.3/whitebox/automation.py` & `whitebox-2.3.4/whitebox/automation.py`

 * *Files identical despite different names*

### Comparing `whitebox-2.3.3/whitebox/download_wbt.py` & `whitebox-2.3.4/whitebox/download_wbt.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,18 +85,20 @@
                 pkg_dir, os.path.basename(url)
             )  # Get WhiteboxTools zip file name
             # Get downloaded zip file extension
             zip_ext = os.path.splitext(zip_name)[1]
             # Download WhiteboxTools
             try:
                 request = urllib.request.urlopen(url, timeout=500)
+                print("Downloading WhiteboxTools binary from {}".format(url))
             except urllib.error.URLError as e:
                 print(e)
                 print("Trying backup link ...")
                 url = backup_links[platform.system()]
+                print("Downloading WhiteboxTools binary from {}".format(url))
                 request = urllib.request.urlopen(url, timeout=500)
 
             with open(zip_name, "wb") as f:
                 f.write(request.read())
 
             if verbose:
                 print("Decompressing {} ...".format(os.path.basename(url)))
@@ -136,47 +138,51 @@
             if os.path.exists(src_dir):
                 shutil.move(src_dir, pkg_dir)
 
             if os.path.exists(new_img_dir):
                 shutil.rmtree(new_img_dir)
             if os.path.exists(new_plugin_dir):
                 shutil.rmtree(new_plugin_dir)
+            if os.path.exists(new_plugin_dir):
+                shutil.rmtree(new_plugin_dir)
 
-            if os.path.exists(new_img_dir):
+            if os.path.exists(init_img_dir):
                 shutil.copytree(init_img_dir, new_img_dir)
 
-            if os.path.exists(new_plugin_dir):
+            if os.path.exists(init_plugin_dir):
                 shutil.copytree(init_plugin_dir, new_plugin_dir)
 
             if os.path.exists(zip_dir):
                 shutil.rmtree(zip_dir)
             exe_ext = ""  # file extension for MacOS/Linux
             if platform.system() == "Windows":
                 exe_ext = ".exe"
             exe_name = "whitebox_tools{}".format(exe_ext)
             exe_path = os.path.join(exe_dir, exe_name)
-            # runner_name = "whitebox_runner{}".format(exe_ext)
-            # runner_path = os.path.join(exe_dir, runner_name)
+            runner_name = "whitebox_runner{}".format(exe_ext)
+            runner_path = os.path.join(exe_dir, runner_name)
 
             # grant executable permission
             if platform.system() != "Windows":
                 os.system("chmod 755 " + exe_path)
-                # os.system("chmod 755 " + runner_path)
+                if os.path.exists(runner_path):
+                    os.system("chmod 755 " + runner_path)
             plugins = list(
                 set(glob.glob(os.path.join(new_plugin_dir, "*")))
                 - set(glob.glob(os.path.join(new_plugin_dir, "*.json")))
             )
             if platform.system() != "Windows":
                 for plugin in plugins:
                     os.system("chmod 755 " + plugin)
 
             exe_path_new = os.path.join(pkg_dir, exe_name)
             shutil.copy(exe_path, exe_path_new)
-            # runner_path_new = os.path.join(pkg_dir, runner_name)
-            # shutil.copy(runner_path, runner_path_new)
+            runner_path_new = os.path.join(pkg_dir, runner_name)
+            if os.path.exists(runner_path):
+                shutil.copy(runner_path, runner_path_new)
 
             try:
                 os.remove(zip_name)
             except:
                 pass
 
             # # The official WhiteboxTools Linux binary from whiteboxgeo.com requires GLIBC 2.29,
```

### Comparing `whitebox-2.3.3/whitebox/example.py` & `whitebox-2.3.4/whitebox/example.py`

 * *Files identical despite different names*

### Comparing `whitebox-2.3.3/whitebox/whitebox_example.py` & `whitebox-2.3.4/whitebox/whitebox_example.py`

 * *Files identical despite different names*

### Comparing `whitebox-2.3.3/whitebox/whitebox_tools.py` & `whitebox-2.3.4/whitebox/whitebox_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,18 +114,20 @@
                 pkg_dir, os.path.basename(url)
             )  # Get WhiteboxTools zip file name
             # Get downloaded zip file extension
             zip_ext = os.path.splitext(zip_name)[1]
             # Download WhiteboxTools
             try:
                 request = urllib.request.urlopen(url, timeout=500)
+                print("Downloading WhiteboxTools binary from {}".format(url))
             except urllib.error.URLError as e:
                 print(e)
                 print("Trying backup link ...")
                 url = backup_links[platform.system()]
+                print("Downloading WhiteboxTools binary from {}".format(url))
                 request = urllib.request.urlopen(url, timeout=500)
 
             with open(zip_name, "wb") as f:
                 f.write(request.read())
 
             if verbose:
                 print("Decompressing {} ...".format(os.path.basename(url)))
@@ -165,47 +167,51 @@
             if os.path.exists(src_dir):
                 shutil.move(src_dir, pkg_dir)
 
             if os.path.exists(new_img_dir):
                 shutil.rmtree(new_img_dir)
             if os.path.exists(new_plugin_dir):
                 shutil.rmtree(new_plugin_dir)
+            if os.path.exists(new_plugin_dir):
+                shutil.rmtree(new_plugin_dir)
 
-            if os.path.exists(new_img_dir):
+            if os.path.exists(init_img_dir):
                 shutil.copytree(init_img_dir, new_img_dir)
 
-            if os.path.exists(new_plugin_dir):
+            if os.path.exists(init_plugin_dir):
                 shutil.copytree(init_plugin_dir, new_plugin_dir)
 
             if os.path.exists(zip_dir):
                 shutil.rmtree(zip_dir)
             exe_ext = ""  # file extension for MacOS/Linux
             if platform.system() == "Windows":
                 exe_ext = ".exe"
             exe_name = "whitebox_tools{}".format(exe_ext)
             exe_path = os.path.join(exe_dir, exe_name)
-            # runner_name = "whitebox_runner{}".format(exe_ext)
-            # runner_path = os.path.join(exe_dir, runner_name)
+            runner_name = "whitebox_runner{}".format(exe_ext)
+            runner_path = os.path.join(exe_dir, runner_name)
 
             # grant executable permission
             if platform.system() != "Windows":
                 os.system("chmod 755 " + exe_path)
-                # os.system("chmod 755 " + runner_path)
+                if os.path.exists(runner_path):
+                    os.system("chmod 755 " + runner_path)
             plugins = list(
                 set(glob.glob(os.path.join(new_plugin_dir, "*")))
                 - set(glob.glob(os.path.join(new_plugin_dir, "*.json")))
             )
             if platform.system() != "Windows":
                 for plugin in plugins:
                     os.system("chmod 755 " + plugin)
 
             exe_path_new = os.path.join(pkg_dir, exe_name)
             shutil.copy(exe_path, exe_path_new)
-            # runner_path_new = os.path.join(pkg_dir, runner_name)
-            # shutil.copy(runner_path, runner_path_new)
+            runner_path_new = os.path.join(pkg_dir, runner_name)
+            if os.path.exists(runner_path):
+                shutil.copy(runner_path, runner_path_new)
 
             try:
                 os.remove(zip_name)
             except:
                 pass
 
             # # The official WhiteboxTools Linux binary from whiteboxgeo.com requires GLIBC 2.29,
```

### Comparing `whitebox-2.3.3/whitebox.egg-info/PKG-INFO` & `whitebox-2.3.4/whitebox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: whitebox
-Version: 2.3.3
+Version: 2.3.4
 Summary: An advanced geospatial data analysis platform 
-Home-page: https://github.com/opengeos/whitebox
+Home-page: https://github.com/opengeos/whitebox-python
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: whitebox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -244,15 +244,15 @@
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-.. _example.py: https://github.com/opengeos/whitebox/blob/master/whitebox/example.py
+.. _example.py: https://github.com/opengeos/whitebox-python/blob/master/whitebox/example.py
 .. _WhiteboxTools: https://github.com/jblindsay/whitebox-tools
 .. _webpage: https://jblindsay.github.io/ghrg/index.html
 .. _jblindsay: https://github.com/jblindsay
 .. _`Geomorphometry and Hydrogeomatics Research Group`: https://jblindsay.github.io/ghrg/index.html
 .. _`conda user guide`: https://conda.io/docs/user-guide/install/index.html
 .. _`managing Python environment`: https://conda.io/docs/user-guide/tasks/manage-environments.html
 .. _`WhiteboxTools Usage`: https://github.com/jblindsay/whitebox-tools#3-usage
```

### Comparing `whitebox-2.3.3/whitebox.egg-info/SOURCES.txt` & `whitebox-2.3.4/whitebox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

