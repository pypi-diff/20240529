# Comparing `tmp/djmicrosip_exportaimportaprecios-1.8.3.tar.gz` & `tmp/djmicrosip_exportaimportaprecios-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\djmicrosip_exportaimportaprecios-1.8.3.tar", last modified: Fri Apr 19 16:23:16 2024, max compression
+gzip compressed data, was "dist\djmicrosip_exportaimportaprecios-1.8.4.tar", last modified: Wed May 29 01:31:50 2024, max compression
```

## Comparing `djmicrosip_exportaimportaprecios-1.8.3.tar` & `djmicrosip_exportaimportaprecios-1.8.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 16:23:16.000000 djmicrosip_exportaimportaprecios-1.8.3/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:23:16.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/
--rw-rw-rw-   0        0        0      453 2024-04-19 16:23:13.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/config.pyc
--rw-rw-rw-   0        0        0     3283 2024-04-19 16:23:13.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/forms.pyc
--rw-rw-rw-   0        0        0      542 2024-04-19 16:23:13.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/models.pyc
-drwxrwxrwx   0        0        0        0 2024-04-19 16:23:16.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/static/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:23:16.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/static/djmicrosip_exportaimportaprecios/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:23:16.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/static/djmicrosip_exportaimportaprecios/js/
--rw-rw-rw-   0        0        0       94 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/static/djmicrosip_exportaimportaprecios/js/core.js
-drwxrwxrwx   0        0        0        0 2024-04-19 16:23:16.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/templates/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:23:16.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/
--rw-rw-rw-   0        0        0     1292 2020-10-22 18:31:02.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/base.html
--rw-rw-rw-   0        0        0      650 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/exportar_precios.html
--rw-rw-rw-   0        0        0     1035 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/importar_precios.html
--rw-rw-rw-   0        0        0      416 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/index.html
--rw-rw-rw-   0        0        0     1425 2024-04-06 01:31:51.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/preferencias.html
--rw-rw-rw-   0        0        0      599 2024-04-19 16:23:13.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/urls.pyc
--rw-rw-rw-   0        0        0    12324 2024-04-19 16:23:13.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/views.pyc
--rw-rw-rw-   0        0        0        0 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/__init__.py
--rw-rw-rw-   0        0        0      205 2024-04-19 16:23:13.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/__init__.pyc
-drwxrwxrwx   0        0        0        0 2024-04-19 16:23:16.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-19 16:23:13.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      769 2024-04-19 16:23:13.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-19 16:23:13.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1191 2024-04-19 16:23:14.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       33 2024-04-19 16:23:13.000000 djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      585 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.3/MANIFEST.in
--rw-rw-rw-   0        0        0      769 2024-04-19 16:23:16.000000 djmicrosip_exportaimportaprecios-1.8.3/PKG-INFO
--rw-rw-rw-   0        0        0      295 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.3/README.rst
--rw-rw-rw-   0        0        0       44 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.3/requirements.txt
--rw-rw-rw-   0        0        0       86 2024-04-19 16:23:16.000000 djmicrosip_exportaimportaprecios-1.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1816 2024-04-19 16:23:10.000000 djmicrosip_exportaimportaprecios-1.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/
+-rw-rw-rw-   0        0        0      453 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/config.pyc
+-rw-rw-rw-   0        0        0     3283 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/forms.pyc
+-rw-rw-rw-   0        0        0      542 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/models.pyc
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/static/
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/static/djmicrosip_exportaimportaprecios/
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/static/djmicrosip_exportaimportaprecios/js/
+-rw-rw-rw-   0        0        0       94 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/static/djmicrosip_exportaimportaprecios/js/core.js
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/
+-rw-rw-rw-   0        0        0     1292 2020-10-22 18:31:02.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/base.html
+-rw-rw-rw-   0        0        0      650 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/exportar_precios.html
+-rw-rw-rw-   0        0        0     1035 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/importar_precios.html
+-rw-rw-rw-   0        0        0      416 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/index.html
+-rw-rw-rw-   0        0        0     1425 2024-04-06 01:31:51.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/preferencias.html
+-rw-rw-rw-   0        0        0      599 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/urls.pyc
+-rw-rw-rw-   0        0        0    12245 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/views.pyc
+-rw-rw-rw-   0        0        0        0 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/__init__.py
+-rw-rw-rw-   0        0        0      205 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/__init__.pyc
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      769 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1191 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       33 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      585 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      769 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/README.rst
+-rw-rw-rw-   0        0        0       44 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/requirements.txt
+-rw-rw-rw-   0        0        0       86 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     1816 2024-05-29 01:31:17.000000 djmicrosip_exportaimportaprecios-1.8.4/setup.py
```

### Comparing `djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/forms.pyc` & `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/forms.pyc`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/models.pyc` & `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/models.pyc`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/base.html` & `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/base.html`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/exportar_precios.html` & `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/exportar_precios.html`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/importar_precios.html` & `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/importar_precios.html`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/preferencias.html` & `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/preferencias.html`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/urls.pyc` & `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/urls.pyc`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios/views.pyc` & `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/views.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a 923f 2166 6300 0000 0000 0000  .....?!fc.......
+00000000: 03f3 0d0a 5c85 5666 6300 0000 0000 0000  ....\.Vfc.......
 00000010: 0003 0000 0040 0000 0073 3f01 0000 6400  .....@...s?...d.
 00000020: 0064 0100 6c00 006d 0100 5a01 0001 6400  .d..l..m..Z...d.
 00000030: 0064 0200 6c02 006d 0300 5a03 0001 6400  .d..l..m..Z...d.
 00000040: 0064 0300 6c04 006d 0500 5a05 0001 6404  .d..l..m..Z...d.
 00000050: 0064 0500 6c06 0054 6404 0064 0600 6c07  .d..l..Td..d..l.
 00000060: 006d 0800 5a08 006d 0900 5a09 006d 0a00  .m..Z..m..Z..m..
 00000070: 5a0a 0001 6400 0064 0700 6c0b 005a 0b00  Z...d..d..l..Z..
@@ -188,584 +188,579 @@
 00000bb0: 0c01 0902 0602 0c01 0902 0602 0c01 0902  ................
 00000bc0: 0601 1401 0301 0701 0701 0701 0701 0a03  ................
 00000bd0: 1b01 0c01 0d02 0301 0a02 7336 0000 0064  ..........s6...d
 00000be0: 6a6d 6963 726f 7369 705f 6578 706f 7274  jmicrosip_export
 00000bf0: 6169 6d70 6f72 7461 7072 6563 696f 732f  aimportaprecios/
 00000c00: 696d 706f 7274 6172 5f70 7265 6369 6f73  importar_precios
 00000c10: 2e68 746d 6c63 0200 0000 2300 0000 0c00  .htmlc....#.....
-00000c20: 0000 4300 0000 73bf 0c00 0074 0000 7c00  ..C...s....t..|.
+00000c20: 0000 4300 0000 7399 0c00 0074 0000 7c00  ..C...s....t..|.
 00000c30: 006a 0100 700f 0064 0000 7c00 006a 0300  .j..p..d..|..j..
 00000c40: 8302 007d 0200 6401 007d 0300 7c02 006a  ...}..d..}..|..j
-00000c50: 0400 8300 0072 920c 7c02 006a 0500 6402  .....r..|..j..d.
+00000c50: 0400 8300 0072 6c0c 7c02 006a 0500 6402  .....rl.|..j..d.
 00000c60: 0019 7d04 007c 0200 6a05 0064 0300 197d  ..}..|..j..d...}
 00000c70: 0500 7c02 006a 0500 6404 0019 7d06 0074  ..|..j..d...}..t
 00000c80: 0600 6a07 0064 0500 7c04 006a 0800 8300  ..j..d..|..j....
 00000c90: 0083 0001 7d07 007c 0700 6a09 0064 0600  ....}..|..j..d..
 00000ca0: 8301 007d 0800 7c08 006a 0a00 6407 0018  ...}..|..j..d...
 00000cb0: 7d09 0069 0000 7d0a 0069 0000 7d0b 0069  }..i..}..i..}..i
 00000cc0: 0000 7d0c 007c 0800 6a0b 007d 0d00 6401  ..}..|..j..}..d.
 00000cd0: 007d 0e00 740c 006a 0d00 6a0e 0064 0800  .}..t..j..j..d..
 00000ce0: 6409 0083 0001 6a0f 0083 0000 640a 006b  d.....j.....d..k
 00000cf0: 0200 72d3 0064 0b00 7d0f 006e 0600 640c  ..r..d..}..n..d.
-00000d00: 007d 0f00 7847 0074 1000 7c0f 007c 0d00  .}..xG.t..|..|..
-00000d10: 8302 0044 5d36 007d 1000 7c08 006a 1100  ...D]6.}..|..j..
-00000d20: 640d 0064 0600 640e 007c 1000 8300 027d  d..d..d..|.....}
-00000d30: 1100 7c10 007c 0a00 7c11 003c 7c10 0064  ..|..|..|..<|..d
-00000d40: 0700 177c 0c00 7c11 003c 71e9 0057 7839  ...|..|..<q..Wx9
-00000d50: 0074 1000 7c0f 007c 0d00 8302 0044 5d28  .t..|..|.....D](
-00000d60: 007d 1000 7c08 006a 1100 640d 0064 0600  .}..|..j..d..d..
-00000d70: 640e 007c 1000 8300 027d 1200 7c10 007c  d..|.....}..|..|
-00000d80: 0b00 7c12 003c 7133 0157 6406 007d 1300  ..|..<q3.Wd..}..
-00000d90: 782a 0b7c 1300 7c09 006b 0000 728e 0c7c  x*.|..|..k..r..|
-00000da0: 1300 6407 0037 7d13 007c 1300 4748 7c08  ..d..7}..|..GH|.
-00000db0: 006a 1100 640d 007c 1300 640e 0064 0c00  .j..d..|..d..d..
-00000dc0: 8300 027d 0e00 7412 0074 1300 6a0d 006a  ...}..t..t..j..j
-00000dd0: 1400 640f 007c 0800 6a11 0064 0d00 7c13  ..d..|..j..d..|.
-00000de0: 0064 0e00 6406 0083 0002 8300 0183 0100  .d..d...........
-00000df0: 7d14 007c 0500 7352 0574 0c00 6a0d 006a  }..|..sR.t..j..j
-00000e00: 0e00 6408 0064 0900 8300 016a 0f00 8300  ..d..d.....j....
-00000e10: 0064 0a00 6b02 0072 4602 7412 0074 1500  .d..k..rF.t..t..
-00000e20: 6a0d 006a 1400 6408 007c 0800 6a11 0064  j..j..d..|..j..d
-00000e30: 0d00 7c13 0064 0e00 640c 0083 0002 8300  ..|..d..d.......
-00000e40: 0183 0100 7d15 0064 1000 7c15 0066 0200  ....}..d..|..f..
-00000e50: 4748 7c15 0072 4602 7c15 007c 1400 5f16  GH|..rF.|..|.._.
-00000e60: 007c 1400 6a17 0083 0000 0171 4602 6e00  .|..j......qF.n.
-00000e70: 0074 0c00 6a0d 006a 0e00 6408 0064 1100  .t..j..j..d..d..
-00000e80: 8300 016a 0f00 8300 0064 0a00 6b02 0072  ...j.....d..k..r
-00000e90: 9502 7c08 006a 1100 640d 007c 1300 640e  ..|..j..d..|..d.
-00000ea0: 0064 1200 8300 027d 1600 7c16 007c 1400  .d.....}..|..|..
-00000eb0: 5f18 007c 1400 6a17 0083 0000 016e 0000  _..|..j......n..
-00000ec0: 740c 006a 0d00 6a0e 0064 0800 6413 0083  t..j..j..d..d...
-00000ed0: 0001 6a0f 0083 0000 640a 006b 0200 7298  ..j.....d..k..r.
-00000ee0: 0378 df00 7c0a 006a 1900 8300 0044 5dce  .x..|..j.....D].
-00000ef0: 005c 0200 7d11 007d 1700 7c08 006a 1100  .\..}..}..|..j..
-00000f00: 640d 007c 1300 640e 007c 1700 8300 027d  d..|..d..|.....}
-00000f10: 1800 741a 007c 1800 8301 0072 c302 741b  ..t..|.....r..t.
-00000f20: 006a 0d00 6a0e 0064 0800 7c11 0083 0001  .j..j..d..|.....
-00000f30: 7d19 0074 1200 741c 006a 0d00 6a14 0064  }..t..t..j..j..d
-00000f40: 1400 7c14 0064 1500 7c11 0083 0002 8301  ..|..d..|.......
-00000f50: 007d 1a00 741d 007c 1800 6412 0083 0200  .}..t..|..d.....
-00000f60: 7d18 007c 1a00 7263 037c 1800 7c1a 005f  }..|..rc.|..|.._
-00000f70: 1e00 7c06 007c 1a00 5f1f 007c 1a00 6a17  ..|..|.._..|..j.
-00000f80: 0064 1600 642d 0083 0001 0171 9103 741c  .d..d-.....q..t.
-00000f90: 006a 0d00 6a20 0064 1400 7c14 0064 1800  .j..j .d..|..d..
-00000fa0: 7c19 0064 0400 7c06 0064 1700 7c18 0064  |..d..|..d..|..d
-00000fb0: 1900 6406 0083 0005 0171 c302 71c3 0257  ..d......q..q..W
-00000fc0: 6e00 0074 0c00 6a0d 006a 0e00 6408 0064  n..t..j..j..d..d
-00000fd0: 1a00 8300 016a 0f00 8300 0064 0a00 6b02  .....j.....d..k.
-00000fe0: 0072 d104 7c08 006a 1100 640d 007c 1300  .r..|..j..d..|..
-00000ff0: 640e 007c 0b00 641b 0019 8300 027d 1b00  d..|..d......}..
-00001000: 7c08 006a 1100 640d 007c 1300 640e 007c  |..j..d..|..d..|
-00001010: 0b00 641c 0019 8300 027d 1c00 7c08 006a  ..d......}..|..j
-00001020: 1100 640d 007c 1300 640e 007c 0b00 641d  ..d..|..d..|..d.
-00001030: 0019 8300 027d 1d00 7c08 006a 1100 640d  .....}..|..j..d.
-00001040: 007c 1300 640e 007c 0b00 641e 0019 8300  .|..d..|..d.....
-00001050: 027d 1e00 7c08 006a 1100 640d 007c 1300  .}..|..j..d..|..
-00001060: 640e 007c 0b00 641f 0019 8300 027d 1f00  d..|..d......}..
-00001070: 7412 0074 2100 6a0d 006a 1400 6414 007c  t..t!.j..j..d..|
-00001080: 1400 6420 007c 1b00 8300 0283 0100 7d20  ..d .|........} 
-00001090: 007c 2000 72a3 047c 1c00 7c20 005f 2200  .| .r..|..| ._".
-000010a0: 7c1d 007c 2000 5f23 007c 1e00 7c20 005f  |..| ._#.|..| ._
-000010b0: 2400 7c1f 007c 2000 5f25 007c 2000 6a17  $.|..| ._%.| .j.
-000010c0: 0064 1600 642e 0083 0001 0171 d104 7421  .d..d......q..t!
-000010d0: 006a 0d00 6a20 0064 1400 7c14 0064 2100  .j..j .d..|..d!.
-000010e0: 7c1c 0064 2200 7c1d 0064 2300 7c1e 0064  |..d".|..d#.|..d
-000010f0: 2400 7c1f 0083 0005 016e 0000 740c 006a  $.|......n..t..j
-00001100: 0d00 6a0e 0064 0800 6425 0083 0001 6a0f  ..j..d..d%....j.
-00001110: 0083 0000 640a 006b 0200 7249 0574 1200  ....d..k..rI.t..
-00001120: 7426 006a 0d00 6a14 0064 1400 7c14 0064  t&.j..j..d..|..d
-00001130: 2600 6427 0083 0002 8301 007d 2100 7c21  &.d'.......}!.|!
-00001140: 0072 4905 7c21 0047 487c 0800 6a11 0064  .rI.|!.GH|..j..d
-00001150: 0d00 7c13 0064 0e00 6407 0083 0002 7c21  ..|..d..d.....|!
-00001160: 005f 2700 7c21 006a 1700 8300 0001 7149  ._'.|!.j......qI
-00001170: 056e 0000 6428 007d 0300 7168 017c 0e00  .n..d(.}..qh.|..
-00001180: 7c05 006a 1800 6b02 0072 f808 6429 0047  |..j..k..r..d).G
-00001190: 487c 0e00 7c05 006a 1800 6602 0047 4874  H|..|..j..f..GHt
-000011a0: 0c00 6a0d 006a 0e00 6408 0064 0900 8300  ..j..j..d..d....
-000011b0: 016a 0f00 8300 0064 0a00 6b02 0072 ec05  .j.....d..k..r..
-000011c0: 7412 0074 1500 6a0d 006a 1400 6408 007c  t..t..j..j..d..|
-000011d0: 0800 6a11 0064 0d00 7c13 0064 0e00 640c  ..j..d..|..d..d.
-000011e0: 0083 0002 8300 0183 0100 7d15 0064 1000  ..........}..d..
-000011f0: 7c15 0066 0200 4748 7c15 0072 ec05 7c15  |..f..GH|..r..|.
-00001200: 007c 1400 5f16 007c 1400 6a17 0083 0000  .|.._..|..j.....
-00001210: 0171 ec05 6e00 0074 0c00 6a0d 006a 0e00  .q..n..t..j..j..
-00001220: 6408 0064 1100 8300 016a 0f00 8300 0064  d..d.....j.....d
-00001230: 0a00 6b02 0072 3b06 7c08 006a 1100 640d  ..k..r;.|..j..d.
-00001240: 007c 1300 640e 0064 1200 8300 027d 1600  .|..d..d.....}..
-00001250: 7c16 007c 1400 5f18 007c 1400 6a17 0083  |..|.._..|..j...
-00001260: 0000 016e 0000 740c 006a 0d00 6a0e 0064  ...n..t..j..j..d
-00001270: 0800 6413 0083 0001 6a0f 0083 0000 640a  ..d.....j.....d.
-00001280: 006b 0200 723e 0778 df00 7c0a 006a 1900  .k..r>.x..|..j..
-00001290: 8300 0044 5dce 005c 0200 7d11 007d 1700  ...D]..\..}..}..
-000012a0: 7c08 006a 1100 640d 007c 1300 640e 007c  |..j..d..|..d..|
-000012b0: 1700 8300 027d 1800 741a 007c 1800 8301  .....}..t..|....
-000012c0: 0072 6906 741b 006a 0d00 6a0e 0064 0800  .ri.t..j..j..d..
-000012d0: 7c11 0083 0001 7d19 0074 1200 741c 006a  |.....}..t..t..j
-000012e0: 0d00 6a14 0064 1400 7c14 0064 1500 7c11  ..j..d..|..d..|.
-000012f0: 0083 0002 8301 007d 1a00 741d 007c 1800  .......}..t..|..
-00001300: 6412 0083 0200 7d18 007c 1a00 7209 077c  d.....}..|..r..|
-00001310: 1800 7c1a 005f 1e00 7c06 007c 1a00 5f1f  ..|.._..|..|.._.
-00001320: 007c 1a00 6a17 0064 1600 642f 0083 0001  .|..j..d..d/....
-00001330: 0171 3707 741c 006a 0d00 6a20 0064 1400  .q7.t..j..j .d..
-00001340: 7c14 0064 1800 7c19 0064 0400 7c06 0064  |..d..|..d..|..d
-00001350: 1700 7c18 0064 1900 6406 0083 0005 0171  ..|..d..d......q
-00001360: 6906 7169 0657 6e00 0074 0c00 6a0d 006a  i.qi.Wn..t..j..j
-00001370: 0e00 6408 0064 1a00 8300 016a 0f00 8300  ..d..d.....j....
-00001380: 0064 0a00 6b02 0072 7708 7c08 006a 1100  .d..k..rw.|..j..
-00001390: 640d 007c 1300 640e 007c 0b00 641b 0019  d..|..d..|..d...
-000013a0: 8300 027d 1b00 7c08 006a 1100 640d 007c  ...}..|..j..d..|
-000013b0: 1300 640e 007c 0b00 641c 0019 8300 027d  ..d..|..d......}
-000013c0: 1c00 7c08 006a 1100 640d 007c 1300 640e  ..|..j..d..|..d.
-000013d0: 007c 0b00 641d 0019 8300 027d 1d00 7c08  .|..d......}..|.
-000013e0: 006a 1100 640d 007c 1300 640e 007c 0b00  .j..d..|..d..|..
-000013f0: 641e 0019 8300 027d 1e00 7c08 006a 1100  d......}..|..j..
-00001400: 640d 007c 1300 640e 007c 0b00 641f 0019  d..|..d..|..d...
-00001410: 8300 027d 1f00 7412 0074 2100 6a0d 006a  ...}..t..t!.j..j
-00001420: 1400 6414 007c 1400 6420 007c 1b00 8300  ..d..|..d .|....
-00001430: 0283 0100 7d20 007c 2000 7249 087c 1c00  ....} .| .rI.|..
-00001440: 7c20 005f 2200 7c1d 007c 2000 5f23 007c  | ._".|..| ._#.|
-00001450: 1e00 7c20 005f 2400 7c1f 007c 2000 5f25  ..| ._$.|..| ._%
-00001460: 007c 2000 6a17 0064 1600 6430 0083 0001  .| .j..d..d0....
-00001470: 0171 7708 7421 006a 0d00 6a20 0064 1400  .qw.t!.j..j .d..
-00001480: 7c14 0064 2100 7c1c 0064 2200 7c1d 0064  |..d!.|..d".|..d
-00001490: 2300 7c1e 0064 2400 7c1f 0083 0005 016e  #.|..d$.|......n
-000014a0: 0000 740c 006a 0d00 6a0e 0064 0800 6425  ..t..j..j..d..d%
-000014b0: 0083 0001 6a0f 0083 0000 640a 006b 0200  ....j.....d..k..
-000014c0: 72ef 0874 1200 7426 006a 0d00 6a14 0064  r..t..t&.j..j..d
-000014d0: 1400 7c14 0064 2600 6427 0083 0002 8301  ..|..d&.d'......
-000014e0: 007d 2100 7c21 0072 ef08 7c21 0047 487c  .}!.|!.r..|!.GH|
-000014f0: 0800 6a11 0064 0d00 7c13 0064 0e00 6407  ..j..d..|..d..d.
-00001500: 0083 0002 7c21 005f 2700 7c21 006a 1700  ....|!._'.|!.j..
-00001510: 8300 0001 71ef 086e 0000 6428 007d 0300  ....q..n..d(.}..
-00001520: 7168 017c 1400 6a16 007c 0500 6b02 0072  qh.|..j..|..k..r
-00001530: 6801 740c 006a 0d00 6a0e 0064 0800 6409  h.t..j..j..d..d.
-00001540: 0083 0001 6a0f 0083 0000 640a 006b 0200  ....j.....d..k..
-00001550: 727f 0974 1200 7415 006a 0d00 6a14 0064  r..t..t..j..j..d
-00001560: 0800 7c08 006a 1100 640d 007c 1300 640e  ..|..j..d..|..d.
-00001570: 0064 0c00 8300 0283 0001 8301 007d 1500  .d...........}..
-00001580: 6410 007c 1500 6602 0047 487c 1500 727f  d..|..f..GH|..r.
-00001590: 097c 1500 7c14 005f 1600 7c14 006a 1700  .|..|.._..|..j..
-000015a0: 8300 0001 717f 096e 0000 740c 006a 0d00  ....q..n..t..j..
-000015b0: 6a0e 0064 0800 6411 0083 0001 6a0f 0083  j..d..d.....j...
-000015c0: 0000 640a 006b 0200 72ce 097c 0800 6a11  ..d..k..r..|..j.
-000015d0: 0064 0d00 7c13 0064 0e00 6412 0083 0002  .d..|..d..d.....
-000015e0: 7d16 007c 1600 7c14 005f 1800 7c14 006a  }..|..|.._..|..j
-000015f0: 1700 8300 0001 6e00 0074 0c00 6a0d 006a  ......n..t..j..j
-00001600: 0e00 6408 0064 1300 8300 016a 0f00 8300  ..d..d.....j....
-00001610: 0064 0a00 6b02 0072 d10a 78df 007c 0a00  .d..k..r..x..|..
-00001620: 6a19 0083 0000 445d ce00 5c02 007d 1100  j.....D]..\..}..
-00001630: 7d17 007c 0800 6a11 0064 0d00 7c13 0064  }..|..j..d..|..d
-00001640: 0e00 7c17 0083 0002 7d18 0074 1a00 7c18  ..|.....}..t..|.
-00001650: 0083 0100 72fc 0974 1b00 6a0d 006a 0e00  ....r..t..j..j..
-00001660: 6408 007c 1100 8300 017d 1900 7412 0074  d..|.....}..t..t
-00001670: 1c00 6a0d 006a 1400 6414 007c 1400 6415  ..j..j..d..|..d.
-00001680: 007c 1100 8300 0283 0100 7d1a 0074 1d00  .|........}..t..
-00001690: 7c18 0064 1200 8302 007d 1800 7c1a 0072  |..d.....}..|..r
-000016a0: 9c0a 7c18 007c 1a00 5f1e 007c 0600 7c1a  ..|..|.._..|..|.
-000016b0: 005f 1f00 7c1a 006a 1700 6416 0064 3100  ._..|..j..d..d1.
-000016c0: 8300 0101 71ca 0a74 1c00 6a0d 006a 2000  ....q..t..j..j .
-000016d0: 6414 007c 1400 6418 007c 1900 6404 007c  d..|..d..|..d..|
-000016e0: 0600 6417 007c 1800 6419 0064 0600 8300  ..d..|..d..d....
-000016f0: 0501 71fc 0971 fc09 576e 0000 740c 006a  ..q..q..Wn..t..j
-00001700: 0d00 6a0e 0064 0800 641a 0083 0001 6a0f  ..j..d..d.....j.
-00001710: 0083 0000 640a 006b 0200 720a 0c7c 0800  ....d..k..r..|..
-00001720: 6a11 0064 0d00 7c13 0064 0e00 7c0b 0064  j..d..|..d..|..d
-00001730: 1b00 1983 0002 7d1b 007c 0800 6a11 0064  ......}..|..j..d
-00001740: 0d00 7c13 0064 0e00 7c0b 0064 1c00 1983  ..|..d..|..d....
-00001750: 0002 7d1c 007c 0800 6a11 0064 0d00 7c13  ..}..|..j..d..|.
-00001760: 0064 0e00 7c0b 0064 1d00 1983 0002 7d1d  .d..|..d......}.
-00001770: 007c 0800 6a11 0064 0d00 7c13 0064 0e00  .|..j..d..|..d..
-00001780: 7c0b 0064 1e00 1983 0002 7d1e 007c 0800  |..d......}..|..
-00001790: 6a11 0064 0d00 7c13 0064 0e00 7c0b 0064  j..d..|..d..|..d
-000017a0: 1f00 1983 0002 7d1f 0074 1200 7421 006a  ......}..t..t!.j
-000017b0: 0d00 6a14 0064 1400 7c14 0064 2000 7c1b  ..j..d..|..d .|.
-000017c0: 0083 0002 8301 007d 2000 7c20 0072 dc0b  .......} .| .r..
-000017d0: 7c1c 007c 2000 5f22 007c 1d00 7c20 005f  |..| ._".|..| ._
-000017e0: 2300 7c1e 007c 2000 5f24 007c 1f00 7c20  #.|..| ._$.|..| 
-000017f0: 005f 2500 7c20 006a 1700 6416 0064 3200  ._%.| .j..d..d2.
-00001800: 8300 0101 710a 0c74 2100 6a0d 006a 2000  ....q..t!.j..j .
-00001810: 6414 007c 1400 6421 007c 1c00 6422 007c  d..|..d!.|..d".|
-00001820: 1d00 6423 007c 1e00 6424 007c 1f00 8300  ..d#.|..d$.|....
-00001830: 0501 6e00 0074 0c00 6a0d 006a 0e00 6408  ..n..t..j..j..d.
-00001840: 0064 2500 8300 016a 0f00 8300 0064 0a00  .d%....j.....d..
-00001850: 6b02 0072 820c 7412 0074 2600 6a0d 006a  k..r..t..t&.j..j
-00001860: 1400 6414 007c 1400 6426 0064 2700 8300  ..d..|..d&.d'...
-00001870: 0283 0100 7d21 007c 2100 7282 0c7c 2100  ....}!.|!.r..|!.
-00001880: 4748 7c08 006a 1100 640d 007c 1300 640e  GH|..j..d..|..d.
-00001890: 0064 0700 8300 027c 2100 5f27 007c 2100  .d.....|!._'.|!.
-000018a0: 6a17 0083 0000 0171 820c 6e00 0064 2800  j......q..n..d(.
-000018b0: 7d03 0071 6801 7168 0157 6e00 0069 0200  }..qh.qh.Wn..i..
-000018c0: 7c02 0064 2a00 367c 0300 642b 0036 7d22  |..d*.6|..d+.6}"
-000018d0: 0074 2800 7c01 007c 2200 642c 0074 2900  .t(.|..|".d,.t).
-000018e0: 7c00 0083 0100 8302 0153 2833 0000 004e  |........S(3...N
-000018f0: 521d 0000 0074 0700 0000 6172 6368 6976  R....t....archiv
-00001900: 6f52 2300 0000 7406 0000 006d 6f6e 6564  oR#...t....moned
-00001910: 6174 0d00 0000 6669 6c65 5f63 6f6e 7465  at....file_conte
-00001920: 6e74 7369 0000 0000 6901 0000 0052 1600  ntsi....i....R..
-00001930: 0000 5218 0000 0052 2200 0000 6904 0000  ..R....R"...i...
-00001940: 0069 0300 0000 7404 0000 0072 6f77 7874  .i....t....rowxt
-00001950: 0400 0000 636f 6c78 7402 0000 0069 6473  ....colxt....ids
-00001960: 0400 0000 2d2d 2d2d 5221 0000 0069 0200  ....----R!...i..
-00001970: 0000 521e 0000 0074 0800 0000 6172 7469  ..R....t....arti
-00001980: 6375 6c6f 7416 0000 0070 7265 6369 6f5f  culot....precio_
-00001990: 656d 7072 6573 615f 5f6e 6f6d 6272 6574  empresa__nombret
-000019a0: 0d00 0000 7570 6461 7465 5f66 6965 6c64  ....update_field
-000019b0: 7374 0600 0000 7072 6563 696f 740e 0000  st....preciot...
-000019c0: 0070 7265 6369 6f5f 656d 7072 6573 6174  .precio_empresat
-000019d0: 0600 0000 6d61 7267 656e 5220 0000 0074  ....margenR ...t
-000019e0: 0700 0000 416c 6d61 6365 6e74 0c00 0000  ....Almacent....
-000019f0: 4c6f 6361 6c69 7a61 6369 6f6e 7406 0000  Localizaciont...
-00001a00: 004d 6178 696d 6f74 0700 0000 5265 6f72  .Maximot....Reor
-00001a10: 6465 6e74 0600 0000 4d69 6e69 6d6f 740f  dent....Minimot.
-00001a20: 0000 0061 6c6d 6163 656e 5f5f 6e6f 6d62  ...almacen__nomb
-00001a30: 7265 740c 0000 006c 6f63 616c 697a 6163  ret....localizac
-00001a40: 696f 6e74 0600 0000 6d61 7869 6d6f 7407  iont....maximot.
-00001a50: 0000 0072 656f 7264 656e 7406 0000 006d  ...reordent....m
-00001a60: 696e 696d 6f52 1f00 0000 740c 0000 0072  inimoR....t....r
-00001a70: 6f6c 5f5f 6573 5f70 7061 6c74 0100 0000  ol__es_ppalt....
-00001a80: 5373 2400 0000 4172 7469 6375 6c6f 7320  Ss$...Articulos 
-00001a90: 6163 7475 616c 697a 6164 6f73 2063 6f72  actualizados cor
-00001aa0: 7265 6374 616d 656e 7465 730d 0000 006c  rectamentes....l
-00001ab0: 696e 6561 2061 7263 6869 766f 5229 0000  inea archivoR)..
-00001ac0: 0074 0300 0000 6d73 6752 1200 0000 2802  .t....msgR....(.
-00001ad0: 0000 0052 4100 0000 5239 0000 0028 0400  ...RA...R9...(..
-00001ae0: 0000 524a 0000 0052 4b00 0000 524c 0000  ..RJ...RK...RL..
-00001af0: 0052 4d00 0000 2802 0000 0052 4100 0000  .RM...(....RA...
-00001b00: 5239 0000 0028 0400 0000 524a 0000 0052  R9...(....RJ...R
-00001b10: 4b00 0000 524c 0000 0052 4d00 0000 2802  K...RL...RM...(.
-00001b20: 0000 0052 4100 0000 5239 0000 0028 0400  ...RA...R9...(..
-00001b30: 0000 524a 0000 0052 4b00 0000 524c 0000  ..RJ...RK...RL..
-00001b40: 0052 4d00 0000 282a 0000 0052 0500 0000  .RM...(*...R....
-00001b50: 5232 0000 0052 3100 0000 7405 0000 0046  R2...R1...t....F
-00001b60: 494c 4553 5233 0000 0074 0c00 0000 636c  ILESR3...t....cl
-00001b70: 6561 6e65 645f 6461 7461 7404 0000 0078  eaned_datat....x
-00001b80: 6c72 6474 0d00 0000 6f70 656e 5f77 6f72  lrdt....open_wor
-00001b90: 6b62 6f6f 6b74 0400 0000 7265 6164 740e  kbookt....readt.
-00001ba0: 0000 0073 6865 6574 5f62 795f 696e 6465  ...sheet_by_inde
-00001bb0: 7874 0500 0000 6e72 6f77 7374 0500 0000  xt....nrowst....
-00001bc0: 6e63 6f6c 7352 2a00 0000 522b 0000 0052  ncolsR*...R+...R
-00001bd0: 2f00 0000 5230 0000 0074 0500 0000 7261  /...R0...t....ra
-00001be0: 6e67 6574 0a00 0000 6365 6c6c 5f76 616c  nget....cell_val
-00001bf0: 7565 5209 0000 0074 0800 0000 4172 7469  ueR....t....Arti
-00001c00: 6375 6c6f 522c 0000 0074 0e00 0000 4c69  culoR,...t....Li
-00001c10: 6e65 6141 7274 6963 756c 6f73 5223 0000  neaArticulosR#..
-00001c20: 0052 3400 0000 5216 0000 0074 0500 0000  .R4...R....t....
-00001c30: 6974 656d 7352 1000 0000 740d 0000 0050  itemsR....t....P
-00001c40: 7265 6369 6f45 6d70 7265 7361 740e 0000  recioEmpresat...
-00001c50: 0041 7274 6963 756c 6f50 7265 6369 6f74  .ArticuloPreciot
-00001c60: 0500 0000 726f 756e 6452 4100 0000 5239  ....roundRA...R9
-00001c70: 0000 0052 2e00 0000 740d 0000 0041 7274  ...R....t....Art
-00001c80: 6963 756c 6f4e 6976 656c 524a 0000 0052  iculoNivelRJ...R
-00001c90: 4b00 0000 524c 0000 0052 4d00 0000 740d  K...RL...RM...t.
-00001ca0: 0000 0041 7274 6963 756c 6f43 6c61 7665  ...ArticuloClave
-00001cb0: 5225 0000 0052 0000 0000 5201 0000 0028  R%...R....R....(
-00001cc0: 2300 0000 5213 0000 0052 1400 0000 5229  #...R....R....R)
-00001cd0: 0000 0052 5000 0000 5238 0000 0052 2300  ...RP...R8...R#.
-00001ce0: 0000 5239 0000 0074 0400 0000 626f 6f6b  ..R9...t....book
-00001cf0: 7405 0000 0073 6865 6574 7408 0000 006e  t....sheett....n
-00001d00: 756d 5f72 6f77 7374 1200 0000 7072 6563  um_rowst....prec
-00001d10: 696f 735f 706f 7369 6369 6f6e 6573 7412  ios_posicionest.
-00001d20: 0000 006e 6976 656c 6573 5f70 6f73 6963  ...niveles_posic
-00001d30: 696f 6e65 7374 1300 0000 6d61 7267 656e  ionest....margen
-00001d40: 6573 5f70 6f73 6963 696f 6e65 7352 5800  es_posicionesRX.
-00001d50: 0000 740c 0000 006c 696e 6561 5f6e 6f6d  ..t....linea_nom
-00001d60: 6272 6574 0300 0000 6e75 6d74 0800 0000  bret....numt....
-00001d70: 6375 7272 5f63 6f6c 740d 0000 0070 7265  curr_colt....pre
-00001d80: 6369 6f5f 6e6f 6d62 7265 7410 0000 0063  cio_nombret....c
-00001d90: 6f6c 5f6e 6976 656c 5f6e 6f6d 6272 6574  ol_nivel_nombret
-00001da0: 0800 0000 6375 7272 5f72 6f77 523e 0000  ....curr_rowR>..
-00001db0: 0074 0900 0000 6c69 6e65 615f 6172 7452  .t....linea_artR
-00001dc0: 2600 0000 7408 0000 0070 6f73 6963 696f  &...t....posicio
-00001dd0: 6e52 4100 0000 5242 0000 0074 0f00 0000  nRA...RB...t....
-00001de0: 6172 7469 6375 6c6f 5f70 7265 6369 6f74  articulo_preciot
-00001df0: 0700 0000 616c 6d61 6365 6e52 4a00 0000  ....almacenRJ...
-00001e00: 524b 0000 0052 4c00 0000 524d 0000 0074  RK...RL...RM...t
-00001e10: 0e00 0000 6e69 7665 6c5f 6172 7469 6375  ....nivel_articu
-00001e20: 6c6f 740e 0000 0061 7274 6963 756c 6f5f  lot....articulo_
-00001e30: 636c 6176 6552 3600 0000 2800 0000 0028  claveR6...(....(
-00001e40: 0000 0000 7373 0000 0045 3a5c 5265 706f  ....ss...E:\Repo
-00001e50: 7369 746f 7269 6f73 2032 3032 325c 5765  sitorios 2022\We
-00001e60: 625c 646a 6d69 6372 6f73 6970 5f61 7070  b\djmicrosip_app
-00001e70: 735c 646a 6d69 6372 6f73 6970 5f65 7870  s\djmicrosip_exp
-00001e80: 6f72 7461 696d 706f 7274 6170 7265 6369  ortaimportapreci
-00001e90: 6f73 5c64 6a6d 6963 726f 7369 705f 6578  os\djmicrosip_ex
-00001ea0: 706f 7274 6169 6d70 6f72 7461 7072 6563  portaimportaprec
-00001eb0: 696f 735c 7669 6577 732e 7079 7415 0000  ios\views.pyt...
-00001ec0: 0069 6d70 6f72 7461 725f 7072 6563 696f  .importar_precio
-00001ed0: 735f 7669 6577 7300 0000 738c 0100 0000  s_views...s.....
-00001ee0: 021b 0106 010c 010d 010d 010d 0218 010f  ................
-00001ef0: 010d 0206 0106 0106 0109 0106 0121 0109  .............!..
-00001f00: 0206 0216 0118 010a 0112 0216 0118 010e  ................
-00001f10: 0206 010f 010a 0105 0118 032d 0306 0321  ...........-...!
-00001f20: 012d 010b 0106 0109 0110 0221 0118 0109  .-.........!....
-00001f30: 010d 0321 0119 0118 010c 0115 0221 010f  ...!.........!..
-00001f40: 0106 0109 0109 0113 020c 0106 0106 0106  ................
-00001f50: 0106 0111 0221 011c 011c 011c 011c 011c  .....!..........
-00001f60: 0221 0106 0109 0109 0109 0109 0113 020c  .!..............
-00001f70: 0106 0106 0106 0106 010a 0621 0121 0106  ...........!.!..
-00001f80: 0105 021b 0110 0209 030f 0105 010e 0221  ...............!
-00001f90: 012d 010b 0106 0109 0110 0221 0118 0109  .-.........!....
-00001fa0: 010d 0321 0119 0118 010c 0115 0221 010f  ...!.........!..
-00001fb0: 0106 0109 0109 0113 020c 0106 0106 0106  ................
-00001fc0: 0106 0111 0221 011c 011c 011c 011c 011c  .....!..........
-00001fd0: 0221 0106 0109 0109 0109 0109 0113 020c  .!..............
-00001fe0: 0106 0106 0106 0106 010a 0421 0121 0106  ...........!.!..
-00001ff0: 0105 011b 0110 0209 050f 0221 012d 010b  ...........!.-..
-00002000: 0106 0109 0110 0221 0118 0109 010d 0321  .......!.......!
-00002010: 0119 0118 010c 0115 0221 010f 0106 0109  .........!......
-00002020: 0109 0113 020c 0106 0106 0106 0106 0111  ................
-00002030: 0221 011c 011c 011c 011c 011c 0221 0106  .!...........!..
-00002040: 0109 0109 0109 0109 0113 020c 0106 0106  ................
-00002050: 0106 0106 010a 0421 0121 0106 0105 011b  .......!.!......
-00002060: 0110 0210 0303 0107 010a 0273 3600 0000  ...........s6...
-00002070: 646a 6d69 6372 6f73 6970 5f65 7870 6f72  djmicrosip_expor
-00002080: 7461 696d 706f 7274 6170 7265 6369 6f73  taimportaprecios
-00002090: 2f65 7870 6f72 7461 725f 7072 6563 696f  /exportar_precio
-000020a0: 732e 6874 6d6c 6302 0000 0019 0000 0007  s.htmlc.........
-000020b0: 0000 0043 0000 0073 bd08 0000 7400 007c  ...C...s....t..|
-000020c0: 0000 6a01 0070 0f00 6400 0083 0100 7d02  ..j..p..d.....}.
-000020d0: 007c 0200 6a03 0083 0000 7297 087c 0200  .|..j.....r..|..
-000020e0: 6a04 0064 0100 197d 0300 7405 0064 0200  j..d...}..t..d..
-000020f0: 6403 0083 0001 7d04 007c 0300 7278 0064  d.....}..|..rx.d
-00002100: 0400 7c03 006a 0600 6a07 0064 0500 6406  ..|..j..j..d..d.
-00002110: 0083 0200 167c 0400 6407 003c 7408 006a  .....|..d..<t..j
-00002120: 0900 6a0a 0064 0100 7c03 0083 0001 7d05  ..j..d..|.....}.
-00002130: 006e 1900 6408 007c 0400 6407 003c 7408  .n..d..|..d..<t.
-00002140: 006a 0900 6a0b 0083 0000 7d05 0074 0c00  .j..j.....}..t..
-00002150: 6a0d 0083 0000 7d06 007c 0600 6a0e 0064  j.....}..|..j..d
-00002160: 0900 8301 007d 0700 640a 007d 0800 7c07  .....}..d..}..|.
-00002170: 006a 0f00 640b 0083 0100 6a10 0064 0b00  .j..d.....j..d..
-00002180: 640c 0083 0200 0174 1100 6a09 006a 1200  d......t..j..j..
-00002190: 640d 0064 0e00 8300 016a 1300 8300 0064  d..d.....j.....d
-000021a0: 0f00 6b02 0072 7201 7c07 006a 0f00 640b  ..k..rr.|..j..d.
-000021b0: 0083 0100 6a10 0064 1000 6411 0083 0200  ....j..d..d.....
-000021c0: 017c 0700 6a0f 0064 0b00 8301 006a 1000  .|..j..d.....j..
-000021d0: 640a 0064 1200 8302 0001 7c08 0064 1000  d..d......|..d..
-000021e0: 177d 0800 7411 006a 0900 6a12 0064 0d00  .}..t..j..j..d..
-000021f0: 6413 0083 0001 6a13 0083 0000 640f 006b  d.....j.....d..k
-00002200: 0200 72d2 017c 0700 6a0f 0064 0b00 8301  ..r..|..j..d....
-00002210: 006a 1000 6414 0064 1500 8302 0001 7c08  .j..d..d......|.
-00002220: 0064 1000 177d 0800 71d2 016e 6000 7c07  .d...}..q..n`.|.
-00002230: 006a 0f00 640b 0083 0100 6a10 0064 1000  .j..d.....j..d..
-00002240: 6412 0083 0200 0174 1100 6a09 006a 1200  d......t..j..j..
-00002250: 640d 0064 1300 8300 016a 1300 8300 0064  d..d.....j.....d
-00002260: 0f00 6b02 0072 d201 7c07 006a 0f00 640b  ..k..r..|..j..d.
-00002270: 0083 0100 6a10 0064 0a00 6415 0083 0200  ....j..d..d.....
-00002280: 017c 0800 6410 0017 7d08 006e 0000 7414  .|..d...}..n..t.
-00002290: 006a 0900 6a0b 0083 0000 7d09 0069 0000  .j..j.....}..i..
-000022a0: 7d0a 0074 1100 6a09 006a 1200 640d 0064  }..t..j..j..d..d
-000022b0: 1600 8300 016a 1300 8300 0064 0f00 6b02  .....j.....d..k.
-000022c0: 0072 4f02 7844 007c 0900 445d 3900 7d0b  .rO.xD.|..D]9.}.
-000022d0: 007c 0700 6a0f 0064 0b00 8301 006a 1000  .|..j..d.....j..
-000022e0: 7c08 007c 0b00 6a06 0083 0200 017c 0800  |..|..j......|..
-000022f0: 7c0a 007c 0b00 6a06 003c 7c08 0064 1000  |..|..j..<|..d..
-00002300: 377d 0800 710f 0257 6e00 0074 1500 6a09  7}..q..Wn..t..j.
-00002310: 006a 0b00 8300 007d 0c00 6900 007d 0d00  .j.....}..i..}..
-00002320: 7411 006a 0900 6a12 0064 0d00 6417 0083  t..j..j..d..d...
-00002330: 0001 6a13 0083 0000 640f 006b 0200 7269  ..j.....d..k..ri
-00002340: 037c 0700 6a0f 0064 0b00 8301 006a 1000  .|..j..d.....j..
-00002350: 7c08 0064 1800 8302 0001 7c08 007c 0d00  |..d......|..|..
-00002360: 6418 003c 7c08 0064 1000 377d 0800 7c07  d..<|..d..7}..|.
-00002370: 006a 0f00 640b 0083 0100 6a10 007c 0800  .j..d.....j..|..
-00002380: 6419 0083 0200 017c 0800 7c0d 0064 1900  d......|..|..d..
-00002390: 3c7c 0800 6410 0037 7d08 007c 0700 6a0f  <|..d..7}..|..j.
-000023a0: 0064 0b00 8301 006a 1000 7c08 0064 1a00  .d.....j..|..d..
-000023b0: 8302 0001 7c08 007c 0d00 641a 003c 7c08  ....|..|..d..<|.
-000023c0: 0064 1000 377d 0800 7c07 006a 0f00 640b  .d..7}..|..j..d.
-000023d0: 0083 0100 6a10 007c 0800 641b 0083 0200  ....j..|..d.....
-000023e0: 017c 0800 7c0d 0064 1b00 3c7c 0800 6410  .|..|..d..<|..d.
-000023f0: 0037 7d08 007c 0700 6a0f 0064 0b00 8301  .7}..|..j..d....
-00002400: 006a 1000 7c08 0064 1c00 8302 0001 7c08  .j..|..d......|.
-00002410: 007c 0d00 641c 003c 7c08 0064 1000 377d  .|..d..<|..d..7}
-00002420: 0800 6e00 0064 1000 7d0e 0074 1100 6a09  ..n..d..}..t..j.
-00002430: 006a 1200 640d 0064 1700 8300 016a 1300  .j..d..d.....j..
-00002440: 8300 0064 0f00 6b02 0072 7a06 7c05 006a  ...d..k..rz.|..j
-00002450: 1600 641d 0064 1e00 7417 0083 0101 7d0f  ..d..d..t.....}.
-00002460: 0074 1500 6a09 006a 0a00 641f 007c 0f00  .t..j..j..d..|..
-00002470: 8300 017d 0c00 78c9 047c 0c00 445d b202  ...}..x..|..D]..
-00002480: 7d10 0074 1800 7419 006a 0900 6a0a 0064  }..t..t..j..j..d
-00002490: 2000 7c10 006a 1a00 6421 0064 2200 8300   .|..j..d!.d"...
-000024a0: 0283 0100 7d11 007c 1100 72fd 037c 1100  ....}..|..r..|..
-000024b0: 6a1b 007d 1200 6e06 0064 2300 7d12 007c  j..}..n..d#.}..|
-000024c0: 0700 6a0f 007c 0e00 8301 006a 1000 640b  ..j..|.....j..d.
-000024d0: 007c 1000 6a1a 006a 1c00 8302 0001 7411  .|..j..j......t.
-000024e0: 006a 0900 6a12 0064 0d00 640e 0083 0001  .j..j..d..d.....
-000024f0: 6a13 0083 0000 640f 006b 0200 72c4 047c  j.....d..k..r..|
-00002500: 0700 6a0f 007c 0e00 8301 006a 1000 6410  ..j..|.....j..d.
-00002510: 007c 1200 8302 0001 7c07 006a 0f00 7c0e  .|......|..j..|.
-00002520: 0083 0100 6a10 0064 0a00 7c10 006a 1a00  ....j..d..|..j..
-00002530: 6a06 0083 0200 0174 1100 6a09 006a 1200  j......t..j..j..
-00002540: 640d 0064 1300 8300 016a 1300 8300 0064  d..d.....j.....d
-00002550: 0f00 6b02 0072 2905 7c07 006a 0f00 7c0e  ..k..r).|..j..|.
-00002560: 0083 0100 6a10 0064 1400 7c10 006a 1a00  ....j..d..|..j..
-00002570: 6a1d 006a 0600 8302 0001 7129 056e 6500  j..j......q).ne.
-00002580: 7c07 006a 0f00 7c0e 0083 0100 6a10 0064  |..j..|.....j..d
-00002590: 1000 7c10 006a 1a00 6a06 0083 0200 0174  ..|..j..j......t
-000025a0: 1100 6a09 006a 1200 640d 0064 1300 8300  ..j..j..d..d....
-000025b0: 016a 1300 8300 0064 0f00 6b02 0072 2905  .j.....d..k..r).
-000025c0: 7c07 006a 0f00 7c0e 0083 0100 6a10 0064  |..j..|.....j..d
-000025d0: 0a00 7c10 006a 1a00 6a1d 006a 0600 8302  ..|..j..j..j....
-000025e0: 0001 6e00 0074 1e00 6a09 006a 0a00 6420  ..n..t..j..j..d 
-000025f0: 007c 1000 6a1a 0083 0001 7d13 0074 1100  .|..j.....}..t..
-00002600: 6a09 006a 1200 640d 0064 1600 8300 016a  j..j..d..d.....j
-00002610: 1300 8300 0064 0f00 6b02 0072 b105 784c  .....d..k..r..xL
-00002620: 007c 1300 445d 4100 7d14 007c 1400 7269  .|..D]A.}..|..ri
-00002630: 057c 1400 6a1f 007d 1500 7c14 006a 2000  .|..j..}..|..j .
-00002640: 6a06 007d 1600 7c07 006a 0f00 7c0e 0083  j..}..|..j..|...
-00002650: 0100 6a10 007c 0a00 7c16 0019 7c15 0083  ..j..|..|...|...
-00002660: 0200 0171 6905 7169 0557 6e00 007c 1000  ...qi.qi.Wn..|..
-00002670: 6a1a 0072 6906 7c10 0072 6906 7c07 006a  j..ri.|..ri.|..j
-00002680: 0f00 7c0e 0083 0100 6a10 007c 0d00 6418  ..|.....j..|..d.
-00002690: 0019 7c10 006a 2100 6a06 0083 0200 017c  ..|..j!.j......|
-000026a0: 0700 6a0f 007c 0e00 8301 006a 1000 7c0d  ..j..|.....j..|.
-000026b0: 0064 1900 197c 1000 6a22 0083 0200 017c  .d...|..j".....|
-000026c0: 0700 6a0f 007c 0e00 8301 006a 1000 7c0d  ..j..|.....j..|.
-000026d0: 0064 1a00 197c 1000 6a23 0083 0200 017c  .d...|..j#.....|
-000026e0: 0700 6a0f 007c 0e00 8301 006a 1000 7c0d  ..j..|.....j..|.
-000026f0: 0064 1b00 197c 1000 6a24 0083 0200 017c  .d...|..j$.....|
-00002700: 0700 6a0f 007c 0e00 8301 006a 1000 7c0d  ..j..|.....j..|.
-00002710: 0064 1c00 197c 1000 6a25 0083 0200 0171  .d...|..j%.....q
-00002720: 6906 6e00 007c 0e00 6410 0037 7d0e 0071  i.n..|..d..7}..q
-00002730: c103 576e 0c02 7809 027c 0500 445d 0102  ..Wn..x..|..D]..
-00002740: 7d17 007c 1700 6a1d 0047 4874 1800 7419  }..|..j..GHt..t.
-00002750: 006a 0900 6a0a 0064 2000 7c17 0064 2100  .j..j..d .|..d!.
-00002760: 6422 0083 0002 8301 007d 1100 7c17 0072  d".......}..|..r
-00002770: 8106 640b 007d 1500 7c11 0072 ce06 7c11  ..d..}..|..r..|.
-00002780: 006a 1b00 7d12 006e 0600 6423 007d 1200  .j..}..n..d#.}..
-00002790: 7c07 006a 0f00 7c0e 0083 0100 6a10 0064  |..j..|.....j..d
-000027a0: 0b00 7c17 006a 1c00 8302 0001 7411 006a  ..|..j......t..j
-000027b0: 0900 6a12 0064 0d00 640e 0083 0001 6a13  ..j..d..d.....j.
-000027c0: 0083 0000 640f 006b 0200 728c 077c 0700  ....d..k..r..|..
-000027d0: 6a0f 007c 0e00 8301 006a 1000 6410 007c  j..|.....j..d..|
-000027e0: 1200 8302 0001 7c07 006a 0f00 7c0e 0083  ......|..j..|...
-000027f0: 0100 6a10 0064 0a00 7c17 006a 0600 8302  ..j..d..|..j....
-00002800: 0001 7411 006a 0900 6a12 0064 0d00 6413  ..t..j..j..d..d.
-00002810: 0083 0001 6a13 0083 0000 640f 006b 0200  ....j.....d..k..
-00002820: 72eb 077c 0700 6a0f 007c 0e00 8301 006a  r..|..j..|.....j
-00002830: 1000 6414 007c 1700 6a1d 006a 0600 8302  ..d..|..j..j....
-00002840: 0001 71eb 076e 5f00 7c07 006a 0f00 7c0e  ..q..n_.|..j..|.
-00002850: 0083 0100 6a10 0064 1000 7c17 006a 0600  ....j..d..|..j..
-00002860: 8302 0001 7411 006a 0900 6a12 0064 0d00  ....t..j..j..d..
-00002870: 6413 0083 0001 6a13 0083 0000 640f 006b  d.....j.....d..k
-00002880: 0200 72eb 077c 0700 6a0f 007c 0e00 8301  ..r..|..j..|....
-00002890: 006a 1000 640a 007c 1700 6a1d 006a 0600  .j..d..|..j..j..
-000028a0: 8302 0001 6e00 0074 1e00 6a09 006a 0a00  ....n..t..j..j..
-000028b0: 6420 007c 1700 8300 017d 1300 7411 006a  d .|.....}..t..j
-000028c0: 0900 6a12 0064 0d00 6416 0083 0001 6a13  ..j..d..d.....j.
-000028d0: 0083 0000 640f 006b 0200 7270 0878 4c00  ....d..k..rp.xL.
-000028e0: 7c13 0044 5d41 007d 1400 7c14 0072 2808  |..D]A.}..|..r(.
-000028f0: 7c14 006a 1f00 7d15 007c 1400 6a20 006a  |..j..}..|..j .j
-00002900: 0600 7d16 007c 0700 6a0f 007c 0e00 8301  ..}..|..j..|....
-00002910: 006a 1000 7c0a 007c 1600 197c 1500 8302  .j..|..|...|....
-00002920: 0001 7128 0871 2808 576e 0000 7c0c 0047  ..q(.q(.Wn..|..G
-00002930: 487c 0e00 6410 0037 7d0e 0071 8106 7181  H|..d..7}..q..q.
-00002940: 0657 7c06 006a 2600 7c04 0083 0100 017c  .W|..j&.|......|
-00002950: 0400 5369 0100 7c02 0064 2400 367d 1800  ..Si..|..d$.6}..
-00002960: 7427 007c 0100 7c18 0064 2500 7428 007c  t'.|..|..d%.t(.|
-00002970: 0000 8301 0083 0201 5328 2600 0000 4e52  ........S(&...NR
-00002980: 2300 0000 7408 0000 006d 696d 6574 7970  #...t....mimetyp
-00002990: 6573 1400 0000 6170 706c 6963 6174 696f  es....applicatio
-000029a0: 6e2f 6d73 2d65 7863 656c 731b 0000 0061  n/ms-excels....a
-000029b0: 7474 6163 686d 656e 743b 2066 696c 656e  ttachment; filen
-000029c0: 616d 653d 2573 2e78 6c73 7401 0000 0020  ame=%s.xlst.... 
-000029d0: 7401 0000 005f 7313 0000 0043 6f6e 7465  t...._s....Conte
-000029e0: 6e74 2d44 6973 706f 7369 7469 6f6e 731d  nt-Dispositions.
-000029f0: 0000 0061 7474 6163 686d 656e 743b 2066  ...attachment; f
-00002a00: 696c 656e 616d 653d 6172 7473 2e78 6c73  ilename=arts.xls
-00002a10: 7407 0000 0050 7265 6369 6f73 6902 0000  t....Preciosi...
-00002a20: 0069 0000 0000 7402 0000 0049 6452 1600  .i....t....IdR..
-00002a30: 0000 521f 0000 0052 2200 0000 6901 0000  ..R....R"...i...
-00002a40: 0074 0500 0000 436c 6176 6552 5b00 0000  .t....ClaveR[...
-00002a50: 5218 0000 0069 0300 0000 7405 0000 004c  R....i....t....L
-00002a60: 696e 6561 521e 0000 0052 2000 0000 5244  ineaR....R ...RD
-00002a70: 0000 0052 4500 0000 5246 0000 0052 4700  ...RE...RF...RG.
-00002a80: 0000 5248 0000 0052 3d00 0000 7404 0000  ..RH...R=...t...
-00002a90: 0066 6c61 7474 1000 0000 6172 7469 6375  .flatt....articu
-00002aa0: 6c6f 5f5f 6964 5f5f 696e 523e 0000 0052  lo__id__inR>...R
-00002ab0: 4e00 0000 524f 0000 0052 1d00 0000 5229  N...RO...R....R)
-00002ac0: 0000 0052 1200 0000 2829 0000 0052 0400  ...R....()...R..
-00002ad0: 0000 5232 0000 0052 3100 0000 5233 0000  ..R2...R1...R3..
-00002ae0: 0052 5200 0000 5207 0000 0052 1600 0000  .RR...R....R....
-00002af0: 7407 0000 0072 6570 6c61 6365 525b 0000  t....replaceR[..
-00002b00: 0052 2b00 0000 522c 0000 0074 0300 0000  .R+...R,...t....
-00002b10: 616c 6c74 0400 0000 786c 7774 7408 0000  allt....xlwtt...
-00002b20: 0057 6f72 6b62 6f6f 6b74 0900 0000 6164  .Workbookt....ad
-00002b30: 645f 7368 6565 7474 0300 0000 726f 7774  d_sheett....rowt
-00002b40: 0500 0000 7772 6974 6552 2a00 0000 522f  ....writeR*...R/
-00002b50: 0000 0052 3000 0000 525e 0000 0052 6100  ...R0...R^...Ra.
-00002b60: 0000 740b 0000 0076 616c 7565 735f 6c69  ..t....values_li
-00002b70: 7374 520c 0000 0052 0900 0000 5262 0000  stR....R....Rb..
-00002b80: 0052 3e00 0000 5225 0000 0052 3d00 0000  .R>...R%...R=...
-00002b90: 5223 0000 0052 5f00 0000 5241 0000 0052  R#...R_...RA...R
-00002ba0: 4200 0000 5272 0000 0052 4a00 0000 524b  B...Rr...RJ...RK
-00002bb0: 0000 0052 4c00 0000 524d 0000 0052 3400  ...RL...RM...R4.
-00002bc0: 0000 5200 0000 0052 0100 0000 2819 0000  ..R....R....(...
-00002bd0: 0052 1300 0000 5214 0000 0052 2900 0000  .R....R....R)...
-00002be0: 5223 0000 0074 0800 0000 7265 7370 6f6e  R#...t....respon
-00002bf0: 7365 7409 0000 0061 7274 6963 756c 6f73  set....articulos
-00002c00: 7402 0000 0077 6274 0200 0000 7773 526b  t....wbt....wsRk
-00002c10: 0000 0074 0f00 0000 7072 6563 696f 735f  ...t....precios_
-00002c20: 656d 7072 6573 6152 6600 0000 5242 0000  empresaRf...RB..
-00002c30: 0074 1100 0000 6e69 7665 6c65 735f 6172  .t....niveles_ar
-00002c40: 7469 6375 6c6f 7352 6700 0000 7401 0000  ticulosRg...t...
-00002c50: 0072 7404 0000 0061 7274 7352 7300 0000  .rt....artsRs...
-00002c60: 5274 0000 0052 2500 0000 7411 0000 0061  Rt...R%...t....a
-00002c70: 7274 6963 756c 6f73 5f70 7265 6369 6f73  rticulos_precios
-00002c80: 5271 0000 0052 4100 0000 7413 0000 006c  Rq...RA...t....l
-00002c90: 6973 7461 5f70 7265 6369 6f5f 6e6f 6d62  ista_precio_nomb
-00002ca0: 7265 523e 0000 0052 3600 0000 2800 0000  reR>...R6...(...
-00002cb0: 0028 0000 0000 7373 0000 0045 3a5c 5265  .(....ss...E:\Re
-00002cc0: 706f 7369 746f 7269 6f73 2032 3032 325c  positorios 2022\
-00002cd0: 5765 625c 646a 6d69 6372 6f73 6970 5f61  Web\djmicrosip_a
-00002ce0: 7070 735c 646a 6d69 6372 6f73 6970 5f65  pps\djmicrosip_e
-00002cf0: 7870 6f72 7461 696d 706f 7274 6170 7265  xportaimportapre
-00002d00: 6369 6f73 5c64 6a6d 6963 726f 7369 705f  cios\djmicrosip_
-00002d10: 6578 706f 7274 6169 6d70 6f72 7461 7072  exportaimportapr
-00002d20: 6563 696f 735c 7669 6577 732e 7079 7415  ecios\views.pyt.
-00002d30: 0000 0065 7870 6f72 7461 725f 7072 6563  ...exportar_prec
-00002d40: 696f 735f 7669 6577 7b01 0000 73e2 0000  ios_view{...s...
-00002d50: 0000 0215 010c 010d 010f 0106 011d 0118  ................
-00002d60: 020a 010f 010c 010f 0306 0119 0121 0119  .............!..
-00002d70: 0119 010a 0121 0119 0110 0219 0121 0119  .....!.......!..
-00002d80: 010d 070f 0106 0121 010d 011c 010d 0111  .......!........
-00002d90: 020f 0106 0121 0219 010a 010a 0219 010a  .....!..........
-00002da0: 010a 0219 010a 010a 0219 010a 010a 0219  ................
-00002db0: 010a 010d 0306 0221 0115 0115 010d 0124  .......!.......$
-00002dc0: 0106 010c 0206 011f 0121 0119 011f 0221  .........!.....!
-00002dd0: 0128 021f 0121 0125 0118 0121 010d 0106  .(...!.%...!....
-00002de0: 0109 010c 0127 0109 0106 0123 0120 0120  .....'.....#. . 
-00002df0: 0120 0126 0111 030d 0108 0121 0106 0106  . .&.......!....
-00002e00: 0106 010c 0206 011c 0221 0119 011c 0221  .........!.....!
-00002e10: 0125 021c 0121 0122 0215 0121 010d 0106  .%...!."...!....
-00002e20: 0109 010c 0127 0305 0311 020d 0104 0103  .....'..........
-00002e30: 010a 0228 1c00 0000 7410 0000 0064 6a61  ...(....t....dja
-00002e40: 6e67 6f2e 7368 6f72 7463 7574 7352 0000  ngo.shortcutsR..
-00002e50: 0000 740f 0000 0064 6a61 6e67 6f2e 7465  ..t....django.te
-00002e60: 6d70 6c61 7465 5201 0000 0074 1e00 0000  mplateR....t....
-00002e70: 646a 616e 676f 2e63 6f6e 7472 6962 2e61  django.contrib.a
-00002e80: 7574 682e 6465 636f 7261 746f 7273 5202  uth.decoratorsR.
-00002e90: 0000 0074 0600 0000 6d6f 6465 6c73 7405  ...t....modelst.
-00002ea0: 0000 0066 6f72 6d73 5204 0000 0052 0500  ...formsR....R..
-00002eb0: 0000 5206 0000 0074 0300 0000 6373 7674  ..R....t....csvt
-00002ec0: 0b00 0000 646a 616e 676f 2e68 7474 7052  ....django.httpR
-00002ed0: 0700 0000 7419 0000 0064 6a61 6e67 6f2e  ....t....django.
-00002ee0: 7669 6577 732e 6765 6e65 7269 632e 6c69  views.generic.li
-00002ef0: 7374 5208 0000 0074 0a00 0000 756e 6963  stR....t....unic
-00002f00: 6f64 6563 7376 7419 0000 006d 6963 726f  odecsvt....micro
-00002f10: 7369 705f 6170 692e 636f 6d75 6e2e 7369  sip_api.comun.si
-00002f20: 635f 6462 5209 0000 0074 0700 0000 6465  c_dbR....t....de
-00002f30: 6369 6d61 6c52 0a00 0000 5281 0000 0052  cimalR....R....R
-00002f40: 5300 0000 5210 0000 0052 1500 0000 5237  S...R....R....R7
-00002f50: 0000 0052 7500 0000 5291 0000 0028 0000  ...Ru...R....(..
-00002f60: 0000 2800 0000 0028 0000 0000 7373 0000  ..(....(....ss..
-00002f70: 0045 3a5c 5265 706f 7369 746f 7269 6f73  .E:\Repositorios
-00002f80: 2032 3032 325c 5765 625c 646a 6d69 6372   2022\Web\djmicr
-00002f90: 6f73 6970 5f61 7070 735c 646a 6d69 6372  osip_apps\djmicr
-00002fa0: 6f73 6970 5f65 7870 6f72 7461 696d 706f  osip_exportaimpo
-00002fb0: 7274 6170 7265 6369 6f73 5c64 6a6d 6963  rtaprecios\djmic
-00002fc0: 726f 7369 705f 6578 706f 7274 6169 6d70  rosip_exportaimp
-00002fd0: 6f72 7461 7072 6563 696f 735c 7669 6577  ortaprecios\view
-00002fe0: 732e 7079 7408 0000 003c 6d6f 6475 6c65  s.pyt....<module
-00002ff0: 3e02 0000 0073 2a00 0000 1001 1001 1002  >....s*.........
-00003000: 0a01 1c01 0c01 1001 1001 0c01 1001 1001  ................
-00003010: 1802 0907 0c01 0f03 0c01 0f57 0c01 0fff  ...........W....
-00003020: 0008 0c01                                ....
+00000d00: 007d 0f00 7869 0074 1000 7c0f 007c 0d00  .}..xi.t..|..|..
+00000d10: 8302 0044 5d58 007d 1000 7c08 006a 1100  ...D]X.}..|..j..
+00000d20: 640d 0064 0600 640e 007c 1000 8300 0264  d..d..d..|.....d
+00000d30: 0f00 6b02 0072 1101 506e 0000 7c08 006a  ..k..r..Pn..|..j
+00000d40: 1100 640d 0064 0600 640e 007c 1000 8300  ..d..d..d..|....
+00000d50: 027d 1100 7c10 007c 0a00 7c11 003c 7c10  .}..|..|..|..<|.
+00000d60: 0064 0700 177c 0c00 7c11 003c 71e9 0057  .d...|..|..<q..W
+00000d70: 7839 0074 1000 7c0f 007c 0d00 8302 0044  x9.t..|..|.....D
+00000d80: 5d28 007d 1000 7c08 006a 1100 640d 0064  ](.}..|..j..d..d
+00000d90: 0600 640e 007c 1000 8300 027d 1200 7c10  ..d..|.....}..|.
+00000da0: 007c 0b00 7c12 003c 7155 0157 6406 007d  .|..|..<qU.Wd..}
+00000db0: 1300 78e2 0a7c 1300 7c09 006b 0000 7268  ..x..|..|..k..rh
+00000dc0: 0c7c 1300 6407 0037 7d13 007c 0800 6a11  .|..d..7}..|..j.
+00000dd0: 0064 0d00 7c13 0064 0e00 640c 0083 0002  .d..|..d..d.....
+00000de0: 7d0e 0074 1200 7413 006a 0d00 6a14 0064  }..t..t..j..j..d
+00000df0: 1000 7c08 006a 1100 640d 007c 1300 640e  ..|..j..d..|..d.
+00000e00: 0064 0600 8300 0283 0001 8301 007d 1400  .d...........}..
+00000e10: 7c05 0073 5f05 740c 006a 0d00 6a0e 0064  |..s_.t..j..j..d
+00000e20: 0800 6409 0083 0001 6a0f 0083 0000 640a  ..d.....j.....d.
+00000e30: 006b 0200 7258 0274 1200 7415 006a 0d00  .k..rX.t..t..j..
+00000e40: 6a14 0064 0800 7c08 006a 1100 640d 007c  j..d..|..j..d..|
+00000e50: 1300 640e 0064 0c00 8300 0283 0001 8301  ..d..d..........
+00000e60: 007d 1500 7c15 0072 5802 7c15 007c 1400  .}..|..rX.|..|..
+00000e70: 5f16 007c 1400 6a17 0083 0000 0171 5802  _..|..j......qX.
+00000e80: 6e00 0074 0c00 6a0d 006a 0e00 6408 0064  n..t..j..j..d..d
+00000e90: 1100 8300 016a 0f00 8300 0064 0a00 6b02  .....j.....d..k.
+00000ea0: 0072 a702 7c08 006a 1100 640d 007c 1300  .r..|..j..d..|..
+00000eb0: 640e 0064 1200 8300 027d 1600 7c16 007c  d..d.....}..|..|
+00000ec0: 1400 5f18 007c 1400 6a17 0083 0000 016e  .._..|..j......n
+00000ed0: 0000 740c 006a 0d00 6a0e 0064 0800 6413  ..t..j..j..d..d.
+00000ee0: 0083 0001 6a0f 0083 0000 640a 006b 0200  ....j.....d..k..
+00000ef0: 72aa 0378 df00 7c0a 006a 1900 8300 0044  r..x..|..j.....D
+00000f00: 5dce 005c 0200 7d11 007d 1700 7c08 006a  ]..\..}..}..|..j
+00000f10: 1100 640d 007c 1300 640e 007c 1700 8300  ..d..|..d..|....
+00000f20: 027d 1800 741a 007c 1800 8301 0072 d502  .}..t..|.....r..
+00000f30: 741b 006a 0d00 6a0e 0064 0800 7c11 0083  t..j..j..d..|...
+00000f40: 0001 7d19 0074 1200 741c 006a 0d00 6a14  ..}..t..t..j..j.
+00000f50: 0064 1400 7c14 0064 1500 7c11 0083 0002  .d..|..d..|.....
+00000f60: 8301 007d 1a00 741d 007c 1800 6412 0083  ...}..t..|..d...
+00000f70: 0200 7d18 007c 1a00 7275 037c 1800 7c1a  ..}..|..ru.|..|.
+00000f80: 005f 1e00 7c06 007c 1a00 5f1f 007c 1a00  ._..|..|.._..|..
+00000f90: 6a17 0064 1600 642b 0083 0001 0171 a303  j..d..d+.....q..
+00000fa0: 741c 006a 0d00 6a20 0064 1400 7c14 0064  t..j..j .d..|..d
+00000fb0: 1800 7c19 0064 0400 7c06 0064 1700 7c18  ..|..d..|..d..|.
+00000fc0: 0064 1900 6406 0083 0005 0171 d502 71d5  .d..d......q..q.
+00000fd0: 0257 6e00 0074 0c00 6a0d 006a 0e00 6408  .Wn..t..j..j..d.
+00000fe0: 0064 1a00 8300 016a 0f00 8300 0064 0a00  .d.....j.....d..
+00000ff0: 6b02 0072 e304 7c08 006a 1100 640d 007c  k..r..|..j..d..|
+00001000: 1300 640e 007c 0b00 640f 0019 8300 027d  ..d..|..d......}
+00001010: 1b00 7c08 006a 1100 640d 007c 1300 640e  ..|..j..d..|..d.
+00001020: 007c 0b00 641b 0019 8300 027d 1c00 7c08  .|..d......}..|.
+00001030: 006a 1100 640d 007c 1300 640e 007c 0b00  .j..d..|..d..|..
+00001040: 641c 0019 8300 027d 1d00 7c08 006a 1100  d......}..|..j..
+00001050: 640d 007c 1300 640e 007c 0b00 641d 0019  d..|..d..|..d...
+00001060: 8300 027d 1e00 7c08 006a 1100 640d 007c  ...}..|..j..d..|
+00001070: 1300 640e 007c 0b00 641e 0019 8300 027d  ..d..|..d......}
+00001080: 1f00 7412 0074 2100 6a0d 006a 1400 6414  ..t..t!.j..j..d.
+00001090: 007c 1400 641f 007c 1b00 8300 0283 0100  .|..d..|........
+000010a0: 7d20 007c 2000 72b5 047c 1c00 7c20 005f  } .| .r..|..| ._
+000010b0: 2200 7c1d 007c 2000 5f23 007c 1e00 7c20  ".|..| ._#.|..| 
+000010c0: 005f 2400 7c1f 007c 2000 5f25 007c 2000  ._$.|..| ._%.| .
+000010d0: 6a17 0064 1600 642c 0083 0001 0171 e304  j..d..d,.....q..
+000010e0: 7421 006a 0d00 6a20 0064 1400 7c14 0064  t!.j..j .d..|..d
+000010f0: 2000 7c1c 0064 2100 7c1d 0064 2200 7c1e   .|..d!.|..d".|.
+00001100: 0064 2300 7c1f 0083 0005 016e 0000 740c  .d#.|......n..t.
+00001110: 006a 0d00 6a0e 0064 0800 6424 0083 0001  .j..j..d..d$....
+00001120: 6a0f 0083 0000 640a 006b 0200 7256 0574  j.....d..k..rV.t
+00001130: 1200 7426 006a 0d00 6a14 0064 1400 7c14  ..t&.j..j..d..|.
+00001140: 0064 2500 6426 0083 0002 8301 007d 2100  .d%.d&.......}!.
+00001150: 7c21 0072 5605 7c08 006a 1100 640d 007c  |!.rV.|..j..d..|
+00001160: 1300 640e 0064 0700 8300 027c 2100 5f27  ..d..d.....|!._'
+00001170: 007c 2100 6a17 0083 0000 0171 5605 6e00  .|!.j......qV.n.
+00001180: 0064 2700 7d03 0071 8a01 7c0e 007c 0500  .d'.}..q..|..|..
+00001190: 6a18 006b 0200 72e2 0874 0c00 6a0d 006a  j..k..r..t..j..j
+000011a0: 0e00 6408 0064 0900 8300 016a 0f00 8300  ..d..d.....j....
+000011b0: 0064 0a00 6b02 0072 db05 7412 0074 1500  .d..k..r..t..t..
+000011c0: 6a0d 006a 1400 6408 007c 0800 6a11 0064  j..j..d..|..j..d
+000011d0: 0d00 7c13 0064 0e00 640c 0083 0002 8300  ..|..d..d.......
+000011e0: 0183 0100 7d15 007c 1500 72db 057c 1500  ....}..|..r..|..
+000011f0: 7c14 005f 1600 7c14 006a 1700 8300 0001  |.._..|..j......
+00001200: 71db 056e 0000 740c 006a 0d00 6a0e 0064  q..n..t..j..j..d
+00001210: 0800 6411 0083 0001 6a0f 0083 0000 640a  ..d.....j.....d.
+00001220: 006b 0200 722a 067c 0800 6a11 0064 0d00  .k..r*.|..j..d..
+00001230: 7c13 0064 0e00 6412 0083 0002 7d16 007c  |..d..d.....}..|
+00001240: 1600 7c14 005f 1800 7c14 006a 1700 8300  ..|.._..|..j....
+00001250: 0001 6e00 0074 0c00 6a0d 006a 0e00 6408  ..n..t..j..j..d.
+00001260: 0064 1300 8300 016a 0f00 8300 0064 0a00  .d.....j.....d..
+00001270: 6b02 0072 2d07 78df 007c 0a00 6a19 0083  k..r-.x..|..j...
+00001280: 0000 445d ce00 5c02 007d 1100 7d17 007c  ..D]..\..}..}..|
+00001290: 0800 6a11 0064 0d00 7c13 0064 0e00 7c17  ..j..d..|..d..|.
+000012a0: 0083 0002 7d18 0074 1a00 7c18 0083 0100  ....}..t..|.....
+000012b0: 7258 0674 1b00 6a0d 006a 0e00 6408 007c  rX.t..j..j..d..|
+000012c0: 1100 8300 017d 1900 7412 0074 1c00 6a0d  .....}..t..t..j.
+000012d0: 006a 1400 6414 007c 1400 6415 007c 1100  .j..d..|..d..|..
+000012e0: 8300 0283 0100 7d1a 0074 1d00 7c18 0064  ......}..t..|..d
+000012f0: 1200 8302 007d 1800 7c1a 0072 f806 7c18  .....}..|..r..|.
+00001300: 007c 1a00 5f1e 007c 0600 7c1a 005f 1f00  .|.._..|..|.._..
+00001310: 7c1a 006a 1700 6416 0064 2d00 8300 0101  |..j..d..d-.....
+00001320: 7126 0774 1c00 6a0d 006a 2000 6414 007c  q&.t..j..j .d..|
+00001330: 1400 6418 007c 1900 6404 007c 0600 6417  ..d..|..d..|..d.
+00001340: 007c 1800 6419 0064 0600 8300 0501 7158  .|..d..d......qX
+00001350: 0671 5806 576e 0000 740c 006a 0d00 6a0e  .qX.Wn..t..j..j.
+00001360: 0064 0800 641a 0083 0001 6a0f 0083 0000  .d..d.....j.....
+00001370: 640a 006b 0200 7266 087c 0800 6a11 0064  d..k..rf.|..j..d
+00001380: 0d00 7c13 0064 0e00 7c0b 0064 0f00 1983  ..|..d..|..d....
+00001390: 0002 7d1b 007c 0800 6a11 0064 0d00 7c13  ..}..|..j..d..|.
+000013a0: 0064 0e00 7c0b 0064 1b00 1983 0002 7d1c  .d..|..d......}.
+000013b0: 007c 0800 6a11 0064 0d00 7c13 0064 0e00  .|..j..d..|..d..
+000013c0: 7c0b 0064 1c00 1983 0002 7d1d 007c 0800  |..d......}..|..
+000013d0: 6a11 0064 0d00 7c13 0064 0e00 7c0b 0064  j..d..|..d..|..d
+000013e0: 1d00 1983 0002 7d1e 007c 0800 6a11 0064  ......}..|..j..d
+000013f0: 0d00 7c13 0064 0e00 7c0b 0064 1e00 1983  ..|..d..|..d....
+00001400: 0002 7d1f 0074 1200 7421 006a 0d00 6a14  ..}..t..t!.j..j.
+00001410: 0064 1400 7c14 0064 1f00 7c1b 0083 0002  .d..|..d..|.....
+00001420: 8301 007d 2000 7c20 0072 3808 7c1c 007c  ...} .| .r8.|..|
+00001430: 2000 5f22 007c 1d00 7c20 005f 2300 7c1e   ._".|..| ._#.|.
+00001440: 007c 2000 5f24 007c 1f00 7c20 005f 2500  .| ._$.|..| ._%.
+00001450: 7c20 006a 1700 6416 0064 2e00 8300 0101  | .j..d..d......
+00001460: 7166 0874 2100 6a0d 006a 2000 6414 007c  qf.t!.j..j .d..|
+00001470: 1400 6420 007c 1c00 6421 007c 1d00 6422  ..d .|..d!.|..d"
+00001480: 007c 1e00 6423 007c 1f00 8300 0501 6e00  .|..d#.|......n.
+00001490: 0074 0c00 6a0d 006a 0e00 6408 0064 2400  .t..j..j..d..d$.
+000014a0: 8300 016a 0f00 8300 0064 0a00 6b02 0072  ...j.....d..k..r
+000014b0: d908 7412 0074 2600 6a0d 006a 1400 6414  ..t..t&.j..j..d.
+000014c0: 007c 1400 6425 0064 2600 8300 0283 0100  .|..d%.d&.......
+000014d0: 7d21 007c 2100 72d9 087c 0800 6a11 0064  }!.|!.r..|..j..d
+000014e0: 0d00 7c13 0064 0e00 6407 0083 0002 7c21  ..|..d..d.....|!
+000014f0: 005f 2700 7c21 006a 1700 8300 0001 71d9  ._'.|!.j......q.
+00001500: 086e 0000 6427 007d 0300 718a 017c 1400  .n..d'.}..q..|..
+00001510: 6a16 007c 0500 6b02 0072 8a01 740c 006a  j..|..k..r..t..j
+00001520: 0d00 6a0e 0064 0800 6409 0083 0001 6a0f  ..j..d..d.....j.
+00001530: 0083 0000 640a 006b 0200 725e 0974 1200  ....d..k..r^.t..
+00001540: 7415 006a 0d00 6a14 0064 0800 7c08 006a  t..j..j..d..|..j
+00001550: 1100 640d 007c 1300 640e 0064 0c00 8300  ..d..|..d..d....
+00001560: 0283 0001 8301 007d 1500 7c15 0072 5e09  .......}..|..r^.
+00001570: 7c15 007c 1400 5f16 007c 1400 6a17 0083  |..|.._..|..j...
+00001580: 0000 0171 5e09 6e00 0074 0c00 6a0d 006a  ...q^.n..t..j..j
+00001590: 0e00 6408 0064 1100 8300 016a 0f00 8300  ..d..d.....j....
+000015a0: 0064 0a00 6b02 0072 ad09 7c08 006a 1100  .d..k..r..|..j..
+000015b0: 640d 007c 1300 640e 0064 1200 8300 027d  d..|..d..d.....}
+000015c0: 1600 7c16 007c 1400 5f18 007c 1400 6a17  ..|..|.._..|..j.
+000015d0: 0083 0000 016e 0000 740c 006a 0d00 6a0e  .....n..t..j..j.
+000015e0: 0064 0800 6413 0083 0001 6a0f 0083 0000  .d..d.....j.....
+000015f0: 640a 006b 0200 72b0 0a78 df00 7c0a 006a  d..k..r..x..|..j
+00001600: 1900 8300 0044 5dce 005c 0200 7d11 007d  .....D]..\..}..}
+00001610: 1700 7c08 006a 1100 640d 007c 1300 640e  ..|..j..d..|..d.
+00001620: 007c 1700 8300 027d 1800 741a 007c 1800  .|.....}..t..|..
+00001630: 8301 0072 db09 741b 006a 0d00 6a0e 0064  ...r..t..j..j..d
+00001640: 0800 7c11 0083 0001 7d19 0074 1200 741c  ..|.....}..t..t.
+00001650: 006a 0d00 6a14 0064 1400 7c14 0064 1500  .j..j..d..|..d..
+00001660: 7c11 0083 0002 8301 007d 1a00 741d 007c  |........}..t..|
+00001670: 1800 6412 0083 0200 7d18 007c 1a00 727b  ..d.....}..|..r{
+00001680: 0a7c 1800 7c1a 005f 1e00 7c06 007c 1a00  .|..|.._..|..|..
+00001690: 5f1f 007c 1a00 6a17 0064 1600 642f 0083  _..|..j..d..d/..
+000016a0: 0001 0171 a90a 741c 006a 0d00 6a20 0064  ...q..t..j..j .d
+000016b0: 1400 7c14 0064 1800 7c19 0064 0400 7c06  ..|..d..|..d..|.
+000016c0: 0064 1700 7c18 0064 1900 6406 0083 0005  .d..|..d..d.....
+000016d0: 0171 db09 71db 0957 6e00 0074 0c00 6a0d  .q..q..Wn..t..j.
+000016e0: 006a 0e00 6408 0064 1a00 8300 016a 0f00  .j..d..d.....j..
+000016f0: 8300 0064 0a00 6b02 0072 e90b 7c08 006a  ...d..k..r..|..j
+00001700: 1100 640d 007c 1300 640e 007c 0b00 640f  ..d..|..d..|..d.
+00001710: 0019 8300 027d 1b00 7c08 006a 1100 640d  .....}..|..j..d.
+00001720: 007c 1300 640e 007c 0b00 641b 0019 8300  .|..d..|..d.....
+00001730: 027d 1c00 7c08 006a 1100 640d 007c 1300  .}..|..j..d..|..
+00001740: 640e 007c 0b00 641c 0019 8300 027d 1d00  d..|..d......}..
+00001750: 7c08 006a 1100 640d 007c 1300 640e 007c  |..j..d..|..d..|
+00001760: 0b00 641d 0019 8300 027d 1e00 7c08 006a  ..d......}..|..j
+00001770: 1100 640d 007c 1300 640e 007c 0b00 641e  ..d..|..d..|..d.
+00001780: 0019 8300 027d 1f00 7412 0074 2100 6a0d  .....}..t..t!.j.
+00001790: 006a 1400 6414 007c 1400 641f 007c 1b00  .j..d..|..d..|..
+000017a0: 8300 0283 0100 7d20 007c 2000 72bb 0b7c  ......} .| .r..|
+000017b0: 1c00 7c20 005f 2200 7c1d 007c 2000 5f23  ..| ._".|..| ._#
+000017c0: 007c 1e00 7c20 005f 2400 7c1f 007c 2000  .|..| ._$.|..| .
+000017d0: 5f25 007c 2000 6a17 0064 1600 6430 0083  _%.| .j..d..d0..
+000017e0: 0001 0171 e90b 7421 006a 0d00 6a20 0064  ...q..t!.j..j .d
+000017f0: 1400 7c14 0064 2000 7c1c 0064 2100 7c1d  ..|..d .|..d!.|.
+00001800: 0064 2200 7c1e 0064 2300 7c1f 0083 0005  .d".|..d#.|.....
+00001810: 016e 0000 740c 006a 0d00 6a0e 0064 0800  .n..t..j..j..d..
+00001820: 6424 0083 0001 6a0f 0083 0000 640a 006b  d$....j.....d..k
+00001830: 0200 725c 0c74 1200 7426 006a 0d00 6a14  ..r\.t..t&.j..j.
+00001840: 0064 1400 7c14 0064 2500 6426 0083 0002  .d..|..d%.d&....
+00001850: 8301 007d 2100 7c21 0072 5c0c 7c08 006a  ...}!.|!.r\.|..j
+00001860: 1100 640d 007c 1300 640e 0064 0700 8300  ..d..|..d..d....
+00001870: 027c 2100 5f27 007c 2100 6a17 0083 0000  .|!._'.|!.j.....
+00001880: 0171 5c0c 6e00 0064 2700 7d03 0071 8a01  .q\.n..d'.}..q..
+00001890: 718a 0157 6e00 0069 0200 7c02 0064 2800  q..Wn..i..|..d(.
+000018a0: 367c 0300 6429 0036 7d22 0074 2800 7c01  6|..d).6}".t(.|.
+000018b0: 007c 2200 642a 0074 2900 7c00 0083 0100  .|".d*.t).|.....
+000018c0: 8302 0153 2831 0000 004e 521d 0000 0074  ...S(1...NR....t
+000018d0: 0700 0000 6172 6368 6976 6f52 2300 0000  ....archivoR#...
+000018e0: 7406 0000 006d 6f6e 6564 6174 0d00 0000  t....monedat....
+000018f0: 6669 6c65 5f63 6f6e 7465 6e74 7369 0000  file_contentsi..
+00001900: 0000 6901 0000 0052 1600 0000 5218 0000  ..i....R....R...
+00001910: 0052 2200 0000 6904 0000 0069 0300 0000  .R"...i....i....
+00001920: 7404 0000 0072 6f77 7874 0400 0000 636f  t....rowxt....co
+00001930: 6c78 7407 0000 0041 6c6d 6163 656e 7402  lxt....Almacent.
+00001940: 0000 0069 6452 2100 0000 6902 0000 0052  ...idR!...i....R
+00001950: 1e00 0000 7408 0000 0061 7274 6963 756c  ....t....articul
+00001960: 6f74 1600 0000 7072 6563 696f 5f65 6d70  ot....precio_emp
+00001970: 7265 7361 5f5f 6e6f 6d62 7265 740d 0000  resa__nombret...
+00001980: 0075 7064 6174 655f 6669 656c 6473 7406  .update_fieldst.
+00001990: 0000 0070 7265 6369 6f74 0e00 0000 7072  ...preciot....pr
+000019a0: 6563 696f 5f65 6d70 7265 7361 7406 0000  ecio_empresat...
+000019b0: 006d 6172 6765 6e52 2000 0000 740c 0000  .margenR ...t...
+000019c0: 004c 6f63 616c 697a 6163 696f 6e74 0600  .Localizaciont..
+000019d0: 0000 4d61 7869 6d6f 7407 0000 0052 656f  ..Maximot....Reo
+000019e0: 7264 656e 7406 0000 004d 696e 696d 6f74  rdent....Minimot
+000019f0: 0f00 0000 616c 6d61 6365 6e5f 5f6e 6f6d  ....almacen__nom
+00001a00: 6272 6574 0c00 0000 6c6f 6361 6c69 7a61  bret....localiza
+00001a10: 6369 6f6e 7406 0000 006d 6178 696d 6f74  ciont....maximot
+00001a20: 0700 0000 7265 6f72 6465 6e74 0600 0000  ....reordent....
+00001a30: 6d69 6e69 6d6f 521f 0000 0074 0c00 0000  minimoR....t....
+00001a40: 726f 6c5f 5f65 735f 7070 616c 7401 0000  rol__es_ppalt...
+00001a50: 0053 7324 0000 0041 7274 6963 756c 6f73  .Ss$...Articulos
+00001a60: 2061 6374 7561 6c69 7a61 646f 7320 636f   actualizados co
+00001a70: 7272 6563 7461 6d65 6e74 6552 2900 0000  rrectamenteR)...
+00001a80: 7403 0000 006d 7367 5212 0000 0028 0200  t....msgR....(..
+00001a90: 0000 5242 0000 0052 3900 0000 2804 0000  ..RB...R9...(...
+00001aa0: 0052 4a00 0000 524b 0000 0052 4c00 0000  .RJ...RK...RL...
+00001ab0: 524d 0000 0028 0200 0000 5242 0000 0052  RM...(....RB...R
+00001ac0: 3900 0000 2804 0000 0052 4a00 0000 524b  9...(....RJ...RK
+00001ad0: 0000 0052 4c00 0000 524d 0000 0028 0200  ...RL...RM...(..
+00001ae0: 0000 5242 0000 0052 3900 0000 2804 0000  ..RB...R9...(...
+00001af0: 0052 4a00 0000 524b 0000 0052 4c00 0000  .RJ...RK...RL...
+00001b00: 524d 0000 0028 2a00 0000 5205 0000 0052  RM...(*...R....R
+00001b10: 3200 0000 5231 0000 0074 0500 0000 4649  2...R1...t....FI
+00001b20: 4c45 5352 3300 0000 740c 0000 0063 6c65  LESR3...t....cle
+00001b30: 616e 6564 5f64 6174 6174 0400 0000 786c  aned_datat....xl
+00001b40: 7264 740d 0000 006f 7065 6e5f 776f 726b  rdt....open_work
+00001b50: 626f 6f6b 7404 0000 0072 6561 6474 0e00  bookt....readt..
+00001b60: 0000 7368 6565 745f 6279 5f69 6e64 6578  ..sheet_by_index
+00001b70: 7405 0000 006e 726f 7773 7405 0000 006e  t....nrowst....n
+00001b80: 636f 6c73 522a 0000 0052 2b00 0000 522f  colsR*...R+...R/
+00001b90: 0000 0052 3000 0000 7405 0000 0072 616e  ...R0...t....ran
+00001ba0: 6765 740a 0000 0063 656c 6c5f 7661 6c75  get....cell_valu
+00001bb0: 6552 0900 0000 7408 0000 0041 7274 6963  eR....t....Artic
+00001bc0: 756c 6f52 2c00 0000 740e 0000 004c 696e  uloR,...t....Lin
+00001bd0: 6561 4172 7469 6375 6c6f 7352 2300 0000  eaArticulosR#...
+00001be0: 5234 0000 0052 1600 0000 7405 0000 0069  R4...R....t....i
+00001bf0: 7465 6d73 5210 0000 0074 0d00 0000 5072  temsR....t....Pr
+00001c00: 6563 696f 456d 7072 6573 6174 0e00 0000  ecioEmpresat....
+00001c10: 4172 7469 6375 6c6f 5072 6563 696f 7405  ArticuloPreciot.
+00001c20: 0000 0072 6f75 6e64 5242 0000 0052 3900  ...roundRB...R9.
+00001c30: 0000 522e 0000 0074 0d00 0000 4172 7469  ..R....t....Arti
+00001c40: 6375 6c6f 4e69 7665 6c52 4a00 0000 524b  culoNivelRJ...RK
+00001c50: 0000 0052 4c00 0000 524d 0000 0074 0d00  ...RL...RM...t..
+00001c60: 0000 4172 7469 6375 6c6f 436c 6176 6552  ..ArticuloClaveR
+00001c70: 2500 0000 5200 0000 0052 0100 0000 2823  %...R....R....(#
+00001c80: 0000 0052 1300 0000 5214 0000 0052 2900  ...R....R....R).
+00001c90: 0000 5250 0000 0052 3800 0000 5223 0000  ..RP...R8...R#..
+00001ca0: 0052 3900 0000 7404 0000 0062 6f6f 6b74  .R9...t....bookt
+00001cb0: 0500 0000 7368 6565 7474 0800 0000 6e75  ....sheett....nu
+00001cc0: 6d5f 726f 7773 7412 0000 0070 7265 6369  m_rowst....preci
+00001cd0: 6f73 5f70 6f73 6963 696f 6e65 7374 1200  os_posicionest..
+00001ce0: 0000 6e69 7665 6c65 735f 706f 7369 6369  ..niveles_posici
+00001cf0: 6f6e 6573 7413 0000 006d 6172 6765 6e65  onest....margene
+00001d00: 735f 706f 7369 6369 6f6e 6573 5258 0000  s_posicionesRX..
+00001d10: 0074 0c00 0000 6c69 6e65 615f 6e6f 6d62  .t....linea_nomb
+00001d20: 7265 7403 0000 006e 756d 7408 0000 0063  ret....numt....c
+00001d30: 7572 725f 636f 6c74 0d00 0000 7072 6563  urr_colt....prec
+00001d40: 696f 5f6e 6f6d 6272 6574 1000 0000 636f  io_nombret....co
+00001d50: 6c5f 6e69 7665 6c5f 6e6f 6d62 7265 7408  l_nivel_nombret.
+00001d60: 0000 0063 7572 725f 726f 7752 3f00 0000  ...curr_rowR?...
+00001d70: 7409 0000 006c 696e 6561 5f61 7274 5226  t....linea_artR&
+00001d80: 0000 0074 0800 0000 706f 7369 6369 6f6e  ...t....posicion
+00001d90: 5242 0000 0052 4300 0000 740f 0000 0061  RB...RC...t....a
+00001da0: 7274 6963 756c 6f5f 7072 6563 696f 7407  rticulo_preciot.
+00001db0: 0000 0061 6c6d 6163 656e 524a 0000 0052  ...almacenRJ...R
+00001dc0: 4b00 0000 524c 0000 0052 4d00 0000 740e  K...RL...RM...t.
+00001dd0: 0000 006e 6976 656c 5f61 7274 6963 756c  ...nivel_articul
+00001de0: 6f74 0e00 0000 6172 7469 6375 6c6f 5f63  ot....articulo_c
+00001df0: 6c61 7665 5236 0000 0028 0000 0000 2800  laveR6...(....(.
+00001e00: 0000 0073 7300 0000 453a 5c52 6570 6f73  ...ss...E:\Repos
+00001e10: 6974 6f72 696f 7320 3230 3232 5c57 6562  itorios 2022\Web
+00001e20: 5c64 6a6d 6963 726f 7369 705f 6170 7073  \djmicrosip_apps
+00001e30: 5c64 6a6d 6963 726f 7369 705f 6578 706f  \djmicrosip_expo
+00001e40: 7274 6169 6d70 6f72 7461 7072 6563 696f  rtaimportaprecio
+00001e50: 735c 646a 6d69 6372 6f73 6970 5f65 7870  s\djmicrosip_exp
+00001e60: 6f72 7461 696d 706f 7274 6170 7265 6369  ortaimportapreci
+00001e70: 6f73 5c76 6965 7773 2e70 7974 1500 0000  os\views.pyt....
+00001e80: 696d 706f 7274 6172 5f70 7265 6369 6f73  importar_precios
+00001e90: 5f76 6965 7773 0000 0073 7e01 0000 0002  _views...s~.....
+00001ea0: 1b01 0601 0c01 0d01 0d01 0d02 1801 0f01  ................
+00001eb0: 0d02 0601 0601 0601 0901 0601 2101 0902  ............!...
+00001ec0: 0602 1601 1e01 0401 1802 0a01 1205 1601  ................
+00001ed0: 1801 0e02 0601 0f01 0a02 1803 2d03 0603  ............-...
+00001ee0: 2101 2d02 0601 0901 1002 2101 1801 0901  !.-.......!.....
+00001ef0: 0d03 2101 1901 1801 0c01 1502 2101 0f01  ..!.........!...
+00001f00: 0601 0901 0901 1302 0c01 0601 0601 0601  ................
+00001f10: 0601 1102 2101 1c01 1c01 1c01 1c01 1c02  ....!...........
+00001f20: 2101 0601 0901 0901 0901 0901 1302 0c01  !...............
+00001f30: 0601 0601 0601 0601 0a06 2101 2101 0603  ..........!.!...
+00001f40: 1b01 1002 0903 0f04 2101 2d02 0601 0901  ........!.-.....
+00001f50: 1002 2101 1801 0901 0d03 2101 1901 1802  ..!.......!.....
+00001f60: 0c01 1502 2101 0f01 0601 0901 0901 1302  ....!...........
+00001f70: 0c01 0601 0601 0601 0601 1102 2101 1c01  ............!...
+00001f80: 1c01 1c01 1c01 1c02 2101 0601 0901 0901  ........!.......
+00001f90: 0901 0901 1302 0c01 0601 0601 0601 0601  ................
+00001fa0: 0a04 2101 2101 0602 1b01 1002 0905 0f02  ..!.!...........
+00001fb0: 2101 2d02 0601 0901 1002 2101 1801 0901  !.-.......!.....
+00001fc0: 0d03 2101 1901 1801 0c01 1502 2101 0f01  ..!.........!...
+00001fd0: 0601 0901 0901 1302 0c01 0601 0601 0601  ................
+00001fe0: 0601 1102 2101 1c01 1c01 1c01 1c01 1c02  ....!...........
+00001ff0: 2101 0601 0901 0901 0901 0901 1302 0c01  !...............
+00002000: 0601 0601 0601 0601 0a04 2101 2101 0602  ..........!.!...
+00002010: 1b01 1002 1003 0301 0701 0a02 7336 0000  ............s6..
+00002020: 0064 6a6d 6963 726f 7369 705f 6578 706f  .djmicrosip_expo
+00002030: 7274 6169 6d70 6f72 7461 7072 6563 696f  rtaimportaprecio
+00002040: 732f 6578 706f 7274 6172 5f70 7265 6369  s/exportar_preci
+00002050: 6f73 2e68 746d 6c63 0200 0000 1900 0000  os.htmlc........
+00002060: 0700 0000 4300 0000 73bd 0800 0074 0000  ....C...s....t..
+00002070: 7c00 006a 0100 700f 0064 0000 8301 007d  |..j..p..d.....}
+00002080: 0200 7c02 006a 0300 8300 0072 9708 7c02  ..|..j.....r..|.
+00002090: 006a 0400 6401 0019 7d03 0074 0500 6402  .j..d...}..t..d.
+000020a0: 0064 0300 8300 017d 0400 7c03 0072 7800  .d.....}..|..rx.
+000020b0: 6404 007c 0300 6a06 006a 0700 6405 0064  d..|..j..j..d..d
+000020c0: 0600 8302 0016 7c04 0064 0700 3c74 0800  ......|..d..<t..
+000020d0: 6a09 006a 0a00 6401 007c 0300 8300 017d  j..j..d..|.....}
+000020e0: 0500 6e19 0064 0800 7c04 0064 0700 3c74  ..n..d..|..d..<t
+000020f0: 0800 6a09 006a 0b00 8300 007d 0500 740c  ..j..j.....}..t.
+00002100: 006a 0d00 8300 007d 0600 7c06 006a 0e00  .j.....}..|..j..
+00002110: 6409 0083 0100 7d07 0064 0a00 7d08 007c  d.....}..d..}..|
+00002120: 0700 6a0f 0064 0b00 8301 006a 1000 640b  ..j..d.....j..d.
+00002130: 0064 0c00 8302 0001 7411 006a 0900 6a12  .d......t..j..j.
+00002140: 0064 0d00 640e 0083 0001 6a13 0083 0000  .d..d.....j.....
+00002150: 640f 006b 0200 7272 017c 0700 6a0f 0064  d..k..rr.|..j..d
+00002160: 0b00 8301 006a 1000 6410 0064 1100 8302  .....j..d..d....
+00002170: 0001 7c07 006a 0f00 640b 0083 0100 6a10  ..|..j..d.....j.
+00002180: 0064 0a00 6412 0083 0200 017c 0800 6410  .d..d......|..d.
+00002190: 0017 7d08 0074 1100 6a09 006a 1200 640d  ..}..t..j..j..d.
+000021a0: 0064 1300 8300 016a 1300 8300 0064 0f00  .d.....j.....d..
+000021b0: 6b02 0072 d201 7c07 006a 0f00 640b 0083  k..r..|..j..d...
+000021c0: 0100 6a10 0064 1400 6415 0083 0200 017c  ..j..d..d......|
+000021d0: 0800 6410 0017 7d08 0071 d201 6e60 007c  ..d...}..q..n`.|
+000021e0: 0700 6a0f 0064 0b00 8301 006a 1000 6410  ..j..d.....j..d.
+000021f0: 0064 1200 8302 0001 7411 006a 0900 6a12  .d......t..j..j.
+00002200: 0064 0d00 6413 0083 0001 6a13 0083 0000  .d..d.....j.....
+00002210: 640f 006b 0200 72d2 017c 0700 6a0f 0064  d..k..r..|..j..d
+00002220: 0b00 8301 006a 1000 640a 0064 1500 8302  .....j..d..d....
+00002230: 0001 7c08 0064 1000 177d 0800 6e00 0074  ..|..d...}..n..t
+00002240: 1400 6a09 006a 0b00 8300 007d 0900 6900  ..j..j.....}..i.
+00002250: 007d 0a00 7411 006a 0900 6a12 0064 0d00  .}..t..j..j..d..
+00002260: 6416 0083 0001 6a13 0083 0000 640f 006b  d.....j.....d..k
+00002270: 0200 724f 0278 4400 7c09 0044 5d39 007d  ..rO.xD.|..D]9.}
+00002280: 0b00 7c07 006a 0f00 640b 0083 0100 6a10  ..|..j..d.....j.
+00002290: 007c 0800 7c0b 006a 0600 8302 0001 7c08  .|..|..j......|.
+000022a0: 007c 0a00 7c0b 006a 0600 3c7c 0800 6410  .|..|..j..<|..d.
+000022b0: 0037 7d08 0071 0f02 576e 0000 7415 006a  .7}..q..Wn..t..j
+000022c0: 0900 6a0b 0083 0000 7d0c 0069 0000 7d0d  ..j.....}..i..}.
+000022d0: 0074 1100 6a09 006a 1200 640d 0064 1700  .t..j..j..d..d..
+000022e0: 8300 016a 1300 8300 0064 0f00 6b02 0072  ...j.....d..k..r
+000022f0: 6903 7c07 006a 0f00 640b 0083 0100 6a10  i.|..j..d.....j.
+00002300: 007c 0800 6418 0083 0200 017c 0800 7c0d  .|..d......|..|.
+00002310: 0064 1800 3c7c 0800 6410 0037 7d08 007c  .d..<|..d..7}..|
+00002320: 0700 6a0f 0064 0b00 8301 006a 1000 7c08  ..j..d.....j..|.
+00002330: 0064 1900 8302 0001 7c08 007c 0d00 6419  .d......|..|..d.
+00002340: 003c 7c08 0064 1000 377d 0800 7c07 006a  .<|..d..7}..|..j
+00002350: 0f00 640b 0083 0100 6a10 007c 0800 641a  ..d.....j..|..d.
+00002360: 0083 0200 017c 0800 7c0d 0064 1a00 3c7c  .....|..|..d..<|
+00002370: 0800 6410 0037 7d08 007c 0700 6a0f 0064  ..d..7}..|..j..d
+00002380: 0b00 8301 006a 1000 7c08 0064 1b00 8302  .....j..|..d....
+00002390: 0001 7c08 007c 0d00 641b 003c 7c08 0064  ..|..|..d..<|..d
+000023a0: 1000 377d 0800 7c07 006a 0f00 640b 0083  ..7}..|..j..d...
+000023b0: 0100 6a10 007c 0800 641c 0083 0200 017c  ..j..|..d......|
+000023c0: 0800 7c0d 0064 1c00 3c7c 0800 6410 0037  ..|..d..<|..d..7
+000023d0: 7d08 006e 0000 6410 007d 0e00 7411 006a  }..n..d..}..t..j
+000023e0: 0900 6a12 0064 0d00 6417 0083 0001 6a13  ..j..d..d.....j.
+000023f0: 0083 0000 640f 006b 0200 727a 067c 0500  ....d..k..rz.|..
+00002400: 6a16 0064 1d00 641e 0074 1700 8301 017d  j..d..d..t.....}
+00002410: 0f00 7415 006a 0900 6a0a 0064 1f00 7c0f  ..t..j..j..d..|.
+00002420: 0083 0001 7d0c 0078 c904 7c0c 0044 5db2  ....}..x..|..D].
+00002430: 027d 1000 7418 0074 1900 6a09 006a 0a00  .}..t..t..j..j..
+00002440: 6420 007c 1000 6a1a 0064 2100 6422 0083  d .|..j..d!.d"..
+00002450: 0002 8301 007d 1100 7c11 0072 fd03 7c11  .....}..|..r..|.
+00002460: 006a 1b00 7d12 006e 0600 6423 007d 1200  .j..}..n..d#.}..
+00002470: 7c07 006a 0f00 7c0e 0083 0100 6a10 0064  |..j..|.....j..d
+00002480: 0b00 7c10 006a 1a00 6a1c 0083 0200 0174  ..|..j..j......t
+00002490: 1100 6a09 006a 1200 640d 0064 0e00 8300  ..j..j..d..d....
+000024a0: 016a 1300 8300 0064 0f00 6b02 0072 c404  .j.....d..k..r..
+000024b0: 7c07 006a 0f00 7c0e 0083 0100 6a10 0064  |..j..|.....j..d
+000024c0: 1000 7c12 0083 0200 017c 0700 6a0f 007c  ..|......|..j..|
+000024d0: 0e00 8301 006a 1000 640a 007c 1000 6a1a  .....j..d..|..j.
+000024e0: 006a 0600 8302 0001 7411 006a 0900 6a12  .j......t..j..j.
+000024f0: 0064 0d00 6413 0083 0001 6a13 0083 0000  .d..d.....j.....
+00002500: 640f 006b 0200 7229 057c 0700 6a0f 007c  d..k..r).|..j..|
+00002510: 0e00 8301 006a 1000 6414 007c 1000 6a1a  .....j..d..|..j.
+00002520: 006a 1d00 6a06 0083 0200 0171 2905 6e65  .j..j......q).ne
+00002530: 007c 0700 6a0f 007c 0e00 8301 006a 1000  .|..j..|.....j..
+00002540: 6410 007c 1000 6a1a 006a 0600 8302 0001  d..|..j..j......
+00002550: 7411 006a 0900 6a12 0064 0d00 6413 0083  t..j..j..d..d...
+00002560: 0001 6a13 0083 0000 640f 006b 0200 7229  ..j.....d..k..r)
+00002570: 057c 0700 6a0f 007c 0e00 8301 006a 1000  .|..j..|.....j..
+00002580: 640a 007c 1000 6a1a 006a 1d00 6a06 0083  d..|..j..j..j...
+00002590: 0200 016e 0000 741e 006a 0900 6a0a 0064  ...n..t..j..j..d
+000025a0: 2000 7c10 006a 1a00 8300 017d 1300 7411   .|..j.....}..t.
+000025b0: 006a 0900 6a12 0064 0d00 6416 0083 0001  .j..j..d..d.....
+000025c0: 6a13 0083 0000 640f 006b 0200 72b1 0578  j.....d..k..r..x
+000025d0: 4c00 7c13 0044 5d41 007d 1400 7c14 0072  L.|..D]A.}..|..r
+000025e0: 6905 7c14 006a 1f00 7d15 007c 1400 6a20  i.|..j..}..|..j 
+000025f0: 006a 0600 7d16 007c 0700 6a0f 007c 0e00  .j..}..|..j..|..
+00002600: 8301 006a 1000 7c0a 007c 1600 197c 1500  ...j..|..|...|..
+00002610: 8302 0001 7169 0571 6905 576e 0000 7c10  ....qi.qi.Wn..|.
+00002620: 006a 1a00 7269 067c 1000 7269 067c 0700  .j..ri.|..ri.|..
+00002630: 6a0f 007c 0e00 8301 006a 1000 7c0d 0064  j..|.....j..|..d
+00002640: 1800 197c 1000 6a21 006a 0600 8302 0001  ...|..j!.j......
+00002650: 7c07 006a 0f00 7c0e 0083 0100 6a10 007c  |..j..|.....j..|
+00002660: 0d00 6419 0019 7c10 006a 2200 8302 0001  ..d...|..j".....
+00002670: 7c07 006a 0f00 7c0e 0083 0100 6a10 007c  |..j..|.....j..|
+00002680: 0d00 641a 0019 7c10 006a 2300 8302 0001  ..d...|..j#.....
+00002690: 7c07 006a 0f00 7c0e 0083 0100 6a10 007c  |..j..|.....j..|
+000026a0: 0d00 641b 0019 7c10 006a 2400 8302 0001  ..d...|..j$.....
+000026b0: 7c07 006a 0f00 7c0e 0083 0100 6a10 007c  |..j..|.....j..|
+000026c0: 0d00 641c 0019 7c10 006a 2500 8302 0001  ..d...|..j%.....
+000026d0: 7169 066e 0000 7c0e 0064 1000 377d 0e00  qi.n..|..d..7}..
+000026e0: 71c1 0357 6e0c 0278 0902 7c05 0044 5d01  q..Wn..x..|..D].
+000026f0: 027d 1700 7c17 006a 1d00 4748 7418 0074  .}..|..j..GHt..t
+00002700: 1900 6a09 006a 0a00 6420 007c 1700 6421  ..j..j..d .|..d!
+00002710: 0064 2200 8300 0283 0100 7d11 007c 1700  .d".......}..|..
+00002720: 7281 0664 0b00 7d15 007c 1100 72ce 067c  r..d..}..|..r..|
+00002730: 1100 6a1b 007d 1200 6e06 0064 2300 7d12  ..j..}..n..d#.}.
+00002740: 007c 0700 6a0f 007c 0e00 8301 006a 1000  .|..j..|.....j..
+00002750: 640b 007c 1700 6a1c 0083 0200 0174 1100  d..|..j......t..
+00002760: 6a09 006a 1200 640d 0064 0e00 8300 016a  j..j..d..d.....j
+00002770: 1300 8300 0064 0f00 6b02 0072 8c07 7c07  .....d..k..r..|.
+00002780: 006a 0f00 7c0e 0083 0100 6a10 0064 1000  .j..|.....j..d..
+00002790: 7c12 0083 0200 017c 0700 6a0f 007c 0e00  |......|..j..|..
+000027a0: 8301 006a 1000 640a 007c 1700 6a06 0083  ...j..d..|..j...
+000027b0: 0200 0174 1100 6a09 006a 1200 640d 0064  ...t..j..j..d..d
+000027c0: 1300 8300 016a 1300 8300 0064 0f00 6b02  .....j.....d..k.
+000027d0: 0072 eb07 7c07 006a 0f00 7c0e 0083 0100  .r..|..j..|.....
+000027e0: 6a10 0064 1400 7c17 006a 1d00 6a06 0083  j..d..|..j..j...
+000027f0: 0200 0171 eb07 6e5f 007c 0700 6a0f 007c  ...q..n_.|..j..|
+00002800: 0e00 8301 006a 1000 6410 007c 1700 6a06  .....j..d..|..j.
+00002810: 0083 0200 0174 1100 6a09 006a 1200 640d  .....t..j..j..d.
+00002820: 0064 1300 8300 016a 1300 8300 0064 0f00  .d.....j.....d..
+00002830: 6b02 0072 eb07 7c07 006a 0f00 7c0e 0083  k..r..|..j..|...
+00002840: 0100 6a10 0064 0a00 7c17 006a 1d00 6a06  ..j..d..|..j..j.
+00002850: 0083 0200 016e 0000 741e 006a 0900 6a0a  .....n..t..j..j.
+00002860: 0064 2000 7c17 0083 0001 7d13 0074 1100  .d .|.....}..t..
+00002870: 6a09 006a 1200 640d 0064 1600 8300 016a  j..j..d..d.....j
+00002880: 1300 8300 0064 0f00 6b02 0072 7008 784c  .....d..k..rp.xL
+00002890: 007c 1300 445d 4100 7d14 007c 1400 7228  .|..D]A.}..|..r(
+000028a0: 087c 1400 6a1f 007d 1500 7c14 006a 2000  .|..j..}..|..j .
+000028b0: 6a06 007d 1600 7c07 006a 0f00 7c0e 0083  j..}..|..j..|...
+000028c0: 0100 6a10 007c 0a00 7c16 0019 7c15 0083  ..j..|..|...|...
+000028d0: 0200 0171 2808 7128 0857 6e00 007c 0c00  ...q(.q(.Wn..|..
+000028e0: 4748 7c0e 0064 1000 377d 0e00 7181 0671  GH|..d..7}..q..q
+000028f0: 8106 577c 0600 6a26 007c 0400 8301 0001  ..W|..j&.|......
+00002900: 7c04 0053 6901 007c 0200 6424 0036 7d18  |..Si..|..d$.6}.
+00002910: 0074 2700 7c01 007c 1800 6425 0074 2800  .t'.|..|..d%.t(.
+00002920: 7c00 0083 0100 8302 0153 2826 0000 004e  |........S(&...N
+00002930: 5223 0000 0074 0800 0000 6d69 6d65 7479  R#...t....mimety
+00002940: 7065 7314 0000 0061 7070 6c69 6361 7469  pes....applicati
+00002950: 6f6e 2f6d 732d 6578 6365 6c73 1b00 0000  on/ms-excels....
+00002960: 6174 7461 6368 6d65 6e74 3b20 6669 6c65  attachment; file
+00002970: 6e61 6d65 3d25 732e 786c 7374 0100 0000  name=%s.xlst....
+00002980: 2074 0100 0000 5f73 1300 0000 436f 6e74   t...._s....Cont
+00002990: 656e 742d 4469 7370 6f73 6974 696f 6e73  ent-Dispositions
+000029a0: 1d00 0000 6174 7461 6368 6d65 6e74 3b20  ....attachment; 
+000029b0: 6669 6c65 6e61 6d65 3d61 7274 732e 786c  filename=arts.xl
+000029c0: 7374 0700 0000 5072 6563 696f 7369 0200  st....Preciosi..
+000029d0: 0000 6900 0000 0074 0200 0000 4964 5216  ..i....t....IdR.
+000029e0: 0000 0052 1f00 0000 5222 0000 0069 0100  ...R....R"...i..
+000029f0: 0000 7405 0000 0043 6c61 7665 525b 0000  ..t....ClaveR[..
+00002a00: 0052 1800 0000 6903 0000 0074 0500 0000  .R....i....t....
+00002a10: 4c69 6e65 6152 1e00 0000 5220 0000 0052  LineaR....R ...R
+00002a20: 3d00 0000 5245 0000 0052 4600 0000 5247  =...RE...RF...RG
+00002a30: 0000 0052 4800 0000 523e 0000 0074 0400  ...RH...R>...t..
+00002a40: 0000 666c 6174 7410 0000 0061 7274 6963  ..flatt....artic
+00002a50: 756c 6f5f 5f69 645f 5f69 6e52 3f00 0000  ulo__id__inR?...
+00002a60: 524e 0000 0052 4f00 0000 521d 0000 0052  RN...RO...R....R
+00002a70: 2900 0000 5212 0000 0028 2900 0000 5204  )...R....()...R.
+00002a80: 0000 0052 3200 0000 5231 0000 0052 3300  ...R2...R1...R3.
+00002a90: 0000 5252 0000 0052 0700 0000 5216 0000  ..RR...R....R...
+00002aa0: 0074 0700 0000 7265 706c 6163 6552 5b00  .t....replaceR[.
+00002ab0: 0000 522b 0000 0052 2c00 0000 7403 0000  ..R+...R,...t...
+00002ac0: 0061 6c6c 7404 0000 0078 6c77 7474 0800  .allt....xlwtt..
+00002ad0: 0000 576f 726b 626f 6f6b 7409 0000 0061  ..Workbookt....a
+00002ae0: 6464 5f73 6865 6574 7403 0000 0072 6f77  dd_sheett....row
+00002af0: 7405 0000 0077 7269 7465 522a 0000 0052  t....writeR*...R
+00002b00: 2f00 0000 5230 0000 0052 5e00 0000 5261  /...R0...R^...Ra
+00002b10: 0000 0074 0b00 0000 7661 6c75 6573 5f6c  ...t....values_l
+00002b20: 6973 7452 0c00 0000 5209 0000 0052 6200  istR....R....Rb.
+00002b30: 0000 523f 0000 0052 2500 0000 523e 0000  ..R?...R%...R>..
+00002b40: 0052 2300 0000 525f 0000 0052 4200 0000  .R#...R_...RB...
+00002b50: 5243 0000 0052 7200 0000 524a 0000 0052  RC...Rr...RJ...R
+00002b60: 4b00 0000 524c 0000 0052 4d00 0000 5234  K...RL...RM...R4
+00002b70: 0000 0052 0000 0000 5201 0000 0028 1900  ...R....R....(..
+00002b80: 0000 5213 0000 0052 1400 0000 5229 0000  ..R....R....R)..
+00002b90: 0052 2300 0000 7408 0000 0072 6573 706f  .R#...t....respo
+00002ba0: 6e73 6574 0900 0000 6172 7469 6375 6c6f  nset....articulo
+00002bb0: 7374 0200 0000 7762 7402 0000 0077 7352  st....wbt....wsR
+00002bc0: 6b00 0000 740f 0000 0070 7265 6369 6f73  k...t....precios
+00002bd0: 5f65 6d70 7265 7361 5266 0000 0052 4300  _empresaRf...RC.
+00002be0: 0000 7411 0000 006e 6976 656c 6573 5f61  ..t....niveles_a
+00002bf0: 7274 6963 756c 6f73 5267 0000 0074 0100  rticulosRg...t..
+00002c00: 0000 7274 0400 0000 6172 7473 5273 0000  ..rt....artsRs..
+00002c10: 0052 7400 0000 5225 0000 0074 1100 0000  .Rt...R%...t....
+00002c20: 6172 7469 6375 6c6f 735f 7072 6563 696f  articulos_precio
+00002c30: 7352 7100 0000 5242 0000 0074 1300 0000  sRq...RB...t....
+00002c40: 6c69 7374 615f 7072 6563 696f 5f6e 6f6d  lista_precio_nom
+00002c50: 6272 6552 3f00 0000 5236 0000 0028 0000  breR?...R6...(..
+00002c60: 0000 2800 0000 0073 7300 0000 453a 5c52  ..(....ss...E:\R
+00002c70: 6570 6f73 6974 6f72 696f 7320 3230 3232  epositorios 2022
+00002c80: 5c57 6562 5c64 6a6d 6963 726f 7369 705f  \Web\djmicrosip_
+00002c90: 6170 7073 5c64 6a6d 6963 726f 7369 705f  apps\djmicrosip_
+00002ca0: 6578 706f 7274 6169 6d70 6f72 7461 7072  exportaimportapr
+00002cb0: 6563 696f 735c 646a 6d69 6372 6f73 6970  ecios\djmicrosip
+00002cc0: 5f65 7870 6f72 7461 696d 706f 7274 6170  _exportaimportap
+00002cd0: 7265 6369 6f73 5c76 6965 7773 2e70 7974  recios\views.pyt
+00002ce0: 1500 0000 6578 706f 7274 6172 5f70 7265  ....exportar_pre
+00002cf0: 6369 6f73 5f76 6965 7782 0100 0073 e200  cios_view....s..
+00002d00: 0000 0002 1501 0c01 0d01 0f01 0601 1d01  ................
+00002d10: 1802 0a01 0f01 0c01 0f03 0601 1901 2101  ..............!.
+00002d20: 1901 1901 0a01 2101 1901 1002 1901 2101  ......!.......!.
+00002d30: 1901 0d07 0f01 0601 2101 0d01 1c01 0d01  ........!.......
+00002d40: 1102 0f01 0601 2102 1901 0a01 0a02 1901  ......!.........
+00002d50: 0a01 0a02 1901 0a01 0a02 1901 0a01 0a02  ................
+00002d60: 1901 0a01 0d03 0602 2101 1501 1501 0d01  ........!.......
+00002d70: 2401 0601 0c02 0601 1f01 2101 1901 1f02  $.........!.....
+00002d80: 2101 2802 1f01 2101 2501 1801 2101 0d01  !.(...!.%...!...
+00002d90: 0601 0901 0c01 2701 0901 0601 2301 2001  ......'.....#. .
+00002da0: 2001 2001 2601 1103 0d01 0801 2101 0601   . .&.......!...
+00002db0: 0601 0601 0c02 0601 1c02 2101 1901 1c02  ..........!.....
+00002dc0: 2101 2502 1c01 2101 2202 1501 2101 0d01  !.%...!."...!...
+00002dd0: 0601 0901 0c01 2703 0503 1102 0d01 0401  ......'.........
+00002de0: 0301 0a02 281c 0000 0074 1000 0000 646a  ....(....t....dj
+00002df0: 616e 676f 2e73 686f 7274 6375 7473 5200  ango.shortcutsR.
+00002e00: 0000 0074 0f00 0000 646a 616e 676f 2e74  ...t....django.t
+00002e10: 656d 706c 6174 6552 0100 0000 741e 0000  emplateR....t...
+00002e20: 0064 6a61 6e67 6f2e 636f 6e74 7269 622e  .django.contrib.
+00002e30: 6175 7468 2e64 6563 6f72 6174 6f72 7352  auth.decoratorsR
+00002e40: 0200 0000 7406 0000 006d 6f64 656c 7374  ....t....modelst
+00002e50: 0500 0000 666f 726d 7352 0400 0000 5205  ....formsR....R.
+00002e60: 0000 0052 0600 0000 7403 0000 0063 7376  ...R....t....csv
+00002e70: 740b 0000 0064 6a61 6e67 6f2e 6874 7470  t....django.http
+00002e80: 5207 0000 0074 1900 0000 646a 616e 676f  R....t....django
+00002e90: 2e76 6965 7773 2e67 656e 6572 6963 2e6c  .views.generic.l
+00002ea0: 6973 7452 0800 0000 740a 0000 0075 6e69  istR....t....uni
+00002eb0: 636f 6465 6373 7674 1900 0000 6d69 6372  codecsvt....micr
+00002ec0: 6f73 6970 5f61 7069 2e63 6f6d 756e 2e73  osip_api.comun.s
+00002ed0: 6963 5f64 6252 0900 0000 7407 0000 0064  ic_dbR....t....d
+00002ee0: 6563 696d 616c 520a 0000 0052 8100 0000  ecimalR....R....
+00002ef0: 5253 0000 0052 1000 0000 5215 0000 0052  RS...R....R....R
+00002f00: 3700 0000 5275 0000 0052 9100 0000 2800  7...Ru...R....(.
+00002f10: 0000 0028 0000 0000 2800 0000 0073 7300  ...(....(....ss.
+00002f20: 0000 453a 5c52 6570 6f73 6974 6f72 696f  ..E:\Repositorio
+00002f30: 7320 3230 3232 5c57 6562 5c64 6a6d 6963  s 2022\Web\djmic
+00002f40: 726f 7369 705f 6170 7073 5c64 6a6d 6963  rosip_apps\djmic
+00002f50: 726f 7369 705f 6578 706f 7274 6169 6d70  rosip_exportaimp
+00002f60: 6f72 7461 7072 6563 696f 735c 646a 6d69  ortaprecios\djmi
+00002f70: 6372 6f73 6970 5f65 7870 6f72 7461 696d  crosip_exportaim
+00002f80: 706f 7274 6170 7265 6369 6f73 5c76 6965  portaprecios\vie
+00002f90: 7773 2e70 7974 0800 0000 3c6d 6f64 756c  ws.pyt....<modul
+00002fa0: 653e 0200 0000 732a 0000 0010 0110 0110  e>....s*........
+00002fb0: 020a 011c 010c 0110 0110 010c 0110 0110  ................
+00002fc0: 0118 0209 070c 010f 030c 010f 570c 010f  ............W...
+00002fd0: ff00 0f0c 01                             .....
```

### Comparing `djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios.egg-info/PKG-INFO` & `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: djmicrosip-exportaimportaprecios
-Version: 1.8.3
+Version: 1.8.4
 Summary: djmicrosip_exportaimportaprecios
 Home-page: UNKNOWN
 Author: Servicios de Ingenieria Computacional
 Author-email: desarrollo@siccomputacion.com
 License: BSD License
 Description: README
 Platform: UNKNOWN
```

### Comparing `djmicrosip_exportaimportaprecios-1.8.3/djmicrosip_exportaimportaprecios.egg-info/SOURCES.txt` & `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.3/MANIFEST.in` & `djmicrosip_exportaimportaprecios-1.8.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.3/PKG-INFO` & `djmicrosip_exportaimportaprecios-1.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: djmicrosip_exportaimportaprecios
-Version: 1.8.3
+Version: 1.8.4
 Summary: djmicrosip_exportaimportaprecios
 Home-page: UNKNOWN
 Author: Servicios de Ingenieria Computacional
 Author-email: desarrollo@siccomputacion.com
 License: BSD License
 Description: README
 Platform: UNKNOWN
```

### Comparing `djmicrosip_exportaimportaprecios-1.8.3/setup.py` & `djmicrosip_exportaimportaprecios-1.8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
 
     username = '__token__',
     password = 'pypi-AgEIcHlwaS5vcmcCJDMzNzQ3N2Y4LWJjOWYtNDNlOS1hOGM2LWMwODNhNmYxYjc5MgACKlszLCI0YzkyNTJkMC05YWFmLTQ5ZTYtYmU5ZS01YWYxOWZlZGI5ZDUiXQAABiCXuYtQg-eQ-vWH2gycMSobsCgYaxWgr_CUsJBbWdUQtQ',
     name = 'djmicrosip_exportaimportaprecios',
-    version = '1.8.3',
+    version = '1.8.4',
     packages = find_packages(),
     include_package_data = True,
     license = 'BSD License', # example license
     description = 'djmicrosip_exportaimportaprecios',
     long_description = 'README',
     url = '',
     author = 'Servicios de Ingenieria Computacional',
```

