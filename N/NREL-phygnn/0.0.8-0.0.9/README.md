# Comparing `tmp/NREL-phygnn-0.0.8.tar.gz` & `tmp/NREL-phygnn-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NREL-phygnn-0.0.8.tar", last modified: Wed Feb  3 16:09:03 2021, max compression
+gzip compressed data, was "NREL-phygnn-0.0.9.tar", last modified: Wed Feb  3 17:05:03 2021, max compression
```

## Comparing `NREL-phygnn-0.0.8.tar` & `NREL-phygnn-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 16:09:03.858739 NREL-phygnn-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 16:09:03.854739 NREL-phygnn-0.0.8/NREL_phygnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (117)     8851 2021-02-03 16:09:03.000000 NREL-phygnn-0.0.8/NREL_phygnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (117)      638 2021-02-03 16:09:03.000000 NREL-phygnn-0.0.8/NREL_phygnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (117)        1 2021-02-03 16:09:03.000000 NREL-phygnn-0.0.8/NREL_phygnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (117)        1 2021-02-03 16:09:03.000000 NREL-phygnn-0.0.8/NREL_phygnn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (117)      124 2021-02-03 16:09:03.000000 NREL-phygnn-0.0.8/NREL_phygnn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (117)        7 2021-02-03 16:09:03.000000 NREL-phygnn-0.0.8/NREL_phygnn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (117)     8851 2021-02-03 16:09:03.858739 NREL-phygnn-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (117)     7266 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 16:09:03.854739 NREL-phygnn-0.0.8/phygnn/
--rw-r--r--   0 runner    (1001) docker     (117)      459 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/phygnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 16:09:03.858739 NREL-phygnn-0.0.8/phygnn/model_interfaces/
--rw-r--r--   0 runner    (1001) docker     (117)      166 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/phygnn/model_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (117)    28920 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/phygnn/model_interfaces/base_model.py
--rw-r--r--   0 runner    (1001) docker     (117)    24258 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/phygnn/model_interfaces/phygnn_model.py
--rw-r--r--   0 runner    (1001) docker     (117)     9729 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/phygnn/model_interfaces/random_forest_model.py
--rw-r--r--   0 runner    (1001) docker     (117)    22338 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/phygnn/model_interfaces/tf_model.py
--rw-r--r--   0 runner    (1001) docker     (117)    35317 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/phygnn/phygnn.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 16:09:03.858739 NREL-phygnn-0.0.8/phygnn/utilities/
--rw-r--r--   0 runner    (1001) docker     (117)      167 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/phygnn/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (117)     2236 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/phygnn/utilities/loss_metrics.py
--rw-r--r--   0 runner    (1001) docker     (117)    17540 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/phygnn/utilities/pre_processing.py
--rw-r--r--   0 runner    (1001) docker     (117)    12634 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/phygnn/utilities/tf_layers.py
--rw-r--r--   0 runner    (1001) docker     (117)      504 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/phygnn/utilities/tf_utilities.py
--rw-r--r--   0 runner    (1001) docker     (117)       92 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/phygnn/version.py
--rw-r--r--   0 runner    (1001) docker     (117)       38 2021-02-03 16:09:03.858739 NREL-phygnn-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (117)     2105 2021-02-03 16:08:54.000000 NREL-phygnn-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 17:05:03.453420 NREL-phygnn-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 17:05:03.449420 NREL-phygnn-0.0.9/NREL_phygnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (117)     8844 2021-02-03 17:05:03.000000 NREL-phygnn-0.0.9/NREL_phygnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (117)      638 2021-02-03 17:05:03.000000 NREL-phygnn-0.0.9/NREL_phygnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (117)        1 2021-02-03 17:05:03.000000 NREL-phygnn-0.0.9/NREL_phygnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (117)        1 2021-02-03 17:05:03.000000 NREL-phygnn-0.0.9/NREL_phygnn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (117)      124 2021-02-03 17:05:03.000000 NREL-phygnn-0.0.9/NREL_phygnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (117)        7 2021-02-03 17:05:03.000000 NREL-phygnn-0.0.9/NREL_phygnn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (117)     8844 2021-02-03 17:05:03.453420 NREL-phygnn-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (117)     7235 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 17:05:03.449420 NREL-phygnn-0.0.9/phygnn/
+-rw-r--r--   0 runner    (1001) docker     (117)      459 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/phygnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 17:05:03.449420 NREL-phygnn-0.0.9/phygnn/model_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (117)      166 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/phygnn/model_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (117)    28920 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/phygnn/model_interfaces/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (117)    24258 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/phygnn/model_interfaces/phygnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (117)     9729 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/phygnn/model_interfaces/random_forest_model.py
+-rw-r--r--   0 runner    (1001) docker     (117)    22338 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/phygnn/model_interfaces/tf_model.py
+-rw-r--r--   0 runner    (1001) docker     (117)    35317 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/phygnn/phygnn.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 17:05:03.453420 NREL-phygnn-0.0.9/phygnn/utilities/
+-rw-r--r--   0 runner    (1001) docker     (117)      167 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/phygnn/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (117)     2236 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/phygnn/utilities/loss_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (117)    17540 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/phygnn/utilities/pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (117)    12634 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/phygnn/utilities/tf_layers.py
+-rw-r--r--   0 runner    (1001) docker     (117)      504 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/phygnn/utilities/tf_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (117)       92 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/phygnn/version.py
+-rw-r--r--   0 runner    (1001) docker     (117)       38 2021-02-03 17:05:03.453420 NREL-phygnn-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (117)     2105 2021-02-03 17:04:54.000000 NREL-phygnn-0.0.9/setup.py
```

### Comparing `NREL-phygnn-0.0.8/NREL_phygnn.egg-info/PKG-INFO` & `NREL-phygnn-0.0.9/NREL_phygnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-phygnn
-Version: 0.0.8
+Version: 0.0.9
 Summary: Physics-Guided Neural Networks (phygnn)
 Home-page: https://github.com/NREL/phygnn
 Author: Grant Buster
 Author-email: grant.buster@nrel.gov
 License: BSD 3-Clause
 Description: ######
         phygnn
@@ -46,17 +46,17 @@
         integrate machine learning models into physics and engineering applications.
         This framework should help alleviate some challenges that are often encountered
         when applying purely data-driven machine learning models to scientific
         applications, such as when machine learning models produce physically
         inconsistent results or have trouble generalizing to out-of-sample scenarios.
         
         For details on the phygnn class framework see `the phygnn module documentation
-        here. <https://nrel.github.io/phygnn/phygnn/phygnn.phygnn.html>`_ 
+        here. <https://nrel.github.io/phygnn/phygnn/phygnn.phygnn.html>`_
         
-        For example notebooks using the phygnn architecture for regression, 
+        For example notebooks using the phygnn architecture for regression,
         classification, and even GAN applications, see `the example notebooks here.
         <https://github.com/NREL/phygnn/tree/master/examples>`_
         
         At the National Renewable Energy Lab (NREL), we are using the phygnn framework
         to supplement traditional satellite-based cloud property prediction models. We
         use phygnn to predict cloud optical properties when the traditional mechanistic
         models fail and use a full tensor-based radiative transfer model as the
@@ -79,17 +79,20 @@
             * Jared Willard, Xiaowei Jia, Shaoming Xu, Michael Steinbach, and Vipin Kumar, “Integrating Physics-Based Modeling with Machine Learning: A Survey.” ArXiv abs/2003.04919 (2020).
             * Forssell, U. and P. Lindskog. “Combining Semi-Physical and Neural Network Modeling: An Example ofIts Usefulness.” IFAC Proceedings Volumes 30 (1997): 767-770.
             * Xinyue Hu, Haoji Hu, Saurabh Verma, and Zhi-Li Zhang, “Physics-Guided Deep Neural Networks for PowerFlow Analysis”, arXiv:2002.00097v1 (2020).
             * Anuj Karpatne, William Watkins, Jordan Read, and Vipin Kumar, "Physics-guided Neural Networks (PGNN): An Application in Lake Temperature Modeling". arXiv:1710.11431v2 (2018).
             * Anuj Karpatne, Gowtham Atluri, James H Faghmous, Michael Steinbach, Arindam Banerjee, Auroop Ganguly, Shashi Shekhar, Nagiza Samatova, and Vipin Kumar. 2017. Theory-guided data science: A new paradigm for scientific discovery from data. IEEE Transactions on knowledge and data engineering 29, 10 (2017), 2318–2331.
             * Justin Sirignano, Jonathan F. MacArt, Jonathan B. Freund, "DPM: A deep learning PDE augmentation method with application to large-eddy simulation". Journal of Computational Physics, Volume 423, 2020, ISSN 0021-9991, https://doi.org/10.1016/j.jcp.2020.109811.
         
-        Suggested citation if you use the phygnn architecture:
+        Suggested Citation
+        ==================
+        
+        
+        Buster G, Rossol M, Bannister M, and Hettinger D, “physics-guided neural networks (phygnn).” GitHub. https://github.com/NREL/phygnn. Version 0.0.7. Accessed 14 January 2021
         
-            * Buster G, Rossol M, Bannister M, and Hettinger D, “physics-guided neural networks (phygnn).” GitHub. https://github.com/NREL/phygnn. Version 0.0.7. Accessed 14 January 2021
         
         Installation
         ============
         
         
         Simple Install
         --------------
@@ -113,16 +116,16 @@
         3. Clone the phygnn repository: ``git clone https://github.com/NREL/phygnn.git`` or ``git clone git@github.com:NREL/phygnn.git``
         4. Navigate to the cloned repo and checkout your desired branch: ``git checkout master`` or ``git checkout <branch>``
         5. Navigate to the phygnn directory that contains setup.py and run: ``pip install -e .`` (developer install) or ``pip install .`` (static install).
         6. Test your installation:
         
             i. Start ipython and test the following import: ``from phygnn import PhysicsGuidedNeuralNetwork``
             ii. Navigate to the ``tests/`` directory and run the command: ``pytest``
-            
-            
+        
+        
         Acknowledgements
         ================
         This work was authored by the National Renewable Energy Laboratory, operated by Alliance for Sustainable Energy,
         LLC, for the U.S. Department of Energy (DOE) under Contract No. DE-AC36-08GO28308. This material is based upon
         work supported by the U.S. Department of Energy’s Office of Energy Efficiency and Renewable Energy (EERE) under
         the Solar Energy Technologies Office (Systems Integration Subprogram) Contract Number 36598. The views
         expressed in the article do not necessarily represent the views of the DOE or the U.S. Government. The U.S.
```

### Comparing `NREL-phygnn-0.0.8/NREL_phygnn.egg-info/SOURCES.txt` & `NREL-phygnn-0.0.9/NREL_phygnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NREL-phygnn-0.0.8/PKG-INFO` & `NREL-phygnn-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-phygnn
-Version: 0.0.8
+Version: 0.0.9
 Summary: Physics-Guided Neural Networks (phygnn)
 Home-page: https://github.com/NREL/phygnn
 Author: Grant Buster
 Author-email: grant.buster@nrel.gov
 License: BSD 3-Clause
 Description: ######
         phygnn
@@ -46,17 +46,17 @@
         integrate machine learning models into physics and engineering applications.
         This framework should help alleviate some challenges that are often encountered
         when applying purely data-driven machine learning models to scientific
         applications, such as when machine learning models produce physically
         inconsistent results or have trouble generalizing to out-of-sample scenarios.
         
         For details on the phygnn class framework see `the phygnn module documentation
-        here. <https://nrel.github.io/phygnn/phygnn/phygnn.phygnn.html>`_ 
+        here. <https://nrel.github.io/phygnn/phygnn/phygnn.phygnn.html>`_
         
-        For example notebooks using the phygnn architecture for regression, 
+        For example notebooks using the phygnn architecture for regression,
         classification, and even GAN applications, see `the example notebooks here.
         <https://github.com/NREL/phygnn/tree/master/examples>`_
         
         At the National Renewable Energy Lab (NREL), we are using the phygnn framework
         to supplement traditional satellite-based cloud property prediction models. We
         use phygnn to predict cloud optical properties when the traditional mechanistic
         models fail and use a full tensor-based radiative transfer model as the
@@ -79,17 +79,20 @@
             * Jared Willard, Xiaowei Jia, Shaoming Xu, Michael Steinbach, and Vipin Kumar, “Integrating Physics-Based Modeling with Machine Learning: A Survey.” ArXiv abs/2003.04919 (2020).
             * Forssell, U. and P. Lindskog. “Combining Semi-Physical and Neural Network Modeling: An Example ofIts Usefulness.” IFAC Proceedings Volumes 30 (1997): 767-770.
             * Xinyue Hu, Haoji Hu, Saurabh Verma, and Zhi-Li Zhang, “Physics-Guided Deep Neural Networks for PowerFlow Analysis”, arXiv:2002.00097v1 (2020).
             * Anuj Karpatne, William Watkins, Jordan Read, and Vipin Kumar, "Physics-guided Neural Networks (PGNN): An Application in Lake Temperature Modeling". arXiv:1710.11431v2 (2018).
             * Anuj Karpatne, Gowtham Atluri, James H Faghmous, Michael Steinbach, Arindam Banerjee, Auroop Ganguly, Shashi Shekhar, Nagiza Samatova, and Vipin Kumar. 2017. Theory-guided data science: A new paradigm for scientific discovery from data. IEEE Transactions on knowledge and data engineering 29, 10 (2017), 2318–2331.
             * Justin Sirignano, Jonathan F. MacArt, Jonathan B. Freund, "DPM: A deep learning PDE augmentation method with application to large-eddy simulation". Journal of Computational Physics, Volume 423, 2020, ISSN 0021-9991, https://doi.org/10.1016/j.jcp.2020.109811.
         
-        Suggested citation if you use the phygnn architecture:
+        Suggested Citation
+        ==================
+        
+        
+        Buster G, Rossol M, Bannister M, and Hettinger D, “physics-guided neural networks (phygnn).” GitHub. https://github.com/NREL/phygnn. Version 0.0.7. Accessed 14 January 2021
         
-            * Buster G, Rossol M, Bannister M, and Hettinger D, “physics-guided neural networks (phygnn).” GitHub. https://github.com/NREL/phygnn. Version 0.0.7. Accessed 14 January 2021
         
         Installation
         ============
         
         
         Simple Install
         --------------
@@ -113,16 +116,16 @@
         3. Clone the phygnn repository: ``git clone https://github.com/NREL/phygnn.git`` or ``git clone git@github.com:NREL/phygnn.git``
         4. Navigate to the cloned repo and checkout your desired branch: ``git checkout master`` or ``git checkout <branch>``
         5. Navigate to the phygnn directory that contains setup.py and run: ``pip install -e .`` (developer install) or ``pip install .`` (static install).
         6. Test your installation:
         
             i. Start ipython and test the following import: ``from phygnn import PhysicsGuidedNeuralNetwork``
             ii. Navigate to the ``tests/`` directory and run the command: ``pytest``
-            
-            
+        
+        
         Acknowledgements
         ================
         This work was authored by the National Renewable Energy Laboratory, operated by Alliance for Sustainable Energy,
         LLC, for the U.S. Department of Energy (DOE) under Contract No. DE-AC36-08GO28308. This material is based upon
         work supported by the U.S. Department of Energy’s Office of Energy Efficiency and Renewable Energy (EERE) under
         the Solar Energy Technologies Office (Systems Integration Subprogram) Contract Number 36598. The views
         expressed in the article do not necessarily represent the views of the DOE or the U.S. Government. The U.S.
```

### Comparing `NREL-phygnn-0.0.8/README.rst` & `NREL-phygnn-0.0.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 integrate machine learning models into physics and engineering applications.
 This framework should help alleviate some challenges that are often encountered
 when applying purely data-driven machine learning models to scientific
 applications, such as when machine learning models produce physically
 inconsistent results or have trouble generalizing to out-of-sample scenarios.
 
 For details on the phygnn class framework see `the phygnn module documentation
-here. <https://nrel.github.io/phygnn/phygnn/phygnn.phygnn.html>`_ 
+here. <https://nrel.github.io/phygnn/phygnn/phygnn.phygnn.html>`_
 
-For example notebooks using the phygnn architecture for regression, 
+For example notebooks using the phygnn architecture for regression,
 classification, and even GAN applications, see `the example notebooks here.
 <https://github.com/NREL/phygnn/tree/master/examples>`_
 
 At the National Renewable Energy Lab (NREL), we are using the phygnn framework
 to supplement traditional satellite-based cloud property prediction models. We
 use phygnn to predict cloud optical properties when the traditional mechanistic
 models fail and use a full tensor-based radiative transfer model as the
@@ -71,17 +71,20 @@
     * Jared Willard, Xiaowei Jia, Shaoming Xu, Michael Steinbach, and Vipin Kumar, “Integrating Physics-Based Modeling with Machine Learning: A Survey.” ArXiv abs/2003.04919 (2020).
     * Forssell, U. and P. Lindskog. “Combining Semi-Physical and Neural Network Modeling: An Example ofIts Usefulness.” IFAC Proceedings Volumes 30 (1997): 767-770.
     * Xinyue Hu, Haoji Hu, Saurabh Verma, and Zhi-Li Zhang, “Physics-Guided Deep Neural Networks for PowerFlow Analysis”, arXiv:2002.00097v1 (2020).
     * Anuj Karpatne, William Watkins, Jordan Read, and Vipin Kumar, "Physics-guided Neural Networks (PGNN): An Application in Lake Temperature Modeling". arXiv:1710.11431v2 (2018).
     * Anuj Karpatne, Gowtham Atluri, James H Faghmous, Michael Steinbach, Arindam Banerjee, Auroop Ganguly, Shashi Shekhar, Nagiza Samatova, and Vipin Kumar. 2017. Theory-guided data science: A new paradigm for scientific discovery from data. IEEE Transactions on knowledge and data engineering 29, 10 (2017), 2318–2331.
     * Justin Sirignano, Jonathan F. MacArt, Jonathan B. Freund, "DPM: A deep learning PDE augmentation method with application to large-eddy simulation". Journal of Computational Physics, Volume 423, 2020, ISSN 0021-9991, https://doi.org/10.1016/j.jcp.2020.109811.
 
-Suggested citation if you use the phygnn architecture:
+Suggested Citation
+==================
+
+
+Buster G, Rossol M, Bannister M, and Hettinger D, “physics-guided neural networks (phygnn).” GitHub. https://github.com/NREL/phygnn. Version 0.0.7. Accessed 14 January 2021
 
-    * Buster G, Rossol M, Bannister M, and Hettinger D, “physics-guided neural networks (phygnn).” GitHub. https://github.com/NREL/phygnn. Version 0.0.7. Accessed 14 January 2021
 
 Installation
 ============
 
 
 Simple Install
 --------------
@@ -105,16 +108,16 @@
 3. Clone the phygnn repository: ``git clone https://github.com/NREL/phygnn.git`` or ``git clone git@github.com:NREL/phygnn.git``
 4. Navigate to the cloned repo and checkout your desired branch: ``git checkout master`` or ``git checkout <branch>``
 5. Navigate to the phygnn directory that contains setup.py and run: ``pip install -e .`` (developer install) or ``pip install .`` (static install).
 6. Test your installation:
 
     i. Start ipython and test the following import: ``from phygnn import PhysicsGuidedNeuralNetwork``
     ii. Navigate to the ``tests/`` directory and run the command: ``pytest``
-    
-    
+
+
 Acknowledgements
 ================
 This work was authored by the National Renewable Energy Laboratory, operated by Alliance for Sustainable Energy,
 LLC, for the U.S. Department of Energy (DOE) under Contract No. DE-AC36-08GO28308. This material is based upon
 work supported by the U.S. Department of Energy’s Office of Energy Efficiency and Renewable Energy (EERE) under
 the Solar Energy Technologies Office (Systems Integration Subprogram) Contract Number 36598. The views
 expressed in the article do not necessarily represent the views of the DOE or the U.S. Government. The U.S.
```

### Comparing `NREL-phygnn-0.0.8/phygnn/model_interfaces/base_model.py` & `NREL-phygnn-0.0.9/phygnn/model_interfaces/base_model.py`

 * *Files identical despite different names*

### Comparing `NREL-phygnn-0.0.8/phygnn/model_interfaces/phygnn_model.py` & `NREL-phygnn-0.0.9/phygnn/model_interfaces/phygnn_model.py`

 * *Files identical despite different names*

### Comparing `NREL-phygnn-0.0.8/phygnn/model_interfaces/random_forest_model.py` & `NREL-phygnn-0.0.9/phygnn/model_interfaces/random_forest_model.py`

 * *Files identical despite different names*

### Comparing `NREL-phygnn-0.0.8/phygnn/model_interfaces/tf_model.py` & `NREL-phygnn-0.0.9/phygnn/model_interfaces/tf_model.py`

 * *Files identical despite different names*

### Comparing `NREL-phygnn-0.0.8/phygnn/phygnn.py` & `NREL-phygnn-0.0.9/phygnn/phygnn.py`

 * *Files identical despite different names*

### Comparing `NREL-phygnn-0.0.8/phygnn/utilities/loss_metrics.py` & `NREL-phygnn-0.0.9/phygnn/utilities/loss_metrics.py`

 * *Files identical despite different names*

### Comparing `NREL-phygnn-0.0.8/phygnn/utilities/pre_processing.py` & `NREL-phygnn-0.0.9/phygnn/utilities/pre_processing.py`

 * *Files identical despite different names*

### Comparing `NREL-phygnn-0.0.8/phygnn/utilities/tf_layers.py` & `NREL-phygnn-0.0.9/phygnn/utilities/tf_layers.py`

 * *Files identical despite different names*

### Comparing `NREL-phygnn-0.0.8/setup.py` & `NREL-phygnn-0.0.9/setup.py`

 * *Files identical despite different names*

