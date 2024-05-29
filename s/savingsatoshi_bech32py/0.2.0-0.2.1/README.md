# Comparing `tmp/savingsatoshi_bech32py-0.2.0.tar.gz` & `tmp/savingsatoshi_bech32py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "savingsatoshi_bech32py-0.2.0.tar", max compression
+gzip compressed data, was "savingsatoshi_bech32py-0.2.1.tar", max compression
```

## Comparing `savingsatoshi_bech32py-0.2.0.tar` & `savingsatoshi_bech32py-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-12-18 18:20:46.978590 savingsatoshi_bech32py-0.2.0/bech32py/__init__.py
--rw-r--r--   0        0        0     5106 2023-11-17 14:52:07.574039 savingsatoshi_bech32py-0.2.0/bech32py/bech32.py
--rw-r--r--   0        0        0      364 2023-12-21 18:29:00.569910 savingsatoshi_bech32py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 savingsatoshi_bech32py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-18 18:20:46.978590 savingsatoshi_bech32py-0.2.1/bech32py/__init__.py
+-rw-r--r--   0        0        0     5526 2024-05-29 19:59:07.952610 savingsatoshi_bech32py-0.2.1/bech32py/bech32.py
+-rw-r--r--   0        0        0      364 2024-05-29 20:01:41.658720 savingsatoshi_bech32py-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 savingsatoshi_bech32py-0.2.1/PKG-INFO
```

### Comparing `savingsatoshi_bech32py-0.2.0/bech32py/bech32.py` & `savingsatoshi_bech32py-0.2.1/bech32py/bech32.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,58 +41,58 @@
         top = chk >> 25
         chk = (chk & 0x1ffffff) << 5 ^ value
         for i in range(5):
             chk ^= generator[i] if ((top >> i) & 1) else 0
     return chk
 
 
-def bech32_hrp_expand(hrp):
-    """Expand the HRP into values for checksum computation."""
-    return [ord(x) >> 5 for x in hrp] + [0] + [ord(x) & 31 for x in hrp]
+def bech32_hrp_expand(human_readable_prefix):
+    """Expand the human readable prefix into values for checksum computation."""
+    return [ord(x) >> 5 for x in human_readable_prefix] + [0] + [ord(x) & 31 for x in human_readable_prefix]
 
 
-def bech32_verify_checksum(hrp, data):
-    """Verify a checksum given HRP and converted data characters."""
-    const = bech32_polymod(bech32_hrp_expand(hrp) + data)
+def bech32_verify_checksum(human_readable_prefix, data):
+    """Verify a checksum given human readable prefix and converted data characters."""
+    const = bech32_polymod(bech32_hrp_expand(human_readable_prefix) + data)
     if const == 1:
         return Encoding.BECH32
     if const == BECH32M_CONST:
         return Encoding.BECH32M
     return None
 
-def bech32_create_checksum(hrp, data, spec):
-    """Compute the checksum values given HRP and data."""
-    values = bech32_hrp_expand(hrp) + data
+def bech32_create_checksum(human_readable_prefix, data, spec):
+    """Compute the checksum values given a human readable prefix and data."""
+    values = bech32_hrp_expand(human_readable_prefix) + data
     const = BECH32M_CONST if spec == Encoding.BECH32M else 1
     polymod = bech32_polymod(values + [0, 0, 0, 0, 0, 0]) ^ const
     return [(polymod >> 5 * (5 - i)) & 31 for i in range(6)]
 
 
-def bech32_encode(hrp, data, spec):
-    """Compute a Bech32 string given HRP and data values."""
-    combined = data + bech32_create_checksum(hrp, data, spec)
-    return hrp + '1' + ''.join([CHARSET[d] for d in combined])
+def bech32_encode(human_readable_prefix, data, spec):
+    """Compute a Bech32 string given a human readable prefix and data values."""
+    combined = data + bech32_create_checksum(human_readable_prefix, data, spec)
+    return human_readable_prefix + '1' + ''.join([CHARSET[d] for d in combined])
 
 def bech32_decode(bech):
-    """Validate a Bech32/Bech32m string, and determine HRP and data."""
+    """Validate a Bech32/Bech32m string, and determine a human readable prefix and data."""
     if ((any(ord(x) < 33 or ord(x) > 126 for x in bech)) or
             (bech.lower() != bech and bech.upper() != bech)):
         return (None, None, None)
     bech = bech.lower()
     pos = bech.rfind('1')
     if pos < 1 or pos + 7 > len(bech) or len(bech) > 90:
         return (None, None, None)
     if not all(x in CHARSET for x in bech[pos+1:]):
         return (None, None, None)
-    hrp = bech[:pos]
+    human_readable_prefix = bech[:pos]
     data = [CHARSET.find(x) for x in bech[pos+1:]]
-    spec = bech32_verify_checksum(hrp, data)
+    spec = bech32_verify_checksum(human_readable_prefix, data)
     if spec is None:
         return (None, None, None)
-    return (hrp, data[:-6], spec)
+    return (human_readable_prefix, data[:-6], spec)
 
 def convertbits(data, frombits, tobits, pad=True):
     """General power-of-2 base conversion."""
     acc = 0
     bits = 0
     ret = []
     maxv = (1 << tobits) - 1
@@ -109,31 +109,31 @@
         if bits:
             ret.append((acc << (tobits - bits)) & maxv)
     elif bits >= frombits or ((acc << (tobits - bits)) & maxv):
         return None
     return ret
 
 
-def decode(hrp, addr):
+def decode(human_readable_prefix, addr):
     """Decode a segwit address."""
     hrpgot, data, spec = bech32_decode(addr)
-    if hrpgot != hrp:
+    if hrpgot != human_readable_prefix:
         return (None, None)
     decoded = convertbits(data[1:], 5, 8, False)
     if decoded is None or len(decoded) < 2 or len(decoded) > 40:
         return (None, None)
     if data[0] > 16:
         return (None, None)
     if data[0] == 0 and len(decoded) != 20 and len(decoded) != 32:
         return (None, None)
     if data[0] == 0 and spec != Encoding.BECH32 or data[0] != 0 and spec != Encoding.BECH32M:
         return (None, None)
     return (data[0], decoded)
 
 
-def encode(hrp, witver, witprog):
+def encode(human_readable_prefix, witver, witprog):
     """Encode a segwit address."""
     spec = Encoding.BECH32 if witver == 0 else Encoding.BECH32M
-    ret = bech32_encode(hrp, [witver] + convertbits(witprog, 8, 5), spec)
-    if decode(hrp, ret) == (None, None):
+    ret = bech32_encode(human_readable_prefix, [witver] + convertbits(witprog, 8, 5), spec)
+    if decode(human_readable_prefix, ret) == (None, None):
         return None
     return ret
```

