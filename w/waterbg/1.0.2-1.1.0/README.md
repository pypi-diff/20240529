# Comparing `tmp/waterbg-1.0.2.tar.gz` & `tmp/waterbg-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waterbg-1.0.2.tar", last modified: Fri Oct 20 17:43:56 2023, max compression
+gzip compressed data, was "waterbg-1.1.0.tar", last modified: Wed May 29 18:29:38 2024, max compression
```

## Comparing `waterbg-1.0.2.tar` & `waterbg-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-10-20 17:43:56.324903 waterbg-1.0.2/
--rw-rw-rw-   0        0        0     1188 2023-10-20 17:42:51.000000 waterbg-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      427 2023-10-20 17:43:56.321911 waterbg-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-10-20 17:39:32.000000 waterbg-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-10-20 17:43:56.324903 waterbg-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      545 2023-10-20 17:43:24.000000 waterbg-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-20 17:43:56.320917 waterbg-1.0.2/waterbg.egg-info/
--rw-rw-rw-   0        0        0      427 2023-10-20 17:43:56.000000 waterbg-1.0.2/waterbg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-10-20 17:43:56.000000 waterbg-1.0.2/waterbg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-20 17:43:56.000000 waterbg-1.0.2/waterbg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-10-20 17:43:56.000000 waterbg-1.0.2/waterbg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-10-20 17:43:56.000000 waterbg-1.0.2/waterbg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9099 2023-10-20 17:17:42.000000 waterbg-1.0.2/waterbg.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:29:38.889836 waterbg-1.1.0/
+-rw-rw-rw-   0        0        0     1188 2024-05-29 18:22:28.000000 waterbg-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      427 2024-05-29 18:29:38.878884 waterbg-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-29 18:28:31.000000 waterbg-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:29:38.889836 waterbg-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      545 2024-05-29 18:28:11.000000 waterbg-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:29:38.878884 waterbg-1.1.0/waterbg.egg-info/
+-rw-rw-rw-   0        0        0      427 2024-05-29 18:29:38.000000 waterbg-1.1.0/waterbg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2024-05-29 18:29:38.000000 waterbg-1.1.0/waterbg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:29:38.000000 waterbg-1.1.0/waterbg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-29 18:29:38.000000 waterbg-1.1.0/waterbg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-29 18:29:38.000000 waterbg-1.1.0/waterbg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9091 2024-05-29 18:26:57.000000 waterbg-1.1.0/waterbg.py
```

### Comparing `waterbg-1.0.2/LICENSE` & `waterbg-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `waterbg-1.0.2/setup.py` & `waterbg-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='waterbg',
-    version='1.0.2',
+    version='1.1.0',
     py_modules=['waterbg'],
     license='MIT',
     author='Szabolcs Dombi',
     author_email='cprogrammer1994@gmail.com',
     url='https://github.com/szabolcsdombi/pyodide-water-background',
     project_urls={
         'Source': 'https://github.com/szabolcsdombi/pyodide-water-background',
```

### Comparing `waterbg-1.0.2/waterbg.py` & `waterbg-1.1.0/waterbg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import struct
 
 import js
 import pyodide
-import pyodide_js
 import zengl
 
 js.document.getElementById('loading').remove()
+js.document.getElementById('jquery-terminal-logo').remove()
 js.document.getElementsByClassName('terminal')[0].style.backgroundColor = 'transparent'
 js.document.getElementsByClassName('terminal')[0].style.textShadow = 'black 1px 1px 1px, black 1px 1px 0'
 
 width = js.window.innerWidth
 height = js.window.innerHeight
 
 canvas = js.document.createElement('canvas')
+canvas.id = 'canvas'
 canvas.style.position = 'fixed'
 canvas.style.top = '0'
 canvas.style.left = '0'
 canvas.style.width = width
 canvas.style.height = width
 canvas.width = width
 canvas.height = height
@@ -28,17 +29,14 @@
     premultipliedAlpha=False,
     antialias=False,
     alpha=False,
     depth=False,
     stencil=False,
 )
 
-setup_gl = js.eval(zengl.setup_gl)
-setup_gl(pyodide_js._module, gl)
-
 ctx = zengl.context()
 
 pipeline = ctx.pipeline(
     vertex_shader='''
         #version 300 es
         precision highp float;
```

