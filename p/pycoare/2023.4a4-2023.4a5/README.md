# Comparing `tmp/pycoare-2023.4a4.tar.gz` & `tmp/pycoare-2023.4a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycoare-2023.4a4.tar", last modified: Tue Apr 18 01:08:09 2023, max compression
+gzip compressed data, was "pycoare-2023.4a5.tar", last modified: Fri May 26 22:35:27 2023, max compression
```

## Comparing `pycoare-2023.4a4.tar` & `pycoare-2023.4a5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:08:09.383320 pycoare-2023.4a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-18 01:07:58.000000 pycoare-2023.4a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-18 01:08:09.383320 pycoare-2023.4a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-04-18 01:07:58.000000 pycoare-2023.4a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:08:09.379320 pycoare-2023.4a4/pycoare/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 01:07:58.000000 pycoare-2023.4a4/pycoare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-04-18 01:07:58.000000 pycoare-2023.4a4/pycoare/coare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:08:09.383320 pycoare-2023.4a4/pycoare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-18 01:08:09.000000 pycoare-2023.4a4/pycoare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-18 01:08:09.000000 pycoare-2023.4a4/pycoare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:08:09.000000 pycoare-2023.4a4/pycoare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 01:08:09.000000 pycoare-2023.4a4/pycoare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 01:08:09.000000 pycoare-2023.4a4/pycoare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-18 01:07:58.000000 pycoare-2023.4a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 01:08:09.383320 pycoare-2023.4a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:08:09.383320 pycoare-2023.4a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-18 01:07:58.000000 pycoare-2023.4a4/tests/test_coare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 22:35:27.028080 pycoare-2023.4a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-26 22:35:16.000000 pycoare-2023.4a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-26 22:35:27.028080 pycoare-2023.4a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-05-26 22:35:16.000000 pycoare-2023.4a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 22:35:27.028080 pycoare-2023.4a5/pycoare/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-26 22:35:16.000000 pycoare-2023.4a5/pycoare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-26 22:35:16.000000 pycoare-2023.4a5/pycoare/coare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-26 22:35:16.000000 pycoare-2023.4a5/pycoare/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 22:35:27.028080 pycoare-2023.4a5/pycoare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-26 22:35:27.000000 pycoare-2023.4a5/pycoare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-26 22:35:27.000000 pycoare-2023.4a5/pycoare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 22:35:27.000000 pycoare-2023.4a5/pycoare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 22:35:27.000000 pycoare-2023.4a5/pycoare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 22:35:27.000000 pycoare-2023.4a5/pycoare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-26 22:35:16.000000 pycoare-2023.4a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 22:35:27.028080 pycoare-2023.4a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 22:35:27.028080 pycoare-2023.4a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-26 22:35:16.000000 pycoare-2023.4a5/tests/test_coare.py
```

### Comparing `pycoare-2023.4a4/LICENSE` & `pycoare-2023.4a5/LICENSE`

 * *Files identical despite different names*

### Comparing `pycoare-2023.4a4/PKG-INFO` & `pycoare-2023.4a5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,41 @@
-Metadata-Version: 2.1
-Name: pycoare
-Version: 2023.4a4
-Summary: A Python implementation of the COARE bulk air-sea flux algorithm.
-Author: C. W. Fairall, Byron Blomquist, Ludovic Bariteau, J. B. Edson
-Maintainer-email: Andrew Scherer <scherand@oregonstate.edu>
-License: MIT License
-Project-URL: Source, https://github.com/andrew-s28/COARE-algorithm
-Keywords: oceanography,air-sea,bulk flux
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pyCOARE
-[![CI](https://github.com/andrew-s28/COARE-algorithm/workflows/tests/badge.svg?branch=master)](https://github.com/andrew-s28/COARE-algorithm/actions)
-[![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](ttps://github.com/andrew-s28/COARE-algorithm/blob/master/LICENSE.txt)
-[![Code coverage](https://codecov.io/gh/andrew-s28/COARE-algorithm/branch/master/graph/badge.svg)](https://app.codecov.io/gh/andrew-s28/COARE-algorithm)
+[![Tests](https://github.com/pyCOARE/coare/actions/workflows/tests.yml/badge.svg)](https://github.com/pyCOARE/coare/actions/workflows/tests.yml)
+[![License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](ttps://github.com/pyCOARE/coare/blob/master/LICENSE.txt)
+[![Code coverage](https://codecov.io/gh/pyCOARE/coare/branch/main/graph/badge.svg)](https://app.codecov.io/gh/pyCOARE/coare)
+[![Docs](https://readthedocs.org/projects/coare-live/badge/?version=latest)](https://coare-live.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://img.shields.io/pypi/v/pycoare?style=plastic)](https://pypi.org/project/pycoare/)
 
 ## COARE-algorithm
 
 This is an alpha-quality fork of the Python version of the [COARE algorithm](https://github.com/NOAA-PSL/COARE-algorithm) that was written with the goal of standardizing testing, packaging, and distribution of the algorithm. Currently only COARE v3.5 is implemented - hopefully v3.6 will come soon! 
 
-The functionality of the code is ideally the same as that for the scripts found in the NOAA PSL repository linked above. My only intended contributions are towards formatting, testing, and packaging. To that end, tests have been constructed based on the output of the original MATLAB code for COARE v3.5. [View the results of the tests](https://github.com/andrew-s28/COARE-algorithm/actions) or [download the data](https://github.com/andrew-s28/COARE-algorithm/tree/master/tests/data) and run them yourself. All results from this script agree to at least five significant figures with the MATLAB scripts in the NOAA repository, provided the testing badge above stays green. 
+The functionality of the code is ideally the same as that for the scripts found in the NOAA PSL repository linked above. My only intended contributions are towards formatting, testing, and packaging. To that end, tests have been constructed based on the output of the original MATLAB code for COARE v3.5. [View the results of the tests](https://github.com/pyCOARE/coare/actions) or [download the data](https://github.com/pyCOARE/coare/tree/main/tests/data) and run them yourself. All results from this script agree to at least five significant figures with the MATLAB scripts in the NOAA repository, provided the testing badge above stays green. 
 
 ## Installation
 
 The latest stable version (currently still an alpha) can be downloaded using Pip
 ```
 pip install pycoare
 ```
 
 You can install the most up-to-date version using 
 ```
-pip install git+https://github.com/andrew-s28/COARE-algorithm
+pip install git+https://github.com/pyCOARE/coare
 ```
 
 ## Contribution
 
-I welcome any contributions - please feel free to raise an issue or submit a pull request. My hope is that this implementation will get better as those with more knowledge on bulk air-sea fluxes or Python software development get involved. 
+I welcome any contributions - please feel free to [raise an issue](https://github.com/pyCOARE/coare/issues) or submit a [pull request](https://github.com/pyCOARE/coare/pulls).
 
-## Origins
+## Origins and Credits
 The international TOGA-COARE field program which took place in the western Pacific warm pool over 4 months from November 1992 to February 1993 ([Fairall et al. 1996a](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Fairall%20et%20al.%201996a%20-%20cool%20skin%20warm%20layer.pdf), [1996b](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Fairall%20et%20al.%201996b%20-%20bulk%20fluxes%20of%20variables.pdf) and [1997](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Fairall%20et%20al.%201997%20-%20ship%20measurements%20MABL.pdf)) spurred the development of the COARE model. The algorithm is intended to provide estimates of `momentum, sensible heat`, and `latent heat fluxes` using inputs of bulk atmospheric variables (`wind speed, SST, air temperature, air humidity`). The algorithm contains subroutines/functions to handle near-surface gradients of temperature in the ocean.
 
+This Python implementation of the COARE algorithm was initially translated from MATLAB by Byron Blomquist and Ludovic Bariteau. For more information on the people and publications that developed the COARE algorithm, see the references below.
+
 ## Versions
 - **Version 2.5** was published in 1996. 
 - **Version 3.0** was published in 2003; it was a major update from Version 2.5. This update was based on new observations at higher wind speeds (10 to 20 m/s). Available in MATLAB and FORTRAN only.
 - **Version 3.5** was released in 2013 following the publication of [Edson et al. 2013](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Edson%20et%20al.%202013%20-%20momentum%20flux.pdf), which made adjustments to the wind speed dependence of the Charnock parameter based on a large database of direct covariance stress observations (principally from a buoy). This led to an increase in stress for wind speeds greater than about 18 m/s. The roughness Reynolds number formulation of the scalar roughness length was tuned slightly to give the same values of `Ch` and `Ce` as Version 3.0. The diurnal warm layer model was structured as a separate routine instead of embedded in a driver program. COARE 3.5 was based on Edson’s buoy data ([Edson et al. 2013](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Edson%20et%20al.%202013%20-%20momentum%20flux.pdf)) and was compared to a large database (a total of 16,000 hours of observations) combining observations from NOAA, WHOI, and U. Miami ([Fairall et al. 2011](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Fairall%20et%20al.%202011%20-%20COAREG.pdf)). It is available in Python and MATLAB.
 - **Version 3.6** is slightly restructured and built around improvements in the representation of the effects of waves on fluxes. This includes improved relationships of `surface roughness`, $z_o$, and `whitecap fraction`, $W_f$, on wave parameters.  More details can be found in [coare3.6\_readme\_1.pdf](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/coare36_readme_1.pdf). This version is available in Python, MATLAB and FORTRAN.
```

### Comparing `pycoare-2023.4a4/README.md` & `pycoare-2023.4a5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,60 @@
+Metadata-Version: 2.1
+Name: pycoare
+Version: 2023.4a5
+Summary: A Python implementation of the COARE bulk air-sea flux algorithm.
+Author-email: Andrew Scherer <scherand@oregonstate.edu>
+Maintainer-email: Andrew Scherer <scherand@oregonstate.edu>
+License: MIT License
+Project-URL: Source, https://github.com/pyCOARE/coare
+Keywords: oceanography,air-sea,bulk flux
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pyCOARE
-[![CI](https://github.com/andrew-s28/COARE-algorithm/workflows/tests/badge.svg?branch=master)](https://github.com/andrew-s28/COARE-algorithm/actions)
-[![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](ttps://github.com/andrew-s28/COARE-algorithm/blob/master/LICENSE.txt)
-[![Code coverage](https://codecov.io/gh/andrew-s28/COARE-algorithm/branch/master/graph/badge.svg)](https://app.codecov.io/gh/andrew-s28/COARE-algorithm)
+[![Tests](https://github.com/pyCOARE/coare/actions/workflows/tests.yml/badge.svg)](https://github.com/pyCOARE/coare/actions/workflows/tests.yml)
+[![License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](ttps://github.com/pyCOARE/coare/blob/master/LICENSE.txt)
+[![Code coverage](https://codecov.io/gh/pyCOARE/coare/branch/main/graph/badge.svg)](https://app.codecov.io/gh/pyCOARE/coare)
+[![Docs](https://readthedocs.org/projects/coare-live/badge/?version=latest)](https://coare-live.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://img.shields.io/pypi/v/pycoare?style=plastic)](https://pypi.org/project/pycoare/)
 
 ## COARE-algorithm
 
 This is an alpha-quality fork of the Python version of the [COARE algorithm](https://github.com/NOAA-PSL/COARE-algorithm) that was written with the goal of standardizing testing, packaging, and distribution of the algorithm. Currently only COARE v3.5 is implemented - hopefully v3.6 will come soon! 
 
-The functionality of the code is ideally the same as that for the scripts found in the NOAA PSL repository linked above. My only intended contributions are towards formatting, testing, and packaging. To that end, tests have been constructed based on the output of the original MATLAB code for COARE v3.5. [View the results of the tests](https://github.com/andrew-s28/COARE-algorithm/actions) or [download the data](https://github.com/andrew-s28/COARE-algorithm/tree/master/tests/data) and run them yourself. All results from this script agree to at least five significant figures with the MATLAB scripts in the NOAA repository, provided the testing badge above stays green. 
+The functionality of the code is ideally the same as that for the scripts found in the NOAA PSL repository linked above. My only intended contributions are towards formatting, testing, and packaging. To that end, tests have been constructed based on the output of the original MATLAB code for COARE v3.5. [View the results of the tests](https://github.com/pyCOARE/coare/actions) or [download the data](https://github.com/pyCOARE/coare/tree/main/tests/data) and run them yourself. All results from this script agree to at least five significant figures with the MATLAB scripts in the NOAA repository, provided the testing badge above stays green. 
 
 ## Installation
 
 The latest stable version (currently still an alpha) can be downloaded using Pip
 ```
 pip install pycoare
 ```
 
 You can install the most up-to-date version using 
 ```
-pip install git+https://github.com/andrew-s28/COARE-algorithm
+pip install git+https://github.com/pyCOARE/coare
 ```
 
 ## Contribution
 
-I welcome any contributions - please feel free to raise an issue or submit a pull request. My hope is that this implementation will get better as those with more knowledge on bulk air-sea fluxes or Python software development get involved. 
+I welcome any contributions - please feel free to [raise an issue](https://github.com/pyCOARE/coare/issues) or submit a [pull request](https://github.com/pyCOARE/coare/pulls).
 
-## Origins
+## Origins and Credits
 The international TOGA-COARE field program which took place in the western Pacific warm pool over 4 months from November 1992 to February 1993 ([Fairall et al. 1996a](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Fairall%20et%20al.%201996a%20-%20cool%20skin%20warm%20layer.pdf), [1996b](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Fairall%20et%20al.%201996b%20-%20bulk%20fluxes%20of%20variables.pdf) and [1997](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Fairall%20et%20al.%201997%20-%20ship%20measurements%20MABL.pdf)) spurred the development of the COARE model. The algorithm is intended to provide estimates of `momentum, sensible heat`, and `latent heat fluxes` using inputs of bulk atmospheric variables (`wind speed, SST, air temperature, air humidity`). The algorithm contains subroutines/functions to handle near-surface gradients of temperature in the ocean.
 
+This Python implementation of the COARE algorithm was initially translated from MATLAB by Byron Blomquist and Ludovic Bariteau. For more information on the people and publications that developed the COARE algorithm, see the references below.
+
 ## Versions
 - **Version 2.5** was published in 1996. 
 - **Version 3.0** was published in 2003; it was a major update from Version 2.5. This update was based on new observations at higher wind speeds (10 to 20 m/s). Available in MATLAB and FORTRAN only.
 - **Version 3.5** was released in 2013 following the publication of [Edson et al. 2013](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Edson%20et%20al.%202013%20-%20momentum%20flux.pdf), which made adjustments to the wind speed dependence of the Charnock parameter based on a large database of direct covariance stress observations (principally from a buoy). This led to an increase in stress for wind speeds greater than about 18 m/s. The roughness Reynolds number formulation of the scalar roughness length was tuned slightly to give the same values of `Ch` and `Ce` as Version 3.0. The diurnal warm layer model was structured as a separate routine instead of embedded in a driver program. COARE 3.5 was based on Edson’s buoy data ([Edson et al. 2013](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Edson%20et%20al.%202013%20-%20momentum%20flux.pdf)) and was compared to a large database (a total of 16,000 hours of observations) combining observations from NOAA, WHOI, and U. Miami ([Fairall et al. 2011](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Fairall%20et%20al.%202011%20-%20COAREG.pdf)). It is available in Python and MATLAB.
 - **Version 3.6** is slightly restructured and built around improvements in the representation of the effects of waves on fluxes. This includes improved relationships of `surface roughness`, $z_o$, and `whitecap fraction`, $W_f$, on wave parameters.  More details can be found in [coare3.6\_readme\_1.pdf](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/coare36_readme_1.pdf). This version is available in Python, MATLAB and FORTRAN.
```

### Comparing `pycoare-2023.4a4/pycoare.egg-info/PKG-INFO` & `pycoare-2023.4a5/pycoare.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 Metadata-Version: 2.1
 Name: pycoare
-Version: 2023.4a4
+Version: 2023.4a5
 Summary: A Python implementation of the COARE bulk air-sea flux algorithm.
-Author: C. W. Fairall, Byron Blomquist, Ludovic Bariteau, J. B. Edson
+Author-email: Andrew Scherer <scherand@oregonstate.edu>
 Maintainer-email: Andrew Scherer <scherand@oregonstate.edu>
 License: MIT License
-Project-URL: Source, https://github.com/andrew-s28/COARE-algorithm
+Project-URL: Source, https://github.com/pyCOARE/coare
 Keywords: oceanography,air-sea,bulk flux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyCOARE
-[![CI](https://github.com/andrew-s28/COARE-algorithm/workflows/tests/badge.svg?branch=master)](https://github.com/andrew-s28/COARE-algorithm/actions)
-[![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](ttps://github.com/andrew-s28/COARE-algorithm/blob/master/LICENSE.txt)
-[![Code coverage](https://codecov.io/gh/andrew-s28/COARE-algorithm/branch/master/graph/badge.svg)](https://app.codecov.io/gh/andrew-s28/COARE-algorithm)
+[![Tests](https://github.com/pyCOARE/coare/actions/workflows/tests.yml/badge.svg)](https://github.com/pyCOARE/coare/actions/workflows/tests.yml)
+[![License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](ttps://github.com/pyCOARE/coare/blob/master/LICENSE.txt)
+[![Code coverage](https://codecov.io/gh/pyCOARE/coare/branch/main/graph/badge.svg)](https://app.codecov.io/gh/pyCOARE/coare)
+[![Docs](https://readthedocs.org/projects/coare-live/badge/?version=latest)](https://coare-live.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://img.shields.io/pypi/v/pycoare?style=plastic)](https://pypi.org/project/pycoare/)
 
 ## COARE-algorithm
 
 This is an alpha-quality fork of the Python version of the [COARE algorithm](https://github.com/NOAA-PSL/COARE-algorithm) that was written with the goal of standardizing testing, packaging, and distribution of the algorithm. Currently only COARE v3.5 is implemented - hopefully v3.6 will come soon! 
 
-The functionality of the code is ideally the same as that for the scripts found in the NOAA PSL repository linked above. My only intended contributions are towards formatting, testing, and packaging. To that end, tests have been constructed based on the output of the original MATLAB code for COARE v3.5. [View the results of the tests](https://github.com/andrew-s28/COARE-algorithm/actions) or [download the data](https://github.com/andrew-s28/COARE-algorithm/tree/master/tests/data) and run them yourself. All results from this script agree to at least five significant figures with the MATLAB scripts in the NOAA repository, provided the testing badge above stays green. 
+The functionality of the code is ideally the same as that for the scripts found in the NOAA PSL repository linked above. My only intended contributions are towards formatting, testing, and packaging. To that end, tests have been constructed based on the output of the original MATLAB code for COARE v3.5. [View the results of the tests](https://github.com/pyCOARE/coare/actions) or [download the data](https://github.com/pyCOARE/coare/tree/main/tests/data) and run them yourself. All results from this script agree to at least five significant figures with the MATLAB scripts in the NOAA repository, provided the testing badge above stays green. 
 
 ## Installation
 
 The latest stable version (currently still an alpha) can be downloaded using Pip
 ```
 pip install pycoare
 ```
 
 You can install the most up-to-date version using 
 ```
-pip install git+https://github.com/andrew-s28/COARE-algorithm
+pip install git+https://github.com/pyCOARE/coare
 ```
 
 ## Contribution
 
-I welcome any contributions - please feel free to raise an issue or submit a pull request. My hope is that this implementation will get better as those with more knowledge on bulk air-sea fluxes or Python software development get involved. 
+I welcome any contributions - please feel free to [raise an issue](https://github.com/pyCOARE/coare/issues) or submit a [pull request](https://github.com/pyCOARE/coare/pulls).
 
-## Origins
+## Origins and Credits
 The international TOGA-COARE field program which took place in the western Pacific warm pool over 4 months from November 1992 to February 1993 ([Fairall et al. 1996a](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Fairall%20et%20al.%201996a%20-%20cool%20skin%20warm%20layer.pdf), [1996b](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Fairall%20et%20al.%201996b%20-%20bulk%20fluxes%20of%20variables.pdf) and [1997](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Fairall%20et%20al.%201997%20-%20ship%20measurements%20MABL.pdf)) spurred the development of the COARE model. The algorithm is intended to provide estimates of `momentum, sensible heat`, and `latent heat fluxes` using inputs of bulk atmospheric variables (`wind speed, SST, air temperature, air humidity`). The algorithm contains subroutines/functions to handle near-surface gradients of temperature in the ocean.
 
+This Python implementation of the COARE algorithm was initially translated from MATLAB by Byron Blomquist and Ludovic Bariteau. For more information on the people and publications that developed the COARE algorithm, see the references below.
+
 ## Versions
 - **Version 2.5** was published in 1996. 
 - **Version 3.0** was published in 2003; it was a major update from Version 2.5. This update was based on new observations at higher wind speeds (10 to 20 m/s). Available in MATLAB and FORTRAN only.
 - **Version 3.5** was released in 2013 following the publication of [Edson et al. 2013](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Edson%20et%20al.%202013%20-%20momentum%20flux.pdf), which made adjustments to the wind speed dependence of the Charnock parameter based on a large database of direct covariance stress observations (principally from a buoy). This led to an increase in stress for wind speeds greater than about 18 m/s. The roughness Reynolds number formulation of the scalar roughness length was tuned slightly to give the same values of `Ch` and `Ce` as Version 3.0. The diurnal warm layer model was structured as a separate routine instead of embedded in a driver program. COARE 3.5 was based on Edson’s buoy data ([Edson et al. 2013](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Edson%20et%20al.%202013%20-%20momentum%20flux.pdf)) and was compared to a large database (a total of 16,000 hours of observations) combining observations from NOAA, WHOI, and U. Miami ([Fairall et al. 2011](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/Fairall%20et%20al.%202011%20-%20COAREG.pdf)). It is available in Python and MATLAB.
 - **Version 3.6** is slightly restructured and built around improvements in the representation of the effects of waves on fluxes. This includes improved relationships of `surface roughness`, $z_o$, and `whitecap fraction`, $W_f$, on wave parameters.  More details can be found in [coare3.6\_readme\_1.pdf](https://github.com/noaa-psd/COARE-algorithm/blob/master/References/coare36_readme_1.pdf). This version is available in Python, MATLAB and FORTRAN.
```

### Comparing `pycoare-2023.4a4/pyproject.toml` & `pycoare-2023.4a5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pycoare"
 authors = [
-    {name = 'C. W. Fairall'},
-    {name = 'Byron Blomquist'},
-    {name = 'Ludovic Bariteau'},
-    {name = 'J. B. Edson'}
+    {name = 'Andrew Scherer', email = 'scherand@oregonstate.edu'}
 ]
 maintainers = [
     {name = 'Andrew Scherer', email = 'scherand@oregonstate.edu'}
 ]
-version = "2023.4a4"
+version = "2023.4a5"
 description = 'A Python implementation of the COARE bulk air-sea flux algorithm.'
 readme = {file = 'README.md', content-type = 'text/markdown'}
 requires-python = ">=3.7"
 keywords = ['oceanography', 'air-sea', 'bulk flux']
 license = {text = "MIT License"}
 classifiers = [
     'Development Status :: 3 - Alpha',
@@ -27,11 +24,11 @@
     'Topic :: Scientific/Engineering',
     'Intended Audience :: Science/Research'
 ]
 dependencies = ['numpy']
 
 [project.urls]
 
-Source = 'https://github.com/andrew-s28/COARE-algorithm'
+Source = 'https://github.com/pyCOARE/coare'
```

### Comparing `pycoare-2023.4a4/tests/test_coare.py` & `pycoare-2023.4a5/tests/test_coare.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,26 +32,26 @@
     from pycoare.coare import c35
     input_data = pd.read_csv(
         os.path.join(
             os.path.dirname(__file__), 'data/test_35_data_input_final.csv'
             )
         ).to_dict(orient='list')
 
-    actual = c35(**input_data, out='full')
+    actual = c35(**input_data, out='default')
     expected = pd.read_csv(
         os.path.join(
             os.path.dirname(__file__), 'data/test_35_data_output_final.csv'
             )
         ).to_numpy()
 
     np.testing.assert_allclose(actual, expected, atol=0, rtol=10**-5)
 
 
 def test_rhcalc():
-    from pycoare.coare import rhcalc
+    from pycoare.util import rhcalc
     input_data = mat_to_df(
         os.path.join(
             os.path.dirname(__file__), 'data/rh_calcs_input.mat'
             )
     )
 
     actual = rhcalc(**input_data)
@@ -62,15 +62,15 @@
     )
 
     np.testing.assert_allclose(actual, expected.values.flatten(),
                                atol=0, rtol=10**-5)
 
 
 def test_psi():
-    from pycoare.coare import psit_26, psiu_26, psiu_40
+    from pycoare.util import psit_26, psiu_26, psiu_40
     input_data = mat_to_df(
         os.path.join(
             os.path.dirname(__file__), 'data/psi_calcs_data.mat'
             )
     )
 
     actual = psit_26(input_data.zet)
@@ -83,15 +83,15 @@
 
     actual = psiu_40(input_data.zet)
     expected = input_data.psiu_40_out.values
     np.testing.assert_allclose(actual, expected, atol=0, rtol=10**-5)
 
 
 def test_qsat():
-    from pycoare.coare import qsat, qsea, qair
+    from pycoare.util import qsat, qsea, qair
     input_data = mat_to_df(
         os.path.join(
             os.path.dirname(__file__), 'data/qsat_calcs_input.mat'
             )
     )
 
     output_data = mat_to_df(
@@ -110,13 +110,13 @@
 
     actual = qair(**input_data)[0]
     expected = output_data.qsat_air.values
     np.testing.assert_allclose(actual, expected, atol=0, rtol=10**-5)
 
 
 def test_find():
-    from pycoare.coare import find
+    from pycoare.util import find
     input_data = np.arange(-100, 100)
     condition = input_data > 0
     actual = find(condition)
     expected = np.arange(101, 200)
     np.testing.assert_equal(actual, expected)
```

