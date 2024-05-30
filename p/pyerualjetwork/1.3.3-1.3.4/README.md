# Comparing `tmp/pyerualjetwork-1.3.3.tar.gz` & `tmp/pyerualjetwork-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.3.3.tar", last modified: Wed May 29 18:19:20 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.3.4.tar", last modified: Wed May 29 18:38:24 2024, max compression
```

## Comparing `pyerualjetwork-1.3.3.tar` & `pyerualjetwork-1.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 18:19:20.757344 pyerualjetwork-1.3.3/
--rw-rw-rw-   0        0        0      502 2024-05-29 18:19:20.756349 pyerualjetwork-1.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-29 18:19:20.721831 pyerualjetwork-1.3.3/plan/
--rw-rw-rw-   0        0        0      375 2024-05-29 18:09:13.000000 pyerualjetwork-1.3.3/plan/__init__.py
--rw-rw-rw-   0        0        0    44206 2024-05-29 18:16:26.000000 pyerualjetwork-1.3.3/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-29 18:19:20.753351 pyerualjetwork-1.3.3/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      502 2024-05-29 18:19:19.000000 pyerualjetwork-1.3.3/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-29 18:19:20.000000 pyerualjetwork-1.3.3/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 18:19:19.000000 pyerualjetwork-1.3.3/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-29 18:19:19.000000 pyerualjetwork-1.3.3/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 18:19:20.757344 pyerualjetwork-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      681 2024-05-29 18:19:10.000000 pyerualjetwork-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:38:24.241115 pyerualjetwork-1.3.4/
+-rw-rw-rw-   0        0        0      502 2024-05-29 18:38:24.241115 pyerualjetwork-1.3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-29 18:38:24.203721 pyerualjetwork-1.3.4/plan/
+-rw-rw-rw-   0        0        0      375 2024-05-29 18:09:13.000000 pyerualjetwork-1.3.4/plan/__init__.py
+-rw-rw-rw-   0        0        0    44211 2024-05-29 18:37:16.000000 pyerualjetwork-1.3.4/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:38:24.241115 pyerualjetwork-1.3.4/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      502 2024-05-29 18:38:23.000000 pyerualjetwork-1.3.4/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-29 18:38:23.000000 pyerualjetwork-1.3.4/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:38:23.000000 pyerualjetwork-1.3.4/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-29 18:38:23.000000 pyerualjetwork-1.3.4/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:38:24.241115 pyerualjetwork-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      681 2024-05-29 18:37:49.000000 pyerualjetwork-1.3.4/setup.py
```

### Comparing `pyerualjetwork-1.3.3/plan/plan.py` & `pyerualjetwork-1.3.4/plan/plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         membran_thresholds (list[str]): List of membran_thresholds.
         membran_potentials (list[num]): List of membran_potentials.
         normalizations (List[str]): Whether normalization will be performed at indexed layers ("y" or "n").
         activations (list[str]): List of activation functions.
         visualize (str): visualize Training procces or not visualize ('y' or 'n')
     
     Returns:
-        list([num]): (Weight matrices list, TrainPredictions list, Trainacc).
+        list([num]): (Weight matrices list, train_predictions list, Trainacc).
         error handled ?: Process status ('e')
 """
         
     if visualize != 'y' and visualize != 'n':
         print(Fore.RED + "ERROR109: visualize parameter must be 'y' or 'n'. TrainPLAN",infoPLAN)
         return 'e'
         
@@ -145,17 +145,17 @@
     
     x_train[0] = np.array(x_train[0])
     x_train[0] = x_train[0].ravel()
     x_train_size = len(x_train[0])
     
     W = WeightIdentification(len(layers) - 1,class_count,neurons,x_train_size)
     Divides = SynapticDividing(class_count,W)
-    TrainedWs = [1] * len(W)
+    trained_W = [1] * len(W)
     print(Fore.GREEN + "Train Started with 0 ERROR" + Style.RESET_ALL,)
-    TrainPredictions = [None] * len(y_train)
+    train_predictions = [None] * len(y_train)
     true = 0
     start_time = time.time()
     for index, inp in enumerate(x_train):
         uni_start_time = time.time()
         inp = np.array(inp)
         inp = inp.ravel()
         
@@ -195,41 +195,41 @@
                 neural_layer,W[Lindex] = Cat(neural_layer, W[Lindex], membran_thresholds[Lindex], membran_potentials[Lindex],1)
                 
         RealOutput = np.argmax(y_train[index])
         PredictedOutput = np.argmax(neural_layer)
         if RealOutput == PredictedOutput:
             true += 1
         acc = true / len(y_train)
-        TrainPredictions[index] = PredictedOutput
+        train_predictions[index] = PredictedOutput
         
         if visualize == 'y':
         
             y_trainVisual = np.copy(y_train) 
             y_trainVisual = np.argmax(y_trainVisual, axis=1)
             
             plt.figure(figsize=(12, 6))
             sns.kdeplot(y_trainVisual, label='Real Outputs', fill=True)
-            sns.kdeplot(TrainPredictions, label='Predictions', fill=True)
+            sns.kdeplot(train_predictions, label='Predictions', fill=True)
             plt.legend()
             plt.xlabel('Class')
             plt.ylabel('Data size')
             plt.title('Predictions and Real Outputs for Training KDE Plot')
             plt.show()
             
             if index + 1 != len(x_train):
             
                 plt.close('all')
         
         if index == 0:
             for i, w in enumerate(W):
-                TrainedWs[i] = w
+                trained_W[i] = w
                      
         else:
             for i, w in enumerate(W):
-                TrainedWs[i] = TrainedWs[i] + w
+                trained_W[i] = trained_W[i] + w
             
                 
         W = WeightIdentification(len(layers) - 1,class_count,neurons,x_train_size)
          
                
         uni_end_time = time.time()
         
@@ -270,15 +270,15 @@
     
     elif acc < 0.6:
         print(Fore.RED+ '\nTotal Train accuracy: ' ,acc, '\n',Style.RESET_ALL)
     
     
     
 
-    return TrainedWs,TrainPredictions,acc
+    return trained_W,train_predictions,acc
         
 # FUNCTIONS -----
 
 def WeightIdentification(
     layer_count,      # int: Number of layers in the neural network.
     class_count,      # int: Number of classes in the classification task.
     neurons,         # list[num]: List of neuron counts for each layer.
@@ -1130,10 +1130,10 @@
         
     return 6
     
 def GetPreds():
         
     return 1
     
-def Getacc():
+def GetAcc():
         
     return 2
```

### Comparing `pyerualjetwork-1.3.3/setup.py` & `pyerualjetwork-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "1.3.3",
+      version = "1.3.4",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
       description= "Advanced python deep learning library. New Features: 'SyntheticAugmentation' function added for unbalanced datasets. Changes for variable names to snake_case (Function names are still PascalCase). (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks'],
```

