# Comparing `tmp/solarmach-0.3.4.tar.gz` & `tmp/solarmach-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarmach-0.3.4.tar", last modified: Wed Apr 24 15:08:11 2024, max compression
+gzip compressed data, was "solarmach-0.4.0.tar", last modified: Thu May 30 12:11:28 2024, max compression
```

## Comparing `solarmach-0.3.4.tar` & `solarmach-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-04-24 15:08:11.311487 solarmach-0.3.4/
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.3.4/LICENSE.rst
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      457 2022-01-10 16:26:49.000000 solarmach-0.3.4/MANIFEST.in
--rw-r--r--   0 jagies    (1000) jagies    (1000)     8273 2024-04-24 15:08:11.311487 solarmach-0.3.4/PKG-INFO
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     6505 2024-03-25 08:09:12.000000 solarmach-0.3.4/README.rst
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     3370 2022-03-30 15:50:45.000000 solarmach-0.3.4/code_of_conduct.md
-drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-04-24 15:08:11.307487 solarmach-0.3.4/docs/
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      634 2023-07-25 12:11:02.000000 solarmach-0.3.4/docs/Makefile
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     1281 2024-03-25 08:09:12.000000 solarmach-0.3.4/docs/conf.py
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     2356 2024-03-25 08:09:12.000000 solarmach-0.3.4/docs/index.rst
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      324 2024-03-25 08:09:12.000000 solarmach-0.3.4/docs/installation.rst
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      800 2024-03-25 08:09:12.000000 solarmach-0.3.4/docs/make.bat
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      103 2024-03-25 08:09:12.000000 solarmach-0.3.4/docs/requirements.txt
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      220 2024-03-25 08:09:12.000000 solarmach-0.3.4/docs/solarmach.rst
--rw-rw-r--   0 jagies    (1000) jagies    (1000)       43 2024-03-25 08:09:12.000000 solarmach-0.3.4/docs/usage.nblink
-drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-04-24 15:08:11.307487 solarmach-0.3.4/examples/
--rw-rw-r--   0 jagies    (1000) jagies    (1000)  4699075 2024-03-25 08:09:12.000000 solarmach-0.3.4/examples/example.ipynb
--rw-rw-r--   0 jagies    (1000) jagies    (1000)   348683 2022-03-14 16:09:27.000000 solarmach-0.3.4/examples/solarmach.png
-drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-04-24 15:08:11.307487 solarmach-0.3.4/licenses/
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.3.4/licenses/LICENSE.rst
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     1659 2022-01-10 16:26:49.000000 solarmach-0.3.4/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      133 2024-03-25 08:09:12.000000 solarmach-0.3.4/pyproject.toml
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      192 2024-03-25 08:09:12.000000 solarmach-0.3.4/requirements.txt
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     2255 2024-04-24 15:08:11.311487 solarmach-0.3.4/setup.cfg
--rwxrwxr-x   0 jagies    (1000) jagies    (1000)      660 2022-03-14 12:48:51.000000 solarmach-0.3.4/setup.py
-drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-04-24 15:08:11.311487 solarmach-0.3.4/solarmach/
--rw-rw-r--   0 jagies    (1000) jagies    (1000)   104676 2024-04-24 13:54:06.000000 solarmach-0.3.4/solarmach/__init__.py
--rw-rw-r--   0 jagies    (1000) jagies    (1000)    24330 2024-03-25 08:09:12.000000 solarmach-0.3.4/solarmach/pfss_utilities.py
-drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-04-24 15:08:11.311487 solarmach-0.3.4/solarmach/tests/
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      108 2022-01-10 16:26:49.000000 solarmach-0.3.4/solarmach/tests/__init__.py
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      230 2024-04-24 15:00:51.000000 solarmach-0.3.4/solarmach/tests/figure_hashes_mpl_353.json
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     6605 2024-04-24 13:56:25.000000 solarmach-0.3.4/solarmach/tests/test.py
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      345 2024-04-24 15:08:11.000000 solarmach-0.3.4/solarmach/version.py
-drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-04-24 15:08:11.311487 solarmach-0.3.4/solarmach.egg-info/
--rw-r--r--   0 jagies    (1000) jagies    (1000)     8273 2024-04-24 15:08:11.000000 solarmach-0.3.4/solarmach.egg-info/PKG-INFO
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      708 2024-04-24 15:08:11.000000 solarmach-0.3.4/solarmach.egg-info/SOURCES.txt
--rw-rw-r--   0 jagies    (1000) jagies    (1000)        1 2024-04-24 15:08:11.000000 solarmach-0.3.4/solarmach.egg-info/dependency_links.txt
--rw-rw-r--   0 jagies    (1000) jagies    (1000)        1 2022-03-17 17:20:48.000000 solarmach-0.3.4/solarmach.egg-info/not-zip-safe
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      274 2024-04-24 15:08:11.000000 solarmach-0.3.4/solarmach.egg-info/requires.txt
--rw-rw-r--   0 jagies    (1000) jagies    (1000)       10 2024-04-24 15:08:11.000000 solarmach-0.3.4/solarmach.egg-info/top_level.txt
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     1305 2024-03-25 08:09:12.000000 solarmach-0.3.4/tox.ini
+drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-05-30 12:11:28.100852 solarmach-0.4.0/
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.4.0/LICENSE.rst
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      457 2022-01-10 16:26:49.000000 solarmach-0.4.0/MANIFEST.in
+-rw-r--r--   0 jagies    (1000) jagies    (1000)     8296 2024-05-30 12:11:28.100852 solarmach-0.4.0/PKG-INFO
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     6506 2024-05-30 09:05:15.000000 solarmach-0.4.0/README.rst
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     3370 2022-03-30 15:50:45.000000 solarmach-0.4.0/code_of_conduct.md
+drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-05-30 12:11:28.096852 solarmach-0.4.0/docs/
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      634 2023-07-25 12:11:02.000000 solarmach-0.4.0/docs/Makefile
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     1281 2024-03-25 08:09:12.000000 solarmach-0.4.0/docs/conf.py
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     2188 2024-05-30 09:01:55.000000 solarmach-0.4.0/docs/index.rst
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      325 2024-05-30 09:05:35.000000 solarmach-0.4.0/docs/installation.rst
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      800 2024-03-25 08:09:12.000000 solarmach-0.4.0/docs/make.bat
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      103 2024-03-25 08:09:12.000000 solarmach-0.4.0/docs/requirements.txt
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      220 2024-03-25 08:09:12.000000 solarmach-0.4.0/docs/solarmach.rst
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)       43 2024-03-25 08:09:12.000000 solarmach-0.4.0/docs/usage.nblink
+drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-05-30 12:11:28.100852 solarmach-0.4.0/examples/
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)  4699075 2024-03-25 08:09:12.000000 solarmach-0.4.0/examples/example.ipynb
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)   348683 2022-03-14 16:09:27.000000 solarmach-0.4.0/examples/solarmach.png
+drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-05-30 12:11:28.100852 solarmach-0.4.0/licenses/
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.4.0/licenses/LICENSE.rst
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     1659 2022-01-10 16:26:49.000000 solarmach-0.4.0/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      133 2024-03-25 08:09:12.000000 solarmach-0.4.0/pyproject.toml
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      156 2024-05-30 11:57:42.000000 solarmach-0.4.0/requirements.txt
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     2228 2024-05-30 12:11:28.104852 solarmach-0.4.0/setup.cfg
+-rwxrwxr-x   0 jagies    (1000) jagies    (1000)      660 2022-03-14 12:48:51.000000 solarmach-0.4.0/setup.py
+drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-05-30 12:11:28.100852 solarmach-0.4.0/solarmach/
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)   104833 2024-05-21 12:52:09.000000 solarmach-0.4.0/solarmach/__init__.py
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)    24292 2024-05-30 08:59:42.000000 solarmach-0.4.0/solarmach/pfss_utilities.py
+drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-05-30 12:11:28.100852 solarmach-0.4.0/solarmach/tests/
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      108 2022-01-10 16:26:49.000000 solarmach-0.4.0/solarmach/tests/__init__.py
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      230 2024-05-30 09:21:16.000000 solarmach-0.4.0/solarmach/tests/figure_hashes_mpl_390.json
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     6574 2024-05-30 09:28:49.000000 solarmach-0.4.0/solarmach/tests/test.py
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      345 2024-05-30 12:11:28.000000 solarmach-0.4.0/solarmach/version.py
+drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-05-30 12:11:28.100852 solarmach-0.4.0/solarmach.egg-info/
+-rw-r--r--   0 jagies    (1000) jagies    (1000)     8296 2024-05-30 12:11:28.000000 solarmach-0.4.0/solarmach.egg-info/PKG-INFO
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      708 2024-05-30 12:11:28.000000 solarmach-0.4.0/solarmach.egg-info/SOURCES.txt
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)        1 2024-05-30 12:11:28.000000 solarmach-0.4.0/solarmach.egg-info/dependency_links.txt
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)        1 2022-03-17 17:20:48.000000 solarmach-0.4.0/solarmach.egg-info/not-zip-safe
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      278 2024-05-30 12:11:28.000000 solarmach-0.4.0/solarmach.egg-info/requires.txt
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)       10 2024-05-30 12:11:28.000000 solarmach-0.4.0/solarmach.egg-info/top_level.txt
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     1307 2024-05-30 09:08:00.000000 solarmach-0.4.0/tox.ini
```

### Comparing `solarmach-0.3.4/LICENSE.rst` & `solarmach-0.4.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.4/PKG-INFO` & `solarmach-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: solarmach
-Version: 0.3.4
+Version: 0.4.0
 Summary: Multi-spacecraft longitudinal configuration plotter
 Home-page: https://github.com/jgieseler/solarmach
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Project-URL: Documentation, https://solarmach.readthedocs.io
 Project-URL: Changelog, https://github.com/jgieseler/solarmach/releases
 Project-URL: Issue Tracker, https://github.com/jgieseler/solarmach/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 License-File: licenses/LICENSE.rst
 Requires-Dist: astropy
-Requires-Dist: astroquery
 Requires-Dist: cmasher
 Requires-Dist: drms
 Requires-Dist: imageio>=2.31.6
 Requires-Dist: Jinja2
 Requires-Dist: lxml
-Requires-Dist: matplotlib==3.5.3
+Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: pfsspy
 Requires-Dist: plotly
 Requires-Dist: python-dateutil
 Requires-Dist: scipy
-Requires-Dist: speasy>=1.2.0
+Requires-Dist: setuptools
+Requires-Dist: speasy>=1.2.7
+Requires-Dist: sunkit_magex
 Requires-Dist: sunpy
+Requires-Dist: tqdm
 Requires-Dist: zeep
 Provides-Extra: all
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-doctestplus; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mpl; extra == "test"
@@ -72,15 +73,15 @@
 
 
 The Solar MAgnetic Connection Haus (Solar-MACH) tool is a multi-spacecraft longitudinal configuration plotter. This is the repository of the pip/conda package of Solar-MACH, called **solarmach**. For the corresponding streamlit repository, which is used for `solar-mach.github.io <https://solar-mach.github.io>`_, see `github.com/jgieseler/Solar-MACH <https://github.com/jgieseler/Solar-MACH>`_.
 
 Installation
 ------------
 
-solarmach requires python >= 3.8.
+solarmach requires python >= 3.10.
 
 It can be installed either from `PyPI <https://pypi.org/project/solarmach/>`_ using:
 
 .. code:: bash
 
     pip install solarmach
```

### Comparing `solarmach-0.3.4/README.rst` & `solarmach-0.4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 The Solar MAgnetic Connection Haus (Solar-MACH) tool is a multi-spacecraft longitudinal configuration plotter. This is the repository of the pip/conda package of Solar-MACH, called **solarmach**. For the corresponding streamlit repository, which is used for `solar-mach.github.io <https://solar-mach.github.io>`_, see `github.com/jgieseler/Solar-MACH <https://github.com/jgieseler/Solar-MACH>`_.
 
 Installation
 ------------
 
-solarmach requires python >= 3.8.
+solarmach requires python >= 3.10.
 
 It can be installed either from `PyPI <https://pypi.org/project/solarmach/>`_ using:
 
 .. code:: bash
 
     pip install solarmach
```

### Comparing `solarmach-0.3.4/code_of_conduct.md` & `solarmach-0.4.0/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.4/docs/Makefile` & `solarmach-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.4/docs/conf.py` & `solarmach-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.4/docs/index.rst` & `solarmach-0.4.0/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -36,21 +36,18 @@
 Acknowledgements
 ----------------
  
 The Solar-MACH tool was originally developed at Kiel University, Germany and further discussed within the `ESA Heliophysics Archives USer (HAUS) <https://www.cosmos.esa.int/web/esdc/archives-user-groups/heliophysics>`_ group.
 
 This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 101004159.
 
-Powered by: |matplotlib| |sunpy| |speasy| |pfsspy|
+Powered by: |matplotlib| |sunpy| |speasy|
 
 .. |matplotlib| image:: https://matplotlib.org/_static/logo_dark.svg
    :width: 15%
    :target: https://matplotlib.org
 .. |sunpy| image:: https://raw.githubusercontent.com/sunpy/sunpy-logo/master/generated/sunpy_logo_landscape.svg
    :width: 15%
    :target: https://sunpy.org
 .. |speasy| image:: https://raw.githubusercontent.com/SciQLop/speasy/main/logo/logo_speasy.svg
    :width: 15%
    :target: https://pypi.org/project/speasy/
-.. |pfsspy| image:: https://raw.githubusercontent.com/dstansby/pfsspy/main/logo/logo_rectangle.png
-   :width: 15%
-   :target: https://pypi.org/project/pfsspy/
```

### Comparing `solarmach-0.3.4/docs/make.bat` & `solarmach-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.4/examples/example.ipynb` & `solarmach-0.4.0/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.4/examples/solarmach.png` & `solarmach-0.4.0/examples/solarmach.png`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.4/licenses/LICENSE.rst` & `solarmach-0.4.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.4/licenses/TEMPLATE_LICENSE.rst` & `solarmach-0.4.0/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.4/setup.cfg` & `solarmach-0.4.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -13,42 +13,43 @@
 	Issue Tracker = https://github.com/jgieseler/solarmach/issues
 classifiers = 
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 zip_safe = False
 packages = find:
 include_package_data = True
-python_requires = >=3.8
+python_requires = >=3.10
 setup_requires = setuptools_scm
 install_requires = 
 	astropy
-	astroquery
 	cmasher
 	drms
 	imageio>=2.31.6
 	Jinja2
 	lxml
-	matplotlib==3.5.3
+	matplotlib
 	numpy
 	pandas
-	pfsspy  # TODO: replace with sunkit_magex
 	plotly
 	python-dateutil
 	scipy
-	speasy>=1.2.0
+	setuptools
+	speasy>=1.2.7
+	sunkit_magex
 	sunpy
+	tqdm
 	zeep
 
 [options.extras_require]
 all = 
 test = 
 	pytest
 	pytest-doctestplus
```

### Comparing `solarmach-0.3.4/setup.py` & `solarmach-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.4/solarmach/__init__.py` & `solarmach-0.4.0/solarmach/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -703,16 +703,17 @@
                                margin=dict(l=100, r=100, b=0, t=50),
                                # paper_bgcolor="LightSteelBlue",
                                legend=dict(yanchor="middle", y=test_plotly_legend[1], xanchor="center", x=test_plotly_legend[0]))
             # fig.show()
             # if using streamlit, send plot to streamlit output, else call plt.show()
             if _isstreamlit():
                 import streamlit as st
+                import streamlit.components.v1 as components
                 # st.plotly_chart(pfig, theme="streamlit")
-                st.components.v1.html(pfig.to_html(include_mathjax='cdn'), height=500)
+                components.html(pfig.to_html(include_mathjax='cdn'), height=500)
             else:
                 pfig.show()
 
         if long_sector is not None:
             if type(long_sector) == list and np.array(long_sector).ndim==1:
                 long_sector = [long_sector]
                 long_sector_vsw = [long_sector_vsw]
@@ -1836,16 +1837,17 @@
                                      z=np.zeros((100, 100)),
                                      hoverinfo='skip',
                                      colorscale='gray', showscale=False, opacity=0.2))
 
         if _isstreamlit():
             fig.update_layout(width=700, height=700)
             import streamlit as st
+            import streamlit.components.v1 as components
             # st.plotly_chart(pfig, theme="streamlit")
-            st.components.v1.html(fig.to_html(include_mathjax='cdn'), height=700)
+            components.html(fig.to_html(include_mathjax='cdn'), height=700)
         else:
             fig.show()
 
         return
 
     def plot_3d(self,
                 plot_spirals=True,
@@ -2017,16 +2019,17 @@
                                      z=np.zeros((100, 100)),
                                      hoverinfo='skip',
                                      colorscale='gray', showscale=False, opacity=0.2))
 
         if _isstreamlit():
             fig.update_layout(width=700, height=700)
             import streamlit as st
+            import streamlit.components.v1 as components
             # st.plotly_chart(pfig, theme="streamlit")
-            st.components.v1.html(fig.to_html(include_mathjax='cdn'), height=700)
+            components.html(fig.to_html(include_mathjax='cdn'), height=700)
         else:
             fig.show()
 
         return
 
 
 def sc_distance(sc1, sc2, dtime):
```

### Comparing `solarmach-0.3.4/solarmach/pfss_utilities.py` & `solarmach-0.4.0/solarmach/pfss_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import os
 import pickle
 
 import astropy.constants as aconst
 import astropy.units as u
 import matplotlib.pyplot as plt
 import numpy as np
-import pfsspy  # TODO: replace with "import sunkit_magex.pfss as pfsspy"
+import sunkit_magex.pfss as pfsspy
 import sunpy.map
 from astropy.coordinates import SkyCoord
 from sunpy.net import Fido
 from sunpy.net import attrs as a
 
 
 # @st_cache_decorator
```

### Comparing `solarmach-0.3.4/solarmach/tests/test.py` & `solarmach-0.4.0/solarmach/tests/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import astropy
 import astropy.units as u
 import datetime as dt
 import matplotlib
 import numpy as np
 import pandas
-import pfsspy
+import sunkit_magex.pfss as pfsspy
 import pytest
 import sunpy
 from pathlib import Path
 from solarmach import SolarMACH, print_body_list, get_gong_map, calculate_pfss_solution, sc_distance, get_sw_speed
 
 
 def test_print_body_list():
@@ -93,19 +93,19 @@
     # check SolarMACH
     with pytest.raises(ValueError):
         sm = SolarMACH(date=date, body_list=body_list, coord_sys='Stonyhurst')
 
 
 """
 Create/update hash library for the following matplotlib tests by running for example the following command from the base package dir:
-tox -e py310-test -- --mpl-generate-hash-library=solarmach/tests/figure_hashes_mpl_353.json --mpl-deterministic
+tox -e py310-test -- --mpl-generate-hash-library=solarmach/tests/figure_hashes_mpl_390.json --mpl-deterministic
 """
 
 
-@pytest.mark.mpl_image_compare(hash_library=Path(__file__).parent / 'figure_hashes_mpl_353.json', deterministic=True)
+@pytest.mark.mpl_image_compare(hash_library=Path(__file__).parent / 'figure_hashes_mpl_390.json', deterministic=True)
 def test_solarmach_plot():
     body_list = ['STEREO-A']
     vsw_list = [400]
     date = '2021-10-28 15:15:00'
     reference_long = 273
     reference_lat = 9
     reference_vsw = 400
@@ -121,22 +121,22 @@
                       show_earth_centered_coord=False, markers='numbers',
                       long_sector=long_sector, long_sector_vsw=long_sector_vsw, long_sector_color=long_sector_color,
                       background_spirals=background_spirals, outfile=filename, return_plot_object=True)
     assert os.path.exists(os.getcwd()+os.sep+filename)
     return fig
 
 
-@pytest.mark.mpl_image_compare(hash_library=Path(__file__).parent / 'figure_hashes_mpl_353.json', deterministic=True)
+@pytest.mark.mpl_image_compare(hash_library=Path(__file__).parent / 'figure_hashes_mpl_390.json', deterministic=True)
 def test_solarmach_pfss():
     date = '2021-4-1 1:00:00'
     body_list = ['Earth', 'STEREO-A']
     vsw_list = [400, 400]   # position-sensitive solar wind speed per body in body_list
     sm = SolarMACH(date, body_list, vsw_list, reference_long=100, reference_lat=10, coord_sys='Carrington')
     gong_map = get_gong_map(time=date, filepath=None)
-    assert isinstance(gong_map, pfsspy.map.GongSynopticMap) or isinstance(gong_map, sunpy.map.sources.gong.GONGSynopticMap)
+    assert isinstance(gong_map, sunpy.map.sources.gong.GONGSynopticMap)
     pfss_solution = calculate_pfss_solution(gong_map=gong_map, rss=2.5, coord_sys='Carrington')
     assert isinstance(pfss_solution, pfsspy.output.Output)
     fig, ax = sm.plot_pfss(rss=2.5, pfss_solution=pfss_solution, vary=True, return_plot_object=True,
                            markers='numbers', long_sector=[290, 328], long_sector_vsw=[400, 600],
                            long_sector_color='red', reference_vsw=400.0)
     assert isinstance(fig, matplotlib.figure.Figure)
     return fig
```

### Comparing `solarmach-0.3.4/solarmach.egg-info/PKG-INFO` & `solarmach-0.4.0/solarmach.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: solarmach
-Version: 0.3.4
+Version: 0.4.0
 Summary: Multi-spacecraft longitudinal configuration plotter
 Home-page: https://github.com/jgieseler/solarmach
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Project-URL: Documentation, https://solarmach.readthedocs.io
 Project-URL: Changelog, https://github.com/jgieseler/solarmach/releases
 Project-URL: Issue Tracker, https://github.com/jgieseler/solarmach/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 License-File: licenses/LICENSE.rst
 Requires-Dist: astropy
-Requires-Dist: astroquery
 Requires-Dist: cmasher
 Requires-Dist: drms
 Requires-Dist: imageio>=2.31.6
 Requires-Dist: Jinja2
 Requires-Dist: lxml
-Requires-Dist: matplotlib==3.5.3
+Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: pfsspy
 Requires-Dist: plotly
 Requires-Dist: python-dateutil
 Requires-Dist: scipy
-Requires-Dist: speasy>=1.2.0
+Requires-Dist: setuptools
+Requires-Dist: speasy>=1.2.7
+Requires-Dist: sunkit_magex
 Requires-Dist: sunpy
+Requires-Dist: tqdm
 Requires-Dist: zeep
 Provides-Extra: all
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-doctestplus; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mpl; extra == "test"
@@ -72,15 +73,15 @@
 
 
 The Solar MAgnetic Connection Haus (Solar-MACH) tool is a multi-spacecraft longitudinal configuration plotter. This is the repository of the pip/conda package of Solar-MACH, called **solarmach**. For the corresponding streamlit repository, which is used for `solar-mach.github.io <https://solar-mach.github.io>`_, see `github.com/jgieseler/Solar-MACH <https://github.com/jgieseler/Solar-MACH>`_.
 
 Installation
 ------------
 
-solarmach requires python >= 3.8.
+solarmach requires python >= 3.10.
 
 It can be installed either from `PyPI <https://pypi.org/project/solarmach/>`_ using:
 
 .. code:: bash
 
     pip install solarmach
```

### Comparing `solarmach-0.3.4/solarmach.egg-info/SOURCES.txt` & `solarmach-0.4.0/solarmach.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 solarmach.egg-info/PKG-INFO
 solarmach.egg-info/SOURCES.txt
 solarmach.egg-info/dependency_links.txt
 solarmach.egg-info/not-zip-safe
 solarmach.egg-info/requires.txt
 solarmach.egg-info/top_level.txt
 solarmach/tests/__init__.py
-solarmach/tests/figure_hashes_mpl_353.json
+solarmach/tests/figure_hashes_mpl_390.json
 solarmach/tests/test.py
```

### Comparing `solarmach-0.3.4/tox.ini` & `solarmach-0.4.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 envlist =
-    py{38,39,310}-test
+    py{310,311,312}-test
     build_docs
     codestyle
 isolated_build = true
 # This is included for testing of the template. You can remove it safely.
 skip_missing_interpreters = True
 
 [testenv]
```

