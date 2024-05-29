# Comparing `tmp/hammingencoder-0.1.6.tar.gz` & `tmp/hammingencoder-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hammingencoder-0.1.6.tar", last modified: Wed May 29 17:06:23 2024, max compression
+gzip compressed data, was "hammingencoder-0.1.7.tar", last modified: Wed May 29 17:59:01 2024, max compression
```

## Comparing `hammingencoder-0.1.6.tar` & `hammingencoder-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 17:06:23.185539 hammingencoder-0.1.6/
-drwxrwxrwx   0        0        0        0 2024-05-29 17:06:23.163598 hammingencoder-0.1.6/HammingEncoder/
--rw-rw-rw-   0        0        0    10004 2024-05-29 17:06:18.000000 hammingencoder-0.1.6/HammingEncoder/HammingEncoder.py
--rw-rw-rw-   0        0        0       74 2024-05-29 14:54:44.000000 hammingencoder-0.1.6/HammingEncoder/__init__.py
--rw-rw-rw-   0        0        0     1670 2024-05-29 14:53:05.000000 hammingencoder-0.1.6/HammingEncoder/data_generator.py
--rw-rw-rw-   0        0        0     1500 2024-05-29 14:42:22.000000 hammingencoder-0.1.6/HammingEncoder/test.py
--rw-rw-rw-   0        0        0     4430 2024-05-29 17:06:14.000000 hammingencoder-0.1.6/HammingEncoder/train_function.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:06:23.183545 hammingencoder-0.1.6/HammingEncoder.egg-info/
--rw-rw-rw-   0        0        0     1655 2024-05-29 17:06:23.000000 hammingencoder-0.1.6/HammingEncoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2024-05-29 17:06:23.000000 hammingencoder-0.1.6/HammingEncoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 17:06:23.000000 hammingencoder-0.1.6/HammingEncoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-29 17:06:23.000000 hammingencoder-0.1.6/HammingEncoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-29 17:06:23.000000 hammingencoder-0.1.6/HammingEncoder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1655 2024-05-29 17:06:23.184542 hammingencoder-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1676 2024-05-29 16:49:27.000000 hammingencoder-0.1.6/README.rst
--rw-rw-rw-   0        0        0       42 2024-05-29 17:06:23.186537 hammingencoder-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      750 2024-05-29 17:05:46.000000 hammingencoder-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:59:01.757315 hammingencoder-0.1.7/
+drwxrwxrwx   0        0        0        0 2024-05-29 17:59:01.732382 hammingencoder-0.1.7/HammingEncoder/
+-rw-rw-rw-   0        0        0    11168 2024-05-29 17:57:44.000000 hammingencoder-0.1.7/HammingEncoder/HammingEncoder.py
+-rw-rw-rw-   0        0        0       74 2024-05-29 14:54:44.000000 hammingencoder-0.1.7/HammingEncoder/__init__.py
+-rw-rw-rw-   0        0        0     1666 2024-05-29 17:37:09.000000 hammingencoder-0.1.7/HammingEncoder/data_generator.py
+-rw-rw-rw-   0        0        0      904 2024-05-29 17:35:42.000000 hammingencoder-0.1.7/HammingEncoder/test.py
+-rw-rw-rw-   0        0        0     4430 2024-05-29 17:06:14.000000 hammingencoder-0.1.7/HammingEncoder/train_function.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:59:01.755322 hammingencoder-0.1.7/HammingEncoder.egg-info/
+-rw-rw-rw-   0        0        0     1689 2024-05-29 17:59:01.000000 hammingencoder-0.1.7/HammingEncoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2024-05-29 17:59:01.000000 hammingencoder-0.1.7/HammingEncoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 17:59:01.000000 hammingencoder-0.1.7/HammingEncoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-29 17:59:01.000000 hammingencoder-0.1.7/HammingEncoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-29 17:59:01.000000 hammingencoder-0.1.7/HammingEncoder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1689 2024-05-29 17:59:01.756320 hammingencoder-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1180 2024-05-29 17:58:54.000000 hammingencoder-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 17:59:01.757315 hammingencoder-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      750 2024-05-29 17:58:04.000000 hammingencoder-0.1.7/setup.py
```

### Comparing `hammingencoder-0.1.6/HammingEncoder/HammingEncoder.py` & `hammingencoder-0.1.7/HammingEncoder/HammingEncoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 import torch
-from .data_generator import datainput, SequenceDataset
+from data_generator import datainput, SequenceDataset
 from torch import nn
 import torch.nn.functional as F
 from torch.autograd import Function
 from torch.utils.data import Dataset, DataLoader
 from tqdm.auto import tqdm
-
+from sklearn.metrics import accuracy_score
 
 class Round_by_columnMax(Function):
     @staticmethod
     def forward(self, input):
         idx = torch.argmax(input, dim=2, keepdims=True)
         output = torch.zeros_like(input).scatter_(2, idx, 1.)
         return output
@@ -103,46 +103,46 @@
     itemset = list(itemset)
     int_itemset = [str(x) for x in itemset]
     int_itemset.sort()
     itemset = [str(x) for x in int_itemset]
     return itemset
 
 
-def seq_picture(db, itemset):
+def seq_p(db, itemset):
     # convert the sequence to a target data, which is sequence picture.
-    seq_picture = []
+    seq_p = []
     for i in tqdm(db):
-        temp_seq_picture = np.zeros(
+        temp_seq_p = np.zeros(
             [1, len(itemset), len(i)], dtype='int8')  # Only create the necessary size, no padding here
         for j in range(len(itemset)):
             for k in range(len(i)):
                 if i[k] == itemset[j]:
-                    temp_seq_picture[0, j, k] = 1
-        seq_picture.append(temp_seq_picture)
-    return seq_picture
+                    temp_seq_p[0, j, k] = 1
+        seq_p.append(temp_seq_p)
+    return seq_p
 
 def collate_fn(batch, kmer= 6):
     # Find the longest sequence in this batch
     max_length = max(max([item[0].shape[2] for item in batch]), kmer)
-    batch_seq_pictures = []
+    batch_seq_ps = []
     batch_labels = []
     
-    for seq_picture, label in batch:
+    for seq_p, label in batch:
         # Pad each sequence to have the same length
-        padded_seq = np.pad(seq_picture, ((0, 0), (0, 0), (0, max_length - seq_picture.shape[2])), mode='constant')
-        batch_seq_pictures.append(padded_seq)
+        padded_seq = np.pad(seq_p, ((0, 0), (0, 0), (0, max_length - seq_p.shape[2])), mode='constant')
+        batch_seq_ps.append(padded_seq)
         batch_labels.append(label)
 
 
-    batch_seq_pictures = np.vstack(batch_seq_pictures).astype(np.float32)  # Stack along the first dimension,    # current torch.Size([32, 94, 108]), but we need torch.Size([32, 1, 94, 108])
-    batch_seq_pictures = np.expand_dims(batch_seq_pictures, axis=1)
+    batch_seq_ps = np.vstack(batch_seq_ps).astype(np.float32)  # Stack along the first dimension,    # current torch.Size([32, 94, 108]), but we need torch.Size([32, 1, 94, 108])
+    batch_seq_ps = np.expand_dims(batch_seq_ps, axis=1)
     if batch[0][1] is None:
-        return torch.from_numpy(batch_seq_pictures)
+        return torch.from_numpy(batch_seq_ps)
 
-    return torch.from_numpy(batch_seq_pictures), torch.tensor(batch_labels)
+    return torch.from_numpy(batch_seq_ps), torch.tensor(batch_labels)
  
 def calculate_intensity(sequence, kmer_pattern):
 
     window_size = len(kmer_pattern)
     max_intensity = 0
     for i in range(len(sequence)-window_size+1):
         temp_intensity = 0
@@ -162,17 +162,18 @@
     for kmer_pattern in kmer_pattern_list:
         feature_vector.append(calculate_intensity(sequence, kmer_pattern))
     return feature_vector
 
         
         
 class HammingEncoder(nn.Module):
-    def __init__(self, X, Y, gap_constrain=5, label_number=2, Preset_set_pattern_num=100):
+    def __init__(self, X, Y, gap_constrain=5, label_number=2, Preset_set_pattern_num=100, device='cpu'):
         super(HammingEncoder, self).__init__()
-
+        self.device = device
+        print(f"Using {device}")
         self.X = X
         self.Y = Y
         self.item_set = gen_itemset(X) 
         item_size = len(self.item_set)
         self.cnn = nn.Sequential(
             Conv2d_Q(1,
                      Preset_set_pattern_num,
@@ -208,69 +209,100 @@
         conv1_weight = self.cnn[0].weight
         conv1_weight = Round_by_columnMax.apply(conv1_weight)
         conv1_weight = conv1_weight.squeeze()
         # decoupling
         kmer_patterns = generate_kmer_pattern(conv1_weight, self.item_set)
         
         return kmer_patterns
+    def predict(self, input_seqs):
+        test_p = seq_p(input_seqs, self.item_set)
+        test_set = SequenceDataset(
+            test_p, [None]*len(input_seqs))
+        test_loader = DataLoader(
+            test_set, batch_size=64, shuffle=False, num_workers=0, pin_memory=True, collate_fn=collate_fn)
+        self.eval()
+        predictions = []
+        for batch in test_loader:
+            imgs = batch
+            imgs = imgs.to(self.device)
+            outputs = self(imgs)
+            predictions.extend(outputs.argmax(dim=-1).cpu().numpy())
+        return predictions
+    
+    
+    def test(self, X, Y):
+        test_p = seq_p(X, self.item_set)
+        test_set = SequenceDataset(
+            test_p, Y)
+        test_loader = DataLoader(
+            test_set, batch_size=64, shuffle=False, num_workers=0, pin_memory=True, collate_fn=collate_fn)
+        self.eval()
+        predictions = []
+        for batch in test_loader:
+            imgs, labels = batch
+            imgs, labels = imgs.to(self.device), labels.to(self.device)
+            outputs = self(imgs)
+            predictions.extend(outputs.argmax(dim=-1).cpu().numpy())
+        acc = accuracy_score(Y, predictions)
+        return acc
     
-    def fit(self, n_epochs=100, patience=50, batchsize=64, kmer_length=5, patten_number=256,device='cuda'):
+    
+    def fit(self, n_epochs=100, patience=50, batch_size=64):
+        self.to(self.device)
         criterion = nn.CrossEntropyLoss()        
         optimizer = torch.optim.Adam(
             self.parameters(), lr=0.0003, weight_decay=1e-5)
         total_acc = []
         total_loss = []
-        seq_pictures = seq_picture(self.X, self.item_set)
+        seq_ps = seq_p(self.X, self.item_set)
         data_set = SequenceDataset(
-            seq_pictures, self.Y)
+            seq_ps, self.Y)
         data_loader = DataLoader(
-            data_set, batch_size=batchsize, shuffle=True, num_workers=0, pin_memory=True,  collate_fn=collate_fn)
+            data_set, batch_size=batch_size, shuffle=True, num_workers=0, pin_memory=True,  collate_fn=collate_fn)
         # start training
         stale = 0
         best_acc = 0
         best_train_loss = float('inf')
         for epoch in tqdm(range(n_epochs)):
             # Make sure the model is in train mode before training.
             self.train()
             # These are used to record information in training.
             train_loss_list = []
             train_accs = []
             for batch in data_loader:
                 imgs, labels = batch
-                imgs, labels = imgs.to(device), labels.to(device)
+                imgs, labels = imgs.to(self.device), labels.to(self.device)
                 outputs = self(imgs)
                 loss = criterion(outputs, labels)
                 optimizer.zero_grad()
                 loss.backward()
                 optimizer.step()
                 train_correct = (outputs.argmax(dim=-1)
                                     == labels).float().mean()
                 train_loss_list.append(loss.item())
                 train_accs.append(train_correct)
             # save loss list to csv
             train_loss = sum(train_loss_list) / len(train_loss_list)
             train_acc = sum(train_accs) / len(train_accs)
 
-            print(
-                f"[ Train | {epoch + 1:03d}/{n_epochs:03d} ] loss = {train_loss:.5f}, acc = {train_acc:.5f}")
 
             if train_loss < best_train_loss:
                 best_model = self
                 best_train_loss = train_loss
                 stale = 0
             else:
                 stale += 1
                 if stale > patience:
                     print(
                         f"No improvment {patience} consecutive epochs, early stopping")
                     break
             total_loss.append(train_loss)
             self = best_model
-    
+        print(f"[ Train | {epoch + 1:03d}/{n_epochs:03d} ] loss = {train_loss:.5f}, acc = {train_acc:.5f}")
+
     def transform(self, input_seqs):
         kmer_patterns = self.get_kmers()
         feature_vectors = []
         for seq in input_seqs:
             feature_vectors.append(generate_feature_vector(seq, kmer_patterns))
         return feature_vectors
-
```

### Comparing `hammingencoder-0.1.6/HammingEncoder/data_generator.py` & `hammingencoder-0.1.7/HammingEncoder/data_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import pandas as pd
-
-
 from torch.utils.data import Dataset
 import sklearn
 
 def datainput(filepath):
     # db: list form of a sequence
     # strdb: string form of a sequence
     # data_label: list of the label of the sequence
```

### Comparing `hammingencoder-0.1.6/HammingEncoder/train_function.py` & `hammingencoder-0.1.7/HammingEncoder/train_function.py`

 * *Files identical despite different names*

### Comparing `hammingencoder-0.1.6/HammingEncoder.egg-info/PKG-INFO` & `hammingencoder-0.1.7/HammingEncoder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HammingEncoder
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Hamming Encoder package
 Home-page: https://github.com/jd445/HammingEncoder
 Author: Junjie Dong
 Author-email: jd445@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,29 +30,32 @@
 ## Usage
 
 Here's how to use the HammingEncoder package:
 
 ### Importing the package
 
 ```python
-
 from HammingEncoder import HammingEncoder
 
 # Example data
 sequences = [
     ['0', '1', '2', '3', '4', '5', '1', '6', '5', '1', '7', '4', '5', '8', '5'], 
     ['0', '1', '4', '2', '3', '4', '5', '8', '5', '1', '7', '4', '5', '1', '5', '1', '5', '6', '5'],
     ['0', '1', '2', '3', '4', '5', '8', '5', '1', '5', '7', '5', '1', '8', '5', '1', '5', '1', '5', '1', '6', '4', '5'], 
     ['0', '4', '2', '3', '5', '7', '5', '1', '5', '4', '6', '5', '1', '5', '4', '5'],
     ]
 labels = [0, 1, 0, 1]
 
 # Initialize the encoder
-encoder = HammingEncoder(sequences, labels, gap_constrain=5, label_number=2, Preset_set_pattern_num=1024)
+encoder = HammingEncoder(sequences, labels, gap_constrain=5, label_number=2, Preset_set_pattern_num=1024, device='cpu')
 
 # Fit the model
-encoder.fit(n_epochs=100, patience=50, batch_size=64, kmer_length=5, pattern_number=1024, device='cpu')
+encoder.fit(n_epochs=100, patience=2, batchsize=64)
 
 # Transform the data
 encoded_data = encoder.transform(sequences)
 
 print("Encoded data:", encoded_data)
+
+# test
+acc = encoder.test(sequences, labels)
+print("Accuracy:", acc)
```

### Comparing `hammingencoder-0.1.6/PKG-INFO` & `hammingencoder-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HammingEncoder
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Hamming Encoder package
 Home-page: https://github.com/jd445/HammingEncoder
 Author: Junjie Dong
 Author-email: jd445@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,29 +30,32 @@
 ## Usage
 
 Here's how to use the HammingEncoder package:
 
 ### Importing the package
 
 ```python
-
 from HammingEncoder import HammingEncoder
 
 # Example data
 sequences = [
     ['0', '1', '2', '3', '4', '5', '1', '6', '5', '1', '7', '4', '5', '8', '5'], 
     ['0', '1', '4', '2', '3', '4', '5', '8', '5', '1', '7', '4', '5', '1', '5', '1', '5', '6', '5'],
     ['0', '1', '2', '3', '4', '5', '8', '5', '1', '5', '7', '5', '1', '8', '5', '1', '5', '1', '5', '1', '6', '4', '5'], 
     ['0', '4', '2', '3', '5', '7', '5', '1', '5', '4', '6', '5', '1', '5', '4', '5'],
     ]
 labels = [0, 1, 0, 1]
 
 # Initialize the encoder
-encoder = HammingEncoder(sequences, labels, gap_constrain=5, label_number=2, Preset_set_pattern_num=1024)
+encoder = HammingEncoder(sequences, labels, gap_constrain=5, label_number=2, Preset_set_pattern_num=1024, device='cpu')
 
 # Fit the model
-encoder.fit(n_epochs=100, patience=50, batch_size=64, kmer_length=5, pattern_number=1024, device='cpu')
+encoder.fit(n_epochs=100, patience=2, batchsize=64)
 
 # Transform the data
 encoded_data = encoder.transform(sequences)
 
 print("Encoded data:", encoded_data)
+
+# test
+acc = encoder.test(sequences, labels)
+print("Accuracy:", acc)
```

### Comparing `hammingencoder-0.1.6/setup.py` & `hammingencoder-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='HammingEncoder',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'torch',
         'scikit-learn',
         'pandas',
         'tqdm'
```

