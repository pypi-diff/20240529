# Comparing `tmp/djmicrosip_exportaimportaprecios-1.8.4.tar.gz` & `tmp/djmicrosip_exportaimportaprecios-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\djmicrosip_exportaimportaprecios-1.8.4.tar", last modified: Wed May 29 01:31:50 2024, max compression
+gzip compressed data, was "dist\djmicrosip_exportaimportaprecios-1.8.5.tar", last modified: Wed May 29 02:15:35 2024, max compression
```

## Comparing `djmicrosip_exportaimportaprecios-1.8.4.tar` & `djmicrosip_exportaimportaprecios-1.8.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/
-drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/
--rw-rw-rw-   0        0        0      453 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/config.pyc
--rw-rw-rw-   0        0        0     3283 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/forms.pyc
--rw-rw-rw-   0        0        0      542 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/models.pyc
-drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/static/
-drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/static/djmicrosip_exportaimportaprecios/
-drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/static/djmicrosip_exportaimportaprecios/js/
--rw-rw-rw-   0        0        0       94 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/static/djmicrosip_exportaimportaprecios/js/core.js
-drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/
-drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/
--rw-rw-rw-   0        0        0     1292 2020-10-22 18:31:02.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/base.html
--rw-rw-rw-   0        0        0      650 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/exportar_precios.html
--rw-rw-rw-   0        0        0     1035 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/importar_precios.html
--rw-rw-rw-   0        0        0      416 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/index.html
--rw-rw-rw-   0        0        0     1425 2024-04-06 01:31:51.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/preferencias.html
--rw-rw-rw-   0        0        0      599 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/urls.pyc
--rw-rw-rw-   0        0        0    12245 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/views.pyc
--rw-rw-rw-   0        0        0        0 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/__init__.py
--rw-rw-rw-   0        0        0      205 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/__init__.pyc
-drwxrwxrwx   0        0        0        0 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/
--rw-rw-rw-   0        0        0        1 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      769 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1191 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       33 2024-05-29 01:31:48.000000 djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      585 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/MANIFEST.in
--rw-rw-rw-   0        0        0      769 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/PKG-INFO
--rw-rw-rw-   0        0        0      295 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/README.rst
--rw-rw-rw-   0        0        0       44 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.4/requirements.txt
--rw-rw-rw-   0        0        0       86 2024-05-29 01:31:50.000000 djmicrosip_exportaimportaprecios-1.8.4/setup.cfg
--rw-rw-rw-   0        0        0     1816 2024-05-29 01:31:17.000000 djmicrosip_exportaimportaprecios-1.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/
+drwxrwxrwx   0        0        0        0 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/
+-rw-rw-rw-   0        0        0      453 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/config.pyc
+-rw-rw-rw-   0        0        0     3291 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/forms.pyc
+-rw-rw-rw-   0        0        0      542 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/models.pyc
+drwxrwxrwx   0        0        0        0 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/static/
+drwxrwxrwx   0        0        0        0 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/static/djmicrosip_exportaimportaprecios/
+drwxrwxrwx   0        0        0        0 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/static/djmicrosip_exportaimportaprecios/js/
+-rw-rw-rw-   0        0        0       94 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/static/djmicrosip_exportaimportaprecios/js/core.js
+drwxrwxrwx   0        0        0        0 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/templates/
+drwxrwxrwx   0        0        0        0 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/
+-rw-rw-rw-   0        0        0     1292 2020-10-22 18:31:02.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/base.html
+-rw-rw-rw-   0        0        0      650 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/exportar_precios.html
+-rw-rw-rw-   0        0        0     1035 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/importar_precios.html
+-rw-rw-rw-   0        0        0      416 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/index.html
+-rw-rw-rw-   0        0        0     1425 2024-04-06 01:31:51.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/preferencias.html
+-rw-rw-rw-   0        0        0      599 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/urls.pyc
+-rw-rw-rw-   0        0        0    12245 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/views.pyc
+-rw-rw-rw-   0        0        0        0 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/__init__.py
+-rw-rw-rw-   0        0        0      205 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/__init__.pyc
+drwxrwxrwx   0        0        0        0 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      769 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1191 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       33 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      585 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      769 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.5/README.rst
+-rw-rw-rw-   0        0        0       44 2019-09-13 21:10:10.000000 djmicrosip_exportaimportaprecios-1.8.5/requirements.txt
+-rw-rw-rw-   0        0        0       86 2024-05-29 02:15:35.000000 djmicrosip_exportaimportaprecios-1.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     1816 2024-05-29 02:15:29.000000 djmicrosip_exportaimportaprecios-1.8.5/setup.py
```

### Comparing `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/forms.pyc` & `djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/forms.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a bfa5 1066 6300 0000 0000 0000  .......fc.......
+00000000: 03f3 0d0a e78d 5666 6300 0000 0000 0000  ......Vfc.......
 00000010: 0003 0000 0040 0000 0073 8700 0000 6400  .....@...s....d.
 00000020: 0064 0100 6c00 006d 0100 5a01 0001 6402  .d..l..m..Z...d.
 00000030: 0064 0300 6c02 0054 6400 0064 0400 6c03  .d..l..Td..d..l.
 00000040: 005a 0300 6405 0084 0000 5a04 0064 0600  .Z..d.....Z..d..
 00000050: 6501 006a 0500 6601 0064 0700 8400 0083  e..j..f..d......
 00000060: 0000 595a 0600 6408 0067 0100 5a07 0064  ..YZ..d..g..Z..d
 00000070: 0900 6501 006a 0500 6601 0064 0a00 8400  ..e..j..f..d....
@@ -125,82 +125,82 @@
 000007c0: 8300 015a 0500 6502 006a 0300 6400 0065  ...Z..e..j..d..e
 000007d0: 0400 8300 015a 0600 6502 006a 0300 6400  .....Z..e..j..d.
 000007e0: 0065 0400 8300 015a 0700 6502 006a 0300  .e.....Z..e..j..
 000007f0: 6400 0065 0400 8300 015a 0800 6502 006a  d..e.....Z..e..j
 00000800: 0300 6400 0065 0400 8300 015a 0900 6401  ..d..e.....Z..d.
 00000810: 0084 0000 5a0a 0052 5328 0200 0000 520e  ....Z..RS(....R.
 00000820: 0000 0063 0100 0000 0800 0000 0300 0000  ...c............
-00000830: 4f00 0000 73cb 0000 0064 0100 7d03 0064  O...s....d..}..d
+00000830: 4f00 0000 73d1 0000 0064 0100 7d03 0064  O...s....d..}..d
 00000840: 0100 7d04 0064 0100 7d05 0064 0100 7d06  ..}..d..}..d..}.
-00000850: 007c 0000 6a00 0064 0200 1972 2e00 6403  .|..j..d...r..d.
-00000860: 007d 0300 6e00 007c 0000 6a00 0064 0400  .}..n..|..j..d..
-00000870: 1972 4400 6403 007d 0400 6e00 007c 0000  .rD.d..}..n..|..
-00000880: 6a00 0064 0500 1972 5a00 6403 007d 0500  j..d...rZ.d..}..
-00000890: 6e00 007c 0000 6a00 0064 0600 1972 7000  n..|..j..d...rp.
-000008a0: 6403 007d 0600 6e00 007c 0000 6a00 0064  d..}..n..|..j..d
-000008b0: 0700 1972 8600 6403 007d 0700 6e00 0074  ...r..d..}..n..t
-000008c0: 0100 6408 007c 0300 8302 0001 7401 0064  ..d..|......t..d
-000008d0: 0900 7c04 0083 0200 0174 0100 640a 007c  ..|......t..d..|
-000008e0: 0500 8302 0001 7401 0064 0b00 7c06 0083  ......t..d..|...
-000008f0: 0200 0174 0100 640c 007c 0700 8302 0001  ...t..d..|......
-00000900: 6400 0053 280d 0000 004e 6900 0000 0052  d..S(....Ni....R
-00000910: 1600 0000 6901 0000 0074 0700 0000 7072  ....i....t....pr
-00000920: 6563 696f 7374 0500 0000 636c 6176 6574  eciost....clavet
-00000930: 0b00 0000 6465 7363 7269 7063 696f 6e74  ....descripciont
-00000940: 0d00 0000 7075 6e74 6f5f 7265 6f72 6465  ....punto_reorde
-00000950: 6e74 1a00 0000 5349 435f 4578 706f 7274  nt....SIC_Export
-00000960: 6172 496d 706f 7274 6172 5f4c 696e 6561  arImportar_Linea
-00000970: 741c 0000 0053 4943 5f45 7870 6f72 7461  t....SIC_Exporta
-00000980: 7249 6d70 6f72 7461 725f 5072 6563 696f  rImportar_Precio
-00000990: 7374 1a00 0000 5349 435f 4578 706f 7274  st....SIC_Export
-000009a0: 6172 496d 706f 7274 6172 5f43 6c61 7665  arImportar_Clave
-000009b0: 7420 0000 0053 4943 5f45 7870 6f72 7461  t ...SIC_Exporta
-000009c0: 7249 6d70 6f72 7461 725f 4465 7363 7269  rImportar_Descri
-000009d0: 7063 696f 6e74 2200 0000 5349 435f 4578  pciont"...SIC_Ex
-000009e0: 706f 7274 6172 496d 706f 7274 6172 5f50  portarImportar_P
-000009f0: 756e 746f 7352 656f 7264 656e 2802 0000  untosReorden(...
-00000a00: 0052 1900 0000 520b 0000 0028 0800 0000  .R....R....(....
-00000a10: 5220 0000 0074 0400 0000 6172 6773 7406  R ...t....argst.
-00000a20: 0000 006b 7761 7267 7352 1600 0000 5227  ...kwargsR....R'
-00000a30: 0000 0052 2800 0000 5229 0000 0052 2a00  ...R(...R)...R*.
-00000a40: 0000 2800 0000 0028 0000 0000 7373 0000  ..(....(....ss..
-00000a50: 0045 3a5c 5265 706f 7369 746f 7269 6f73  .E:\Repositorios
-00000a60: 2032 3032 325c 5765 625c 646a 6d69 6372   2022\Web\djmicr
-00000a70: 6f73 6970 5f61 7070 735c 646a 6d69 6372  osip_apps\djmicr
-00000a80: 6f73 6970 5f65 7870 6f72 7461 696d 706f  osip_exportaimpo
-00000a90: 7274 6170 7265 6369 6f73 5c64 6a6d 6963  rtaprecios\djmic
-00000aa0: 726f 7369 705f 6578 706f 7274 6169 6d70  rosip_exportaimp
-00000ab0: 6f72 7461 7072 6563 696f 735c 666f 726d  ortaprecios\form
-00000ac0: 732e 7079 5207 0000 0025 0000 0073 2600  s.pyR....%...s&.
-00000ad0: 0000 0001 0601 0601 0601 0601 0d01 0901  ................
-00000ae0: 0d01 0901 0d01 0901 0d01 0901 0d01 0903  ................
-00000af0: 0d01 0d01 0d01 0d01 280b 0000 0052 0f00  ........(....R..
-00000b00: 0000 5210 0000 0052 0000 0000 740c 0000  ..R....R....t...
-00000b10: 0042 6f6f 6c65 616e 4669 656c 6452 1500  .BooleanFieldR..
-00000b20: 0000 5216 0000 0052 2700 0000 5228 0000  ..R....R'...R(..
-00000b30: 0052 2900 0000 522a 0000 0052 0700 0000  .R)...R*...R....
-00000b40: 2800 0000 0028 0000 0000 2800 0000 0073  (....(....(....s
-00000b50: 7300 0000 453a 5c52 6570 6f73 6974 6f72  s...E:\Repositor
-00000b60: 696f 7320 3230 3232 5c57 6562 5c64 6a6d  ios 2022\Web\djm
-00000b70: 6963 726f 7369 705f 6170 7073 5c64 6a6d  icrosip_apps\djm
-00000b80: 6963 726f 7369 705f 6578 706f 7274 6169  icrosip_exportai
-00000b90: 6d70 6f72 7461 7072 6563 696f 735c 646a  mportaprecios\dj
-00000ba0: 6d69 6372 6f73 6970 5f65 7870 6f72 7461  microsip_exporta
-00000bb0: 696d 706f 7274 6170 7265 6369 6f73 5c66  importaprecios\f
-00000bc0: 6f72 6d73 2e70 7952 2600 0000 1d00 0000  orms.pyR&.......
-00000bd0: 730c 0000 0006 0112 0112 0112 0112 0112  s...............
-00000be0: 0328 0a00 0000 7406 0000 0064 6a61 6e67  .(....t....djang
-00000bf0: 6f52 0000 0000 7406 0000 006d 6f64 656c  oR....t....model
-00000c00: 7352 1a00 0000 520b 0000 0074 0400 0000  sR....R....t....
-00000c10: 466f 726d 520c 0000 0052 1e00 0000 5217  FormR....R....R.
-00000c20: 0000 0052 2600 0000 2800 0000 0028 0000  ...R&...(....(..
-00000c30: 0000 2800 0000 0073 7300 0000 453a 5c52  ..(....ss...E:\R
-00000c40: 6570 6f73 6974 6f72 696f 7320 3230 3232  epositorios 2022
-00000c50: 5c57 6562 5c64 6a6d 6963 726f 7369 705f  \Web\djmicrosip_
-00000c60: 6170 7073 5c64 6a6d 6963 726f 7369 705f  apps\djmicrosip_
-00000c70: 6578 706f 7274 6169 6d70 6f72 7461 7072  exportaimportapr
-00000c80: 6563 696f 735c 646a 6d69 6372 6f73 6970  ecios\djmicrosip
-00000c90: 5f65 7870 6f72 7461 696d 706f 7274 6170  _exportaimportap
-00000ca0: 7265 6369 6f73 5c66 6f72 6d73 2e70 7974  recios\forms.pyt
-00000cb0: 0800 0000 3c6d 6f64 756c 653e 0200 0000  ....<module>....
-00000cc0: 730e 0000 0010 010a 010c 0409 0519 0309  s...............
-00000cd0: 0119 0c                                  ...
+00000850: 0064 0100 7d07 007c 0000 6a00 0064 0200  .d..}..|..j..d..
+00000860: 1972 3400 6403 007d 0300 6e00 007c 0000  .r4.d..}..n..|..
+00000870: 6a00 0064 0400 1972 4a00 6403 007d 0400  j..d...rJ.d..}..
+00000880: 6e00 007c 0000 6a00 0064 0500 1972 6000  n..|..j..d...r`.
+00000890: 6403 007d 0500 6e00 007c 0000 6a00 0064  d..}..n..|..j..d
+000008a0: 0600 1972 7600 6403 007d 0600 6e00 007c  ...rv.d..}..n..|
+000008b0: 0000 6a00 0064 0700 1972 8c00 6403 007d  ..j..d...r..d..}
+000008c0: 0700 6e00 0074 0100 6408 007c 0300 8302  ..n..t..d..|....
+000008d0: 0001 7401 0064 0900 7c04 0083 0200 0174  ..t..d..|......t
+000008e0: 0100 640a 007c 0500 8302 0001 7401 0064  ..d..|......t..d
+000008f0: 0b00 7c06 0083 0200 0174 0100 640c 007c  ..|......t..d..|
+00000900: 0700 8302 0001 6400 0053 280d 0000 004e  ......d..S(....N
+00000910: 6900 0000 0052 1600 0000 6901 0000 0074  i....R....i....t
+00000920: 0700 0000 7072 6563 696f 7374 0500 0000  ....preciost....
+00000930: 636c 6176 6574 0b00 0000 6465 7363 7269  clavet....descri
+00000940: 7063 696f 6e74 0d00 0000 7075 6e74 6f5f  pciont....punto_
+00000950: 7265 6f72 6465 6e74 1a00 0000 5349 435f  reordent....SIC_
+00000960: 4578 706f 7274 6172 496d 706f 7274 6172  ExportarImportar
+00000970: 5f4c 696e 6561 741c 0000 0053 4943 5f45  _Lineat....SIC_E
+00000980: 7870 6f72 7461 7249 6d70 6f72 7461 725f  xportarImportar_
+00000990: 5072 6563 696f 7374 1a00 0000 5349 435f  Preciost....SIC_
+000009a0: 4578 706f 7274 6172 496d 706f 7274 6172  ExportarImportar
+000009b0: 5f43 6c61 7665 7420 0000 0053 4943 5f45  _Clavet ...SIC_E
+000009c0: 7870 6f72 7461 7249 6d70 6f72 7461 725f  xportarImportar_
+000009d0: 4465 7363 7269 7063 696f 6e74 2200 0000  Descripciont"...
+000009e0: 5349 435f 4578 706f 7274 6172 496d 706f  SIC_ExportarImpo
+000009f0: 7274 6172 5f50 756e 746f 7352 656f 7264  rtar_PuntosReord
+00000a00: 656e 2802 0000 0052 1900 0000 520b 0000  en(....R....R...
+00000a10: 0028 0800 0000 5220 0000 0074 0400 0000  .(....R ...t....
+00000a20: 6172 6773 7406 0000 006b 7761 7267 7352  argst....kwargsR
+00000a30: 1600 0000 5227 0000 0052 2800 0000 5229  ....R'...R(...R)
+00000a40: 0000 0052 2a00 0000 2800 0000 0028 0000  ...R*...(....(..
+00000a50: 0000 7373 0000 0045 3a5c 5265 706f 7369  ..ss...E:\Reposi
+00000a60: 746f 7269 6f73 2032 3032 325c 5765 625c  torios 2022\Web\
+00000a70: 646a 6d69 6372 6f73 6970 5f61 7070 735c  djmicrosip_apps\
+00000a80: 646a 6d69 6372 6f73 6970 5f65 7870 6f72  djmicrosip_expor
+00000a90: 7461 696d 706f 7274 6170 7265 6369 6f73  taimportaprecios
+00000aa0: 5c64 6a6d 6963 726f 7369 705f 6578 706f  \djmicrosip_expo
+00000ab0: 7274 6169 6d70 6f72 7461 7072 6563 696f  rtaimportaprecio
+00000ac0: 735c 666f 726d 732e 7079 5207 0000 0025  s\forms.pyR....%
+00000ad0: 0000 0073 2800 0000 0001 0601 0601 0601  ...s(...........
+00000ae0: 0601 0601 0d01 0901 0d01 0901 0d01 0901  ................
+00000af0: 0d01 0901 0d01 0903 0d01 0d01 0d01 0d01  ................
+00000b00: 280b 0000 0052 0f00 0000 5210 0000 0052  (....R....R....R
+00000b10: 0000 0000 740c 0000 0042 6f6f 6c65 616e  ....t....Boolean
+00000b20: 4669 656c 6452 1500 0000 5216 0000 0052  FieldR....R....R
+00000b30: 2700 0000 5228 0000 0052 2900 0000 522a  '...R(...R)...R*
+00000b40: 0000 0052 0700 0000 2800 0000 0028 0000  ...R....(....(..
+00000b50: 0000 2800 0000 0073 7300 0000 453a 5c52  ..(....ss...E:\R
+00000b60: 6570 6f73 6974 6f72 696f 7320 3230 3232  epositorios 2022
+00000b70: 5c57 6562 5c64 6a6d 6963 726f 7369 705f  \Web\djmicrosip_
+00000b80: 6170 7073 5c64 6a6d 6963 726f 7369 705f  apps\djmicrosip_
+00000b90: 6578 706f 7274 6169 6d70 6f72 7461 7072  exportaimportapr
+00000ba0: 6563 696f 735c 646a 6d69 6372 6f73 6970  ecios\djmicrosip
+00000bb0: 5f65 7870 6f72 7461 696d 706f 7274 6170  _exportaimportap
+00000bc0: 7265 6369 6f73 5c66 6f72 6d73 2e70 7952  recios\forms.pyR
+00000bd0: 2600 0000 1d00 0000 730c 0000 0006 0112  &.......s.......
+00000be0: 0112 0112 0112 0112 0328 0a00 0000 7406  .........(....t.
+00000bf0: 0000 0064 6a61 6e67 6f52 0000 0000 7406  ...djangoR....t.
+00000c00: 0000 006d 6f64 656c 7352 1a00 0000 520b  ...modelsR....R.
+00000c10: 0000 0074 0400 0000 466f 726d 520c 0000  ...t....FormR...
+00000c20: 0052 1e00 0000 5217 0000 0052 2600 0000  .R....R....R&...
+00000c30: 2800 0000 0028 0000 0000 2800 0000 0073  (....(....(....s
+00000c40: 7300 0000 453a 5c52 6570 6f73 6974 6f72  s...E:\Repositor
+00000c50: 696f 7320 3230 3232 5c57 6562 5c64 6a6d  ios 2022\Web\djm
+00000c60: 6963 726f 7369 705f 6170 7073 5c64 6a6d  icrosip_apps\djm
+00000c70: 6963 726f 7369 705f 6578 706f 7274 6169  icrosip_exportai
+00000c80: 6d70 6f72 7461 7072 6563 696f 735c 646a  mportaprecios\dj
+00000c90: 6d69 6372 6f73 6970 5f65 7870 6f72 7461  microsip_exporta
+00000ca0: 696d 706f 7274 6170 7265 6369 6f73 5c66  importaprecios\f
+00000cb0: 6f72 6d73 2e70 7974 0800 0000 3c6d 6f64  orms.pyt....<mod
+00000cc0: 756c 653e 0200 0000 730e 0000 0010 010a  ule>....s.......
+00000cd0: 010c 0409 0519 0309 0119 0c              ...........
```

### Comparing `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/models.pyc` & `djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/models.pyc`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/base.html` & `djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/base.html`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/exportar_precios.html` & `djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/exportar_precios.html`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/importar_precios.html` & `djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/importar_precios.html`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/preferencias.html` & `djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/templates/djmicrosip_exportaimportaprecios/preferencias.html`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/urls.pyc` & `djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/urls.pyc`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios/views.pyc` & `djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios/views.pyc`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/PKG-INFO` & `djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: djmicrosip-exportaimportaprecios
-Version: 1.8.4
+Version: 1.8.5
 Summary: djmicrosip_exportaimportaprecios
 Home-page: UNKNOWN
 Author: Servicios de Ingenieria Computacional
 Author-email: desarrollo@siccomputacion.com
 License: BSD License
 Description: README
 Platform: UNKNOWN
```

### Comparing `djmicrosip_exportaimportaprecios-1.8.4/djmicrosip_exportaimportaprecios.egg-info/SOURCES.txt` & `djmicrosip_exportaimportaprecios-1.8.5/djmicrosip_exportaimportaprecios.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.4/MANIFEST.in` & `djmicrosip_exportaimportaprecios-1.8.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `djmicrosip_exportaimportaprecios-1.8.4/PKG-INFO` & `djmicrosip_exportaimportaprecios-1.8.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: djmicrosip_exportaimportaprecios
-Version: 1.8.4
+Version: 1.8.5
 Summary: djmicrosip_exportaimportaprecios
 Home-page: UNKNOWN
 Author: Servicios de Ingenieria Computacional
 Author-email: desarrollo@siccomputacion.com
 License: BSD License
 Description: README
 Platform: UNKNOWN
```

### Comparing `djmicrosip_exportaimportaprecios-1.8.4/setup.py` & `djmicrosip_exportaimportaprecios-1.8.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
 
     username = '__token__',
     password = 'pypi-AgEIcHlwaS5vcmcCJDMzNzQ3N2Y4LWJjOWYtNDNlOS1hOGM2LWMwODNhNmYxYjc5MgACKlszLCI0YzkyNTJkMC05YWFmLTQ5ZTYtYmU5ZS01YWYxOWZlZGI5ZDUiXQAABiCXuYtQg-eQ-vWH2gycMSobsCgYaxWgr_CUsJBbWdUQtQ',
     name = 'djmicrosip_exportaimportaprecios',
-    version = '1.8.4',
+    version = '1.8.5',
     packages = find_packages(),
     include_package_data = True,
     license = 'BSD License', # example license
     description = 'djmicrosip_exportaimportaprecios',
     long_description = 'README',
     url = '',
     author = 'Servicios de Ingenieria Computacional',
```

