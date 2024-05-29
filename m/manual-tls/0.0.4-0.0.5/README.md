# Comparing `tmp/manual_tls-0.0.4.tar.gz` & `tmp/manual_tls-0.0.5.tar.gz`

## Comparing `manual_tls-0.0.4.tar` & `manual_tls-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     1223 2020-02-02 00:00:00.000000 manual_tls-0.0.4/client.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manual_tls-0.0.4/manual_tls/__init__.py
--rwxr-xr-x   0        0        0    41167 2020-02-02 00:00:00.000000 manual_tls-0.0.4/manual_tls/manual_tls.py
--rwxr-xr-x   0        0        0     3299 2020-02-02 00:00:00.000000 manual_tls-0.0.4/.gitignore
--rwxr-xr-x   0        0        0     1105 2020-02-02 00:00:00.000000 manual_tls-0.0.4/LICENSE
--rwxr-xr-x   0        0        0     8441 2020-02-02 00:00:00.000000 manual_tls-0.0.4/README.md
--rwxr-xr-x   0        0        0      632 2020-02-02 00:00:00.000000 manual_tls-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 manual_tls-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1186 2020-02-02 00:00:00.000000 manual_tls-0.0.5/client.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manual_tls-0.0.5/manual_tls/__init__.py
+-rwxr-xr-x   0        0        0    41441 2020-02-02 00:00:00.000000 manual_tls-0.0.5/manual_tls/manual_tls.py
+-rwxr-xr-x   0        0        0     3299 2020-02-02 00:00:00.000000 manual_tls-0.0.5/.gitignore
+-rwxr-xr-x   0        0        0     1105 2020-02-02 00:00:00.000000 manual_tls-0.0.5/LICENSE
+-rwxr-xr-x   0        0        0     8441 2020-02-02 00:00:00.000000 manual_tls-0.0.5/README.md
+-rwxr-xr-x   0        0        0      632 2020-02-02 00:00:00.000000 manual_tls-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 manual_tls-0.0.5/PKG-INFO
```

### Comparing `manual_tls-0.0.4/client.py` & `manual_tls-0.0.5/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import socket
 from manual_tls.manual_tls import ManualComm, ManualTls
 
-# HOST = "habr.com"
-# PORT = 443
-HOST = "localhost"
-PORT = 4433
+HOST = "habr.com"
+PORT = 443
 TIMEOUT = 10
 REQUEST = b"HEAD /ru/company/habr/blog/522330/ HTTP/1.1\r\nHost: habr.com\r\nConnection: close\r\n\r\n"
 
 class SocektComm(ManualComm):
     def __init__(self, host, port, timeout) -> None:
         self.host = host
         self.port = port
```

### Comparing `manual_tls-0.0.4/manual_tls/manual_tls.py` & `manual_tls-0.0.5/manual_tls/manual_tls.py`

 * *Files 0% similar despite different names*

```diff
@@ -763,14 +763,17 @@
     def load_client_key(self, key_file):
         with open(key_file, "r") as file:
             pem = file.read()
             self.client_key = SigningKey.from_pem(pem)
             pub_key = self.client_key.verifying_key.to_string()
             return pub_key[0:32], pub_key[32:64]
 
+    def is_client_certificate_requested(self) -> bool:
+        return self.client_certificate_requested
+
     def establish(self):
         print("Generating params for a client hello, the first message of TLS handshake")
         SECP256R1_P = 0xffffffff00000001000000000000000000000000ffffffffffffffffffffffff
         SECP256R1_A = 0xffffffff00000001000000000000000000000000fffffffffffffffffffffffc
         SECP256R1_G = (0x6b17d1f2e12c4247f8bce6e563a440f277037d812deb33a0f4a13945d898c296,
                     0x4fe342e2fe1a7f9b8ee7eb4a7c0f9e162bce33576b315ececbb6406837bf51f5)
 
@@ -903,33 +906,34 @@
         self.prepare_send_tls(CHANGE_CIPHER, self.gen_change_cipher())
 
         ###########################
         # All client messages beyond this point are encrypted
         msgs_so_far = msgs_so_far + finished
         transcript_hash = one_shot_sha256(msgs_so_far)
 
-        if self.client_certificate_requested:
+        if self.is_client_certificate_requested():
             client_certificate_msg, msg = self.gen_encrypted_client_certificate(
                 client_write_key, client_write_iv, client_seq_num
             )
-            self.prepare_send_tls(APPLICATION_DATA, client_certificate_msg)
-            client_seq_num += 1
-
-            msgs_so_far = msgs_so_far + msg
+            
+            if client_certificate_msg is not None:
+                self.prepare_send_tls(APPLICATION_DATA, client_certificate_msg)
+                client_seq_num += 1
+                msgs_so_far = msgs_so_far + msg
 
             client_certificate_verify_msg, msg = (
                 self.gen_encrypted_client_certificate_verify(
                     client_write_key, client_write_iv, client_seq_num, msgs_so_far
                 )
             )
 
-            msgs_so_far = msgs_so_far + msg
-
-            self.prepare_send_tls(APPLICATION_DATA, client_certificate_verify_msg)
-            client_seq_num += 1
+            if client_certificate_verify_msg is not None:
+                self.prepare_send_tls(APPLICATION_DATA, client_certificate_verify_msg)
+                client_seq_num += 1
+                msgs_so_far = msgs_so_far + msg                
 
         msgs_sha256 = one_shot_sha256(msgs_so_far)
 
         client_finish_val = hmac_sha256(client_finished_key, msgs_sha256)
 
         print("Handshake: sending an encrypted finished msg")
         encrypted_handshake_msg = self.gen_encrypted_finished(
```

### Comparing `manual_tls-0.0.4/.gitignore` & `manual_tls-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `manual_tls-0.0.4/LICENSE` & `manual_tls-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `manual_tls-0.0.4/README.md` & `manual_tls-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `manual_tls-0.0.4/pyproject.toml` & `manual_tls-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "manual_tls"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Alexander Bersenev / Adam Augustyn", email="watsug@gmail.com" },
 ]
 description = "A tiny TLS 1.3 pure Python implementation"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `manual_tls-0.0.4/PKG-INFO` & `manual_tls-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: manual_tls
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tiny TLS 1.3 pure Python implementation
 Project-URL: Homepage, https://github.com/watsug/manual-tls
 Project-URL: Issues, https://github.com/watsug/manual-tls
 Author-email: Alexander Bersenev / Adam Augustyn <watsug@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

