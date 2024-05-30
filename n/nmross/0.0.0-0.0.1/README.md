# Comparing `tmp/nmross-0.0.0.tar.gz` & `tmp/nmross-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmross-0.0.0.tar", last modified: Tue May 28 08:57:20 2024, max compression
+gzip compressed data, was "nmross-0.0.1.tar", last modified: Thu May 30 07:43:16 2024, max compression
```

## Comparing `nmross-0.0.0.tar` & `nmross-0.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 08:57:20.125342 nmross-0.0.0/
--rw-rw-rw-   0        0        0     1120 2024-05-27 15:11:46.000000 nmross-0.0.0/LICENSE
--rw-rw-rw-   0        0        0     6802 2024-05-28 08:57:20.125342 nmross-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3995 2024-05-27 15:11:46.000000 nmross-0.0.0/README.md
--rw-rw-rw-   0        0        0     1636 2024-05-27 15:30:00.000000 nmross-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-28 08:57:20.133313 nmross-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-28 08:57:20.022800 nmross-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-28 08:57:20.065201 nmross-0.0.0/src/nmross/
--rw-rw-rw-   0        0        0    66108 2024-05-27 15:11:46.000000 nmross-0.0.0/src/nmross/NMRoss.py
--rw-rw-rw-   0        0        0      811 2024-05-27 15:11:46.000000 nmross-0.0.0/src/nmross/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:57:20.125342 nmross-0.0.0/src/nmross.egg-info/
--rw-rw-rw-   0        0        0     6802 2024-05-28 08:57:19.000000 nmross-0.0.0/src/nmross.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-05-28 08:57:19.000000 nmross-0.0.0/src/nmross.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 08:57:19.000000 nmross-0.0.0/src/nmross.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2024-05-28 08:57:19.000000 nmross-0.0.0/src/nmross.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-28 08:57:19.000000 nmross-0.0.0/src/nmross.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-28 08:57:20.119496 nmross-0.0.0/tests/
--rw-rw-rw-   0        0        0    27343 2024-05-27 15:11:46.000000 nmross-0.0.0/tests/test_NMRoss.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:43:16.593904 nmross-0.0.1/
+-rw-rw-rw-   0        0        0     1120 2024-05-27 15:11:46.000000 nmross-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0     6926 2024-05-30 07:43:16.593904 nmross-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4119 2024-05-30 07:38:33.000000 nmross-0.0.1/README.md
+-rw-rw-rw-   0        0        0     1630 2024-05-30 07:42:43.000000 nmross-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 07:43:16.593904 nmross-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-30 07:43:16.515690 nmross-0.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 07:43:16.531278 nmross-0.0.1/src/nmross/
+-rw-rw-rw-   0        0        0    66162 2024-05-29 17:54:58.000000 nmross-0.0.1/src/nmross/NMRoss.py
+-rw-rw-rw-   0        0        0      811 2024-05-27 15:11:46.000000 nmross-0.0.1/src/nmross/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:43:16.578072 nmross-0.0.1/src/nmross.egg-info/
+-rw-rw-rw-   0        0        0     6926 2024-05-30 07:43:16.000000 nmross-0.0.1/src/nmross.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-05-30 07:43:16.000000 nmross-0.0.1/src/nmross.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 07:43:16.000000 nmross-0.0.1/src/nmross.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2024-05-30 07:43:16.000000 nmross-0.0.1/src/nmross.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 07:43:16.000000 nmross-0.0.1/src/nmross.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 07:43:16.578072 nmross-0.0.1/tests/
+-rw-rw-rw-   0        0        0    27408 2024-05-29 18:24:31.000000 nmross-0.0.1/tests/test_NMRoss.py
```

### Comparing `nmross-0.0.0/LICENSE` & `nmross-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nmross-0.0.0/PKG-INFO` & `nmross-0.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmross
-Version: 0.0.0
+Version: 0.0.1
 Summary: Gives an approximate 1H NMR when given a smiles or a IUPAC name of a molecule with maximum one aromatic ring and no double bonds.
 Author-email: Cedric Rossboth <cedric.rossboth@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Cedric Rossboth <cedric.rossboth@epfl.ch>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -65,15 +65,35 @@
 </h1>
 
 <br>
 
 
 Gives an approximate 1H NMR when given a smiles or a IUPAC name of a molecule with maximum one aromatic ring and no double bonds.
 
-## `👷‍♂️:` Installation
+## `🧑‍🔧:` Installation 
+Here are the steps to directly install the nmross package using pip install.
+
+## 1. Create a Virtual Environment 
+
+We advise you to create an environment where you want to work on the project. Then activate the environment:
+```
+conda create -n nmross python=3.10
+conda activate nmross
+```
+## 2. Install Package
+```
+pip install nmross
+```
+## 3. Install JupyterLab
+```
+pip install jupyter lab
+jupyter lab
+```
+
+## `👷‍♂️:` Local installation 
 
 ## 1. Fork the Repository
 
 First, fork the repository to your own GitHub account. This creates a copy of the repository under your GitHub account.
 
 ## 2. Clone the Repository
 
@@ -125,65 +145,41 @@
 
 The function Show takes as inputs either the IUPAC name of the compound or the smiles representation of it and an index in the molecule. The function outputs a plot of the 1H NMR of the molecule with the peak of the atom chosen hihlighted and a Mol object with all equivalent hydrogens highlighted. The function only ever plots a NMR spectrum if the atom with the index chosen has at least one hydrogen. The plot appears automatically when using the Show() method but the Mol object needs to be stocked in a variable to be shown.
 
 One who only ever wants to know the 1H NMR of ethanol would use the package like this:
 
 ```python
 from nmross.NMRoss import NMR
-NMR('CCO')
+plt, mol = NMR('CCO')
+mol
 ```
 
 One who would like to know which peak is the one of the terminal carbon would use the package like this. First:
 
 ```python
-from nmross.NMRoss import NMR
-from nmross.NMRoss import Show
+from nmross.NMRoss import NMR, Show
 plt, mol = NMR('CCO')
 mol
 ```
 
-The second line serves to identify how the program gives the indices to the atoms in the molecule. One of these indices can then be used during the following step. In this case, the terminal carbon is the one that is meant to be identified. Thus, the next steps are:
+The 'mol' code line serves to identify how the program gives the indices to the atoms in the molecule. One of these indices can then be used during the following step. In this case, the terminal carbon is the one that is meant to be identified. Thus, the next steps are:
 ```python
 plt, mol = Show('CCO', 0)
 mol
 ```
 This shows that the primary carbon has hydrogens which are non equivalent to other hydrogens in the molecule.
 
+## `📖:`Tests
 
-Click to add a cell.
-
-
-
-
-## `💥:` Development installation
-
-Initialize Git (only for the first time). 
-
-Note: You should have create an empty repository on `https://github.com:CedricRossboth/nmross`.
-
-```
-git init
-git add * 
-git add .*
-git commit -m "Initial commit" 
-git branch -M main
-git remote add origin git@github.com:CedricRossboth/nmross.git 
-git push -u origin main
+To run the tests, one would need to clone the repository as shown above and then simply write the line code below in the terminal. Be aware that you need to change direction in order to be in the correct file.
+```python
+pip install pytest
+pytest
 ```
 
-Then add and commit changes as usual. 
 
-To install the package, run
 
-```
-(nmross) $ pip install -e ".[test,doc]"
-```
 
-### Run tests and coverage
 
-```
-(conda_env) $ pip install tox
-(conda_env) $ tox
-```
```

### Comparing `nmross-0.0.0/README.md` & `nmross-0.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,35 @@
 </h1>
 
 <br>
 
 
 Gives an approximate 1H NMR when given a smiles or a IUPAC name of a molecule with maximum one aromatic ring and no double bonds.
 
-## `👷‍♂️:` Installation
+## `🧑‍🔧:` Installation 
+Here are the steps to directly install the nmross package using pip install.
+
+## 1. Create a Virtual Environment 
+
+We advise you to create an environment where you want to work on the project. Then activate the environment:
+```
+conda create -n nmross python=3.10
+conda activate nmross
+```
+## 2. Install Package
+```
+pip install nmross
+```
+## 3. Install JupyterLab
+```
+pip install jupyter lab
+jupyter lab
+```
+
+## `👷‍♂️:` Local installation 
 
 ## 1. Fork the Repository
 
 First, fork the repository to your own GitHub account. This creates a copy of the repository under your GitHub account.
 
 ## 2. Clone the Repository
 
@@ -67,65 +87,41 @@
 
 The function Show takes as inputs either the IUPAC name of the compound or the smiles representation of it and an index in the molecule. The function outputs a plot of the 1H NMR of the molecule with the peak of the atom chosen hihlighted and a Mol object with all equivalent hydrogens highlighted. The function only ever plots a NMR spectrum if the atom with the index chosen has at least one hydrogen. The plot appears automatically when using the Show() method but the Mol object needs to be stocked in a variable to be shown.
 
 One who only ever wants to know the 1H NMR of ethanol would use the package like this:
 
 ```python
 from nmross.NMRoss import NMR
-NMR('CCO')
+plt, mol = NMR('CCO')
+mol
 ```
 
 One who would like to know which peak is the one of the terminal carbon would use the package like this. First:
 
 ```python
-from nmross.NMRoss import NMR
-from nmross.NMRoss import Show
+from nmross.NMRoss import NMR, Show
 plt, mol = NMR('CCO')
 mol
 ```
 
-The second line serves to identify how the program gives the indices to the atoms in the molecule. One of these indices can then be used during the following step. In this case, the terminal carbon is the one that is meant to be identified. Thus, the next steps are:
+The 'mol' code line serves to identify how the program gives the indices to the atoms in the molecule. One of these indices can then be used during the following step. In this case, the terminal carbon is the one that is meant to be identified. Thus, the next steps are:
 ```python
 plt, mol = Show('CCO', 0)
 mol
 ```
 This shows that the primary carbon has hydrogens which are non equivalent to other hydrogens in the molecule.
 
+## `📖:`Tests
 
-Click to add a cell.
-
-
-
-
-## `💥:` Development installation
-
-Initialize Git (only for the first time). 
-
-Note: You should have create an empty repository on `https://github.com:CedricRossboth/nmross`.
-
-```
-git init
-git add * 
-git add .*
-git commit -m "Initial commit" 
-git branch -M main
-git remote add origin git@github.com:CedricRossboth/nmross.git 
-git push -u origin main
+To run the tests, one would need to clone the repository as shown above and then simply write the line code below in the terminal. Be aware that you need to change direction in order to be in the correct file.
+```python
+pip install pytest
+pytest
 ```
 
-Then add and commit changes as usual. 
 
-To install the package, run
 
-```
-(nmross) $ pip install -e ".[test,doc]"
-```
 
-### Run tests and coverage
 
-```
-(conda_env) $ pip install tox
-(conda_env) $ tox
-```
```

### Comparing `nmross-0.0.0/pyproject.toml` & `nmross-0.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
+version = "0.0.1"
 name = "nmross"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 description = "Gives an approximate 1H NMR when given a smiles or a IUPAC name of a molecule with maximum one aromatic ring and no double bonds."
 dependencies = [ 
     "pubchempy==1.0.4","numpy","rdkit","matplotlib"
@@ -25,16 +26,14 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 keywords = ['NMR']
 
-dynamic = ["version"]
-
 [project.urls]
 source = "https://github.com/CedricRossboth/nmross"
 tracker = "https://github.com/CedricRossboth/nmross/issues"
 
 [project.optional-dependencies]
 test = [
     "hypothesis",
```

### Comparing `nmross-0.0.0/src/nmross/NMRoss.py` & `nmross-0.0.1/src/nmross/NMRoss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1115,16 +1115,15 @@
     
     return matches
 
 
 
 def search_multiple_aromatics(substituents, smiles_dict):
     """
-    Searches for multiple aromatic substituents in the provided smiles_dict.
-    Appends results to a list of lists 'results' based on the structure of 'substituents'.
+    Searches for the functional groups in smiles_dict in the substituents list of list, works for the case of multiple aromatic rings.
 
     Parameters:
     substituents (list of list of str): List of lists containing SMILES strings or 'H'.
     smiles_dict (dict): Dictionary where keys are SMILES strings and values are priorities.
 
     Returns:
     list of list of dict: A list of lists containing dictionaries with matched SMILES strings and their indices.
@@ -1618,15 +1617,18 @@
     try:        
         # The SMILES of the molecule is acquired.
         crude_smiles = get_smiles_from_input(name)
 
         # Rearrange the molecule SMILES.
         smiles = canonicalize_smiles(crude_smiles)
         # The IUPAC name is acquired to show it on the graph.
-        chemical_name = get_name_from_smiles(smiles)
+        if is_valid_smiles(name):
+            chemical_name = get_name_from_smiles(smiles)
+        else:
+            chemical_name = name
 
         # The SMILES is turned into a Mol object.
         mol = Chem.MolFromSmiles(smiles)
 
         # The multiplicity of each hydrogen is calculated.
         mult, dict_Hs = multiplicity(smiles)
         dict_shift = {}
```

### Comparing `nmross-0.0.0/src/nmross/__init__.py` & `nmross-0.0.1/src/nmross/__init__.py`

 * *Files identical despite different names*

### Comparing `nmross-0.0.0/src/nmross.egg-info/PKG-INFO` & `nmross-0.0.1/src/nmross.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmross
-Version: 0.0.0
+Version: 0.0.1
 Summary: Gives an approximate 1H NMR when given a smiles or a IUPAC name of a molecule with maximum one aromatic ring and no double bonds.
 Author-email: Cedric Rossboth <cedric.rossboth@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Cedric Rossboth <cedric.rossboth@epfl.ch>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -65,15 +65,35 @@
 </h1>
 
 <br>
 
 
 Gives an approximate 1H NMR when given a smiles or a IUPAC name of a molecule with maximum one aromatic ring and no double bonds.
 
-## `👷‍♂️:` Installation
+## `🧑‍🔧:` Installation 
+Here are the steps to directly install the nmross package using pip install.
+
+## 1. Create a Virtual Environment 
+
+We advise you to create an environment where you want to work on the project. Then activate the environment:
+```
+conda create -n nmross python=3.10
+conda activate nmross
+```
+## 2. Install Package
+```
+pip install nmross
+```
+## 3. Install JupyterLab
+```
+pip install jupyter lab
+jupyter lab
+```
+
+## `👷‍♂️:` Local installation 
 
 ## 1. Fork the Repository
 
 First, fork the repository to your own GitHub account. This creates a copy of the repository under your GitHub account.
 
 ## 2. Clone the Repository
 
@@ -125,65 +145,41 @@
 
 The function Show takes as inputs either the IUPAC name of the compound or the smiles representation of it and an index in the molecule. The function outputs a plot of the 1H NMR of the molecule with the peak of the atom chosen hihlighted and a Mol object with all equivalent hydrogens highlighted. The function only ever plots a NMR spectrum if the atom with the index chosen has at least one hydrogen. The plot appears automatically when using the Show() method but the Mol object needs to be stocked in a variable to be shown.
 
 One who only ever wants to know the 1H NMR of ethanol would use the package like this:
 
 ```python
 from nmross.NMRoss import NMR
-NMR('CCO')
+plt, mol = NMR('CCO')
+mol
 ```
 
 One who would like to know which peak is the one of the terminal carbon would use the package like this. First:
 
 ```python
-from nmross.NMRoss import NMR
-from nmross.NMRoss import Show
+from nmross.NMRoss import NMR, Show
 plt, mol = NMR('CCO')
 mol
 ```
 
-The second line serves to identify how the program gives the indices to the atoms in the molecule. One of these indices can then be used during the following step. In this case, the terminal carbon is the one that is meant to be identified. Thus, the next steps are:
+The 'mol' code line serves to identify how the program gives the indices to the atoms in the molecule. One of these indices can then be used during the following step. In this case, the terminal carbon is the one that is meant to be identified. Thus, the next steps are:
 ```python
 plt, mol = Show('CCO', 0)
 mol
 ```
 This shows that the primary carbon has hydrogens which are non equivalent to other hydrogens in the molecule.
 
+## `📖:`Tests
 
-Click to add a cell.
-
-
-
-
-## `💥:` Development installation
-
-Initialize Git (only for the first time). 
-
-Note: You should have create an empty repository on `https://github.com:CedricRossboth/nmross`.
-
-```
-git init
-git add * 
-git add .*
-git commit -m "Initial commit" 
-git branch -M main
-git remote add origin git@github.com:CedricRossboth/nmross.git 
-git push -u origin main
+To run the tests, one would need to clone the repository as shown above and then simply write the line code below in the terminal. Be aware that you need to change direction in order to be in the correct file.
+```python
+pip install pytest
+pytest
 ```
 
-Then add and commit changes as usual. 
 
-To install the package, run
 
-```
-(nmross) $ pip install -e ".[test,doc]"
-```
 
-### Run tests and coverage
 
-```
-(conda_env) $ pip install tox
-(conda_env) $ tox
-```
```

### Comparing `nmross-0.0.0/tests/test_NMRoss.py` & `nmross-0.0.1/tests/test_NMRoss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from nmross.NMRoss import get_smiles
+import pytest
+from nmross.NMRoss import *
 
 def test_get_smiles_butanol():
     expected_smiles = 'CCCCO'  # Known SMILES for butanol
     result = get_smiles('butanol')
     assert result == expected_smiles, f"Expected {expected_smiles}, but got {result}"
 
 def test_get_smiles_non_existent():
@@ -185,15 +186,15 @@
     test_search_algo_with_formaldehyde()
     print("All tests passed.")
 
 
 
 
 def test_shift_1_butyric_acid():
-    smiles = 'CCCC(=O)'
+    smiles = 'CCCC(=O)O'
     result = shift_1(0, smiles)
     expected = 0.835
     assert abs(result - expected) < 1e-3, f"Expected {expected}, but got {result}"
 
 def test_shift_1_propanol():
     smiles = 'CCCO'
     result = shift_1(1, smiles)
@@ -266,19 +267,19 @@
     test_non_string_input()
     test_empty_string()
     print("All tests passed.")
 
 
 
 
-def test_valid_smiles():
-    assert find_aromatic_carbon_indexes("c1ccccc1") == [[0, 2, 3, 4, 5, 6]]
+def test_find_aromatic_carbon_indexes_benzene():
+    assert find_aromatic_carbon_indexes("c1ccccc1") == [0, 2, 3, 4, 5, 6]
 
-def test_valid_smiles_with_substituent():
-    assert find_aromatic_carbon_indexes("c1ccccc1C") == [[0, 2, 3, 4, 5, 6]]
+def test_find_aromatic_carbon_indexes_toluene():
+    assert find_aromatic_carbon_indexes("c1ccccc1C") == [0, 2, 3, 4, 5, 6]
 
 def test_invalid_smiles():
     try:
         find_aromatic_carbon_indexes("InvalidSMILES")
     except ValueError:
         pass
     else:
@@ -297,16 +298,16 @@
         find_aromatic_carbon_indexes("")
     except ValueError:
         pass
     else:
         assert False, "Expected ValueError"
 
 if __name__ == "__main__":
-    test_valid_smiles()
-    test_valid_smiles_with_substituent()
+    test_find_aromatic_carbon_indexes_benzene()
+    test_find_aromatic_carbon_indexes_toluene()
     test_invalid_smiles()
     test_non_string_input()
     test_empty_string()
     print("All tests passed.")
```

