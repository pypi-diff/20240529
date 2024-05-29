# Comparing `tmp/gemmi_program-0.6.5.tar.gz` & `tmp/gemmi_program-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemmi_program-0.6.5.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "gemmi_program-0.6.6.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `gemmi_program-0.6.5.tar` & `gemmi_program-0.6.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 gemmi_program-0.6.5/.github/workflows/wheels.yml
--rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 gemmi_program-0.6.5/.gitignore
--rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 gemmi_program-0.6.5/CMakeLists.txt
--rw-r--r--   0        0        0     1038 2022-11-09 12:37:21.000000 gemmi_program-0.6.5/README.md
--rw-r--r--   0        0        0     1076 2022-11-09 12:37:21.000000 gemmi_program-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     1588 2022-11-09 12:37:21.000000 gemmi_program-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 gemmi_program-0.6.6/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 gemmi_program-0.6.6/.gitignore
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 gemmi_program-0.6.6/CMakeLists.txt
+-rw-r--r--   0        0        0     1050 2022-11-09 12:37:21.000000 gemmi_program-0.6.6/README.md
+-rw-r--r--   0        0        0     1076 2022-11-09 12:37:21.000000 gemmi_program-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     1600 2022-11-09 12:37:21.000000 gemmi_program-0.6.6/PKG-INFO
```

### Comparing `gemmi_program-0.6.5/.github/workflows/wheels.yml` & `gemmi_program-0.6.6/.github/workflows/wheels.yml`

 * *Files 15% similar despite different names*

```diff
@@ -12,24 +12,24 @@
     strategy:
       matrix:
         include:
           - os: ubuntu-22.04
             arch: "x86_64"
           - os: windows-2022
             arch: "AMD64"
-          - os: macos-13
+          - os: macos-12
             arch: "x86_64"
           - os: macos-14
             arch: "arm64"
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Build wheels
-      uses: pypa/cibuildwheel@v2.16.5
+      uses: pypa/cibuildwheel@v2.18.1
       env:
         CIBW_ARCHS: "${{ matrix.arch }}"
 
     - run: ls -lh wheelhouse
       shell: bash
 
     - uses: actions/upload-artifact@v4
```

### Comparing `gemmi_program-0.6.5/CMakeLists.txt` & `gemmi_program-0.6.6/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # avoid building python module
 unset(Python_EXECUTABLE CACHE)
 
 include(FetchContent)
 FetchContent_Declare(
   gemmi
   GIT_REPOSITORY https://github.com/project-gemmi/gemmi.git
-  GIT_TAG        v0.6.5
+  GIT_TAG        v0.6.6
   #GIT_TAG        master
   GIT_SHALLOW    TRUE
 )
 
 # We don't want to install all gemmi files.
 # https://stackoverflow.com/questions/65527126/disable-install-for-fetchcontent
 FetchContent_GetProperties(gemmi)
```

### Comparing `gemmi_program-0.6.5/README.md` & `gemmi_program-0.6.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 
 It is, in PyPI, distributed separately from the Python extension module
 [gemmi](https://pypi.org/project/gemmi/),
 because, unlike the module, it does not depend on Python version.
 
 ### notes for myself -- how to make wheels after gemmi release
 
-* update `GIT_TAG` in CMakeLists.txt and `version` in pyproject.toml
-* (optionally) update version of cibuildwheel in .github/workflows/wheels.yml
-  and scikit-build-core in pyproject.toml
+* update:
+  * `GIT_TAG` in CMakeLists.txt
+  * `version` in pyproject.toml
+  * scikit-build-core version in pyproject.toml (optional)
+  * cibuildwheel version in .github/workflows/wheels.yml (optional)
 * test locally with `pip wheel .`
 * make source distribution of this repo: `python -m build --sdist`
 * git push changes to build wheels in [GitHub Actions][1]
 * download the wheels, check them, upload sdist and wheels to PyPI:
 
       twine upload dist/gemmi_program-$VERSION.tar.gz
       twine upload wheels/gemmi_program-$VERSION-*.whl
```

### Comparing `gemmi_program-0.6.5/pyproject.toml` & `gemmi_program-0.6.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["scikit-build-core~=0.8.0"]
+requires = ["scikit-build-core~=0.9.0"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "gemmi-program"
-version = "0.6.5"
+version = "0.6.6"
 requires-python = ">=3.8"
 description="gemmi (program executable only)"
 readme = "README.md"
 authors = [{name="Marcin Wojdyr", email="wojdyr@gmail.com"}]
 urls.repository = "https://github.com/project-gemmi/gemmi_program_wheel"
 license = {text = "MPL-2.0"}  # or, at your option, LGPL-3.0
 classifiers = [
```

### Comparing `gemmi_program-0.6.5/PKG-INFO` & `gemmi_program-0.6.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemmi-program
-Version: 0.6.5
+Version: 0.6.6
 Summary: gemmi (program executable only)
 Author-Email: Marcin Wojdyr <wojdyr@gmail.com>
 License: MPL-2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -20,17 +20,19 @@
 
 It is, in PyPI, distributed separately from the Python extension module
 [gemmi](https://pypi.org/project/gemmi/),
 because, unlike the module, it does not depend on Python version.
 
 ### notes for myself -- how to make wheels after gemmi release
 
-* update `GIT_TAG` in CMakeLists.txt and `version` in pyproject.toml
-* (optionally) update version of cibuildwheel in .github/workflows/wheels.yml
-  and scikit-build-core in pyproject.toml
+* update:
+  * `GIT_TAG` in CMakeLists.txt
+  * `version` in pyproject.toml
+  * scikit-build-core version in pyproject.toml (optional)
+  * cibuildwheel version in .github/workflows/wheels.yml (optional)
 * test locally with `pip wheel .`
 * make source distribution of this repo: `python -m build --sdist`
 * git push changes to build wheels in [GitHub Actions][1]
 * download the wheels, check them, upload sdist and wheels to PyPI:
 
       twine upload dist/gemmi_program-$VERSION.tar.gz
       twine upload wheels/gemmi_program-$VERSION-*.whl
```

