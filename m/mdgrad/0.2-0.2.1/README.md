# Comparing `tmp/mdgrad-0.2.tar.gz` & `tmp/mdgrad-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdgrad-0.2.tar", last modified: Mon May 27 21:40:01 2024, max compression
+gzip compressed data, was "mdgrad-0.2.1.tar", last modified: Thu May 30 19:28:03 2024, max compression
```

## Comparing `mdgrad-0.2.tar` & `mdgrad-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-27 21:40:01.529102 mdgrad-0.2/
--rw-r--r--   0 neddamj    (501) staff       (20)     1070 2024-05-23 16:47:17.000000 mdgrad-0.2/LICENSE
--rw-r--r--   0 neddamj    (501) staff       (20)     1962 2024-05-27 21:40:01.528843 mdgrad-0.2/PKG-INFO
--rw-r--r--   0 neddamj    (501) staff       (20)     1288 2024-05-26 16:44:42.000000 mdgrad-0.2/README.md
-drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-27 21:40:01.524723 mdgrad-0.2/mdgrad/
--rw-r--r--   0 neddamj    (501) staff       (20)       27 2024-05-27 21:31:43.000000 mdgrad-0.2/mdgrad/__init__.py
-drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-27 21:40:01.528162 mdgrad-0.2/mdgrad/nn/
--rw-r--r--   0 neddamj    (501) staff       (20)       70 2024-05-27 21:22:14.000000 mdgrad-0.2/mdgrad/nn/__init__.py
--rw-r--r--   0 neddamj    (501) staff       (20)      643 2024-05-26 16:43:14.000000 mdgrad-0.2/mdgrad/nn/activations.py
--rw-r--r--   0 neddamj    (501) staff       (20)     1952 2024-05-26 18:31:40.000000 mdgrad-0.2/mdgrad/nn/layers.py
--rw-r--r--   0 neddamj    (501) staff       (20)     1636 2024-05-27 21:03:19.000000 mdgrad-0.2/mdgrad/nn/losses.py
--rw-r--r--   0 neddamj    (501) staff       (20)      573 2024-05-27 21:31:27.000000 mdgrad-0.2/mdgrad/optim.py
--rw-r--r--   0 neddamj    (501) staff       (20)    10168 2024-05-27 21:19:31.000000 mdgrad-0.2/mdgrad/tensor.py
-drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-27 21:40:01.528463 mdgrad-0.2/mdgrad.egg-info/
--rw-r--r--   0 neddamj    (501) staff       (20)     1962 2024-05-27 21:40:01.000000 mdgrad-0.2/mdgrad.egg-info/PKG-INFO
--rw-r--r--   0 neddamj    (501) staff       (20)      314 2024-05-27 21:40:01.000000 mdgrad-0.2/mdgrad.egg-info/SOURCES.txt
--rw-r--r--   0 neddamj    (501) staff       (20)        1 2024-05-27 21:40:01.000000 mdgrad-0.2/mdgrad.egg-info/dependency_links.txt
--rw-r--r--   0 neddamj    (501) staff       (20)        6 2024-05-27 21:40:01.000000 mdgrad-0.2/mdgrad.egg-info/requires.txt
--rw-r--r--   0 neddamj    (501) staff       (20)        7 2024-05-27 21:40:01.000000 mdgrad-0.2/mdgrad.egg-info/top_level.txt
--rw-r--r--   0 neddamj    (501) staff       (20)       38 2024-05-27 21:40:01.529153 mdgrad-0.2/setup.cfg
--rw-r--r--   0 neddamj    (501) staff       (20)     2229 2024-05-27 21:39:34.000000 mdgrad-0.2/setup.py
+drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-30 19:28:03.444152 mdgrad-0.2.1/
+-rw-r--r--   0 neddamj    (501) staff       (20)     1070 2024-05-23 16:47:17.000000 mdgrad-0.2.1/LICENSE
+-rw-r--r--   0 neddamj    (501) staff       (20)     1945 2024-05-30 19:28:03.443791 mdgrad-0.2.1/PKG-INFO
+-rw-r--r--   0 neddamj    (501) staff       (20)     1345 2024-05-30 04:03:43.000000 mdgrad-0.2.1/README.md
+drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-30 19:28:03.439799 mdgrad-0.2.1/mdgrad/
+-rw-r--r--   0 neddamj    (501) staff       (20)       27 2024-05-27 21:31:43.000000 mdgrad-0.2.1/mdgrad/__init__.py
+drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-30 19:28:03.442506 mdgrad-0.2.1/mdgrad/nn/
+-rw-r--r--   0 neddamj    (501) staff       (20)       70 2024-05-27 21:22:14.000000 mdgrad-0.2.1/mdgrad/nn/__init__.py
+-rw-r--r--   0 neddamj    (501) staff       (20)      830 2024-05-29 03:21:29.000000 mdgrad-0.2.1/mdgrad/nn/activations.py
+-rw-r--r--   0 neddamj    (501) staff       (20)     1952 2024-05-26 18:31:40.000000 mdgrad-0.2.1/mdgrad/nn/layers.py
+-rw-r--r--   0 neddamj    (501) staff       (20)     1703 2024-05-28 23:43:33.000000 mdgrad-0.2.1/mdgrad/nn/losses.py
+-rw-r--r--   0 neddamj    (501) staff       (20)     1621 2024-05-29 21:08:36.000000 mdgrad-0.2.1/mdgrad/optim.py
+-rw-r--r--   0 neddamj    (501) staff       (20)    10086 2024-05-30 02:58:17.000000 mdgrad-0.2.1/mdgrad/tensor.py
+drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-30 19:28:03.443447 mdgrad-0.2.1/mdgrad.egg-info/
+-rw-r--r--   0 neddamj    (501) staff       (20)     1945 2024-05-30 19:28:03.000000 mdgrad-0.2.1/mdgrad.egg-info/PKG-INFO
+-rw-r--r--   0 neddamj    (501) staff       (20)      334 2024-05-30 19:28:03.000000 mdgrad-0.2.1/mdgrad.egg-info/SOURCES.txt
+-rw-r--r--   0 neddamj    (501) staff       (20)        1 2024-05-30 19:28:03.000000 mdgrad-0.2.1/mdgrad.egg-info/dependency_links.txt
+-rw-r--r--   0 neddamj    (501) staff       (20)        6 2024-05-30 19:28:03.000000 mdgrad-0.2.1/mdgrad.egg-info/requires.txt
+-rw-r--r--   0 neddamj    (501) staff       (20)        7 2024-05-30 19:28:03.000000 mdgrad-0.2.1/mdgrad.egg-info/top_level.txt
+-rw-r--r--   0 neddamj    (501) staff       (20)       38 2024-05-30 19:28:03.444217 mdgrad-0.2.1/setup.cfg
+-rw-r--r--   0 neddamj    (501) staff       (20)     2213 2024-05-30 19:27:10.000000 mdgrad-0.2.1/setup.py
+drwxr-xr-x   0 neddamj    (501) staff       (20)        0 2024-05-30 19:28:03.442848 mdgrad-0.2.1/test/
+-rw-r--r--   0 neddamj    (501) staff       (20)     5133 2024-05-30 03:55:49.000000 mdgrad-0.2.1/test/test_tensor.py
```

### Comparing `mdgrad-0.2/LICENSE` & `mdgrad-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdgrad-0.2/PKG-INFO` & `mdgrad-0.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,29 @@
-Metadata-Version: 2.1
-Name: mdgrad
-Version: 0.2
-Summary: Tensor-based autdiff engine and neural network API
-Author: Jordan Madden
-Author-email: <jordanmadden285@gmail.com>
-Keywords: python,tensors,neural networks,automatic differentiation
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
+from setuptools import setup, find_packages
+import os
 
+VERSION = '0.2.1'
+DESCRIPTION = 'Tensor-based autdiff engine and neural network API'
+LONG_DESCRIPTION = """
 
 # mdgrad
 
-A small autograd engine that implements backpropagation (reverse-mode autodiff). Heavily inspired by karpathy's [micrograd](https://github.com/karpathy/micrograd/tree/master), and extended to support operations on tensors instead of scalars. Includes a small neural network api for building and training neural networks.
+A small autograd engine that implements backpropagation (reverse-mode autodiff). Heavily inspired by karpathy's [micrograd](https://github.com/karpathy/micrograd/tree/master), and extended to support operations on tensors instead of scalars. Includes a small neural network api for building and training neural networks. Has a PyTorch-like API.
 
 Hopefully useful as an educational resource.
 
 ## Installation
 
 ``` bash
 pip install mdgrad
 ```
 
 ## Example Usage
 
-A silly example showing supported operations
+A dumb example showing supported operations
 
 ```python
 
 import mdgrad
 import mdgrad.nn as nn
 
 a = 3 * mdgrad.randn(3, 2)
@@ -45,15 +33,15 @@
 e = d ** 2
 f = e.sum()
 print(f.data) 
 f.backward()
 print(a.grad) 
 ```
 
-An example showing how to define and run a neural network. See demo.ipynb and/or regression_demo.ipynb for more details on training.
+An example showing how to define and run a neural network. See the files in `examples/` for more details on building and training models.
 
 ```python
 
 import mdgrad
 import mdgrad.nn as nn
 
 # Define the model and loss function
@@ -77,9 +65,30 @@
 out = model(X)
 loss = loss_fn(out, target)
 
 # Compute gradients of parameters
 loss.backward()
 ```
 
+                 """
 
-                 
+# Setting up
+setup(
+    name="mdgrad",
+    version=VERSION,
+    author="Jordan Madden",
+    author_email="<jordanmadden285@gmail.com>",
+    description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=LONG_DESCRIPTION,
+    packages=find_packages(),
+    install_requires=['numpy'],
+    keywords=['python', 'tensors', 'neural networks', 'automatic differentiation'],
+    classifiers=[
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ],
+    python_requires='>=3.8'
+)
```

### Comparing `mdgrad-0.2/README.md` & `mdgrad-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # mdgrad
 
-A small autograd engine that implements backpropagation (reverse-mode autodiff). Heavily inspired by karpathy's [micrograd](https://github.com/karpathy/micrograd/tree/master), and extended to support operations on tensors instead of scalars. Includes a small neural network api for building and training neural networks.
+A small autograd engine that implements backpropagation (reverse-mode autodiff). Heavily inspired by karpathy's [micrograd](https://github.com/karpathy/micrograd/tree/master), and extended to support operations on tensors instead of scalars. Includes a small neural network api for building and training neural networks. Has a PyTorch-like API.
 
 Hopefully useful as an educational resource.
 
 ## Installation
 
 ``` bash
 pip install mdgrad
 ```
 
 ## Example Usage
 
-A silly example showing supported operations
+A dumb example showing supported operations
 
 ```python
 
 import mdgrad
 import mdgrad.nn as nn
 
 a = 3 * mdgrad.randn(3, 2)
@@ -26,15 +26,15 @@
 e = d ** 2
 f = e.sum()
 print(f.data) 
 f.backward()
 print(a.grad) 
 ```
 
-An example showing how to define and run a neural network. See demo.ipynb for more details on training.
+An example showing how to define and run a neural network. See the files in `examples/` for more details on building and training models.
 
 ```python
 
 import mdgrad
 import mdgrad.nn as nn
 
 # Define the model and loss function
```

### Comparing `mdgrad-0.2/mdgrad/nn/activations.py` & `mdgrad-0.2.1/mdgrad/nn/activations.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 class Sigmoid(Module):
     def forward(self, x):
         assert isinstance(x, Tensor), 'input must be a Tensor'
         return x.sigmoid()
     
     def parameters(self):
         return []
+    
+class Tanh(Module):
+    def forward(self, x):
+        assert isinstance(x, Tensor), 'input must be a Tensor'
+        return x.tanh()
+    
+    def parameters(self):
+        return []
 
 class SoftMax(Module):
     def forward(self, x):
         assert isinstance(x, Tensor), 'input must be a Tensor'
         return x.softmax()
     
     def parameters(self):
```

### Comparing `mdgrad-0.2/mdgrad/nn/layers.py` & `mdgrad-0.2.1/mdgrad/nn/layers.py`

 * *Files identical despite different names*

### Comparing `mdgrad-0.2/mdgrad/nn/losses.py` & `mdgrad-0.2.1/mdgrad/nn/losses.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,16 @@
             # If y values are one-hot encoded
             confidence = np.sum(probs_clipped * y.numpy(), axis=1)
         nll = -np.log(confidence)
         out = Tensor(np.mean(nll), (x,))
 
         def _backward():
             nonlocal y
+            if type(y) != np.ndarray:
+                y =y.numpy()
             if len(y.shape) == 2:
                 # Turn labels to discrete values if they are
                 # one-hot encoded
                 y = np.argmax(y.numpy(), axis=1)
             # Gradients of inputs
             x.grad[np.arange(len(y.data)), y.astype(int)] -= 1
             x.grad += probs / len(y.data) * out.grad
```

### Comparing `mdgrad-0.2/mdgrad/tensor.py` & `mdgrad-0.2.1/mdgrad/tensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,17 +127,15 @@
             g = value * (1 - value)
             self.grad += g * out.grad
         out._backward = _backward
 
         return out
     
     def tanh(self, dim=1):
-        exp = np.exp(self.data)
-        neg_exp = np.exp(-self.data)
-        val = (exp - neg_exp)/(exp + neg_exp)
+        val = np.tanh(self.data)
         out = Tensor(val, (self,))
 
         def _backward():
             self.grad += (1 - val**2) * out.grad
         out._backward = _backward
 
         return out
```

### Comparing `mdgrad-0.2/mdgrad.egg-info/PKG-INFO` & `mdgrad-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: mdgrad
-Version: 0.2
+Version: 0.2.1
 Summary: Tensor-based autdiff engine and neural network API
 Author: Jordan Madden
 Author-email: <jordanmadden285@gmail.com>
 Keywords: python,tensors,neural networks,automatic differentiation
-Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 
+
 # mdgrad
 
-A small autograd engine that implements backpropagation (reverse-mode autodiff). Heavily inspired by karpathy's [micrograd](https://github.com/karpathy/micrograd/tree/master), and extended to support operations on tensors instead of scalars. Includes a small neural network api for building and training neural networks.
+A small autograd engine that implements backpropagation (reverse-mode autodiff). Heavily inspired by karpathy's [micrograd](https://github.com/karpathy/micrograd/tree/master), and extended to support operations on tensors instead of scalars. Includes a small neural network api for building and training neural networks. Has a PyTorch-like API.
 
 Hopefully useful as an educational resource.
 
 ## Installation
 
 ``` bash
 pip install mdgrad
 ```
 
 ## Example Usage
 
-A silly example showing supported operations
+A dumb example showing supported operations
 
 ```python
 
 import mdgrad
 import mdgrad.nn as nn
 
 a = 3 * mdgrad.randn(3, 2)
@@ -45,15 +45,15 @@
 e = d ** 2
 f = e.sum()
 print(f.data) 
 f.backward()
 print(a.grad) 
 ```
 
-An example showing how to define and run a neural network. See demo.ipynb and/or regression_demo.ipynb for more details on training.
+An example showing how to define and run a neural network. See the files in `examples/` for more details on building and training models.
 
 ```python
 
 import mdgrad
 import mdgrad.nn as nn
 
 # Define the model and loss function
@@ -77,9 +77,8 @@
 out = model(X)
 loss = loss_fn(out, target)
 
 # Compute gradients of parameters
 loss.backward()
 ```
 
-
```

