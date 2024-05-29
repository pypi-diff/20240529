# Comparing `tmp/manual_tls-0.0.3.tar.gz` & `tmp/manual_tls-0.0.4.tar.gz`

## Comparing `manual_tls-0.0.3.tar` & `manual_tls-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 manual_tls-0.0.3/client.py
--rwxr-xr-x   0        0        0      302 2020-02-02 00:00:00.000000 manual_tls-0.0.3/client_key.pem
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manual_tls-0.0.3/manual_tls/__init__.py
--rwxr-xr-x   0        0        0    41158 2020-02-02 00:00:00.000000 manual_tls-0.0.3/manual_tls/manual_tls.py
--rwxr-xr-x   0        0        0     3299 2020-02-02 00:00:00.000000 manual_tls-0.0.3/.gitignore
--rwxr-xr-x   0        0        0     1105 2020-02-02 00:00:00.000000 manual_tls-0.0.3/LICENSE
--rwxr-xr-x   0        0        0     8441 2020-02-02 00:00:00.000000 manual_tls-0.0.3/README.md
--rwxr-xr-x   0        0        0      632 2020-02-02 00:00:00.000000 manual_tls-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 manual_tls-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1223 2020-02-02 00:00:00.000000 manual_tls-0.0.4/client.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manual_tls-0.0.4/manual_tls/__init__.py
+-rwxr-xr-x   0        0        0    41167 2020-02-02 00:00:00.000000 manual_tls-0.0.4/manual_tls/manual_tls.py
+-rwxr-xr-x   0        0        0     3299 2020-02-02 00:00:00.000000 manual_tls-0.0.4/.gitignore
+-rwxr-xr-x   0        0        0     1105 2020-02-02 00:00:00.000000 manual_tls-0.0.4/LICENSE
+-rwxr-xr-x   0        0        0     8441 2020-02-02 00:00:00.000000 manual_tls-0.0.4/README.md
+-rwxr-xr-x   0        0        0      632 2020-02-02 00:00:00.000000 manual_tls-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 manual_tls-0.0.4/PKG-INFO
```

### Comparing `manual_tls-0.0.3/client.py` & `manual_tls-0.0.4/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -31,17 +31,16 @@
 
 print(f"Connecting to {HOST}:{PORT}")
 comm = SocektComm(HOST, PORT, TIMEOUT)
 comm.connect()
 
 tls = ManualTls(comm)
 
-# pub_key_x, pub_key_y = tls.generate_client_key()
-pub_key_x, pub_key_y = tls.load_client_key("client_key.pem")
+pub_key_x, pub_key_y = tls.generate_client_key()
 
 print(f"pub_key_x: {pub_key_x.hex()}")
 print(f"pub_key_y: {pub_key_y.hex()}")
 
 tls.establish()
-resp = tls.transmit(REQUEST)
+resp = tls.transmit(b"\x00\x01")
 print(resp.decode(errors='ignore'))
 tls.transmit(None)
```

### Comparing `manual_tls-0.0.3/manual_tls/manual_tls.py` & `manual_tls-0.0.4/manual_tls/manual_tls.py`

 * *Files 0% similar despite different names*

```diff
@@ -901,16 +901,17 @@
         ###########################
         print("Handshake: sending a change cipher msg")
         self.prepare_send_tls(CHANGE_CIPHER, self.gen_change_cipher())
 
         ###########################
         # All client messages beyond this point are encrypted
         msgs_so_far = msgs_so_far + finished
+        transcript_hash = one_shot_sha256(msgs_so_far)
 
-        if self.client_certificate_requested == True:
+        if self.client_certificate_requested:
             client_certificate_msg, msg = self.gen_encrypted_client_certificate(
                 client_write_key, client_write_iv, client_seq_num
             )
             self.prepare_send_tls(APPLICATION_DATA, client_certificate_msg)
             client_seq_num += 1
 
             msgs_so_far = msgs_so_far + msg
@@ -938,26 +939,25 @@
         self.send_tls(APPLICATION_DATA, encrypted_handshake_msg)
         client_seq_num += 1
 
         print("Handshake finished, regenerating secrets for application data")
 
         ###########################
         # derive application secrets
-        msgs_so_far_hash = one_shot_sha256(msgs_so_far)
         premaster_secret = derive_secret(b"derived", data=one_shot_sha256(b""), key=handshake_secret, hash_len=32)
         master_secret = hmac_sha256(key=premaster_secret, data=b"\x00" * 32)
-        server_secret = derive_secret(b"s ap traffic", data=msgs_so_far_hash, key=master_secret, hash_len=32)
+        server_secret = derive_secret(b"s ap traffic", data=transcript_hash, key=master_secret, hash_len=32)
         self.server_write_key = derive_secret(b"key", data=b"", key=server_secret, hash_len=16)
         self.server_write_iv = derive_secret(b"iv", data=b"", key=server_secret, hash_len=12)
-        client_secret = derive_secret(b"c ap traffic", data=msgs_so_far_hash, key=master_secret, hash_len=32)
+        client_secret = derive_secret(b"c ap traffic", data=transcript_hash, key=master_secret, hash_len=32)
         self.client_write_key = derive_secret(b"key", data=b"", key=client_secret, hash_len=16)
         self.client_write_iv = derive_secret(b"iv", data=b"", key=client_secret, hash_len=12)
 
-        print(f"    server_write_key {server_write_key.hex()} server_write_iv {server_write_iv.hex()}")
-        print(f"    client_write_key {client_write_key.hex()} client_write_iv {client_write_iv.hex()}")
+        print(f"    server_write_key {self.server_write_key.hex()} server_write_iv {self.server_write_iv.hex()}")
+        print(f"    client_write_key {self.client_write_key.hex()} client_write_iv {self.client_write_iv.hex()}")
 
         # reset sequence numbers
         self.client_seq_num = 0
         self.server_seq_num = 0
 
     def transmit(self, data = None):
         ###########################
```

### Comparing `manual_tls-0.0.3/.gitignore` & `manual_tls-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `manual_tls-0.0.3/LICENSE` & `manual_tls-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `manual_tls-0.0.3/README.md` & `manual_tls-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `manual_tls-0.0.3/pyproject.toml` & `manual_tls-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "manual_tls"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Alexander Bersenev / Adam Augustyn", email="watsug@gmail.com" },
 ]
 description = "A tiny TLS 1.3 pure Python implementation"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `manual_tls-0.0.3/PKG-INFO` & `manual_tls-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: manual_tls
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tiny TLS 1.3 pure Python implementation
 Project-URL: Homepage, https://github.com/watsug/manual-tls
 Project-URL: Issues, https://github.com/watsug/manual-tls
 Author-email: Alexander Bersenev / Adam Augustyn <watsug@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

