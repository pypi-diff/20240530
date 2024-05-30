# Comparing `tmp/meafs-4.6.3.tar.gz` & `tmp/meafs-4.7.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meafs-4.6.3.tar", last modified: Tue Apr 23 18:59:59 2024, max compression
+gzip compressed data, was "meafs-4.7.12.tar", last modified: Thu May 30 18:43:08 2024, max compression
```

## Comparing `meafs-4.6.3.tar` & `meafs-4.7.12.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:59:59.607937 meafs-4.6.3/
--rwxr-xr-x   0 castro    (1000) users      (984)     1074 2024-04-23 18:50:35.000000 meafs-4.6.3/LICENSE.txt
--rwxr-xr-x   0 castro    (1000) users      (984)       32 2024-04-23 18:50:35.000000 meafs-4.6.3/MANIFEST.in
--rw-r--r--   0 castro    (1000) users      (984)     9616 2024-04-23 18:59:59.607937 meafs-4.6.3/PKG-INFO
--rwxr-xr-x   0 castro    (1000) users      (984)     8957 2024-04-23 18:55:09.000000 meafs-4.6.3/README.md
-drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:59:59.607937 meafs-4.6.3/meafs.egg-info/
--rw-r--r--   0 castro    (1000) users      (984)     9616 2024-04-23 18:59:59.000000 meafs-4.6.3/meafs.egg-info/PKG-INFO
--rw-r--r--   0 castro    (1000) users      (984)      914 2024-04-23 18:59:59.000000 meafs-4.6.3/meafs.egg-info/SOURCES.txt
--rw-r--r--   0 castro    (1000) users      (984)        1 2024-04-23 18:59:59.000000 meafs-4.6.3/meafs.egg-info/dependency_links.txt
--rw-r--r--   0 castro    (1000) users      (984)      156 2024-04-23 18:59:59.000000 meafs-4.6.3/meafs.egg-info/entry_points.txt
--rw-r--r--   0 castro    (1000) users      (984)       85 2024-04-23 18:59:59.000000 meafs-4.6.3/meafs.egg-info/requires.txt
--rw-r--r--   0 castro    (1000) users      (984)       11 2024-04-23 18:59:59.000000 meafs-4.6.3/meafs.egg-info/top_level.txt
-drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:59:59.604604 meafs-4.6.3/meafs_code/
--rwxr-xr-x   0 castro    (1000) users      (984)       26 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/__init__.py
--rwxr-xr-x   0 castro    (1000) users      (984)       37 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/__main__.py
--rwxr-xr-x   0 castro    (1000) users      (984)       78 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/convert.sh
--rwxr-xr-x   0 castro    (1000) users      (984)     4259 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/desktop_entry.py
--rw-r--r--   0 castro    (1000) users      (984)    11095 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/fitsettings.ui
--rw-r--r--   0 castro    (1000) users      (984)    14517 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/fitsettings_qt.py
--rwxr-xr-x   0 castro    (1000) users      (984)    46643 2024-04-23 18:59:53.000000 meafs-4.6.3/meafs_code/gui.py
--rwxr-xr-x   0 castro    (1000) users      (984)    42133 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/gui_qt.py
-drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:59:59.604604 meafs-4.6.3/meafs_code/images/
--rw-r--r--   0 castro    (1000) users      (984)   190114 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/images/Meafs_Gui.png
--rwxr-xr-x   0 castro    (1000) users      (984)    42476 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/images/Meafs_Icon.ico
--rwxr-xr-x   0 castro    (1000) users      (984)   220589 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/images/Meafs_Logo.png
--rwxr-xr-x   0 castro    (1000) users      (984)    36066 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/meafs.ui
-drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:59:59.607937 meafs-4.6.3/meafs_code/scripts/
--rwxr-xr-x   0 castro    (1000) users      (984)      142 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/scripts/__init__.py
--rwxr-xr-x   0 castro    (1000) users      (984)    12110 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/scripts/abundance_analysis.py
--rwxr-xr-x   0 castro    (1000) users      (984)    28910 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/scripts/abundance_fit.py
--rwxr-xr-x   0 castro    (1000) users      (984)     1936 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/scripts/bisec_interpol.c
--rwxr-xr-x   0 castro    (1000) users      (984)    15472 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/scripts/bisec_interpol.so
--rwxr-xr-x   0 castro    (1000) users      (984)      148 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/scripts/comp.sh
--rw-r--r--   0 castro    (1000) users      (984)     5078 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/scripts/fit_functions.py
--rw-r--r--   0 castro    (1000) users      (984)     4975 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/scripts/turbospec_functions.py
--rwxr-xr-x   0 castro    (1000) users      (984)     3343 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/scripts/unify_plots.py
--rw-r--r--   0 castro    (1000) users      (984)     2868 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/scripts/voigt_functions.py
--rw-r--r--   0 castro    (1000) users      (984)       27 2024-04-23 18:50:35.000000 meafs-4.6.3/meafs_code/settings.csv
--rwxr-xr-x   0 castro    (1000) users      (984)      766 2024-04-23 18:59:53.000000 meafs-4.6.3/pyproject.toml
--rw-r--r--   0 castro    (1000) users      (984)       38 2024-04-23 18:59:59.607937 meafs-4.6.3/setup.cfg
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-05-30 18:43:08.834639 meafs-4.7.12/
+-rwxr-xr-x   0 castro    (1000) users      (984)     1074 2024-05-30 18:40:25.000000 meafs-4.7.12/LICENSE.txt
+-rwxr-xr-x   0 castro    (1000) users      (984)       32 2024-05-30 18:40:25.000000 meafs-4.7.12/MANIFEST.in
+-rw-r--r--   0 castro    (1000) users      (984)    10738 2024-05-30 18:43:08.834639 meafs-4.7.12/PKG-INFO
+-rwxr-xr-x   0 castro    (1000) users      (984)     9998 2024-05-30 18:40:25.000000 meafs-4.7.12/README.md
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-05-30 18:43:08.834639 meafs-4.7.12/meafs.egg-info/
+-rw-r--r--   0 castro    (1000) users      (984)    10738 2024-05-30 18:43:08.000000 meafs-4.7.12/meafs.egg-info/PKG-INFO
+-rw-r--r--   0 castro    (1000) users      (984)      877 2024-05-30 18:43:08.000000 meafs-4.7.12/meafs.egg-info/SOURCES.txt
+-rw-r--r--   0 castro    (1000) users      (984)        1 2024-05-30 18:43:08.000000 meafs-4.7.12/meafs.egg-info/dependency_links.txt
+-rw-r--r--   0 castro    (1000) users      (984)      156 2024-05-30 18:43:08.000000 meafs-4.7.12/meafs.egg-info/entry_points.txt
+-rw-r--r--   0 castro    (1000) users      (984)       95 2024-05-30 18:43:08.000000 meafs-4.7.12/meafs.egg-info/requires.txt
+-rw-r--r--   0 castro    (1000) users      (984)       11 2024-05-30 18:43:08.000000 meafs-4.7.12/meafs.egg-info/top_level.txt
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-05-30 18:43:08.831306 meafs-4.7.12/meafs_code/
+-rwxr-xr-x   0 castro    (1000) users      (984)       26 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/__init__.py
+-rwxr-xr-x   0 castro    (1000) users      (984)       37 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/__main__.py
+-rwxr-xr-x   0 castro    (1000) users      (984)       78 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/convert.sh
+-rwxr-xr-x   0 castro    (1000) users      (984)     4452 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/desktop_entry.py
+-rw-r--r--   0 castro    (1000) users      (984)    11095 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/fitsettings.ui
+-rw-r--r--   0 castro    (1000) users      (984)    14517 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/fitsettings_qt.py
+-rwxr-xr-x   0 castro    (1000) users      (984)    62126 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/gui.py
+-rwxr-xr-x   0 castro    (1000) users      (984)    43257 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/gui_qt.py
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-05-30 18:43:08.831306 meafs-4.7.12/meafs_code/images/
+-rw-r--r--   0 castro    (1000) users      (984)   190114 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/images/Meafs_Gui.png
+-rwxr-xr-x   0 castro    (1000) users      (984)    42476 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/images/Meafs_Icon.ico
+-rwxr-xr-x   0 castro    (1000) users      (984)   220589 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/images/Meafs_Logo.png
+-rwxr-xr-x   0 castro    (1000) users      (984)    36492 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/meafs.ui
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-05-30 18:43:08.834639 meafs-4.7.12/meafs_code/scripts/
+-rwxr-xr-x   0 castro    (1000) users      (984)      142 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/scripts/__init__.py
+-rwxr-xr-x   0 castro    (1000) users      (984)    13799 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/scripts/abundance_analysis.py
+-rwxr-xr-x   0 castro    (1000) users      (984)    34350 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/scripts/abundance_fit.py
+-rwxr-xr-x   0 castro    (1000) users      (984)     2321 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/scripts/bisec_interpol.c
+-rwxr-xr-x   0 castro    (1000) users      (984)      148 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/scripts/comp.sh
+-rw-r--r--   0 castro    (1000) users      (984)     6249 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/scripts/fit_functions.py
+-rw-r--r--   0 castro    (1000) users      (984)     6727 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/scripts/turbospec_functions.py
+-rwxr-xr-x   0 castro    (1000) users      (984)     3410 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/scripts/unify_plots.py
+-rw-r--r--   0 castro    (1000) users      (984)     5129 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/scripts/voigt_functions.py
+-rw-r--r--   0 castro    (1000) users      (984)       27 2024-05-30 18:40:25.000000 meafs-4.7.12/meafs_code/settings.csv
+-rwxr-xr-x   0 castro    (1000) users      (984)      831 2024-05-30 18:40:25.000000 meafs-4.7.12/pyproject.toml
+-rw-r--r--   0 castro    (1000) users      (984)       38 2024-05-30 18:43:08.834639 meafs-4.7.12/setup.cfg
```

### Comparing `meafs-4.6.3/LICENSE.txt` & `meafs-4.7.12/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meafs-4.6.3/PKG-INFO` & `meafs-4.7.12/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: meafs
-Version: 4.6.3
+Version: 4.7.12
 Summary: Multiple Element Abundance Fit Software
 Author: Matheus J. Castro
-Project-URL: Homepage, https://github.com/MatheusJCastro/meafs
+Project-URL: homepage, https://meafs.readthedocs.io/
+Project-URL: repository, https://github.com/MatheusJCastro/meafs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: astropy
@@ -16,42 +17,52 @@
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: desktop_file==1.3
 Requires-Dist: pathlib
 Requires-Dist: PyQt6
 Requires-Dist: dill
+Requires-Dist: qtconsole
 
 ![Meafs Logo](meafs_code/images/Meafs_Logo.png)
 
 # Multiple Element Abundance Fit Software - MEAFS
 
 *Written by: Matheus J. Castro*  
 *Under MIT License*  
 
+More information at: [https://meafs.readthedocs.io/](https://meafs.readthedocs.io/)
+
 <hr/>
 <hr/>
 
 ## Table of Contents
 
-1. [Aims](#Aims)
-2. [Prerequisites](#Prerequisites)
-3. [Instalation](#Instalation)
-    1. [Creating Anaconda Environment (recommended)](<#creating-anaconda-environment-recommended>)
-    2. [Getting the pip version (recommended)](<#getting-the-pip-version-recommended-not-yet-working>)
-    3. [Cloning from GitHub](<#cloning-from-github>)
-    4. [Adding the PATH (for non Anaconda installations)](<#adding-the-path-for-non-anaconda-installations>)
-    5. [Step-by-Step for Windows (Python + GCC)](<#step-by-step-for-windows-python--gcc>)
-    6. [Compilation](<#compilation>)
-4. [Usage](#Usage)
-    1. [With Installation](<#with-installation>)
-    2. [Without Installation](<#without-installation>)
-    3. [Flags and Arguments](<#flags-and-arguments>)
-    4. [Auto Save](<#auto-save>)
-5. [Uninstall](#Uninstall)
+- [Multiple Element Abundance Fit Software - MEAFS](#multiple-element-abundance-fit-software---meafs)
+  - [Table of Contents](#table-of-contents)
+  - [Aims](#aims)
+  - [Prerequisites](#prerequisites)
+    - [Creating Anaconda Environment (recommended)](#creating-anaconda-environment-recommended)
+    - [Step-by-Step for Windows (Python + GCC)](#step-by-step-for-windows-python--gcc)
+      - [Python](#python)
+      - [GCC](#gcc)
+  - [Installation](#installation)
+    - [Getting the pip version (recommended)](#getting-the-pip-version-recommended)
+    - [Cloning from GitHub](#cloning-from-github)
+  - [Post Installation](#post-installation)
+    - [Adding the PATH (for non Anaconda installations)](#adding-the-path-for-non-anaconda-installations)
+      - [Linux](#linux)
+      - [Windows](#windows)
+    - [Compilation](#compilation)
+  - [Uninstall](#uninstall)
+  - [Basic Usage](#basic-usage)
+    - [With Installation](#with-installation)
+    - [Without Installation](#without-installation)
+    - [Flags and Arguments](#flags-and-arguments)
+    - [Auto Save](#auto-save)
 
 ## Aims
 
 The MEAFS is a fitting tool software for spectra abundance analysis. The aims is to provide a medium to high analysis for each individual absorption line in a given spectrum.  
 The software also fits the wavelength shift, continuum and convolution of the spectrum.
 
 ![Meafs GUI](meafs_code/images/Meafs_Gui.png)
@@ -59,36 +70,63 @@
 ## Prerequisites
 
 - Python3 and GCC needs to be previously installed in the system (step-by-step to install for Windows users [bellow](<#step-by-step-for-windows-python--gcc>));
 
 - A software for creating a synthetic spectrum also needs to be previously installed. This version of MEAFS is compatible with the following softwares:
     - Turbospectrum2019: [https://github.com/bertrandplez/Turbospectrum2019](https://github.com/bertrandplez/Turbospectrum2019)
 
-- Optionally: to execute the `unify_plots.py`, a LaTeX installation must be present on the system.
+- Optionally: to execute the *unify_plots.py*, a LaTeX installation must be present on the system.
 
 - Optionally: [Anaconda](<#creating-anaconda-environment-recommended>).
 
-## Instalation
-
-There are many options to run MEAFS. We strongly recommend the use of Anaconda environment, but it is not mandatory.  
-You can install it from pip or run directly the source code from the repository.  
-
-All the methods listed below work in Linux, Windows or MacOS **if you have python and gcc installed** (step-by-step to install for Windows users [bellow](<#step-by-step-for-windows-python--gcc>)).
-
 ### Creating Anaconda Environment (recommended)
 - First, download anaconda [here](https://www.anaconda.com/products/individual#download-section) and execute the script.
 
     - For Linux users, if needed, export anaconda to your path by adding the line `export PATH="/home/USERNAME/anaconda3/bin:$PATH"` (changing the `USERNAME` to your user) to the `~/.bashrc` file. Close and open a new terminal to update the path.
 
     - If desirable, disable autoactivation of anaconda with `conda config --set auto_activate_base false`.
 
 - Create MEAFS enviroment with `conda create python -n meafs`;
 
 - Then, to activate the environment, type `conda activate meafs`;
 
+### Step-by-Step for Windows (Python + GCC)
+
+If you are running Windows **without** Anaconda, you need to install Python and GCC, if you did not already have them. Otherwise, you can skip this.  
+If you are using Windows **with** Anaconda, only GCC is required.
+
+Obs: this step-by-step guide was made using a fresh new install of Windows 10.
+
+#### Python
+
+Go to [Python Windows Releases](https://www.python.org/downloads/windows/) and download an stable release by clicking on it and downloading the *Windows installer (64-bit) Recommended*. After downloading, exectue the files and follow the installation process.
+
+- Add the Python folder to the path.
+    - Open the menu and search for *path*, click in *Edit the system environment variables*, at the bottom right click in *Environment Variables...*, in the tab *System variables* (attention: not the *User variables for Username*), look for the variable *Path* and click on *Edit*. Add two new lines:
+        - `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311`
+        - `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311\Scripts`
+        - Change `USERNAME` with your username and `Python311` to the actual version that you installed.
+- Go to the python folder (ex: `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311`) and create a copy of the `python.exe` file in the same location with the name `python3.11.exe`
+
+#### GCC
+
+Download the *x64* version of [Winlibs](https://winlibs.com).
+    
+- Choose the x64 MCF **with** all the libraries;
+- After downloading, decompress the file and move the `mingw64` folder to `C:\Program Files\`;
+- Now add the folder `bin` of the `mingw64` folder to the path:
+  - Use the sames steps as before but now add the line: `C:\Program Files\mingw64\bin`.
+
+## Installation
+
+There are many options to run MEAFS. We strongly recommend the use of Anaconda environment, but it is not mandatory.  
+You can install it from pip or run directly the source code from the repository.  
+
+All the methods listed below work in Linux, Windows or MacOS **if you have python and gcc installed** (step-by-step to install for Windows users [bellow](<#step-by-step-for-windows-python--gcc>)).
+
 ### Getting the pip version (recommended)
 
 The pip version can easily be acquired by typing in the terminal:
 
 ```bash
 pip install meafs
 ```
@@ -97,29 +135,31 @@
 
 Or you can directly clone from the GitHub page with:
 
 ```bash
 git clone https://github.com/MatheusJCastro/meafs.git
 ```
 
-After cloning, you can install it with pip or run without any installation at all (see the [Usage](<#without-installation>)  section).  
+After cloning, you can install it with pip or run without any installation at all (see the [Usage - Without Installation](<#without-installation>) section).  
 
 To build the package and install it with pip from the source, first install the `build` package:  
 
 ```bash
 pip install build
 ```
 
 Then go to the MEAFS source code directory and type:
 
 ```bash
 python3 -m build
 pip install .
 ```
 
+## Post Installation
+
 ### Adding the PATH (for non Anaconda installations)
 If you do not use Anaconda, you need to add the path of the pip scripts into the system path variable if you have not already done so.  
 **This step is not necessary if you are running without installation.**
 
 #### Linux
 For Linux users, you can add the following line in the end of the file `~/.bashrc`, changing `USER` to your own user.
 
@@ -129,97 +169,94 @@
 
 For some Linux distributions and Python installations, the locale of the executables can slightly change. If this does not work out, you can try differents paths such as `/usr/local/bin` and others.
 
 #### Windows
 
 For Windows users, you need to open the menu and search for *path*, click in *Edit the system environment variables*, at the bottom right click in *Environment Variables...*, in the tab *System variables* (attention: not the *User variables for Username*), look for the variable *Path* and click on *Edit*. Add a new line with one of the followings (check the python location first):
 
-```bash
+```bat
 C:\Users\Windows\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.11_qbz5n2kfra8p0\LocalCache\local-packages\Python311\Scripts
 ```
 
 Or:
 
-```bash
+```bat
 C:\Users\USERNAME\AppData\Local\Programs\Python\Python311\Scripts
 ```
 
 **Be aware of different Python versions, the path will change also. Always verify if the current path exists.**
 
-### Step-by-Step for Windows (Python + GCC)
-Obs: this step-by-step guide was made using a fresh new install of Windows 10.
-
-#### Python
+### Compilation
 
-Go to [Python Windows Releases](https://www.python.org/downloads/windows/) and download an stable release by clicking on it and downloading the *Windows installer (64-bit) Recommended*. After downloading, exectue the files and follow the installation process.
+There is one file written in C Language (`meafs/meafs_code/scripts/bisec_interpol.c`), **in the first run, MEAFS will compile the C library using GCC**. Otherwise, the compilation directives can be found in the `meafs/meafs_code/scripts/comp.sh`. The C file needs to be compiled as a shared library, when using *GCC Compiler*, this can be achieved by adding the `-shared` flag.
 
-- Add the Python folder to the path.
-    - Open the menu and search for *path*, click in *Edit the system environment variables*, at the bottom right click in *Environment Variables...*, in the tab *System variables* (attention: not the *User variables for Username*), look for the variable *Path* and click on *Edit*. Add two new lines:
-        - `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311`
-        - `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311\Scripts`
-        - Change `USERNAME` with your username and `Python311` to the actual version that you installed.
-- Go to the python folder (ex: `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311`) and create a copy of the `python.exe` file in the same location with the name `python3.11.exe`
+If the auto compilation fails, for Linux users, just add execution privileges at the `comp.sh` file and execute it in a terminal to create the binary. For that, open a terminal in the `meafs/meafs_code/scripts/` folder and type:
 
-#### GCC
+```bash
+chmod +x comp.sh
+./comp.sh
+```
 
-Download the *x64* version of [Winlibs](https://winlibs.com).
-    
-- Choose the x64 MCF **with** all the libraries;
-- After downloading, decompress the file and move the `mingw64` folder to `C:\Program Files\`;
-- Now add the folder `bin` of the `mingw64` folder to the path:
-        - Use the sames steps as before but now add the line: `C:\Program Files\mingw64\bin`.
+If you are on Windows, check this `comp.sh` file for the full `gcc` command.
 
-### Compilation
+## Uninstall
 
-There is one file written in C Language (`meafs/meafs_code/scripts/bisec_interpol.c`), the compilation directives can be found in the `meafs/meafs_code/scripts/comp.sh`. The C file needs to be compiled as a shared library, when using *GCC Compiler*, this can be achieved by adding the `-shared` flag.
+If you did not install with pip (both directly or by cloning), you can just erase the *meafs* folder.  
 
-For Linux users just add execution privileges at the `comp.sh` file and execute it in a terminal to create the binary. For that, open a terminal in the `meafs/meafs_code/scripts/` folder and type:
+Otherwise, first remove the menu entries (if you have added it, see [Usage - With Installation](<#with-installation>)) and then uninstall:
 
 ```bash
-chmod +x comp.sh
-./comp.sh
+meafs-desktop-remove
+pip uninstall meafs
 ```
 
-## Usage
+## Basic Usage
 
 ### With Installation
 You can create menu entries for MEAFS by typing in the terminal or cmd:  
 
 ```bash
 meafs-desktop-create
 ```
 
 Then, search in the menu for *MEAFS*, and in Windows, a Desktop link will also be created.  
-But, if you do not want to create menu entries, just type `meafs` or `python -m meafs` in the terminal or cmd to launch it.
+Or, you can just type in the terminal or cmd: 
+
+```bash
+meafs
+```
+
+Or:
+
+```bash
+python -m meafs
+```
+
+For the command line option, do not forget to activate the Anaconda environment if you are using it. For the menu entry, this is done automatically if necessary.
 
 ### Without Installation
-Simply execute the file `gui.py` and it will power the GUI.
+Simply execute the file `meafs_code/gui.py` and it will power the GUI.
 
 ### Flags and Arguments
 
 There are some flags that can be passed with the command-line.
 
-- `-h` or `--help`: Show the help section;
-- `-v` or `--version`: Show version number;
-- `-l` or `--last`: Load the last closed session. Default location is `meafs_code/auto_save_last.pkl`
-- `-s` or `--load-auto-save`: Load the auto saved session. Default location is: `meafs_code/auto_save.pkl`
+- `-h`, `--help`: Show the help section;
+- `-v`, `--version`: Show version number;
+- `-l`, `--last`: Load the last closed session. Default location is `meafs_code/auto_save_last.pkl`;
+- `-s`, `--load-auto-save`: Load the auto saved session. Default location is: `meafs_code/auto_save.pkl`.
 
-Also, any saved section can be passed as an argument. It will power the GUI with it. If no argument is given, the GUI will power with a new empty session.
+Also, any saved section can be passed as an argument and meafs will power the GUI with it:
+
+```bash
+meafs path/to/session.pkl
+```
+
+If no argument is given, the GUI will power with a new empty session.
 
 ### Auto Save
 In the *File* menu there is an *Auto Save* option. When checked, MEAFS will save the session every 5 seconds in a file named `auto_save.pkl`.  
 Also, if auto save is enabled, when MEAFS is closed, it will save the session in the `auto_save_last.pkl` file.  
 These files are located under the MEAFS directory and the `-h` [flag](<#flags-and-arguments>) will show the location.  
-To load any of these files, simply use the [flags](<#flags-and-arguments>) or load them in the *File* - *Open...* menu
-
-## Uninstall
-
-If you did not install with pip (both directly or by cloning), you can just erase the *meafs* folder.  
-
-Otherwise, first remove the menu entries (if you have added it) and then uninstall:
-
-```bash
-meafs-desktop-remove
-pip uninstall meafs
-```
+To load any of these files, simply use the [flags](<#flags-and-arguments>) or load them in the *File* - *Open...* menu.
 
 <hr/>
```

### Comparing `meafs-4.6.3/README.md` & `meafs-4.7.12/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 ![Meafs Logo](meafs_code/images/Meafs_Logo.png)
 
 # Multiple Element Abundance Fit Software - MEAFS
 
 *Written by: Matheus J. Castro*  
 *Under MIT License*  
 
+More information at: [https://meafs.readthedocs.io/](https://meafs.readthedocs.io/)
+
 <hr/>
 <hr/>
 
 ## Table of Contents
 
-1. [Aims](#Aims)
-2. [Prerequisites](#Prerequisites)
-3. [Instalation](#Instalation)
-    1. [Creating Anaconda Environment (recommended)](<#creating-anaconda-environment-recommended>)
-    2. [Getting the pip version (recommended)](<#getting-the-pip-version-recommended-not-yet-working>)
-    3. [Cloning from GitHub](<#cloning-from-github>)
-    4. [Adding the PATH (for non Anaconda installations)](<#adding-the-path-for-non-anaconda-installations>)
-    5. [Step-by-Step for Windows (Python + GCC)](<#step-by-step-for-windows-python--gcc>)
-    6. [Compilation](<#compilation>)
-4. [Usage](#Usage)
-    1. [With Installation](<#with-installation>)
-    2. [Without Installation](<#without-installation>)
-    3. [Flags and Arguments](<#flags-and-arguments>)
-    4. [Auto Save](<#auto-save>)
-5. [Uninstall](#Uninstall)
+- [Multiple Element Abundance Fit Software - MEAFS](#multiple-element-abundance-fit-software---meafs)
+  - [Table of Contents](#table-of-contents)
+  - [Aims](#aims)
+  - [Prerequisites](#prerequisites)
+    - [Creating Anaconda Environment (recommended)](#creating-anaconda-environment-recommended)
+    - [Step-by-Step for Windows (Python + GCC)](#step-by-step-for-windows-python--gcc)
+      - [Python](#python)
+      - [GCC](#gcc)
+  - [Installation](#installation)
+    - [Getting the pip version (recommended)](#getting-the-pip-version-recommended)
+    - [Cloning from GitHub](#cloning-from-github)
+  - [Post Installation](#post-installation)
+    - [Adding the PATH (for non Anaconda installations)](#adding-the-path-for-non-anaconda-installations)
+      - [Linux](#linux)
+      - [Windows](#windows)
+    - [Compilation](#compilation)
+  - [Uninstall](#uninstall)
+  - [Basic Usage](#basic-usage)
+    - [With Installation](#with-installation)
+    - [Without Installation](#without-installation)
+    - [Flags and Arguments](#flags-and-arguments)
+    - [Auto Save](#auto-save)
 
 ## Aims
 
 The MEAFS is a fitting tool software for spectra abundance analysis. The aims is to provide a medium to high analysis for each individual absorption line in a given spectrum.  
 The software also fits the wavelength shift, continuum and convolution of the spectrum.
 
 ![Meafs GUI](meafs_code/images/Meafs_Gui.png)
@@ -36,36 +45,63 @@
 ## Prerequisites
 
 - Python3 and GCC needs to be previously installed in the system (step-by-step to install for Windows users [bellow](<#step-by-step-for-windows-python--gcc>));
 
 - A software for creating a synthetic spectrum also needs to be previously installed. This version of MEAFS is compatible with the following softwares:
     - Turbospectrum2019: [https://github.com/bertrandplez/Turbospectrum2019](https://github.com/bertrandplez/Turbospectrum2019)
 
-- Optionally: to execute the `unify_plots.py`, a LaTeX installation must be present on the system.
+- Optionally: to execute the *unify_plots.py*, a LaTeX installation must be present on the system.
 
 - Optionally: [Anaconda](<#creating-anaconda-environment-recommended>).
 
-## Instalation
-
-There are many options to run MEAFS. We strongly recommend the use of Anaconda environment, but it is not mandatory.  
-You can install it from pip or run directly the source code from the repository.  
-
-All the methods listed below work in Linux, Windows or MacOS **if you have python and gcc installed** (step-by-step to install for Windows users [bellow](<#step-by-step-for-windows-python--gcc>)).
-
 ### Creating Anaconda Environment (recommended)
 - First, download anaconda [here](https://www.anaconda.com/products/individual#download-section) and execute the script.
 
     - For Linux users, if needed, export anaconda to your path by adding the line `export PATH="/home/USERNAME/anaconda3/bin:$PATH"` (changing the `USERNAME` to your user) to the `~/.bashrc` file. Close and open a new terminal to update the path.
 
     - If desirable, disable autoactivation of anaconda with `conda config --set auto_activate_base false`.
 
 - Create MEAFS enviroment with `conda create python -n meafs`;
 
 - Then, to activate the environment, type `conda activate meafs`;
 
+### Step-by-Step for Windows (Python + GCC)
+
+If you are running Windows **without** Anaconda, you need to install Python and GCC, if you did not already have them. Otherwise, you can skip this.  
+If you are using Windows **with** Anaconda, only GCC is required.
+
+Obs: this step-by-step guide was made using a fresh new install of Windows 10.
+
+#### Python
+
+Go to [Python Windows Releases](https://www.python.org/downloads/windows/) and download an stable release by clicking on it and downloading the *Windows installer (64-bit) Recommended*. After downloading, exectue the files and follow the installation process.
+
+- Add the Python folder to the path.
+    - Open the menu and search for *path*, click in *Edit the system environment variables*, at the bottom right click in *Environment Variables...*, in the tab *System variables* (attention: not the *User variables for Username*), look for the variable *Path* and click on *Edit*. Add two new lines:
+        - `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311`
+        - `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311\Scripts`
+        - Change `USERNAME` with your username and `Python311` to the actual version that you installed.
+- Go to the python folder (ex: `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311`) and create a copy of the `python.exe` file in the same location with the name `python3.11.exe`
+
+#### GCC
+
+Download the *x64* version of [Winlibs](https://winlibs.com).
+    
+- Choose the x64 MCF **with** all the libraries;
+- After downloading, decompress the file and move the `mingw64` folder to `C:\Program Files\`;
+- Now add the folder `bin` of the `mingw64` folder to the path:
+  - Use the sames steps as before but now add the line: `C:\Program Files\mingw64\bin`.
+
+## Installation
+
+There are many options to run MEAFS. We strongly recommend the use of Anaconda environment, but it is not mandatory.  
+You can install it from pip or run directly the source code from the repository.  
+
+All the methods listed below work in Linux, Windows or MacOS **if you have python and gcc installed** (step-by-step to install for Windows users [bellow](<#step-by-step-for-windows-python--gcc>)).
+
 ### Getting the pip version (recommended)
 
 The pip version can easily be acquired by typing in the terminal:
 
 ```bash
 pip install meafs
 ```
@@ -74,29 +110,31 @@
 
 Or you can directly clone from the GitHub page with:
 
 ```bash
 git clone https://github.com/MatheusJCastro/meafs.git
 ```
 
-After cloning, you can install it with pip or run without any installation at all (see the [Usage](<#without-installation>)  section).  
+After cloning, you can install it with pip or run without any installation at all (see the [Usage - Without Installation](<#without-installation>) section).  
 
 To build the package and install it with pip from the source, first install the `build` package:  
 
 ```bash
 pip install build
 ```
 
 Then go to the MEAFS source code directory and type:
 
 ```bash
 python3 -m build
 pip install .
 ```
 
+## Post Installation
+
 ### Adding the PATH (for non Anaconda installations)
 If you do not use Anaconda, you need to add the path of the pip scripts into the system path variable if you have not already done so.  
 **This step is not necessary if you are running without installation.**
 
 #### Linux
 For Linux users, you can add the following line in the end of the file `~/.bashrc`, changing `USER` to your own user.
 
@@ -106,97 +144,94 @@
 
 For some Linux distributions and Python installations, the locale of the executables can slightly change. If this does not work out, you can try differents paths such as `/usr/local/bin` and others.
 
 #### Windows
 
 For Windows users, you need to open the menu and search for *path*, click in *Edit the system environment variables*, at the bottom right click in *Environment Variables...*, in the tab *System variables* (attention: not the *User variables for Username*), look for the variable *Path* and click on *Edit*. Add a new line with one of the followings (check the python location first):
 
-```bash
+```bat
 C:\Users\Windows\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.11_qbz5n2kfra8p0\LocalCache\local-packages\Python311\Scripts
 ```
 
 Or:
 
-```bash
+```bat
 C:\Users\USERNAME\AppData\Local\Programs\Python\Python311\Scripts
 ```
 
 **Be aware of different Python versions, the path will change also. Always verify if the current path exists.**
 
-### Step-by-Step for Windows (Python + GCC)
-Obs: this step-by-step guide was made using a fresh new install of Windows 10.
-
-#### Python
+### Compilation
 
-Go to [Python Windows Releases](https://www.python.org/downloads/windows/) and download an stable release by clicking on it and downloading the *Windows installer (64-bit) Recommended*. After downloading, exectue the files and follow the installation process.
+There is one file written in C Language (`meafs/meafs_code/scripts/bisec_interpol.c`), **in the first run, MEAFS will compile the C library using GCC**. Otherwise, the compilation directives can be found in the `meafs/meafs_code/scripts/comp.sh`. The C file needs to be compiled as a shared library, when using *GCC Compiler*, this can be achieved by adding the `-shared` flag.
 
-- Add the Python folder to the path.
-    - Open the menu and search for *path*, click in *Edit the system environment variables*, at the bottom right click in *Environment Variables...*, in the tab *System variables* (attention: not the *User variables for Username*), look for the variable *Path* and click on *Edit*. Add two new lines:
-        - `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311`
-        - `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311\Scripts`
-        - Change `USERNAME` with your username and `Python311` to the actual version that you installed.
-- Go to the python folder (ex: `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311`) and create a copy of the `python.exe` file in the same location with the name `python3.11.exe`
+If the auto compilation fails, for Linux users, just add execution privileges at the `comp.sh` file and execute it in a terminal to create the binary. For that, open a terminal in the `meafs/meafs_code/scripts/` folder and type:
 
-#### GCC
+```bash
+chmod +x comp.sh
+./comp.sh
+```
 
-Download the *x64* version of [Winlibs](https://winlibs.com).
-    
-- Choose the x64 MCF **with** all the libraries;
-- After downloading, decompress the file and move the `mingw64` folder to `C:\Program Files\`;
-- Now add the folder `bin` of the `mingw64` folder to the path:
-        - Use the sames steps as before but now add the line: `C:\Program Files\mingw64\bin`.
+If you are on Windows, check this `comp.sh` file for the full `gcc` command.
 
-### Compilation
+## Uninstall
 
-There is one file written in C Language (`meafs/meafs_code/scripts/bisec_interpol.c`), the compilation directives can be found in the `meafs/meafs_code/scripts/comp.sh`. The C file needs to be compiled as a shared library, when using *GCC Compiler*, this can be achieved by adding the `-shared` flag.
+If you did not install with pip (both directly or by cloning), you can just erase the *meafs* folder.  
 
-For Linux users just add execution privileges at the `comp.sh` file and execute it in a terminal to create the binary. For that, open a terminal in the `meafs/meafs_code/scripts/` folder and type:
+Otherwise, first remove the menu entries (if you have added it, see [Usage - With Installation](<#with-installation>)) and then uninstall:
 
 ```bash
-chmod +x comp.sh
-./comp.sh
+meafs-desktop-remove
+pip uninstall meafs
 ```
 
-## Usage
+## Basic Usage
 
 ### With Installation
 You can create menu entries for MEAFS by typing in the terminal or cmd:  
 
 ```bash
 meafs-desktop-create
 ```
 
 Then, search in the menu for *MEAFS*, and in Windows, a Desktop link will also be created.  
-But, if you do not want to create menu entries, just type `meafs` or `python -m meafs` in the terminal or cmd to launch it.
+Or, you can just type in the terminal or cmd: 
+
+```bash
+meafs
+```
+
+Or:
+
+```bash
+python -m meafs
+```
+
+For the command line option, do not forget to activate the Anaconda environment if you are using it. For the menu entry, this is done automatically if necessary.
 
 ### Without Installation
-Simply execute the file `gui.py` and it will power the GUI.
+Simply execute the file `meafs_code/gui.py` and it will power the GUI.
 
 ### Flags and Arguments
 
 There are some flags that can be passed with the command-line.
 
-- `-h` or `--help`: Show the help section;
-- `-v` or `--version`: Show version number;
-- `-l` or `--last`: Load the last closed session. Default location is `meafs_code/auto_save_last.pkl`
-- `-s` or `--load-auto-save`: Load the auto saved session. Default location is: `meafs_code/auto_save.pkl`
+- `-h`, `--help`: Show the help section;
+- `-v`, `--version`: Show version number;
+- `-l`, `--last`: Load the last closed session. Default location is `meafs_code/auto_save_last.pkl`;
+- `-s`, `--load-auto-save`: Load the auto saved session. Default location is: `meafs_code/auto_save.pkl`.
 
-Also, any saved section can be passed as an argument. It will power the GUI with it. If no argument is given, the GUI will power with a new empty session.
+Also, any saved section can be passed as an argument and meafs will power the GUI with it:
+
+```bash
+meafs path/to/session.pkl
+```
+
+If no argument is given, the GUI will power with a new empty session.
 
 ### Auto Save
 In the *File* menu there is an *Auto Save* option. When checked, MEAFS will save the session every 5 seconds in a file named `auto_save.pkl`.  
 Also, if auto save is enabled, when MEAFS is closed, it will save the session in the `auto_save_last.pkl` file.  
 These files are located under the MEAFS directory and the `-h` [flag](<#flags-and-arguments>) will show the location.  
-To load any of these files, simply use the [flags](<#flags-and-arguments>) or load them in the *File* - *Open...* menu
-
-## Uninstall
-
-If you did not install with pip (both directly or by cloning), you can just erase the *meafs* folder.  
-
-Otherwise, first remove the menu entries (if you have added it) and then uninstall:
-
-```bash
-meafs-desktop-remove
-pip uninstall meafs
-```
+To load any of these files, simply use the [flags](<#flags-and-arguments>) or load them in the *File* - *Open...* menu.
 
 <hr/>
```

### Comparing `meafs-4.6.3/meafs.egg-info/PKG-INFO` & `meafs-4.7.12/meafs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: meafs
-Version: 4.6.3
+Version: 4.7.12
 Summary: Multiple Element Abundance Fit Software
 Author: Matheus J. Castro
-Project-URL: Homepage, https://github.com/MatheusJCastro/meafs
+Project-URL: homepage, https://meafs.readthedocs.io/
+Project-URL: repository, https://github.com/MatheusJCastro/meafs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: astropy
@@ -16,42 +17,52 @@
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: desktop_file==1.3
 Requires-Dist: pathlib
 Requires-Dist: PyQt6
 Requires-Dist: dill
+Requires-Dist: qtconsole
 
 ![Meafs Logo](meafs_code/images/Meafs_Logo.png)
 
 # Multiple Element Abundance Fit Software - MEAFS
 
 *Written by: Matheus J. Castro*  
 *Under MIT License*  
 
+More information at: [https://meafs.readthedocs.io/](https://meafs.readthedocs.io/)
+
 <hr/>
 <hr/>
 
 ## Table of Contents
 
-1. [Aims](#Aims)
-2. [Prerequisites](#Prerequisites)
-3. [Instalation](#Instalation)
-    1. [Creating Anaconda Environment (recommended)](<#creating-anaconda-environment-recommended>)
-    2. [Getting the pip version (recommended)](<#getting-the-pip-version-recommended-not-yet-working>)
-    3. [Cloning from GitHub](<#cloning-from-github>)
-    4. [Adding the PATH (for non Anaconda installations)](<#adding-the-path-for-non-anaconda-installations>)
-    5. [Step-by-Step for Windows (Python + GCC)](<#step-by-step-for-windows-python--gcc>)
-    6. [Compilation](<#compilation>)
-4. [Usage](#Usage)
-    1. [With Installation](<#with-installation>)
-    2. [Without Installation](<#without-installation>)
-    3. [Flags and Arguments](<#flags-and-arguments>)
-    4. [Auto Save](<#auto-save>)
-5. [Uninstall](#Uninstall)
+- [Multiple Element Abundance Fit Software - MEAFS](#multiple-element-abundance-fit-software---meafs)
+  - [Table of Contents](#table-of-contents)
+  - [Aims](#aims)
+  - [Prerequisites](#prerequisites)
+    - [Creating Anaconda Environment (recommended)](#creating-anaconda-environment-recommended)
+    - [Step-by-Step for Windows (Python + GCC)](#step-by-step-for-windows-python--gcc)
+      - [Python](#python)
+      - [GCC](#gcc)
+  - [Installation](#installation)
+    - [Getting the pip version (recommended)](#getting-the-pip-version-recommended)
+    - [Cloning from GitHub](#cloning-from-github)
+  - [Post Installation](#post-installation)
+    - [Adding the PATH (for non Anaconda installations)](#adding-the-path-for-non-anaconda-installations)
+      - [Linux](#linux)
+      - [Windows](#windows)
+    - [Compilation](#compilation)
+  - [Uninstall](#uninstall)
+  - [Basic Usage](#basic-usage)
+    - [With Installation](#with-installation)
+    - [Without Installation](#without-installation)
+    - [Flags and Arguments](#flags-and-arguments)
+    - [Auto Save](#auto-save)
 
 ## Aims
 
 The MEAFS is a fitting tool software for spectra abundance analysis. The aims is to provide a medium to high analysis for each individual absorption line in a given spectrum.  
 The software also fits the wavelength shift, continuum and convolution of the spectrum.
 
 ![Meafs GUI](meafs_code/images/Meafs_Gui.png)
@@ -59,36 +70,63 @@
 ## Prerequisites
 
 - Python3 and GCC needs to be previously installed in the system (step-by-step to install for Windows users [bellow](<#step-by-step-for-windows-python--gcc>));
 
 - A software for creating a synthetic spectrum also needs to be previously installed. This version of MEAFS is compatible with the following softwares:
     - Turbospectrum2019: [https://github.com/bertrandplez/Turbospectrum2019](https://github.com/bertrandplez/Turbospectrum2019)
 
-- Optionally: to execute the `unify_plots.py`, a LaTeX installation must be present on the system.
+- Optionally: to execute the *unify_plots.py*, a LaTeX installation must be present on the system.
 
 - Optionally: [Anaconda](<#creating-anaconda-environment-recommended>).
 
-## Instalation
-
-There are many options to run MEAFS. We strongly recommend the use of Anaconda environment, but it is not mandatory.  
-You can install it from pip or run directly the source code from the repository.  
-
-All the methods listed below work in Linux, Windows or MacOS **if you have python and gcc installed** (step-by-step to install for Windows users [bellow](<#step-by-step-for-windows-python--gcc>)).
-
 ### Creating Anaconda Environment (recommended)
 - First, download anaconda [here](https://www.anaconda.com/products/individual#download-section) and execute the script.
 
     - For Linux users, if needed, export anaconda to your path by adding the line `export PATH="/home/USERNAME/anaconda3/bin:$PATH"` (changing the `USERNAME` to your user) to the `~/.bashrc` file. Close and open a new terminal to update the path.
 
     - If desirable, disable autoactivation of anaconda with `conda config --set auto_activate_base false`.
 
 - Create MEAFS enviroment with `conda create python -n meafs`;
 
 - Then, to activate the environment, type `conda activate meafs`;
 
+### Step-by-Step for Windows (Python + GCC)
+
+If you are running Windows **without** Anaconda, you need to install Python and GCC, if you did not already have them. Otherwise, you can skip this.  
+If you are using Windows **with** Anaconda, only GCC is required.
+
+Obs: this step-by-step guide was made using a fresh new install of Windows 10.
+
+#### Python
+
+Go to [Python Windows Releases](https://www.python.org/downloads/windows/) and download an stable release by clicking on it and downloading the *Windows installer (64-bit) Recommended*. After downloading, exectue the files and follow the installation process.
+
+- Add the Python folder to the path.
+    - Open the menu and search for *path*, click in *Edit the system environment variables*, at the bottom right click in *Environment Variables...*, in the tab *System variables* (attention: not the *User variables for Username*), look for the variable *Path* and click on *Edit*. Add two new lines:
+        - `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311`
+        - `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311\Scripts`
+        - Change `USERNAME` with your username and `Python311` to the actual version that you installed.
+- Go to the python folder (ex: `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311`) and create a copy of the `python.exe` file in the same location with the name `python3.11.exe`
+
+#### GCC
+
+Download the *x64* version of [Winlibs](https://winlibs.com).
+    
+- Choose the x64 MCF **with** all the libraries;
+- After downloading, decompress the file and move the `mingw64` folder to `C:\Program Files\`;
+- Now add the folder `bin` of the `mingw64` folder to the path:
+  - Use the sames steps as before but now add the line: `C:\Program Files\mingw64\bin`.
+
+## Installation
+
+There are many options to run MEAFS. We strongly recommend the use of Anaconda environment, but it is not mandatory.  
+You can install it from pip or run directly the source code from the repository.  
+
+All the methods listed below work in Linux, Windows or MacOS **if you have python and gcc installed** (step-by-step to install for Windows users [bellow](<#step-by-step-for-windows-python--gcc>)).
+
 ### Getting the pip version (recommended)
 
 The pip version can easily be acquired by typing in the terminal:
 
 ```bash
 pip install meafs
 ```
@@ -97,29 +135,31 @@
 
 Or you can directly clone from the GitHub page with:
 
 ```bash
 git clone https://github.com/MatheusJCastro/meafs.git
 ```
 
-After cloning, you can install it with pip or run without any installation at all (see the [Usage](<#without-installation>)  section).  
+After cloning, you can install it with pip or run without any installation at all (see the [Usage - Without Installation](<#without-installation>) section).  
 
 To build the package and install it with pip from the source, first install the `build` package:  
 
 ```bash
 pip install build
 ```
 
 Then go to the MEAFS source code directory and type:
 
 ```bash
 python3 -m build
 pip install .
 ```
 
+## Post Installation
+
 ### Adding the PATH (for non Anaconda installations)
 If you do not use Anaconda, you need to add the path of the pip scripts into the system path variable if you have not already done so.  
 **This step is not necessary if you are running without installation.**
 
 #### Linux
 For Linux users, you can add the following line in the end of the file `~/.bashrc`, changing `USER` to your own user.
 
@@ -129,97 +169,94 @@
 
 For some Linux distributions and Python installations, the locale of the executables can slightly change. If this does not work out, you can try differents paths such as `/usr/local/bin` and others.
 
 #### Windows
 
 For Windows users, you need to open the menu and search for *path*, click in *Edit the system environment variables*, at the bottom right click in *Environment Variables...*, in the tab *System variables* (attention: not the *User variables for Username*), look for the variable *Path* and click on *Edit*. Add a new line with one of the followings (check the python location first):
 
-```bash
+```bat
 C:\Users\Windows\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.11_qbz5n2kfra8p0\LocalCache\local-packages\Python311\Scripts
 ```
 
 Or:
 
-```bash
+```bat
 C:\Users\USERNAME\AppData\Local\Programs\Python\Python311\Scripts
 ```
 
 **Be aware of different Python versions, the path will change also. Always verify if the current path exists.**
 
-### Step-by-Step for Windows (Python + GCC)
-Obs: this step-by-step guide was made using a fresh new install of Windows 10.
-
-#### Python
+### Compilation
 
-Go to [Python Windows Releases](https://www.python.org/downloads/windows/) and download an stable release by clicking on it and downloading the *Windows installer (64-bit) Recommended*. After downloading, exectue the files and follow the installation process.
+There is one file written in C Language (`meafs/meafs_code/scripts/bisec_interpol.c`), **in the first run, MEAFS will compile the C library using GCC**. Otherwise, the compilation directives can be found in the `meafs/meafs_code/scripts/comp.sh`. The C file needs to be compiled as a shared library, when using *GCC Compiler*, this can be achieved by adding the `-shared` flag.
 
-- Add the Python folder to the path.
-    - Open the menu and search for *path*, click in *Edit the system environment variables*, at the bottom right click in *Environment Variables...*, in the tab *System variables* (attention: not the *User variables for Username*), look for the variable *Path* and click on *Edit*. Add two new lines:
-        - `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311`
-        - `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311\Scripts`
-        - Change `USERNAME` with your username and `Python311` to the actual version that you installed.
-- Go to the python folder (ex: `C:\Users\USERNAME\AppData\Local\Programs\Python\Python311`) and create a copy of the `python.exe` file in the same location with the name `python3.11.exe`
+If the auto compilation fails, for Linux users, just add execution privileges at the `comp.sh` file and execute it in a terminal to create the binary. For that, open a terminal in the `meafs/meafs_code/scripts/` folder and type:
 
-#### GCC
+```bash
+chmod +x comp.sh
+./comp.sh
+```
 
-Download the *x64* version of [Winlibs](https://winlibs.com).
-    
-- Choose the x64 MCF **with** all the libraries;
-- After downloading, decompress the file and move the `mingw64` folder to `C:\Program Files\`;
-- Now add the folder `bin` of the `mingw64` folder to the path:
-        - Use the sames steps as before but now add the line: `C:\Program Files\mingw64\bin`.
+If you are on Windows, check this `comp.sh` file for the full `gcc` command.
 
-### Compilation
+## Uninstall
 
-There is one file written in C Language (`meafs/meafs_code/scripts/bisec_interpol.c`), the compilation directives can be found in the `meafs/meafs_code/scripts/comp.sh`. The C file needs to be compiled as a shared library, when using *GCC Compiler*, this can be achieved by adding the `-shared` flag.
+If you did not install with pip (both directly or by cloning), you can just erase the *meafs* folder.  
 
-For Linux users just add execution privileges at the `comp.sh` file and execute it in a terminal to create the binary. For that, open a terminal in the `meafs/meafs_code/scripts/` folder and type:
+Otherwise, first remove the menu entries (if you have added it, see [Usage - With Installation](<#with-installation>)) and then uninstall:
 
 ```bash
-chmod +x comp.sh
-./comp.sh
+meafs-desktop-remove
+pip uninstall meafs
 ```
 
-## Usage
+## Basic Usage
 
 ### With Installation
 You can create menu entries for MEAFS by typing in the terminal or cmd:  
 
 ```bash
 meafs-desktop-create
 ```
 
 Then, search in the menu for *MEAFS*, and in Windows, a Desktop link will also be created.  
-But, if you do not want to create menu entries, just type `meafs` or `python -m meafs` in the terminal or cmd to launch it.
+Or, you can just type in the terminal or cmd: 
+
+```bash
+meafs
+```
+
+Or:
+
+```bash
+python -m meafs
+```
+
+For the command line option, do not forget to activate the Anaconda environment if you are using it. For the menu entry, this is done automatically if necessary.
 
 ### Without Installation
-Simply execute the file `gui.py` and it will power the GUI.
+Simply execute the file `meafs_code/gui.py` and it will power the GUI.
 
 ### Flags and Arguments
 
 There are some flags that can be passed with the command-line.
 
-- `-h` or `--help`: Show the help section;
-- `-v` or `--version`: Show version number;
-- `-l` or `--last`: Load the last closed session. Default location is `meafs_code/auto_save_last.pkl`
-- `-s` or `--load-auto-save`: Load the auto saved session. Default location is: `meafs_code/auto_save.pkl`
+- `-h`, `--help`: Show the help section;
+- `-v`, `--version`: Show version number;
+- `-l`, `--last`: Load the last closed session. Default location is `meafs_code/auto_save_last.pkl`;
+- `-s`, `--load-auto-save`: Load the auto saved session. Default location is: `meafs_code/auto_save.pkl`.
 
-Also, any saved section can be passed as an argument. It will power the GUI with it. If no argument is given, the GUI will power with a new empty session.
+Also, any saved section can be passed as an argument and meafs will power the GUI with it:
+
+```bash
+meafs path/to/session.pkl
+```
+
+If no argument is given, the GUI will power with a new empty session.
 
 ### Auto Save
 In the *File* menu there is an *Auto Save* option. When checked, MEAFS will save the session every 5 seconds in a file named `auto_save.pkl`.  
 Also, if auto save is enabled, when MEAFS is closed, it will save the session in the `auto_save_last.pkl` file.  
 These files are located under the MEAFS directory and the `-h` [flag](<#flags-and-arguments>) will show the location.  
-To load any of these files, simply use the [flags](<#flags-and-arguments>) or load them in the *File* - *Open...* menu
-
-## Uninstall
-
-If you did not install with pip (both directly or by cloning), you can just erase the *meafs* folder.  
-
-Otherwise, first remove the menu entries (if you have added it) and then uninstall:
-
-```bash
-meafs-desktop-remove
-pip uninstall meafs
-```
+To load any of these files, simply use the [flags](<#flags-and-arguments>) or load them in the *File* - *Open...* menu.
 
 <hr/>
```

### Comparing `meafs-4.6.3/meafs.egg-info/SOURCES.txt` & `meafs-4.7.12/meafs.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -21,13 +21,12 @@
 meafs_code/images/Meafs_Gui.png
 meafs_code/images/Meafs_Icon.ico
 meafs_code/images/Meafs_Logo.png
 meafs_code/scripts/__init__.py
 meafs_code/scripts/abundance_analysis.py
 meafs_code/scripts/abundance_fit.py
 meafs_code/scripts/bisec_interpol.c
-meafs_code/scripts/bisec_interpol.so
 meafs_code/scripts/comp.sh
 meafs_code/scripts/fit_functions.py
 meafs_code/scripts/turbospec_functions.py
 meafs_code/scripts/unify_plots.py
 meafs_code/scripts/voigt_functions.py
```

### Comparing `meafs-4.6.3/meafs_code/desktop_entry.py` & `meafs-4.7.12/meafs_code/desktop_entry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-#####################################################
-# MEAFS Desktop Entry Creation                      #
-# Matheus J. Castro                                 #
-# v1.2                                              #
-# Last Modification: 04/12/2024                     #
-# Contact: matheusdejesuscastro@gmail.com           #
-#####################################################
+"""
+| MEAFS Desktop Entry Creation
+| Matheus J. Castro
+| v1.3
+
+| This file analyse and create aliases in the system to run MEAFS through an entry in the system menu.
+"""
 
 import desktop_file as df
 from pathlib import Path
 import sys
 import os
 
 
 def get_curr_dir():
+
+    """
+    Get the current environment running python (like anaconda or system)
+    and the directory where the file is located.
+
+    :return: the command that activates anaconda environment (if present) and the file absolute path.
+    """
+
+
     def anaconda_error():
         sys.exit("Error: anaconda environment detected but path not found.")
 
     pre = sys.prefix
     if "anaconda" in pre:
         print("Anaconda detected.")
 
@@ -47,14 +56,16 @@
     path = Path(__file__).parts[:-1]
     path = Path(path[0]).joinpath(*path[1:])
 
     return conda_activate, str(path)
 
 
 def create():
+    """Create the menu entry in the system to run MEAFS."""
+
     def module_create(path):
         print("Creating shortcut at: ", path)
         shortcut = df.Shortcut(path, "MEAFS", "{}python{} -m meafs_code".format(conda, vers))
         shortcut.setTitle("MEAFS")
         shortcut.setWorkingDirectory(dir)
         shortcut.setComment("Multiple Element Abundance Fit Software")
         shortcut.setIcon(icon_path)
@@ -65,15 +76,15 @@
     icon_path = str(Path(dir).joinpath("images", "Meafs_Icon.ico"))
 
     # Get the actual Python version
     vers = str(sys.version_info.major) + "." + str(sys.version_info.minor)
 
     if "linux" in sys.platform:
         module_create(df.getMenuPath())
-    elif "win" in sys.platform:
+    elif "win" in sys.platform and "darwin" not in sys.platform:
         import win32com.client
 
         fls = os.listdir(dir)
         for fl in fls:
             if "MEAFS" in fl and ".bat" in fl:
                 os.remove(str(Path(dir).joinpath(fl)))
 
@@ -99,14 +110,16 @@
         print("Creating shortcut at: ", df.getMenuPath())
         os.system("copy {} \"{}\"".format(src, df.getMenuPath()))
 
     print("No errors reported. Logout and login again for changes to take effect.")
 
 
 def remove():
+    """Remove the menu entry in the system that run MEAFS."""
+
     def erasing(path_fl, fl):
         path_fl = str(Path(path_fl).joinpath(fl))
         print("Removing file: ", path_fl)
 
         try:
             os.remove(path_fl)
             print("Done.")
```

### Comparing `meafs-4.6.3/meafs_code/fitsettings.ui` & `meafs-4.7.12/meafs_code/fitsettings.ui`

 * *Files identical despite different names*

### Comparing `meafs-4.6.3/meafs_code/fitsettings_qt.py` & `meafs-4.7.12/meafs_code/fitsettings_qt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Form implementation generated from reading ui file 'fitsettings.ui'
 #
-# Created by: PyQt6 UI code generator 6.6.1
+# Created by: PyQt6 UI code generator 6.7.0
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
```

### Comparing `meafs-4.6.3/meafs_code/gui_qt.py` & `meafs-4.7.12/meafs_code/gui_qt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,75 @@
 # Form implementation generated from reading ui file 'meafs.ui'
 #
-# Created by: PyQt6 UI code generator 6.6.1
+# Created by: PyQt6 UI code generator 6.7.0
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_MEAFS(object):
     def setupUi(self, MEAFS):
         MEAFS.setObjectName("MEAFS")
-        MEAFS.resize(1203, 781)
+        MEAFS.resize(1203, 739)
         self.centralwidget = QtWidgets.QWidget(parent=MEAFS)
         self.centralwidget.setObjectName("centralwidget")
         self.gridLayout = QtWidgets.QGridLayout(self.centralwidget)
         self.gridLayout.setObjectName("gridLayout")
-        self.results = QtWidgets.QGridLayout()
-        self.results.setObjectName("results")
-        self.label = QtWidgets.QLabel(parent=self.centralwidget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Fixed)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.label.sizePolicy().hasHeightForWidth())
-        self.label.setSizePolicy(sizePolicy)
+        self.refer = QtWidgets.QGridLayout()
+        self.refer.setObjectName("refer")
+        self.refername = QtWidgets.QLineEdit(parent=self.centralwidget)
+        self.refername.setObjectName("refername")
+        self.refer.addWidget(self.refername, 1, 1, 1, 1)
+        self.referlabel = QtWidgets.QLabel(parent=self.centralwidget)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
-        self.label.setFont(font)
-        self.label.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
-        self.label.setObjectName("label")
-        self.results.addWidget(self.label, 0, 0, 1, 1)
-        self.plot = QtWidgets.QGridLayout()
-        self.plot.setSizeConstraint(QtWidgets.QLayout.SizeConstraint.SetFixedSize)
-        self.plot.setObjectName("plot")
-        self.results.addLayout(self.plot, 1, 0, 1, 1)
-        self.gridLayout.addLayout(self.results, 3, 1, 2, 3)
+        self.referlabel.setFont(font)
+        self.referlabel.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.referlabel.setObjectName("referlabel")
+        self.refer.addWidget(self.referlabel, 0, 0, 1, 4)
+        self.referlabel2 = QtWidgets.QLabel(parent=self.centralwidget)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.referlabel2.setFont(font)
+        self.referlabel2.setObjectName("referlabel2")
+        self.refer.addWidget(self.referlabel2, 1, 0, 1, 1)
+        self.verticalLayout_3 = QtWidgets.QVBoxLayout()
+        self.verticalLayout_3.setObjectName("verticalLayout_3")
+        self.referaddline = QtWidgets.QPushButton(parent=self.centralwidget)
+        self.referaddline.setObjectName("referaddline")
+        self.verticalLayout_3.addWidget(self.referaddline)
+        self.referremoveline = QtWidgets.QPushButton(parent=self.centralwidget)
+        self.referremoveline.setObjectName("referremoveline")
+        self.verticalLayout_3.addWidget(self.referremoveline)
+        self.refer.addLayout(self.verticalLayout_3, 2, 3, 1, 1)
+        self.referbrowse = QtWidgets.QPushButton(parent=self.centralwidget)
+        self.referbrowse.setObjectName("referbrowse")
+        self.refer.addWidget(self.referbrowse, 1, 2, 1, 1)
+        self.referload = QtWidgets.QPushButton(parent=self.centralwidget)
+        self.referload.setObjectName("referload")
+        self.refer.addWidget(self.referload, 1, 3, 1, 1)
+        self.refercontent = QtWidgets.QTableWidget(parent=self.centralwidget)
+        self.refercontent.setObjectName("refercontent")
+        self.refercontent.setColumnCount(2)
+        self.refercontent.setRowCount(0)
+        item = QtWidgets.QTableWidgetItem()
+        self.refercontent.setHorizontalHeaderItem(0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.refercontent.setHorizontalHeaderItem(1, item)
+        self.refercontent.horizontalHeader().setVisible(True)
+        self.refercontent.horizontalHeader().setCascadingSectionResizes(False)
+        self.refercontent.horizontalHeader().setSortIndicatorShown(False)
+        self.refercontent.horizontalHeader().setStretchLastSection(True)
+        self.refer.addWidget(self.refercontent, 2, 0, 1, 3)
+        self.gridLayout.addLayout(self.refer, 4, 3, 1, 1)
         self.outputabundances = QtWidgets.QGridLayout()
         self.outputabundances.setObjectName("outputabundances")
         self.outputbrowse = QtWidgets.QPushButton(parent=self.centralwidget)
         self.outputbrowse.setObjectName("outputbrowse")
         self.outputabundances.addWidget(self.outputbrowse, 3, 4, 1, 1)
         self.outputname = QtWidgets.QLineEdit(parent=self.centralwidget)
         self.outputname.setObjectName("outputname")
@@ -109,15 +138,15 @@
         self.outputlabel.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.outputlabel.setFont(font)
         self.outputlabel.setObjectName("outputlabel")
         self.outputabundances.addWidget(self.outputlabel, 3, 1, 1, 2)
-        self.gridLayout.addLayout(self.outputabundances, 5, 1, 1, 1)
+        self.gridLayout.addLayout(self.outputabundances, 4, 1, 1, 1)
         self.linelist = QtWidgets.QGridLayout()
         self.linelist.setObjectName("linelist")
         self.linelistlabel = QtWidgets.QLabel(parent=self.centralwidget)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.linelistlabel.setFont(font)
@@ -183,15 +212,15 @@
         self.linelistcontent.setHorizontalHeaderItem(0, item)
         item = QtWidgets.QTableWidgetItem()
         self.linelistcontent.setHorizontalHeaderItem(1, item)
         item = QtWidgets.QTableWidgetItem()
         self.linelistcontent.setHorizontalHeaderItem(2, item)
         self.linelistcontent.horizontalHeader().setStretchLastSection(True)
         self.linelist.addWidget(self.linelistcontent, 3, 0, 1, 4)
-        self.gridLayout.addLayout(self.linelist, 3, 4, 1, 1)
+        self.gridLayout.addLayout(self.linelist, 3, 3, 1, 1)
         self.methodsdatafittab = QtWidgets.QTabWidget(parent=self.centralwidget)
         self.methodsdatafittab.setObjectName("methodsdatafittab")
         self.datatab = QtWidgets.QWidget()
         self.datatab.setObjectName("datatab")
         self.gridLayout_11 = QtWidgets.QGridLayout(self.datatab)
         self.gridLayout_11.setObjectName("gridLayout_11")
         self.gridLayout_10 = QtWidgets.QGridLayout()
@@ -484,64 +513,45 @@
         self.horizontalLayout.addWidget(self.currentvaluesplotbutton)
         self.currentvaluessavebutton = QtWidgets.QPushButton(parent=self.fitparameterstab)
         self.currentvaluessavebutton.setObjectName("currentvaluessavebutton")
         self.horizontalLayout.addWidget(self.currentvaluessavebutton)
         self.fitparameters.addLayout(self.horizontalLayout, 7, 0, 1, 3)
         self.gridLayout_13.addLayout(self.fitparameters, 0, 0, 1, 1)
         self.methodsdatafittab.addTab(self.fitparameterstab, "")
-        self.gridLayout.addWidget(self.methodsdatafittab, 5, 2, 1, 1)
-        self.refer = QtWidgets.QGridLayout()
-        self.refer.setObjectName("refer")
-        self.refername = QtWidgets.QLineEdit(parent=self.centralwidget)
-        self.refername.setObjectName("refername")
-        self.refer.addWidget(self.refername, 1, 1, 1, 1)
-        self.referlabel = QtWidgets.QLabel(parent=self.centralwidget)
-        font = QtGui.QFont()
-        font.setBold(True)
-        font.setWeight(75)
-        self.referlabel.setFont(font)
-        self.referlabel.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
-        self.referlabel.setObjectName("referlabel")
-        self.refer.addWidget(self.referlabel, 0, 0, 1, 4)
-        self.referlabel2 = QtWidgets.QLabel(parent=self.centralwidget)
-        font = QtGui.QFont()
-        font.setBold(True)
-        font.setWeight(75)
-        self.referlabel2.setFont(font)
-        self.referlabel2.setObjectName("referlabel2")
-        self.refer.addWidget(self.referlabel2, 1, 0, 1, 1)
-        self.verticalLayout_3 = QtWidgets.QVBoxLayout()
-        self.verticalLayout_3.setObjectName("verticalLayout_3")
-        self.referaddline = QtWidgets.QPushButton(parent=self.centralwidget)
-        self.referaddline.setObjectName("referaddline")
-        self.verticalLayout_3.addWidget(self.referaddline)
-        self.referremoveline = QtWidgets.QPushButton(parent=self.centralwidget)
-        self.referremoveline.setObjectName("referremoveline")
-        self.verticalLayout_3.addWidget(self.referremoveline)
-        self.refer.addLayout(self.verticalLayout_3, 2, 3, 1, 1)
-        self.referbrowse = QtWidgets.QPushButton(parent=self.centralwidget)
-        self.referbrowse.setObjectName("referbrowse")
-        self.refer.addWidget(self.referbrowse, 1, 2, 1, 1)
-        self.referload = QtWidgets.QPushButton(parent=self.centralwidget)
-        self.referload.setObjectName("referload")
-        self.refer.addWidget(self.referload, 1, 3, 1, 1)
-        self.refercontent = QtWidgets.QTableWidget(parent=self.centralwidget)
-        self.refercontent.setObjectName("refercontent")
-        self.refercontent.setColumnCount(2)
-        self.refercontent.setRowCount(0)
-        item = QtWidgets.QTableWidgetItem()
-        self.refercontent.setHorizontalHeaderItem(0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.refercontent.setHorizontalHeaderItem(1, item)
-        self.refercontent.horizontalHeader().setVisible(True)
-        self.refercontent.horizontalHeader().setCascadingSectionResizes(False)
-        self.refercontent.horizontalHeader().setSortIndicatorShown(False)
-        self.refercontent.horizontalHeader().setStretchLastSection(True)
-        self.refer.addWidget(self.refercontent, 2, 0, 1, 3)
-        self.gridLayout.addLayout(self.refer, 5, 4, 1, 1)
+        self.gridLayout.addWidget(self.methodsdatafittab, 4, 2, 1, 1)
+        self.tabplotshels = QtWidgets.QTabWidget(parent=self.centralwidget)
+        self.tabplotshels.setObjectName("tabplotshels")
+        self.tabplot = QtWidgets.QWidget()
+        self.tabplot.setObjectName("tabplot")
+        self.horizontalLayout_4 = QtWidgets.QHBoxLayout(self.tabplot)
+        self.horizontalLayout_4.setObjectName("horizontalLayout_4")
+        self.plot = QtWidgets.QHBoxLayout()
+        self.plot.setObjectName("plot")
+        self.horizontalLayout_4.addLayout(self.plot)
+        self.tabplotshels.addTab(self.tabplot, "")
+        self.tabjupyshell = QtWidgets.QWidget()
+        self.tabjupyshell.setObjectName("tabjupyshell")
+        self.gridLayout_16 = QtWidgets.QGridLayout(self.tabjupyshell)
+        self.gridLayout_16.setObjectName("gridLayout_16")
+        self.layoutjupyshell = QtWidgets.QGridLayout()
+        self.layoutjupyshell.setObjectName("layoutjupyshell")
+        self.gridLayout_16.addLayout(self.layoutjupyshell, 0, 0, 1, 1)
+        self.tabplotshels.addTab(self.tabjupyshell, "")
+        self.tabstoutstderr = QtWidgets.QWidget()
+        self.tabstoutstderr.setObjectName("tabstoutstderr")
+        self.gridLayout_12 = QtWidgets.QGridLayout(self.tabstoutstderr)
+        self.gridLayout_12.setObjectName("gridLayout_12")
+        self.clearstdbutton = QtWidgets.QToolButton(parent=self.tabstoutstderr)
+        self.clearstdbutton.setObjectName("clearstdbutton")
+        self.gridLayout_12.addWidget(self.clearstdbutton, 2, 1, 1, 1)
+        self.stdtext = QtWidgets.QTextEdit(parent=self.tabstoutstderr)
+        self.stdtext.setObjectName("stdtext")
+        self.gridLayout_12.addWidget(self.stdtext, 1, 0, 1, 2)
+        self.tabplotshels.addTab(self.tabstoutstderr, "")
+        self.gridLayout.addWidget(self.tabplotshels, 3, 1, 1, 2)
         MEAFS.setCentralWidget(self.centralwidget)
         self.menubar = QtWidgets.QMenuBar(parent=MEAFS)
         self.menubar.setGeometry(QtCore.QRect(0, 0, 1203, 30))
         self.menubar.setObjectName("menubar")
         self.menuFile = QtWidgets.QMenu(parent=self.menubar)
         self.menuFile.setObjectName("menuFile")
         self.menuView = QtWidgets.QMenu(parent=self.menubar)
@@ -598,20 +608,30 @@
         self.menubar.addAction(self.menuFile.menuAction())
         self.menubar.addAction(self.menuEdit.menuAction())
         self.menubar.addAction(self.menuView.menuAction())
 
         self.retranslateUi(MEAFS)
         self.methodsdatafittab.setCurrentIndex(1)
         self.methodstab.setCurrentIndex(0)
+        self.tabplotshels.setCurrentIndex(2)
         QtCore.QMetaObject.connectSlotsByName(MEAFS)
 
     def retranslateUi(self, MEAFS):
         _translate = QtCore.QCoreApplication.translate
         MEAFS.setWindowTitle(_translate("MEAFS", "MEAFS"))
-        self.label.setText(_translate("MEAFS", "Spectrum Plot"))
+        self.referlabel.setText(_translate("MEAFS", "Abundance Reference"))
+        self.referlabel2.setText(_translate("MEAFS", "Abund. Ref. Location:"))
+        self.referaddline.setText(_translate("MEAFS", "Add Line"))
+        self.referremoveline.setText(_translate("MEAFS", "Remove Line"))
+        self.referbrowse.setText(_translate("MEAFS", "Browse"))
+        self.referload.setText(_translate("MEAFS", "Load"))
+        item = self.refercontent.horizontalHeaderItem(0)
+        item.setText(_translate("MEAFS", "Element"))
+        item = self.refercontent.horizontalHeaderItem(1)
+        item.setText(_translate("MEAFS", "Abundance"))
         self.outputbrowse.setText(_translate("MEAFS", "Browse"))
         self.abundanceslabel.setText(_translate("MEAFS", "Abundances"))
         item = self.abundancetable.horizontalHeaderItem(0)
         item.setText(_translate("MEAFS", "Element"))
         item = self.abundancetable.horizontalHeaderItem(1)
         item.setText(_translate("MEAFS", "Wavelength"))
         self.stop.setText(_translate("MEAFS", "Stop"))
@@ -669,24 +689,18 @@
         self.manualfitbutton.setText(_translate("MEAFS", "Manual Fit"))
         self.lambshiflabel.setText(_translate("MEAFS", "Lamb Shift"))
         self.convolutionlabel.setText(_translate("MEAFS", "Convolution"))
         self.abundancelabel.setText(_translate("MEAFS", "Abundance"))
         self.currentvaluesplotbutton.setText(_translate("MEAFS", "Plot Current Values"))
         self.currentvaluessavebutton.setText(_translate("MEAFS", "Save Current Values"))
         self.methodsdatafittab.setTabText(self.methodsdatafittab.indexOf(self.fitparameterstab), _translate("MEAFS", "Fit Parameters"))
-        self.referlabel.setText(_translate("MEAFS", "Abundance Reference"))
-        self.referlabel2.setText(_translate("MEAFS", "Abund. Ref. Location:"))
-        self.referaddline.setText(_translate("MEAFS", "Add Line"))
-        self.referremoveline.setText(_translate("MEAFS", "Remove Line"))
-        self.referbrowse.setText(_translate("MEAFS", "Browse"))
-        self.referload.setText(_translate("MEAFS", "Load"))
-        item = self.refercontent.horizontalHeaderItem(0)
-        item.setText(_translate("MEAFS", "Element"))
-        item = self.refercontent.horizontalHeaderItem(1)
-        item.setText(_translate("MEAFS", "Abundance"))
+        self.tabplotshels.setTabText(self.tabplotshels.indexOf(self.tabplot), _translate("MEAFS", "Spectrum Plot"))
+        self.tabplotshels.setTabText(self.tabplotshels.indexOf(self.tabjupyshell), _translate("MEAFS", "Jupyter Shell"))
+        self.clearstdbutton.setText(_translate("MEAFS", "Clear"))
+        self.tabplotshels.setTabText(self.tabplotshels.indexOf(self.tabstoutstderr), _translate("MEAFS", "Stdout"))
         self.menuFile.setTitle(_translate("MEAFS", "File"))
         self.menuView.setTitle(_translate("MEAFS", "View"))
         self.menuEdit.setTitle(_translate("MEAFS", "Edit"))
         self.actionOpen.setText(_translate("MEAFS", "Open"))
         self.actionSave.setText(_translate("MEAFS", "Save"))
         self.open.setText(_translate("MEAFS", "Open..."))
         self.save.setText(_translate("MEAFS", "Save"))
```

### Comparing `meafs-4.6.3/meafs_code/images/Meafs_Gui.png` & `meafs-4.7.12/meafs_code/images/Meafs_Gui.png`

 * *Files identical despite different names*

### Comparing `meafs-4.6.3/meafs_code/images/Meafs_Icon.ico` & `meafs-4.7.12/meafs_code/images/Meafs_Icon.ico`

 * *Files identical despite different names*

### Comparing `meafs-4.6.3/meafs_code/images/Meafs_Logo.png` & `meafs-4.7.12/meafs_code/images/Meafs_Logo.png`

 * *Files identical despite different names*

### Comparing `meafs-4.6.3/meafs_code/meafs.ui` & `meafs-4.7.12/meafs_code/meafs.ui`

 * *Files 2% similar despite different names*

#### Comparing `meafs-4.6.3/meafs_code/meafs.ui` & `meafs-4.7.12/meafs_code/meafs.ui`

```diff
@@ -3,56 +3,117 @@
   <class>MEAFS</class>
   <widget class="QMainWindow" name="MEAFS">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>1203</width>
-        <height>781</height>
+        <height>739</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>MEAFS</string>
     </property>
     <widget class="QWidget" name="centralwidget">
       <layout class="QGridLayout" name="gridLayout">
-        <item row="3" column="1" rowspan="2" colspan="3">
-          <layout class="QGridLayout" name="results">
-            <item row="0" column="0">
-              <widget class="QLabel" name="label">
-                <property name="sizePolicy">
-                  <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
-                    <horstretch>0</horstretch>
-                    <verstretch>0</verstretch>
-                  </sizepolicy>
-                </property>
+        <item row="4" column="3">
+          <layout class="QGridLayout" name="refer">
+            <item row="1" column="1">
+              <widget class="QLineEdit" name="refername"/>
+            </item>
+            <item row="0" column="0" colspan="4">
+              <widget class="QLabel" name="referlabel">
                 <property name="font">
                   <font>
                     <weight>75</weight>
                     <bold>true</bold>
                   </font>
                 </property>
                 <property name="text">
-                  <string>Spectrum Plot</string>
+                  <string>Abundance Reference</string>
                 </property>
                 <property name="alignment">
                   <set>Qt::AlignCenter</set>
                 </property>
               </widget>
             </item>
             <item row="1" column="0">
-              <layout class="QGridLayout" name="plot">
-                <property name="sizeConstraint">
-                  <enum>QLayout::SetFixedSize</enum>
+              <widget class="QLabel" name="referlabel2">
+                <property name="font">
+                  <font>
+                    <weight>75</weight>
+                    <bold>true</bold>
+                  </font>
                 </property>
+                <property name="text">
+                  <string>Abund. Ref. Location:</string>
+                </property>
+              </widget>
+            </item>
+            <item row="2" column="3">
+              <layout class="QVBoxLayout" name="verticalLayout_3">
+                <item>
+                  <widget class="QPushButton" name="referaddline">
+                    <property name="text">
+                      <string>Add Line</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QPushButton" name="referremoveline">
+                    <property name="text">
+                      <string>Remove Line</string>
+                    </property>
+                  </widget>
+                </item>
               </layout>
             </item>
+            <item row="1" column="2">
+              <widget class="QPushButton" name="referbrowse">
+                <property name="text">
+                  <string>Browse</string>
+                </property>
+              </widget>
+            </item>
+            <item row="1" column="3">
+              <widget class="QPushButton" name="referload">
+                <property name="text">
+                  <string>Load</string>
+                </property>
+              </widget>
+            </item>
+            <item row="2" column="0" colspan="3">
+              <widget class="QTableWidget" name="refercontent">
+                <attribute name="horizontalHeaderVisible">
+                  <bool>true</bool>
+                </attribute>
+                <attribute name="horizontalHeaderCascadingSectionResizes">
+                  <bool>false</bool>
+                </attribute>
+                <attribute name="horizontalHeaderShowSortIndicator" stdset="0">
+                  <bool>false</bool>
+                </attribute>
+                <attribute name="horizontalHeaderStretchLastSection">
+                  <bool>true</bool>
+                </attribute>
+                <column>
+                  <property name="text">
+                    <string>Element</string>
+                  </property>
+                </column>
+                <column>
+                  <property name="text">
+                    <string>Abundance</string>
+                  </property>
+                </column>
+              </widget>
+            </item>
           </layout>
         </item>
-        <item row="5" column="1">
+        <item row="4" column="1">
           <layout class="QGridLayout" name="outputabundances">
             <item row="3" column="4">
               <widget class="QPushButton" name="outputbrowse">
                 <property name="text">
                   <string>Browse</string>
                 </property>
               </widget>
@@ -173,15 +234,15 @@
                 <property name="text">
                   <string>Output Location:</string>
                 </property>
               </widget>
             </item>
           </layout>
         </item>
-        <item row="3" column="4">
+        <item row="3" column="3">
           <layout class="QGridLayout" name="linelist">
             <item row="0" column="0" colspan="5">
               <widget class="QLabel" name="linelistlabel">
                 <property name="font">
                   <font>
                     <weight>75</weight>
                     <bold>true</bold>
@@ -323,15 +384,15 @@
                     <string>Analyze</string>
                   </property>
                 </column>
               </widget>
             </item>
           </layout>
         </item>
-        <item row="5" column="2">
+        <item row="4" column="2">
           <widget class="QTabWidget" name="methodsdatafittab">
             <property name="currentIndex">
               <number>1</number>
             </property>
             <widget class="QWidget" name="datatab">
               <attribute name="title">
                 <string>Data</string>
@@ -894,107 +955,57 @@
                     </item>
                   </layout>
                 </item>
               </layout>
             </widget>
           </widget>
         </item>
-        <item row="5" column="4">
-          <layout class="QGridLayout" name="refer">
-            <item row="1" column="1">
-              <widget class="QLineEdit" name="refername"/>
-            </item>
-            <item row="0" column="0" colspan="4">
-              <widget class="QLabel" name="referlabel">
-                <property name="font">
-                  <font>
-                    <weight>75</weight>
-                    <bold>true</bold>
-                  </font>
-                </property>
-                <property name="text">
-                  <string>Abundance Reference</string>
-                </property>
-                <property name="alignment">
-                  <set>Qt::AlignCenter</set>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="0">
-              <widget class="QLabel" name="referlabel2">
-                <property name="font">
-                  <font>
-                    <weight>75</weight>
-                    <bold>true</bold>
-                  </font>
-                </property>
-                <property name="text">
-                  <string>Abund. Ref. Location:</string>
-                </property>
-              </widget>
-            </item>
-            <item row="2" column="3">
-              <layout class="QVBoxLayout" name="verticalLayout_3">
+        <item row="3" column="1" colspan="2">
+          <widget class="QTabWidget" name="tabplotshels">
+            <property name="currentIndex">
+              <number>2</number>
+            </property>
+            <widget class="QWidget" name="tabplot">
+              <attribute name="title">
+                <string>Spectrum Plot</string>
+              </attribute>
+              <layout class="QHBoxLayout" name="horizontalLayout_4">
                 <item>
-                  <widget class="QPushButton" name="referaddline">
-                    <property name="text">
-                      <string>Add Line</string>
-                    </property>
-                  </widget>
+                  <layout class="QHBoxLayout" name="plot"/>
                 </item>
-                <item>
-                  <widget class="QPushButton" name="referremoveline">
+              </layout>
+            </widget>
+            <widget class="QWidget" name="tabjupyshell">
+              <attribute name="title">
+                <string>Jupyter Shell</string>
+              </attribute>
+              <layout class="QGridLayout" name="gridLayout_16">
+                <item row="0" column="0">
+                  <layout class="QGridLayout" name="layoutjupyshell"/>
+                </item>
+              </layout>
+            </widget>
+            <widget class="QWidget" name="tabstoutstderr">
+              <attribute name="title">
+                <string>Stdout</string>
+              </attribute>
+              <layout class="QGridLayout" name="gridLayout_12">
+                <item row="2" column="1">
+                  <widget class="QToolButton" name="clearstdbutton">
                     <property name="text">
-                      <string>Remove Line</string>
+                      <string>Clear</string>
                     </property>
                   </widget>
                 </item>
+                <item row="1" column="0" colspan="2">
+                  <widget class="QTextEdit" name="stdtext"/>
+                </item>
               </layout>
-            </item>
-            <item row="1" column="2">
-              <widget class="QPushButton" name="referbrowse">
-                <property name="text">
-                  <string>Browse</string>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="3">
-              <widget class="QPushButton" name="referload">
-                <property name="text">
-                  <string>Load</string>
-                </property>
-              </widget>
-            </item>
-            <item row="2" column="0" colspan="3">
-              <widget class="QTableWidget" name="refercontent">
-                <attribute name="horizontalHeaderVisible">
-                  <bool>true</bool>
-                </attribute>
-                <attribute name="horizontalHeaderCascadingSectionResizes">
-                  <bool>false</bool>
-                </attribute>
-                <attribute name="horizontalHeaderShowSortIndicator" stdset="0">
-                  <bool>false</bool>
-                </attribute>
-                <attribute name="horizontalHeaderStretchLastSection">
-                  <bool>true</bool>
-                </attribute>
-                <column>
-                  <property name="text">
-                    <string>Element</string>
-                  </property>
-                </column>
-                <column>
-                  <property name="text">
-                    <string>Abundance</string>
-                  </property>
-                </column>
-              </widget>
-            </item>
-          </layout>
+            </widget>
+          </widget>
         </item>
       </layout>
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
```

### Comparing `meafs-4.6.3/meafs_code/scripts/abundance_analysis.py` & `meafs-4.7.12/meafs_code/scripts/abundance_analysis.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 #!/usr/bin/env python3
-
-#####################################################
-# Abundance Analysis                                #
-# Matheus J. Castro                                 #
-# v3.0                                              #
-# Last Modification: 07/01/2022                     #
-# Contact: matheusdejesuscastro@gmail.com           #
-#####################################################
-
-# This program generates graphics to analyse the results obtained with the abundance_fit.py
-
-# For this code work, it must be in the same folder as the abundance_fit.py file
+"""
+| MEAFS Abundance Analysis
+| Matheus J. Castro
+| v3.0
+
+| This program generates graphics to analyse the results obtained with the abundance_fit.py
+| For this code work, it must be in the same folder as the *abundance_fit.py* file
+"""
 
 import matplotlib.pyplot as plt
 from scipy.stats import norm
 import pandas as pd
 import numpy as np
 import sys
 import os
@@ -23,33 +19,52 @@
 try:
     import abundance_fit as ab_fit
 except ModuleNotFoundError:
     from . import abundance_fit as ab_fit
 
 
 def erase_emission_order(abund):
-    # Function to erase the emission order in the database
+    """
+    Erase the emission order in the database.
+
+    :param abund: pandas element with the abundances for each line.
+    :return: the abundance dataframe without the emission orders.
+    """
+
     new_elem = []
     for i in range(len(abund)):
         new_elem.append(abund.Element.iloc[i][:-1])
 
     abund.Element = new_elem
 
     return abund
 
 
 def erase_null_abund(abund):
-    # Function to erase the empty slots in the database
+    """
+    Erase the empty slots in the database.
+
+    :param abund: pandas element with the abundances.
+    :return: the abundance dataframe without the null elements.
+    """
+
     abund = abund[abund["Fit Abundance"].notnull()]
     return abund
 
 
 def plot_abund_hist(abund, elements, folder):
-    # Plot histograms for abundance for each element
-    # and trace a gaussian with the mean and standard deviation
+    """
+    Creeate histograms for abundance for each element
+    and trace a gaussian with the mean and standard deviation.
+
+    :param abund: pandas element with the abundances.
+    :param elements: elements to create histograms.
+    :param folder: directory to be saved.
+    """
+
     for i in elements:
         elem_abunds = abund["Fit Abundance"][abund.Element == i]
 
         plt.figure(figsize=(16, 9))
 
         plt.title("Found Abundances for Element {}".format(i), fontsize=24)
 
@@ -75,16 +90,23 @@
         plt.legend(fontsize=18)
 
         plt.savefig(folder+"Abundance_Analysis/Abundance_Hist/hist_abundance_{}.pdf".format(i))
         plt.close()
 
 
 def plot_differ_hist(abund, elements, folder):
-    # Plot histograms for abundance shift for each element
-    # and trace a gaussian with the mean and standard deviation
+    """
+    Plot histograms for abundance shift for each element
+    and trace a gaussian with the mean and standard deviation
+
+    :param abund: pandas element with the abundances.
+    :param elements: elements to create histograms.
+    :param folder: directory to be saved.
+    """
+
     for i in elements:
         elem_differ = abund["Differ"][abund.Element == i]
 
         plt.figure(figsize=(16, 9))
 
         plt.title("Difference of Expected and Found Abundances for Element {}".format(i), fontsize=24)
 
@@ -110,14 +132,22 @@
         plt.legend(fontsize=18)
 
         plt.savefig(folder+"Abundance_Analysis/Difference_Hist/hist_differ_{}.pdf".format(i))
         plt.close()
 
 
 def plot_abund_box(abund, elements, folder):
+    """
+    Create the abundance box plot.
+
+    :param abund: pandas element with the abundances.
+    :param elements: elements to create histograms.
+    :param folder: directory to be saved.
+    """
+
     abund_matrix = []
     for i in elements:
         abund_matrix.append(abund["Fit Abundance"][abund.Element == i])
 
     plt.figure(figsize=(16, 9))
 
     plt.title("Elements Abundances", fontsize=24)
@@ -139,38 +169,55 @@
     plt.tight_layout()
 
     plt.savefig(folder+"Abundance_Analysis/Abundance_box.pdf")
     plt.close()
 
 
 def get_spectrum(fit_data, conv_name, config_fl, elem, abundance_shift=0., cut_val=1.):
-    # Function to get the observed spectrum in the desired range
+    """
+    Function to get the synthetic spectrum in the desired range.
+
+    :param fit_data: pandas dataframe with the results.
+    :param conv_name: file name of the TurboSpectrum output file.
+    :param config_fl: file name of the TurboSpectrum configuration file.
+    :param elem: element to be plotted.
+    :param abundance_shift: overall shift in abundance, if needed.
+    :param cut_val: range to plot.
+    :return: the final spectrum.
+    """
 
     # Get data from fit
     lamb = fit_data["Lambda (A)"]
     abundance = fit_data["Fit Abundance"] + abundance_shift
 
     # Run the model with the desired abundance
     ab_fit.change_spec_range_configfl(config_fl, lamb, cut_val)
     ab_fit.change_abund_configfl(config_fl, elem, find=False, abund=abundance)
     ab_fit.run_configfl(config_fl)
 
     # Read and cut the model spectrum to the desired range
-    spec = pd.read_csv(conv_name, header=None, delimiter="\s+")
+    spec = pd.read_csv(conv_name, header=None, delimiter=r"\s+")
     # spec = ab_fit.cut_spec(spec, lamb, cut_val/2)
 
     # Apply the fit resolutions to the spectra
     spec = ab_fit.spec_operations(spec.copy(), lamb_desloc=fit_data["Lamb Shift"], continuum=fit_data.Continuum,
                                   convol=fit_data.Convolution)
 
     return spec
 
 
 def get_diff(spec1, spec2):
-    # Function to get the difference of observed and model spectrum
+    """
+    Get the difference of observed and synthetic spectrum.
+
+    :param spec1: first spectrum.
+    :param spec2: second spectrum.
+    :return: -1 if it finds nothing; otherwise the difference.
+    """
+
     lambs = np.array([])
     sp1_interpol = np.array([])
     sp2_interpol = np.array([])
 
     for i in spec2.iloc():
         pos = ab_fit.bisec(spec1, i[0])
         if pos != -1:
@@ -189,15 +236,29 @@
         return -1
     else:
         return [lambs, sp2_interpol-sp1_interpol]
 
 
 def plot_lines(obs_specs, abund, refer_fl, conv_name, config_fl, folder, order_sep, cut_val=.5, abundance_shift=.1,
                drop=0):
-    # Plot the spectrum fit and the observed one
+    """
+    Plot the spectrum fit and the observed one
+
+    :param obs_specs: spectrum data.
+    :param abund: abundance pandas object.
+    :param refer_fl: file name of the reference abundances file.
+    :param conv_name: file name of the TurboSpectrum output file.
+    :param config_fl: file name of the TurboSpectrum configuration file.
+    :param folder: directory to save.
+    :param order_sep: it needs to get of the order in the elements.
+    :param cut_val: range to plot the lines.
+    :param abundance_shift: overall abundance shift.
+    :param drop: remove elements of the ``abund`` dataframe.
+    """
+
     abund.drop(range(drop), inplace=True)
 
     for i in range(len(abund)):
         elem = abund.Element.iloc[i]
         lamb = abund["Lambda (A)"].iloc[i]
         abundance = abund["Fit Abundance"].iloc[i]
 
@@ -287,27 +348,36 @@
         plt.savefig(folder+"Abundance_Analysis/Lines_Plot/fit_{}_{}_ang.pdf".format(elem+order, lamb))
         plt.close()
 
         print("{} of {} finished.".format(i+1, len(abund)))
 
 
 def folders_creation(folder):
-    # Subroutine to create necessary folders
+    """
+    Subroutine to create necessary folders
+
+    :param folder: root folder of the results.
+    """
+
     if not os.path.exists(folder+"Abundance_Analysis"):
         os.mkdir(folder+"Abundance_Analysis")
     if not os.path.exists(folder+"Abundance_Analysis/Abundance_Hist"):
         os.mkdir(folder+"Abundance_Analysis/Abundance_Hist")
     if not os.path.exists(folder+"Abundance_Analysis/Difference_Hist"):
         os.mkdir(folder+"Abundance_Analysis/Difference_Hist")
     if not os.path.exists(folder+"Abundance_Analysis/Lines_Plot"):
         os.mkdir(folder+"Abundance_Analysis/Lines_Plot")
 
 
 def main(args):
-    # Main Routine
+    """
+    Main Routine.
+
+    :param args: command line arguments.
+    """
 
     # Arguments Menu Call
     config_name = ab_fit.args_menu(args)
 
     # Read Configuration File
     list_name, refer_name, type_synth, config_fl, conv_name, folder, observed_name = ab_fit.read_config(config_name)
     order_sep = list_name[2]
```

### Comparing `meafs-4.6.3/meafs_code/scripts/abundance_fit.py` & `meafs-4.7.12/meafs_code/scripts/abundance_fit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
-#####################################################
-# Abundance Fit                                     #
-# Matheus J. Castro                                 #
-# v4.6                                              #
-# Last Modification: 04/23/2024                     #
-# Contact: matheusdejesuscastro@gmail.com           #
-#####################################################
+"""
+| MEAFS Abundance Fit
+| Matheus J. Castro
+| v4.7
+
+| Main fit code to do all the operations with the spectrum, call the modules to generate
+  the synthetic spectrum, plot the curves and more.
+"""
 
 from specutils.analysis import equivalent_width
 from PyQt6 import QtWidgets, QtCore
 from specutils import Spectrum1D
 import matplotlib.pyplot as plt
 import astropy.units as u
 from pathlib import Path
@@ -19,35 +20,58 @@
 import sys
 import os
 
 from . import fit_functions as ff
 from . import voigt_functions as vf
 from . import turbospec_functions as tf
 
-version = 4.6
+version = "4.7"
 
 
 def open_linelist_refer_fl(list_name):
-    # Function to open the Linelist using PANDAS
+    """
+    Open the Linelist using PANDAS.
+
+    :param list_name: file name of the linelist.
+    :return: the pandas dataframe with the linelist.
+    """
+
     return pd.read_csv(list_name, header=None)
 
 
 def open_spec_obs(observed_name, delimiter=None, increment=1):
-    # Function to open the observed spectrum file using PANDAS
+    """
+    Open the observed spectrum file using PANDAS.
+
+    :param observed_name: file name with the spectrum.
+    :param delimiter: delimiter type of the file.
+    :param increment: increment to get the delimiter automatically
+                      (previously necessary in the older no-gui version).
+    :return: the pandas dataframe with the spectrum.
+    """
+
     spec_obs = []
 
     for i in range(0, len(observed_name), increment):
         if increment == 2:
             delimiter = observed_name[i + 1]
-        spec_obs.append(pd.read_csv(observed_name[i], header=None, delimiter=delimiter))
+        spec_obs.append(pd.read_csv(observed_name[i], header=None, delimiter=delimiter, comment="#"))
     return spec_obs
 
 
 def open_previous(linelist, columns_names, fl_name=Path("found_values.csv")):
-    # Function to open the previous results and analyze it
+    """
+    Open the previous results and analyse it.
+
+    :param linelist: linelist object.
+    :param columns_names: names of the columns in the file.
+    :param fl_name: file name.
+    :return: the new linelist and the pandas dataframe with the previous results.
+    """
+
     try:
         # Try to open
         prev = pd.read_csv(fl_name, delimiter=",")
     except (FileNotFoundError, pd.errors.EmptyDataError):
         # If file not found or empty database, create a new one and return
         return linelist, pd.DataFrame(columns=columns_names)
 
@@ -60,14 +84,24 @@
         if ind.tolist() == []:
             new_linelist.loc[i] = linelist.iloc[i]
 
     return new_linelist, prev
 
 
 def plot_spec_gui(specs, canvas, ax, plot_line_refer):
+    """
+    Plot the spectrum in the GUI.
+
+    :param specs: spectrum data to be plotted.
+    :param canvas: canvas to plot.
+    :param ax: ax to plot.
+    :param plot_line_refer: array to save the reference label of the plots.
+    :return: the actualized ``plot_line_refer`` array.
+    """
+
     if specs != []:
         min_all_old = min(specs[0].iloc[:, 0])
         max_all_old = max(specs[0].iloc[:, 0])
     else:
         min_all_old = 0
         max_all_old = 1
 
@@ -92,15 +126,28 @@
     ax.set_xlim(min_all_old, max_all_old)
     canvas.draw()
 
     return plot_line_refer
 
 
 def plot_spec(spec1, spec2, spec3, lamb, elem, folder, show=False, save=True):
-    # Plot the spectra
+    """
+    Plot the spectra (previously necessary in the older no-gui version).
+
+    :param spec1: first spectrum data.
+    :param spec2: second spectrum data.
+    :param spec3: third spectrum data.
+    :param lamb: current wavelength.
+    :param elem: current element.
+    :param folder: directory to save the plot.
+    :param show: true to show with the ``matplotlib.pyplot.show()``.
+    :param save: true to save the spectrum.
+    """
+
+
     plt.figure(figsize=(16, 9))
 
     plt.plot(spec1[0], spec1[1], label="Observed")
     plt.plot(spec2[0], spec2[1], label="Abundance Fit")
     if spec3 is not None:
         plt.plot(spec3[0], spec3[1], label="Final Fit")
     if lamb is not None:
@@ -111,15 +158,30 @@
     if show:
         plt.show()
     if save:
         plt.savefig(Path(folder).joinpath("On_time_Plots", "fit_{}_{}_ang.pdf".format(elem, lamb)))
     plt.close()
 
 
-def plot_spec_ui(spec_fit_arr, folder, elem, lamb, order, ax, canvas, plot_line_refer):
+def plot_spec_ui(spec_fit_arr, folder, elem, lamb, order, ax, canvas, plot_line_refer, vline=True):
+    """
+    Plot the current line results in the GUI.
+
+    :param spec_fit_arr: spectrum line data.
+    :param folder: directory to save.
+    :param elem: current element.
+    :param lamb: current wavelength.
+    :param order: current order of the line.
+    :param ax: ax to plot.
+    :param canvas: canvas to plot.
+    :param plot_line_refer: array to save the reference label of the plots.
+    :param vline: if it also plots a vertical line or not.
+    :return: the actualized ``plot_line_refer`` array.
+    """
+
     # noinspection PySimplifyBooleanCheck
     if spec_fit_arr != []:
         min_all_old = min(spec_fit_arr[0].iloc[:, 0])
         max_all_old = max(spec_fit_arr[0].iloc[:, 0])
     else:
         min_all_old = 0
         max_all_old = 1
@@ -128,51 +190,78 @@
         ind = plot_line_refer[(plot_line_refer["elem"] == elem + order) &
                               (plot_line_refer["wave"] == lamb)].index
         for line in plot_line_refer.loc[ind, "refer"]: line.remove()
         plot_line_refer.drop(ind, inplace=True)
         plot_line_refer.reset_index(drop=True, inplace=True)
 
         lineplot = ax.plot(sp.iloc[:, 0], sp.iloc[:, 1], "--", linewidth=1.5)
-        axvlineplot = ax.axvline(lamb, ls="-.", c="red", linewidth=.5)
+
         min_all = min(sp.iloc[:, 0])
         max_all = max(sp.iloc[:, 0])
         if min_all < min_all_old:
             min_all_old = min_all
         if max_all > max_all_old:
             max_all_old = max_all
 
         plot_line_refer.loc[len(plot_line_refer)] = {"elem": elem+order, "wave": lamb, "refer": lineplot[0]}
-        plot_line_refer.loc[len(plot_line_refer)] = {"elem": elem+order, "wave": lamb, "refer": axvlineplot}
+
+        if vline:
+            axvlineplot = ax.axvline(lamb, ls="-.", c="red", linewidth=.5)
+            plot_line_refer.loc[len(plot_line_refer)] = {"elem": elem+order, "wave": lamb, "refer": axvlineplot}
 
         sp.to_csv(Path(folder).joinpath("On_time_Plots",
                                         "fit_{}_{}_ang_{}.csv".format(elem + order, lamb, j + 1)),
                   index=False,
                   float_format="%.4f",
                   header=None)
 
     ax.set_xlim(min_all_old, max_all_old)
     canvas.draw()
 
     return plot_line_refer
 
 
 def check_order(elem):
+    """
+    | Check if the current element has any type of order written in the end of the string.
+    | Supported types are: roman numbers *(I, II, III...)* and western digits *(1, 2, 3...)*.
+
+    :param elem:
+    :return: the element without the order and the order itself.
+    """
+
     if elem[1].isdigit() or elem[1] == "I" or elem[1] == "V" or elem[1] == "X" or elem[1] == " ":
         order = elem[1:]
         elem = elem[0]
     else:
         order = elem[2:]
         elem = elem[0:2]
 
     return elem, order
 
 
 def plot_abund_nofit(elem, lamb, abundplot, refer_fl, folder, type_synth,
                      cut_val=None, canvas=None, ax=None, plot_line_refer=None,
                      opt_pars=None):
+    """
+    Plot in the GUI the specified parameters.
+
+    :param elem: current element.
+    :param lamb: current wavelength.
+    :param abundplot: abundance to be plotted.
+    :param refer_fl: reference abundance dataframe.
+    :param folder: directory to save.
+    :param type_synth: type of the current synthetics spectrum generator.
+    :param cut_val: range to plot.
+    :param canvas: canvas to plot.
+    :param ax: ax to plot.
+    :param plot_line_refer: array to save the reference label of the plots.
+    :param opt_pars: parameters for the convolution, wavelength shift and continuum.
+    :return: the actualized ``plot_line_refer`` array.
+    """
 
     if type_synth[0] == "TurboSpectrum":
         conv_name = type_synth[1]
         config_fl = type_synth[2]
     else:
         conv_name = None
         config_fl = None
@@ -194,15 +283,15 @@
     elif type_synth[0] == "TurboSpectrum":
         tf.change_abund_configfl(config_fl, elem, find=False, abund=abundplot)
         tf.change_spec_range_configfl(config_fl, lamb, cut_val[3])
         tf.run_configfl(config_fl)
         # Return the Turbospectrum2019 configuration file to original abundance value
         tf.change_abund_configfl(config_fl, elem, find=False, abund=abund_val_refer)
 
-        spec_conv = pd.read_csv(conv_name, header=None, delimiter="\s+")
+        spec_conv = pd.read_csv(conv_name, header=None, delimiter=r"\s+")
 
         # noinspection PyTypeChecker
         spec_fit = ff.spec_operations(spec_conv.copy(), lamb_desloc=opt_pars[0], continuum=opt_pars[1],
                                       convol=opt_pars[2])
     else:
         return plot_line_refer
 
@@ -213,15 +302,39 @@
 
 
 def fit_abundance(linelist, spec_obs, refer_fl, folder, type_synth, cut_val=None,
                   abund_lim_df=1., restart=False, save_name="found_values.csv",
                   ui=None, canvas=None, ax=None, plot_line_refer=None,
                   opt_pars=None, repfit=2, max_iter=None, convovbound=None,
                   contpars=None, wavebound=None):
-    # Function to analyse the spectrum and find the fit values for it
+    """
+    Main function to analyse the spectrum and find the fit values for it
+
+    :param linelist: linelist dataframe.
+    :param spec_obs: spectrum data.
+    :param refer_fl: reference abundace dataframe.
+    :param folder: directory to save.
+    :param type_synth: type of the current synthetics spectrum generator.
+    :param cut_val: ranges to cut the spectrum.
+    :param abund_lim_df: default value of the range of the allowed abundance.
+    :param restart: if it should ignore past results in the database.
+    :param save_name: file name of the previous results.
+    :param ui: main GUI QT object.
+    :param canvas: canvas to plot.
+    :param ax: ax to plot.
+    :param plot_line_refer: array to save the reference label of the plots.
+    :param opt_pars: convolution, wavelength shift and continuum initial guess.
+    :param repfit: number of iterations of the main fit function.
+    :param max_iter: maximum allowed iterations of the Nelder-Mead method.
+    :param convovbound: range to fit the convolution.
+    :param contpars: the calibration values of the overall continuum fit method.
+    :param wavebound: range to fit the wavelength shift.
+    :return: dataframe with the results of the fit, the actualized
+             ``ax`` array and the actualized ``plot_line_refer`` array.
+    """
 
     stop = False
 
     def stop_state():
         nonlocal stop
         stop = True
 
@@ -348,20 +461,22 @@
             spec_obs_cut = ff.cut_spec(spec_obs, lamb, cut_val=cut_val[0])
 
             if type_synth[0] == "Equivalent Width":
                 if opt_pars is None:
                     opt_pars, chi, spec_fit = vf.optimize_spec(spec_obs_cut, type_synth, lamb, continuum,
                                                                iterac=max_iter[1], convovbound=convovbound,
                                                                wavebound=wavebound)
-                ui.abundancelabel.setText("Deepth")
+                if ui is not None:
+                    ui.abundancelabel.setText("Deepth")
             elif type_synth[0] == "TurboSpectrum":
                 tf.change_spec_range_configfl(config_fl, lamb, cut_val[0])
                 tf.run_configfl(config_fl)
-                spec_conv = pd.read_csv(conv_name, header=None, delimiter="\s+")
-                ui.abundancelabel.setText("Abundance")
+                spec_conv = pd.read_csv(conv_name, header=None, delimiter=r"\s+")
+                if ui is not None:
+                    ui.abundancelabel.setText("Abundance")
 
                 if opt_pars is None:
                     opt_pars = tf.optimize_spec(spec_obs_cut, spec_conv, lamb, cut_val, continuum,
                                                 init=opt_pars, iterac=max_iter[1], convovbound=convovbound,
                                                 wavebound=wavebound)
             # opt_pars = [0,0,0]
 
@@ -398,23 +513,23 @@
 
             # Fit of Equivalent Width Observed Spectrum
             # noinspection PyUnresolvedReferences
             spec1d = Spectrum1D(spectral_axis=np.asarray(spec_obs_cut[0]) * u.AA,
                                 flux=np.asarray(spec_obs_cut[1]) * u.Jy)
             equiv_width_obs = equivalent_width(spec1d)
             # noinspection PyUnresolvedReferences
-            equiv_width_obs = np.float128(equiv_width_obs / u.AA)
+            equiv_width_obs = np.float16(equiv_width_obs / u.AA)
 
             # Fit of Equivalent Width Fitted Spectrum
             # noinspection PyUnresolvedReferences
             spec1d = Spectrum1D(spectral_axis=np.asarray(spec_fit[0]) * u.AA,
                                 flux=np.asarray(spec_fit[1]) * u.Jy)
             equiv_width_fit = equivalent_width(spec1d)
             # noinspection PyUnresolvedReferences
-            equiv_width_fit = np.float128(equiv_width_fit / u.AA)
+            equiv_width_fit = np.float16(equiv_width_fit / u.AA)
 
         found_val.loc[index_append] = [elem+order, lamb, opt_pars[0], opt_pars[1], opt_pars[2], abund_val_refer,
                                        par[0], np.abs(par[0]-abund_val_refer), "{:.4e}".format(chi),
                                        "{:.4e}".format(equiv_width_obs), "{:.4e}".format(equiv_width_fit)]
 
         # Plot of data
         spec_obs_cut = ff.cut_spec(spec_obs, lamb, cut_val=cut_val[3])
@@ -425,15 +540,15 @@
         elif type_synth[0] == "TurboSpectrum":
             tf.change_abund_configfl(config_fl, elem, find=False, abund=par[0])
             tf.change_spec_range_configfl(config_fl, lamb, cut_val[3])
             tf.run_configfl(config_fl)
             # Return the Turbospectrum2019 configuration file to original abundance value
             tf.change_abund_configfl(config_fl, elem, find=False, abund=abund_val_refer)
 
-            spec_conv = pd.read_csv(conv_name, header=None, delimiter="\s+")
+            spec_conv = pd.read_csv(conv_name, header=None, delimiter=r"\s+")
 
             # noinspection PyTypeChecker
             spec_fit = ff.spec_operations(spec_conv.copy(), lamb_desloc=opt_pars[0], continuum=opt_pars[1],
                                           convol=opt_pars[2])
 
         if ui is None:
             plot_spec(spec_obs_cut, spec_conv, spec_fit, lamb, elem+order, folder)
@@ -453,21 +568,31 @@
             # linescurrent = ui.progressvalue.text().split("/")
             ui.progressvalue.setText("{}/{}".format(i+1, len(linelist)))
 
     return found_val, ax, plot_line_refer
 
 
 def read_config(config_name):
-    # Function to read the configuration file
+    """
+    Function to read the configuration file (previously necessary in
+    the older no-gui version).
+
+    :param config_name: configuration file name.
+    :return: linelist file name, reference abundance file name, type of the
+             synthetics spectrum to use, TurboSpectrum configuration file name,
+             TurboSpectrum results file name, directory to save the results,
+             spectrum file name.
+    """
+
     def separator(sep):
         # Define the type of separator
         if sep == "comma":
             return ","
         elif sep == "tab":
-            return "\s+"
+            return r"\s+"
         else:
             return ","
 
     # Read file
     config_data = pd.read_csv(config_name, comment="#", header=None)
 
     # Enable long strings
@@ -496,14 +621,33 @@
         observed_name[i] = separator(observed_name[i])
 
     return list_name, refer_name, type_synth, config_fl, conv_name, folder, observed_name
 
 
 def gui_call(spec_obs, ui, checkstate, canvas, ax, cut_val=None, plot_line_refer=None, opt_pars=None,
              repfit=2, abundplot=None, results_array=None):
+    """
+    Main function to be called from the GUI.
+
+    :param spec_obs: spectrum data.
+    :param ui: main GUI QT object.
+    :param checkstate: QT checked state for checkboxes.
+    :param canvas: GUI canvas plot object.
+    :param ax: GUI ax plot object.
+    :param cut_val: range to cut the spectrum.
+    :param plot_line_refer: array with a list of the current available plots.
+    :param opt_pars: convolution, wavelength shift and continuum parameters.
+    :param repfit: number of iterations of the main fit function.
+    :param abundplot: overwrite the abundance fit and only plot the value
+                      present in this variable.
+    :param results_array: array for the results of the fit.
+    :return: the results of the fit, the actualized ``ax`` variable and the
+             actualized ``plot_line_refer`` variable.
+    """
+
     # Time Counter
     init = time.time()
     init_local = time.localtime()
     init_time = "Run started at: {} {} {}, {}:{}:{}.".format(init_local.tm_year,
                                                              init_local.tm_mon,
                                                              init_local.tm_mday,
                                                              init_local.tm_hour,
@@ -524,18 +668,16 @@
         restart = True
     else:
         restart = False
 
     folder = ui.outputname.text()
 
     # Create necessary folders
-    if not os.path.exists(folder):
-        os.mkdir(folder)
-    if not os.path.exists(Path(folder).joinpath("On_time_Plots")):
-        os.mkdir(Path(folder).joinpath("On_time_Plots"))
+    folder_create = Path(folder).joinpath("On_time_Plots")
+    os.makedirs(folder_create, exist_ok=True)
 
     linelist = []
     for line in range(ui.linelistcontent.rowCount()):
         item = ui.linelistcontent.cellWidget(line, 2).layout().itemAt(0).widget()
         if item.checkState() == checkstate and \
            ui.linelistcontent.item(line, 0) is not None and \
            ui.linelistcontent.item(line, 1) is not None:
@@ -597,30 +739,34 @@
 
     ui.run.setText("Run")
     ui.run.setStyleSheet("background-color: none")
 
     # Time Counter
     end = time.time()
     dif = end - init
-    time_spent = "Time spent: {:.0f} h {:.0f} m {:.0f} s ({:.0f} s).".format(dif // 3600, (dif // 60) % 60, dif % 60,
-                                                                             dif)
+    time_spent = "Time spent: {:.0f} h {:.0f} m {:.0f} s ({:.0f} s).\n".format(dif // 3600, (dif // 60) % 60,
+                                                                               dif % 60, dif)
 
     # noinspection PyTypeChecker
     with open(str(Path(folder).joinpath("log.txt")), "a") as f:
         f.write(init_time)
         f.write(time_spent)
         f.write("\n")
         f.close()
     print(time_spent)
 
     return results_array, ax, plot_line_refer
 
 
 def main(args):
-    # Main subroutine to call the functions
+    """
+    Main subroutine to call the functions (previously necessary in the older no-gui version).
+
+    :param args: system command line arguments.
+    """
 
     # Time Counter
     init = time.time()
 
     # Arguments Menu Call
     config_name = args_menu(args)
 
@@ -660,14 +806,19 @@
 
     # noinspection PyTypeChecker
     np.savetxt(folder+"log.txt", [time_spent], fmt="%s")
     print(time_spent)
 
 
 def args_menu(args):
+    """
+    Run the arguments resolve and print them if necessary (previously necessary in the older no-gui version).
+
+    :param args: system command line arguments.
+    """
 
     if len(args) <= 1 and not any((i == "-h" or i == "--h" or i == "-help" or i == "--help") for i in args):
         if len(args) != 0:
             config_name = args[0]
         else:
             config_name = "meafs_config.txt"
 
@@ -685,8 +836,8 @@
                    "Options are:\n -h,  -help\t|\tShow this help;\n--h, --help\t|\tShow this help;\n" \
                    "\n\nExample:\n./abundance_fit.py meafs_config.txt\n".format(version)
         print(help_msg)
 
 
 if __name__ == '__main__':
     arg = sys.argv[1:]
-    main(arg)  # call main subroutine
+    main(arg)  # call main subroutine
```

### Comparing `meafs-4.6.3/meafs_code/scripts/unify_plots.py` & `meafs-4.7.12/meafs_code/scripts/unify_plots.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,63 @@
 #!/usr/bin/env python3
+"""
+| MEAFS Unify generated plots in a single PDF file for each type
+| Matheus J. Castro
+| v2.0
+
+| This script aims to create a single result file for each analyze type created with the abundance_fit.py and
+  abundance_analysis.py scripts.
+| It uses pdflatex to generate it. You can install it following the steps for your OS distribution here:
+  https://www.latex-project.org/get/
 
-############################################################
-# Unify generated plots in a single PDF file for each type #
-# Matheus J. Castro                                        #
-# v2.0                                                     #
-# Last Modification: 07/01/2022                            #
-# Contact: matheusdejesuscastro@gmail.com                  #
-############################################################
-
-# This script aims to create a single result file for each analyze type created with the abundance_fit.py and
-# abundance_analysis.py scripts.
-# It uses pdflatex to generate it. You can install it following the steps for your OS distribution here:
-# https://www.latex-project.org/get/
-
-# For this code work, it must be in the same folder as the abundance_fit.py file
+| For this code work, it must be in the same folder as the *abundance_fit.py* file
+"""
 
 import os
 import sys
 
 # Import the main script
 try:
     import abundance_fit as ab_fit
 except ModuleNotFoundError:
     from . import abundance_fit as ab_fit
 
 
 def write(fl_name, data):
+    """
+    Write the data in a file.
+
+    :param fl_name: file name.
+    :param data: data to be written.
+    """
+
     # Write the latex file
     with open(fl_name, 'w') as file:
         file.write(data)
 
 
 def run_pdflatex(fl_name, folder):
+    """
+    Run the ``pdflatex`` command to generate the unified PDF.
+
+    :param fl_name: file name.
+    :param folder: directory where the file should be created.
+    """
+
     # Run pdflatex command
     os.system("cd {}Unique_Plot && pdflatex -interaction=nonstopmode {}".format(folder, fl_name))
 
 
 def main(args):
+    """
+    Main function that read the plot files.
+
+    :param args: command line arguments.
+    """
+
     # Arguments Menu Call
     config_name = ab_fit.args_menu(args)
 
     # Read Configuration File
     list_name, refer_name, type_synth, config_fl, conv_name, folder, observed_name = ab_fit.read_config(config_name)
 
     # Create necessary folder
```

### Comparing `meafs-4.6.3/pyproject.toml` & `meafs-4.7.12/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "meafs"
-version = "4.6.3"
+version = "4.7.12"
 authors = [
     { name="Matheus J. Castro" }
 ]
 description="Multiple Element Abundance Fit Software"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers=[
@@ -19,18 +19,20 @@
     "scipy",
     "matplotlib",
     "pandas",
     "numpy",
     "desktop_file==1.3",
     "pathlib",
     "PyQt6",
-    "dill"
+    "dill",
+    "qtconsole"
 ]
 
 [project.scripts]
 meafs = "meafs_code.gui:main"
 meafs-desktop-create = "meafs_code.desktop_entry:create"
 meafs-desktop-remove = "meafs_code.desktop_entry:remove"
 
 [project.urls]
-"Homepage" = "https://github.com/MatheusJCastro/meafs"
+"homepage" = "https://meafs.readthedocs.io/"
+"repository" = "https://github.com/MatheusJCastro/meafs"
```

