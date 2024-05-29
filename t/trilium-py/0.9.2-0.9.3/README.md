# Comparing `tmp/trilium_py-0.9.2-py3-none-any.whl.zip` & `tmp/trilium_py-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 35722 bytes, number of entries: 15
+Zip file size: 35730 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      141 b- defN 24-Apr-22 06:33 trilium_py/__init__.py
--rw-r--r--  2.0 unx    46923 b- defN 24-May-20 09:13 trilium_py/client.py
+-rw-r--r--  2.0 unx    46954 b- defN 24-May-29 01:40 trilium_py/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-25 07:17 trilium_py/utils/__init__.py
 -rw-r--r--  2.0 unx     2290 b- defN 24-Apr-22 06:32 trilium_py/utils/html_util.py
--rw-r--r--  2.0 unx     1221 b- defN 24-May-20 09:10 trilium_py/utils/image_util.py
+-rw-r--r--  2.0 unx     1221 b- defN 24-May-20 09:24 trilium_py/utils/image_util.py
 -rw-r--r--  2.0 unx     9328 b- defN 24-Apr-22 06:33 trilium_py/utils/markdown_math.py
 -rw-r--r--  2.0 unx     3909 b- defN 24-Apr-22 06:33 trilium_py/utils/note_util.py
 -rw-r--r--  2.0 unx      681 b- defN 24-Apr-22 06:33 trilium_py/utils/param_util.py
 -rw-r--r--  2.0 unx      208 b- defN 24-Apr-22 06:33 trilium_py/utils/time_util.py
 -rw-r--r--  2.0 unx      486 b- defN 24-Apr-22 06:33 trilium_py/utils/url_util.py
--rwxrwx---  2.0 unx    35184 b- defN 24-May-20 09:15 trilium_py-0.9.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    16639 b- defN 24-May-20 09:15 trilium_py-0.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-20 09:15 trilium_py-0.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-20 09:15 trilium_py-0.9.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1249 b- defN 24-May-20 09:15 trilium_py-0.9.2.dist-info/RECORD
-15 files, 118362 bytes uncompressed, 33648 bytes compressed:  71.6%
+-rwxrwx---  2.0 unx    35184 b- defN 24-May-29 01:43 trilium_py-0.9.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    16639 b- defN 24-May-29 01:43 trilium_py-0.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-29 01:43 trilium_py-0.9.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-29 01:43 trilium_py-0.9.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1249 b- defN 24-May-29 01:43 trilium_py-0.9.3.dist-info/RECORD
+15 files, 118393 bytes uncompressed, 33656 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: trilium_py/utils/time_util.py
 Comment: 
 
 Filename: trilium_py/utils/url_util.py
 Comment: 
 
-Filename: trilium_py-0.9.2.dist-info/LICENSE.txt
+Filename: trilium_py-0.9.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: trilium_py-0.9.2.dist-info/METADATA
+Filename: trilium_py-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: trilium_py-0.9.2.dist-info/WHEEL
+Filename: trilium_py-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: trilium_py-0.9.2.dist-info/top_level.txt
+Filename: trilium_py-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: trilium_py-0.9.2.dist-info/RECORD
+Filename: trilium_py-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trilium_py/client.py

```diff
@@ -867,15 +867,16 @@
                 html = reconstructMath(
                     markdown2.markdown(
                         no_latex_part,
                         extras=['fenced-code-blocks', 'strike', 'tables', 'task_list'],
                     ),
                     list(
                         map(
-                            lambda x: x.replace("<", " \lt ").replace(">", " \gt "), latex_code_part
+                            lambda x: x.replace("<", " \\lt ").replace(">", " \\gt "),
+                            latex_code_part,
                         )
                     ),
                 )
         note_id = ''
 
         # detect images
         # https://github.com/Nriver/trilium-py/issues/36
```

## Comparing `trilium_py-0.9.2.dist-info/LICENSE.txt` & `trilium_py-0.9.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `trilium_py-0.9.2.dist-info/METADATA` & `trilium_py-0.9.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trilium-py
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python client for ETAPI of Trilium Note. With some extra features powered by Python :)
 Home-page: https://github.com/nriver/trilium-py
 Author: Nriver
 Author-email: 
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues
 Project-URL: Funding, https://github.com/nriver/trilium-py
 Project-URL: Say Thanks!, https://github.com/nriver/trilium-py
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trilium-py Version: 0.9.2 Summary: Python client
+Metadata-Version: 2.1 Name: trilium-py Version: 0.9.3 Summary: Python client
 for ETAPI of Trilium Note. With some extra features powered by Python :) Home-
 page: https://github.com/nriver/trilium-py Author: Nriver Author-email:
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues Project-
 URL: Funding, https://github.com/nriver/trilium-py Project-URL: Say Thanks!,
 https://github.com/nriver/trilium-py Project-URL: Source, https://github.com/
 nriver/trilium-py/ Keywords: trilium,etapi,api client Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
```

## Comparing `trilium_py-0.9.2.dist-info/RECORD` & `trilium_py-0.9.3.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 trilium_py/__init__.py,sha256=uSMH49RW2MFU_LVKKKm6lt3xOBsDWo0cb8--nMcNlgY,141
-trilium_py/client.py,sha256=KwExWmLGQYqTrPxxxrxyM9DoxZSPmdi8cbCSbmqg5oY,46923
+trilium_py/client.py,sha256=jN-I3wwxzCRwviG40DA7xCCVZ-MduaZyfm5Uo3qkGQ4,46954
 trilium_py/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 trilium_py/utils/html_util.py,sha256=OuFEt5bHiiNYtBDX_ABPXudDoHpid97GmicFQwuidNE,2290
 trilium_py/utils/image_util.py,sha256=9B02tEtR8LFtOiNNetrqOXU8_aWSPRioqsXlJ_7N20w,1221
 trilium_py/utils/markdown_math.py,sha256=sAiR_5YaCE_EOeQ4vZBjoc5t0Z1n_5EQ4JmJ1TAweCY,9328
 trilium_py/utils/note_util.py,sha256=jSavmxnV8Fn-DKoFeNLFVxtkrn176wQF_pbiPJCdEu8,3909
 trilium_py/utils/param_util.py,sha256=jlnKrCKBtaN1wfQgxDTvGmuMM0p7vk809vpaLgK0dXg,681
 trilium_py/utils/time_util.py,sha256=DIFQmCKZ_wL5lCdeTMJZAtFolZw_dic6NKZ8CCJTa1A,208
 trilium_py/utils/url_util.py,sha256=1eHmHlti4CwsN-hjqfennxiohkrUX0jtuX3UleTD120,486
-trilium_py-0.9.2.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
-trilium_py-0.9.2.dist-info/METADATA,sha256=8SNqYK1LTdExcld8SE54wJFx8LG77U-mk9li8V2kI_E,16639
-trilium_py-0.9.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-trilium_py-0.9.2.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
-trilium_py-0.9.2.dist-info/RECORD,,
+trilium_py-0.9.3.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
+trilium_py-0.9.3.dist-info/METADATA,sha256=_fPVZjK0AxgYSOpRosHnNfFTlQrfM7wA0COZBY_PctU,16639
+trilium_py-0.9.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+trilium_py-0.9.3.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
+trilium_py-0.9.3.dist-info/RECORD,,
```

