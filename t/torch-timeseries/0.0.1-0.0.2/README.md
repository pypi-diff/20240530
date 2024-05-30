# Comparing `tmp/torch_timeseries-0.0.1.tar.gz` & `tmp/torch_timeseries-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_timeseries-0.0.1.tar", last modified: Sat May 25 07:24:04 2024, max compression
+gzip compressed data, was "torch_timeseries-0.0.2.tar", last modified: Wed May 29 13:13:52 2024, max compression
```

## Comparing `torch_timeseries-0.0.1.tar` & `torch_timeseries-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 07:24:03.776640 torch_timeseries-0.0.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-24 14:44:45.000000 torch_timeseries-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    16733 2024-05-25 07:24:03.764646 torch_timeseries-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2818 2024-05-24 16:36:19.000000 torch_timeseries-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)      741 2024-05-25 06:55:33.000000 torch_timeseries-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-25 07:24:03.776640 torch_timeseries-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1046 2024-05-25 07:23:52.000000 torch_timeseries-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 07:24:03.740658 torch_timeseries-0.0.1/torch_timeseries.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16733 2024-05-25 07:24:03.000000 torch_timeseries-0.0.1/torch_timeseries.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      240 2024-05-25 07:24:03.000000 torch_timeseries-0.0.1/torch_timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-25 07:24:03.000000 torch_timeseries-0.0.1/torch_timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2024-05-25 07:24:03.000000 torch_timeseries-0.0.1/torch_timeseries.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-25 07:24:03.000000 torch_timeseries-0.0.1/torch_timeseries.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:13:52.190559 torch_timeseries-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-24 14:44:45.000000 torch_timeseries-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    19635 2024-05-29 13:13:52.190559 torch_timeseries-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5720 2024-05-29 13:12:27.000000 torch_timeseries-0.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      741 2024-05-25 06:55:33.000000 torch_timeseries-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 13:13:52.190559 torch_timeseries-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-05-29 13:13:45.000000 torch_timeseries-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:13:52.182559 torch_timeseries-0.0.2/torch_timeseries/
+-rw-r--r--   0 root         (0) root         (0)       97 2024-05-26 18:31:12.000000 torch_timeseries-0.0.2/torch_timeseries/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:13:52.182559 torch_timeseries-0.0.2/torch_timeseries/dataloader/
+-rw-r--r--   0 root         (0) root         (0)      714 2024-05-29 04:27:55.000000 torch_timeseries-0.0.2/torch_timeseries/dataloader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5635 2024-05-29 04:25:33.000000 torch_timeseries-0.0.2/torch_timeseries/dataloader/anomaly.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2024-05-29 04:25:39.000000 torch_timeseries-0.0.2/torch_timeseries/dataloader/maskts.py
+-rw-r--r--   0 root         (0) root         (0)     5455 2024-05-29 04:26:02.000000 torch_timeseries-0.0.2/torch_timeseries/dataloader/sliding_window.py
+-rw-r--r--   0 root         (0) root         (0)     5954 2024-05-29 04:25:45.000000 torch_timeseries-0.0.2/torch_timeseries/dataloader/sliding_window_ts.py
+-rw-r--r--   0 root         (0) root         (0)     6950 2024-05-29 04:25:51.000000 torch_timeseries-0.0.2/torch_timeseries/dataloader/uea.py
+-rw-r--r--   0 root         (0) root         (0)     6550 2024-05-29 04:28:04.000000 torch_timeseries-0.0.2/torch_timeseries/dataloader/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:13:52.186559 torch_timeseries-0.0.2/torch_timeseries/dataset/
+-rw-r--r--   0 root         (0) root         (0)     1742 2024-05-27 05:33:15.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/ETTh1.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2024-05-27 05:33:19.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/ETTh2.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2024-05-27 05:33:29.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/ETTm1.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2024-05-27 05:33:34.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/ETTm2.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2024-05-27 03:23:05.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/Electricity.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-05-27 05:33:38.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/ExchangeRate.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2024-05-27 06:00:15.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/ILI.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2024-05-27 07:36:21.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/M4.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-05-29 11:08:47.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/MSL.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-05-29 11:08:47.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/PSM.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2024-05-29 11:08:47.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/SMAP.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-05-29 11:08:47.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/SMD.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2024-05-29 11:08:47.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/SWaT.py
+-rw-r--r--   0 root         (0) root         (0)     3445 2024-05-29 12:51:11.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/SolarEnergy.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-05-27 05:33:55.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/Traffic.py
+-rw-r--r--   0 root         (0) root         (0)     4741 2024-05-29 03:53:50.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/UEA.py
+-rw-r--r--   0 root         (0) root         (0)     1796 2024-05-27 05:48:34.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/Weather.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-05-28 14:34:45.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3025 2024-05-28 14:07:55.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:13:52.186559 torch_timeseries-0.0.2/torch_timeseries/dataset/dummies/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-27 05:40:35.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/dummies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-27 05:42:01.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/dummies/dummy.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2024-05-27 05:41:33.000000 torch_timeseries-0.0.2/torch_timeseries/dataset/dummies/dummy_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:13:52.186559 torch_timeseries-0.0.2/torch_timeseries/model/
+-rw-r--r--   0 root         (0) root         (0)     3685 2024-05-28 16:33:34.000000 torch_timeseries-0.0.2/torch_timeseries/model/DLinear.py
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-24 09:25:39.000000 torch_timeseries-0.0.2/torch_timeseries/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:13:52.186559 torch_timeseries-0.0.2/torch_timeseries/scaler/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-29 04:27:08.000000 torch_timeseries-0.0.2/torch_timeseries/scaler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2024-05-29 04:22:59.000000 torch_timeseries-0.0.2/torch_timeseries/scaler/base.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-05-29 04:24:45.000000 torch_timeseries-0.0.2/torch_timeseries/scaler/maxabs.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-05-29 04:24:36.000000 torch_timeseries-0.0.2/torch_timeseries/scaler/standard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 13:13:52.186559 torch_timeseries-0.0.2/torch_timeseries.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19635 2024-05-29 13:13:52.000000 torch_timeseries-0.0.2/torch_timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1556 2024-05-29 13:13:52.000000 torch_timeseries-0.0.2/torch_timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 13:13:52.000000 torch_timeseries-0.0.2/torch_timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2024-05-29 13:13:52.000000 torch_timeseries-0.0.2/torch_timeseries.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-29 13:13:52.000000 torch_timeseries-0.0.2/torch_timeseries.egg-info/top_level.txt
```

### Comparing `torch_timeseries-0.0.1/LICENSE` & `torch_timeseries-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.1/PKG-INFO` & `torch_timeseries-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: torch_timeseries
-Version: 0.0.1
+Version: 0.0.2
 Summary: Timeseries Learning Library for PyTorch.
 Home-page: https://github.com/wayne155/pytorch_timeseries
-Download-URL: https://github.com/wayne155/pytorch_timeseries/archive/0.0.1.tar.gz
+Download-URL: https://github.com/wayne155/pytorch_timeseries/archive/0.0.2.tar.gz
 Author: Weiwei Ye
 Author-email: Wayne Yip <wwye155@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,65 +224,204 @@
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: g
 Requires-Dist: pyg; extra == "g"
 
+[pypi-image]: https://badge.fury.io/py/torch-timeseries.svg
+[pypi-url]: https://pypi.python.org/pypi/torch-timeseries
+[docs-image]: https://readthedocs.org/projects/pytorch-timeseries/badge/?version=latest
+[docs-url]: https://pytorch-timeseries.readthedocs.io/en/latest/?badge=latest
+
+
+
+<p align="center">
+  <img width="90%" src="https://raw.githubusercontent.com/wayne155/pytorch_timeseries/main/docs/_static/img/logo_text.jpg?sanitize=true" />
+</p>
+
+[![PyPI Version][pypi-image]][pypi-url]
+[![Docs Status][docs-image]][docs-url]
+
+
+
+
+
+
 # pytorch_timeseries
 An all in one deep learning library that boost your timeseries research.
+[Check the documentation for more detail](https://pytorch-timeseries.readthedocs.io/en/latest/).
+
+Compared to previous libraries, pytorch_timeseries is 
+- dataset automatically downloaded
+- easy to use and extend 
+- clear documentation 
+- highly customizable 
+- ..........
+
+
 
 ## installation
+
+
+
+```
+pip install torch-timeseries
 ```
-pip install pytorch-timeseries
+
+> ⚠️⚠️⚠️ **Warning: We only support python version >= 3.8+**
+
+### addtional install
+For running Graph Nerual Network based models, pytorch_geometric is also needed.
+
+```python
+pip install torch_geometric
+
+# Optional dependencies
+pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.0.0+cu118.html
 ```
 
-## documentation
-See [Documentation](https://pytorch-timeseries.readthedocs.io/en/latest/).
 
 # Quick Start
 
+## 1 Forecasting
+
+### 1.1 download dataset
+The dataset will be downloaded **automatically!!!!**
 ```python
 from torch_timeseries.dataset import ETTh1
 from torch_timeseries.dataloader import StandardScaler, SlidingWindow, SlidingWindowTS
 from torch_timeseries.model import DLinear
 from torch.nn import MSELoss, L1Loss
 from torch.optim import Adam
 dataset = ETTh1('./data')
+```
+
+### 1.2 setup scaler/dataloader
+
+Once you setup a dataloader and pass a scaler into this dataloader, the scaler will be fitted on the training set.
+
+
+```python
 scaler = StandardScaler()
 dataloader = SlidingWindowTS(dataset, 
                         window=96,
                         horizon=1,
                         steps=336,
                         batch_size=32, 
                         train_ratio=0.7, 
                         val_ratio=0.2, 
                         scaler=scaler,
                         )
 
+```
+After this, you can access the train/val/test loader by `dataloader.train_loader/val_loader/test_loader` 
+
+### 1.3 training
+
 
-model = DLinear(dataloader.window, dataloader.steps, dataset.num_features, individual= True)
 
+```python
+model = DLinear(dataloader.window, dataloader.steps, dataset.num_features, individual= True)
 optimizer = Adam(model.parameters())
 loss_function = MSELoss()
 
+# train
+model.train()
+for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.train_loader:
+    optimizer.zero_grad()
+    
+    scaled_x = scaled_x.float()
+    scaled_y = scaled_y.float()
+    scaled_pred_y = model(scaled_x) 
+    
+    loss = loss_function(scaled_pred_y, scaled_y)
+    loss.backward()
+    optimizer.step()
+    print(loss)
+```
+
+### 1.4 val/test
+
+```python
+# val
+model.eval()
+for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.val_loader:
+    ....your validation code here...
+
+# test
+model.eval()
+for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.test_loader:
+    ....your test code here...
+```
+
+
+
+
+
+## 2 Imputation
+
+### 1. download dataset
+The dataset will be downloaded **automatically!!!!**
+```python
+from torch_timeseries.dataset import ETTh1
+from torch_timeseries.dataloader import StandardScaler, SlidingWindow, SlidingWindowTS
+from torch_timeseries.model import DLinear
+from torch.nn import MSELoss, L1Loss
+from torch.optim import Adam
+dataset = ETTh1('./data')
+```
+
+### 2. setup scaler/dataloader
+
+Once you setup a dataloader and pass a scaler into this dataloader, the scaler will be fitted on the training set.
+
+
+```python
+scaler = StandardScaler()
+dataloader = SlidingWindowTS(dataset, 
+                        window=96,
+                        horizon=1,
+                        steps=336,
+                        batch_size=32, 
+                        train_ratio=0.7, 
+                        val_ratio=0.2, 
+                        scaler=scaler,
+                        )
+
+```
+After this, you can access the train/val/test loader by `dataloader.train_loader/val_loader/test_loader` 
+
+### 3. training
+
+
+
+```python
+model = DLinear(dataloader.window, dataloader.steps, dataset.num_features, individual= True)
+optimizer = Adam(model.parameters())
+loss_function = MSELoss()
 
 # train
 model.train()
 for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.train_loader:
     optimizer.zero_grad()
     
     scaled_x = scaled_x.float()
     scaled_y = scaled_y.float()
     scaled_pred_y = model(scaled_x) 
     
     loss = loss_function(scaled_pred_y, scaled_y)
     loss.backward()
     optimizer.step()
     print(loss)
+```
+
+### 4. val/test
+
+```python
 # val
 model.eval()
 for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.val_loader:
     scaled_x = scaled_x.float()
     scaled_y = scaled_y.float()
     scaled_pred_y = model(scaled_x) 
     loss = loss_function(scaled_pred_y, scaled_y)
@@ -292,15 +431,14 @@
 model.eval()
 for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.test_loader:
     scaled_x = scaled_x.float()
     scaled_y = scaled_y.float()
     scaled_pred_y = model(scaled_x) 
     loss = loss_function(scaled_pred_y, scaled_y)
     
-
 ```
 
 
 
 # dev install 
 
 # install requirements
@@ -309,21 +447,9 @@
 
 **The recommended python version is 3.8.1+.**
 Please first install torch according to your environment.
 ```
 pip3 install torch torchvision torchaudio
 ```
 
-For running Graph Nerual Network based models, pytorch_geometric is also needed.
-
-```python
-pip install torch_geometric
 
-# Optional dependencies
-pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.0.0+cu118.html
-```
 
->check your torch & cuda version before you execute the command above
->```python
->python -c "import torch; print(torch.__version__)"
->python -c "import torch; print(torch.version.cuda)"
->```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torch_timeseries-0.0.1/pyproject.toml` & `torch_timeseries-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.1/setup.py` & `torch_timeseries-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 URL = 'https://github.com/wayne155/pytorch_timeseries'
 
 install_requires = [
     'tqdm',
 ]
 
 full_requires =  [
```

### Comparing `torch_timeseries-0.0.1/torch_timeseries.egg-info/PKG-INFO` & `torch_timeseries-0.0.2/torch_timeseries.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: torch_timeseries
-Version: 0.0.1
+Version: 0.0.2
 Summary: Timeseries Learning Library for PyTorch.
 Home-page: https://github.com/wayne155/pytorch_timeseries
-Download-URL: https://github.com/wayne155/pytorch_timeseries/archive/0.0.1.tar.gz
+Download-URL: https://github.com/wayne155/pytorch_timeseries/archive/0.0.2.tar.gz
 Author: Weiwei Ye
 Author-email: Wayne Yip <wwye155@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,65 +224,204 @@
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: g
 Requires-Dist: pyg; extra == "g"
 
+[pypi-image]: https://badge.fury.io/py/torch-timeseries.svg
+[pypi-url]: https://pypi.python.org/pypi/torch-timeseries
+[docs-image]: https://readthedocs.org/projects/pytorch-timeseries/badge/?version=latest
+[docs-url]: https://pytorch-timeseries.readthedocs.io/en/latest/?badge=latest
+
+
+
+<p align="center">
+  <img width="90%" src="https://raw.githubusercontent.com/wayne155/pytorch_timeseries/main/docs/_static/img/logo_text.jpg?sanitize=true" />
+</p>
+
+[![PyPI Version][pypi-image]][pypi-url]
+[![Docs Status][docs-image]][docs-url]
+
+
+
+
+
+
 # pytorch_timeseries
 An all in one deep learning library that boost your timeseries research.
+[Check the documentation for more detail](https://pytorch-timeseries.readthedocs.io/en/latest/).
+
+Compared to previous libraries, pytorch_timeseries is 
+- dataset automatically downloaded
+- easy to use and extend 
+- clear documentation 
+- highly customizable 
+- ..........
+
+
 
 ## installation
+
+
+
+```
+pip install torch-timeseries
 ```
-pip install pytorch-timeseries
+
+> ⚠️⚠️⚠️ **Warning: We only support python version >= 3.8+**
+
+### addtional install
+For running Graph Nerual Network based models, pytorch_geometric is also needed.
+
+```python
+pip install torch_geometric
+
+# Optional dependencies
+pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.0.0+cu118.html
 ```
 
-## documentation
-See [Documentation](https://pytorch-timeseries.readthedocs.io/en/latest/).
 
 # Quick Start
 
+## 1 Forecasting
+
+### 1.1 download dataset
+The dataset will be downloaded **automatically!!!!**
 ```python
 from torch_timeseries.dataset import ETTh1
 from torch_timeseries.dataloader import StandardScaler, SlidingWindow, SlidingWindowTS
 from torch_timeseries.model import DLinear
 from torch.nn import MSELoss, L1Loss
 from torch.optim import Adam
 dataset = ETTh1('./data')
+```
+
+### 1.2 setup scaler/dataloader
+
+Once you setup a dataloader and pass a scaler into this dataloader, the scaler will be fitted on the training set.
+
+
+```python
 scaler = StandardScaler()
 dataloader = SlidingWindowTS(dataset, 
                         window=96,
                         horizon=1,
                         steps=336,
                         batch_size=32, 
                         train_ratio=0.7, 
                         val_ratio=0.2, 
                         scaler=scaler,
                         )
 
+```
+After this, you can access the train/val/test loader by `dataloader.train_loader/val_loader/test_loader` 
+
+### 1.3 training
+
 
-model = DLinear(dataloader.window, dataloader.steps, dataset.num_features, individual= True)
 
+```python
+model = DLinear(dataloader.window, dataloader.steps, dataset.num_features, individual= True)
 optimizer = Adam(model.parameters())
 loss_function = MSELoss()
 
+# train
+model.train()
+for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.train_loader:
+    optimizer.zero_grad()
+    
+    scaled_x = scaled_x.float()
+    scaled_y = scaled_y.float()
+    scaled_pred_y = model(scaled_x) 
+    
+    loss = loss_function(scaled_pred_y, scaled_y)
+    loss.backward()
+    optimizer.step()
+    print(loss)
+```
+
+### 1.4 val/test
+
+```python
+# val
+model.eval()
+for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.val_loader:
+    ....your validation code here...
+
+# test
+model.eval()
+for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.test_loader:
+    ....your test code here...
+```
+
+
+
+
+
+## 2 Imputation
+
+### 1. download dataset
+The dataset will be downloaded **automatically!!!!**
+```python
+from torch_timeseries.dataset import ETTh1
+from torch_timeseries.dataloader import StandardScaler, SlidingWindow, SlidingWindowTS
+from torch_timeseries.model import DLinear
+from torch.nn import MSELoss, L1Loss
+from torch.optim import Adam
+dataset = ETTh1('./data')
+```
+
+### 2. setup scaler/dataloader
+
+Once you setup a dataloader and pass a scaler into this dataloader, the scaler will be fitted on the training set.
+
+
+```python
+scaler = StandardScaler()
+dataloader = SlidingWindowTS(dataset, 
+                        window=96,
+                        horizon=1,
+                        steps=336,
+                        batch_size=32, 
+                        train_ratio=0.7, 
+                        val_ratio=0.2, 
+                        scaler=scaler,
+                        )
+
+```
+After this, you can access the train/val/test loader by `dataloader.train_loader/val_loader/test_loader` 
+
+### 3. training
+
+
+
+```python
+model = DLinear(dataloader.window, dataloader.steps, dataset.num_features, individual= True)
+optimizer = Adam(model.parameters())
+loss_function = MSELoss()
 
 # train
 model.train()
 for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.train_loader:
     optimizer.zero_grad()
     
     scaled_x = scaled_x.float()
     scaled_y = scaled_y.float()
     scaled_pred_y = model(scaled_x) 
     
     loss = loss_function(scaled_pred_y, scaled_y)
     loss.backward()
     optimizer.step()
     print(loss)
+```
+
+### 4. val/test
+
+```python
 # val
 model.eval()
 for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.val_loader:
     scaled_x = scaled_x.float()
     scaled_y = scaled_y.float()
     scaled_pred_y = model(scaled_x) 
     loss = loss_function(scaled_pred_y, scaled_y)
@@ -292,15 +431,14 @@
 model.eval()
 for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.test_loader:
     scaled_x = scaled_x.float()
     scaled_y = scaled_y.float()
     scaled_pred_y = model(scaled_x) 
     loss = loss_function(scaled_pred_y, scaled_y)
     
-
 ```
 
 
 
 # dev install 
 
 # install requirements
@@ -309,21 +447,9 @@
 
 **The recommended python version is 3.8.1+.**
 Please first install torch according to your environment.
 ```
 pip3 install torch torchvision torchaudio
 ```
 
-For running Graph Nerual Network based models, pytorch_geometric is also needed.
-
-```python
-pip install torch_geometric
 
-# Optional dependencies
-pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.0.0+cu118.html
-```
 
->check your torch & cuda version before you execute the command above
->```python
->python -c "import torch; print(torch.__version__)"
->python -c "import torch; print(torch.version.cuda)"
->```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

