# Comparing `tmp/treat_sim-2.0.0.tar.gz` & `tmp/treat_sim-2.1.0.tar.gz`

## Comparing `treat_sim-2.0.0.tar` & `treat_sim-2.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 treat_sim-2.0.0/treat_sim/__init__.py
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 treat_sim-2.0.0/treat_sim/distributions.py
--rw-r--r--   0        0        0    38601 2020-02-02 00:00:00.000000 treat_sim-2.0.0/treat_sim/model.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 treat_sim-2.0.0/treat_sim/data/ed_arrivals.csv
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 treat_sim-2.0.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 treat_sim-2.0.0/LICENSE
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 treat_sim-2.0.0/README.md
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 treat_sim-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 treat_sim-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 treat_sim-2.1.0/treat_sim/__init__.py
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 treat_sim-2.1.0/treat_sim/distributions.py
+-rw-r--r--   0        0        0    38601 2020-02-02 00:00:00.000000 treat_sim-2.1.0/treat_sim/model.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 treat_sim-2.1.0/treat_sim/data/ed_arrivals.csv
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 treat_sim-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 treat_sim-2.1.0/LICENSE
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 treat_sim-2.1.0/README.md
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 treat_sim-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 treat_sim-2.1.0/PKG-INFO
```

### Comparing `treat_sim-2.0.0/treat_sim/distributions.py` & `treat_sim-2.1.0/treat_sim/distributions.py`

 * *Files identical despite different names*

### Comparing `treat_sim-2.0.0/treat_sim/model.py` & `treat_sim-2.1.0/treat_sim/model.py`

 * *Files identical despite different names*

### Comparing `treat_sim-2.0.0/.gitignore` & `treat_sim-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `treat_sim-2.0.0/LICENSE` & `treat_sim-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `treat_sim-2.0.0/README.md` & `treat_sim-2.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,22 @@
 
 ## Funding
 
 This code is part of independent research supported by the National Institute for Health Research Applied Research Collaboration South West Peninsula. The views expressed in this publication are those of the author(s) and not necessarily those of the National Institute for Health Research or the Department of Health and Social Care.
 
 ## Instructions to run the model
 
+### Install from PyPI
+
+If you do not wish to you the code or would like to use the model as part of your own work you can install the model as a python package.
+
+```bash
+pip install treat-sim
+```
+
 ### Online Notebooks via Binder
 
 The python code for the model has been setup to run online in Jupyter notebooks via binder [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pythonhealthdatascience/stars-treat-sim/HEAD)
 
 > mybinder.org is a free tier service.  If it has not been used in a while Binder will need to re-containerise the code repository, and push to BinderHub. This will take several minutes. After that the online environment will be quick to load.
 
 ### To download code and run locally
@@ -49,24 +57,28 @@
 git clone https://github.com/pythonhealthdatascience/stars-treat-sim
 ```
 
 #### Installing dependencies
 
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
-All dependencies can be found in [`binder/environment.yml`]() and are pulled from conda-forge.  To run the code locally, we recommend install [mini-conda](https://docs.conda.io/en/latest/miniconda.html); navigating your terminal (or cmd prompt) to the directory containing the repo and issuing the following command:
+All dependencies can be found in [`binder/environment.yml`]() and are pulled from conda-forge.  To run the code locally, we recommend installing [miniforge](https://github.com/conda-forge/miniforge);
+
+> miniforge is FOSS alternative to Anaconda and miniconda that uses conda-forge as the default channel for packages. It installs both conda and mamba (a drop in replacement for conda) package managers.  We recommend mamba for faster resolving of dependencies and installation of packages. 
+
+navigating your terminal (or cmd prompt) to the directory containing the repo and issuing the following command:
 
 ```
-conda env create -f binder/environment.yml
+mamba env create -f binder/environment.yml
 ```
 
-Activate the conda environment using the following command:
+Activate the mamba environment using the following command:
 
 ```
-conda activate stars_treat_sim
+mamba activate stars_treat_sim
 ```
 
 #### Running the model
 
 To run 50 multiple replications across a number of example experiments, use the following code:
 
 ```python
@@ -95,67 +107,84 @@
     # use all default parameter values
     base_case = Scenario()
 
     results = multiple_replications(base_case).describe().round(2).T
     print(results)
 
 ```
+#### Testing the model
+
+> See our [online documentation](https://pythonhealthdatascience.github.io/stars-simpy-example-docs/content/02_model_code/05_testing.html) for an overview of testing
+
+To run tests activate the virtual environment and entre the following command:
+
+```bash
+pytest
+```
+
+Alternatively to recieve a test coverage estimate issue the following command
+
+```bash
+pytest --cov=treat_sim tests/
+```
+
 
 ## Repo overview
 
 ```
 .
 ├── binder
 │   └── environment.yml
 ├── CHANGES.md
 ├── CITATION.cff
 ├── LICENSE
-├── MANIFEST.in
 ├── notebooks
 │   └── test_package.ipynb
+├── pyproject.toml
 ├── README.md
-├── requirements.txt
-├── setup.py
+├── tests
+│   └── test_model.ipynb
 └── treat_sim
     ├── data
     │   └── ed_arrivals.csv
     ├── distributions.py
     ├── __init__.py
     └── model.py
 ```
 
 * `binder/` - contains the environment.yml file (sim) and all dependencies managed via conda, used to set-up the notebooks on Binder.
 * `CHANGES.md` - changelog with record of notable changes to project between versions.
 * `CITATION.cff` - citation information for the package.
 * `LICENSE` - details of the MIT permissive license of this work.
-* `MANIFEST.in` - files to include in the package.
 * `notebooks/` - contains a notebook to run the model and provides basic enhanced model documentation.
+* `pyproject.toml` - used to build and distribute python package inc. managing a list of package dependencies.
 * `README.md` - what you are reading now!
-* `requirements.txt` - list of packages and minimum versions required.
-* `setup.py` - used to build and distribute package.
+* `tests/` - contains automated testing code
 * `treat_sim/` - contains packaged version of the model.
     * `data/` - directory containing data file used by package.
     * `distributions.py` - distribution classes.
     * `__init__.py` - required as part of package - contains author and version.
     * `model.py` - example SimPy model.
 
+
 ## Citation
 
 If you use the materials within this repository we would appreciate a citation.
 
 ```
-Monks, T., Harper, A., & Heather, A. (2024). Towards Sharing Tools, and Artifacts, for Reusable Simulation: a minimal model example (v1.2.0). Zenodo. https://doi.org/10.5281//zenodo.10026326
+Monks, T., Harper, A., & Heather, A. (2024). Towards Sharing Tools, and Artifacts, for Reusable Simulation: a minimal model example (v2.1.0). Zenodo. https://doi.org/10.5281//zenodo.10026326
 ```
 
 ```bibtex
 @software{stars_treat_sim,
   author       = {Thomas Monks, Alison Harper and Amy Heather},
   title        = {{Towards Sharing Tools, and Artifacts, for Reusable 
                    Simulation: a minimal model example}},
   month        = May,
   year         = 2024,
   publisher    = {Zenodo},
-  version      = {v1.2.0},
+  version      = {v2.0.0},
   doi          = {10.5281//zenodo.10026326.},
   url          = {https://doi.org/10.5281//zenodo.10026326}
 }
 ```
+
```

### Comparing `treat_sim-2.0.0/pyproject.toml` & `treat_sim-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `treat_sim-2.0.0/PKG-INFO` & `treat_sim-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: treat-sim
-Version: 2.0.0
+Version: 2.1.0
 Summary: A Python Free and Open Source Software implementation of the Treatment Centre Model from Nelson (2013)
 Project-URL: Homepage, https://github.com/pythonhealthdatascience/stars-treat-sim
 Project-URL: Bug Tracker, https://github.com/pythonhealthdatascience/stars-treat-sim
 Project-URL: Documentation, https://pythonhealthdatascience.github.io/stars-simpy-example-docs/
 Author-email: Thomas Monks <forecast-tools@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -54,14 +54,22 @@
 
 ## Funding
 
 This code is part of independent research supported by the National Institute for Health Research Applied Research Collaboration South West Peninsula. The views expressed in this publication are those of the author(s) and not necessarily those of the National Institute for Health Research or the Department of Health and Social Care.
 
 ## Instructions to run the model
 
+### Install from PyPI
+
+If you do not wish to you the code or would like to use the model as part of your own work you can install the model as a python package.
+
+```bash
+pip install treat-sim
+```
+
 ### Online Notebooks via Binder
 
 The python code for the model has been setup to run online in Jupyter notebooks via binder [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pythonhealthdatascience/stars-treat-sim/HEAD)
 
 > mybinder.org is a free tier service.  If it has not been used in a while Binder will need to re-containerise the code repository, and push to BinderHub. This will take several minutes. After that the online environment will be quick to load.
 
 ### To download code and run locally
@@ -74,24 +82,28 @@
 git clone https://github.com/pythonhealthdatascience/stars-treat-sim
 ```
 
 #### Installing dependencies
 
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
-All dependencies can be found in [`binder/environment.yml`]() and are pulled from conda-forge.  To run the code locally, we recommend install [mini-conda](https://docs.conda.io/en/latest/miniconda.html); navigating your terminal (or cmd prompt) to the directory containing the repo and issuing the following command:
+All dependencies can be found in [`binder/environment.yml`]() and are pulled from conda-forge.  To run the code locally, we recommend installing [miniforge](https://github.com/conda-forge/miniforge);
+
+> miniforge is FOSS alternative to Anaconda and miniconda that uses conda-forge as the default channel for packages. It installs both conda and mamba (a drop in replacement for conda) package managers.  We recommend mamba for faster resolving of dependencies and installation of packages. 
+
+navigating your terminal (or cmd prompt) to the directory containing the repo and issuing the following command:
 
 ```
-conda env create -f binder/environment.yml
+mamba env create -f binder/environment.yml
 ```
 
-Activate the conda environment using the following command:
+Activate the mamba environment using the following command:
 
 ```
-conda activate stars_treat_sim
+mamba activate stars_treat_sim
 ```
 
 #### Running the model
 
 To run 50 multiple replications across a number of example experiments, use the following code:
 
 ```python
@@ -120,67 +132,84 @@
     # use all default parameter values
     base_case = Scenario()
 
     results = multiple_replications(base_case).describe().round(2).T
     print(results)
 
 ```
+#### Testing the model
+
+> See our [online documentation](https://pythonhealthdatascience.github.io/stars-simpy-example-docs/content/02_model_code/05_testing.html) for an overview of testing
+
+To run tests activate the virtual environment and entre the following command:
+
+```bash
+pytest
+```
+
+Alternatively to recieve a test coverage estimate issue the following command
+
+```bash
+pytest --cov=treat_sim tests/
+```
+
 
 ## Repo overview
 
 ```
 .
 ├── binder
 │   └── environment.yml
 ├── CHANGES.md
 ├── CITATION.cff
 ├── LICENSE
-├── MANIFEST.in
 ├── notebooks
 │   └── test_package.ipynb
+├── pyproject.toml
 ├── README.md
-├── requirements.txt
-├── setup.py
+├── tests
+│   └── test_model.ipynb
 └── treat_sim
     ├── data
     │   └── ed_arrivals.csv
     ├── distributions.py
     ├── __init__.py
     └── model.py
 ```
 
 * `binder/` - contains the environment.yml file (sim) and all dependencies managed via conda, used to set-up the notebooks on Binder.
 * `CHANGES.md` - changelog with record of notable changes to project between versions.
 * `CITATION.cff` - citation information for the package.
 * `LICENSE` - details of the MIT permissive license of this work.
-* `MANIFEST.in` - files to include in the package.
 * `notebooks/` - contains a notebook to run the model and provides basic enhanced model documentation.
+* `pyproject.toml` - used to build and distribute python package inc. managing a list of package dependencies.
 * `README.md` - what you are reading now!
-* `requirements.txt` - list of packages and minimum versions required.
-* `setup.py` - used to build and distribute package.
+* `tests/` - contains automated testing code
 * `treat_sim/` - contains packaged version of the model.
     * `data/` - directory containing data file used by package.
     * `distributions.py` - distribution classes.
     * `__init__.py` - required as part of package - contains author and version.
     * `model.py` - example SimPy model.
 
+
 ## Citation
 
 If you use the materials within this repository we would appreciate a citation.
 
 ```
-Monks, T., Harper, A., & Heather, A. (2024). Towards Sharing Tools, and Artifacts, for Reusable Simulation: a minimal model example (v1.2.0). Zenodo. https://doi.org/10.5281//zenodo.10026326
+Monks, T., Harper, A., & Heather, A. (2024). Towards Sharing Tools, and Artifacts, for Reusable Simulation: a minimal model example (v2.1.0). Zenodo. https://doi.org/10.5281//zenodo.10026326
 ```
 
 ```bibtex
 @software{stars_treat_sim,
   author       = {Thomas Monks, Alison Harper and Amy Heather},
   title        = {{Towards Sharing Tools, and Artifacts, for Reusable 
                    Simulation: a minimal model example}},
   month        = May,
   year         = 2024,
   publisher    = {Zenodo},
-  version      = {v1.2.0},
+  version      = {v2.0.0},
   doi          = {10.5281//zenodo.10026326.},
   url          = {https://doi.org/10.5281//zenodo.10026326}
 }
 ```
+
```

