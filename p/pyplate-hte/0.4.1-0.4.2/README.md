# Comparing `tmp/pyplate-hte-0.4.1.tar.gz` & `tmp/pyplate_hte-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplate-hte-0.4.1.tar", last modified: Sat Apr  6 16:12:44 2024, max compression
+gzip compressed data, was "pyplate_hte-0.4.2.tar", last modified: Thu May 30 19:01:35 2024, max compression
```

## Comparing `pyplate-hte-0.4.1.tar` & `pyplate_hte-0.4.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-06 16:12:44.267452 pyplate-hte-0.4.1/
--rw-r--r--   0 marvinj    (502) staff       (20)    10945 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/LICENSE.txt
--rw-r--r--   0 marvinj    (502) staff       (20)    15334 2024-04-06 16:12:44.266542 pyplate-hte-0.4.1/PKG-INFO
--rw-r--r--   0 marvinj    (502) staff       (20)     2582 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/README.md
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-06 16:12:44.231970 pyplate-hte-0.4.1/pyplate/
--rw-r--r--   0 marvinj    (502) staff       (20)     1768 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/pyplate/__init__.py
--rw-r--r--   0 marvinj    (502) staff       (20)    12603 2024-04-06 15:54:04.000000 pyplate-hte-0.4.1/pyplate/experiment_design.py
--rw-r--r--   0 marvinj    (502) staff       (20)   108858 2024-04-06 15:54:04.000000 pyplate-hte-0.4.1/pyplate/pyplate.py
--rw-r--r--   0 marvinj    (502) staff       (20)      860 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/pyplate/pyplate.yaml
--rw-r--r--   0 marvinj    (502) staff       (20)    14316 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/pyplate/slicer.py
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-06 16:12:44.265408 pyplate-hte-0.4.1/pyplate_hte.egg-info/
--rw-r--r--   0 marvinj    (502) staff       (20)    15334 2024-04-06 16:12:44.000000 pyplate-hte-0.4.1/pyplate_hte.egg-info/PKG-INFO
--rw-r--r--   0 marvinj    (502) staff       (20)      668 2024-04-06 16:12:44.000000 pyplate-hte-0.4.1/pyplate_hte.egg-info/SOURCES.txt
--rw-r--r--   0 marvinj    (502) staff       (20)        1 2024-04-06 16:12:44.000000 pyplate-hte-0.4.1/pyplate_hte.egg-info/dependency_links.txt
--rw-r--r--   0 marvinj    (502) staff       (20)       20 2024-04-06 16:12:44.000000 pyplate-hte-0.4.1/pyplate_hte.egg-info/requires.txt
--rw-r--r--   0 marvinj    (502) staff       (20)        8 2024-04-06 16:12:44.000000 pyplate-hte-0.4.1/pyplate_hte.egg-info/top_level.txt
--rw-r--r--   0 marvinj    (502) staff       (20)      689 2024-04-06 16:11:48.000000 pyplate-hte-0.4.1/pyproject.toml
--rw-r--r--   0 marvinj    (502) staff       (20)       38 2024-04-06 16:12:44.267587 pyplate-hte-0.4.1/setup.cfg
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-06 16:12:44.264119 pyplate-hte-0.4.1/tests/
--rw-r--r--   0 marvinj    (502) staff       (20)    10740 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_Container.py
--rw-r--r--   0 marvinj    (502) staff       (20)     1975 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_Experiment.py
--rw-r--r--   0 marvinj    (502) staff       (20)     6029 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_ExperimentalSpace.py
--rw-r--r--   0 marvinj    (502) staff       (20)      987 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_Factor.py
--rw-r--r--   0 marvinj    (502) staff       (20)     5325 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_Plate.py
--rw-r--r--   0 marvinj    (502) staff       (20)     6607 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_Recipe.py
--rw-r--r--   0 marvinj    (502) staff       (20)     6292 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_Slicer.py
--rw-r--r--   0 marvinj    (502) staff       (20)     3477 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_Substance.py
--rw-r--r--   0 marvinj    (502) staff       (20)     2827 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_convert.py
--rw-r--r--   0 marvinj    (502) staff       (20)     3762 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_create_solution.py
--rw-r--r--   0 marvinj    (502) staff       (20)     1352 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_dilute.py
--rw-r--r--   0 marvinj    (502) staff       (20)    25879 2024-04-06 15:54:04.000000 pyplate-hte-0.4.1/tests/test_recipe_amount_used.py
--rw-r--r--   0 marvinj    (502) staff       (20)     1392 2024-04-06 15:54:04.000000 pyplate-hte-0.4.1/tests/test_recipe_volume_used.py
--rw-r--r--   0 marvinj    (502) staff       (20)     5796 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_transfers.py
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-05-30 19:01:35.338218 pyplate_hte-0.4.2/
+-rw-r--r--   0 marvinj    (502) staff       (20)    10945 2024-01-28 17:38:34.000000 pyplate_hte-0.4.2/LICENSE.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)    15695 2024-05-30 19:01:35.336542 pyplate_hte-0.4.2/PKG-INFO
+-rw-r--r--   0 marvinj    (502) staff       (20)     2944 2024-04-15 03:08:55.000000 pyplate_hte-0.4.2/README.md
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-05-30 19:01:35.247036 pyplate_hte-0.4.2/pyplate/
+-rw-r--r--   0 marvinj    (502) staff       (20)     2301 2024-05-30 18:57:49.000000 pyplate_hte-0.4.2/pyplate/__init__.py
+-rw-r--r--   0 marvinj    (502) staff       (20)    12580 2024-05-30 18:53:20.000000 pyplate_hte-0.4.2/pyplate/experiment_design.py
+-rw-r--r--   0 marvinj    (502) staff       (20)   131169 2024-05-30 18:53:20.000000 pyplate_hte-0.4.2/pyplate/pyplate.py
+-rw-r--r--   0 marvinj    (502) staff       (20)      940 2024-05-06 17:36:49.000000 pyplate_hte-0.4.2/pyplate/pyplate.yaml
+-rw-r--r--   0 marvinj    (502) staff       (20)    14330 2024-05-30 18:53:20.000000 pyplate_hte-0.4.2/pyplate/slicer.py
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-05-30 19:01:35.333878 pyplate_hte-0.4.2/pyplate_hte.egg-info/
+-rw-r--r--   0 marvinj    (502) staff       (20)    15695 2024-05-30 19:01:35.000000 pyplate_hte-0.4.2/pyplate_hte.egg-info/PKG-INFO
+-rw-r--r--   0 marvinj    (502) staff       (20)      739 2024-05-30 19:01:35.000000 pyplate_hte-0.4.2/pyplate_hte.egg-info/SOURCES.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)        1 2024-05-30 19:01:35.000000 pyplate_hte-0.4.2/pyplate_hte.egg-info/dependency_links.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)       20 2024-05-30 19:01:35.000000 pyplate_hte-0.4.2/pyplate_hte.egg-info/requires.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)        8 2024-05-30 19:01:35.000000 pyplate_hte-0.4.2/pyplate_hte.egg-info/top_level.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)      689 2024-05-30 18:41:13.000000 pyplate_hte-0.4.2/pyproject.toml
+-rw-r--r--   0 marvinj    (502) staff       (20)       38 2024-05-30 19:01:35.338421 pyplate_hte-0.4.2/setup.cfg
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-05-30 19:01:35.293187 pyplate_hte-0.4.2/tests/
+-rw-r--r--   0 marvinj    (502) staff       (20)    15601 2024-05-16 22:26:42.000000 pyplate_hte-0.4.2/tests/test_Container.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     5325 2024-04-15 02:14:28.000000 pyplate_hte-0.4.2/tests/test_Plate.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     6607 2024-04-19 03:26:45.000000 pyplate_hte-0.4.2/tests/test_Recipe.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     6292 2024-03-13 22:47:19.000000 pyplate_hte-0.4.2/tests/test_Slicer.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     3869 2024-04-15 03:08:55.000000 pyplate_hte-0.4.2/tests/test_Substance.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     2877 2024-04-15 03:08:55.000000 pyplate_hte-0.4.2/tests/test_convert.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     3738 2024-05-06 17:36:49.000000 pyplate_hte-0.4.2/tests/test_create_solution.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     1352 2024-04-15 02:14:28.000000 pyplate_hte-0.4.2/tests/test_dilute.py
+-rw-r--r--   0 marvinj    (502) staff       (20)      939 2024-04-04 18:26:24.000000 pyplate_hte-0.4.2/tests/test_eugene.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     4235 2024-05-06 17:36:49.000000 pyplate_hte-0.4.2/tests/test_get_substance_used2.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     2268 2024-05-06 17:36:49.000000 pyplate_hte-0.4.2/tests/test_recipe_amount_remaining.py
+-rw-r--r--   0 marvinj    (502) staff       (20)    12757 2024-05-06 17:36:49.000000 pyplate_hte-0.4.2/tests/test_recipe_get_container_flows.py
+-rw-r--r--   0 marvinj    (502) staff       (20)    27431 2024-05-06 17:36:49.000000 pyplate_hte-0.4.2/tests/test_recipe_get_substance_used.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     5796 2024-04-15 02:14:28.000000 pyplate_hte-0.4.2/tests/test_transfers.py
+-rw-r--r--   0 marvinj    (502) staff       (20)      501 2024-05-16 22:26:42.000000 pyplate_hte-0.4.2/tests/test_volume_used_Plate_transfer.py
```

### Comparing `pyplate-hte-0.4.1/LICENSE.txt` & `pyplate_hte-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4.1/PKG-INFO` & `pyplate_hte-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplate-hte
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Python tool for designing chemistry experiments in plate format
 Author: Eugene Kwan and James Marvin
 Author-email: ekwan16@gmail.com
 License:   				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -205,63 +205,74 @@
 
 # PyPlate
 
 [![PyPI](https://img.shields.io/pypi/v/pyplate-hte)](https://pypi.org/project/pyplate-hte)
 [![Documentation Status](https://readthedocs.org/projects/pyplate-hte/badge/?version=latest)](https://pyplate-hte.readthedocs.io/en/latest/?badge=latest)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyplate-hte)](https://pypi.org/project/pyplate-hte)
 
-An open-source Python tool for high-throughput chemistry.
+An open-source Python-based ontology and tool for designing, implementing, and reproducing high-throughput experiments (HTE).
 
 ### Introduction
 
-PyPlate provides tools for the design and implementation of high-throughput chemistry experiments (in particular, reaction screening).  It allows the user to define a space of experimental parameters to be explored, select points in that space for experimentation, and design liquid/solid handling steps to implement those experiments in 96 well plates.
+PyPlate provides tools for the design and implementation of high-throughput chemistry and biology experiments (e.g., reaction screening, cell assays, chromatography screening).  It allows the user to define a space of experimental parameters to be explored, select points in that space for experimentation, and design liquid/solid handling steps to implement those experiments in 96 well plates.
 
 ### Installation
 
 PyPlate requires Python 3.10 or later.
 
 `pip install pyplate-hte`
 
 To view plate visualizations, you will need an interactive Python shell like Jupyter.
 
-### Philosophy
-
-All experiments are divided into a *design* phase and an *implementation* phase.
-
-**Design Phase**: TBD
-
-**Implementation Phase**: PyPlate mimics the physical process of dispensing solids or liquids into plates.  `Substance`s are placed into `Container`s and dispensed into `Plate`s.  The instructions for creating a set of plates are grouped into `Recipe` objects.
-
-- add something about how to check that the implementation and design are consistent
-- All objects in PyPlate are considered immutable.
+**Note:** A similarly named package `pyplate` also exists on PyPi.  Be sure to install `pyplate-hte` and **not** `pyplate`.
 
 ## Quick Start
 
+Here is a simple example that illustrates some of the core features of `PyPlate`:
+
 ```python
 
 from pyplate import Substance, Container, Plate, Recipe
 
 triethylamine = Substance.liquid(name="triethylamine", mol_weight=101.19, density=0.726)
-DMSO = Substance.liquid(name="DMSO", mol_weight=78.13, density=1.1004)
+water = Substance.liquid(name="water", mol_weight=18.015, density=1.0)
 
-triethylamine_50mM = Container.create_solution(solute=triethylamine, solvent=DMSO, concentration='50 mM',
+triethylamine_50mM = Container.create_solution(solute=triethylamine, solvent=water, concentration='50 mM',
                                                total_quantity='10 mL')
+
 plate = Plate(name='plate', max_volume_per_well='50 uL')
 
 recipe = Recipe().uses(triethylamine_50mM, plate)
 recipe.transfer(source=triethylamine_50mM, destination=plate[2:7, 2:11], quantity='10 uL')
 results = recipe.bake()
 triethylamine_50mM = results[triethylamine_50mM.name]
 plate = results[plate.name]
 
 recipe.visualize(what=plate, mode='final', unit='uL', timeframe=0)
 
 ```
 
 ![img.png](images/simple_visualization.png)
 
-Documentation is available at [ReadTheDocs](https://pyplate-hte.readthedocs.io/en/latest/).
+## Documentation
+
+Online documentation is available at [ReadTheDocs](https://pyplate-hte.readthedocs.io/en/latest/).  To build the documentation locally, please follow these steps:
+
+``make -C docs html``
+
+The resulting HTML files will be in `docs/build/html`.
+
+In order to build the documentation successfully, you must install the packages listed in docs/requirements.txt.  You can do this by running:
+
+``pip install -r docs/requirements.txt``
 
 ## License
 
-Licensed under the Apache License, Version 2.0 (the "License")
-You may obtain a copy of the License at https://www.apache.org/licenses/LICENSE-2.0
+Licensed under the [Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0) (the "License").
+
+## Contributors
+
+**PyPlate** was designed and written by James Marvin, Eugene Kwan, Corin Wagen, Aryamaan Dhomne, and Pravin Mahendran.
+
+## Getting Help
+
+Please open a GitHub issue!  We respond regularly.  Please also feel free to contribute!
```

### Comparing `pyplate-hte-0.4.1/README.md` & `pyplate_hte-0.4.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,73 @@
 # PyPlate
 
 [![PyPI](https://img.shields.io/pypi/v/pyplate-hte)](https://pypi.org/project/pyplate-hte)
 [![Documentation Status](https://readthedocs.org/projects/pyplate-hte/badge/?version=latest)](https://pyplate-hte.readthedocs.io/en/latest/?badge=latest)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyplate-hte)](https://pypi.org/project/pyplate-hte)
 
-An open-source Python tool for high-throughput chemistry.
+An open-source Python-based ontology and tool for designing, implementing, and reproducing high-throughput experiments (HTE).
 
 ### Introduction
 
-PyPlate provides tools for the design and implementation of high-throughput chemistry experiments (in particular, reaction screening).  It allows the user to define a space of experimental parameters to be explored, select points in that space for experimentation, and design liquid/solid handling steps to implement those experiments in 96 well plates.
+PyPlate provides tools for the design and implementation of high-throughput chemistry and biology experiments (e.g., reaction screening, cell assays, chromatography screening).  It allows the user to define a space of experimental parameters to be explored, select points in that space for experimentation, and design liquid/solid handling steps to implement those experiments in 96 well plates.
 
 ### Installation
 
 PyPlate requires Python 3.10 or later.
 
 `pip install pyplate-hte`
 
 To view plate visualizations, you will need an interactive Python shell like Jupyter.
 
-### Philosophy
-
-All experiments are divided into a *design* phase and an *implementation* phase.
-
-**Design Phase**: TBD
-
-**Implementation Phase**: PyPlate mimics the physical process of dispensing solids or liquids into plates.  `Substance`s are placed into `Container`s and dispensed into `Plate`s.  The instructions for creating a set of plates are grouped into `Recipe` objects.
-
-- add something about how to check that the implementation and design are consistent
-- All objects in PyPlate are considered immutable.
+**Note:** A similarly named package `pyplate` also exists on PyPi.  Be sure to install `pyplate-hte` and **not** `pyplate`.
 
 ## Quick Start
 
+Here is a simple example that illustrates some of the core features of `PyPlate`:
+
 ```python
 
 from pyplate import Substance, Container, Plate, Recipe
 
 triethylamine = Substance.liquid(name="triethylamine", mol_weight=101.19, density=0.726)
-DMSO = Substance.liquid(name="DMSO", mol_weight=78.13, density=1.1004)
+water = Substance.liquid(name="water", mol_weight=18.015, density=1.0)
 
-triethylamine_50mM = Container.create_solution(solute=triethylamine, solvent=DMSO, concentration='50 mM',
+triethylamine_50mM = Container.create_solution(solute=triethylamine, solvent=water, concentration='50 mM',
                                                total_quantity='10 mL')
+
 plate = Plate(name='plate', max_volume_per_well='50 uL')
 
 recipe = Recipe().uses(triethylamine_50mM, plate)
 recipe.transfer(source=triethylamine_50mM, destination=plate[2:7, 2:11], quantity='10 uL')
 results = recipe.bake()
 triethylamine_50mM = results[triethylamine_50mM.name]
 plate = results[plate.name]
 
 recipe.visualize(what=plate, mode='final', unit='uL', timeframe=0)
 
 ```
 
 ![img.png](images/simple_visualization.png)
 
-Documentation is available at [ReadTheDocs](https://pyplate-hte.readthedocs.io/en/latest/).
+## Documentation
+
+Online documentation is available at [ReadTheDocs](https://pyplate-hte.readthedocs.io/en/latest/).  To build the documentation locally, please follow these steps:
+
+``make -C docs html``
+
+The resulting HTML files will be in `docs/build/html`.
+
+In order to build the documentation successfully, you must install the packages listed in docs/requirements.txt.  You can do this by running:
+
+``pip install -r docs/requirements.txt``
 
 ## License
 
-Licensed under the Apache License, Version 2.0 (the "License")
-You may obtain a copy of the License at https://www.apache.org/licenses/LICENSE-2.0
+Licensed under the [Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0) (the "License").
+
+## Contributors
+
+**PyPlate** was designed and written by James Marvin, Eugene Kwan, Corin Wagen, Aryamaan Dhomne, and Pravin Mahendran.
+
+## Getting Help
+
+Please open a GitHub issue!  We respond regularly.  Please also feel free to contribute!
```

### Comparing `pyplate-hte-0.4.1/pyplate/__init__.py` & `pyplate_hte-0.4.2/pyplate/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from pathlib import Path
 import os
 import yaml
 
-# import pyplate
-
 
 class Config:
     def __init__(self):
         file_path = None
         for path in [Path(os.environ.get('PYPLATE_CONFIG', '')), Path.home(), Path(os.path.dirname(__file__))]:
             path = path.joinpath('pyplate.yaml')
             if path.is_file():
@@ -29,18 +27,23 @@
         self.moles_display_unit = yaml_config['moles_display_unit']
         assert self.moles_display_unit[-3:] == 'mol'
         self.volume_storage_unit = yaml_config['volume_storage_unit']
         assert self.volume_storage_unit[-1] == 'L'
         self.volume_display_unit = yaml_config['volume_display_unit']
         assert self.volume_display_unit[-1] == 'L'
 
+        self.concentration_display_unit = yaml_config['concentration_display_unit']
+        # we can't use Unit to do a full check of the unit, so we just do a cursory check
+        assert ('/' in self.concentration_display_unit or self.concentration_display_unit[-1] == 'm' or
+                self.concentration_display_unit[-1] == 'M')
         self.default_solid_density = float(yaml_config['default_solid_density'])
         self.default_enzyme_density = float(yaml_config['default_enzyme_density'])
         self.default_weight_volume_units = yaml_config['default_weight_volume_units']
 
-
         self.default_colormap = yaml_config['default_colormap']
         self.default_diverging_colormap = yaml_config['default_diverging_colormap']
         self.precisions = yaml_config['precisions']
 
 
-from .pyplate import Substance, Container, Plate, Recipe
+# This has to be imported after Config is defined, otherwise there will be a circular import.
+from .pyplate import Substance, Container, Plate, Recipe, Unit, RecipeStep  # noqa: E402
+__all__ = ['Substance', 'Container', 'Plate', 'Recipe', 'Unit', 'Config', 'RecipeStep']
```

### Comparing `pyplate-hte-0.4.1/pyplate/experiment_design.py` & `pyplate_hte-0.4.2/pyplate/experiment_design.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Optional, List, Callable
+from typing import Optional, Callable
 
 from pyplate import Substance, Container
 import itertools
 
 
 class Factor:
     """"
@@ -182,16 +182,16 @@
                              f" do not match experimental space factors {self.factors}")
         for factor_name in experiment.factors:
             factor_object = self.get_factor(factor_name)
             if experiment[factor_name] not in factor_object.possible_values:
                 raise ValueError(f"Experiment factor {factor_name} value {experiment[factor_name]}"
                                  f" not in possible values {factor_object.possible_values}")
         if not self.factor_rules(experiment):
-            raise ValueError(f"Experiment does not satisfy factor rules, make sure you don't have any conflicting "
-                             f"factors.")
+            raise ValueError("Experiment does not satisfy factor rules, make sure you don't have any conflicting "
+                             "factors.")
         factor_combination = sorted(experiment.factors.items())
         self.experiments[factor_combination] = experiment
 
     def filter_experiments(self, filter_function: callable) -> None:
         """
         Filter the experiments in the experimental space. This is useful for
         removing experiments that do not meet certain criteria.
@@ -251,15 +251,15 @@
             ],
             [
                 [("Factor 1", "value 1"), ("Factor 2", "value 2"), ("Factor 3", "value 1")],
                 [("Factor 1", "value 1"), ("Factor 2", "value 2"), ("Factor 3", "value 2")],
             ],
             ...
         ]
-        
+
         Easy to use this to create dicts and thus experiments
         """
 
         # If needed form blocking combinations
         blocking_combinations = list(itertools.product(*[filtered_factors[name] for name in blocking_factors]))
 
         # Iterate over each combination of blocking factors
```

### Comparing `pyplate-hte-0.4.1/pyplate/pyplate.py` & `pyplate_hte-0.4.2/pyplate/pyplate.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,26 +31,26 @@
 # Allow typing reference while still building classes
 from __future__ import annotations
 
 from functools import cache
 from typing import Tuple, Dict, Iterable
 from copy import deepcopy, copy
 import numpy
+import numpy as np
 import pandas
+from tabulate import tabulate
 
 from pyplate.slicer import Slicer
 from . import Config
 
 config = Config()
 
 
 class Unit:
     """
-    @private
-
     Provides unit conversion utility functions.
     """
 
     @staticmethod
     def convert_prefix_to_multiplier(prefix: str) -> float:
         """
 
@@ -135,23 +135,23 @@
             raise ValueError("Concentration must be of the form '1 umol/mL'.")
         try:
             numerator[0] = float(numerator[0])
             if len(denominator) > 1:
                 numerator[0] /= float(denominator.pop(0))
         except ValueError as exc:
             raise ValueError("Value is not a float.") from exc
-        units = ('mol', 'L', 'g')
+        units = ('mol', 'L', 'g', 'U')
         for unit in units:
             if numerator[1].endswith(unit):
                 numerator[0] *= Unit.convert_prefix_to_multiplier(numerator[1][:-len(unit)])
                 numerator[1] = unit
             if denominator[0].endswith(unit):
                 numerator[0] /= Unit.convert_prefix_to_multiplier(denominator[0][:-len(unit)])
                 denominator[0] = unit
-        if numerator[1] not in ('U', 'mol', 'L', 'g') or denominator[0] not in ('mol', 'L', 'g'):
+        if numerator[1] not in ('U', 'mol', 'L', 'g') or denominator[0] not in ('U', 'mol', 'L', 'g'):
             raise ValueError("Concentration must be of the form '1 umol/mL'.")
         return round(numerator[0], config.internal_precision), numerator[1], denominator[0]
 
     @staticmethod
     def convert_from(substance: Substance, quantity: float, from_unit: str, to_unit: str) -> float:
         """
                     Convert quantity of substance between units.
@@ -169,70 +169,105 @@
         if not isinstance(substance, Substance):
             raise TypeError(f"Invalid type for substance, {type(substance)}")
         if not isinstance(quantity, (int, float)):
             raise TypeError("Quantity must be a float.")
         if not isinstance(from_unit, str) or not isinstance(to_unit, str):
             raise TypeError("Unit must be a str.")
 
-        if from_unit == 'U' and not substance.is_enzyme():
-            raise ValueError("Only enzymes can be measured in activity units. 'U'")
-
         for suffix in ['U', 'L', 'g', 'mol']:
             if from_unit.endswith(suffix):
                 prefix = from_unit[:-len(suffix)]
                 quantity *= Unit.convert_prefix_to_multiplier(prefix)
                 from_unit = suffix
                 break
+        else:  # suffix not found
+            raise ValueError(f"Invalid unit {from_unit}")
+
+        if from_unit == 'U' and not substance.is_enzyme():
+            raise ValueError("Only enzymes can be measured in activity units.")
+
+        for suffix in ['U', 'L', 'g', 'mol']:
+            if to_unit.endswith(suffix):
+                prefix = to_unit[:-len(suffix)]
+                to_unit = suffix
+                break
+        else:  # suffix not found
+            raise ValueError(f"Invalid unit {to_unit}")
 
         result = None
-        if substance.is_enzyme() and not to_unit.endswith('U'):
-            return 0
-        if to_unit.endswith('U'):
-            prefix = to_unit[:-1]
+
+        if to_unit == 'U':
             if not substance.is_enzyme():
                 return 0
-            if not from_unit == 'U':
-                raise ValueError("Enzymes can only be measured in activity units. 'U'")
-            result = quantity
-        elif to_unit.endswith('L'):
-            prefix = to_unit[:-1]
+            elif from_unit == 'mol':
+                return 0
+            elif from_unit == 'L':
+                # L * (1000 mL/L) * (U/mL)
+                result = quantity * 1000. * substance.density
+            elif from_unit == 'g':
+                # g * (U/g)
+                result = quantity * substance.specific_activity
+            elif from_unit == 'U':
+                result = quantity
+        elif to_unit == 'L':
             if from_unit == 'L':
                 result = quantity
             elif from_unit == 'mol':
+                if substance.is_enzyme():
+                    return 0
                 # mol * g/mol / (g/mL)
                 result_in_mL = quantity * substance.mol_weight / substance.density
-                result = result_in_mL / 1000
+                result = result_in_mL / 1000.
             elif from_unit == 'g':
-                # g / (g/mL)
-                result_in_mL = quantity / substance.density
-                result = result_in_mL / 1000
-        elif to_unit.endswith('mol'):
-            prefix = to_unit[:-3]
-            if from_unit == 'L':
-                value_in_mL = quantity * 1000
+                if substance.is_enzyme():
+                    # g * (U/g) / (U/mL) * (1 L / 1000 mL)
+                    result = quantity * substance.specific_activity / substance.density / 1000.
+                else:
+                    # g / (g/mL)
+                    result_in_mL = quantity / substance.density
+                    result = result_in_mL / 1000
+            elif from_unit == 'U':
+                if not substance.is_enzyme():
+                    return 0
+                # U / (U/mL) * (1 L / 1000 mL)
+                result = quantity / substance.density / 1000.
+        elif to_unit == 'mol':
+            if substance.is_enzyme():
+                return 0
+            if from_unit == 'U':
+                return 0
+            elif from_unit == 'L':
+                value_in_mL = quantity * 1000.  # L * mL/L
                 # mL * g/mL / (g/mol)
                 result = value_in_mL * substance.density / substance.mol_weight
             elif from_unit == 'mol':
                 result = quantity
             elif from_unit == 'g':
                 # g / (g/mol)
                 result = quantity / substance.mol_weight
-        elif to_unit.endswith('g'):
-            prefix = to_unit[:-1]
-            if from_unit == 'L':
-                value_in_mL = quantity * 1000
-                # mL * g/mL
-                result = value_in_mL * substance.density
+        elif to_unit == 'g':
+            if from_unit == 'U':
+                if not substance.is_enzyme():
+                    return 0
+                # U / (U/g)
+                result = quantity / substance.specific_activity
+            elif from_unit == 'L':
+                if substance.is_enzyme():
+                    # L * (1000 mL/L) * (U/mL) / (U/g)
+                    result = quantity * 1000. * substance.density / substance.specific_activity
+                else:
+                    # L * (1000 mL/L) * g/mL
+                    result = quantity * 1000. * substance.density
             elif from_unit == 'mol':
+                if substance.is_enzyme():
+                    return 0
                 # mol * g/mol
                 result = quantity * substance.mol_weight
             elif from_unit == 'g':
                 result = quantity
-        else:
-            raise ValueError("Only L, U, g, and mol are valid units.")
 
         assert result is not None, f"{substance} {quantity} {from_unit} {to_unit}"
 
         return result / Unit.convert_prefix_to_multiplier(prefix)
 
     @staticmethod
     def convert(substance: Substance, quantity: str, unit: str) -> float:
@@ -275,18 +310,18 @@
         if not isinstance(value, (int, float)):
             raise TypeError("Value must be a float.")
         if not isinstance(unit, str):
             raise TypeError("Unit must be a str.")
 
         if unit[-1] == 'L':
             prefix_value = Unit.convert_prefix_to_multiplier(unit[:-1])
-            result = value * prefix_value / Unit.convert_prefix_to_multiplier(config.volume_storage_unit[0])
+            result = value * prefix_value / Unit.convert_prefix_to_multiplier(config.volume_storage_unit[:-1])
         else:  # moles
             prefix_value = Unit.convert_prefix_to_multiplier(unit[:-3])
-            result = value * prefix_value / Unit.convert_prefix_to_multiplier(config.moles_storage_unit[0])
+            result = value * prefix_value / Unit.convert_prefix_to_multiplier(config.moles_storage_unit[:-3])
         return round(result, config.internal_precision)
 
     @staticmethod
     def convert_from_storage(value: float, unit: str) -> float:
         """
 
         Converts value from storage format.
@@ -303,17 +338,19 @@
             raise TypeError("Value must be a float.")
         if not isinstance(unit, str):
             raise TypeError("Unit must be a str.")
 
         if unit[-1] == 'L':
             prefix_value = Unit.convert_prefix_to_multiplier(unit[:-1])
             result = value * Unit.convert_prefix_to_multiplier(config.volume_storage_unit[0]) / prefix_value
-        else:  # moles
+        elif unit[-3:] == 'mol':  # moles
             prefix_value = Unit.convert_prefix_to_multiplier(unit[:-3])
             result = value * Unit.convert_prefix_to_multiplier(config.moles_storage_unit[0]) / prefix_value
+        else:
+            raise ValueError("Invalid unit.")
         return round(result, config.internal_precision)
 
     @staticmethod
     def convert_from_storage_to_standard_format(what: Substance | Container, quantity: float) -> Tuple[float, str]:
         """
         Converts a quantity of a substance or container to a standard format.
         Example: (water, 1e6) -> (18.015, 'mL'), (NaCl, 1e6) -> (58.443, 'g'), (Amylase, 1) -> (1, 'U')
@@ -328,29 +365,29 @@
         if isinstance(what, Substance):
             if what.is_enzyme():
                 unit = 'U'
             elif what.is_solid():
                 unit = 'g'
                 # convert moles to grams
                 # molecular weight is in g/mol
-                quantity *= Unit.convert_prefix_to_multiplier(config.moles_storage_unit[0]) * what.mol_weight
+                quantity *= Unit.convert_prefix_to_multiplier(config.moles_storage_unit[:-3]) * what.mol_weight
             elif what.is_liquid():
                 unit = 'L'
                 # convert moles to liters
                 # molecular weight is in g/mol
                 # density is in g/mL
-                quantity *= (Unit.convert_prefix_to_multiplier(config.moles_storage_unit[0])
+                quantity *= (Unit.convert_prefix_to_multiplier(config.moles_storage_unit[:-3])
                              * what.mol_weight / what.density / 1e3)
             else:
                 # This shouldn't happen.
                 raise TypeError("Invalid type for what.")
         elif isinstance(what, Container):
             # Assume the container contains a liquid
             unit = 'L'
-            quantity *= Unit.convert_prefix_to_multiplier(config.volume_storage_unit[0])
+            quantity *= Unit.convert_prefix_to_multiplier(config.volume_storage_unit[:-1])
         else:
             raise TypeError("Invalid type for what.")
 
         multiplier = 1
         while quantity < 1 and multiplier > 1e-6:
             quantity *= 1e3
             multiplier /= 1e3
@@ -391,14 +428,15 @@
         multiplier = max(multiplier, 1e-6)
 
         return value, {1: '', 1e-3: 'm', 1e-6: 'u'}[multiplier] + unit
 
     @staticmethod
     def calculate_concentration_ratio(solute: Substance, concentration: str, solvent: Substance) \
             -> Tuple[float, str, str]:
+        # TODO: eliminate this from dilute and tests.
         """
         Helper function for dealing with concentrations.
 
         Returns: ratio of moles or Activity Units per mole storage unit ('umol', etc.).
 
         """
         # Formulas used here are found in solution_formulas.rst
@@ -442,35 +480,24 @@
                 ratio = c * solvent.mol_weight / solvent.density / 1000.0
             else:
                 ratio = c
             # ratio can be multiplied by a stored value of moles to get number of U
             ratio *= Unit.convert_from_storage(1, 'mol')
         return ratio, numerator, denominator
 
-    @staticmethod
-    def calculate_concentration_ratio_moles(solute: Substance, quantity: str, solvent: Substance) \
-            -> Tuple[float, str, str]:
-        q, q_unit = Unit.parse_quantity(quantity)
-        if q_unit not in ('g', 'L', 'mol'):
-            raise ValueError("Invalid unit in quantity.")
-        if q_unit == 'g':
-            q /= solute.mol_weight
-        elif q_unit == 'L':
-            q *= solute.density
-        return Unit.calculate_concentration_ratio(solute, f"{q} mol", solvent)
-
 
 class Substance:
     """
     An abstract chemical or biological entity (e.g., reagent, enzyme, solvent, etc.). Immutable.
     Enzymes are assumed to require zero volume.
 
     Attributes:
         name: Name of substance.
         mol_weight: Molecular weight (g/mol).
+        specific_activity: Activity units per mass if `Substance` is an enzyme (U/g).
         density: Density if `Substance` is a liquid (g/mL).
         concentration: Calculated concentration if `Substance` is a liquid (mol/mL).
         molecule: `cctk.Molecule` if provided.
     """
 
     SOLID = 1
     LIQUID = 2
@@ -496,14 +523,15 @@
         if not isinstance(mol_type, int):
             raise TypeError("Type must be an int.")
         if len(name) == 0:
             raise ValueError("Name must not be empty.")
 
         self.name = name
         self._type = mol_type
+        self.specific_activity = None  # U/g
         self.mol_weight = self.concentration = None
         self.density = float('inf')
         self.molecule = molecule
 
     def __repr__(self):
         return f"{self.name} ({'SOLID' if self.is_solid() else 'LIQUID' if self.is_liquid() else 'ENZYME'})"
 
@@ -571,30 +599,51 @@
         substance = Substance(name, Substance.LIQUID, molecule)
         substance.mol_weight = mol_weight  # g / mol
         substance.density = density  # g / mL
         substance.concentration = density / mol_weight  # mol / mL
         return substance
 
     @staticmethod
-    def enzyme(name: str, molecule=None) -> Substance:
+    def enzyme(name: str, specific_activity: str, molecule=None) -> Substance:
         """
         Creates an enzyme.
 
         Arguments:
             name: Name of enzyme.
+            specific_activity: A ratio of activity units to mass ('10 U/g', '10 U/mg', '0.1 mg/U')
             molecule: (optional) A cctk.Molecule
 
         Returns: New substance.
 
         """
         if not isinstance(name, str):
             raise TypeError("Name must be a str.")
 
+        if not isinstance(specific_activity, str):
+            raise TypeError("Specific activity must be a str.")
+
+        try:
+            value, numerator, denominator = Unit.parse_concentration(specific_activity)
+        except Exception:
+            raise ValueError("Specific activity must be in U/g or g/U.")
+
+        if value < 0:
+            raise ValueError("Specific activity must be positive.")
+
         substance = Substance(name, Substance.ENZYME, molecule)
         substance.density = config.default_enzyme_density
+        value, numerator, denominator = Unit.parse_concentration(specific_activity)
+
+        if numerator == 'U' and denominator == 'g':
+            substance.specific_activity = value
+        elif numerator == 'g' and denominator == 'U':
+            substance.specific_activity = 1 / value
+        else:
+            raise ValueError("Specific activity must be in U/g or g/U.")
+
         return substance
 
     def is_solid(self) -> bool:
         """
         Return true if `Substance` is a solid.
         """
         return self._type == Substance.SOLID
@@ -699,19 +748,18 @@
 
         """
         if not isinstance(source, Substance):
             raise TypeError("Source must be a Substance.")
         if not isinstance(quantity, str):
             raise TypeError("Quantity must be a str.")
 
+        volume_to_add = Unit.convert(source, quantity, config.volume_storage_unit)
         if source.is_enzyme():
-            volume_to_add = 0
             amount_to_add = Unit.convert(source, quantity, 'U')
         else:
-            volume_to_add = Unit.convert(source, quantity, config.volume_storage_unit)
             amount_to_add = Unit.convert(source, quantity, config.moles_storage_unit)
         if self.volume + volume_to_add > self.max_volume:
             raise ValueError("Exceeded maximum volume")
         self.volume = round(self.volume + volume_to_add, config.internal_precision)
         self.contents[source] = round(self.contents.get(source, 0) + amount_to_add, config.internal_precision)
 
     def _transfer(self, source_container: Container, quantity: str) -> Tuple[Container, Container]:
@@ -737,22 +785,30 @@
                 raise ValueError(f"Not enough mixture left in source container ({source_container.name}). " +
                                  f"Only {Unit.convert_from_storage(source_container.volume, 'mL')} mL available, " +
                                  f"{Unit.convert_from_storage(volume_to_transfer, 'mL')} mL needed.")
             ratio = volume_to_transfer / source_container.volume
 
         elif unit == 'g':
             mass_to_transfer = round(quantity_to_transfer, config.internal_precision)
-            total_mass = sum(Unit.convert(substance, f"{amount} {config.moles_storage_unit}", "g") for
-                             substance, amount in source_container.contents.items())
+            total_mass = 0
+            for substance, amount in source_container.contents.items():
+                source_unit = 'U' if substance.is_enzyme() else config.moles_storage_unit
+                total_mass += Unit.convert_from(substance, amount, source_unit, "g")
             ratio = mass_to_transfer / total_mass
         elif unit == 'mol':
             moles_to_transfer = Unit.convert_to_storage(quantity_to_transfer, 'mol')
             total_moles = sum(amount for substance, amount in source_container.contents.items()
                               if not substance.is_enzyme())
             ratio = moles_to_transfer / total_moles
+        elif unit == 'U':
+            total_activity = sum(amount for substance, amount in source_container.contents.items()
+                                 if substance.is_enzyme())
+            if total_activity == 0:
+                raise ValueError("There are no enzymes in the source container.")
+            ratio = quantity_to_transfer / total_activity
         else:
             raise ValueError("Invalid quantity unit.")
 
         source_container, to = deepcopy(source_container), deepcopy(self)
         for substance, amount in source_container.contents.items():
             to_transfer = amount * ratio
             to.contents[substance] = round(to.contents.get(substance, 0) + to_transfer,
@@ -764,26 +820,33 @@
             if source_container.contents[substance] == -0.0:
                 source_container.contents[substance] = 0.0
         if source_container.has_liquid():
             transfer = Unit.convert_from_storage(ratio * source_container.volume, 'L')
             transfer, unit = Unit.get_human_readable_unit(transfer, 'L')
         else:
             # total mass in source container times ratio
-            mass = sum(Unit.convert(substance, f"{amount} {config.moles_storage_unit if not substance.is_enzyme() else 'U'}",
+            mass = sum(Unit.convert(substance,
+                                    f"{amount} {config.moles_storage_unit if not substance.is_enzyme() else 'U'}",
                                     "mg") for substance, amount in source_container.contents.items())
             transfer, unit = Unit.get_human_readable_unit(mass * ratio, 'mg')
         precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
         to.instructions += f"\nTransfer {round(transfer, precision)} {unit} of {source_container.name} to {to.name}"
-        to.volume = round(sum(Unit.convert(substance, f"{amount} {config.moles_storage_unit}", config.volume_storage_unit) for
-                              substance, amount in to.contents.items()), config.internal_precision)
+        to.volume = 0
+        for substance, amount in to.contents.items():
+            unit = 'U' if substance.is_enzyme() else config.moles_storage_unit
+            to.volume += Unit.convert(substance, f"{amount} {unit}", config.volume_storage_unit)
+        to.volume = round(to.volume, config.internal_precision)
         if to.volume > to.max_volume:
             raise ValueError(f"Exceeded maximum volume in {to.name}.")
-        source_container.volume = sum(Unit.convert(substance, f"{amount} {config.moles_storage_unit}", config.volume_storage_unit)
-                                      for substance, amount in source_container.contents.items())
+        source_container.volume = 0
+        for substance, amount in source_container.contents.items():
+            unit = 'U' if substance.is_enzyme() else config.moles_storage_unit
+            source_container.volume += Unit.convert(substance, f"{amount} {unit}", config.volume_storage_unit)
         source_container.volume = round(source_container.volume, config.internal_precision)
+
         return source_container, to
 
     def _transfer_slice(self, source_slice: Plate | PlateSlicer, quantity: str) -> Tuple[Plate, Container]:
         """
         Move quantity ('10 mL', '5 mg') from each well in a slice to self.
 
         Arguments:
@@ -808,40 +871,69 @@
         source_slice.plate = deepcopy(source_slice.plate)
 
         to_array = [to]
         source_slice.apply(helper_func)
         to = to_array[0]
         return source_slice.plate, to
 
-    def __repr__(self):
-        # TODO: Make this more readable/beautiful
-        contents = []
-        for substance, value in sorted(self.contents.items(), key=lambda elem: (elem[0]._type, -elem[1])):
-            if substance.is_enzyme():
-                contents.append(f"{substance}: {value} U")
-            else:
-                value, unit = Unit.get_human_readable_unit(Unit.convert_from_storage(value, 'mol'), 'mmol')
-                precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
-                contents.append(
-                    f"{substance}: {round(value, precision)} {unit}")
+    @cache
+    def dataframe(self) -> pandas.DataFrame:
+        df = pandas.DataFrame(columns=['Volume', 'Mass', 'Moles', 'U'])
+        if self.max_volume == float('inf'):
+            df.loc['Maximum Volume'] = ['∞', '-', '-', '-']
+        else:
+            volume, unit = Unit.convert_from_storage_to_standard_format(self, self.max_volume)
+            volume = round(volume,
+                           config.precisions[unit] if unit in config.precisions else config.precisions['default'])
+            df.loc['Maximum Volume'] = [volume, '-', '-', '-']
+        totals = {'L': 0, 'g': 0, 'mol': 0, 'U': 0}
+        for substance, value in self.contents.items():
+            columns = []
+            for unit in ['L', 'g', 'mol', 'U']:
+                if unit == 'mol' and substance.is_enzyme():
+                    columns.append('-')
+                elif unit == 'U' and not substance.is_enzyme():
+                    columns.append('-')
+                else:
+                    from_unit = config.moles_storage_unit if not substance.is_enzyme() else 'U'
+                    converted_value = Unit.convert_from(substance, value, from_unit, unit)
+                    totals[unit] += converted_value
+                    converted_value, unit = Unit.get_human_readable_unit(converted_value, unit)
+                    precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+                    columns.append(f"{round(converted_value, precision)} {unit}")
+            df.loc[substance.name] = columns
+        columns = []
+        for unit in ['L', 'g', 'mol', 'U']:
+            value = totals[unit]
+            value, unit = Unit.get_human_readable_unit(value, unit)
+            precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+            columns.append(f"{round(value, precision)} {unit}")
+        df.loc['Total'] = columns
+
+        df.columns.name = self.name
+        return df
+
+    @cache
+    def _repr_html_(self):
+        return self.dataframe().to_html(notebook=True)
 
-        max_volume = ('/' + str(Unit.convert_from_storage(self.max_volume, 'mL'))) \
-            if self.max_volume != float('inf') else ''
-        return f"Container ({self.name}) ({Unit.convert_from_storage(self.volume, 'mL')}" + \
-            f"{max_volume} mL of ({contents})"
+    @cache
+    def __repr__(self):
+        df = self.dataframe()
+        return tabulate(df, headers=[self.name] + list(df.columns), tablefmt='pretty')
 
     @cache
     def has_liquid(self) -> bool:
         """
         Returns: True if any substance in the container is a liquid.
         """
         return any(substance.is_liquid() for substance in self.contents)
 
     @cache
-    def substances(self):
+    def get_substances(self):
         """
 
         Returns: A set of substances present in the container.
 
         """
         return set(self.contents.keys())
 
@@ -897,21 +989,31 @@
         if not isinstance(solute, Substance):
             raise TypeError("Solute must be a Substance.")
         if not isinstance(units, str):
             raise TypeError("Units must be a str.")
 
         mult, *units = Unit.parse_concentration('1 ' + units)
 
-        numerator = Unit.convert(solute, f"{self.contents.get(solute, 0)} {config.moles_storage_unit}", units[0])
+        if solute.is_enzyme():
+            numerator = Unit.convert_from(solute, self.contents.get(solute, 0), 'U', units[0])
+        else:
+            numerator = Unit.convert_from(solute, self.contents.get(solute, 0), config.moles_storage_unit, units[0])
+
+        if numerator == 0:
+            return 0
+
         if units[1].endswith('L'):
-            denominator = Unit.convert_from_storage(self.volume, units[1])
+            denominator = self.get_volume(units[1])
         else:
-            denominator = sum(
-                Unit.convert(substance, f"{amount} {config.moles_storage_unit}", units[1]) for substance, amount in
-                self.contents.items())
+            denominator = 0
+            for substance, amount in self.contents.items():
+                if substance.is_enzyme():
+                    denominator += Unit.convert_from(substance, amount, 'U', units[1])
+                else:
+                    denominator += Unit.convert_from(substance, amount, config.moles_storage_unit, units[1])
 
         return round(numerator / denominator / mult, config.internal_precision)
 
     def get_volume(self, unit: str = None) -> float:
         """
         Get the volume of the container.
 
@@ -926,105 +1028,169 @@
 
         if not isinstance(unit, str):
             raise TypeError("Unit must be a str.")
 
         return Unit.convert_from_storage(self.volume, unit)
 
     @staticmethod
-    def create_solution(solute: Substance, solvent: Substance, name: str = None, **kwargs) -> Container:
+    def create_solution(solute: Substance | Iterable[Substance], solvent: Substance | Container,
+                        name: str = None, **kwargs) -> Container:
         """
         Create a solution.
 
         Two out of concentration, quantity, and total_quantity must be specified.
 
+        Multiple solutes can be, optionally, provided as a list. Each solute will have the desired concentration
+        or quantity in the final solution.
+
+        If one value is specified for concentration or quantity and multiple solutes are provided, the value will be
+        used for all solutes.
+
         Arguments:
-            solute: What to dissolve.
-            solvent: What to dissolve with.
+            solute: What to dissolve. Can be a single Substance or a list of Substances.
+            solvent: What to dissolve with. Can be a Substance or a Container.
             name: Optional name for new container.
-            concentration: Desired concentration. ('1 M', '0.1 umol/10 uL', etc.)
-            quantity: Desired quantity of solute. ('3 mL', '10 g')
+            concentration: Desired concentration(s). ('1 M', '0.1 umol/10 uL', etc.)
+            quantity: Desired quantity of solute(s). ('3 mL', '10 g')
             total_quantity: Desired total quantity. ('3 mL', '10 g')
 
 
         Returns:
             New container with desired solution.
         """
 
-        if not isinstance(solute, Substance):
-            raise TypeError("Solute must be a Substance.")
-        if not isinstance(solvent, Substance):
-            raise TypeError("Solvent must be a Substance.")
+        if not isinstance(solvent, (Substance, Container)):
+            raise TypeError("Solvent must be a Substance or a Container.")
         if name and not isinstance(name, str):
             raise TypeError("Name must be a str.")
 
-        if 'concentration' in kwargs and not isinstance(kwargs['concentration'], str):
-            raise TypeError("Concentration must be a str.")
-        if 'quantity' in kwargs and not isinstance(kwargs['quantity'], str):
-            raise TypeError("Quantity must be a str.")
-        if 'total_quantity' in kwargs and not isinstance(kwargs['total_quantity'], str):
-            raise TypeError("Total quantity must be a str.")
-        if ('concentration' in kwargs) + ('total_quantity' in kwargs) + ('quantity' in kwargs) != 2:
-            raise ValueError("Must specify two values out of concentration, quantity, and total quantity.")
+        if isinstance(solute, Substance):
+            solute = [solute]
+        elif not isinstance(solute, list) or any(not isinstance(substance, Substance) for substance in solute):
+            raise TypeError("Solute(s) must be a Substance.")
+
+        concentration = kwargs.get('concentration', None)
+        quantity = kwargs.get('quantity', None)
+        total_quantity = kwargs.get('total_quantity', None)
 
-        if not name:
-            name = f"solution of {solute.name} in {solvent.name}"
+        original_solvent = solvent
+        if isinstance(solvent, Container):
+            # Calculate mol_weight and density of solvent
+            # get total mass of solvent
+            total_mass = sum(Unit.convert_from(substance, amount, 'U' if substance.is_enzyme() else 'mol', 'g')
+                             for substance, amount in solvent.contents.items())
+            total_moles = Unit.convert_from_storage(sum(amount for substance, amount in solvent.contents.items()
+                                                        if not substance.is_enzyme()), 'mol')
+            total_volume = solvent.get_volume('mL')
+            if total_moles == 0 or total_volume == 0:
+                raise ValueError("Solvent must contain a non-zero amount of substance.")
+            # mol_weight = g/mol, density = g/mL
+            solvent = Substance.liquid('fake solvent',
+                                       mol_weight=total_mass / total_moles, density=total_mass / total_volume)
 
-        if 'concentration' in kwargs and 'total_quantity' in kwargs:
-            concentration = kwargs['concentration']
-            total_quantity = kwargs['total_quantity']
-            quantity, quantity_unit = Unit.parse_quantity(total_quantity)
-            if quantity <= 0:
-                raise ValueError("Quantity must be positive.")
+        if (concentration is not None) + (quantity is not None) + (total_quantity is not None) != 2:
+            raise ValueError("Must specify two values out of concentration, quantity, and total quantity.")
 
-            ratio, numerator, denominator = Unit.calculate_concentration_ratio(solute, concentration, solvent)
+        if total_quantity and not isinstance(total_quantity, str):
+            raise TypeError("Total quantity must be a str.")
 
-            if ratio <= 0:
-                raise ValueError("Solution is impossible to create.")
+        if not name:
+            name = f"Solution of {','.join(substance.name for substance in solute)} in {solvent.name}"
 
-            if numerator == 'U':
-                if not solute.is_enzyme():
-                    raise TypeError("Solute must be an enzyme.")
-                solvent_quantity = Unit.convert(solvent, f"{quantity} {quantity_unit}", config.moles_storage_unit)
-                units = ratio * solvent_quantity
-                return Container(name,
-                                 initial_contents=((solute, f"{units} U"), (solvent, f"{quantity} {quantity_unit}")))
-
-            if quantity_unit == 'g':
-                ratio *= solute.mol_weight / solvent.mol_weight
-            elif quantity_unit == 'mol':
-                pass
-            elif quantity_unit == 'L':
-                ratio *= (solute.mol_weight / solute.density) / (solvent.mol_weight / solvent.density)
-            else:
-                raise ValueError("Invalid quantity unit.")
+        def convert_one(substance: Substance, u: str) -> float:
+            """ Converts 1 mol or U to unit `u` for a given substance. """
+            return Unit.convert_from(substance, 1, 'U' if substance.is_enzyme() else 'mol', u)
+
+        # result of linalg.solve will be moles (or 'U') for all solutes solvent
+
+        n = len(solute)
+        a = numpy.zeros((n * 2, n + 1), dtype=float)
+        b = numpy.zeros(n * 2, dtype=float)
+        index = 0
+        identity = numpy.identity(n + 1)[0]
+        if concentration is not None:
+            if isinstance(concentration, str):
+                concentration = [concentration] * len(solute)
+            elif not isinstance(concentration, Iterable):
+                raise TypeError("Concentration(s) must be a str.")
+            bottom_arrays = {}
+            for i, (c, substance) in enumerate(zip(concentration, solute)):
+                if not isinstance(c, str):
+                    raise TypeError("Concentration(s) must be a str.")
+                try:
+                    c, numerator, denominator = Unit.parse_concentration(c)
+                except ValueError:
+                    raise ValueError(f"Invalid concentration. ({c})")
+
+                if denominator not in bottom_arrays:
+                    bottom = numpy.array(list(convert_one(substance, denominator) for substance in solute + [solvent]))
+                    bottom_arrays[denominator] = bottom
+                else:
+                    bottom = bottom_arrays[denominator]
 
-            # x is quantity of solute in moles, y is quantity of solvent in moles
+                # c = top/bottom
+                a[index] = c * bottom - numpy.roll(identity, i) * convert_one(substance, numerator)
+                index += 1
+
+        if quantity is not None:
+            if isinstance(quantity, str):
+                quantity = [quantity] * len(solute)
+            elif not isinstance(quantity, Iterable):
+                raise TypeError("Quantity(s) must be a str.")
+            for i, (q, substance) in enumerate(zip(quantity, solute)):
+                if not isinstance(q, str):
+                    raise TypeError("Quantity(s) must be a str.")
+                q, unit = Unit.parse_quantity(q)
+                a[index] = numpy.roll(identity, i) * convert_one(substance, unit)
+                b[index] = q
+                index += 1
+
+        if total_quantity is not None:
+            total_quantity, total_quantity_unit = Unit.parse_quantity(total_quantity)
+            a[index] = numpy.array(
+                list(convert_one(substance, total_quantity_unit) for substance in solute + [solvent]))
+            b[index] = total_quantity
 
-            y = quantity / (1 + ratio)
-            x = quantity - y
+        xs = numpy.linalg.solve(a[:n + 1], b[:n + 1])
+        if any(x <= 0 for x in xs):
+            raise ValueError("Solution is impossible to create.")
 
-            assert x >= 0 and y >= 0
-            solution = Container(name,
-                                 initial_contents=((solute, f"{x} {quantity_unit}"), (solvent, f"{y} {quantity_unit}")))
-            return solution
-        if 'quantity' in kwargs and 'total_quantity' in kwargs:
-            result = Container(name, initial_contents=[(solute, kwargs['quantity'])])
-            result = result.fill_to(solvent, kwargs['total_quantity'])
-        else:  # 'quantity' and 'concentration'
-            concentration = Unit.calculate_concentration_ratio(solute, kwargs['concentration'], solvent)
-            quantity = Unit.convert(solute, kwargs['quantity'], concentration[1])
-            result = Container(name, initial_contents=[(solute, kwargs['quantity'])])
-            result._self_add(solvent, f"{quantity / concentration[0]} {concentration[1]}")
-        contents = []
-        for substance, value in result.contents.items():
-            value, unit = Unit.convert_from_storage_to_standard_format(substance, value)
-            precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
-            contents.append(f"{round(value, precision)} {unit} of {substance.name}")
-        result.instructions = "Add " + ", ".join(contents) + " to a container."
-        return result
+        for i in range(len(a)):
+            if abs(sum(a[i] * xs) - b[i]) > 1e-6:
+                raise ValueError("Solution is impossible to create.")
+
+        initial_contents = list((substance, f"{x} {'U' if substance.is_enzyme() else 'mol'}") for x, substance in
+                                zip(xs, solute + [solvent]))
+        if isinstance(original_solvent, Container):
+            result = Container(name, initial_contents=initial_contents[:-1])
+            contents = []
+            for substance, value in result.contents.items():
+                value, unit = Unit.convert_from_storage_to_standard_format(substance, value)
+                precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+                contents.append(f"{round(value, precision)} {unit} of {substance.name}")
+            _, solvent_amount = initial_contents[-1]
+            solvent_volume = Unit.convert_from(solvent, xs[-1], 'mol', 'L')
+            solvent_volume, volume_unit = Unit.get_human_readable_unit(solvent_volume, 'L')
+            solvent_volume = round(solvent_volume,
+                                   config.precisions[volume_unit] if volume_unit in config.precisions else
+                                   config.precisions['default'])
+
+            original_solvent, result = Container.transfer(original_solvent, result, solvent_amount)
+            result.instructions = ("Add " + ", ".join(contents) +
+                                   f" to {solvent_volume} {volume_unit} of {original_solvent.name}.")
+            return original_solvent, result
+        else:
+            result = Container(name, initial_contents=initial_contents)
+            contents = []
+            for substance, value in result.contents.items():
+                value, unit = Unit.convert_from_storage_to_standard_format(substance, value)
+                precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+                contents.append(f"{round(value, precision)} {unit} of {substance.name}")
+            result.instructions = "Add " + ", ".join(contents) + " to a container."
+            return result
 
     @staticmethod
     def create_solution_from(source: Container, solute: Substance, concentration: str, solvent: Substance | Container,
                              quantity: str, name=None) -> (Tuple[Container, Container] |
                                                            Tuple[Container, Container, Container]):
         """
         Create a diluted solution from an existing solution or solutions.
@@ -1240,17 +1406,17 @@
             # Note: this copies the container twice
             destination = deepcopy(self)
             destination.name = name
         else:
             destination = self
         needed_umoles = f"{required_umoles} umol"
         result = destination._add(solvent, needed_umoles)
-        needed_volume, unit = Unit.get_human_readable_unit(Unit.convert(solvent, needed_umoles, 'umol'), 'L')
+        needed_volume, unit = Unit.get_human_readable_unit(Unit.convert(solvent, needed_umoles, 'L'), 'L')
         precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
-        result.instructions += f"Dilute with {round(needed_volume, precision)} {unit} of {solvent.name}."
+        result.instructions += f"\nDilute with {round(needed_volume, precision)} {unit} of {solvent.name}."
         return result
 
     def fill_to(self, solvent: Substance, quantity: str) -> Container:
         """
         Fills container with `solvent` up to `quantity`.
 
         Args:
@@ -1275,15 +1441,15 @@
                                for substance, value in self.contents.items() if not substance.is_enzyme())
 
         required_quantity = quantity - current_quantity
         result = self._add(solvent, f"{required_quantity} {quantity_unit}")
         required_volume = Unit.convert(solvent, f"{required_quantity} {quantity_unit}", 'L')
         required_volume, unit = Unit.get_human_readable_unit(required_volume, 'L')
         precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
-        result.instructions += f"Fill with {round(required_volume, precision)} {unit} of {solvent.name}."
+        result.instructions += f"\nFill with {round(required_volume, precision)} {unit} of {solvent.name}."
         return result
 
 
 class Plate:
     """
     A spatially ordered collection of Containers, like a 96 well plate.
     The spatial arrangement must be rectangular. Immutable.
@@ -1389,49 +1555,53 @@
             numpy.ndarray of volumes for each well in desired unit.
 
         """
 
         # Arguments are type checked in PlateSlicer.volumes
         return self[:].get_volumes(substance=substance, unit=unit)
 
-    def substances(self) -> set[Substance]:
+    def get_substances(self) -> set[Substance]:
         """
 
         Returns: A set of substances present in the slice.
 
         """
-        return self[:].substances()
+        return self[:].get_substances()
 
     def get_moles(self, substance: (Substance | Iterable[Substance]), unit: str = None) -> numpy.ndarray:
         """
 
         Arguments:
             unit: unit to return moles in. ('mol', 'mmol', 'umol', etc.)
             substance: Substance to display moles of.
 
         Returns: moles of substance in each well.
         """
 
         # Arguments are type checked in PlateSlicer.moles
         return self[:].get_moles(substance=substance, unit=unit)
 
-    def dataframe(self, unit: str, substance: (str | Substance | Iterable[Substance]) = 'all', cmap: str = None) \
+    def dataframe(self, unit: str = None, substance: (str | Substance | Iterable[Substance]) = 'all',
+                  cmap: str = None, highlight=False) \
             -> pandas.io.formats.style.Styler:
         """
 
         Arguments:
             unit: unit to return quantities in.
             substance: (optional) Substance or Substances to display quantity of.
             cmap: Colormap to shade dataframe with.
+            highlight: Highlight all wells.
 
         Returns: Shaded dataframe of quantities in each well.
 
         """
         # Types are checked in PlateSlicer.dataframe
-        return self[:].dataframe(substance=substance, unit=unit, cmap=cmap)
+        if unit is None:
+            unit = config.volume_display_unit
+        return self[:].dataframe(substance=substance, unit=unit, cmap=cmap, highlight=highlight)
 
     def get_volume(self, unit: str = 'uL') -> float:
         """
         Arguments:
             unit: unit to return volumes in.
 
         Returns: total volume stored in slice in uL.
@@ -1483,38 +1653,106 @@
         Returns: New Plate with desired final `quantity` in each well.
 
         """
         return self[:].fill_to(solvent, quantity)
 
 
 class RecipeStep:
-    def __init__(self, operator, frm, to, *operands):
+    """
+    Stores information about a single step in a recipe.
+
+    .. document private functions
+    .. automethod:: _repr_html_
+    """
+
+    def __init__(self, recipe: Recipe, operator: str, frm: Container | PlateSlicer | Plate,
+                 to: Container | PlateSlicer | Plate, *operands):
+        self.frm_slice = None
+        self.to_slice = None
+        self.recipe = recipe
         self.objects_used = set()
         self.substances_used = set()
         self.operator = operator
         self.frm: list[Container | PlateSlicer | Plate | None] = [frm]
         self.to: list[Container | PlateSlicer | Plate] = [to]
         self.trash = {}
         self.operands = operands
         self.instructions = ""
 
+    def _repr_html_(self):
+        """
+
+        Returns: HTML representation of the step.
+
+        """
+        precision = config.precisions[config.volume_display_unit] if config.volume_display_unit in config.precisions \
+            else config.precisions['default']
+        source_visual = None
+        if isinstance(self.frm[0], Container):
+            source_visual = self.frm[0].dataframe()
+        elif isinstance(self.frm[0], Plate):
+            if self.frm_slice is None:
+                source_visual = self.frm[0].dataframe()
+            else:
+                frm_slice: PlateSlicer = copy(self.frm_slice)
+                frm_slice.plate = self.frm[0]
+                source_visual = frm_slice.dataframe(highlight=True)
+        destination_visual = None
+        if isinstance(self.to[0], Container):
+            destination_visual = self.to[1].dataframe()
+        elif isinstance(self.to[0], Plate):
+            if self.to_slice is None:
+                before = self.to[0].dataframe()
+                after = self.to[1].dataframe()
+            else:
+                to_slice: PlateSlicer = copy(self.to_slice)
+                to_slice.plate = self.to[0]
+                before = to_slice.dataframe()
+                to_slice.plate = self.to[1]
+                after = to_slice.dataframe()
+            delta_data = after.data - before.data
+            destination_visual = delta_data.style.format(precision=precision).use(before.export())
+            vmin = min(delta_data.min().min(), 0)
+            vmax = Unit.convert_from_storage(self.to[0].max_volume_per_well, config.volume_display_unit)
+            cmap = config.default_colormap if vmin >= 0 and vmax >= 0 else config.default_diverging_colormap
+            destination_visual = destination_visual.background_gradient(cmap=cmap, vmin=vmin, vmax=vmax)
+
+        if isinstance(source_visual, pandas.DataFrame):
+            source_visual = source_visual.style
+        if isinstance(destination_visual, pandas.DataFrame):
+            destination_visual = destination_visual.style
+
+        label = f"Destination (delta) ({config.volume_display_unit}): " if isinstance(self.to[0], Plate) else "Destination: "
+        destination_visual.set_caption(label + self.to[0].name)
+        if source_visual is None:
+            return self.instructions + '<br/>' + destination_visual.to_html()
+
+        source_visual.set_table_attributes("style='display:inline; margin-right:20px'")
+        if isinstance(self.frm[0], Plate):
+            source_visual.set_caption(f"Source (initial) ({config.volume_display_unit}): {self.frm[0].name}")
+        else:
+            source_visual.set_caption(f"Source (initial): {self.frm[0].name}")
+        destination_visual.set_table_attributes("style='display:inline'")
+        return self.instructions + '<br/>' + source_visual.to_html() + destination_visual.to_html()
+
 
 class Recipe:
     """
     A list of instructions for transforming one set of containers into another. The intended workflow is to declare
     the source containers, enumerate the desired transformations, and call recipe.bake(). The name of each object used
     by the Recipe must be unique. This method will ensure that all solid and liquid handling instructions are valid.
     If they are indeed valid, then the updated containers will be generated. Once recipe.bake() has been called, no
     more instructions can be added and the Recipe is considered immutable.
 
     Attributes:
         locked (boolean): Is the recipe locked from changes?
         steps (list): A list of steps to be completed upon bake() bring called.
         used (list): A list of Containers and Plates to be used in the recipe.
-        results (list): A dictionary used in bake to return the mutated objects.
+        results (dict): A dictionary used in bake to return the mutated objects.
+        stages (dict): A dictionary of stages in the recipe.
     """
 
     def __init__(self):
         self.results: dict[str, Container | Plate | PlateSlicer] = {}
         self.steps: list[RecipeStep] = []
         self.stages: dict[str, slice] = {'all': slice(None, None)}
         self.current_stage = 'all'
@@ -1572,15 +1810,16 @@
                 if not all(isinstance(elem, (Container, Plate)) for elem in unpacked):
                     raise TypeError("Invalid type in iterable.")
                 self.uses(*unpacked)
             else:
                 raise TypeError("Invalid type.")
         return self
 
-    def transfer(self, source: Container, destination: Container | Plate | PlateSlicer, quantity: str) -> None:
+    def transfer(self, source: Container | Plate | PlateSlicer, destination: Container | Plate | PlateSlicer,
+                 quantity: str) -> None:
         """
         Adds a step to the recipe which will move quantity from source to destination.
         Note that all Substances in the source will be transferred in proportion to their respective ratios.
 
         """
         if self.locked:
             raise RuntimeError("This recipe is locked.")
@@ -1595,15 +1834,15 @@
             raise ValueError(f"Destination {destination_name} has not been previously declared for use.")
         if not isinstance(quantity, str):
             raise TypeError("Volume must be a str. ('5 mL')")
         if isinstance(source, Plate):
             source = source[:]
         if isinstance(destination, Plate):
             destination = destination[:]
-        self.steps.append(RecipeStep('transfer', source, destination, quantity))
+        self.steps.append(RecipeStep(self, 'transfer', source, destination, quantity))
 
     def create_container(self, name: str, max_volume: str = 'inf L',
                          initial_contents: Iterable[tuple[Substance, str]] | None = None) -> Container:
 
         """
         Adds a step to the recipe which creates a container.
 
@@ -1630,30 +1869,37 @@
             for substance, quantity in initial_contents:
                 if not isinstance(substance, Substance):
                     raise TypeError("Containers can only be created from substances.")
                 if not isinstance(quantity, str):
                     raise TypeError("Quantity must be a str. ('10 mL')")
         new_container = Container(name, max_volume)
         self.uses(new_container)
-        self.steps.append(RecipeStep('create_container', None, new_container, max_volume, initial_contents))
+        self.steps.append(RecipeStep(self, 'create_container', None, new_container, max_volume, initial_contents))
 
         return new_container
 
-    def create_solution(self, solute, solvent, name=None, **kwargs) -> Container:
+    def create_solution(self, solute: Substance | Iterable[Substance], solvent: Substance | Container,
+                        name=None, **kwargs) -> Container:
         """
         Adds a step to the recipe which creates a solution.
 
         Two out of concentration, quantity, and total_quantity must be specified.
 
+        Multiple solutes can be, optionally, provided as a list. Each solute will have the desired concentration
+        or quantity in the final solution.
+
+        If one value is specified for concentration or quantity and multiple solutes are provided, the value will be
+        used for all solutes.
+
         Arguments:
-            solute: What to dissolve.
-            solvent: What to dissolve with.
+            solute: What to dissolve. Can be a single Substance or an iterable of Substances.
+            solvent: What to dissolve with. Can be a Substance or a Container.
             name: Optional name for new container.
-            concentration: Desired concentration. ('1 M', '0.1 umol/10 uL', etc.)
-            quantity: Desired quantity of solute. ('3 mL', '10 g')
+            concentration: Desired concentration(s). ('1 M', '0.1 umol/10 uL', etc.)
+            quantity: Desired quantity of solute(s). ('3 mL', '10 g')
             total_quantity: Desired total quantity. ('3 mL', '10 g')
 
 
         Returns:
             A new Container so that it may be used in later recipe steps.
         """
 
@@ -1674,15 +1920,15 @@
             raise ValueError("Must specify two values out of concentration, quantity, and total quantity.")
 
         if not name:
             name = f"solution of {solute.name} in {solvent.name}"
 
         new_container = Container(name)
         self.uses(new_container)
-        self.steps.append(RecipeStep('solution', None, new_container, solute, solvent, kwargs))
+        self.steps.append(RecipeStep(self, 'solution', None, new_container, solute, solvent, kwargs))
 
         return new_container
 
     def create_solution_from(self, source: Container, solute: Substance, concentration: str, solvent: Substance,
                              quantity: str, name=None) -> Container:
         """
         Adds a step to create a diluted solution from an existing solution.
@@ -1722,15 +1968,16 @@
 
         new_ratio, numerator, denominator = Unit.calculate_concentration_ratio(solute, concentration, solvent)
         if new_ratio <= 0:
             raise ValueError("Solution is impossible to create.")
 
         new_container = Container(name, max_volume=f"{source.max_volume} {config.volume_storage_unit}")
         self.uses(new_container)
-        self.steps.append(RecipeStep('solution_from', source, new_container, solute, concentration, solvent, quantity))
+        self.steps.append(RecipeStep(self, 'solution_from', source, new_container,
+                                     solute, concentration, solvent, quantity))
 
         return new_container
 
     def remove(self, destination: Container | Plate | PlateSlicer, what=Substance.LIQUID) -> None:
         """
         Adds a step to removes substances from destination.
 
@@ -1744,15 +1991,15 @@
                 raise ValueError(f"Destination {destination.plate.name} has not been previously declared for use.")
         elif isinstance(destination, (Container, Plate)):
             if destination.name not in self.results:
                 raise ValueError(f"Destination {destination.name} has not been previously declared for use.")
         else:
             raise TypeError(f"Invalid destination type: {type(destination)}")
 
-        self.steps.append(RecipeStep('remove', None, destination, what))
+        self.steps.append(RecipeStep(self, 'remove', None, destination, what))
 
     def dilute(self, destination: Container, solute: Substance,
                concentration: str, solvent: Substance, new_name=None) -> None:
         """
         Adds a step to dilute `solute` in `destination` to `concentration`.
 
         Args:
@@ -1782,17 +2029,17 @@
         if ratio <= 0:
             raise ValueError("Concentration is impossible to create.")
 
         if solute.is_enzyme():
             # TODO: Support this.
             raise ValueError("Not currently supported.")
 
-        self.steps.append(RecipeStep('dilute', None, destination, solute, concentration, solvent, new_name))
+        self.steps.append(RecipeStep(self, 'dilute', None, destination, solute, concentration, solvent, new_name))
 
-    def fill_to(self, destination: Container, solvent: Substance, quantity: str) -> None:
+    def fill_to(self, destination: Container | Plate | PlateSlicer, solvent: Substance, quantity: str) -> None:
         """
         Adds a step to fill `destination` container/plate/slice with `solvent` up to `quantity`.
 
         Args:
             destination: Container/Plate/Slice to fill.
             solvent: Substance to use to fill.
             quantity: Desired final quantity in container.
@@ -1807,15 +2054,15 @@
         else:
             raise TypeError(f"Invalid destination type: {type(destination)}")
         if not isinstance(solvent, Substance):
             raise TypeError("Solvent must be a substance.")
         if not isinstance(quantity, str):
             raise TypeError("Quantity must be a str.")
 
-        self.steps.append(RecipeStep('fill_to', None, destination, solvent, quantity))
+        self.steps.append(RecipeStep(self, 'fill_to', None, destination, solvent, quantity))
 
     def bake(self) -> dict[str, Container | Plate]:
         """
         Completes steps stored in recipe.
         Checks validity of each step and ensures all declared objects have been used.
         Locks Recipe from further modification.
 
@@ -1826,58 +2073,60 @@
         if self.locked:
             raise RuntimeError("Recipe has already been baked.")
 
         # Implicitly end the current stage
         if self.current_stage != 'all':
             self.end_stage(self.current_stage)
 
-        # for operation, *rest in self.steps:
         for step in self.steps:
             # Keep track of what was used in each step
             for elem in step.frm + step.to:
                 if isinstance(elem, PlateSlicer):
                     step.objects_used.add(elem.plate.name)
                 elif isinstance(elem, (Container, Plate)):
                     step.objects_used.add(elem.name)
 
+            step.frm_slice = step.frm[0] if isinstance(step.frm[0], PlateSlicer) else None
+            step.to_slice = step.to[0] if isinstance(step.to[0], PlateSlicer) else None
+
             operator = step.operator
             if operator == 'create_container':
                 dest = step.to[0]
                 dest_name = dest.name
                 step.frm.append(None)
                 max_volume, initial_contents = step.operands
                 step.to[0] = self.results[dest_name]
                 self.used.add(dest_name)
                 self.results[dest_name] = Container(dest_name, max_volume, initial_contents)
-                step.substances_used = self.results[dest_name].substances()
+                step.substances_used = self.results[dest_name].get_substances()
                 step.to.append(self.results[dest_name])
-                step.instructions = f"Create container {dest_name} with initial contents: {initial_contents}."
+                step.instructions = f"Create container '{dest_name}'."
             elif operator == 'transfer':
                 source = step.frm[0]
                 source_name = source.plate.name if isinstance(source, PlateSlicer) else source.name
                 dest = step.to[0]
                 dest_name = dest.plate.name if isinstance(dest, PlateSlicer) else dest.name
                 quantity, = step.operands
 
-                step.instructions = f"""Transfer {quantity} from {str(source) if isinstance(source, PlateSlicer) else
-                source_name} to {str(dest) if isinstance(dest, PlateSlicer) else dest_name}."""
+                step.instructions = f"""Transfer {quantity} from '{str(source) if isinstance(source, PlateSlicer) else
+                source_name}' to '{str(dest) if isinstance(dest, PlateSlicer) else dest_name}'."""
 
                 self.used.add(source_name)
                 self.used.add(dest_name)
 
                 # containers and such can change while baking the recipe
                 if isinstance(source, PlateSlicer):
                     source = deepcopy(source)
                     source.plate = self.results[source_name]
                     step.frm[0] = source.plate
                 else:
                     source = self.results[source_name]
                     step.frm[0] = source
 
-                step.substances_used = source.substances()
+                step.substances_used = source.get_substances()
 
                 if isinstance(dest, PlateSlicer):
                     dest = deepcopy(dest)
                     dest.plate = self.results[dest_name]
                     step.to[0] = dest.plate
                 else:
                     dest = self.results[dest_name]
@@ -1896,47 +2145,47 @@
             elif operator == 'solution':
                 dest = step.to[0]
                 dest_name = dest.name
                 step.frm.append(None)
                 solute, solvent, kwargs = step.operands
                 # kwargs should have two out of concentration, quantity, and total_quantity
                 if 'concentration' in kwargs and 'total_quantity' in kwargs:
-                    step.instructions = f"""Create a solution of {solute.name} in {solvent.name
-                    } with a concentration of {kwargs['concentration']
+                    step.instructions = f"""Create a solution of '{solute.name}' in '{solvent.name
+                    }' with a concentration of {kwargs['concentration']
                     } and a total quantity of {kwargs['total_quantity']}."""
                 elif 'concentration' in kwargs and 'quantity' in kwargs:
-                    step.instructions = f"""Create a solution of {solute.name} in {solvent.name
-                    } with a concentration of {kwargs['concentration']
+                    step.instructions = f"""Create a solution of '{solute.name}' in '{solvent.name
+                    }' with a concentration of {kwargs['concentration']
                     } and a quantity of {kwargs['quantity']}."""
                 elif 'quantity' in kwargs and 'total_quantity' in kwargs:
-                    step.instructions = f"""Create a solution of {solute.name} in {solvent.name
-                    } with a total quantity of {kwargs['total_quantity']
+                    step.instructions = f"""Create a solution of '{solute.name}' in '{solvent.name
+                    }' with a total quantity of {kwargs['total_quantity']
                     } and a quantity of {kwargs['quantity']}."""
 
                 step.to[0] = self.results[dest_name]
                 self.used.add(dest_name)
                 self.results[dest_name] = Container.create_solution(solute, solvent, dest_name, **kwargs)
-                step.substances_used = self.results[dest_name].substances()
+                step.substances_used = self.results[dest_name].get_substances()
                 step.to.append(self.results[dest_name])
             elif operator == 'solution_from':
                 source = step.frm[0]
                 source_name = source.name
                 dest = step.to[0]
                 dest_name = dest.name
                 solute, concentration, solvent, quantity = step.operands
                 step.frm[0] = self.results[source_name]
                 step.to[0] = self.results[dest_name]
-                step.instructions = f"""Create {quantity} of a {concentration} solution of {solute.name
-                } in {solvent.name} from {source_name}."""
+                step.instructions = f"""Create {quantity} of a {concentration} solution of '{solute.name
+                }' in '{solvent.name}' from '{source_name}'."""
                 self.used.add(source_name)
                 self.used.add(dest_name)
                 source = self.results[source_name]
                 self.results[source_name], self.results[dest_name] = \
                     Container.create_solution_from(source, solute, concentration, solvent, quantity, dest.name)
-                step.substances_used = self.results[dest_name].substances()
+                step.substances_used = self.results[dest_name].get_substances()
                 step.frm.append(self.results[source_name])
                 step.to.append(self.results[dest_name])
             elif operator == 'remove':
                 dest = step.to[0]
                 step.frm.append(None)
                 what, = step.operands
                 dest_name = dest.plate.name if isinstance(dest, PlateSlicer) else dest.name
@@ -1946,51 +2195,125 @@
                 if isinstance(dest, PlateSlicer):
                     dest = deepcopy(dest)
                     dest.plate = self.results[dest_name]
                 else:
                     dest = self.results[dest_name]
 
                 if isinstance(what, Substance):
-                    step.instructions = f"Remove {what.name} from {dest_name}."
+                    step.instructions = f"Remove {what.name} from '{dest_name}'."
                 else:
-                    step.instructions = f"Remove all {Substance.classes[what]} from {dest_name}."
+                    step.instructions = f"Remove all {Substance.classes[what]} from '{dest_name}'."
                 self.results[dest_name] = dest.remove(what)
                 step.to.append(self.results[dest_name])
                 # substances_used is everything that is in step.to[0] but not in step.to[1]
-                step.substances_used = set.difference(step.to[0].substances(), step.to[1].substances())
-                step.trash = {substance: step.to[0].contents[substance] for substance in step.substances_used}
+                step.substances_used = set.difference(step.to[0].get_substances(), step.to[1].get_substances())
+                if isinstance(dest, Container):
+                    step.trash = {substance: step.to[0].contents[substance] for substance in step.substances_used}
+                else:  # Plate
+                    for well in step.to[0].wells.flatten():
+                        for substance in step.substances_used:
+                            step.trash[substance] = step.trash.get(substance, 0.) + well.contents.get(substance, 0.)
             elif operator == 'dilute':
                 dest = step.to[0]
                 dest_name = dest.name
                 solute, concentration, solvent, new_name = step.operands
                 step.frm.append(None)
                 step.to[0] = self.results[dest_name]
                 self.used.add(dest_name)
                 self.results[dest_name] = self.results[dest_name].dilute(solute, concentration, solvent, new_name)
                 amount_added = self.results[dest_name].contents[solvent] - step.to[0].contents.get(solvent, 0)
                 amount_added = Unit.convert_from(solvent, amount_added, config.moles_storage_unit, 'L')
                 amount_added, unit = Unit.get_human_readable_unit(amount_added, 'L')
                 precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
-                step.instructions = (f"Dilute {solute.name} in {dest_name} to {concentration}" +
-                                     f" by adding {round(amount_added, precision)} {unit} of {solvent.name}.")
+                step.instructions = (f"Dilute '{solute.name}' in '{dest_name}' to {concentration}" +
+                                     f" by adding {round(amount_added, precision)} {unit} of '{solvent.name}'.")
                 step.substances_used.add(solvent)
                 step.to.append(self.results[dest_name])
             elif operator == 'fill_to':
                 dest = step.to[0]
                 dest_name = dest.plate.name if isinstance(dest, PlateSlicer) else dest.name
                 solvent, quantity = step.operands
                 step.frm.append(None)
                 step.to[0] = self.results[dest_name]
                 self.used.add(dest_name)
-                amount_added = self.results[dest_name].contents[solvent] - step.to[0].contents.get(solvent, 0)
-                amount_added = Unit.convert_from(solvent, amount_added, config.moles_storage_unit, 'L')
-                amount_added, unit = Unit.get_human_readable_unit(amount_added, 'L')
-                precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
-                step.instructions = (f"Fill {dest.name} with {solvent.name} up to {quantity}"
-                                     f" by adding {round(amount_added, precision)} {unit}.")
+                self.results[dest_name] = step.to[0].fill_to(solvent, quantity)
+                step.to.append(self.results[dest_name])
+                if isinstance(dest, Container):
+                    amount_added = self.results[dest_name].contents[solvent] - step.to[0].contents.get(solvent, 0)
+                    amount_added = Unit.convert_from(solvent, amount_added, config.moles_storage_unit, 'L')
+                    amount_added, unit = Unit.get_human_readable_unit(amount_added, 'L')
+                    precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+                    step.instructions = (f"Fill '{dest.name}' with '{solvent.name}' up to {quantity}"
+                                         f" by adding {round(amount_added, precision)} {unit}.")
+                else:  # PlateSlicer
+                    def collapse(wells, plate):
+                        result = []
+                        row_run = col_run = None
+                        start_well = end_well = wells[0]
+                        for well in wells[1:]:
+                            if row_run is not None:
+                                if well[0] == row_run and well[1] == end_well[1] + 1:
+                                    end_well = well
+                                else:
+                                    row_run = None
+                                    result.append(
+                                        f"{plate.row_names[start_well[0]]}{plate.column_names[start_well[1]]}:"
+                                        f"{plate.row_names[end_well[0]]}{plate.column_names[end_well[1]]}")
+                                    start_well = end_well = well
+                            elif col_run is not None:
+                                if well[1] == col_run and well[0] == end_well[0] + 1:
+                                    end_well = well
+                                else:
+                                    col_run = None
+                                    result.append(
+                                        f"{plate.row_names[start_well[0]]}{plate.column_names[start_well[1]]}:"
+                                        f"{plate.row_names[end_well[0]]}{plate.column_names[end_well[1]]}")
+                                    start_well = end_well = well
+                            elif well[0] == end_well[0] and well[1] == end_well[1] + 1:
+                                end_well = well
+                                row_run = well[0]
+                            elif well[1] == end_well[1] and well[0] == end_well[0] + 1:
+                                end_well = well
+                                col_run = well[1]
+                            else:
+                                result.append(f"{plate.row_names[start_well[0]]}{plate.column_names[start_well[1]]}")
+                                start_well = end_well = well
+                        if row_run is not None or col_run is not None:
+                            result.append(f"{plate.row_names[start_well[0]]}{plate.column_names[start_well[1]]}:"
+                                          f"{plate.row_names[end_well[0]]}{plate.column_names[end_well[1]]}")
+                        if start_well == end_well:
+                            result.append(f"{plate.row_names[start_well[0]]}{plate.column_names[start_well[1]]}")
+                        return result
+
+                    amounts = dict()
+                    plate = step.to[0]
+                    for row in range(plate.n_rows):
+                        for col in range(plate.n_columns):
+                            amount_added = self.results[dest_name].wells[row, col].contents[solvent] - \
+                                           plate.wells[row, col].contents.get(solvent, 0)
+                            amount_added = Unit.convert_from(solvent, amount_added, config.moles_storage_unit, 'uL')
+                            amounts[(row, col)] = round(amount_added, config.internal_precision)
+                    max_amount = max(amounts.values())
+                    _, unit = Unit.get_human_readable_unit(max_amount / 1e6, 'L')
+                    multiplier = 1e-6 / Unit.convert_prefix_to_multiplier(unit[:-1])
+                    precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
+                    amounts_transpose = dict()
+                    for address, amount in amounts.items():
+                        amount = round(amount * multiplier, precision)
+                        if amount == 0.:
+                            continue
+                        if amount not in amounts_transpose:
+                            amounts_transpose[amount] = []
+                        amounts_transpose[amount].append(address)
+                    step.instructions = f"Fill '{dest.name}' with '{solvent.name}' up to {quantity} by adding: "
+                    amount_strings = []
+                    for amount, addresses in amounts_transpose.items():
+                        addresses = collapse(addresses, plate)
+                        amount_strings.append(f"{amount} {unit} to [{', '.join(addresses)}]")
+                    step.instructions += ', '.join(amount_strings) + "."
 
                 if isinstance(dest, PlateSlicer):
                     dest = deepcopy(dest)
                     dest.plate = self.results[dest_name]
                 else:
                     dest = self.results[dest_name]
 
@@ -2001,16 +2324,16 @@
         if len(self.used) != len(self.results):
             raise ValueError("Something declared as used wasn't used.")
         self.locked = True
         # All the PlateSlicers should have been resolved into Plates by now
         assert all(isinstance(elem, (Container, Plate)) for elem in self.results.values())
         return self.results
 
-    def substance_used(self, substance: Substance, timeframe: str = 'all', unit: str = None,
-                       destinations: Iterable[Container | Plate] | str = "plates"):
+    def get_substance_used(self, substance: Substance, timeframe: str = 'all', unit: str = None,
+                           destinations: Iterable[Container | Plate] | str = "plates"):
         """
         Returns the amount of substance used in the recipe.
 
         Args:
             substance: Substance to check.
             timeframe: 'before' or 'during'. Before refers to the initial state of the containers aka recipe "prep", and
             during refers to
@@ -2035,15 +2358,15 @@
                 dest_names.add(container.name)
         else:
             raise ValueError("Invalid destinations.")
 
         delta = 0
 
         if timeframe not in self.stages.keys():
-            raise ValueError("Invalid Timeframe")
+            raise ValueError("Invalid timeframe")
 
         stage_steps = self.steps[self.stages[timeframe]]
         for step in stage_steps:
             if substance not in step.substances_used:
                 continue
 
             before_substances = 0
@@ -2081,48 +2404,114 @@
             container: Container to check.
             timeframe: 'all' or a stage defined in the recipe.
             unit: Unit to return amount in.
         """
 
         def helper(entry):
             substance, quantity = entry
-            return Unit.convert_from(substance, quantity, 'U' if substance.is_enzyme() else config.moles_storage_unit, unit)
+            return Unit.convert_from(substance, quantity, 'U' if substance.is_enzyme() else config.moles_storage_unit,
+                                     unit)
+
+        def plate_helper(container):
+            entry = container.contents.items()
+            return sum(map(helper, entry))
 
         if unit is None:
             unit = config.volume_display_unit
         if not isinstance(unit, str):
             raise TypeError("Unit must be a str.")
-        if not isinstance(container, Container):
-            raise TypeError("Container must be a Container.")
+        if not isinstance(container, Container) and not isinstance(container, Plate):
+            raise TypeError("Container must be a Container or a Plate.")
         if not isinstance(timeframe, str):
             raise TypeError("Timeframe must be a str.")
         if timeframe not in self.stages.keys():
             raise ValueError("Invalid Timeframe")
         steps = self.steps[self.stages[timeframe]]
         flows = {"in": 0, "out": 0}
+        if isinstance(container, Plate):
+            flows = {"in": np.zeros(container.wells.shape), "out": np.zeros(container.wells.shape)}
         for step in steps:
             if container.name in step.objects_used:
                 if isinstance(step.to[0], Container) and step.to[0].name == container.name:
                     if step.trash:
                         flows["out"] += sum(map(helper, step.trash.items()))
                     else:
                         flows["in"] += (sum(map(helper, step.to[1].contents.items())) -
                                         sum(map(helper, step.to[0].contents.items())))
+                if isinstance(step.to[0], Plate) and step.to[0].name == container.name:
+                    if step.trash:
+                        flows["out"] += sum(map(helper, step.trash.items()))
+                    else:
+                        vfunc = np.vectorize(plate_helper)
+                        flows["in"] += vfunc(step.to[1].wells) - vfunc(step.to[0].wells)
                 if isinstance(step.frm[0], Container) and step.frm[0].name == container.name:
                     flows["out"] += (sum(map(helper, step.frm[0].contents.items())) -
                                      sum(map(helper, step.frm[1].contents.items())))
+                if isinstance(step.frm[0], Plate) and step.frm[0].name == container.name:
+                    vfunc = np.vectorize(plate_helper)
+                    flows["out"] += vfunc(step.frm[0].wells) - vfunc(step.frm[1].wells)
         precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
         for key in flows:
             flows[key] = round(flows[key], precision)
 
         return flows
 
-    def visualize(self, what: Plate, mode: str, unit: str, timeframe: (int | str) = 'all',
+    def get_amount_remaining(self, container: Container | Plate, timeframe: str = 'all',
+                             unit: str | None = None, mode: str = 'after') -> float:
+
+        def conversion_helper(entry):
+            substance, quantity = entry
+            return Unit.convert_from(substance, quantity, 'U' if substance.is_enzyme() else config.moles_storage_unit,
+                                     unit)
+
+        def plate_helper(well):
+            entry = well.contents.items()
+            return sum(map(conversion_helper, entry))
+
+        def container_helper(container):
+            if isinstance(container, Container):
+                entry = container.contents.items()
+                return sum(map(conversion_helper, entry))
+            elif isinstance(container, Plate):
+                vfunc = np.vectorize(plate_helper)
+                return vfunc(container.wells)
+
+        if unit is None:
+            unit = config.volume_display_unit
+        if not isinstance(unit, str):
+            raise TypeError("Unit must be a str.")
+        if not isinstance(container, Container) and not isinstance(container, Plate):
+            raise TypeError("Container must be a Container or a Plate.")
+        if not isinstance(timeframe, str):
+            raise TypeError("Timeframe must be a str.")
+        if timeframe not in self.stages.keys():
+            raise ValueError("Invalid Timeframe")
+
+        steps = self.steps[self.stages[timeframe]]
+        if mode == 'after':
+            steps = reversed(steps)
+
+        query_container = None
+        for step in steps:
+            if container.name in step.objects_used:
+                if step.to[0].name == container.name:
+                    if mode == 'after':
+                        query_container = step.to[1]
+                    else:
+                        query_container = step.to[0]
+                else:
+                    if mode == 'after':
+                        query_container = step.frm[1]
+                    else:
+                        query_container = step.frm[0]
+                return container_helper(query_container)
+
+    def visualize(self, what: Plate, mode: str, unit: str, timeframe: (int | str | RecipeStep) = 'all',
                   substance: (str | Substance) = 'all', cmap: str = None) \
-            -> pandas.io.formats.style.Styler:
+            -> str | pandas.io.formats.style.Styler:
         """
 
         Provide visualization of what happened during the step.
 
         Args:
             what: Plate we are interested in.
             mode: 'delta', or 'final'
@@ -2133,15 +2522,15 @@
 
         Returns: A dataframe with the requested information.
         """
         if not isinstance(what, Plate):
             raise TypeError("What must be a Plate.")
         if mode not in ['delta', 'final']:
             raise ValueError("Invalid mode.")
-        if not isinstance(timeframe, (int, str)):
+        if not isinstance(timeframe, (int, str, RecipeStep)):
             raise TypeError("When must be an int or str.")
         if isinstance(timeframe, str) and timeframe not in self.stages:
             raise ValueError("Invalid stage.")
         if not isinstance(unit, str):
             raise TypeError("Unit must be a str.")
         if substance != 'all' and not isinstance(substance, Substance):
             raise TypeError("Substance must be a Substance or 'all'")
@@ -2158,15 +2547,18 @@
                     substance_unit = 'U' if subst.is_enzyme() else config.moles_storage_unit
                     amount += Unit.convert_from(subst, quantity, substance_unit, unit)
                 return amount
             else:
                 substance_unit = 'U' if substance.is_enzyme() else config.moles_storage_unit
                 return Unit.convert_from(substance, elem.contents.get(substance, 0), substance_unit, unit)
 
-        if isinstance(timeframe, str):
+        if isinstance(timeframe, RecipeStep):
+            start_index = self.steps.index(timeframe)
+            end_index = start_index + 1
+        elif isinstance(timeframe, str):
             start_index = self.stages[timeframe].start
             end_index = self.stages[timeframe].stop
             if start_index is None:
                 start_index = 0
             if end_index is None:
                 end_index = len(self.steps)
         else:
@@ -2186,15 +2578,15 @@
                 break
         for i in range(end_index - 1, start_index - 1, -1):
             step = self.steps[i]
             if what.name in step.objects_used:
                 end = i
                 break
         if start is None or end is None:
-            raise ValueError("Plate not used in the desired step(s).")
+            return "This plate was not used in the specified timeframe."
 
         if mode == 'delta':
             before_data = None
             if what.name == self.steps[start].frm[0].name:
                 before_data = self.steps[start].frm[0][:].get_dataframe()
             elif what.name == self.steps[start].to[0].name:
                 before_data = self.steps[start].to[0][:].get_dataframe()
@@ -2218,15 +2610,17 @@
         df = df.round(precision)
         vmin, vmax = df.min().min(), df.max().max()
         styler = df.style.format(precision=precision).background_gradient(cmap, vmin=vmin, vmax=vmax)
         return styler
 
 
 class PlateSlicer(Slicer):
-    """ @private """
+    """
+    Represents a slice of a Plate.
+    """
 
     def __init__(self, plate, item):
         self.plate = plate
         super().__init__(plate.wells, plate.row_names, plate.column_names, item)
 
     def _get_slice_string(self, item):
         assert isinstance(item, tuple)
@@ -2275,15 +2669,15 @@
 
     @array.setter
     def array(self, array: numpy.ndarray):
         self.plate.wells = array
 
     def get_dataframe(self):
         return pandas.DataFrame(self.plate.wells, columns=self.plate.column_names,
-                                index=self.plate.row_names).iloc[self.slices]
+                                index=self.plate.row_names)
 
     @staticmethod
     def _transfer(frm: Container | PlateSlicer, to: PlateSlicer, quantity):
         if isinstance(frm, Container):
             to = copy(to)
             to.plate = deepcopy(to.plate)
 
@@ -2360,36 +2754,74 @@
             frm.set(frm_result)
             to.set(to_result)
         else:
             raise ValueError("Source and destination slices must be the same size and shape.")
 
         return frm.plate, to.plate
 
-    def dataframe(self, unit: str, substance: (str | Substance | Iterable[Substance]) = 'all', cmap: str = None):
+
+    def highlight_wells(self, styler: pandas.io.formats.style.Styler) -> pandas.io.formats.style.Styler:
+        highlight_wells = []
+        if isinstance(self.slices, list):
+            for slice_ in self.slices:
+                row = slice_[0].start or 0
+                col = slice_[1].start or 0
+                highlight_wells.append((row, self.plate.column_names[col]))
+        else:
+            row_start = self.slices[0].start or 0
+            row_stop = self.slices[0].stop or len(self.plate.row_names)
+            row_step = self.slices[0].step or 1
+            col_start = self.slices[1].start or 0
+            col_stop = self.slices[1].stop or len(self.plate.column_names)
+            col_step = self.slices[1].step or 1
+
+            for row in range(row_start, row_stop, row_step):
+                for col in range(col_start, col_stop, col_step):
+                    highlight_wells.append((row, self.plate.column_names[col]))
+
+        def highlight_func(elem):
+            return ['background-color: yellow' if (i, elem.name) in highlight_wells else '' for i, _ in enumerate(elem)]
+
+        styler.apply(highlight_func)
+        return styler
+
+    def dataframe(self, unit: str = None, substance: (str | Substance | Iterable[Substance]) = 'all',
+                  cmap: str = None, highlight: bool = False):
         """
 
         Arguments:
             unit: unit to return quantities in.
             substance: Substance or Substances to display quantity of.
             cmap: Colormap to shade dataframe with.
+            highlight: Highlight wells in slice(s).
 
         Returns: Shaded dataframe of quantities in each well.
 
         """
+        if unit is None:
+            unit = config.volume_display_unit
+
         if not isinstance(unit, str):
             raise TypeError("Unit must be a str.")
         if (substance != 'all' and not isinstance(substance, Substance) and
                 not (isinstance(substance, Iterable) and all(isinstance(x, Substance) for x in substance))):
             raise TypeError("Substance must be a Substance or 'all'")
         if cmap is None:
             cmap = config.default_colormap
         if not isinstance(cmap, str):
             raise TypeError("Colormap must be a str.")
 
+        if ('/' in unit or unit[-1] == 'm' or unit[-1] == 'M') and substance == 'all':
+            raise ValueError("Cannot display concentrations with respect to 'all' substances.")
+
         def helper(elem):
+            if '/' in unit or unit[-1] == 'm' or unit[-1] == 'M':
+                """ Returns concentration of substance in elem. """
+                return elem.get_concentration(substance, unit)
+            # else
             """ Returns amount of substance in elem. """
             if substance == 'all':
                 amount = 0
                 for subst, quantity in elem.contents.items():
                     substance_unit = 'U' if subst.is_enzyme() else config.moles_storage_unit
                     amount += Unit.convert_from(subst, quantity, substance_unit, unit)
                 return amount
@@ -2401,16 +2833,23 @@
                 return amount
             else:
                 substance_unit = 'U' if substance.is_enzyme() else config.moles_storage_unit
                 return Unit.convert_from(substance, elem.contents.get(substance, 0), substance_unit, unit)
 
         precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
         df = self.get_dataframe().apply(numpy.vectorize(helper, cache=True, otypes='d'))
-        vmin, vmax = df.min().min(), df.max().max()
-        styler = df.style.format(precision=precision).background_gradient(cmap, vmin=vmin, vmax=vmax)
+        styler = df.style.format(precision=precision)
+        if highlight:
+            styler = self.highlight_wells(styler)
+        else:
+            if unit[-1] == 'L':
+                vmax = Unit.convert_from_storage(self.plate.max_volume_per_well, unit)
+            else:
+                vmax = df.max().max()
+            styler = styler.background_gradient(cmap, vmin=0, vmax=vmax)
         return styler
 
     def get_volumes(self, substance: (Substance | Iterable[Substance]) = None, unit: str = None) -> numpy.ndarray:
         """
 
         Arguments:
             unit:  unit to return volumes in.
@@ -2449,15 +2888,15 @@
                 for subs in substance:
                     substance_unit = 'U' if subs.is_enzyme() else config.moles_storage_unit
                     amount += Unit.convert_from(subs, elem.contents.get(subs, 0), substance_unit, unit)
             return amount
 
         return numpy.vectorize(helper, cache=True, otypes='d')(self.get()).round(precision)
 
-    def substances(self) -> set[Substance]:
+    def get_substances(self) -> set[Substance]:
         """
 
         Returns: A set of substances present in the plate.
 
         """
         substances_arr = numpy.vectorize(lambda elem: set(elem.contents.keys()), cache=True)(self.get())
         return set.union(*substances_arr.flatten())
@@ -2473,17 +2912,17 @@
 
         if isinstance(substance, Substance):
             substance = [substance]
         if unit is None:
             unit = config.moles_display_unit
 
         if not isinstance(substance, Iterable) or not all(isinstance(x, Substance) for x in substance):
-            raise TypeError(f"Substance must be a Substance or an Iterable of Substances.")
+            raise TypeError("Substance must be a Substance or an Iterable of Substances.")
         if not isinstance(unit, str):
-            raise TypeError(f"Unit must be a str.")
+            raise TypeError("Unit must be a str.")
 
         precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
 
         def helper(elem):
             amount = 0
             for subs in substance:
                 if not subs.is_enzyme():
```

### Comparing `pyplate-hte-0.4.1/pyplate/pyplate.yaml` & `pyplate_hte-0.4.2/pyplate/pyplate.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # How many digits of precision to maintain in internal calculations
 internal_precision: 10
 
 # How many digits of precision to return to the user
 precisions:
   default: 3
-  uL: 1
+  uL: 0
   umol: 1
-  mg: 2
+  mg: 1
 
 # How to store volumes and moles internally
 # uL means we will store volumes as microliters
 volume_storage_unit: uL
 # uL means we will return volumes as microliters
 volume_display_unit: uL
 
 # umol means we will store moles as micromoles
 moles_storage_unit: umol
 # umol means we will return moles as micromoles
 moles_display_unit: umol
 
-# density for solids/biologics in g/mL or U/mL. Can be set to float('inf') to give solids and biologics zero volume.
+# Default concentration unit for get_concentration()
+concentration_display_unit: M
+
+# density for solids/enzymes in g/mL or U/mL. Can be set to float('inf') to give solids and enzymes zero volume.
 default_solid_density: 1
 default_enzyme_density: 1
 
 # units for %w/v
 default_weight_volume_units: g/mL
 
 # default colormap to be used in visualizations
```

### Comparing `pyplate-hte-0.4.1/pyplate/slicer.py` & `pyplate_hte-0.4.2/pyplate/slicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Label = Union[str, int]
 """@private"""
 Single = Union[Label, Tuple[Label, Label]]
 """@private"""
 Singles = Union[List[Single], Single]
 """@private"""
 Slice = Union[Singles, slice, Tuple[slice, Label], Tuple[Label, slice],
-Tuple[slice, slice], Tuple[List[Single], slice], Tuple[slice, List[Single]]]
+              Tuple[slice, slice], Tuple[List[Single], slice], Tuple[slice, List[Single]]]
 """@private"""
 
 
 class Slicer:
     """
     This is a helper class designed to facilitate slicing operations on composed numpy ndarrays.
     To use this class for a specific application, it needs to be extended.
```

### Comparing `pyplate-hte-0.4.1/pyplate_hte.egg-info/PKG-INFO` & `pyplate_hte-0.4.2/pyplate_hte.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplate-hte
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Python tool for designing chemistry experiments in plate format
 Author: Eugene Kwan and James Marvin
 Author-email: ekwan16@gmail.com
 License:   				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -205,63 +205,74 @@
 
 # PyPlate
 
 [![PyPI](https://img.shields.io/pypi/v/pyplate-hte)](https://pypi.org/project/pyplate-hte)
 [![Documentation Status](https://readthedocs.org/projects/pyplate-hte/badge/?version=latest)](https://pyplate-hte.readthedocs.io/en/latest/?badge=latest)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyplate-hte)](https://pypi.org/project/pyplate-hte)
 
-An open-source Python tool for high-throughput chemistry.
+An open-source Python-based ontology and tool for designing, implementing, and reproducing high-throughput experiments (HTE).
 
 ### Introduction
 
-PyPlate provides tools for the design and implementation of high-throughput chemistry experiments (in particular, reaction screening).  It allows the user to define a space of experimental parameters to be explored, select points in that space for experimentation, and design liquid/solid handling steps to implement those experiments in 96 well plates.
+PyPlate provides tools for the design and implementation of high-throughput chemistry and biology experiments (e.g., reaction screening, cell assays, chromatography screening).  It allows the user to define a space of experimental parameters to be explored, select points in that space for experimentation, and design liquid/solid handling steps to implement those experiments in 96 well plates.
 
 ### Installation
 
 PyPlate requires Python 3.10 or later.
 
 `pip install pyplate-hte`
 
 To view plate visualizations, you will need an interactive Python shell like Jupyter.
 
-### Philosophy
-
-All experiments are divided into a *design* phase and an *implementation* phase.
-
-**Design Phase**: TBD
-
-**Implementation Phase**: PyPlate mimics the physical process of dispensing solids or liquids into plates.  `Substance`s are placed into `Container`s and dispensed into `Plate`s.  The instructions for creating a set of plates are grouped into `Recipe` objects.
-
-- add something about how to check that the implementation and design are consistent
-- All objects in PyPlate are considered immutable.
+**Note:** A similarly named package `pyplate` also exists on PyPi.  Be sure to install `pyplate-hte` and **not** `pyplate`.
 
 ## Quick Start
 
+Here is a simple example that illustrates some of the core features of `PyPlate`:
+
 ```python
 
 from pyplate import Substance, Container, Plate, Recipe
 
 triethylamine = Substance.liquid(name="triethylamine", mol_weight=101.19, density=0.726)
-DMSO = Substance.liquid(name="DMSO", mol_weight=78.13, density=1.1004)
+water = Substance.liquid(name="water", mol_weight=18.015, density=1.0)
 
-triethylamine_50mM = Container.create_solution(solute=triethylamine, solvent=DMSO, concentration='50 mM',
+triethylamine_50mM = Container.create_solution(solute=triethylamine, solvent=water, concentration='50 mM',
                                                total_quantity='10 mL')
+
 plate = Plate(name='plate', max_volume_per_well='50 uL')
 
 recipe = Recipe().uses(triethylamine_50mM, plate)
 recipe.transfer(source=triethylamine_50mM, destination=plate[2:7, 2:11], quantity='10 uL')
 results = recipe.bake()
 triethylamine_50mM = results[triethylamine_50mM.name]
 plate = results[plate.name]
 
 recipe.visualize(what=plate, mode='final', unit='uL', timeframe=0)
 
 ```
 
 ![img.png](images/simple_visualization.png)
 
-Documentation is available at [ReadTheDocs](https://pyplate-hte.readthedocs.io/en/latest/).
+## Documentation
+
+Online documentation is available at [ReadTheDocs](https://pyplate-hte.readthedocs.io/en/latest/).  To build the documentation locally, please follow these steps:
+
+``make -C docs html``
+
+The resulting HTML files will be in `docs/build/html`.
+
+In order to build the documentation successfully, you must install the packages listed in docs/requirements.txt.  You can do this by running:
+
+``pip install -r docs/requirements.txt``
 
 ## License
 
-Licensed under the Apache License, Version 2.0 (the "License")
-You may obtain a copy of the License at https://www.apache.org/licenses/LICENSE-2.0
+Licensed under the [Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0) (the "License").
+
+## Contributors
+
+**PyPlate** was designed and written by James Marvin, Eugene Kwan, Corin Wagen, Aryamaan Dhomne, and Pravin Mahendran.
+
+## Getting Help
+
+Please open a GitHub issue!  We respond regularly.  Please also feel free to contribute!
```

### Comparing `pyplate-hte-0.4.1/pyplate_hte.egg-info/SOURCES.txt` & `pyplate_hte-0.4.2/pyplate_hte.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 pyplate/slicer.py
 pyplate_hte.egg-info/PKG-INFO
 pyplate_hte.egg-info/SOURCES.txt
 pyplate_hte.egg-info/dependency_links.txt
 pyplate_hte.egg-info/requires.txt
 pyplate_hte.egg-info/top_level.txt
 tests/test_Container.py
-tests/test_Experiment.py
-tests/test_ExperimentalSpace.py
-tests/test_Factor.py
 tests/test_Plate.py
 tests/test_Recipe.py
 tests/test_Slicer.py
 tests/test_Substance.py
 tests/test_convert.py
 tests/test_create_solution.py
 tests/test_dilute.py
-tests/test_recipe_amount_used.py
-tests/test_recipe_volume_used.py
-tests/test_transfers.py
+tests/test_eugene.py
+tests/test_get_substance_used2.py
+tests/test_recipe_amount_remaining.py
+tests/test_recipe_get_container_flows.py
+tests/test_recipe_get_substance_used.py
+tests/test_transfers.py
+tests/test_volume_used_Plate_transfer.py
```

### Comparing `pyplate-hte-0.4.1/pyproject.toml` & `pyplate_hte-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=63.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyplate-hte"
-version = "0.4.1"
+version = "0.4.2"
 description = "A Python tool for designing chemistry experiments in plate format"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Eugene Kwan and James Marvin"},
     {email = "ekwan16@gmail.com"}
 ]
```

### Comparing `pyplate-hte-0.4.1/tests/test_Plate.py` & `pyplate_hte-0.4.2/tests/test_Plate.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4.1/tests/test_Recipe.py` & `pyplate_hte-0.4.2/tests/test_Recipe.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4.1/tests/test_Slicer.py` & `pyplate_hte-0.4.2/tests/test_Slicer.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4.1/tests/test_Substance.py` & `pyplate_hte-0.4.2/tests/test_Substance.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     # Argument types checked
     with pytest.raises(TypeError, match="Name must be a str"):
         Substance.solid(1, 1)
     with pytest.raises(ValueError, match="Name must not be empty"):
         Substance.solid('', 1)
     with pytest.raises(TypeError, match="Molecular weight must be a float"):
         Substance.solid('water', '1')
+
     # Arguments are sane
     with pytest.raises(ValueError, match="Molecular weight must be positive"):
         Substance.solid('water', -1)
     with pytest.raises(ValueError, match="Molecular weight must be positive"):
         Substance.solid('water', 0)
 
 
@@ -79,26 +80,32 @@
     """
 
     Tests creating an enzyme `Substance`.
 
     """
     # Argument types checked
     with pytest.raises(TypeError, match="Name must be a str"):
-        Substance.enzyme(1)
+        Substance.enzyme(1, 0)
     with pytest.raises(ValueError, match="Name must not be empty"):
-        Substance.enzyme('')
+        Substance.enzyme('', '1 U/g')
+    with pytest.raises(TypeError, match="Specific activity must be a str."):
+        Substance.enzyme('lipase', 1)
+    for activity in ['1 U', '1 g', '1 U/mL', '1 mL/U']:
+        with pytest.raises(ValueError, match="Specific activity must be in U/g or g/U."):
+            Substance.enzyme('lipase', activity)
 
 
 def test_enzyme(lipase):
     """
 
     Tests that members of an enzyme `Substance` are correct.
 
     """
     assert lipase.name == 'lipase'
+    assert lipase.specific_activity == 10000  # 10 U/mg = 10,000 U/g
 
 
 def test_is_solid(salt, water, lipase):
     """
 
     Tests that is_solid() returns the correct values.
```

### Comparing `pyplate-hte-0.4.1/tests/test_convert.py` & `pyplate_hte-0.4.2/tests/test_convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,17 @@
     with pytest.raises(TypeError, match='Quantity must be a str'):
         Unit.convert(salt, None, '')
     with pytest.raises(TypeError, match='Unit must be a str'):
         Unit.convert(salt, '10 mL', None)
 
     with pytest.raises(ValueError, match='Only enzymes can be measured in activity units'):
         Unit.convert(water, '1 U', 'mL')
-    with pytest.raises(ValueError, match='Enzymes can only be measured in activity units'):
-        Unit.convert(lipase, '1 g', 'U')
+    # with pytest.raises(ValueError, match='Enzymes can only be measured in activity units'):
+    assert Unit.convert(lipase, '1 g', 'U') == 10. * 1000.  # 1 g * 1000 mg/g * 10 U/mg
+
 
     # Only enzymes have activity units
     assert Unit.convert(water, '1 mL', 'U') == 0
     assert Unit.convert(lipase, '1 U', 'U') == 1
 
     # prefixes applied correctly
     assert Unit.convert(water, '1 mL', 'L') == 0.001
```

### Comparing `pyplate-hte-0.4.1/tests/test_dilute.py` & `pyplate_hte-0.4.2/tests/test_dilute.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4.1/tests/test_recipe_amount_used.py` & `pyplate_hte-0.4.2/tests/test_recipe_get_substance_used.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-
 import numpy as np
 import pdb
 from pyplate.pyplate import Recipe, Container, Plate
 import pytest
-import logging 
+import logging
 
-# Set up logging
 
+# Set up logging
 
 
 def test_substance_used(water, salt):
     container = Container('container')
     salt_water = Container.create_solution(salt, water, concentration='1 M', total_quantity='100 mL')
     recipe = Recipe()
     recipe.uses(salt_water, container)
     recipe.transfer(salt_water, container, '10 mL')
     recipe.bake()
-    assert recipe.substance_used(substance=salt, timeframe='all', unit='mmol', destinations=[container]) == 10.0
+    assert recipe.get_substance_used(substance=salt, timeframe='all', unit='mmol', destinations=[container]) == 10.0
 
 
 def test_recipe_tracking_before(water):
     """
     Verify initial and mid-recipe substance volumes in a Recipe context.
 
     This test ensures accurate tracking of a substance's volume both before and during recipe execution, 
@@ -56,16 +55,15 @@
 
     recipe.bake()
     # Assertions
     step = recipe.steps[-1]
 
     print(step.frm)
     print(step.to)
-    assert recipe.substance_used(substance=water, unit='mL', destinations=[container]) == 5.0
-    
+    assert recipe.get_substance_used(substance=water, unit='mL', destinations=[container]) == 5.0
 
 
 def test_container_to_plate(triethylamine, empty_plate):
     # TODO: double check volumes here
     """
     Tests the transfer of a substance from a container to a plate within a Recipe context.
 
@@ -94,28 +92,28 @@
     # create_recipe
     recipe = Recipe()
 
     # define initial and transfer volumes
     initial_volume = '10 mL'
     transfer_volume = '100 uL'
 
-    #define destinations
-    
+    # define destinations
+
     # define initial contents and create container
     initial_contents = [(triethylamine, initial_volume)]
-    container = recipe.create_container('container', max_volume='20 mL', 
+    container = recipe.create_container('container', max_volume='20 mL',
                                         initial_contents=initial_contents)
 
     # Test if container.volume is correct intially
     assert container.volume == 0
 
     # Make sure that the recipe uses empty_plate
     recipe.uses(empty_plate)
 
-    #start first stage
+    # start first stage
     recipe.start_stage('transfer_stage')
     recipe.transfer(container, empty_plate, transfer_volume)
     recipe.end_stage('transfer_stage')
 
     # Bake the recipe
     results = recipe.bake()
 
@@ -131,30 +129,30 @@
     step = recipe.steps[-1]
 
     print(step.frm)
     print(step.to)
 
     print("Assertions start here")
 
-    #Since 9600 muL is in the plate, the volume of the container should be 400 muL
+    # Since 9600 muL is in the plate, the volume of the container should be 400 muL
     assert pytest.approx(container.volume) == 400
-    
-    
-    #assert (np.full((8, 12), expected_volume_container) == plate.volumes(unit='uL')).all()
-    #100 muL is transferred to 96 wells in the plate, hence total expected value is 9600
-    assert pytest.approx(recipe.substance_used(substance=triethylamine, timeframe='transfer_stage', unit='uL', destinations=[empty_plate])) == 9600.0
+
+    # assert (np.full((8, 12), expected_volume_container) == plate.volumes(unit='uL')).all()
+    # 100 muL is transferred to 96 wells in the plate, hence total expected value is 9600
+    assert pytest.approx(recipe.get_substance_used(substance=triethylamine, timeframe='transfer_stage', unit='uL',
+                                               destinations=[empty_plate])) == 9600.0
     # assert pytest.approx(
-    #     recipe.substance_used(substance=triethylamine, timeframe='dispensing', unit='uL')) == expected_volume_plate
+    #     recipe.get_substance_used(substance=triethylamine, timeframe='dispensing', unit='uL')) == expected_volume_plate
 
 
 def test_substance_used_dilute(salt, water):
     """
     Tests that the substance amount tracking is correctly tracked during dilution in a recipe.
 
-    This test checks the `substance_used` method  to correctly report the amount of salt used after diluting a saltwater solution. The procedure involves:
+    This test checks the `get_substance_used` method  to correctly report the amount of salt used after diluting a saltwater solution. The procedure involves:
     - Declaring a container with saltwater as part of a recipe.
     - Adding a specific amount of salt to increase the solution's concentration.
     - Diluting the solution to a target molarity of '0.5 M' using water.
     - Baking the recipe to complete the process.
 
     It asserts that:
     - The total amount of salt reported as used matches the expected '50 mmol', despite the dilution.
@@ -172,79 +170,83 @@
     # Create recipe
     recipe = Recipe()
 
     # container = recipe.create_container('container', '20 mL', [(salt_water, '10 mL')])
 
     # Define what the recipe uses
     recipe.uses(container)
-    salt_solution = recipe.create_solution(salt, water, concentration='0.5 M', 
+    salt_solution = recipe.create_solution(salt, water, concentration='0.5 M',
                                            total_quantity='20 mL')
     # container._add(salt_water, '10 mL')
 
     # Transfer 10 mL of salt solution to container
     recipe.start_stage('dilution_stage')
     recipe.transfer(salt_solution, container, '10 mL')
 
     # Add solute to recipe
     # container = container._add(salt, '50 mmol') #Does not do anything as the container that is used in the recipe is the one that was stored initially
     recipe.dilute(container, solute=salt, concentration='0.25 M', solvent=water)
 
-    
     recipe.end_stage('dilution_stage')
 
-
     recipe.bake()
 
     assert container.volume == 0
     # Results would contain the pointers to the new containers, so assert from there
 
     expected_salt_amount = 5.0
-    assert recipe.substance_used(substance=salt, destinations=[container],timeframe='dilution_stage', unit='mmol') == expected_salt_amount
+    assert recipe.get_substance_used(substance=salt, destinations=[container], timeframe='dilution_stage',
+                                 unit='mmol') == expected_salt_amount
 
 
 # Testing create_solution
-def test_substance_used_create_solution(salt, water, empty_plate):
+def test_substance_used_create_solution(salt, water):
     """
     Tests that the substance amount tracking is accurately implemented during the creation of a solution within a recipe.
 
-    This test verifies the `substance_used` method to correctly report the amount of salt utilized in preparing a specific solution. The testing procedure includes:
+    This test verifies the `get_substance_used` method to correctly report the amount of salt utilized in preparing a specific solution. The testing procedure includes:
     - Initiating a recipe and declaring the usage of salt and water as solute and solvent, respectively.
     - Creating a solution with a predefined concentration of '0.5 M' and a total quantity of '20 mL', effectively dissolving the salt within the water.
     - Executing the `bake` method to finalize the creation of the solution.
 
     The assertions made are:
     - The initial volume of the container is checked before the solution creation, ensuring it starts from a baseline of zero.
-    - The amount of salt reported as used during the recipe matches the expected calculation, which is '10 mmol' for achieving the desired solution concentration and volume. This confirms the `substance_used` method's accuracy in reflecting substance usage throughout the recipe's actions.
+    - The amount of salt reported as used during the recipe matches the expected calculation, which is '10 mmol' for achieving the desired solution concentration and volume. This confirms the `get_substance_used` method's accuracy in reflecting substance usage throughout the recipe's actions.
 
     Parameters:
     - salt (Substance): The salt intended to be dissolved to create the solution.
     - water (Substance): The water used as a solvent for the solution.
 
     """
 
+    plate = Plate(name='plate', max_volume_per_well='20 mL')
     # Create recipe
     recipe = Recipe()
-    recipe.uses(salt, water)
-
-
+    # Recipe.uses only takes Containers and Plates
+    # recipe.uses(salt, water)
+    recipe.uses(plate)
 
     # Create solution and add to container
     recipe.start_stage('stage1')
-    container = recipe.create_solution(salt, water, concentration='0.1 M', total_quantity='20 mL')
+    container = recipe.create_solution(salt, water, concentration='0.1 M', total_quantity='1 L')
     ##What is the initial volume of container here?
     assert container.volume == 0
-    recipe.transfer(container, empty_plate, '10 mL')
+    recipe.transfer(container, plate, '10 mL')
     recipe.end_stage('stage1')
 
     # Bake recipe
     recipe.bake()
 
     # Assertions
-    expected_salt_amount = 10.0
-    assert recipe.substance_used(substance=salt, unit='mmol', destinations=[container], timeframe='stage1') == expected_salt_amount
+    # Container starts with 100 mmol of salt. 1 mmol is dispensed to each of 96 wells in the plate.
+    # A net of 4 mmol is "used" into the container
+    expected_salt_amount = 4.0
+    assert recipe.get_substance_used(substance=salt, unit='mmol', destinations=[container],
+                                 timeframe='stage1') == expected_salt_amount
+
 
 # Try substance with solid and liquid
 def test_substance_used_create_solution_from(salt, water, triethylamine):
     """
     Tests accurate tracking of salt usage when creating a new solution from an existing diluted solution.
 
     This test simulates the scenario of diluting an existing salt solution with a different solvent (triethylamine) to create a new solution with the same concentration. The test procedure involves:
@@ -258,67 +260,72 @@
     - The volume of the newly created container is expected to be '20 mL', reflecting the specified quantity for the new solution.
 
     Parameters:
     - salt (Substance): The solute used in the solutions.
     - water (Substance): The solvent for the initial solution.
     - triethylamine (Substance): The solvent for the new solution created from the existing one.
     """
-   # Creating solution from a diluted solution
+    # Creating solution from a diluted solution
     recipe = Recipe()
-    
+
     # Create initial solution and add to container
     recipe.start_stage('stage1')
     initial_container_name = "initial_salt_solution"
-    container = recipe.create_solution(salt, water, concentration='1 M', total_quantity='20 mL', name=initial_container_name)
-    
+    container = recipe.create_solution(salt, water, concentration='1 M', total_quantity='20 mL',
+                                       name=initial_container_name)
+
     recipe.end_stage('stage1')
 
     recipe.start_stage('stage2')
     # Create solution from the initial one with a new solvent
     new_container_name = "new_solution_from_initial"
-    #pdb.set_trace()
-    new_container = recipe.create_solution_from(source=container, solute=salt, concentration='0.5 M', 
-                                                          solvent=water, quantity='10 mL', name=new_container_name)
-    
+    # pdb.set_trace()
+
+
+    new_container = recipe.create_solution_from(source=container, solute=salt, concentration='0.5 M',
+                                                solvent=water, quantity='10 mL', name=new_container_name)
+
+    #Add a Create Solution function too
     # Bake recipe to finalize
 
     recipe.end_stage('stage2')
     results = recipe.bake()
 
     new_container = results[new_container.name]
     # Assertions for substance amount used and container volumes
     expected_salt_amount_stage1 = 20.0
     expected_salt_amount_stage2 = 0.0
-    #If destination for stage2 was new_container, then expected_salt_amount_stage2 would be 10.0
+    # If destination for stage2 was new_container, then expected_salt_amount_stage2 would be 10.0
 
-    assert recipe.substance_used(substance=salt, timeframe='stage1', unit='mmol', destinations=[container,new_container]) == expected_salt_amount_stage1, "The reported amount of salt used does not match the expected value."
-    assert recipe.substance_used(substance=salt, timeframe='stage2', unit='mmol',destinations=[container,new_container]) == expected_salt_amount_stage2, "The reported amount of salt used does not match the expected value."
-    #assert residual == 0, "Expected residual volume to be 0 after creating new solution."
-    
-
-    #Default unit is not Ml, so it shall be failing. Use Unit to change the units
-    #Changed it to check for millimoles
-    assert new_container.volume == 10000 , "Expected new container volume to match the specified total quantity for the new solution."
+    assert recipe.get_substance_used(substance=salt, timeframe='stage1', unit='mmol', destinations=[container,
+                                                                                                new_container]) == expected_salt_amount_stage1, "The reported amount of salt used does not match the expected value."
+    assert recipe.get_substance_used(substance=salt, timeframe='stage2', unit='mmol', destinations=[container,
+                                                                                                new_container]) == expected_salt_amount_stage2, "The reported amount of salt used does not match the expected value."
+    # assert residual == 0, "Expected residual volume to be 0 after creating new solution."
+
+    # Default unit is not Ml, so it shall be failing. Use Unit to change the units
+    # Changed it to check for millimoles
+    assert new_container.volume == 10000, "Expected new container volume to match the specified total quantity for the new solution."
 
 
 def test_substance_used_remove(salt_water, salt):
     """
     Tests the accuracy of substance amount tracking during the removal of a solution in a recipe.
 
-    This test verifies the `substance_used` method for correctly reporting the amount of salt removed from a container. The procedure includes:
+    This test verifies the `get_substance_used` method for correctly reporting the amount of salt removed from a container. The procedure includes:
     - Creating a recipe and a container with an initial volume of '20 mL' of saltwater, implying a certain concentration of salt.
     - Removing '10 mL' of the saltwater from the container, which would also remove a proportional amount of salt based on the solution's concentration.
     - Baking the recipe to finalize the removal process.
 
     The test asserts:
     - The amount of salt removed during the recipe matches the expected value based on the initial concentration and the volume removed. The expected salt amount should logically reflect the proportion of salt in the removed volume, which, in a homogenous solution, would be half of the initial amount if '20 mL' contained '50 mmol' of salt.
 
     Parameters:
     - salt_water (Container): A fixture representing the saltwater solution to be partially removed.
-    - salt (Substance): The salt substance, expected to be tracked through the `substance_used` method.
+    - salt (Substance): The salt substance, expected to be tracked through the `get_substance_used` method.
     """
 
     # Create recipe
     recipe = Recipe()
 
     # Deine initial contents
     initial_contents = [(salt, '50 mmol')]
@@ -330,20 +337,20 @@
     # Substance is solid, which leads to some errors
     recipe.remove(container, salt)
 
     # Bake recipe
     recipe.bake()
 
     # Assertions
-    expected_salt_amount = 0.0
-    assert recipe.substance_used(substance=salt,destinations=[container],unit='mmol') == expected_salt_amount
+    # All of 50 mmol is removed
+    expected_salt_amount = 50.0
+    assert recipe.get_substance_used(substance=salt, destinations=[container], unit='mmol') == expected_salt_amount
 
 
 def test_stages_subst(water):
-    
     """
     Tests tracking of water usage across recipe stages, focusing on water
     transfers within a specific stage and overall recipe operations.
 
     This test evaluates the functionality of defining, executing, and tracking
     operations within named stages of a recipe using the `Recipe` class. It
     involves transferring water between containers within a named stage ('stage1')
@@ -366,39 +373,37 @@
       water usage should be 17.0 mL.
 
     Parameters:
     - water (Substance): Represents water, used in transfers and solution
       preparation.
     """
 
-
     recipe = Recipe()
 
     recipe.start_stage('stage1')
     other_container = recipe.create_container('other container')
 
     # Add solute and solvent to the create_solution method
     initial_contents = [(water, '20 mL')]
 
     # Implicit definition of container being used
     container = recipe.create_container('container', '20 mL', initial_contents)
 
     # Transfer 5 mL from container to other_container
     recipe.transfer(container, other_container, '5 mL')
     recipe.transfer(container, other_container, '10 mL')
-    
+
     recipe.end_stage('stage1')
     recipe.transfer(container, other_container, '2 mL')
     recipe.bake()
 
-
     destination_container = [other_container]
-    assert recipe.substance_used(water, timeframe='stage1', destinations=[container], unit='mL') == 5.0
-    assert recipe.substance_used(water, timeframe='stage1', destinations=[container, other_container], unit='mL') == 20.0
-    assert recipe.substance_used(water, timeframe='all', unit='mL') == 0.0
+    assert recipe.get_substance_used(water, timeframe='stage1', destinations=[container], unit='mL') == 5.0
+    assert recipe.get_substance_used(water, timeframe='stage1', destinations=[container, other_container], unit='mL') == 20.0
+    assert recipe.get_substance_used(water, timeframe='all', unit='mL') == 0.0
 
 
 def test_stages_2(water):
     """
     Tests water usage across containers and stages within a recipe, ensuring
     accurate tracking of water volume.
 
@@ -429,40 +434,42 @@
     - Asserts the water usage within 'stage1' and across specified containers
       aligns with expected actions taken during this stage.
 
     Parameters:
     - water (Substance): Represents the water used in the recipe's operations.
     """
     recipe = Recipe()
-    container1 = recipe.create_container(name='container1',initial_contents=[(water, "10 mL")])
+    container1 = recipe.create_container(name='container1', initial_contents=[(water, "10 mL")])
     plate1 = Plate('plate1', '100 uL')
     plate2 = Plate('plate2', '100 uL')
     recipe.uses(plate1, plate2)
 
     recipe.transfer(source=container1, destination=plate1, quantity='10 uL')
-
-    #fill the first cell in plate
-    recipe.fill_to(plate1[1,1],solvent=water, quantity='20 uL')
-
-    #start a new stage
+    
     recipe.start_stage('stage1')
+    # fill the first well in plate
+    recipe.fill_to(plate1[1, 1], solvent=water, quantity='20 uL')
+
+    # start a new stage
+    
     recipe.transfer(source=plate1, destination=plate2, quantity='1 uL')
     recipe.remove(plate2, water)
     recipe.end_stage('stage1')
 
-    #bake the recipe
+    # bake the recipe
     recipe.bake()
-    assert recipe.substance_used(water, timeframe='all', unit='mL', dest = [container1,plate1, plate2]) == 30.0
-    assert recipe.substance_used(water, timeframe='all', unit='mL', dest = [plate1, plate2]) == 22.0
-    #assert recipe.substance_used(water, timeframe='stage1', unit='mL', dest = [plate1, plate2]) == -1.0
-    assert recipe.substance_used(water, timeframe='all', unit='mL', dest = [plate1, plate2]) == 0.0
-    assert recipe.substance_used(water, timeframe='all', unit='mL', dest = [plate2]) == 1
+    # dest should be destinations
+    assert recipe.get_substance_used(water, timeframe='all', unit='mL', destinations = [container1, plate1, plate2]) == 10.96
+    assert recipe.get_substance_used(water, timeframe='stage1', unit='mL', destinations = [plate1, plate2]) == 0.96
+    #assert recipe.get_substance_used(water, timeframe='stage1', unit='mL', destinations = [plate1, plate2]) == -
+    assert recipe.get_substance_used(water, timeframe='all', unit='mL', destinations = [plate1, plate2]) == 1.92
+    assert recipe.get_substance_used(water, timeframe='all', unit='mL', destinations = [plate2]) == 0.096
 
 
-def test_stages_dilute(water, salt):
+def test_stages_plates(water, salt):
     """
     Tests the dilution process across different stages within a recipe, focusing on a specific stage's volume and substance usage tracking.
 
     This test assesses the `Recipe` class's ability to handle complex procedures involving the creation of solutions, 
     transfers between containers, and dilution processes, specifically focusing on tracking these actions within 
     defined stages of the recipe. It includes creating a salt solution, transferring it to a plate, diluting the solution,
     transferring it again, and then removing part of the solution—all while tracking the amount of water used during a 
@@ -484,72 +491,75 @@
     used is based on the dilution and transfer processes that occur within this stage.
 
     Parameters:
     - water (Substance): The solvent used for creating solutions and performing dilution, representing water.
     - salt (Substance): The solute used for creating the initial solution, representing salt.
     """
     recipe = Recipe()
-    container1 = recipe.create_solution(salt, water, concentration='1 M', total_quantity='10 mL')
-    water_stock = recipe.create_container(initial_contents=(water, "10 mL"))
+    
+    water_stock = recipe.create_container(name='water_stock', initial_contents=[(water, "10 mL")])
 
     plate1 = Plate('plate1', '100 uL')
     plate2 = Plate('plate2', '100 uL')
     recipe.uses(plate1, plate2)
 
-    recipe.transfer(source=container1, dest=plate1, volume='2 mL')
     recipe.start_stage('stage1')
-    recipe.dilute(plate1, solute=salt, solvent=water, source=water_stock, concentration='0.5 M')
-
-    recipe.transfer(source=plate1, dest=plate2, volume='1 mL')
-    recipe.remove(water, plate2)
-
+    recipe.transfer(source=water_stock, destination=plate1, quantity='2 uL')
     recipe.end_stage('stage1')
+    # You cannot dilute a plate, only a container
+    # recipe.dilute(plate1, solute=salt, solvent=water, concentration='0.5 M')
+    recipe.start_stage('stage2')
+    recipe.transfer(source=plate1, destination=plate2, quantity='1 uL')
+    recipe.remove(plate2, water)
 
-    recipe.bake()
+    recipe.end_stage('stage2')
 
-    #Assertions
-    assert recipe.substance_used(water, timeframe='stage1', unit='mL', ) == 2.0
+    recipe.start_stage
 
+   
 
+    recipe.bake()
 
+    #Assertions
+    assert recipe.get_substance_used(water, timeframe='stage1', unit='uL',destinations=[plate1] ) == 192.0
+    assert recipe.get_substance_used(water, timeframe='stage2', unit='uL',destinations=[plate2] ) == 96.0
 
 def test_substance_used_with_no_usage(salt):
-
     """
     Verifies that the amount of a substance reported as used is zero when the substance is not utilized in the recipe.
 
-    This test case is designed to confirm the functionality of the `substance_used` method in scenarios where a specific substance is declared for a recipe but not actually used in any of the recipe steps. The key actions in this test include:
+    This test case is designed to confirm the functionality of the `get_substance_used` method in scenarios where a specific substance is declared for a recipe but not actually used in any of the recipe steps. The key actions in this test include:
     - Initiating a recipe without adding any steps that involve the use of the specified substance (salt, in this case).
     - Finalizing the recipe preparation process by baking the recipe.
     
     The assertion checks:
-    - That the `substance_used` method correctly reports '0 mmol' for the salt, reflecting that it was not used during the recipe's preparation, thus ensuring accurate tracking of substance usage within the recipe.
+    - That the `get_substance_used` method correctly reports '0 mmol' for the salt, reflecting that it was not used during the recipe's preparation, thus ensuring accurate tracking of substance usage within the recipe.
 
     Parameters:
     - salt (Substance): The substance fixture representing salt, intended to verify the tracking of substance usage.
     """
 
     recipe = Recipe()
     # No usage of salt
     recipe.bake()
     # Expecting 0 usage since salt wasn't used
-    assert recipe.substance_used(substance=salt, timeframe='all', unit='mmol') == 0.0
+    assert recipe.get_substance_used(substance=salt, timeframe='all', unit='mmol') == 0.0
 
 
 def test_substance_used_incorrect_timeframe(salt_water, salt, empty_plate):
     """
     Ensures an error is raised when querying the amount of substance used with an unsupported timeframe.
 
-    This test aims to verify the error handling capabilities of the `substance_used` method within the `Recipe` class, particularly when an invalid or unsupported timeframe is specified. The test follows these steps:
+    This test aims to verify the error handling capabilities of the `get_substance_used` method within the `Recipe` class, particularly when an invalid or unsupported timeframe is specified. The test follows these steps:
     - Initializes a recipe and declares the use of a saltwater solution.
     - Transfers a specified volume of the saltwater solution to a plate, simulating a typical recipe action.
     - Completes the recipe by invoking the `bake` method.
     
     The critical part of this test is the assertion that checks:
-    - A `ValueError` is raised when attempting to call `substance_used` with a timeframe argument that the method does not support (`'later'` in this case). The error message is expected to match "Unsupported timeframe," indicating that the method correctly identifies and rejects invalid timeframe inputs.
+    - A `ValueError` is raised when attempting to call `get_substance_used` with a timeframe argument that the method does not support (`'later'` in this case). The error message is expected to match "Unsupported timeframe," indicating that the method correctly identifies and rejects invalid timeframe inputs.
 
     Parameters:
     - salt_water (Container): A fixture representing the saltwater solution used in the recipe.
     - salt (Substance): The substance fixture representing salt, intended to be tracked within the recipe.
     - plate (Plate): A fixture representing a plate, to which the saltwater solution is transferred as part of the recipe.
     """
     recipe = Recipe()
@@ -558,11 +568,22 @@
     recipe.uses(empty_plate)
     recipe.transfer(salt_water, empty_plate, '10 uL')
     recipe.transfer(salt_water, container, '10 uL')
     recipe.bake()
 
     # Raising errors for unexpected timeframes
     with pytest.raises(ValueError, match="Invalid timeframe"):
-        recipe.substance_used(substance=salt, timeframe='later', unit='mmol')
+        recipe.get_substance_used(substance=salt, timeframe='later', unit='mmol')
 
-    
 
+def test_substance_used_fill_to_plate(salt, water):
+    plate = Plate('plate', max_volume_per_well='2 mL')
+    recipe = Recipe()
+    recipe.uses(plate)
+    salt_water = recipe.create_solution(salt, water, concentration='1 M', total_quantity='100 mL')
+    for x, row in enumerate(plate.row_names):
+        for y, col in enumerate(plate.column_names):
+            recipe.transfer(salt_water, plate[row, col], f"{x * y} uL")
+    recipe.fill_to(plate, solvent=water, quantity='1 mL')
+    recipe.bake()
+
+    assert True
```

### Comparing `pyplate-hte-0.4.1/tests/test_transfers.py` & `pyplate_hte-0.4.2/tests/test_transfers.py`

 * *Files identical despite different names*

