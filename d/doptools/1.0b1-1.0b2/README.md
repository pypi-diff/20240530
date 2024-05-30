# Comparing `tmp/doptools-1.0b1.tar.gz` & `tmp/doptools-1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doptools-1.0b1.tar", last modified: Wed May 29 08:37:08 2024, max compression
+gzip compressed data, was "doptools-1.0b2.tar", last modified: Thu May 30 05:59:13 2024, max compression
```

## Comparing `doptools-1.0b1.tar` & `doptools-1.0b2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-05-29 08:37:08.147767 doptools-1.0b1/
--rw-r--r--   0 pavel      (501) staff       (20)    35149 2021-08-10 08:31:41.000000 doptools-1.0b1/LICENSE
--rw-r--r--   0 pavel      (501) staff       (20)     7235 2024-05-29 08:37:08.147645 doptools-1.0b1/PKG-INFO
--rw-r--r--   0 pavel      (501) staff       (20)     6246 2024-05-29 06:04:08.000000 doptools-1.0b1/README.rst
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-05-29 08:37:08.145576 doptools-1.0b1/doptools/
--rw-r--r--   0 pavel      (501) staff       (20)      806 2024-05-29 04:43:26.000000 doptools-1.0b1/doptools/__init__.py
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-05-29 08:37:08.146737 doptools-1.0b1/doptools/chem/
--rw-r--r--   0 pavel      (501) staff       (20)      884 2024-05-28 15:17:04.000000 doptools-1.0b1/doptools/chem/__init__.py
--rw-r--r--   0 pavel      (501) staff       (20)    31909 2024-05-29 08:27:05.000000 doptools-1.0b1/doptools/chem/chem_features.py
--rw-r--r--   0 pavel      (501) staff       (20)    12065 2024-05-28 15:23:00.000000 doptools-1.0b1/doptools/chem/coloratom.py
--rw-r--r--   0 pavel      (501) staff       (20)    11321 2024-05-28 15:28:36.000000 doptools-1.0b1/doptools/chem/solvents.py
--rw-r--r--   0 pavel      (501) staff       (20)     4386 2024-05-28 05:59:47.000000 doptools-1.0b1/doptools/chem/utils.py
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-05-29 08:37:08.147483 doptools-1.0b1/doptools/optimizer/
--rw-r--r--   0 pavel      (501) staff       (20)      904 2024-05-28 15:19:56.000000 doptools-1.0b1/doptools/optimizer/__init__.py
--rw-r--r--   0 pavel      (501) staff       (20)     5717 2024-05-14 09:18:26.000000 doptools-1.0b1/doptools/optimizer/config.py
--rw-r--r--   0 pavel      (501) staff       (20)    12342 2024-05-29 04:19:01.000000 doptools-1.0b1/doptools/optimizer/optimizer.py
--rw-r--r--   0 pavel      (501) staff       (20)     3011 2024-05-29 04:09:02.000000 doptools-1.0b1/doptools/optimizer/plotter.py
--rw-r--r--   0 pavel      (501) staff       (20)    18306 2024-05-29 04:19:55.000000 doptools-1.0b1/doptools/optimizer/preparer.py
--rw-r--r--   0 pavel      (501) staff       (20)     3965 2024-05-29 04:18:47.000000 doptools-1.0b1/doptools/optimizer/rebuilder.py
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-05-29 08:37:08.146110 doptools-1.0b1/doptools.egg-info/
--rw-r--r--   0 pavel      (501) staff       (20)     7235 2024-05-29 08:37:08.000000 doptools-1.0b1/doptools.egg-info/PKG-INFO
--rw-r--r--   0 pavel      (501) staff       (20)      525 2024-05-29 08:37:08.000000 doptools-1.0b1/doptools.egg-info/SOURCES.txt
--rw-r--r--   0 pavel      (501) staff       (20)        1 2024-05-29 08:37:08.000000 doptools-1.0b1/doptools.egg-info/dependency_links.txt
--rw-r--r--   0 pavel      (501) staff       (20)      176 2024-05-29 08:37:08.000000 doptools-1.0b1/doptools.egg-info/requires.txt
--rw-r--r--   0 pavel      (501) staff       (20)        9 2024-05-29 08:37:08.000000 doptools-1.0b1/doptools.egg-info/top_level.txt
--rw-r--r--   0 pavel      (501) staff       (20)       38 2024-05-29 08:37:08.147811 doptools-1.0b1/setup.cfg
--rw-r--r--   0 pavel      (501) staff       (20)     2573 2024-05-29 08:36:37.000000 doptools-1.0b1/setup.py
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-05-30 05:59:13.584205 doptools-1.0b2/
+-rw-r--r--   0 pavel      (501) staff       (20)    35149 2021-08-10 08:31:41.000000 doptools-1.0b2/LICENSE
+-rw-r--r--   0 pavel      (501) staff       (20)     7334 2024-05-30 05:59:13.584084 doptools-1.0b2/PKG-INFO
+-rw-r--r--   0 pavel      (501) staff       (20)     6345 2024-05-30 05:56:59.000000 doptools-1.0b2/README.rst
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-05-30 05:59:13.582061 doptools-1.0b2/doptools/
+-rw-r--r--   0 pavel      (501) staff       (20)      806 2024-05-29 04:43:26.000000 doptools-1.0b2/doptools/__init__.py
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-05-30 05:59:13.583288 doptools-1.0b2/doptools/chem/
+-rw-r--r--   0 pavel      (501) staff       (20)      884 2024-05-28 15:17:04.000000 doptools-1.0b2/doptools/chem/__init__.py
+-rw-r--r--   0 pavel      (501) staff       (20)    31914 2024-05-30 05:52:54.000000 doptools-1.0b2/doptools/chem/chem_features.py
+-rw-r--r--   0 pavel      (501) staff       (20)    12065 2024-05-28 15:23:00.000000 doptools-1.0b2/doptools/chem/coloratom.py
+-rw-r--r--   0 pavel      (501) staff       (20)    11321 2024-05-28 15:28:36.000000 doptools-1.0b2/doptools/chem/solvents.py
+-rw-r--r--   0 pavel      (501) staff       (20)     4386 2024-05-28 05:59:47.000000 doptools-1.0b2/doptools/chem/utils.py
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-05-30 05:59:13.583934 doptools-1.0b2/doptools/optimizer/
+-rw-r--r--   0 pavel      (501) staff       (20)      904 2024-05-28 15:19:56.000000 doptools-1.0b2/doptools/optimizer/__init__.py
+-rw-r--r--   0 pavel      (501) staff       (20)     5717 2024-05-14 09:18:26.000000 doptools-1.0b2/doptools/optimizer/config.py
+-rw-r--r--   0 pavel      (501) staff       (20)    12342 2024-05-29 04:19:01.000000 doptools-1.0b2/doptools/optimizer/optimizer.py
+-rw-r--r--   0 pavel      (501) staff       (20)     3011 2024-05-29 04:09:02.000000 doptools-1.0b2/doptools/optimizer/plotter.py
+-rw-r--r--   0 pavel      (501) staff       (20)    18692 2024-05-30 05:47:49.000000 doptools-1.0b2/doptools/optimizer/preparer.py
+-rw-r--r--   0 pavel      (501) staff       (20)     3965 2024-05-29 04:18:47.000000 doptools-1.0b2/doptools/optimizer/rebuilder.py
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-05-30 05:59:13.582639 doptools-1.0b2/doptools.egg-info/
+-rw-r--r--   0 pavel      (501) staff       (20)     7334 2024-05-30 05:59:13.000000 doptools-1.0b2/doptools.egg-info/PKG-INFO
+-rw-r--r--   0 pavel      (501) staff       (20)      525 2024-05-30 05:59:13.000000 doptools-1.0b2/doptools.egg-info/SOURCES.txt
+-rw-r--r--   0 pavel      (501) staff       (20)        1 2024-05-30 05:59:13.000000 doptools-1.0b2/doptools.egg-info/dependency_links.txt
+-rw-r--r--   0 pavel      (501) staff       (20)      176 2024-05-30 05:59:13.000000 doptools-1.0b2/doptools.egg-info/requires.txt
+-rw-r--r--   0 pavel      (501) staff       (20)        9 2024-05-30 05:59:13.000000 doptools-1.0b2/doptools.egg-info/top_level.txt
+-rw-r--r--   0 pavel      (501) staff       (20)       38 2024-05-30 05:59:13.584240 doptools-1.0b2/setup.cfg
+-rw-r--r--   0 pavel      (501) staff       (20)     2573 2024-05-30 05:56:06.000000 doptools-1.0b2/setup.py
```

### Comparing `doptools-1.0b1/LICENSE` & `doptools-1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `doptools-1.0b1/PKG-INFO` & `doptools-1.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doptools
-Version: 1.0b1
+Version: 1.0b2
 Summary: A package for calculation of molecular descriptors in Scikit-Learn compatible way and model optimization
 Home-page: https://github.com/POSidorov/DOPtools
 Author: Dr. Pavel Sidorov
 Author-email: pavel.o.sidorov@gmail.com
 License: LGPLv3
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Science/Research
@@ -34,15 +34,19 @@
 * ComplexFragmentor as a tool to concatenate descriptors of several structures into one table,
 * ColorAtom implementation in Python, usable with CircuS desciriptors,
 * Scripts for CLI descriptor calculation and model optimization.
 
 Installation
 =============
 
-activate your virtual environment with python 3.9+ , clone project and cd into the DOPtools folder, then run
+Package can be installed from PyPI:
+
+    pip install doptools
+
+Otherwise, if downloaded from github, activate your virtual environment with python 3.9+ , clone project and cd into the DOPtools folder, then run
 
     pip install -U -e .
 
 Requirements
 ============
 
 The requirements are listed in setup.py and should be installed with the library.
@@ -52,15 +56,15 @@
 Calculation of molecular descriptors is organized as a scikit-learn transformer class, therefore, pandas and scikit-learn libraries are required.
 
 CircuS descriptors
 ==================
 
 The descriptors are implemented using CGRtools library and its native substructure extraction functions. Their functionality is the following. The user indicates the desired lower and upper limits for the size of substructures, as the topological radius (number of bonds from a certain atom). Size of 0 means only atom itself, size of 1 – atom and all atoms directly connected to it, and so on. It should be noted that due to the way how substructure extraction is implemented in CGRtools library, the size means the number of atoms from the center, and all the bonds between selected atoms will be present, which may be slightly counterintuitive (see an example for a 5-member ring below). This is repeated for all atoms in the molecule/CGR and for all sizes from lower to upper limit to construct the fragment table.
 
-.. image:: /docs/img/circus-demo1.png
+.. image:: docs/img/circus-demo1.png
 
 The calculation of CircuS descriptors is done by the ChythonCircus class in the chem_features module. As an extension of scikit-learn transformer class, it can take alist, an array, or pandas Series containing the molecules and perform the fragmentation, resultsing in a pandas DataFrame of descriptors. The required parameters are the lower and upper limits of the size, format of the input molecules (CGRtools MoleculeContainer or CGRContainer or SMILES), and whether or not the CGR will be processed by taking into account only dynamic objects or not. *fit* and *transform* functions are used as usual. The feature names (SMILES of the fragments) can be accessed after training ia *get_feature_names* function. 
 
 ComplexFragmentor
 ==================
 
 ComplexFragmentor class is a scikit-learn compatible transformer that concatenates the features according to specified associations. The most important argument is the *associator* - a dictionary that establishes the correspondence between a column in a data frame X and the transformer that is trained on it.
@@ -85,9 +89,9 @@
 
 Current implementation is designed for regression tasks, for models built with Scikit-learn library and using ISIDA fragments implemented in CIMtools or CircuS fragments implemented in chem_features module of this library. 
 
 The application of the ColorAtom requires a trained pipeline containing a fragmentor (CircuS are supported), features preprocessing and a model. *calculate_atom_contributions* calculates the contributions of each atom for a given molecule and returns them numerically as a dictionary. Otherwise, they can visualized directly in Jupyter Notebook via *output_html* function that returns an HTML table containing an SVG for each structure in the molecule. Since complexFragmentor is also supported, several structures in one data point can be processed simultaneously. 
 
 The coloring is done with matplotlib library. The atom contributions are normalized between 0 and 1 according to the maximum absolute value of the contribution. Therefore, if several structures are present, they will all have their colors normalized by the maximum value amond all contributions. The default colormap is PiYG. The "lower" (more negative) contributions are shown by red color, the "upper" (more positive) - by green. An example can be seen below:
 
-.. image:: /docs/img/coloratom-demo1.png
+.. image:: docs/img/coloratom-demo1.png
```

### Comparing `doptools-1.0b1/README.rst` & `doptools-1.0b2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 * ComplexFragmentor as a tool to concatenate descriptors of several structures into one table,
 * ColorAtom implementation in Python, usable with CircuS desciriptors,
 * Scripts for CLI descriptor calculation and model optimization.
 
 Installation
 =============
 
-activate your virtual environment with python 3.9+ , clone project and cd into the DOPtools folder, then run
+Package can be installed from PyPI:
+
+    pip install doptools
+
+Otherwise, if downloaded from github, activate your virtual environment with python 3.9+ , clone project and cd into the DOPtools folder, then run
 
     pip install -U -e .
 
 Requirements
 ============
 
 The requirements are listed in setup.py and should be installed with the library.
@@ -29,15 +33,15 @@
 Calculation of molecular descriptors is organized as a scikit-learn transformer class, therefore, pandas and scikit-learn libraries are required.
 
 CircuS descriptors
 ==================
 
 The descriptors are implemented using CGRtools library and its native substructure extraction functions. Their functionality is the following. The user indicates the desired lower and upper limits for the size of substructures, as the topological radius (number of bonds from a certain atom). Size of 0 means only atom itself, size of 1 – atom and all atoms directly connected to it, and so on. It should be noted that due to the way how substructure extraction is implemented in CGRtools library, the size means the number of atoms from the center, and all the bonds between selected atoms will be present, which may be slightly counterintuitive (see an example for a 5-member ring below). This is repeated for all atoms in the molecule/CGR and for all sizes from lower to upper limit to construct the fragment table.
 
-.. image:: /docs/img/circus-demo1.png
+.. image:: docs/img/circus-demo1.png
 
 The calculation of CircuS descriptors is done by the ChythonCircus class in the chem_features module. As an extension of scikit-learn transformer class, it can take alist, an array, or pandas Series containing the molecules and perform the fragmentation, resultsing in a pandas DataFrame of descriptors. The required parameters are the lower and upper limits of the size, format of the input molecules (CGRtools MoleculeContainer or CGRContainer or SMILES), and whether or not the CGR will be processed by taking into account only dynamic objects or not. *fit* and *transform* functions are used as usual. The feature names (SMILES of the fragments) can be accessed after training ia *get_feature_names* function. 
 
 ComplexFragmentor
 ==================
 
 ComplexFragmentor class is a scikit-learn compatible transformer that concatenates the features according to specified associations. The most important argument is the *associator* - a dictionary that establishes the correspondence between a column in a data frame X and the transformer that is trained on it.
@@ -62,9 +66,9 @@
 
 Current implementation is designed for regression tasks, for models built with Scikit-learn library and using ISIDA fragments implemented in CIMtools or CircuS fragments implemented in chem_features module of this library. 
 
 The application of the ColorAtom requires a trained pipeline containing a fragmentor (CircuS are supported), features preprocessing and a model. *calculate_atom_contributions* calculates the contributions of each atom for a given molecule and returns them numerically as a dictionary. Otherwise, they can visualized directly in Jupyter Notebook via *output_html* function that returns an HTML table containing an SVG for each structure in the molecule. Since complexFragmentor is also supported, several structures in one data point can be processed simultaneously. 
 
 The coloring is done with matplotlib library. The atom contributions are normalized between 0 and 1 according to the maximum absolute value of the contribution. Therefore, if several structures are present, they will all have their colors normalized by the maximum value amond all contributions. The default colormap is PiYG. The "lower" (more negative) contributions are shown by red color, the "upper" (more positive) - by green. An example can be seen below:
 
-.. image:: /docs/img/coloratom-demo1.png
+.. image:: docs/img/coloratom-demo1.png
```

### Comparing `doptools-1.0b1/doptools/__init__.py` & `doptools-1.0b2/doptools/__init__.py`

 * *Files identical despite different names*

### Comparing `doptools-1.0b1/doptools/chem/__init__.py` & `doptools-1.0b2/doptools/chem/__init__.py`

 * *Files identical despite different names*

### Comparing `doptools-1.0b1/doptools/chem/chem_features.py` & `doptools-1.0b2/doptools/chem/chem_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
 
         :param y: required by default by scikit-learn standards, but
             doesn't change the function at all.
         :type y: None
         """
         for k, v in self.associator.items():
             v.fit(x[k])
-            self.feature_names += [k+f for f in v.get_feature_names()]
+            self.feature_names += [k+'::'+f for f in v.get_feature_names()]
         return self
     
     def transform(self, x:DataFrame) -> DataFrame:
         """
         Transforms the given data frame to a data frame of features
         with their values. Applies each feature generator
         separately, then concatenates them.
```

### Comparing `doptools-1.0b1/doptools/chem/coloratom.py` & `doptools-1.0b2/doptools/chem/coloratom.py`

 * *Files identical despite different names*

### Comparing `doptools-1.0b1/doptools/chem/solvents.py` & `doptools-1.0b2/doptools/chem/solvents.py`

 * *Files identical despite different names*

### Comparing `doptools-1.0b1/doptools/chem/utils.py` & `doptools-1.0b2/doptools/chem/utils.py`

 * *Files identical despite different names*

### Comparing `doptools-1.0b1/doptools/optimizer/__init__.py` & `doptools-1.0b2/doptools/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `doptools-1.0b1/doptools/optimizer/config.py` & `doptools-1.0b2/doptools/optimizer/config.py`

 * *Files identical despite different names*

### Comparing `doptools-1.0b1/doptools/optimizer/optimizer.py` & `doptools-1.0b2/doptools/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `doptools-1.0b1/doptools/optimizer/plotter.py` & `doptools-1.0b2/doptools/optimizer/plotter.py`

 * *Files identical despite different names*

### Comparing `doptools-1.0b1/doptools/optimizer/preparer.py` & `doptools-1.0b2/doptools/optimizer/preparer.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,18 @@
     if args.atompairs:
         for nb in _set_default(args.atompairs_nBits, [1024]):
             param_dict[_make_name(('atompairs',nb))] = {'nBits':nb}
     if args.circus:
         for lower in _set_default(args.circus_min, [1]):
             for upper in _set_default(args.circus_max, [2]):
                 if int(lower) <= int(upper):
-                    param_dict[_make_name(('circus',lower, upper))] = {'lower':lower, 'upper':upper}
+                    if args.onbond:
+                        param_dict[_make_name(('circus_b',lower, upper))] = {'lower':lower, 'upper':upper, 'on_bond':True}
+                    else:
+                        param_dict[_make_name(('circus',lower, upper))] = {'lower':lower, 'upper':upper}
     if args.linear:
         for lower in _set_default(args.linear_min, [2]):
             for upper in _set_default(args.linear_max, [5]):
                 if int(lower) <= int(upper):
                     param_dict[_make_name(('chyline',lower, upper))] = {'lower':lower, 'upper':upper}
     if args.mordred2d:
         param_dict[_make_name(('mordred2d',))] = {}
@@ -164,14 +167,15 @@
             if len(input_dict['structures'].columns) == 1 and 'solvents' not in input_dict.keys():
                 calculator = eval(calculators[desc_type])
                 desc = calculator.fit_transform(input_dict['structures'][base_column].iloc[d['indices']])
             else:
                 calculators_dict = {}
                 for c in input_dict['structures'].columns:
                     calculators_dict[c] = eval(calculators[desc_type])
+                input_table = input_dict['structures']
                 if 'solvents' in input_dict.keys():
                     calculators_dict[input_dict['solvents'].name] = SolventVectorizer()
                     input_table = pd.concat([input_dict['structures'], input_dict['solvents']], axis=1)
 
                 calculator = ComplexFragmentor(associator = calculators_dict, 
                                                structure_columns=[base_column])
                 desc = calculator.fit_transform(input_table.iloc[d['indices']])
@@ -301,14 +305,16 @@
 
     parser.add_argument('--circus', action='store_true', 
                         help='put the option to calculate CircuS fragments')
     parser.add_argument('--circus_min', nargs='+', action='extend', type=int, default=[],
                         help='minimum radius of CircuS fragments. Allows several numbers, which will be stored separately. Default value 1')
     parser.add_argument('--circus_max', nargs='+', action='extend', type=int, default=[],
                         help='maximum radius of CircuS fragments. Allows several numbers, which will be stored separately. Default value 2')
+    parser.add_argument('--onbond', action='store_true', 
+                        help='toggle the calculation of CircuS fragments on bonds')
 
     parser.add_argument('--mordred2d', action='store_true', 
                         help='put the option to calculate Mordred 2D descriptors')
 
     parser.add_argument('--solvent', type=str, action='store', default='',
                         help='column that contains the solvents. Check the available solvents in the solvents.py script')
```

### Comparing `doptools-1.0b1/doptools/optimizer/rebuilder.py` & `doptools-1.0b2/doptools/optimizer/rebuilder.py`

 * *Files identical despite different names*

### Comparing `doptools-1.0b1/doptools.egg-info/PKG-INFO` & `doptools-1.0b2/doptools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doptools
-Version: 1.0b1
+Version: 1.0b2
 Summary: A package for calculation of molecular descriptors in Scikit-Learn compatible way and model optimization
 Home-page: https://github.com/POSidorov/DOPtools
 Author: Dr. Pavel Sidorov
 Author-email: pavel.o.sidorov@gmail.com
 License: LGPLv3
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Science/Research
@@ -34,15 +34,19 @@
 * ComplexFragmentor as a tool to concatenate descriptors of several structures into one table,
 * ColorAtom implementation in Python, usable with CircuS desciriptors,
 * Scripts for CLI descriptor calculation and model optimization.
 
 Installation
 =============
 
-activate your virtual environment with python 3.9+ , clone project and cd into the DOPtools folder, then run
+Package can be installed from PyPI:
+
+    pip install doptools
+
+Otherwise, if downloaded from github, activate your virtual environment with python 3.9+ , clone project and cd into the DOPtools folder, then run
 
     pip install -U -e .
 
 Requirements
 ============
 
 The requirements are listed in setup.py and should be installed with the library.
@@ -52,15 +56,15 @@
 Calculation of molecular descriptors is organized as a scikit-learn transformer class, therefore, pandas and scikit-learn libraries are required.
 
 CircuS descriptors
 ==================
 
 The descriptors are implemented using CGRtools library and its native substructure extraction functions. Their functionality is the following. The user indicates the desired lower and upper limits for the size of substructures, as the topological radius (number of bonds from a certain atom). Size of 0 means only atom itself, size of 1 – atom and all atoms directly connected to it, and so on. It should be noted that due to the way how substructure extraction is implemented in CGRtools library, the size means the number of atoms from the center, and all the bonds between selected atoms will be present, which may be slightly counterintuitive (see an example for a 5-member ring below). This is repeated for all atoms in the molecule/CGR and for all sizes from lower to upper limit to construct the fragment table.
 
-.. image:: /docs/img/circus-demo1.png
+.. image:: docs/img/circus-demo1.png
 
 The calculation of CircuS descriptors is done by the ChythonCircus class in the chem_features module. As an extension of scikit-learn transformer class, it can take alist, an array, or pandas Series containing the molecules and perform the fragmentation, resultsing in a pandas DataFrame of descriptors. The required parameters are the lower and upper limits of the size, format of the input molecules (CGRtools MoleculeContainer or CGRContainer or SMILES), and whether or not the CGR will be processed by taking into account only dynamic objects or not. *fit* and *transform* functions are used as usual. The feature names (SMILES of the fragments) can be accessed after training ia *get_feature_names* function. 
 
 ComplexFragmentor
 ==================
 
 ComplexFragmentor class is a scikit-learn compatible transformer that concatenates the features according to specified associations. The most important argument is the *associator* - a dictionary that establishes the correspondence between a column in a data frame X and the transformer that is trained on it.
@@ -85,9 +89,9 @@
 
 Current implementation is designed for regression tasks, for models built with Scikit-learn library and using ISIDA fragments implemented in CIMtools or CircuS fragments implemented in chem_features module of this library. 
 
 The application of the ColorAtom requires a trained pipeline containing a fragmentor (CircuS are supported), features preprocessing and a model. *calculate_atom_contributions* calculates the contributions of each atom for a given molecule and returns them numerically as a dictionary. Otherwise, they can visualized directly in Jupyter Notebook via *output_html* function that returns an HTML table containing an SVG for each structure in the molecule. Since complexFragmentor is also supported, several structures in one data point can be processed simultaneously. 
 
 The coloring is done with matplotlib library. The atom contributions are normalized between 0 and 1 according to the maximum absolute value of the contribution. Therefore, if several structures are present, they will all have their colors normalized by the maximum value amond all contributions. The default colormap is PiYG. The "lower" (more negative) contributions are shown by red color, the "upper" (more positive) - by green. An example can be seen below:
 
-.. image:: /docs/img/coloratom-demo1.png
+.. image:: docs/img/coloratom-demo1.png
```

### Comparing `doptools-1.0b1/doptools.egg-info/SOURCES.txt` & `doptools-1.0b2/doptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doptools-1.0b1/setup.py` & `doptools-1.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <https://www.gnu.org/licenses/>.
 #
 from pathlib import Path
 from setuptools import setup, find_packages
 
 
-version = '1.0b1'
+version = '1.0b2'
 
 setup(
     name='doptools',
     version=version,
     packages=find_packages(),
     url='https://github.com/POSidorov/DOPtools',
     license='LGPLv3',
```

