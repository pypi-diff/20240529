# Comparing `tmp/oahspe-0.0.6.tar.gz` & `tmp/oahspe-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oahspe-0.0.6.tar", last modified: Tue May 28 12:12:18 2024, max compression
+gzip compressed data, was "oahspe-0.0.7.tar", last modified: Tue May 28 15:10:46 2024, max compression
```

## Comparing `oahspe-0.0.6.tar` & `oahspe-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 12:12:18.699352 oahspe-0.0.6/
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1066 2024-05-26 13:20:10.000000 oahspe-0.0.6/LICENSE.txt
--rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-28 12:12:18.699352 oahspe-0.0.6/PKG-INFO
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        9 2024-05-27 17:45:26.000000 oahspe-0.0.6/README.md
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 12:12:18.695352 oahspe-0.0.6/oahspe/
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3841 2024-05-26 16:33:26.000000 oahspe-0.0.6/oahspe/SSL.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    13322 2024-05-28 12:11:32.000000 oahspe-0.0.6/oahspe/crypt.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8461 2024-05-26 15:35:40.000000 oahspe-0.0.6/oahspe/execute.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1925 2024-05-26 13:20:10.000000 oahspe-0.0.6/oahspe/host.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8115 2024-05-28 11:17:16.000000 oahspe-0.0.6/oahspe/tool.py
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 12:12:18.699352 oahspe-0.0.6/oahspe.egg-info/
--rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-28 12:12:18.000000 oahspe-0.0.6/oahspe.egg-info/PKG-INFO
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      228 2024-05-28 12:12:18.000000 oahspe-0.0.6/oahspe.egg-info/SOURCES.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        1 2024-05-28 12:12:18.000000 oahspe-0.0.6/oahspe.egg-info/dependency_links.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        7 2024-05-28 12:12:18.000000 oahspe-0.0.6/oahspe.egg-info/top_level.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)       38 2024-05-28 12:12:18.699352 oahspe-0.0.6/setup.cfg
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      640 2024-05-28 12:12:04.000000 oahspe-0.0.6/setup.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 15:10:46.608739 oahspe-0.0.7/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1066 2024-05-26 13:20:10.000000 oahspe-0.0.7/LICENSE.txt
+-rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-28 15:10:46.608739 oahspe-0.0.7/PKG-INFO
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        9 2024-05-28 12:40:50.000000 oahspe-0.0.7/README.md
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 15:10:46.608739 oahspe-0.0.7/oahspe/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3841 2024-05-26 16:33:26.000000 oahspe-0.0.7/oahspe/SSL.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    13322 2024-05-28 12:11:32.000000 oahspe-0.0.7/oahspe/crypt.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8461 2024-05-26 15:35:40.000000 oahspe-0.0.7/oahspe/execute.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1925 2024-05-26 13:20:10.000000 oahspe-0.0.7/oahspe/host.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8558 2024-05-28 15:06:17.000000 oahspe-0.0.7/oahspe/tool.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 15:10:46.608739 oahspe-0.0.7/oahspe.egg-info/
+-rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-28 15:10:46.000000 oahspe-0.0.7/oahspe.egg-info/PKG-INFO
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      228 2024-05-28 15:10:46.000000 oahspe-0.0.7/oahspe.egg-info/SOURCES.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        1 2024-05-28 15:10:46.000000 oahspe-0.0.7/oahspe.egg-info/dependency_links.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        7 2024-05-28 15:10:46.000000 oahspe-0.0.7/oahspe.egg-info/top_level.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)       38 2024-05-28 15:10:46.608739 oahspe-0.0.7/setup.cfg
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      640 2024-05-28 15:10:16.000000 oahspe-0.0.7/setup.py
```

### Comparing `oahspe-0.0.6/LICENSE.txt` & `oahspe-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.6/PKG-INFO` & `oahspe-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oahspe
-Version: 0.0.6
+Version: 0.0.7
 Summary: Cloud DevOps
 Home-page: https://github.com/quangproo/oahspe
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: quangproo
 Author-email: contact@quang.pro
 License: MIT
 Keywords: oahspe
```

### Comparing `oahspe-0.0.6/oahspe/SSL.py` & `oahspe-0.0.7/oahspe/SSL.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.6/oahspe/crypt.py` & `oahspe-0.0.7/oahspe/crypt.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.6/oahspe/execute.py` & `oahspe-0.0.7/oahspe/execute.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.6/oahspe/host.py` & `oahspe-0.0.7/oahspe/host.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.6/oahspe/tool.py` & `oahspe-0.0.7/oahspe/tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 # coding: utf-8
 
 from pytz import timezone
 from datetime import datetime
 import os, hashlib, base64
 
 
+def tmp_write(content):
+  tmp = gen_uuid()
+  tmp = f'tmp/{tmp}'
+  if isinstance(content, str):
+    mode = 'w'
+  else:
+    content = to_byte(content)
+    mode = 'wb'
+  with open(tmp, mode) as f:
+    f.write(content)
+  return tmp
+
+
 def checksum(content, chunk=100*1024*1024):
   from binascii import unhexlify
   content = to_byte(content)
   if len(content) <= chunk:
     return hashlib.md5(content).hexdigest()
   else:
     content = split_size(content, chunk)
@@ -46,45 +59,53 @@
       data = str(data)
     elif hasattr(data, '__dict__'):
       data = json_dump(data.__dict__)
   data = data.encode('UTF-8')
   return data
 
 
-def encrypt_aes(plain, key, b64=True, algo_hash='sha3_256', mode='MODE_GCM') -> bytes:
-  from Crypto.Cipher import AES
-  from Crypto import Random
+def encrypt_full(plain, key, b64=True, algo_hash='sha3_256', mode='GCM') -> bytes:
   key = to_byte(key)
   algo_hash = getattr(hashlib, algo_hash)
   if len(key) != algo_hash().digest_size: key = algo_hash(key).digest()
   plain = to_byte(plain)
+  cipher = encrypt_byte(plain, key, mode)
+  if b64: cipher = base64.b64encode(cipher)
+  return cipher
+
+
+def encrypt_byte(plain:bytes, key:bytes, mode='GCM') -> bytes:
+  from Crypto.Cipher import AES
+  from Crypto import Random
   bs = AES.block_size
   iv = Random.new().read(bs)
   bs = bs - len(plain) % bs
-  plain = plain + bs*chr(bs).encode('UTF-8')
+  mode = 'MODE_' + mode
   mode = getattr(AES, mode)
-  cipher = iv + AES.new(key, mode, iv).encrypt(plain)
-  if b64: cipher = base64.b64encode(cipher)
+  cipher = iv + AES.new(key, mode, iv).encrypt(plain + bs*chr(bs).encode('UTF-8'))
   return cipher
 
 
-def decrypt_aes(enc, key, b64=True, algo_hash='sha3_256', mode='MODE_GCM') -> bytes:
-  from Crypto.Cipher import AES
+def decrypt_full(enc, key, b64=True, algo_hash='sha3_256', mode='GCM') -> bytes:
   key = to_byte(key)
   algo_hash = getattr(hashlib, algo_hash)
   if len(key) != algo_hash().digest_size: key = algo_hash(key).digest()
   enc = to_byte(enc)
   if b64: enc = base64.b64decode(enc)
+  return decrypt_byte(enc, key, mode)
+
+
+def decrypt_byte(enc, key, mode='GCM') -> bytes:
+  from Crypto.Cipher import AES
+  mode = 'MODE_' + mode
   mode = getattr(AES, mode)
   plain = AES.new(key, mode, enc[:AES.block_size]).decrypt(enc[AES.block_size:])
   return plain[:-ord(plain[len(plain)-1:])]
 
 
-
-
 def find_file(pattern, dir):
   import fnmatch
   res = []
   for root, dirs, files in os.walk(dir):
     for name in files:
       if fnmatch.fnmatch(name, pattern):
         res.append(os.path.join(root, name))
@@ -110,22 +131,23 @@
   name = file.split('/')[-1].split('.')
   name, ext = name[0], name[-1]
   with tarfile.open(file, f'r:{ext}') as f:
     f.extractall(f'tmp/{name}')
 
 
 
-def tar(src, type='bz2'):
+def tar(src, dst=None, type='bz2'):
   def func(target):
     if os.path.isdir(target): stream.add(target, '')
     else: stream.add(target, target.split('/')[-1])
   import tarfile
   os.system('mkdir -p tmp')
-  dst = gen_uuid()[:16]
-  dst = f'tmp/{dst}.tar.{type}'
+  if dst is None:
+    dst = gen_uuid()[:16]
+    dst = f'tmp/{dst}.tar.{type}'
   stream = tarfile.open(dst, f'w:{type}')
   if isinstance(src, str): func(src)
   else:
     for g in src: func(g)
   stream.close()
   return dst
 
@@ -295,22 +317,18 @@
   while not check(uuid): uuid = rand()
   uuid = ''.join(uuid)
   uuid = first + uuid
   return uuid
 
 
 def bash(code):
-  import os
-  sh = gen_uuid()
-  sh = f'/tmp/{sh}.sh'
-  with open(sh, 'w') as f:
-    f.write('#!/usr/bin/bash\n')
-    f.write(code)
+  code = '#!/usr/bin/bash\n' + code
+  sh = tmp_write(code)
   os.system(f'chmod +x {sh}')
-  os.system(sh)
+  os.system(f'/usr/bin/bash {sh}')
   os.remove(sh)
 
 
 def output(code:str|bytes, path:str|None=None, title:str=''):
   if path is None:
     if isinstance(code, bytes):
       print(title)
```

### Comparing `oahspe-0.0.6/oahspe.egg-info/PKG-INFO` & `oahspe-0.0.7/oahspe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oahspe
-Version: 0.0.6
+Version: 0.0.7
 Summary: Cloud DevOps
 Home-page: https://github.com/quangproo/oahspe
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: quangproo
 Author-email: contact@quang.pro
 License: MIT
 Keywords: oahspe
```

### Comparing `oahspe-0.0.6/setup.py` & `oahspe-0.0.7/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 setup(
   name = 'oahspe',
   packages = ['oahspe'],
   keywords = ['oahspe'],
-  version = '0.0.6',
+  version = '0.0.7',
   author = 'quangproo',
   license='MIT',
   description = 'Cloud DevOps',
   author_email = 'contact@quang.pro',
   url = 'https://github.com/quangproo/oahspe',
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',
   install_requires = [],
```

