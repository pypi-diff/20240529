# Comparing `tmp/ctqkit-0.1.7.tar.gz` & `tmp/ctqkit-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctqkit-0.1.7.tar", max compression
+gzip compressed data, was "ctqkit-0.1.8.tar", max compression
```

## Comparing `ctqkit-0.1.7.tar` & `ctqkit-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1060 2024-03-05 02:31:31.872856 ctqkit-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0      956 2024-05-27 06:19:04.813322 ctqkit-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       42 2024-03-04 09:21:32.455518 ctqkit-0.1.7/README.md
--rw-r--r--   0        0        0       62 2024-03-28 02:46:26.350830 ctqkit-0.1.7/src/CtqKit/__init__.py
--rw-r--r--   0        0        0     2919 2024-04-02 07:04:18.419446 ctqkit-0.1.7/src/CtqKit/account.py
--rw-r--r--   0        0        0       92 2024-04-25 08:58:29.310258 ctqkit-0.1.7/src/CtqKit/circuit/__init__.py
--rw-r--r--   0        0        0      542 2024-04-25 08:59:38.213625 ctqkit-0.1.7/src/CtqKit/circuit/barrier.py
--rw-r--r--   0        0        0      408 2024-04-25 09:07:16.885102 ctqkit-0.1.7/src/CtqKit/circuit/gate/__init__.py
--rw-r--r--   0        0        0     1393 2024-04-25 09:54:45.281271 ctqkit-0.1.7/src/CtqKit/circuit/gate/gate.py
--rw-r--r--   0        0        0      365 2024-04-25 09:55:29.916726 ctqkit-0.1.7/src/CtqKit/circuit/gate/h.py
--rw-r--r--   0        0        0      392 2024-04-25 09:57:13.755696 ctqkit-0.1.7/src/CtqKit/circuit/gate/i.py
--rw-r--r--   0        0        0      561 2024-04-25 07:57:03.110911 ctqkit-0.1.7/src/CtqKit/circuit/gate/rx.py
--rw-r--r--   0        0        0      676 2024-04-25 08:11:02.166345 ctqkit-0.1.7/src/CtqKit/circuit/gate/rxy.py
--rw-r--r--   0        0        0      551 2024-04-25 07:58:07.284707 ctqkit-0.1.7/src/CtqKit/circuit/gate/ry.py
--rw-r--r--   0        0        0      587 2024-04-25 08:28:07.056689 ctqkit-0.1.7/src/CtqKit/circuit/gate/rz.py
--rw-r--r--   0        0        0      601 2024-04-25 09:55:29.893837 ctqkit-0.1.7/src/CtqKit/circuit/gate/s.py
--rw-r--r--   0        0        0      656 2024-04-25 09:55:29.952290 ctqkit-0.1.7/src/CtqKit/circuit/gate/t.py
--rw-r--r--   0        0        0      327 2024-04-25 09:55:29.945274 ctqkit-0.1.7/src/CtqKit/circuit/gate/x.py
--rw-r--r--   0        0        0      431 2024-04-25 09:55:29.902247 ctqkit-0.1.7/src/CtqKit/circuit/gate/x2m.py
--rw-r--r--   0        0        0      430 2024-04-25 09:55:29.876786 ctqkit-0.1.7/src/CtqKit/circuit/gate/x2p.py
--rw-r--r--   0        0        0      330 2024-04-25 09:55:29.925444 ctqkit-0.1.7/src/CtqKit/circuit/gate/y.py
--rw-r--r--   0        0        0      428 2024-04-25 09:55:29.937166 ctqkit-0.1.7/src/CtqKit/circuit/gate/y2m.py
--rw-r--r--   0        0        0      425 2024-04-25 09:55:29.886773 ctqkit-0.1.7/src/CtqKit/circuit/gate/y2p.py
--rw-r--r--   0        0        0      686 2024-04-25 09:55:29.931492 ctqkit-0.1.7/src/CtqKit/circuit/gate/z.py
--rw-r--r--   0        0        0      561 2024-04-25 08:52:49.827958 ctqkit-0.1.7/src/CtqKit/circuit/instruction.py
--rw-r--r--   0        0        0      547 2024-04-25 09:04:52.115202 ctqkit-0.1.7/src/CtqKit/circuit/measure.py
--rw-r--r--   0        0        0    33420 2024-05-27 06:16:20.817255 ctqkit-0.1.7/src/CtqKit/platform.py
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 ctqkit-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-03-05 02:31:31.872856 ctqkit-0.1.8/LICENSE.txt
+-rw-r--r--   0        0        0      956 2024-05-29 01:09:04.019818 ctqkit-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-03-04 09:21:32.455518 ctqkit-0.1.8/README.md
+-rw-r--r--   0        0        0       62 2024-03-28 02:46:26.350830 ctqkit-0.1.8/src/CtqKit/__init__.py
+-rw-r--r--   0        0        0     2919 2024-04-02 07:04:18.419446 ctqkit-0.1.8/src/CtqKit/account.py
+-rw-r--r--   0        0        0       92 2024-04-25 08:58:29.310258 ctqkit-0.1.8/src/CtqKit/circuit/__init__.py
+-rw-r--r--   0        0        0      542 2024-04-25 08:59:38.213625 ctqkit-0.1.8/src/CtqKit/circuit/barrier.py
+-rw-r--r--   0        0        0      408 2024-04-25 09:07:16.885102 ctqkit-0.1.8/src/CtqKit/circuit/gate/__init__.py
+-rw-r--r--   0        0        0     1393 2024-04-25 09:54:45.281271 ctqkit-0.1.8/src/CtqKit/circuit/gate/gate.py
+-rw-r--r--   0        0        0      365 2024-04-25 09:55:29.916726 ctqkit-0.1.8/src/CtqKit/circuit/gate/h.py
+-rw-r--r--   0        0        0      392 2024-04-25 09:57:13.755696 ctqkit-0.1.8/src/CtqKit/circuit/gate/i.py
+-rw-r--r--   0        0        0      561 2024-04-25 07:57:03.110911 ctqkit-0.1.8/src/CtqKit/circuit/gate/rx.py
+-rw-r--r--   0        0        0      676 2024-04-25 08:11:02.166345 ctqkit-0.1.8/src/CtqKit/circuit/gate/rxy.py
+-rw-r--r--   0        0        0      551 2024-04-25 07:58:07.284707 ctqkit-0.1.8/src/CtqKit/circuit/gate/ry.py
+-rw-r--r--   0        0        0      587 2024-04-25 08:28:07.056689 ctqkit-0.1.8/src/CtqKit/circuit/gate/rz.py
+-rw-r--r--   0        0        0      601 2024-04-25 09:55:29.893837 ctqkit-0.1.8/src/CtqKit/circuit/gate/s.py
+-rw-r--r--   0        0        0      656 2024-04-25 09:55:29.952290 ctqkit-0.1.8/src/CtqKit/circuit/gate/t.py
+-rw-r--r--   0        0        0      327 2024-04-25 09:55:29.945274 ctqkit-0.1.8/src/CtqKit/circuit/gate/x.py
+-rw-r--r--   0        0        0      431 2024-04-25 09:55:29.902247 ctqkit-0.1.8/src/CtqKit/circuit/gate/x2m.py
+-rw-r--r--   0        0        0      430 2024-04-25 09:55:29.876786 ctqkit-0.1.8/src/CtqKit/circuit/gate/x2p.py
+-rw-r--r--   0        0        0      330 2024-04-25 09:55:29.925444 ctqkit-0.1.8/src/CtqKit/circuit/gate/y.py
+-rw-r--r--   0        0        0      428 2024-04-25 09:55:29.937166 ctqkit-0.1.8/src/CtqKit/circuit/gate/y2m.py
+-rw-r--r--   0        0        0      425 2024-04-25 09:55:29.886773 ctqkit-0.1.8/src/CtqKit/circuit/gate/y2p.py
+-rw-r--r--   0        0        0      686 2024-04-25 09:55:29.931492 ctqkit-0.1.8/src/CtqKit/circuit/gate/z.py
+-rw-r--r--   0        0        0      561 2024-04-25 08:52:49.827958 ctqkit-0.1.8/src/CtqKit/circuit/instruction.py
+-rw-r--r--   0        0        0      547 2024-04-25 09:04:52.115202 ctqkit-0.1.8/src/CtqKit/circuit/measure.py
+-rw-r--r--   0        0        0    33371 2024-05-29 01:08:50.918946 ctqkit-0.1.8/src/CtqKit/platform.py
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 ctqkit-0.1.8/PKG-INFO
```

### Comparing `ctqkit-0.1.7/LICENSE.txt` & `ctqkit-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.7/pyproject.toml` & `ctqkit-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "CtqKit"
-version = "0.1.7"
+version = "0.1.8"
 description = "中国电信天衍量子计算云平台 Python SDK (ChinaTelecom Quantum Kit)"
 authors = ["Gao Jianjian <jianjian001@outlook.com>"]
 readme = "README.md"
 license = "Apache 2.0"
 documentation = "https://qc.zdxlz.com/informationSpace"
 homepage = "https://qc.zdxlz.com/"
 classifiers = [
```

### Comparing `ctqkit-0.1.7/src/CtqKit/account.py` & `ctqkit-0.1.8/src/CtqKit/account.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.7/src/CtqKit/circuit/barrier.py` & `ctqkit-0.1.8/src/CtqKit/circuit/barrier.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.7/src/CtqKit/circuit/gate/gate.py` & `ctqkit-0.1.8/src/CtqKit/circuit/gate/gate.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.7/src/CtqKit/circuit/gate/rx.py` & `ctqkit-0.1.8/src/CtqKit/circuit/gate/rx.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.7/src/CtqKit/circuit/gate/rxy.py` & `ctqkit-0.1.8/src/CtqKit/circuit/gate/rxy.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.7/src/CtqKit/circuit/gate/ry.py` & `ctqkit-0.1.8/src/CtqKit/circuit/gate/ry.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.7/src/CtqKit/circuit/gate/rz.py` & `ctqkit-0.1.8/src/CtqKit/circuit/gate/rz.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.7/src/CtqKit/circuit/gate/s.py` & `ctqkit-0.1.8/src/CtqKit/circuit/gate/s.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.7/src/CtqKit/circuit/gate/t.py` & `ctqkit-0.1.8/src/CtqKit/circuit/gate/t.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.7/src/CtqKit/circuit/gate/z.py` & `ctqkit-0.1.8/src/CtqKit/circuit/gate/z.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.7/src/CtqKit/circuit/instruction.py` & `ctqkit-0.1.8/src/CtqKit/circuit/instruction.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.7/src/CtqKit/circuit/measure.py` & `ctqkit-0.1.8/src/CtqKit/circuit/measure.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.7/src/CtqKit/platform.py` & `ctqkit-0.1.8/src/CtqKit/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -684,15 +684,15 @@
         Returns:
             Dict: corrected probability.
         """
         CM_CACHE = {}
         if config_json is None:
             config_json = self.download_config(save_file=False)
         # qubit_num = [f'Q{i}' for i in result.get('resultStatus')[0]]
-        qubit_num = [f'Q{i}' for i in range(len(list(result.get('result').keys())[0]))]
+        qubit_num = result.get('keys')
         n = len(qubit_num)  # 测量比特个数
         qubits = config_json['readout']['readoutArray']['|0> readout fidelity']['qubit_used']
         readout_fidelity0 = config_json['readout']['readoutArray']['|0> readout fidelity']['param_list']
         readout_fidelity1 = config_json['readout']['readoutArray']['|1> readout fidelity']['param_list']
         iq2prob_fidelity = [[readout_fidelity0[qubits.index(q)], readout_fidelity1[qubits.index(q)]] for q in qubit_num]
         P = self.readout_data_to_state_probabilities_whole(result)
         Pm = list(P.values())
```

### Comparing `ctqkit-0.1.7/PKG-INFO` & `ctqkit-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CtqKit
-Version: 0.1.7
+Version: 0.1.8
 Summary: 中国电信天衍量子计算云平台 Python SDK (ChinaTelecom Quantum Kit)
 Home-page: https://qc.zdxlz.com/
 License: Apache 2.0
 Author: Gao Jianjian
 Author-email: jianjian001@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

