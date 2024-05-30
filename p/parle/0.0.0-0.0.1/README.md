# Comparing `tmp/parle-0.0.0.tar.gz` & `tmp/parle-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parle-0.0.0.tar", last modified: Wed May 29 22:58:56 2024, max compression
+gzip compressed data, was "parle-0.0.1.tar", last modified: Thu May 30 13:40:36 2024, max compression
```

## Comparing `parle-0.0.0.tar` & `parle-0.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jantonio  (2146) studentslegacy   (501)        0 2024-05-29 22:58:56.971277 parle-0.0.0/
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     1075 2024-05-29 10:21:00.000000 parle-0.0.0/LICENSE
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     5360 2024-05-29 22:58:56.967277 parle-0.0.0/PKG-INFO
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     4479 2024-05-29 22:58:49.000000 parle-0.0.0/README.md
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     1293 2024-05-29 22:58:49.000000 parle-0.0.0/pyproject.toml
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)       38 2024-05-29 22:58:56.972277 parle-0.0.0/setup.cfg
-drwxr-xr-x   0 jantonio  (2146) studentslegacy   (501)        0 2024-05-29 22:58:56.872275 parle-0.0.0/src/
-drwxr-xr-x   0 jantonio  (2146) studentslegacy   (501)        0 2024-05-29 22:58:56.961277 parle-0.0.0/src/parle.egg-info/
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     5360 2024-05-29 22:58:56.000000 parle-0.0.0/src/parle.egg-info/PKG-INFO
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)      353 2024-05-29 22:58:56.000000 parle-0.0.0/src/parle.egg-info/SOURCES.txt
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)        1 2024-05-29 22:58:56.000000 parle-0.0.0/src/parle.egg-info/dependency_links.txt
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)       76 2024-05-29 22:58:56.000000 parle-0.0.0/src/parle.egg-info/requires.txt
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)       21 2024-05-29 22:58:56.000000 parle-0.0.0/src/parle.egg-info/top_level.txt
-drwxr-xr-x   0 jantonio  (2146) studentslegacy   (501)        0 2024-05-29 22:58:56.955277 parle-0.0.0/src/piler/
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)        0 2024-05-29 22:50:46.000000 parle-0.0.0/src/piler/__init__.py
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     4920 2024-05-29 22:50:46.000000 parle-0.0.0/src/piler/__main__.py
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)      113 2024-05-29 22:50:46.000000 parle-0.0.0/src/piler/errors.py
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     4102 2024-05-29 22:50:46.000000 parle-0.0.0/src/piler/plr.py
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     3096 2024-05-29 22:50:46.000000 parle-0.0.0/src/piler/random_reconciliation.py
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     6572 2024-05-29 22:50:46.000000 parle-0.0.0/src/piler/simulate.py
--rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     3980 2024-05-29 22:50:46.000000 parle-0.0.0/src/piler/utils.py
+drwxr-xr-x   0 jantonio  (2146) studentslegacy   (501)        0 2024-05-30 13:40:36.962418 parle-0.0.1/
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     1075 2024-05-29 10:21:00.000000 parle-0.0.1/LICENSE
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     4410 2024-05-30 13:40:36.958418 parle-0.0.1/PKG-INFO
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     3396 2024-05-30 13:39:35.000000 parle-0.0.1/README.md
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     1280 2024-05-30 13:14:34.000000 parle-0.0.1/pyproject.toml
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)       38 2024-05-30 13:40:36.963418 parle-0.0.1/setup.cfg
+drwxr-xr-x   0 jantonio  (2146) studentslegacy   (501)        0 2024-05-30 13:40:36.893417 parle-0.0.1/src/
+drwxr-xr-x   0 jantonio  (2146) studentslegacy   (501)        0 2024-05-30 13:40:36.928417 parle-0.0.1/src/parle/
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)        0 2024-05-30 13:14:34.000000 parle-0.0.1/src/parle/__init__.py
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     4837 2024-05-30 13:20:27.000000 parle-0.0.1/src/parle/__main__.py
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)      113 2024-05-30 13:14:34.000000 parle-0.0.1/src/parle/errors.py
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     4102 2024-05-30 13:14:34.000000 parle-0.0.1/src/parle/plr.py
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     3096 2024-05-30 13:14:34.000000 parle-0.0.1/src/parle/random_reconciliation.py
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     6488 2024-05-30 13:22:54.000000 parle-0.0.1/src/parle/simulate.py
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     3980 2024-05-30 13:14:34.000000 parle-0.0.1/src/parle/utils.py
+drwxr-xr-x   0 jantonio  (2146) studentslegacy   (501)        0 2024-05-30 13:40:36.954418 parle-0.0.1/src/parle.egg-info/
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)     4410 2024-05-30 13:40:36.000000 parle-0.0.1/src/parle.egg-info/PKG-INFO
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)      353 2024-05-30 13:40:36.000000 parle-0.0.1/src/parle.egg-info/SOURCES.txt
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)        1 2024-05-30 13:40:36.000000 parle-0.0.1/src/parle.egg-info/dependency_links.txt
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)       76 2024-05-30 13:40:36.000000 parle-0.0.1/src/parle.egg-info/requires.txt
+-rw-r--r--   0 jantonio  (2146) studentslegacy   (501)       21 2024-05-30 13:40:36.000000 parle-0.0.1/src/parle.egg-info/top_level.txt
```

### Comparing `parle-0.0.0/LICENSE` & `parle-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parle-0.0.0/PKG-INFO` & `parle-0.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: parle
-Version: 0.0.0
-Summary: PILER : Path and Internal Label Evaluation and Reconciliation
+Version: 0.0.1
+Summary: PARLE: Path Analysis, Reconciliation, and Label Evaluation
 Author-email: José Antonio Ramírez-Rafael <jose.ramirezra@cinvestav.mx>, Alitzel López Sánchez <alitzel.lopez.sanchez@usherbrooke.ca>, Alejandro Flores-Lamas <alejandrofloreslamas@cinvestav.mx>, Maribel Hernández-Rosales <maribel.hr@cinvestav.mx>, Manuel Lafond <manuel.lafond@usherbrooke.ca>
+Project-URL: Homepage, https://gitlab.com/jarr.tecn/recondist
+Project-URL: Bug Tracker, https://gitlab.com/jarr.tecn/recondist/-/issues
 Keywords: tree reconciliation,gene trees,species trees,evolutionary scenarios
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,98 +16,100 @@
 Requires-Dist: networkx>=3.3
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: tqdm>=4.66.4
 
 # PARLE: Path Analysis, Reconciliation, and Label Evaluation
 
-This tool computes the path-label reconciliation (PLR) dissimilarity measure.
-
----
-
-[TOC]
-
----
-
-# Abstract
-
-In this study, we investigate the problem of comparing gene trees reconciled with the same species tree using a novel semi-metric, called the Path-Label Reconciliation (PLR) dissimilarity measure.
-This approach not only quantifies differences in the topology of reconciled gene trees, but also considers discrepancies in predicted ancestral gene-species maps and speciation/duplication events, offering a refinement of existing metrics such Robinson-Foulds (RF) and their labeled extensions LRF and ELRF. A tunable parameter $\alpha$ also allows users to adjust the balance between its species map and event labeling components. We show that PLR can be computed in linear time and that it is a semi-metric. We also discuss the diameters of reconciled gene tree measures, which are important in practice for normalization, and provide initial bounds on PLR, LRF, and ELRF.
-
-To validate PLR, we simulate reconciliations and perform comparisons with LRF and ELRF. The results show that PLR provides a more evenly distributed range of distances, highlighting its sensitivity and effectiveness, at the same time being computationally efficient. Our findings suggest that the theoretical diameter is rarely reached in practice. The PLR measure advances phylogenetic reconciliation by combining theoretical rigor with practical applicability. Future research will refine its mathematical properties,  explore its performance on different tree types, and integrate it with existing bioinformatics tools for large-scale evolutionary analyses.
-
-**Keywords:** Reconciliation, gene trees, species trees, evolutionary scenarios
-
-**Reference:** Alitzel López Sánchez • José Antonio Ramírez-Rafael • Alejandro Flores Lamas • Maribel Hernandez-Rosales • Manuel Lafond (2024) **The Path-Label Reconciliation (PLR) Dissimilarity1
-Measure for Gene Trees**. (currently under review at the [WABI 2004 conference](https://algo-conference.org/2024/wabi/))
-
----
+This tool computes the path-label reconciliation (PLR) dissimilarity measure. ([see abstract][https://gitlab.com/jarr.tecn/recondist]).
 
 # Installation
 
 ```bash
-pip install piler
+pip install parle
 ```
 
 # Synopsis of the tool
 
 This code is a command-line tool designed to generate and compare reconciled gene trees with a given species tree, accounting for evolutionary events. It uses a proposed semi-metric *PLR* to quantify differences between reconciled gene trees, considering discrepancies in tree topology, gene-species mapping, and speciation/duplication events.
 
 This tool supports benchmarking and validation by simulating reconciliations and comparing results with metrics like *LRF* and *ELRF*. The tool aims to enhance phylogenetic reconciliation by providing a refined and efficient method for comparing reconciled gene trees.
 
 The tool can be used with the following syntax:
 
 ```bash
 # Compute disimilarity
-python -m piler gene_trees species_tree <optional arguments>
+python -m parle gene_trees species_tree <optional arguments>
 
 # Compute distance
-python -m piler.simulate_reconciliations species_tree n_genes n_recons <optional arguments>
+python -m parle.simulate_reconciliations species_tree n_genes n_recons <optional arguments>
 
 
 ```
 
 For detailed usage information, you can access the help documentation of the modules:
 
 ```bash
-python -m piler -h
-python -m piler.simulate -h
+python -m parle -h
+python -m parle.simulate -h
 ```
 
 # Tutorial
 
+We will see how to generate and analyze datasets for 10 species, maximum 2 gene per species, and 20 gene trees/pairs of gene trees. These numbers can be modified.
+
+The species tree can be simulated by PARLE or can be inputed as a .nhx file.
+
 ## To Generate Data
 
 Generate a list of reconciliations with the same species tree and set of genes for all the reconciliations:
 
 ```bash
-# 5 species, maximum 1 gene per species, 10 gene trees
-python -m piler.simulate 5 1 10
+python -m parle.simulate 10 2 20
 ```
 
+Output files: `plr.species_tree.list.nhx`, `plr.random_reconciliations.list.tsv`
+
+---
+
 Generate pairs of reconciliations with the same species tree for all the reconciliations and pair-specific sets of genes:
 
 ```bash
- 5 species, maximum 1 gene per species, 10 gene trees
-python -m piler.simulate 5 1 10 -m pairs
+python -m parle.simulate 10 2 20 -m pairs
+```
+
+Output files: `plr.species_tree.pairs.nhx`, `plr.random_reconciliations.pairs.tsv`.
+
+---
+
+To use an external species tree use the name of the file instead of `5`, an example, if you have a file `species_tree.nhx` with the content `((((((16,17)15,14)7,6)5,((10,11)9,8)4)3,((18,19)13,12)2)1)0;`, then you can use the commands:
+
+```bash
+python -m parle.simulate species_tree.nhx 1 10
+python -m parle.simulate species_tree.nhx 1 10 -m pairs
 ```
 
 ## To Compute Distances
 
 Compute distances of pairs of trees sorted by rows:
 
 ```bash
-python -m piler plr.random_reconciliations.list.tsv plr.species_tree.list.nhx
+python -m parle plr.random_reconciliations.list.tsv plr.species_tree.list.nhx
 ```
 
 Compute distances for all possible pairs of gene trees in a list:
 
 ```bash
-python -m piler plr.random_reconciliations.list.tsv plr.species_tree.list.nhx -m all_vs_all
+python -m parle plr.random_reconciliations.list.tsv plr.species_tree.list.nhx -m all_vs_all
 ```
 
+## Visualization
+
+- For gene tree visualization we recomend [itol](itol.embl.de/).
+- For trees reconciliation we recommend [REvolutionH-tl](pypi.org/project/revolutionhtl/).
+
 # Additional Information
 
 - The tool uses the PLR metric, which is designed to compare reconciled gene trees by taking into account all three components of reconciliations (tree topology, gene-species map, and event labeling) as well as duplication clusters.
 
 - The metric is linear-time computable, making it suitable for large datasets.
 - For more detailed documentation and examples, please refer to the project documentation within the repository.
```

### Comparing `parle-0.0.0/README.md` & `parle-0.0.1/src/parle.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,115 @@
-# PARLE: Path Analysis, Reconciliation, and Label Evaluation
-
-This tool computes the path-label reconciliation (PLR) dissimilarity measure.
-
----
-
-[TOC]
-
----
+Metadata-Version: 2.1
+Name: parle
+Version: 0.0.1
+Summary: PARLE: Path Analysis, Reconciliation, and Label Evaluation
+Author-email: José Antonio Ramírez-Rafael <jose.ramirezra@cinvestav.mx>, Alitzel López Sánchez <alitzel.lopez.sanchez@usherbrooke.ca>, Alejandro Flores-Lamas <alejandrofloreslamas@cinvestav.mx>, Maribel Hernández-Rosales <maribel.hr@cinvestav.mx>, Manuel Lafond <manuel.lafond@usherbrooke.ca>
+Project-URL: Homepage, https://gitlab.com/jarr.tecn/recondist
+Project-URL: Bug Tracker, https://gitlab.com/jarr.tecn/recondist/-/issues
+Keywords: tree reconciliation,gene trees,species trees,evolutionary scenarios
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: revolutionhtl>=1.2.0
+Requires-Dist: networkx>=3.3
+Requires-Dist: pandas>=2.2.2
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: tqdm>=4.66.4
 
-# Abstract
-
-In this study, we investigate the problem of comparing gene trees reconciled with the same species tree using a novel semi-metric, called the Path-Label Reconciliation (PLR) dissimilarity measure.
-This approach not only quantifies differences in the topology of reconciled gene trees, but also considers discrepancies in predicted ancestral gene-species maps and speciation/duplication events, offering a refinement of existing metrics such Robinson-Foulds (RF) and their labeled extensions LRF and ELRF. A tunable parameter $\alpha$ also allows users to adjust the balance between its species map and event labeling components. We show that PLR can be computed in linear time and that it is a semi-metric. We also discuss the diameters of reconciled gene tree measures, which are important in practice for normalization, and provide initial bounds on PLR, LRF, and ELRF.
-
-To validate PLR, we simulate reconciliations and perform comparisons with LRF and ELRF. The results show that PLR provides a more evenly distributed range of distances, highlighting its sensitivity and effectiveness, at the same time being computationally efficient. Our findings suggest that the theoretical diameter is rarely reached in practice. The PLR measure advances phylogenetic reconciliation by combining theoretical rigor with practical applicability. Future research will refine its mathematical properties,  explore its performance on different tree types, and integrate it with existing bioinformatics tools for large-scale evolutionary analyses.
-
-**Keywords:** Reconciliation, gene trees, species trees, evolutionary scenarios
-
-**Reference:** Alitzel López Sánchez • José Antonio Ramírez-Rafael • Alejandro Flores Lamas • Maribel Hernandez-Rosales • Manuel Lafond (2024) **The Path-Label Reconciliation (PLR) Dissimilarity1
-Measure for Gene Trees**. (currently under review at the [WABI 2004 conference](https://algo-conference.org/2024/wabi/))
+# PARLE: Path Analysis, Reconciliation, and Label Evaluation
 
----
+This tool computes the path-label reconciliation (PLR) dissimilarity measure. ([see abstract][https://gitlab.com/jarr.tecn/recondist]).
 
 # Installation
 
 ```bash
-pip install piler
+pip install parle
 ```
 
 # Synopsis of the tool
 
 This code is a command-line tool designed to generate and compare reconciled gene trees with a given species tree, accounting for evolutionary events. It uses a proposed semi-metric *PLR* to quantify differences between reconciled gene trees, considering discrepancies in tree topology, gene-species mapping, and speciation/duplication events.
 
 This tool supports benchmarking and validation by simulating reconciliations and comparing results with metrics like *LRF* and *ELRF*. The tool aims to enhance phylogenetic reconciliation by providing a refined and efficient method for comparing reconciled gene trees.
 
 The tool can be used with the following syntax:
 
 ```bash
 # Compute disimilarity
-python -m piler gene_trees species_tree <optional arguments>
+python -m parle gene_trees species_tree <optional arguments>
 
 # Compute distance
-python -m piler.simulate_reconciliations species_tree n_genes n_recons <optional arguments>
+python -m parle.simulate_reconciliations species_tree n_genes n_recons <optional arguments>
 
 
 ```
 
 For detailed usage information, you can access the help documentation of the modules:
 
 ```bash
-python -m piler -h
-python -m piler.simulate -h
+python -m parle -h
+python -m parle.simulate -h
 ```
 
 # Tutorial
 
+We will see how to generate and analyze datasets for 10 species, maximum 2 gene per species, and 20 gene trees/pairs of gene trees. These numbers can be modified.
+
+The species tree can be simulated by PARLE or can be inputed as a .nhx file.
+
 ## To Generate Data
 
 Generate a list of reconciliations with the same species tree and set of genes for all the reconciliations:
 
 ```bash
-# 5 species, maximum 1 gene per species, 10 gene trees
-python -m piler.simulate 5 1 10
+python -m parle.simulate 10 2 20
 ```
 
+Output files: `plr.species_tree.list.nhx`, `plr.random_reconciliations.list.tsv`
+
+---
+
 Generate pairs of reconciliations with the same species tree for all the reconciliations and pair-specific sets of genes:
 
 ```bash
- 5 species, maximum 1 gene per species, 10 gene trees
-python -m piler.simulate 5 1 10 -m pairs
+python -m parle.simulate 10 2 20 -m pairs
+```
+
+Output files: `plr.species_tree.pairs.nhx`, `plr.random_reconciliations.pairs.tsv`.
+
+---
+
+To use an external species tree use the name of the file instead of `5`, an example, if you have a file `species_tree.nhx` with the content `((((((16,17)15,14)7,6)5,((10,11)9,8)4)3,((18,19)13,12)2)1)0;`, then you can use the commands:
+
+```bash
+python -m parle.simulate species_tree.nhx 1 10
+python -m parle.simulate species_tree.nhx 1 10 -m pairs
 ```
 
 ## To Compute Distances
 
 Compute distances of pairs of trees sorted by rows:
 
 ```bash
-python -m piler plr.random_reconciliations.list.tsv plr.species_tree.list.nhx
+python -m parle plr.random_reconciliations.list.tsv plr.species_tree.list.nhx
 ```
 
 Compute distances for all possible pairs of gene trees in a list:
 
 ```bash
-python -m piler plr.random_reconciliations.list.tsv plr.species_tree.list.nhx -m all_vs_all
+python -m parle plr.random_reconciliations.list.tsv plr.species_tree.list.nhx -m all_vs_all
 ```
 
+## Visualization
+
+- For gene tree visualization we recomend [itol](itol.embl.de/).
+- For trees reconciliation we recommend [REvolutionH-tl](pypi.org/project/revolutionhtl/).
+
 # Additional Information
 
 - The tool uses the PLR metric, which is designed to compare reconciled gene trees by taking into account all three components of reconciliations (tree topology, gene-species map, and event labeling) as well as duplication clusters.
 
 - The metric is linear-time computable, making it suitable for large datasets.
-- For more detailed documentation and examples, please refer to the project documentation within the repository.
+- For more detailed documentation and examples, please refer to the project documentation within the repository.
```

### Comparing `parle-0.0.0/pyproject.toml` & `parle-0.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "parle"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
   { name="José Antonio Ramírez-Rafael", email="jose.ramirezra@cinvestav.mx" },
   { name="Alitzel López Sánchez", email="alitzel.lopez.sanchez@usherbrooke.ca" },
   { name="Alejandro Flores-Lamas", email="alejandrofloreslamas@cinvestav.mx" },
   { name="Maribel Hernández-Rosales", email="maribel.hr@cinvestav.mx" },
   { name="Manuel Lafond", email="manuel.lafond@usherbrooke.ca" },
 ]
-description = "PILER : Path and Internal Label Evaluation and Reconciliation"
+description = "PARLE: Path Analysis, Reconciliation, and Label Evaluation"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -29,10 +29,10 @@
                 "networkx >= 3.3",
                 "pandas >= 2.2.2",
                 "numpy >= 1.26.4",
                 "tqdm >= 4.66.4",
                 ]
 
 [project.urls]
-#"Homepage" = "https://gitlab.com/jarr.tecn/revolutionh-tl"
-#"Bug Tracker" = "https://gitlab.com/jarr.tecn/revolutionh-tl/issues"
+"Homepage" = "https://gitlab.com/jarr.tecn/recondist"
+"Bug Tracker" = "https://gitlab.com/jarr.tecn/recondist/-/issues"
```

### Comparing `parle-0.0.0/src/piler/__main__.py` & `parle-0.0.1/src/parle/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,32 +34,30 @@
 For more examples go to [PYPI WEBSITE]
 
 Output
 ------
 A table containing the PLR disimilarity measure between the input reconciliations.
 """
 
-hello= """
-       .__.__                
-______ |__|  |   ___________ 
-\____ \|  |  | _/ __ \_  __ \
-|  |_> >  |  |_\  ___/|  | \/
-|   __/|__|____/\___  >__|   
-|__|                \/       
-"""
+hello="""
+         .   
+._  _.._.| _ 
+[_)(_][  |(/,
+|            """
 
 if __name__ == "__main__":
     import argparse
+    from importlib.metadata import version
 
-    V_plr= version('piler')
-    txt= f"piler V{V_plr}"
+    V_plr= version('parle')
+    txt= f"parle V{V_plr}"
 
-    parser = argparse.ArgumentParser(prog= 'piler',
+    parser = argparse.ArgumentParser(prog= 'parle',
                                      description=f'{txt}\n{desc_def}',
-                                     usage='python -m piler gene_trees species_tree <optional arguments>',
+                                     usage='python -m parle gene_trees species_tree <optional arguments>',
                                      formatter_class=argparse.RawDescriptionHelpFormatter,
                                     )
 
     parser.add_argument('gene_trees',
                         help= '[str] .tsv file containing gene trees and reconciliation maps.',
                         type= str,
                        )
```

### Comparing `parle-0.0.0/src/piler/plr.py` & `parle-0.0.1/src/parle/plr.py`

 * *Files identical despite different names*

### Comparing `parle-0.0.0/src/piler/random_reconciliation.py` & `parle-0.0.1/src/parle/random_reconciliation.py`

 * *Files identical despite different names*

### Comparing `parle-0.0.0/src/piler/simulate.py` & `parle-0.0.1/src/parle/simulate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 desc_def= """
 """
 
-hello = """
-       .__.__                
-______ |__|  |   ___________ 
-\____ \|  |  | _/ __ \_  __ \
-|  |_> >  |  |_\  ___/|  | \/
-|   __/|__|____/\___  >__|   
-|__|                \/       
-"""
+hello="""
+         .   
+._  _.._.| _ 
+[_)(_][  |(/,
+|            """
 
 if __name__ == "__main__":
     import argparse
+    from importlib.metadata import version
 
-    V_plr= version('piler')
-    txt= f"piler.simulate_reconciliations V{V_plr}"
+    V_plr= version('parle')
+    txt= f"parle.simulate_reconciliations V{V_plr}"
 
-    parser = argparse.ArgumentParser(prog= 'piler.simulate_reconciliations',
+    parser = argparse.ArgumentParser(prog= 'parle.simulate_reconciliations',
                                      description=f'{txt}\n{desc_def}',
-                                     usage='python -m piler.simulate_reconciliations species_tree n_genes n_recons <optional arguments>',
+                                     usage='python -m parle.simulate_reconciliations species_tree n_genes n_recons <optional arguments>',
                                      formatter_class=argparse.RawDescriptionHelpFormatter,
                                     )
 
     parser.add_argument('species_tree',
                         help= '[str or int] .txt file containing a species tree in nhx format or number of species to simulate by "random merges".',
                        )
```

### Comparing `parle-0.0.0/src/piler/utils.py` & `parle-0.0.1/src/parle/utils.py`

 * *Files identical despite different names*

