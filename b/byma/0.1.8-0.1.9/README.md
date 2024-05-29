# Comparing `tmp/byma-0.1.8.tar.gz` & `tmp/byma-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byma-0.1.8.tar", last modified: Tue May 28 05:53:29 2024, max compression
+gzip compressed data, was "byma-0.1.9.tar", last modified: Tue May 28 06:31:47 2024, max compression
```

## Comparing `byma-0.1.8.tar` & `byma-0.1.9.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.552209 byma-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-05-28 05:53:17.000000 byma-0.1.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-05-28 05:53:17.000000 byma-0.1.8/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      721 2024-05-28 05:53:17.000000 byma-0.1.8/CHANGELOG.txt
--rwxrwxrwx   0 root         (0) root         (0)     1836 2024-05-28 05:53:17.000000 byma-0.1.8/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-28 05:53:17.000000 byma-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3304 2024-05-28 05:53:29.552209 byma-0.1.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2409 2024-05-28 05:53:17.000000 byma-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.538209 byma-0.1.8/byma/
--rw-rw-rw-   0 root         (0) root         (0)     1384 2024-05-28 05:53:17.000000 byma-0.1.8/byma/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-28 05:53:29.000000 byma-0.1.8/byma/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.540209 byma-0.1.8/byma/interface/
--rw-rw-rw-   0 root         (0) root         (0)     2612 2024-05-28 05:53:17.000000 byma-0.1.8/byma/interface/BaseInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     3589 2024-05-28 05:53:17.000000 byma-0.1.8/byma/interface/NonlinearHeat.py
--rw-rw-rw-   0 root         (0) root         (0)    11496 2024-05-28 05:53:17.000000 byma-0.1.8/byma/interface/Time.py
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-05-28 05:53:17.000000 byma-0.1.8/byma/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.542209 byma-0.1.8/byma/iteral/
--rw-rw-rw-   0 root         (0) root         (0)     8900 2024-05-28 05:53:17.000000 byma-0.1.8/byma/iteral/GradientDescent.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2024-05-28 05:53:17.000000 byma-0.1.8/byma/iteral/Iteral.py
--rw-rw-rw-   0 root         (0) root         (0)     6420 2024-05-28 05:53:17.000000 byma-0.1.8/byma/iteral/NesterovMethod.py
--rw-rw-rw-   0 root         (0) root         (0)     5149 2024-05-28 05:53:17.000000 byma-0.1.8/byma/iteral/Newton.py
--rw-rw-rw-   0 root         (0) root         (0)     4832 2024-05-28 05:53:17.000000 byma-0.1.8/byma/iteral/OrthogonalSubspace.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2024-05-28 05:53:17.000000 byma-0.1.8/byma/iteral/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.542209 byma-0.1.8/byma/nuby/
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-28 05:53:17.000000 byma-0.1.8/byma/nuby/Bifurcation.py
--rw-rw-rw-   0 root         (0) root         (0)     7951 2024-05-28 05:53:17.000000 byma-0.1.8/byma/nuby/Continuation.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-05-28 05:53:17.000000 byma-0.1.8/byma/nuby/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-05-28 05:53:17.000000 byma-0.1.8/byma/nuby/_nuby.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.543209 byma-0.1.8/byma/numy/
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-28 05:53:17.000000 byma-0.1.8/byma/numy/Numy.py
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-05-28 05:53:17.000000 byma-0.1.8/byma/numy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-05-28 05:53:17.000000 byma-0.1.8/byma/numy/_numy.py
--rw-rw-rw-   0 root         (0) root         (0)     3576 2024-05-28 05:53:17.000000 byma-0.1.8/byma/numy/integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.544209 byma-0.1.8/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-28 05:53:17.000000 byma-0.1.8/byma/pyplot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6292 2024-05-28 05:53:17.000000 byma-0.1.8/byma/pyplot/plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.552209 byma-0.1.8/byma.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3304 2024-05-28 05:53:29.000000 byma-0.1.8/byma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2143 2024-05-28 05:53:29.000000 byma-0.1.8/byma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 05:53:29.000000 byma-0.1.8/byma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-28 05:53:29.000000 byma-0.1.8/byma.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.544209 byma-0.1.8/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-05-28 05:53:17.000000 byma-0.1.8/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-28 05:53:17.000000 byma-0.1.8/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-28 05:53:17.000000 byma-0.1.8/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.545209 byma-0.1.8/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.545209 byma-0.1.8/docs/source/autoapi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.545209 byma-0.1.8/docs/source/autoapi/OrthogonalSubspace/
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/OrthogonalSubspace/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.545209 byma-0.1.8/docs/source/autoapi/byma/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.546209 byma-0.1.8/docs/source/autoapi/byma/_version/
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/_version/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      849 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.546209 byma-0.1.8/docs/source/autoapi/byma/interface/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.546209 byma-0.1.8/docs/source/autoapi/byma/interface/BaseInterface/
--rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/interface/BaseInterface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.546209 byma-0.1.8/docs/source/autoapi/byma/interface/NonlinearHeat/
--rw-rw-rw-   0 root         (0) root         (0)     2086 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.547209 byma-0.1.8/docs/source/autoapi/byma/interface/Time/
--rw-rw-rw-   0 root         (0) root         (0)     6226 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/interface/Time/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     9459 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/interface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.547209 byma-0.1.8/docs/source/autoapi/byma/iteral/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.547209 byma-0.1.8/docs/source/autoapi/byma/iteral/GradientDescent/
--rw-rw-rw-   0 root         (0) root         (0)     3947 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/iteral/GradientDescent/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.547209 byma-0.1.8/docs/source/autoapi/byma/iteral/Iteral/
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/iteral/Iteral/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.547209 byma-0.1.8/docs/source/autoapi/byma/iteral/NesterovMethod/
--rw-rw-rw-   0 root         (0) root         (0)     3433 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/iteral/NesterovMethod/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.548209 byma-0.1.8/docs/source/autoapi/byma/iteral/Newton/
--rw-rw-rw-   0 root         (0) root         (0)     3365 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/iteral/Newton/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.548209 byma-0.1.8/docs/source/autoapi/byma/iteral/OrthogonalSubspace/
--rw-rw-rw-   0 root         (0) root         (0)     3588 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      509 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/iteral/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.548209 byma-0.1.8/docs/source/autoapi/byma/nuby/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.548209 byma-0.1.8/docs/source/autoapi/byma/nuby/Bifurcation/
--rw-rw-rw-   0 root         (0) root         (0)      278 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.549209 byma-0.1.8/docs/source/autoapi/byma/nuby/Continuation/
--rw-rw-rw-   0 root         (0) root         (0)     7798 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/nuby/Continuation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.549209 byma-0.1.8/docs/source/autoapi/byma/nuby/_nuby/
--rw-rw-rw-   0 root         (0) root         (0)     4840 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/nuby/_nuby/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5104 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/nuby/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.549209 byma-0.1.8/docs/source/autoapi/byma/numy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.549209 byma-0.1.8/docs/source/autoapi/byma/numy/Numy/
--rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/numy/Numy/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.549209 byma-0.1.8/docs/source/autoapi/byma/numy/_numy/
--rw-rw-rw-   0 root         (0) root         (0)     1858 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/numy/_numy/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2108 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/numy/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.550209 byma-0.1.8/docs/source/autoapi/byma/numy/integration/
--rw-rw-rw-   0 root         (0) root         (0)     4818 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/numy/integration/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.550209 byma-0.1.8/docs/source/autoapi/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     3579 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/pyplot/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.550209 byma-0.1.8/docs/source/autoapi/byma/pyplot/plots/
--rw-rw-rw-   0 root         (0) root         (0)     3522 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/byma/pyplot/plots/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/autoapi/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3805 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1926 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.551209 byma-0.1.8/docs/source/user/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/user/Installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/user/index.rst
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/user/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-28 05:53:17.000000 byma-0.1.8/docs/source/user/whatisbyma.rst
--rwxrwxrwx   0 root         (0) root         (0)     1005 2024-05-28 05:53:17.000000 byma-0.1.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-28 05:53:17.000000 byma-0.1.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 05:53:29.552209 byma-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1021 2024-05-28 05:53:17.000000 byma-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:53:29.551209 byma-0.1.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 05:53:17.000000 byma-0.1.8/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.412532 byma-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-05-28 06:31:35.000000 byma-0.1.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-05-28 06:31:35.000000 byma-0.1.9/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      827 2024-05-28 06:31:35.000000 byma-0.1.9/CHANGELOG.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1836 2024-05-28 06:31:35.000000 byma-0.1.9/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-28 06:31:35.000000 byma-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3304 2024-05-28 06:31:47.411532 byma-0.1.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2409 2024-05-28 06:31:35.000000 byma-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.398533 byma-0.1.9/byma/
+-rw-rw-rw-   0 root         (0) root         (0)     1384 2024-05-28 06:31:35.000000 byma-0.1.9/byma/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-28 06:31:47.000000 byma-0.1.9/byma/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.400533 byma-0.1.9/byma/interface/
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2024-05-28 06:31:35.000000 byma-0.1.9/byma/interface/BaseInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2024-05-28 06:31:35.000000 byma-0.1.9/byma/interface/NonlinearHeat.py
+-rw-rw-rw-   0 root         (0) root         (0)    11496 2024-05-28 06:31:35.000000 byma-0.1.9/byma/interface/Time.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-05-28 06:31:35.000000 byma-0.1.9/byma/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.401533 byma-0.1.9/byma/iteral/
+-rw-rw-rw-   0 root         (0) root         (0)     8970 2024-05-28 06:31:35.000000 byma-0.1.9/byma/iteral/GradientDescent.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2024-05-28 06:31:35.000000 byma-0.1.9/byma/iteral/Iteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     6482 2024-05-28 06:31:35.000000 byma-0.1.9/byma/iteral/NesterovMethod.py
+-rw-rw-rw-   0 root         (0) root         (0)     5149 2024-05-28 06:31:35.000000 byma-0.1.9/byma/iteral/Newton.py
+-rw-rw-rw-   0 root         (0) root         (0)     4832 2024-05-28 06:31:35.000000 byma-0.1.9/byma/iteral/OrthogonalSubspace.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2024-05-28 06:31:35.000000 byma-0.1.9/byma/iteral/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.402533 byma-0.1.9/byma/nuby/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-28 06:31:35.000000 byma-0.1.9/byma/nuby/Bifurcation.py
+-rw-rw-rw-   0 root         (0) root         (0)     7951 2024-05-28 06:31:35.000000 byma-0.1.9/byma/nuby/Continuation.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-05-28 06:31:35.000000 byma-0.1.9/byma/nuby/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-05-28 06:31:35.000000 byma-0.1.9/byma/nuby/_nuby.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.403533 byma-0.1.9/byma/numy/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-28 06:31:35.000000 byma-0.1.9/byma/numy/Numy.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-05-28 06:31:35.000000 byma-0.1.9/byma/numy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-05-28 06:31:35.000000 byma-0.1.9/byma/numy/_numy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3576 2024-05-28 06:31:35.000000 byma-0.1.9/byma/numy/integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.403533 byma-0.1.9/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-28 06:31:35.000000 byma-0.1.9/byma/pyplot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6292 2024-05-28 06:31:35.000000 byma-0.1.9/byma/pyplot/plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.411532 byma-0.1.9/byma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3304 2024-05-28 06:31:47.000000 byma-0.1.9/byma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2143 2024-05-28 06:31:47.000000 byma-0.1.9/byma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 06:31:47.000000 byma-0.1.9/byma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-28 06:31:47.000000 byma-0.1.9/byma.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.404533 byma-0.1.9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-05-28 06:31:35.000000 byma-0.1.9/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-28 06:31:35.000000 byma-0.1.9/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-28 06:31:35.000000 byma-0.1.9/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.404533 byma-0.1.9/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.405533 byma-0.1.9/docs/source/autoapi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.405533 byma-0.1.9/docs/source/autoapi/OrthogonalSubspace/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/OrthogonalSubspace/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.405533 byma-0.1.9/docs/source/autoapi/byma/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.405533 byma-0.1.9/docs/source/autoapi/byma/_version/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/_version/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      849 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.406533 byma-0.1.9/docs/source/autoapi/byma/interface/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.406533 byma-0.1.9/docs/source/autoapi/byma/interface/BaseInterface/
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/interface/BaseInterface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.406533 byma-0.1.9/docs/source/autoapi/byma/interface/NonlinearHeat/
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.406533 byma-0.1.9/docs/source/autoapi/byma/interface/Time/
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/interface/Time/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9459 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/interface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.407533 byma-0.1.9/docs/source/autoapi/byma/iteral/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.407533 byma-0.1.9/docs/source/autoapi/byma/iteral/GradientDescent/
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/iteral/GradientDescent/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.407533 byma-0.1.9/docs/source/autoapi/byma/iteral/Iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/iteral/Iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.407533 byma-0.1.9/docs/source/autoapi/byma/iteral/NesterovMethod/
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/iteral/NesterovMethod/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.407533 byma-0.1.9/docs/source/autoapi/byma/iteral/Newton/
+-rw-rw-rw-   0 root         (0) root         (0)     3365 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/iteral/Newton/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.408532 byma-0.1.9/docs/source/autoapi/byma/iteral/OrthogonalSubspace/
+-rw-rw-rw-   0 root         (0) root         (0)     3588 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      509 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.408532 byma-0.1.9/docs/source/autoapi/byma/nuby/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.408532 byma-0.1.9/docs/source/autoapi/byma/nuby/Bifurcation/
+-rw-rw-rw-   0 root         (0) root         (0)      278 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.408532 byma-0.1.9/docs/source/autoapi/byma/nuby/Continuation/
+-rw-rw-rw-   0 root         (0) root         (0)     7798 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/nuby/Continuation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.408532 byma-0.1.9/docs/source/autoapi/byma/nuby/_nuby/
+-rw-rw-rw-   0 root         (0) root         (0)     4840 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/nuby/_nuby/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5104 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/nuby/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.409533 byma-0.1.9/docs/source/autoapi/byma/numy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.409533 byma-0.1.9/docs/source/autoapi/byma/numy/Numy/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/numy/Numy/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.409533 byma-0.1.9/docs/source/autoapi/byma/numy/_numy/
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/numy/_numy/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2108 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/numy/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.409533 byma-0.1.9/docs/source/autoapi/byma/numy/integration/
+-rw-rw-rw-   0 root         (0) root         (0)     4818 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/numy/integration/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.410533 byma-0.1.9/docs/source/autoapi/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     3579 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/pyplot/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.410533 byma-0.1.9/docs/source/autoapi/byma/pyplot/plots/
+-rw-rw-rw-   0 root         (0) root         (0)     3522 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/byma/pyplot/plots/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/autoapi/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3805 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.411532 byma-0.1.9/docs/source/user/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/user/Installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/user/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/user/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-28 06:31:35.000000 byma-0.1.9/docs/source/user/whatisbyma.rst
+-rwxrwxrwx   0 root         (0) root         (0)     1005 2024-05-28 06:31:35.000000 byma-0.1.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-28 06:31:35.000000 byma-0.1.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 06:31:47.412532 byma-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2024-05-28 06:31:35.000000 byma-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:31:47.411532 byma-0.1.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 06:31:35.000000 byma-0.1.9/tests/__init__.py
```

### Comparing `byma-0.1.8/.gitlab-ci.yml` & `byma-0.1.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/LICENSE.md` & `byma-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/PKG-INFO` & `byma-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Project-URL: documentation, https://bytemath.gitlab.io/python/ByMa/index.html
 Project-URL: source, https://gitlab.com/ByteMath/python/ByMa
 Project-URL: download, https://pypi.org/project/byma/#files
```

### Comparing `byma-0.1.8/README.md` & `byma-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/byma/__init__.py` & `byma-0.1.9/byma/__init__.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/byma/interface/BaseInterface.py` & `byma-0.1.9/byma/interface/BaseInterface.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/byma/interface/NonlinearHeat.py` & `byma-0.1.9/byma/interface/NonlinearHeat.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/byma/interface/Time.py` & `byma-0.1.9/byma/interface/Time.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/byma/iteral/GradientDescent.py` & `byma-0.1.9/byma/iteral/GradientDescent.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,21 +23,21 @@
     "sigma": 0.5,
     "alpha": None,
     "c": 1,
     "p": 1
     }
 
 
-def _returns(x, fnorm, dxnorm, mode, method):
+def _returns(minx, fnorm, dxnorm, mode, method):
     """
     Helper function to format the return value based on the mode.
 
     Parameters
     ----------
-    x : array_like
+    minx : array_like
         Root obtained after iterations.
     fnorm : float
         Norm of the residuals.
     dxnorm : float
         Norm of the correction.
     mode : str
         Mode of the output ('full', 'partial', None).
@@ -47,23 +47,23 @@
     Returns
     -------
     tuple
         Tuple containing the formatted output based on the mode.
     """
     
     if mode == 'full':
-        return x, dxnorm, fnorm
+        return minx, dxnorm, fnorm
     elif mode == 'partial':
         if method == 'normal': 
-            return x, dxnorm 
+            return minx[-1], dxnorm 
         else: 
-            return x, fnorm
+            return minx[-1], fnorm
         
     elif ((mode == None) or (mode == False)):
-        return x, dxnorm, fnorm
+        return minx[-1], dxnorm, fnorm
 
 
 def calc_numerical_gradient(f, x, delta_x):
     """Function for computing gradient numerically."""
     val_at_x = f(x)
     val_at_next = f(x + delta_x)
     return (val_at_next - val_at_x) / delta_x
@@ -247,14 +247,15 @@
         print('------ Start iteration ------')
         
     # initialize solution lists
     f_value = f(x)
     df_value = df(x)
     normdx = []
     normf = []
+    minx = []
     
     
     for iter in range(maxit):
         
         # Initialize the prescibe type of method 
         alpha = _step(step, f, df, sigma, alpha, gamma, x, c, p, iter, beta)
         
@@ -266,14 +267,15 @@
             dxnorm = sp.linalg.norm(df(x))
         else:
             fnorm = np.linalg.norm(f(x))
             dxnorm = np.linalg.norm(df(x))
             
         normdx.append(dxnorm)
         normf.append(fnorm)
+        minx.append(x)
         
         if  (verbose != 0 and verbose != False) and (iter % verbose == 0):
             print(f"Gradient Descent  status at iteration {iter + 1}: ||dx|| = {dxnorm} and ||F|| = {fnorm}")
         
         if (fnorm < tol and stop == 'residual-check'):
             if verbose:
                 print(f'Gradient Descent converged in {iter + 1} iterations with ||F|| = {fnorm}')
@@ -288,8 +290,8 @@
             if domain(x) == False:
                 print('Guess is out of bounds')
                 break
         
     if verbose:
         print(f'Gradient Descent did not converge within {maxit} iterations')
 
-    return _returns(x, fnorm=fnorm, dxnorm=normdx, mode=mode, method=stop)
+    return _returns(minx, fnorm=fnorm, dxnorm=normdx, mode=mode, method=stop)
```

### Comparing `byma-0.1.8/byma/iteral/NesterovMethod.py` & `byma-0.1.9/byma/iteral/NesterovMethod.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "domain": None, 
     "l": 1,
     "alpha": None,
     "gamma": 1,
     }
 
 
-def _returns(x, fnorm, dxnorm, mode, method):
+def _returns(minx, fnorm, dxnorm, mode, method):
     """
     Helper function to format the return value based on the mode.
 
     Parameters
     ----------
     x : array_like
         Root obtained after iterations.
@@ -42,23 +42,23 @@
     Returns
     -------
     tuple
         Tuple containing the formatted output based on the mode.
     """
     
     if mode == 'full':
-        return x, dxnorm, fnorm
+        return minx, dxnorm, fnorm
     elif mode == 'partial':
         if method == 'normal': 
-            return x, dxnorm 
+            return minx[-1], dxnorm 
         else: 
-            return x, fnorm
+            return minx[-1], fnorm
         
     elif ((mode == None) or (mode == False)):
-        return x, dxnorm, fnorm
+        return minx[-1], dxnorm, fnorm
 
 
 def calc_numerical_gradient(f, x, delta_x):
     """Function for computing gradient numerically."""
     val_at_x = f(x)
     val_at_next = f(x + delta_x)
     return (val_at_next - val_at_x) / delta_x
@@ -162,15 +162,15 @@
         print('------ Start iteration ------')
         
     # initialize solution lists
     f_value = f(x)
     df_value = df(x)
     normdx = []
     normf = []
-    
+    minx = []
     
     for iter in range(maxit):
         
         # Initialize the prescibe type of method 
         y_curr = x - alpha * df(x)
         x = (1 - gamma) * y_curr + gamma * y_prev
         y_prev = y_curr
@@ -187,14 +187,15 @@
             dxnorm = sp.linalg.norm(df(x))
         else:
             fnorm = np.linalg.norm(f(x))
             dxnorm = np.linalg.norm(df(x))
             
         normdx.append(dxnorm)
         normf.append(fnorm)
+        minx.append(x)
         
         if  (verbose != 0 and verbose != False) and (iter % verbose == 0):
             print(f"Nesterov method  status at iteration {iter + 1}: ||dx|| = {dxnorm} and ||F|| = {fnorm}")
         
         if (fnorm < tol and stop == 'residual-check'):
             if verbose:
                 print(f'Nesterov method converged in {iter + 1} iterations with ||F|| = {fnorm}')
@@ -209,8 +210,8 @@
             if domain(x) == False:
                 print('Guess is out of bounds')
                 break
         
     if verbose:
         print(f'Nesterov method did not converge within {maxit} iterations')
 
-    return _returns(x, fnorm=fnorm, dxnorm=normdx, mode=mode, method=stop)
+    return _returns(minx, fnorm=fnorm, dxnorm=normdx, mode=mode, method=stop)
```

### Comparing `byma-0.1.8/byma/iteral/Newton.py` & `byma-0.1.9/byma/iteral/Newton.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/byma/iteral/OrthogonalSubspace.py` & `byma-0.1.9/byma/iteral/OrthogonalSubspace.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/byma/nuby/Continuation.py` & `byma-0.1.9/byma/nuby/Continuation.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/byma/numy/integration.py` & `byma-0.1.9/byma/numy/integration.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/byma/pyplot/plots.py` & `byma-0.1.9/byma/pyplot/plots.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/byma.egg-info/PKG-INFO` & `byma-0.1.9/byma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Project-URL: documentation, https://bytemath.gitlab.io/python/ByMa/index.html
 Project-URL: source, https://gitlab.com/ByteMath/python/ByMa
 Project-URL: download, https://pypi.org/project/byma/#files
```

### Comparing `byma-0.1.8/byma.egg-info/SOURCES.txt` & `byma-0.1.9/byma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/Makefile` & `byma-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/make.bat` & `byma-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/interface/BaseInterface/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/interface/BaseInterface/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/interface/Time/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/interface/Time/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/interface/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/interface/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/iteral/GradientDescent/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/iteral/GradientDescent/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/iteral/NesterovMethod/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/iteral/NesterovMethod/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/iteral/Newton/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/iteral/Newton/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/nuby/Continuation/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/nuby/Continuation/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/nuby/_nuby/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/nuby/_nuby/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/nuby/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/nuby/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/numy/_numy/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/numy/_numy/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/numy/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/numy/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/numy/integration/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/numy/integration/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/pyplot/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/pyplot/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/autoapi/byma/pyplot/plots/index.rst` & `byma-0.1.9/docs/source/autoapi/byma/pyplot/plots/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/conf.py` & `byma-0.1.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/docs/source/index.rst` & `byma-0.1.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/pyproject.toml` & `byma-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `byma-0.1.8/setup.py` & `byma-0.1.9/setup.py`

 * *Files identical despite different names*

