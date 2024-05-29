# Comparing `tmp/pyerualjetwork-1.3.1.tar.gz` & `tmp/pyerualjetwork-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.3.1.tar", last modified: Tue May 28 20:54:26 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.3.2.tar", last modified: Wed May 29 18:16:42 2024, max compression
```

## Comparing `pyerualjetwork-1.3.1.tar` & `pyerualjetwork-1.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 20:54:26.655541 pyerualjetwork-1.3.1/
--rw-rw-rw-   0        0        0      421 2024-05-28 20:54:26.654545 pyerualjetwork-1.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-28 20:54:26.629903 pyerualjetwork-1.3.1/plan/
--rw-rw-rw-   0        0        0      352 2024-05-26 16:54:30.000000 pyerualjetwork-1.3.1/plan/__init__.py
--rw-rw-rw-   0        0        0    42343 2024-05-28 20:54:14.000000 pyerualjetwork-1.3.1/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-28 20:54:26.651323 pyerualjetwork-1.3.1/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      421 2024-05-28 20:54:26.000000 pyerualjetwork-1.3.1/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-28 20:54:26.000000 pyerualjetwork-1.3.1/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 20:54:26.000000 pyerualjetwork-1.3.1/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-28 20:54:26.000000 pyerualjetwork-1.3.1/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 20:54:26.656539 pyerualjetwork-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-05-28 20:53:36.000000 pyerualjetwork-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:16:42.650583 pyerualjetwork-1.3.2/
+-rw-rw-rw-   0        0        0      259 2024-05-29 18:16:42.649586 pyerualjetwork-1.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-29 18:16:42.627473 pyerualjetwork-1.3.2/plan/
+-rw-rw-rw-   0        0        0      375 2024-05-29 18:09:13.000000 pyerualjetwork-1.3.2/plan/__init__.py
+-rw-rw-rw-   0        0        0    44206 2024-05-29 18:16:26.000000 pyerualjetwork-1.3.2/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:16:42.646589 pyerualjetwork-1.3.2/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      259 2024-05-29 18:16:41.000000 pyerualjetwork-1.3.2/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-29 18:16:42.000000 pyerualjetwork-1.3.2/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:16:41.000000 pyerualjetwork-1.3.2/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-29 18:16:41.000000 pyerualjetwork-1.3.2/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:16:42.651579 pyerualjetwork-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      684 2024-05-29 18:12:38.000000 pyerualjetwork-1.3.2/setup.py
```

### Comparing `pyerualjetwork-1.3.1/plan/plan.py` & `pyerualjetwork-1.3.2/plan/plan.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,489 +5,489 @@
 import math
 from scipy.special import expit, softmax
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 # BUILD -----
 def TrainPLAN(
-    TrainInputs: List[Union[int, float]], 
-    TrainLabels: List[Union[int, float, str]], # At least two.. and one hot encoded
-    ClassCount: int,
-    Layers: List[str],
-    Neurons: List[Union[int, float]],
-    MembranThresholds: List[str],
-    MembranPotentials: List[Union[int, float]],
-    Normalizations: List[str],
-    Activations: List[str],
-    Visualize: str
+    x_train: List[Union[int, float]], 
+    y_train: List[Union[int, float, str]], # At least two.. and one hot encoded
+    class_count: int,
+    layers: List[str],
+    neurons: List[Union[int, float]],
+    membran_thresholds: List[str],
+    membran_potentials: List[Union[int, float]],
+    normalizations: List[str],
+    activations: List[str],
+    visualize: str
 ) -> str:
         
     infoPLAN = """
     Creates and configures a PLAN model.
     
     Args:
-        TrainInputs (list[num]): List of input data.
-        TrainLabels (list[num]): List of TrainLabels. (one hot encoded)
-        ClassCount (int): Number of classes.
-        Layers (list[str]): List of layer names. (options: 'fex' (Feature Extraction), 'cat' (Catalyser))
-        Neurons (list[num]): List of neuron counts for each layer.
-        MembranThresholds (list[str]): List of MembranThresholds.
-        MembranPotentials (list[num]): List of MembranPotentials.
-        Normalizations (List[str]): Whether normalization will be performed at indexed layers ("y" or "n").
-        Activations (list[str]): List of activation functions.
-        Visualize (str): Visualize Training procces or not visualize ('y' or 'n')
+        x_train (list[num]): List of input data.
+        y_train (list[num]): List of y_train. (one hot encoded)
+        class_count (int): Number of classes.
+        layers (list[str]): List of layer names. (options: 'fex' (Feature Extraction), 'cat' (Catalyser))
+        neurons (list[num]): List of neuron counts for each layer.
+        membran_thresholds (list[str]): List of membran_thresholds.
+        membran_potentials (list[num]): List of membran_potentials.
+        normalizations (List[str]): Whether normalization will be performed at indexed layers ("y" or "n").
+        activations (list[str]): List of activation functions.
+        visualize (str): visualize Training procces or not visualize ('y' or 'n')
     
     Returns:
-        list([num]): (Weight matrices list, TrainPredictions list, TrainAcc).
+        list([num]): (Weight matrices list, TrainPredictions list, Trainacc).
         error handled ?: Process status ('e')
 """
         
-    if Visualize != 'y' and Visualize != 'n':
-        print(Fore.RED + "ERROR109: Visualize parameter must be 'y' or 'n'. TrainPLAN",infoPLAN)
+    if visualize != 'y' and visualize != 'n':
+        print(Fore.RED + "ERROR109: visualize parameter must be 'y' or 'n'. TrainPLAN",infoPLAN)
         return 'e'
         
     
-    LastNeuron = Neurons[-1:][0]
-    if LastNeuron != ClassCount:
+    LastNeuron = neurons[-1:][0]
+    if LastNeuron != class_count:
             print(Fore.RED + "ERROR108: Last layer of neuron count must be equal class count. from: TrainPLAN",infoPLAN)
             return 'e'
     
-    if len(Normalizations) != len(MembranPotentials):
+    if len(normalizations) != len(membran_potentials):
         
-            print(Fore.RED + "ERROR307: Normalization list length must be equal to length of MembranThresholds List,MembranPotentials List,Layers List,Neurons List. from: TrainPLAN",infoPLAN)
+            print(Fore.RED + "ERROR307: Normalization list length must be equal to length of membran_thresholds List,membran_potentials List,layers List,neurons List. from: TrainPLAN",infoPLAN)
             return 'e'
     
-    if len(TrainInputs) != len(TrainLabels):
-        print(Fore.RED + "ERROR301: TrainInputs list and TrainLabels list must be same length.",infoPLAN)
+    if len(x_train) != len(y_train):
+        print(Fore.RED + "ERROR301: x_train list and y_train list must be same length.",infoPLAN)
         return 'e'
     
-    for i, Value in enumerate(MembranPotentials):
+    for i, Value in enumerate(membran_potentials):
         
-        if Normalizations[i] != 'y' and Normalizations[i] != 'n':
+        if normalizations[i] != 'y' and normalizations[i] != 'n':
                 print(Fore.RED + "ERROR105: Normalization list must be 'y' or 'n'.",infoPLAN)
                 return 'e'
             
-        if MembranThresholds[i] == 'none':
+        if membran_thresholds[i] == 'none':
             print(Fore.MAGENTA + "WARNING102: We are advise to do not put 'none' Threshold sign. But some cases improves performance of the model from: TrainPLAN",infoPLAN  + Style.RESET_ALL)
             time.sleep(3)
             
         if isinstance(Value, str):
             print(Fore.RED + "ERROR201: MEMBRAN POTENTIALS must be numeric. from: TrainPLAN")
             return 'e'
         
-        if isinstance(Neurons[i], str):
-            print(Fore.RED + "ERROR202: Neurons list must be numeric.")
+        if isinstance(neurons[i], str):
+            print(Fore.RED + "ERROR202: neurons list must be numeric.")
             return 'e'
     
-    if len(MembranThresholds) != len(MembranPotentials):
+    if len(membran_thresholds) != len(membran_potentials):
         print(Fore.RED + "ERROR302: MEMBRAN THRESHOLDS list and MEMBRAN POTENTIALS list must be same length. from: TrainPLAN",infoPLAN)
         return 'e'
     
-    if len(Layers) != len(Neurons):
-        print(Fore.RED + "ERROR303: Layers list and Neurons list must same length. from: TrainPLAN",infoPLAN)
+    if len(layers) != len(neurons):
+        print(Fore.RED + "ERROR303: layers list and neurons list must same length. from: TrainPLAN",infoPLAN)
         return 'e'
     
-    if len(MembranPotentials) != len(Layers) or len(MembranThresholds) != len(Layers):
-        print(Fore.RED + "ERROR306: MEMBRAN POTENTIALS and MEMBRAN THRESHOLDS lists length must be same Layers list length. from: TrainPLAN",infoPLAN)
+    if len(membran_potentials) != len(layers) or len(membran_thresholds) != len(layers):
+        print(Fore.RED + "ERROR306: MEMBRAN POTENTIALS and MEMBRAN THRESHOLDS lists length must be same layers list length. from: TrainPLAN",infoPLAN)
         return 'e'
     
     
-    for Activation in Activations:
+    for Activation in activations:
         if Activation != 'softmax' and Activation != 'sigmoid' and Activation != 'relu' and Activation != 'none':
-            print(Fore.RED + "ERROR108: Activations list must be 'sigmoid' or 'softmax' or 'relu' or 'none' from: TrainPLAN",infoPLAN)
+            print(Fore.RED + "ERROR108: activations list must be 'sigmoid' or 'softmax' or 'relu' or 'none' from: TrainPLAN",infoPLAN)
             return 'e'
     
 
-    for index, Neuron in enumerate(Neurons):
+    for index, Neuron in enumerate(neurons):
         if Neuron < 1:
-            print(Fore.RED + "ERROR101: Neurons list must be positive non zero integer. from: TrainPLAN",infoPLAN)
+            print(Fore.RED + "ERROR101: neurons list must be positive non zero integer. from: TrainPLAN",infoPLAN)
             return 'e'
         
-        if index + 1 != len(Neurons) and Neuron % 2 != 0:
+        if index + 1 != len(neurons) and Neuron % 2 != 0:
             print(Fore.MAGENTA + "WARNING101: We strongly advise to do Neuron counts be should even numbers. from: TrainPLAN",infoPLAN)
             time.sleep(3)
             
-        if Neuron < ClassCount:
+        if Neuron < class_count:
             print(Fore.RED + "ERROR102: Neuron count must be greater than class count(For PLAN). from: TrainPLAN")
             return 'e'
         
-        if Layers[index] != 'fex' and Layers[index] != 'cat':
-            print(Fore.RED + "ERROR107: Layers list must be 'fex'(Feature Extraction Layer) or 'cat' (Catalyser Layer). from: TrainPLAN",infoPLAN)
+        if layers[index] != 'fex' and layers[index] != 'cat':
+            print(Fore.RED + "ERROR107: layers list must be 'fex'(Feature Extraction Layer) or 'cat' (Catalyser Layer). from: TrainPLAN",infoPLAN)
             return 'e'
     
-    if len(MembranThresholds) != len(MembranPotentials):
+    if len(membran_thresholds) != len(membran_potentials):
         print(Fore.RED + "ERROR305: MEMBRAN THRESHOLDS list and MEMBRAN POTENTIALS list must be same length. from: TrainPLAN",infoPLAN)
         return 'e'
     
     
-    for i, Sign in enumerate(MembranThresholds):
+    for i, Sign in enumerate(membran_thresholds):
         if Sign != '>' and Sign != '<' and Sign != '==' and Sign != '!=' and Sign != 'none':
             print(Fore.RED + "ERROR104: MEMBRAN THRESHOLDS must be '>' or '<' or '==' or '!='. or 'none' WE SUGGEST '<' FOR FEX LAYER AND '==' FOR CAT LAYER (Your data, your hyperparameter) from: TrainPLAN",infoPLAN)
             return 'e'
         
-        if Layers[i] == 'fex' and Sign == 'none':
+        if layers[i] == 'fex' and Sign == 'none':
             print(Fore.RED + "ERROR109: at layer type 'fex', pairing with 'none' Threshold is not acceptlable. if you want to 'none' put '==' and make threshold value '0'. from: TrainPLAN ",infoPLAN)
             return 'e'
         
-    UniqueTrainLabels = set()
-    for sublist in TrainLabels:
+    Uniquey_train = set()
+    for sublist in y_train:
       
-        UniqueTrainLabels.add(tuple(sublist))
+        Uniquey_train.add(tuple(sublist))
     
     
-    UniqueTrainLabels = list(UniqueTrainLabels)
+    Uniquey_train = list(Uniquey_train)
     
-    TrainLabels = [tuple(sublist) for sublist in TrainLabels]
+    y_train = [tuple(sublist) for sublist in y_train]
     
     
-    if len(UniqueTrainLabels) != ClassCount:
+    if len(Uniquey_train) != class_count:
         print(Fore.RED + "ERROR106: Label variety length must be same Class Count. from: TrainPLAN",infoPLAN)
         return 'e'
     
-    TrainInputs[0] = np.array(TrainInputs[0])
-    TrainInputs[0] = TrainInputs[0].ravel()
-    TrainInputsize = len(TrainInputs[0])
+    x_train[0] = np.array(x_train[0])
+    x_train[0] = x_train[0].ravel()
+    x_train_size = len(x_train[0])
     
-    W = WeightIdentification(len(Layers) - 1,ClassCount,Neurons,TrainInputsize)
-    Divides = SynapticDividing(ClassCount,W)
+    W = WeightIdentification(len(layers) - 1,class_count,neurons,x_train_size)
+    Divides = SynapticDividing(class_count,W)
     TrainedWs = [1] * len(W)
     print(Fore.GREEN + "Train Started with 0 ERROR" + Style.RESET_ALL,)
-    TrainPredictions = [None] * len(TrainLabels)
+    TrainPredictions = [None] * len(y_train)
     true = 0
-    StartTime = time.time()
-    for index, inp in enumerate(TrainInputs):
-        UniStartTime = time.time()
+    start_time = time.time()
+    for index, inp in enumerate(x_train):
+        uni_start_time = time.time()
         inp = np.array(inp)
         inp = inp.ravel()
         
-        if TrainInputsize != len(inp):
-            print(Fore.RED +"ERROR304: All input matrices or vectors in TrainInputs list, must be same size. from: TrainPLAN",infoPLAN + Style.RESET_ALL)
+        if x_train_size != len(inp):
+            print(Fore.RED +"ERROR304: All input matrices or vectors in x_train list, must be same size. from: TrainPLAN",infoPLAN + Style.RESET_ALL)
             return 'e'
         
         
-        for Ulindex, Ul in enumerate(UniqueTrainLabels):
+        for Ulindex, Ul in enumerate(Uniquey_train):
             
-            if Ul == TrainLabels[index]:
+            if Ul == y_train[index]:
                 for Windex, w in enumerate(W):
                     for i, ul in enumerate(Ul):
                         if ul == 1.0:
                             k = i
-                    Cs = Divides[int(k)][Windex][0]
+                    cs = Divides[int(k)][Windex][0]
        
-                    W[Windex] = SynapticPruning(w, Cs, 'row', int(k),ClassCount)
+                    W[Windex] = SynapticPruning(w, cs, 'row', int(k),class_count)
 
-        NeuralLayer = inp
+        neural_layer = inp
         
-        for Lindex, Layer in enumerate(Layers):
+        for Lindex, Layer in enumerate(layers):
             
-            if Normalizations[Lindex] == 'y':
-                NeuralLayer = Normalization(NeuralLayer)
+            if normalizations[Lindex] == 'y':
+                neural_layer = Normalization(neural_layer)
                 
-            if Activations[Lindex] == 'relu':
-                NeuralLayer = Relu(NeuralLayer)
-            elif Activations[Lindex] == 'sigmoid':
-                NeuralLayer = Sigmoid(NeuralLayer)
-            elif Activations[Lindex] == 'softmax':
-                NeuralLayer = Softmax(NeuralLayer)
+            if activations[Lindex] == 'relu':
+                neural_layer = Relu(neural_layer)
+            elif activations[Lindex] == 'sigmoid':
+                neural_layer = Sigmoid(neural_layer)
+            elif activations[Lindex] == 'softmax':
+                neural_layer = Softmax(neural_layer)
                 
             if Layer == 'fex':
-                NeuralLayer,W[Lindex] = Fex(NeuralLayer, W[Lindex], MembranThresholds[Lindex], MembranPotentials[Lindex])
+                neural_layer,W[Lindex] = Fex(neural_layer, W[Lindex], membran_thresholds[Lindex], membran_potentials[Lindex])
             elif Layer == 'cat':
-                NeuralLayer,W[Lindex] = Cat(NeuralLayer, W[Lindex], MembranThresholds[Lindex], MembranPotentials[Lindex],1)
+                neural_layer,W[Lindex] = Cat(neural_layer, W[Lindex], membran_thresholds[Lindex], membran_potentials[Lindex],1)
                 
-        RealOutput = np.argmax(TrainLabels[index])
-        PredictedOutput = np.argmax(NeuralLayer)
+        RealOutput = np.argmax(y_train[index])
+        PredictedOutput = np.argmax(neural_layer)
         if RealOutput == PredictedOutput:
             true += 1
-        Acc = true / len(TrainLabels)
+        acc = true / len(y_train)
         TrainPredictions[index] = PredictedOutput
         
-        if Visualize == 'y':
+        if visualize == 'y':
         
-            TrainLabelsVisual = np.copy(TrainLabels) 
-            TrainLabelsVisual = np.argmax(TrainLabelsVisual, axis=1)
+            y_trainVisual = np.copy(y_train) 
+            y_trainVisual = np.argmax(y_trainVisual, axis=1)
             
             plt.figure(figsize=(12, 6))
-            sns.kdeplot(TrainLabelsVisual, label='Real Outputs', fill=True)
+            sns.kdeplot(y_trainVisual, label='Real Outputs', fill=True)
             sns.kdeplot(TrainPredictions, label='Predictions', fill=True)
             plt.legend()
             plt.xlabel('Class')
             plt.ylabel('Data size')
             plt.title('Predictions and Real Outputs for Training KDE Plot')
             plt.show()
             
-            if index + 1 != len(TrainInputs):
+            if index + 1 != len(x_train):
             
                 plt.close('all')
         
         if index == 0:
             for i, w in enumerate(W):
                 TrainedWs[i] = w
                      
         else:
             for i, w in enumerate(W):
                 TrainedWs[i] = TrainedWs[i] + w
             
                 
-        W = WeightIdentification(len(Layers) - 1,ClassCount,Neurons,TrainInputsize)
+        W = WeightIdentification(len(layers) - 1,class_count,neurons,x_train_size)
          
                
-        UniEndTime = time.time()
+        uni_end_time = time.time()
         
-        CalculatingEst = round((UniEndTime - UniStartTime) * (len(TrainInputs) - index),3)
+        calculating_est = round((uni_end_time - uni_start_time) * (len(x_train) - index),3)
         
-        if CalculatingEst < 60:
-            print('\rest......(sec):',CalculatingEst,'\n',end= "")
-            print('\rTrain Accuracy: ' ,Acc ,"\n", end="")
+        if calculating_est < 60:
+            print('\rest......(sec):',calculating_est,'\n',end= "")
+            print('\rTrain accuracy: ' ,acc ,"\n", end="")
         
-        elif CalculatingEst > 60 and CalculatingEst < 3600:
-            print('\rest......(min):',CalculatingEst/60,'\n',end= "")
-            print('\rTrain Accuracy: ' ,Acc ,"\n", end="")
+        elif calculating_est > 60 and calculating_est < 3600:
+            print('\rest......(min):',calculating_est/60,'\n',end= "")
+            print('\rTrain accuracy: ' ,acc ,"\n", end="")
         
-        elif CalculatingEst > 3600:
-            print('\rest......(h):',CalculatingEst/3600,'\n',end= "")
-            print('\rTrain Accuracy: ' ,Acc ,"\n", end="")
+        elif calculating_est > 3600:
+            print('\rest......(h):',calculating_est/3600,'\n',end= "")
+            print('\rTrain accuracy: ' ,acc ,"\n", end="")
         
     EndTime = time.time()
     
-    CalculatingEst = round(EndTime - StartTime,2)
+    calculating_est = round(EndTime - start_time,2)
     
     print(Fore.GREEN + " \nTrain Finished with 0 ERROR\n")
     
-    if CalculatingEst < 60:
-        print('Total training time(sec): ',CalculatingEst)
+    if calculating_est < 60:
+        print('Total training time(sec): ',calculating_est)
         
-    elif CalculatingEst > 60 and CalculatingEst < 3600:
-        print('Total training time(min): ',CalculatingEst/60)
+    elif calculating_est > 60 and calculating_est < 3600:
+        print('Total training time(min): ',calculating_est/60)
         
-    elif CalculatingEst > 3600:
-        print('Total training time(h): ',CalculatingEst/3600)
+    elif calculating_est > 3600:
+        print('Total training time(h): ',calculating_est/3600)
         
-    if Acc > 0.8:
-        print(Fore.GREEN + '\nTotal Train Accuracy: ' ,Acc, '\n',Style.RESET_ALL)
+    if acc > 0.8:
+        print(Fore.GREEN + '\nTotal Train accuracy: ' ,acc, '\n',Style.RESET_ALL)
     
-    elif Acc < 0.8 and Acc > 0.6:
-        print(Fore.MAGENTA + '\nTotal Train Accuracy: ' ,Acc, '\n',Style.RESET_ALL)
+    elif acc < 0.8 and acc > 0.6:
+        print(Fore.MAGENTA + '\nTotal Train accuracy: ' ,acc, '\n',Style.RESET_ALL)
     
-    elif Acc < 0.6:
-        print(Fore.RED+ '\nTotal Train Accuracy: ' ,Acc, '\n',Style.RESET_ALL)
+    elif acc < 0.6:
+        print(Fore.RED+ '\nTotal Train accuracy: ' ,acc, '\n',Style.RESET_ALL)
     
     
     
 
-    return TrainedWs,TrainPredictions,Acc
+    return TrainedWs,TrainPredictions,acc
         
 # FUNCTIONS -----
 
 def WeightIdentification(
-    LayerCount,      # int: Number of layers in the neural network.
-    ClassCount,      # int: Number of classes in the classification task.
-    Neurons,         # list[num]: List of neuron counts for each layer.
-    TrainInputsize        # int: Size of the input data.
+    layer_count,      # int: Number of layers in the neural network.
+    class_count,      # int: Number of classes in the classification task.
+    neurons,         # list[num]: List of neuron counts for each layer.
+    x_train_size        # int: Size of the input data.
 ) -> str:
     """
     Identifies the weights for a neural network model.
 
     Args:
-        LayerCount (int): Number of layers in the neural network.
-        ClassCount (int): Number of classes in the classification task.
-        Neurons (list[num]): List of neuron counts for each layer.
-        TrainInputsize (int): Size of the input data.
+        layer_count (int): Number of layers in the neural network.
+        class_count (int): Number of classes in the classification task.
+        neurons (list[num]): List of neuron counts for each layer.
+        x_train_size (int): Size of the input data.
 
     Returns:
         list([numpy_arrays],[...]): Weight matices of the model. .
     """
 
     
-    Wlen = LayerCount + 1
+    Wlen = layer_count + 1
     W = [None] * Wlen
-    W[0] = np.ones((Neurons[0],TrainInputsize))
-    ws = LayerCount - 1
+    W[0] = np.ones((neurons[0],x_train_size))
+    ws = layer_count - 1
     for w in range(ws):
-        W[w + 1] = np.ones((Neurons[w + 1],Neurons[w]))
-    W[LayerCount] = np.ones((ClassCount,Neurons[LayerCount - 1]))
+        W[w + 1] = np.ones((neurons[w + 1],neurons[w]))
+    W[layer_count] = np.ones((class_count,neurons[layer_count - 1]))
     return W
 
 def SynapticPruning(
     w,            # list[list[num]]: Weight matrix of the neural network.
-    Cs,           # list[list[num]]: Synaptic connections between neurons.
-    Key,          # int: Key for identifying synaptic connections.
+    cs,           # list[list[num]]: Synaptic connections between neurons.
+    key,          # int: key for identifying synaptic connections.
     Class,        # int: Class label for the current training instance.
-    ClassCount   # int: Total number of classes in the dataset.
+    class_count   # int: Total number of classes in the dataset.
     
 ) -> str:
     infoPruning = """
     Performs synaptic pruning in a neural network model.
 
     Args:
         w (list[list[num]]): Weight matrix of the neural network.
-        Cs (list[list[num]]): Synaptic connections between neurons.
-        Key (str): Key for identifying synaptic row or col connections.
+        cs (list[list[num]]): Synaptic connections between neurons.
+        key (str): key for identifying synaptic row or col connections.
         Class (int): Class label for the current training instance.
-        ClassCount (int): Total number of classes in the dataset.
+        class_count (int): Total number of classes in the dataset.
 
     Returns:
         numpy array: Weight matrix.
     """
 
     
     Class += 1 # because index start 0
     
-    if Class != ClassCount and Class != 1:
+    if Class != class_count and Class != 1:
             
-            Ce = Cs / Class
+            ce = cs / Class
      
-            w[int(Ce)-1::-1,:] = 0
+            w[int(ce)-1::-1,:] = 0
           
-            w[Cs:,:] = 0
+            w[cs:,:] = 0
     
 
     else:
         
         if Class == 1:
-            if Key == 'row':
+            if key == 'row':
     
-                w[Cs:,:] = 0
+                w[cs:,:] = 0
     
-            elif Key == 'col':
+            elif key == 'col':
     
-                w[:,Cs] = 0
+                w[:,cs] = 0
     
             else:
-                print(Fore.RED + "ERROR103: SynapticPruning func's Key parameter must be 'row' or 'col' from: SynapticPruning" + infoPruning)
+                print(Fore.RED + "ERROR103: SynapticPruning func's key parameter must be 'row' or 'col' from: SynapticPruning" + infoPruning)
                 return 'e'
         else:
-            if Key == 'row':
+            if key == 'row':
     
-                w[Cs:,:] = 0
+                w[cs:,:] = 0
     
-                Ce = int(round(w.shape[0] - Cs / ClassCount))
-                w[Ce-1::-1,:] = 0
+                ce = int(round(w.shape[0] - cs / class_count))
+                w[ce-1::-1,:] = 0
     
-            elif Key == 'col':
+            elif key == 'col':
     
-                w[:,Cs] = 0
+                w[:,cs] = 0
     
             else:
-                print(Fore.RED + "ERROR103: SynapticPruning func's Key parameter must be 'row' or 'col' from: SynapticPruning" + infoPruning + Style.RESET_ALL)
+                print(Fore.RED + "ERROR103: SynapticPruning func's key parameter must be 'row' or 'col' from: SynapticPruning" + infoPruning + Style.RESET_ALL)
                 return 'e'
     return w
 
 def SynapticDividing(
-    ClassCount,    # int: Total number of classes in the dataset.
+    class_count,    # int: Total number of classes in the dataset.
     W              # list[list[num]]: Weight matrix of the neural network.
 ) -> str:
     """
     Divides the synaptic weights of a neural network model based on class count.
 
     Args:
-        ClassCount (int): Total number of classes in the dataset.
+        class_count (int): Total number of classes in the dataset.
         W (list[list[num]]): Weight matrix of the neural network.
 
     Returns:
         list: a 3D list holds informations of divided net.
     """
 
     
     Piece = [1] * len(W)
     #print('Piece:' + Piece)
     #input()
     # Boş bir üç boyutlu liste oluşturma
-    Divides = [[[0] for _ in range(len(W))] for _ in range(ClassCount)]
+    Divides = [[[0] for _ in range(len(W))] for _ in range(class_count)]
     
     for i in range(len(W)):
             
 
-            Piece[i] = int(math.floor(W[i].shape[0] / ClassCount))
+            Piece[i] = int(math.floor(W[i].shape[0] / class_count))
 
-    Cs = 0
+    cs = 0
     # j = Classes, i = Weights, [0] = CutStart.
 
     for i in range(len(W)):
-        for j in range(ClassCount):
-            Cs = Cs + Piece[i]
-            Divides[j][i][0] = Cs
+        for j in range(class_count):
+            cs = cs + Piece[i]
+            Divides[j][i][0] = cs
             #print('Divides: ' + j + i + ' = ' + Divides[j][i][0])
             #input()
         
         j = 0
-        Cs = 0
+        cs = 0
         
     return Divides
         
 
 def Fex(
     Input,               # list[num]: Input data.
     w,                   # list[list[num]]: Weight matrix of the neural network.
-    MembranThreshold,      # str: Sign for threshold comparison ('<', '>', '==', '!=').
-    MembranPotential       # num: Threshold value for comparison.
+    membran_threshold,      # str: Sign for threshold comparison ('<', '>', '==', '!=').
+    membran_potential       # num: Threshold value for comparison.
 ) -> tuple:
     """
     Applies feature extraction process to the input data using synaptic pruning.
 
     Args:
         Input (list[num]): Input data.
         w (list[list[num]]): Weight matrix of the neural network.
-        MembranThreshold (str): Sign for threshold comparison ('<', '>', '==', '!=').
-        MembranPotential (num): Threshold value for comparison.
+        membran_threshold (str): Sign for threshold comparison ('<', '>', '==', '!=').
+        membran_potential (num): Threshold value for comparison.
 
     Returns:
         tuple: A tuple (vector) containing the neural layer result and the updated weight matrix.
     """
 
-    if MembranThreshold == '<':
-        PruneIndex = np.where(Input < MembranPotential)
-    elif MembranThreshold == '>': 
-        PruneIndex = np.where(Input > MembranPotential)
-    elif MembranThreshold == '==':
-        PruneIndex = np.where(Input == MembranPotential)
-    elif MembranThreshold == '!=':
-        PruneIndex = np.where(Input != MembranPotential)
+    if membran_threshold == '<':
+        PruneIndex = np.where(Input < membran_potential)
+    elif membran_threshold == '>': 
+        PruneIndex = np.where(Input > membran_potential)
+    elif membran_threshold == '==':
+        PruneIndex = np.where(Input == membran_potential)
+    elif membran_threshold == '!=':
+        PruneIndex = np.where(Input != membran_potential)
 
     w = SynapticPruning(w, PruneIndex, 'col', 0, 0)
 
-    NeuralLayer = np.dot(w, Input)
-    return NeuralLayer,w
+    neural_layer = np.dot(w, Input)
+    return neural_layer,w
 
 def Cat(
     Input,               # list[num]: Input data.
     w,                   # list[list[num]]: Weight matrix of the neural network.
-    MembranThreshold,      # str: Sign for threshold comparison ('<', '>', '==', '!=').
-    MembranPotential,      # num: Threshold value for comparison.
+    membran_threshold,      # str: Sign for threshold comparison ('<', '>', '==', '!=').
+    membran_potential,      # num: Threshold value for comparison.
     isTrain              # int: Flag indicating if the function is called during training (1 for training, 0 otherwise).
 ) -> tuple:
     """
     Applies categorization process to the input data using synaptic pruning if specified.
 
     Args:
         Input (list[num]): Input data.
         w (list[list[num]]): Weight matrix of the neural network.
-        MembranThreshold (str): Sign for threshold comparison ('<', '>', '==', '!=').
-        MembranPotential (num): Threshold value for comparison.
+        membran_threshold (str): Sign for threshold comparison ('<', '>', '==', '!=').
+        membran_potential (num): Threshold value for comparison.
         isTrain (int): Flag indicating if the function is called during training (1 for training, 0 otherwise).
 
     Returns:
         tuple: A tuple containing the neural layer (vector) result and the possibly updated weight matrix.
     """
 
-    if MembranThreshold == '<':     
-        PruneIndex = np.where(Input < MembranPotential)
-    elif MembranThreshold == '>':     
-        PruneIndex = np.where(Input > MembranPotential)
-    elif MembranThreshold == '==':
-        PruneIndex = np.where(Input == MembranPotential)
-    elif MembranThreshold == '!=':     
-        PruneIndex = np.where(Input != MembranPotential)
-    if isTrain == 1 and MembranThreshold != 'none':
+    if membran_threshold == '<':     
+        PruneIndex = np.where(Input < membran_potential)
+    elif membran_threshold == '>':     
+        PruneIndex = np.where(Input > membran_potential)
+    elif membran_threshold == '==':
+        PruneIndex = np.where(Input == membran_potential)
+    elif membran_threshold == '!=':     
+        PruneIndex = np.where(Input != membran_potential)
+    if isTrain == 1 and membran_threshold != 'none':
      
             w = SynapticPruning(w, PruneIndex, 'col', 0, 0)
      
     
-    NeuralLayer = np.dot(w, Input)
-    return NeuralLayer,w
+    neural_layer = np.dot(w, Input)
+    return neural_layer,w
 
 
 def Normalization(
     Input  # list[num]: Input data to be normalized.
 ):
     """
     Normalizes the input data using maximum absolute scaling.
@@ -554,199 +554,199 @@
     """
 
     
     return np.maximum(0, x)
 
 
 def TestPLAN(
-    TestInputs,         # list[list[num]]: Test input data.
-    TestLabels,         # list[num]: Test labels.
-    Layers,             # list[str]: List of layer names.
-    MembranThresholds,     # list[str]: List of MEMBRAN THRESHOLDS for each layer.
-    MembranPotentials,    # list[num]: List of MEMBRAN POTENTIALS for each layer.
-    Normalizations,    # str: Whether normalization will be performed ("y" or "n").
-    Activations,       # str: Activation function list for the neural network.
-    Visualize,         # Visualize Testing procces or not visualize ('y' or 'n')
+    x_test,         # list[list[num]]: Test input data.
+    y_test,         # list[num]: Test labels.
+    layers,             # list[str]: List of layer names.
+    membran_thresholds,     # list[str]: List of MEMBRAN THRESHOLDS for each layer.
+    membran_potentials,    # list[num]: List of MEMBRAN POTENTIALS for each layer.
+    normalizations,    # str: Whether normalization will be performed ("y" or "n").
+    activations,       # str: Activation function list for the neural network.
+    visualize,         # visualize Testing procces or not visualize ('y' or 'n')
     W                  # list[list[num]]: Weight matrix of the neural network.
 ) -> tuple:
     infoTestModel =  """
     Tests the neural network model with the given test data.
 
     Args:
-        TestInputs (list[list[num]]): Test input data.
-        TestLabels (list[num]): Test labels.
-        Layers (list[str]): List of layer names.
-        MembranThresholds (list[str]): List of MEMBRAN THRESHOLDS for each layer.
-        MembranPotentials (list[num]): List of MEMBRAN POTENTIALS for each layer.
-        Normalizatios list([str]): Whether normalization will be performed ("yes" or "no").
-        Activation (str): Activation function for the neural network.
+        x_test (list[list[num]]): Test input data.
+        y_test (list[num]): Test labels.
+        layers (list[str]): List of layer names.
+        membran_thresholds (list[str]): List of MEMBRAN THRESHOLDS for each layer.
+        membran_potentials (list[num]): List of MEMBRAN POTENTIALS for each layer.
+        normalizatios list([str]): Whether normalization will be performed ("yes" or "no").
+        activations (list[str]): Activation function for the neural network.
         W (list[list[num]]): Weight matrix of the neural network.
 
     Returns:
         tuple: A tuple containing the predicted labels and the accuracy of the model.
     """
 
 
     try:
         Wc = [0] * len(W)
         true = 0
-        TestPredictions = [None] * len(TestLabels)
+        TestPredictions = [None] * len(y_test)
         for i, w in enumerate(W):
             Wc[i] = np.copy(w)
             print('\rCopying weights.....',i+1,'/',len(W),end = "")
                 
         print(Fore.GREEN + "\n\nTest Started with 0 ERROR\n" + Style.RESET_ALL)
-        StartTime = time.time()
-        for inpIndex,Input in enumerate(TestInputs):
+        start_time = time.time()
+        for inpIndex,Input in enumerate(x_test):
             Input = np.array(Input)
             Input = Input.ravel()
-            UniStartTime = time.time()
-            NeuralLayer = Input
+            uni_start_time = time.time()
+            neural_layer = Input
             
-            for index, Layer in enumerate(Layers):
-                if Normalizations[index] == 'y':
-                    NeuralLayer = Normalization(NeuralLayer)
-                if Activations[index] == 'relu':
-                        NeuralLayer = Relu(NeuralLayer)
-                elif Activations[index] == 'sigmoid':
-                        NeuralLayer = Sigmoid(NeuralLayer)
-                elif Activations[index] == 'softmax':
-                        NeuralLayer = Softmax(NeuralLayer)
+            for index, Layer in enumerate(layers):
+                if normalizations[index] == 'y':
+                    neural_layer = Normalization(neural_layer)
+                if activations[index] == 'relu':
+                        neural_layer = Relu(neural_layer)
+                elif activations[index] == 'sigmoid':
+                        neural_layer = Sigmoid(neural_layer)
+                elif activations[index] == 'softmax':
+                        neural_layer = Softmax(neural_layer)
                         
-                if Layers[index] == 'fex':
-                    NeuralLayer,useless = Fex(NeuralLayer, W[index], MembranThresholds[index], MembranPotentials[index])
-                if Layers[index] == 'cat':
-                    NeuralLayer,useless = Cat(NeuralLayer, W[index], MembranThresholds[index], MembranPotentials[index],0)
+                if layers[index] == 'fex':
+                    neural_layer,useless = Fex(neural_layer, W[index], membran_thresholds[index], membran_potentials[index])
+                if layers[index] == 'cat':
+                    neural_layer,useless = Cat(neural_layer, W[index], membran_thresholds[index], membran_potentials[index],0)
             for i, w in enumerate(Wc):
                 W[i] = np.copy(w)
-            RealOutput = np.argmax(TestLabels[inpIndex])
-            PredictedOutput = np.argmax(NeuralLayer)
+            RealOutput = np.argmax(y_test[inpIndex])
+            PredictedOutput = np.argmax(neural_layer)
             if RealOutput == PredictedOutput:
                 true += 1
-            Acc = true / len(TestLabels)
+            acc = true / len(y_test)
             TestPredictions[inpIndex] = PredictedOutput
             
-            if Visualize == 'y':
+            if visualize == 'y':
             
-                TestLabelsVisual = np.copy(TestLabels) 
-                TestLabelsVisual = np.argmax(TestLabelsVisual, axis=1)
+                y_testVisual = np.copy(y_test) 
+                y_testVisual = np.argmax(y_testVisual, axis=1)
                 
                 plt.figure(figsize=(12, 6))
-                sns.kdeplot(TestLabelsVisual, label='Real Outputs', fill=True)
+                sns.kdeplot(y_testVisual, label='Real Outputs', fill=True)
                 sns.kdeplot(TestPredictions, label='Predictions', fill=True)
                 plt.legend()
                 plt.xlabel('Class')
                 plt.ylabel('Data size')
                 plt.title('Predictions and Real Outputs for Testing KDE Plot')
                 plt.show()
                 
-                if inpIndex + 1 != len(TestInputs):
+                if inpIndex + 1 != len(x_test):
                 
                     plt.close('all')
             
-            UniEndTime = time.time()
+            uni_end_time = time.time()
                 
-            CalculatingEst = round((UniEndTime - UniStartTime) * (len(TestInputs) - inpIndex),3)
+            calculating_est = round((uni_end_time - uni_start_time) * (len(x_test) - inpIndex),3)
                 
-            if CalculatingEst < 60:
-                print('\rest......(sec):',CalculatingEst,'\n',end= "")
-                print('\rTest Accuracy: ' ,Acc ,"\n", end="")
-            
-            elif CalculatingEst > 60 and CalculatingEst < 3600:
-                print('\rest......(min):',CalculatingEst/60,'\n',end= "")
-                print('\rTest Accuracy: ' ,Acc ,"\n", end="")
-            
-            elif CalculatingEst > 3600:
-                print('\rest......(h):',CalculatingEst/3600,'\n',end= "")
-                print('\rTest Accuracy: ' ,Acc ,"\n", end="")
+            if calculating_est < 60:
+                print('\rest......(sec):',calculating_est,'\n',end= "")
+                print('\rTest accuracy: ' ,acc ,"\n", end="")
+            
+            elif calculating_est > 60 and calculating_est < 3600:
+                print('\rest......(min):',calculating_est/60,'\n',end= "")
+                print('\rTest accuracy: ' ,acc ,"\n", end="")
+            
+            elif calculating_est > 3600:
+                print('\rest......(h):',calculating_est/3600,'\n',end= "")
+                print('\rTest accuracy: ' ,acc ,"\n", end="")
                 
         EndTime = time.time()
         for i, w in enumerate(Wc):
             W[i] = np.copy(w)
 
-        CalculatingEst = round(EndTime - StartTime,2)
+        calculating_est = round(EndTime - start_time,2)
         
         print(Fore.GREEN + "\nTest Finished with 0 ERROR\n")
         
-        if CalculatingEst < 60:
-            print('Total testing time(sec): ',CalculatingEst)
+        if calculating_est < 60:
+            print('Total testing time(sec): ',calculating_est)
             
-        elif CalculatingEst > 60 and CalculatingEst < 3600:
-            print('Total testing time(min): ',CalculatingEst/60)
+        elif calculating_est > 60 and calculating_est < 3600:
+            print('Total testing time(min): ',calculating_est/60)
             
-        elif CalculatingEst > 3600:
-            print('Total testing time(h): ',CalculatingEst/3600)
+        elif calculating_est > 3600:
+            print('Total testing time(h): ',calculating_est/3600)
             
-        if Acc >= 0.8:
-            print(Fore.GREEN + '\nTotal Test Accuracy: ' ,Acc, '\n' + Style.RESET_ALL)
+        if acc >= 0.8:
+            print(Fore.GREEN + '\nTotal Test accuracy: ' ,acc, '\n' + Style.RESET_ALL)
         
-        elif Acc < 0.8 and Acc > 0.6:
-            print(Fore.MAGENTA + '\nTotal Test Accuracy: ' ,Acc, '\n' + Style.RESET_ALL)
+        elif acc < 0.8 and acc > 0.6:
+            print(Fore.MAGENTA + '\nTotal Test accuracy: ' ,acc, '\n' + Style.RESET_ALL)
         
-        elif Acc <= 0.6:
-            print(Fore.RED+ '\nTotal Test Accuracy: ' ,Acc, '\n' + Style.RESET_ALL)   
+        elif acc <= 0.6:
+            print(Fore.RED+ '\nTotal Test accuracy: ' ,acc, '\n' + Style.RESET_ALL)   
     
     except:
         
-        print(Fore.RED + "ERROR: Testing model parameters like 'Layers' 'MembranCounts' must be same as trained model. Check parameters. Are you sure weights are loaded ? from: TestPLAN" + infoTestModel + Style.RESET_ALL)
+        print(Fore.RED + "ERROR: Testing model parameters like 'layers' 'MembranCounts' must be same as trained model. Check parameters. Are you sure weights are loaded ? from: TestPLAN" + infoTestModel + Style.RESET_ALL)
         return 'e'
    
-    return W,TestPredictions,Acc
+    return W,TestPredictions,acc
 
-def SavePLAN(ModelName,
-             ModelType,
-             Layers,
-             ClassCount,
-             MembranThresholds,
-             MembranPotentials,
-             Normalizations,
-             Activations,
-             TestAcc,
-             LogType,
-             WeightsType,
-             WeightsFormat,
-             ModelPath,
+def SavePLAN(model_name,
+             model_type,
+             layers,
+             class_count,
+             membran_thresholds,
+             membran_potentials,
+             normalizations,
+             activations,
+             test_acc,
+             log_type,
+             weights_type,
+             weights_format,
+             model_path,
              W
  ):
     
     infoSavePLAN = """
     Function to save a deep learning model.
 
     Arguments:
-    ModelName (str): Name of the model.
-    ModelType (str): Type of the model.(options: PLAN)
-    Layers (list): List containing 'fex' and 'cat' layers.
-    ClassCount (int): Number of classes.
-    MembranThresholds (list): List containing MEMBRAN THRESHOLDS.
-    MembranPotentials (list): List containing MEMBRAN POTENTIALS.
+    model_name (str): Name of the model.
+    model_type (str): Type of the model.(options: PLAN)
+    layers (list): List containing 'fex' and 'cat' layers.
+    class_count (int): Number of classes.
+    membran_thresholds (list): List containing MEMBRAN THRESHOLDS.
+    membran_potentials (list): List containing MEMBRAN POTENTIALS.
     DoNormalization (str): is that normalized data ? 'y' or 'n'.
-    Activations (list): List containing activation functions for each layer.
-    TestAcc (float): Test accuracy of the model.
-    LogType (str): Type of log to save (options: 'csv', 'txt', 'hdf5').
-    WeightsType (str): Type of weights to save (options: 'txt', 'npy', 'mat').
+    activations (list): List containing activation functions for each layer.
+    test_acc (float): Test accuracy of the model.
+    log_type (str): Type of log to save (options: 'csv', 'txt', 'hdf5').
+    weights_type (str): Type of weights to save (options: 'txt', 'npy', 'mat').
     WeightFormat (str): Format of the weights (options: 'd', 'f', 'raw').
-    ModelPath (str): Path where the model will be saved. For example: C:/Users/beydili/Desktop/denemePLAN/
+    model_path (str): Path where the model will be saved. For example: C:/Users/beydili/Desktop/denemePLAN/
     W: Weights of the model.
     
     Returns:
     str: Message indicating if the model was saved successfully or encountered an error.
     """
     
     # Operations to be performed by the function will be written here
     pass
 
-    if LogType != 'csv' and  LogType != 'txt' and LogType != 'hdf5':
+    if log_type != 'csv' and  log_type != 'txt' and log_type != 'hdf5':
         print(Fore.RED + "ERROR109: Save Log Type (File Extension) must be 'csv' or 'txt' or 'hdf5' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     
-    if WeightsType != 'txt' and  WeightsType != 'npy' and WeightsType != 'mat':
+    if weights_type != 'txt' and  weights_type != 'npy' and weights_type != 'mat':
         print(Fore.RED + "ERROR110: Save Weight type (File Extension) Type must be 'txt' or 'npy' or 'mat' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     
-    if WeightsFormat != 'd' and  WeightsFormat != 'f' and WeightsFormat != 'raw':
+    if weights_format != 'd' and  weights_format != 'f' and weights_format != 'raw':
         print(Fore.RED + "ERROR111: Weight Format Type must be 'd' or 'f' or 'raw' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     
     NeuronCount = 0
     SynapseCount = 0
     try:
         for w in W:
@@ -756,108 +756,108 @@
         
         print(Fore.RED + "ERROR: Weight matrices has a problem from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     import pandas as pd
     from datetime import datetime
     from scipy import io
     
-    data = {'MODEL NAME': ModelName,
-            'MODEL TYPE': ModelType,
-            'LAYERS': Layers,
-            'LAYER COUNT': len(Layers),
-            'CLASS COUNT': ClassCount,
-            'MEMBRAN THRESHOLDS': MembranThresholds,
-            'MEMBRAN POTENTIALS': MembranPotentials,
-            'NORMALIZATION': Normalizations,
-            'ACTIVATIONS': Activations,
+    data = {'MODEL NAME': model_name,
+            'MODEL TYPE': model_type,
+            'LAYERS': layers,
+            'LAYER COUNT': len(layers),
+            'CLASS COUNT': class_count,
+            'MEMBRAN THRESHOLDS': membran_thresholds,
+            'MEMBRAN POTENTIALS': membran_potentials,
+            'NORMALIZATION': normalizations,
+            'ACTIVATIONS': activations,
             'NEURON COUNT': NeuronCount,
             'SYNAPSE COUNT': SynapseCount,
-            'TEST ACCURACY': TestAcc,
+            'TEST ACCURACY': test_acc,
             'SAVE DATE': datetime.now(),
-            'WEIGHTS TYPE': WeightsType,
-            'WEIGHTS FORMAT': WeightsFormat,
-            'MODEL PATH': ModelPath
+            'WEIGHTS TYPE': weights_type,
+            'WEIGHTS FORMAT': weights_format,
+            'MODEL PATH': model_path
             }
     try:
         
         df = pd.DataFrame(data)
         
-        if  LogType == 'csv':
+        if  log_type == 'csv':
         
-            df.to_csv(ModelPath + ModelName + '.csv', sep='\t', index=False)
+            df.to_csv(model_path + model_name + '.csv', sep='\t', index=False)
             
-        elif LogType == 'txt':
+        elif log_type == 'txt':
             
-            df.to_csv(ModelPath + ModelName + '.txt', sep='\t', index=False)
+            df.to_csv(model_path + model_name + '.txt', sep='\t', index=False)
             
-        elif LogType == 'hdf5':
+        elif log_type == 'hdf5':
             
-            df.to_hdf(ModelPath + ModelName + '.h5', key='data', mode='w')
+            df.to_hdf(model_path + model_name + '.h5', key='data', mode='w')
             
     except:
         
-        print(Fore.RED + "ERROR: Model log not saved probably ModelPath incorrect. Check the log parameters from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
+        print(Fore.RED + "ERROR: Model log not saved probably model_path incorrect. Check the log parameters from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     try:
         
-        if WeightsType == 'txt' and WeightsFormat == 'd':
+        if weights_type == 'txt' and weights_format == 'd':
             
             for i, w in enumerate(W):
-                np.savetxt(ModelPath + ModelName +  str(i+1) + 'w.txt' ,  w, fmt='%d')
+                np.savetxt(model_path + model_name +  str(i+1) + 'w.txt' ,  w, fmt='%d')
                 
-        if WeightsType == 'txt' and WeightsFormat == 'f':
+        if weights_type == 'txt' and weights_format == 'f':
              
             for i, w in enumerate(W):
-                 np.savetxt(ModelPath + ModelName +  str(i+1) + 'w.txt' ,  w, fmt='%f')
+                 np.savetxt(model_path + model_name +  str(i+1) + 'w.txt' ,  w, fmt='%f')
         
-        if WeightsType == 'txt' and WeightsFormat == 'raw':
+        if weights_type == 'txt' and weights_format == 'raw':
             
             for i, w in enumerate(W):
-                np.savetxt(ModelPath + ModelName +  str(i+1) + 'w.txt' ,  w)
+                np.savetxt(model_path + model_name +  str(i+1) + 'w.txt' ,  w)
             
                 
         ###
         
         
-        if WeightsType == 'npy' and WeightsFormat == 'd':
+        if weights_type == 'npy' and weights_format == 'd':
             
             for i, w in enumerate(W):
-                np.save(ModelPath + ModelName + str(i+1) + 'w.npy', w.astype(int))
+                np.save(model_path + model_name + str(i+1) + 'w.npy', w.astype(int))
         
-        if WeightsType == 'npy' and WeightsFormat == 'f':
+        if weights_type == 'npy' and weights_format == 'f':
              
             for i, w in enumerate(W):
-                 np.save(ModelPath + ModelName +  str(i+1) + 'w.npy' ,  w, w.astype(float))
+                 np.save(model_path + model_name +  str(i+1) + 'w.npy' ,  w, w.astype(float))
         
-        if WeightsType == 'npy' and WeightsFormat == 'raw':
+        if weights_type == 'npy' and weights_format == 'raw':
             
             for i, w in enumerate(W):
-                np.save(ModelPath + ModelName +  str(i+1) + 'w.npy' ,  w)
+                np.save(model_path + model_name +  str(i+1) + 'w.npy' ,  w)
                 
            
         ###
         
          
-        if WeightsType == 'mat' and WeightsFormat == 'd':
+        if weights_type == 'mat' and weights_format == 'd':
             
             for i, w in enumerate(W):
                 w = {'w': w.astype(int)}
-                io.savemat(ModelPath + ModelName + str(i+1) + 'w.mat', w)
+                io.savemat(model_path + model_name + str(i+1) + 'w.mat', w)
     
-        if WeightsType == 'mat' and WeightsFormat == 'f':
+        if weights_type == 'mat' and weights_format == 'f':
              
             for i, w in enumerate(W):
                 w = {'w': w.astype(float)}
-                io.savemat(ModelPath + ModelName + str(i+1) + 'w.mat', w)
+                io.savemat(model_path + model_name + str(i+1) + 'w.mat', w)
         
-        if WeightsType == 'mat' and WeightsFormat == 'raw':
+        if weights_type == 'mat' and weights_format == 'raw':
             
             for i, w in enumerate(W):
                 w = {'w': w}
-                io.savemat(ModelPath + ModelName + str(i+1) + 'w.mat', w)
+                io.savemat(model_path + model_name + str(i+1) + 'w.mat', w)
             
     except:
         
         print(Fore.RED + "ERROR: Model Weights not saved. Check the Weight parameters. SaveFilePath expl: 'C:/Users/hasancanbeydili/Desktop/denemePLAN/' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     print(df)
     message = (
@@ -865,231 +865,275 @@
         Fore.MAGENTA + "Don't forget, if you want to load model: model log file and weight files must be in the same directory." + 
         Style.RESET_ALL
         )
     
     return print(message)
 
 
-def LoadPLAN(ModelName,
-             ModelPath,
-             LogType,
+def LoadPLAN(model_name,
+             model_path,
+             log_type,
 ):
    infoLoadPLAN = """
    Function to load a deep learning model.
 
    Arguments:
-   ModelName (str): Name of the model.
-   ModelPath (str): Path where the model is saved.
-   LogType (str): Type of log to load (options: 'csv', 'txt', 'hdf5').
+   model_name (str): Name of the model.
+   model_path (str): Path where the model is saved.
+   log_type (str): Type of log to load (options: 'csv', 'txt', 'hdf5').
 
    Returns:
-   lists: W(list[num]), Layers, MembranThresholds, MembranPotentials, Normalization,Activations
+   lists: W(list[num]), layers, membran_thresholds, membran_potentials, Normalization,activations
     """
    pass
 
     
    import pandas as pd
    import scipy.io as sio
    
    try:
    
-       if LogType == 'csv':
-           df = pd.read_csv(ModelPath + ModelName + '.' + LogType)
+       if log_type == 'csv':
+           df = pd.read_csv(model_path + model_name + '.' + log_type)
         
     
-       if LogType == 'txt':
-           df = pd.read_csv(ModelPath + ModelName + '.' + LogType, delimiter='\t')
+       if log_type == 'txt':
+           df = pd.read_csv(model_path + model_name + '.' + log_type, delimiter='\t')
         
     
-       if LogType == 'hdf5':
-           df = pd.read_hdf(ModelPath + ModelName + '.' + LogType)
+       if log_type == 'hdf5':
+           df = pd.read_hdf(model_path + model_name + '.' + log_type)
    except:
-       print(Fore.RED + "ERROR: Model Path error. Accaptable form: 'C:/Users/hasancanbeydili/Desktop/denemePLAN/' from: LoadPLAN" + infoLoadPLAN + Style.RESET_ALL)
+       print(Fore.RED + "ERROR: Model Path error. accaptable form: 'C:/Users/hasancanbeydili/Desktop/denemePLAN/' from: LoadPLAN" + infoLoadPLAN + Style.RESET_ALL)
 
-   ModelName = str(df['MODEL NAME'].iloc[0])
-   Layers = df['LAYERS'].tolist()
-   LayerCount = int(df['LAYER COUNT'].iloc[0])
-   ClassCount = int(df['CLASS COUNT'].iloc[0])
-   MembranThresholds = df['MEMBRAN THRESHOLDS'].tolist()
-   MembranPotentials = df['MEMBRAN POTENTIALS'].tolist()
-   Normalizations = df['NORMALIZATION'].tolist()
-   Activations = df['ACTIVATIONS'].tolist()
+   model_name = str(df['MODEL NAME'].iloc[0])
+   layers = df['LAYERS'].tolist()
+   layer_count = int(df['LAYER COUNT'].iloc[0])
+   class_count = int(df['CLASS COUNT'].iloc[0])
+   membran_thresholds = df['MEMBRAN THRESHOLDS'].tolist()
+   membran_potentials = df['MEMBRAN POTENTIALS'].tolist()
+   normalizations = df['NORMALIZATION'].tolist()
+   activations = df['ACTIVATIONS'].tolist()
    NeuronCount = int(df['NEURON COUNT'].iloc[0])
    SynapseCount = int(df['SYNAPSE COUNT'].iloc[0])
-   TestAcc = int(df['TEST ACCURACY'].iloc[0])
-   ModelType = str(df['MODEL TYPE'].iloc[0])
+   test_acc = int(df['TEST ACCURACY'].iloc[0])
+   model_type = str(df['MODEL TYPE'].iloc[0])
    WeightType = str(df['WEIGHTS TYPE'].iloc[0])
    WeightFormat = str(df['WEIGHTS FORMAT'].iloc[0])
-   ModelPath = str(df['MODEL PATH'].iloc[0])
+   model_path = str(df['MODEL PATH'].iloc[0])
 
-   W = [0] * LayerCount
+   W = [0] * layer_count
    
    if WeightType == 'txt':
-       for i in range(LayerCount):
-           W[i] = np.loadtxt(ModelPath + ModelName + str(i+1) + 'w.txt')
+       for i in range(layer_count):
+           W[i] = np.loadtxt(model_path + model_name + str(i+1) + 'w.txt')
    elif WeightType == 'npy':
-       for i in range(LayerCount):    
-           W[i] = np.load(ModelPath + ModelName + str(i+1) + 'w.npy')
+       for i in range(layer_count):    
+           W[i] = np.load(model_path + model_name + str(i+1) + 'w.npy')
    elif WeightType == 'mat':
-       for i in range(LayerCount):  
-           W[i] = sio.loadmat(ModelPath + ModelName + str(i+1) + 'w.mat')
+       for i in range(layer_count):  
+           W[i] = sio.loadmat(model_path + model_name + str(i+1) + 'w.mat')
    else:
         raise ValueError(Fore.RED + "Incorrect weight type value. Value must be 'txt', 'npy' or 'mat' from: LoadPLAN."  + infoLoadPLAN + Style.RESET_ALL)
    print(Fore.GREEN + "Model loaded succesfully" + Style.RESET_ALL)     
-   return W,Layers,MembranThresholds,MembranPotentials,Normalizations,Activations,df
+   return W,layers,membran_thresholds,membran_potentials,normalizations,activations,df
 
-def PredictFromDiscPLAN(Input,ModelName,ModelPath,LogType):
+def PredictFromDiscPLAN(Input,model_name,model_path,log_type):
     infoPredictFromDİscPLAN = """
     Function to make a prediction using a divided pruning deep learning neural network (PLAN).
 
     Arguments:
     Input (list or ndarray): Input data for the model (single vector or single matrix).
-    ModelName (str): Name of the model.
-    ModelPath (str): Path where the model is saved.
-    LogType (str): Type of log to load (options: 'csv', 'txt', 'hdf5').
+    model_name (str): Name of the model.
+    model_path (str): Path where the model is saved.
+    log_type (str): Type of log to load (options: 'csv', 'txt', 'hdf5').
 
     Returns:
     ndarray: Output from the model.
     """
-    W,Layers,MembranThresholds,MembranPotentials,Normalizations,Activations = LoadPLAN(ModelName,ModelPath,
-                                                                                  LogType)[0:6]
+    W,layers,membran_thresholds,membran_potentials,normalizations,activations = LoadPLAN(model_name,model_path,
+                                                                                  log_type)[0:6]
     Wc = [0] * len(W)
     for i, w in enumerate(W):
         Wc[i] = np.copy(w)
     try:
-        NeuralLayer = Input
-        NeuralLayer = np.array(NeuralLayer)
-        NeuralLayer = NeuralLayer.ravel()
-        for index, Layer in enumerate(Layers):                                                                          
+        neural_layer = Input
+        neural_layer = np.array(neural_layer)
+        neural_layer = neural_layer.ravel()
+        for index, Layer in enumerate(layers):                                                                          
             if Normalization == 'y':
-                NeuralLayer = Normalization(NeuralLayer)
-            if Activations[index] == 'relu':
-                NeuralLayer = Relu(NeuralLayer)
-            elif Activations[index] == 'sigmoid':
-                NeuralLayer = Sigmoid(NeuralLayer)
-            elif Activations[index] == 'softmax':
-                NeuralLayer = Softmax(NeuralLayer)
+                neural_layer = Normalization(neural_layer)
+            if activations[index] == 'relu':
+                neural_layer = Relu(neural_layer)
+            elif activations[index] == 'sigmoid':
+                neural_layer = Sigmoid(neural_layer)
+            elif activations[index] == 'softmax':
+                neural_layer = Softmax(neural_layer)
                                 
-            if Layers[index] == 'fex':
-                NeuralLayer,useless = Fex(NeuralLayer, W[index],
-                                          MembranThresholds[index],
-                                          MembranPotentials[index])
-            if Layers[index] == 'cat':
-                NeuralLayer,useless = Cat(NeuralLayer, W[index],
-                                          MembranThresholds[index],
-                                          MembranPotentials[index],
+            if layers[index] == 'fex':
+                neural_layer,useless = Fex(neural_layer, W[index],
+                                          membran_thresholds[index],
+                                          membran_potentials[index])
+            if layers[index] == 'cat':
+                neural_layer,useless = Cat(neural_layer, W[index],
+                                          membran_thresholds[index],
+                                          membran_potentials[index],
                                           0)
     except:
        print(Fore.RED + "ERROR: The input was probably entered incorrectly. from: PredictFromDiscPLAN"  + infoPredictFromDİscPLAN + Style.RESET_ALL)
        return 'e'
     for i, w in enumerate(Wc):
         W[i] = np.copy(w)
-    return NeuralLayer
+    return neural_layer
 
 
-def PredictFromRamPLAN(Input,Layers,MembranThresholds,MembranPotentials,Normalizations,Activations,W):
+def PredictFromRamPLAN(Input,layers,membran_thresholds,membran_potentials,normalizations,activations,W):
     infoPredictFromRamPLAN = """
     Function to make a prediction using a pruning learning artificial neural network (PLAN)
     from weights and parameters stored in memory.
 
     Arguments:
     Input (list or ndarray): Input data for the model (single vector or single matrix).
-    Layers (list): Number and types of layers.
-    MembranThresholds (list): MEMBRAN THRESHOLDS.
-    MembranPotentials (list): MEMBRAN POTENTIALS.
+    layers (list): Number and types of layers.
+    membran_thresholds (list): MEMBRAN THRESHOLDS.
+    membran_potentials (list): MEMBRAN POTENTIALS.
     DoNormalization (str): Whether to normalize ('y' or 'n').
-    Activations (list): Activation functions for each layer.
+    activations (list): Activation functions for each layer.
     W (list of ndarrays): Weights of the model.
 
     Returns:
     ndarray: Output from the model.
     """
     
     Wc = [0] * len(W)
     for i, w in enumerate(W):
         Wc[i] = np.copy(w)
     try:
-        NeuralLayer = Input
-        NeuralLayer = np.array(NeuralLayer)
-        NeuralLayer = NeuralLayer.ravel()
-        for index, Layer in enumerate(Layers):                                                                          
-            if Normalizations[index] == 'y':
-                NeuralLayer = Normalization(NeuralLayer)
-            if Activations[index] == 'relu':
-                NeuralLayer = Relu(NeuralLayer)
-            elif Activations[index] == 'sigmoid':
-                NeuralLayer = Sigmoid(NeuralLayer)
-            elif Activations[index] == 'softmax':
-                NeuralLayer = Softmax(NeuralLayer)
+        neural_layer = Input
+        neural_layer = np.array(neural_layer)
+        neural_layer = neural_layer.ravel()
+        for index, Layer in enumerate(layers):                                                                          
+            if normalizations[index] == 'y':
+                neural_layer = Normalization(neural_layer)
+            if activations[index] == 'relu':
+                neural_layer = Relu(neural_layer)
+            elif activations[index] == 'sigmoid':
+                neural_layer = Sigmoid(neural_layer)
+            elif activations[index] == 'softmax':
+                neural_layer = Softmax(neural_layer)
                                 
-            if Layers[index] == 'fex':
-                NeuralLayer,useless = Fex(NeuralLayer, W[index],
-                                          MembranThresholds[index],
-                                          MembranPotentials[index])
-            if Layers[index] == 'cat':
-                NeuralLayer,useless = Cat(NeuralLayer, W[index],
-                                          MembranThresholds[index],
-                                          MembranPotentials[index],0)
+            if layers[index] == 'fex':
+                neural_layer,useless = Fex(neural_layer, W[index],
+                                          membran_thresholds[index],
+                                          membran_potentials[index])
+            if layers[index] == 'cat':
+                neural_layer,useless = Cat(neural_layer, W[index],
+                                          membran_thresholds[index],
+                                          membran_potentials[index],0)
     except:
         print(Fore.RED + "ERROR: Unexpected input or wrong model parameters from: PredictFromRamPLAN."  + infoPredictFromRamPLAN + Style.RESET_ALL)
         return 'e'
     for i, w in enumerate(Wc):
         W[i] = np.copy(w)
-    return NeuralLayer
+    return neural_layer
     
 
-def AutoBalancer(TrainInputs, TrainLabels, ClassCount):
+def AutoBalancer(x_train, y_train, class_count):
    infoAutoBalancer = """
    Function to balance the training data across different classes.
 
    Arguments:
-   TrainInputs (list): Input data for training.
-   TrainLabels (list): Labels corresponding to the input data.
-   ClassCount (int): Number of classes.
+   x_train (list): Input data for training.
+   y_train (list): Labels corresponding to the input data.
+   class_count (int): Number of classes.
 
    Returns:
    tuple: A tuple containing balanced input data and labels.
    """
    try:
-        ClassIndices = {i: np.where(np.array(TrainLabels)[:, i] == 1)[0] for i in range(ClassCount)}
-        ClassCounts = [len(ClassIndices[i]) for i in range(ClassCount)]
+        ClassIndices = {i: np.where(np.array(y_train)[:, i] == 1)[0] for i in range(class_count)}
+        class_counts = [len(ClassIndices[i]) for i in range(class_count)]
         
-        if len(set(ClassCounts)) == 1:
+        if len(set(class_counts)) == 1:
             print(Fore.WHITE + "INFO: All training data have already balanced. from: AutoBalancer"  + Style.RESET_ALL)
-            return TrainInputs, TrainLabels
+            return x_train, y_train
         
-        MinCount = min(ClassCounts)
+        MinCount = min(class_counts)
         
         BalancedIndices = []
-        for i in range(ClassCount):
+        for i in range(class_count):
             if len(ClassIndices[i]) > MinCount:
                 SelectedIndices = np.random.choice(ClassIndices[i], MinCount, replace=False)
             else:
                 SelectedIndices = ClassIndices[i]
             BalancedIndices.extend(SelectedIndices)
         
-        BalancedInputs = [TrainInputs[idx] for idx in BalancedIndices]
-        BalancedLabels = [TrainLabels[idx] for idx in BalancedIndices]
+        BalancedInputs = [x_train[idx] for idx in BalancedIndices]
+        BalancedLabels = [y_train[idx] for idx in BalancedIndices]
         
-        print(Fore.GREEN + "All Training Data Succesfully Balanced from: " + str(len(TrainInputs)) + " to: " + str(len(BalancedInputs)) + ". from: AutoBalancer " + Style.RESET_ALL)
+        print(Fore.GREEN + "All Training Data Succesfully Balanced from: " + str(len(x_train)) + " to: " + str(len(BalancedInputs)) + ". from: AutoBalancer " + Style.RESET_ALL)
    except:
         print(Fore.RED + "ERROR: Inputs and labels must be same length check parameters" + infoAutoBalancer)
         return 'e'
         
    return BalancedInputs, BalancedLabels
    
+def SyntheticAugmentation(x, y, class_count):
+    """
+    Generates synthetic examples to balance classes with fewer examples.
+    
+    Arguments:
+    x -- Input dataset (examples) - list format
+    y -- Class labels (one-hot encoded) - list format
+    class_count -- Number of classes
+    
+    Returns:
+    x_balanced -- Balanced input dataset (list format)
+    y_balanced -- Balanced class labels (one-hot encoded, list format)
+    """
+    # Calculate class distribution
+    class_distribution = {i: 0 for i in range(class_count)}
+    for label in y:
+        class_distribution[np.argmax(label)] += 1
+    
+    max_class_count = max(class_distribution.values())
+    
+    x_balanced = list(x)
+    y_balanced = list(y)
+    
+    for class_label in range(class_count):
+        class_indices = [i for i, label in enumerate(y) if np.argmax(label) == class_label]
+        num_samples = len(class_indices)
+        
+        if num_samples < max_class_count:
+            while num_samples < max_class_count:
+                # Select two random examples
+                random_indices = np.random.choice(class_indices, 2, replace=False)
+                sample1 = x[random_indices[0]]
+                sample2 = x[random_indices[1]]
+                
+                # Generate a new synthetic example between the two selected examples
+                synthetic_sample = sample1 + (np.array(sample2) - np.array(sample1)) * np.random.rand()
+                
+                x_balanced.append(synthetic_sample.tolist())
+                y_balanced.append(y[class_indices[0]])  # The new example has the same class label
+                
+                num_samples += 1
+    
+    return np.array(x_balanced), np.array(y_balanced)
+
    
 def GetWeights():
         
     return 0
     
 def GetDf():
         
     return 6
     
 def GetPreds():
         
     return 1
     
-def GetAcc():
+def Getacc():
         
     return 2
```

### Comparing `pyerualjetwork-1.3.1/setup.py` & `pyerualjetwork-1.3.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "1.3.1",
+      version = "1.3.2",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
-      description= "Advanced python deep learning library. New Visualize parameter added ('y' or 'n') for TrainPLAN and TestPLAN funcs. (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
+      description= "Advanced python deep learning library. \n New Features: 'SyntheticAugmentation' function added for unbalanced datasets. Changes for variable names to snake_case (Function names are still PascalCase). (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks'],
 
       
       )
```

