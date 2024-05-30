# Comparing `tmp/datawaza-0.1.2.tar.gz` & `tmp/datawaza-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawaza-0.1.2.tar", last modified: Wed Mar 20 06:46:46 2024, max compression
+gzip compressed data, was "datawaza-0.1.3.tar", last modified: Thu May 30 10:02:47 2024, max compression
```

## Comparing `datawaza-0.1.2.tar` & `datawaza-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2024-03-20 06:46:46.718453 datawaza-0.1.2/
--rw-r--r--   0 jim        (501) staff       (20)    35149 2024-01-24 04:34:45.000000 datawaza-0.1.2/LICENSE
--rw-r--r--   0 jim        (501) staff       (20)    12292 2024-03-20 06:46:46.717971 datawaza-0.1.2/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)     9909 2024-03-20 06:37:32.000000 datawaza-0.1.2/README.md
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2024-03-20 06:46:46.696256 datawaza-0.1.2/datawaza/
--rw-r--r--   0 jim        (501) staff       (20)     2345 2024-03-20 02:57:09.000000 datawaza-0.1.2/datawaza/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)    38611 2024-03-20 05:22:03.000000 datawaza-0.1.2/datawaza/clean.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2024-03-20 06:46:46.714445 datawaza-0.1.2/datawaza/data/
--rw-rw----   0 jim        (501) staff       (20)        5 2019-04-15 15:15:56.000000 datawaza-0.1.2/datawaza/data/cb_2018_us_county_5m.cpg
--rw-rw----   0 jim        (501) staff       (20)   527301 2019-04-15 15:15:58.000000 datawaza-0.1.2/datawaza/data/cb_2018_us_county_5m.dbf
--rw-rw----   0 jim        (501) staff       (20)      165 2019-04-15 15:15:56.000000 datawaza-0.1.2/datawaza/data/cb_2018_us_county_5m.prj
--rw-rw----   0 jim        (501) staff       (20)  3674580 2019-04-15 15:15:58.000000 datawaza-0.1.2/datawaza/data/cb_2018_us_county_5m.shp
--rwxrwxrwx   0 jim        (501) staff       (20)    21754 2019-04-15 15:17:33.000000 datawaza-0.1.2/datawaza/data/cb_2018_us_county_5m.shp.ea.iso.xml
--rwxrwxrwx   0 jim        (501) staff       (20)    35636 2019-04-15 15:17:32.000000 datawaza-0.1.2/datawaza/data/cb_2018_us_county_5m.shp.iso.xml
--rw-rw----   0 jim        (501) staff       (20)    25964 2019-04-15 15:15:58.000000 datawaza-0.1.2/datawaza/data/cb_2018_us_county_5m.shx
--rw-r--r--   0 jim        (501) staff       (20)    58834 2024-03-20 05:22:03.000000 datawaza-0.1.2/datawaza/explore.py
--rw-r--r--   0 jim        (501) staff       (20)    60032 2024-03-20 05:22:03.000000 datawaza-0.1.2/datawaza/model.py
--rw-r--r--   0 jim        (501) staff       (20)    42650 2024-03-20 05:22:03.000000 datawaza-0.1.2/datawaza/tools.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2024-03-20 06:46:46.715324 datawaza-0.1.2/datawaza.egg-info/
--rw-r--r--   0 jim        (501) staff       (20)    12292 2024-03-20 06:46:46.000000 datawaza-0.1.2/datawaza.egg-info/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)      572 2024-03-20 06:46:46.000000 datawaza-0.1.2/datawaza.egg-info/SOURCES.txt
--rw-r--r--   0 jim        (501) staff       (20)        1 2024-03-20 06:46:46.000000 datawaza-0.1.2/datawaza.egg-info/dependency_links.txt
--rw-r--r--   0 jim        (501) staff       (20)      619 2024-03-20 06:46:46.000000 datawaza-0.1.2/datawaza.egg-info/requires.txt
--rw-r--r--   0 jim        (501) staff       (20)        9 2024-03-20 06:46:46.000000 datawaza-0.1.2/datawaza.egg-info/top_level.txt
--rw-r--r--   0 jim        (501) staff       (20)       38 2024-03-20 06:46:46.718552 datawaza-0.1.2/setup.cfg
--rw-r--r--   0 jim        (501) staff       (20)     2699 2024-03-20 05:22:03.000000 datawaza-0.1.2/setup.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2024-05-30 10:02:47.079028 datawaza-0.1.3/
+-rw-r--r--   0 jim        (501) staff       (20)    35149 2024-01-24 04:34:45.000000 datawaza-0.1.3/LICENSE
+-rw-r--r--   0 jim        (501) staff       (20)    16650 2024-05-30 10:02:47.077808 datawaza-0.1.3/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)    14133 2024-05-30 04:50:49.000000 datawaza-0.1.3/README.md
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2024-05-30 10:02:47.030680 datawaza-0.1.3/datawaza/
+-rw-r--r--   0 jim        (501) staff       (20)     2703 2024-05-29 22:39:59.000000 datawaza-0.1.3/datawaza/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)    38611 2024-03-20 07:41:07.000000 datawaza-0.1.3/datawaza/clean.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2024-05-30 10:02:47.067883 datawaza-0.1.3/datawaza/data/
+-rw-rw----   0 jim        (501) staff       (20)        5 2019-04-15 15:15:56.000000 datawaza-0.1.3/datawaza/data/cb_2018_us_county_5m.cpg
+-rw-rw----   0 jim        (501) staff       (20)   527301 2019-04-15 15:15:58.000000 datawaza-0.1.3/datawaza/data/cb_2018_us_county_5m.dbf
+-rw-rw----   0 jim        (501) staff       (20)      165 2019-04-15 15:15:56.000000 datawaza-0.1.3/datawaza/data/cb_2018_us_county_5m.prj
+-rw-rw----   0 jim        (501) staff       (20)  3674580 2019-04-15 15:15:58.000000 datawaza-0.1.3/datawaza/data/cb_2018_us_county_5m.shp
+-rwxrwxrwx   0 jim        (501) staff       (20)    21754 2019-04-15 15:17:33.000000 datawaza-0.1.3/datawaza/data/cb_2018_us_county_5m.shp.ea.iso.xml
+-rwxrwxrwx   0 jim        (501) staff       (20)    35636 2019-04-15 15:17:32.000000 datawaza-0.1.3/datawaza/data/cb_2018_us_county_5m.shp.iso.xml
+-rw-rw----   0 jim        (501) staff       (20)    25964 2019-04-15 15:15:58.000000 datawaza-0.1.3/datawaza/data/cb_2018_us_county_5m.shx
+-rw-r--r--   0 jim        (501) staff       (20)  3137364 2024-05-29 21:38:50.000000 datawaza-0.1.3/datawaza/data/mnist_28x28_ch1_x0.pt
+-rw-r--r--   0 jim        (501) staff       (20)  1230169 2024-05-29 21:57:28.000000 datawaza-0.1.3/datawaza/data/svhn_32x32_ch3_x0.pt
+-rw-r--r--   0 jim        (501) staff       (20)  1230189 2024-05-29 21:57:28.000000 datawaza-0.1.3/datawaza/data/svhn_32x32_ch3_xhat0.pt
+-rw-r--r--   0 jim        (501) staff       (20)    91822 2024-05-30 01:28:49.000000 datawaza-0.1.3/datawaza/explore.py
+-rw-r--r--   0 jim        (501) staff       (20)   199592 2024-05-30 09:27:55.000000 datawaza-0.1.3/datawaza/model.py
+-rw-r--r--   0 jim        (501) staff       (20)    51349 2024-04-10 02:18:07.000000 datawaza-0.1.3/datawaza/tools.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2024-05-30 10:02:47.073699 datawaza-0.1.3/datawaza.egg-info/
+-rw-r--r--   0 jim        (501) staff       (20)    16650 2024-05-30 10:02:46.000000 datawaza-0.1.3/datawaza.egg-info/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)      681 2024-05-30 10:02:46.000000 datawaza-0.1.3/datawaza.egg-info/SOURCES.txt
+-rw-r--r--   0 jim        (501) staff       (20)        1 2024-05-30 10:02:46.000000 datawaza-0.1.3/datawaza.egg-info/dependency_links.txt
+-rw-r--r--   0 jim        (501) staff       (20)      600 2024-05-30 10:02:46.000000 datawaza-0.1.3/datawaza.egg-info/requires.txt
+-rw-r--r--   0 jim        (501) staff       (20)        9 2024-05-30 10:02:46.000000 datawaza-0.1.3/datawaza.egg-info/top_level.txt
+-rw-r--r--   0 jim        (501) staff       (20)       38 2024-05-30 10:02:47.079194 datawaza-0.1.3/setup.cfg
+-rw-r--r--   0 jim        (501) staff       (20)     2884 2024-05-30 10:01:42.000000 datawaza-0.1.3/setup.py
```

### Comparing `datawaza-0.1.2/LICENSE` & `datawaza-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datawaza-0.1.2/PKG-INFO` & `datawaza-0.1.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,7 @@
-Metadata-Version: 2.1
-Name: datawaza
-Version: 0.1.2
-Summary: Datawaza is a collection of tools for data exploration, visualization, data cleaning, pipeline creation, model iteration, and evaluation.
-Home-page: https://datawaza.com
-Author: Jim Beno
-Author-email: jim@jimbeno.net
-Project-URL: Documentation, https://datawaza.com
-Project-URL: Source, https://github.com/jbeno/datawaza
-Keywords: data science,visualization,machine learning,data analysis
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pandas~=1.2.1
-Requires-Dist: numpy~=1.26.2
-Requires-Dist: matplotlib~=3.8.2
-Requires-Dist: seaborn~=0.13.0
-Requires-Dist: pytz~=2024.1
-Requires-Dist: scikit-learn~=1.4.1.post1
-Requires-Dist: category_encoders~=2.6.3
-Requires-Dist: joblib~=1.3.2
-Requires-Dist: setuptools~=69.1.1
-Requires-Dist: typing~=3.7.4.3
-Requires-Dist: scipy~=1.11.4
-Requires-Dist: cartopy~=0.22.0
-Requires-Dist: geopandas~=0.14.3
-Requires-Dist: statsmodels~=0.14.1
-Requires-Dist: plotly~=5.19.0
-Provides-Extra: dev
-Requires-Dist: pydata_sphinx_theme==0.15.2; extra == "dev"
-Requires-Dist: sphinx-design==0.5.0; extra == "dev"
-Requires-Dist: Sphinx==7.2.6; extra == "dev"
-Requires-Dist: sphinx-rtd-theme==2.0.0; extra == "dev"
-Requires-Dist: sphinxcontrib-applehelp==1.0.8; extra == "dev"
-Requires-Dist: sphinxcontrib-devhelp==1.0.6; extra == "dev"
-Requires-Dist: sphinxcontrib-htmlhelp==2.0.5; extra == "dev"
-Requires-Dist: sphinxcontrib-jquery==4.1; extra == "dev"
-Requires-Dist: sphinxcontrib-jsmath==1.0.1; extra == "dev"
-Requires-Dist: sphinxcontrib-qthelp==1.0.7; extra == "dev"
-Requires-Dist: sphinxcontrib-serializinghtml==1.1.10; extra == "dev"
-Requires-Dist: myst-parser==2.0.0; extra == "dev"
-Requires-Dist: sphinx-favicon==1.0.1; extra == "dev"
-Requires-Dist: nbsphinx==0.9.3; extra == "dev"
-
 <br />
 <img src="https://www.datawaza.com/en/latest/_static/datawaza_logo_name_trans.svg" alt="datawaza_logo_name_trans.svg" width="300"/>
 
 --------------------------------------
 [![PyPI Version](https://img.shields.io/pypi/v/datawaza)](https://pypi.org/project/datawaza/)
 [![License](https://img.shields.io/github/license/jbeno/datawaza)](https://github.com/jbeno/datawaza/blob/main/LICENSE)
 [![Last Commit](https://img.shields.io/github/last-commit/jbeno/datawaza)](https://github.com/jbeno/datawaza)
@@ -64,64 +10,66 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/datawaza)]()
 
 Datawaza streamlines common Data Science tasks. It's a collection of tools for data exploration, visualization, data cleaning, pipeline creation, hyper-parameter searching, model iteration, and evaluation. It builds upon core libraries like [Pandas](https://pandas.pydata.org/), [Matplotlib](https://matplotlib.org/), [Seaborn](https://seaborn.pydata.org/), and [Scikit-Learn](https://scikit-learn.org/stable/).
 
 <p align="center">
   <a href="https://www.datawaza.com/en/latest/explore.html#datawaza.explore.plot_charts"><img src="https://www.datawaza.com/en/latest/_static/plot_charts.png" width="30%" /></a>
   <a href="https://www.datawaza.com/en/latest/explore.html#datawaza.explore.plot_map_ca"><img src="https://www.datawaza.com/en/latest/_static/plot_map_ca.png" width="30%" style="margin:0 1%;" /></a>
-  <a href="https://www.datawaza.com/en/latest/explore.html#datawaza.explore.plot_3d"><img src="https://www.datawaza.com/en/latest/_static/plot_3d.png" width="30%" /></a>
+  <a href="https://www.datawaza.com/en/latest/model.html#datawaza.model.compare_models"><img src="https://www.datawaza.com/en/latest/_static/compare_models_2.png" width="30%" /></a>
 </p>
 <p align="center">
+  <a href="https://www.datawaza.com/en/latest/explore.html#datawaza.explore.plot_corr"><img src="https://www.datawaza.com/en/latest/_static/plot_corr.png" width="30%" /></a>
+  <a href="https://www.datawaza.com/en/latest/model.html#datawaza.model.plot_train_history"><img src="https://www.datawaza.com/en/latest/_static/plot_train_history.png" width="30%" /></a>
   <a href="https://www.datawaza.com/en/latest/model.html#datawaza.model.iterate_model"><img src="https://www.datawaza.com/en/latest/_static/iterate_model_1.png" width="30%" /></a>
-  <a href="https://www.datawaza.com/en/latest/model.html#datawaza.model.iterate_model"><img src="https://www.datawaza.com/en/latest/_static/iterate_model_2.png" width="30%" style="margin:0 1%;" /></a>
-  <a href="https://www.datawaza.com/en/latest/model.html#datawaza.model.plot_results"><img src="https://www.datawaza.com/en/latest/_static/plot_results.png" width="30%" /></a>
 </p>
 <p align="center">
-  <a href="https://www.datawaza.com/en/latest/explore.html#datawaza.explore.get_corr"><img src="https://www.datawaza.com/en/latest/_static/get_corr.png" width="30%" /></a>
-  <a href="https://www.datawaza.com/en/latest/clean.html#datawaza.clean.reduce_multicollinearity"><img src="https://www.datawaza.com/en/latest/_static/reduce_multicollinearity.png" width="30%" style="margin:0 1%;" /></a>
-  <a href="https://www.datawaza.com/en/latest/explore.html#datawaza.explore.plot_corr"><img src="https://www.datawaza.com/en/latest/_static/plot_corr.png" width="30%" /></a>
+  <a href="https://www.datawaza.com/en/latest/model.html#datawaza.model.iterate_model"><img src="https://www.datawaza.com/en/latest/_static/iterate_model_2.png" width="30%" style="margin:0 1%;" /></a>
+  <a href="https://www.datawaza.com/en/latest/model.html#datawaza.model.plot_results"><img src="https://www.datawaza.com/en/latest/_static/plot_results.png" width="30%" /></a>
+  <a href="https://www.datawaza.com/en/latest/explore.html#datawaza.explore.plot_3d"><img src="https://www.datawaza.com/en/latest/_static/plot_3d.png" width="30%" /></a>
 </p>
 
 Installation
 ------------
 
-The latest release can be found on [PyPI](https://pypi.org/project/datawaza/). See the [Change Log](CHANGELOG.md) for a history of changes. Install Datawaza with pip:
+The latest release can be found on [PyPI](https://pypi.org/project/datawaza/). Install Datawaza with pip:
 
     pip install datawaza
 
+See the [Change Log](CHANGELOG.md) for a history of changes.
+
+Dependencies
+------------
+
+Datawaza supports Python 3.9 - 3.12. Because Cartopy does not support Python 3.8, and that's a dependency for `plot_map_ca`, 3.8 is not supported.
+
+Installation requires NumPy, Pandas, Matplotlib, Seaborn, Plotly, Scikit-Learn, SciPy, Cartopy, GeoPandas, StatsModels, TensorFlow, Keras, SciKeras (if utilizing KerasClassifier as a model), PyTorch, and a few other supporting packages. See the [Requirements.txt](https://github.com/jbeno/datawaza/blob/main/requirements.txt).
+
 Documentation
 -------------
 
 Online documentation is available at [Datawaza.com](https://datawaza.com).
 
 The [User Guide](https://www.datawaza.com/en/latest/userguide.html) is a Jupyter notebook that walks through how to use the Datawaza functions. It's probably the best place to start. There is also an API reference for the major modules: [Clean](https://www.datawaza.com/en/latest/clean.html), [Explore](https://www.datawaza.com/en/latest/explore.html), [Model](https://www.datawaza.com/en/latest/model.html), and [Tools](https://www.datawaza.com/en/latest/tools.html).
 
 Development
 -----------
 
 The [Datawaza repo](https://github.com/jbeno/datawaza) is on GitHub.
 
-Please submit bugs that you encounter to the [Issue Tracker](https://github.com/jbeno/datawaza/issues). Contributions and ideas for enhancements are welcome! So far this is a solo effort, but I would love to collaborate.
-
-Dependencies
-------------
-
-Datawaza supports Python 3.10. It may support other versions, but these have not been tested yet.
-
-Due to the breadth of use cases, installation requires NumPy, Pandas, Matplotlib, Seaborn, Plotly, Scikit-Learn, SciPy, Cartopy, GeoPandas, StatsModels, and a few other supporting packages. See the [Requirements.txt](https://github.com/jbeno/datawaza/blob/main/requirements.txt).
+Please submit bugs that you encounter to the [Issue Tracker](https://github.com/jbeno/datawaza/issues). Contributions and ideas for enhancements are welcome!
 
 What is Waza?
 -------------
 
 Waza (技) means "technique" in Japanese. In martial arts like Aikido, it is paired with words like "suwari-waza" (sitting techniques) or "kaeshi-waza" (reversal techniques). So we've paired it with "data" to represent Data Science techniques: データ技 "data-waza".
 
 Origin Story
 -------------
 
-Most of these functions were created while I was pursuing a [Professional Certificate in Machine Learning & Artificial Intelligence](https://em-executive.berkeley.edu/professional-certificate-machine-learning-artificial-intelligence) from U.C. Berkeley. With every assignment, I tried to simplify repetitive tasks and streamline my workflow. They served me well, and I hope you will find some value in them.
+Most of these functions were created while I was pursuing a [Professional Certificate](https://em-executive.berkeley.edu/professional-certificate-machine-learning-artificial-intelligence) in Machine Learning & Artificial Intelligence from U.C. Berkeley. With each assignment, I tried to simplify repetitive tasks and streamline my workflow. They served me well at the time, so perhaps they will be of value to others.
 
 Quick Start
 -----------
 
 The [User Guide](https://www.datawaza.com/en/latest/userguide.html) will show you how to use Datawaza's functions in depth. Assuming you already have data loaded, here are some examples of what it can do:
 
     >>> import datawaza as dw
@@ -150,39 +98,39 @@
     marital has 4 unique values:
     
         married        24928   60.52%
         single         11568   28.09%
         divorced       4612    11.2%
         unknown        80      0.19%
 
-Plot bar charts of categorical variables, dimensioned by the target variable:
+Plot bar charts of categorical variables:
 
-    >>> dw.plot_charts(df, plot_type='cat', cat_cols=cat_columns, hue='y', rotation=90)
+    >>> dw.plot_charts(df, plot_type='cat', cat_cols=cat_columns, rotation=90)
 
 ![plot_charts output](https://www.datawaza.com/en/latest/_static/plot_charts_output.png)
 
 Get the top positive and negative correlations with the target variable, and save to lists:
 
     >>> pos_features, neg_features = dw.get_corr(df_enc, n=10, var='subscribed_enc', return_arrays=True)
 
     Top 10 positive correlations:
-    Variable 1      Variable 2  Correlation
+                  Variable 1      Variable 2  Correlation
     0               duration  subscribed_enc         0.41
     1       poutcome_success  subscribed_enc         0.32
     2   previously_contacted  subscribed_enc         0.32
     3                  pdays  subscribed_enc         0.27
     4               previous  subscribed_enc         0.23
     5              month_mar  subscribed_enc         0.14
     6              month_oct  subscribed_enc         0.14
     7              month_sep  subscribed_enc         0.12
     8           no_default_1  subscribed_enc         0.10
     9            job_student  subscribed_enc         0.09
     
     Top 10 negative correlations:
-    Variable 1      Variable 2  Correlation
+                  Variable 1      Variable 2  Correlation
     0            nr.employed  subscribed_enc        -0.35
     1              euribor3m  subscribed_enc        -0.31
     2           emp.var.rate  subscribed_enc        -0.30
     3   poutcome_nonexistent  subscribed_enc        -0.19
     4      contact_telephone  subscribed_enc        -0.14
     5         cons.price.idx  subscribed_enc        -0.14
     6              month_may  subscribed_enc        -0.11
@@ -192,15 +140,15 @@
 
 Plot a chart showing the top correlations with the target variable:
 
     >>> dw.plot_corr(df_enc, 'subscribed_enc', n=16, size=(12,6), rotation=90)
 
 ![plot_corr output](https://www.datawaza.com/en/latest/_static/plot_corr_output.png)
 
-Run a model iteration, which dynamically assembles a pipeline and evaluates the model, including
+Run a regression model iteration, which dynamically assembles a pipeline and evaluates the model, including
 charts of residuals, predicted vs. actual, and coefficients:
 
     >>> results_df, iteration_6 = dw.iterate_model(X2_train, X2_test, y2_train, y2_test,
     ...     transformers=['ohe', 'log', 'poly3'], model='linreg',
     ...     iteration='6', note='X2. Test size: 0.25, Pipeline: OHE > Log > Poly3 > LinReg',
     ...     plot=True, lowess=True, coef=True, perm=True, vif=True, decimal=2,
     ...     save=True, save_df=results_df, config=my_config)
@@ -212,8 +160,101 @@
 Compare train/test scores across model iterations, and select the best result:
 
     >>> dw.plot_results(results_df, metrics=['Train MAE', 'Test MAE'], y_label='Mean Absolute Error',
     ...     select_metric='Test MAE', select_criteria='min', decimal=0)
 
 ![plot_results output](https://www.datawaza.com/en/latest/_static/plot_results_output.png)
 
+Define a configuration file to compare multiple binary classification models:
+
+    >>> # Set some variables referenced in the config
+    >>> random_state = 42
+    >>> class_weight = None
+    >>> max_iter = 10000
+    >>>
+    >>> # Set column lists referenced in the config
+    >>> num_columns = list(X.columns)
+    >>> cat_columns = []
+    >>>
+    >>> # Create a custom configuration file with 3 models and grid search params
+    >>> my_config = {
+    ...     'models' : {
+    ...         'logreg': LogisticRegression(max_iter=max_iter,
+    ...                   random_state=random_state, class_weight=class_weight),
+    ...         'knn_class': KNeighborsClassifier(),
+    ...         'tree_class': DecisionTreeClassifier(random_state=random_state,
+    ...                       class_weight=class_weight)
+    ...     },
+    ...     'imputers': {
+    ...         'simple_imputer': SimpleImputer()
+    ...     },
+    ...     'transformers': {
+    ...         'ohe': (OneHotEncoder(drop='if_binary', handle_unknown='ignore'),
+    ...                     cat_columns)
+    ...     },
+    ...     'scalers': {
+    ...         'stand': StandardScaler()
+    ...     },
+    ...     'selectors': {
+    ...         'sfs_logreg': SequentialFeatureSelector(LogisticRegression(
+    ...                       max_iter=max_iter, random_state=random_state,
+    ...                       class_weight=class_weight))
+    ...     },
+    ...     'params' : {
+    ...         'logreg': {
+    ...             'logreg__C': [0.0001, 0.001, 0.01, 0.1, 1, 10, 100],
+    ...             'logreg__solver': ['newton-cg', 'lbfgs', 'saga']
+    ...         },
+    ...         'knn_class': {
+    ...             'knn_class__n_neighbors': [3, 5, 10, 15, 20, 25],
+    ...             'knn_class__weights': ['uniform', 'distance'],
+    ...             'knn_class__metric': ['euclidean', 'manhattan']
+    ...         },
+    ...         'tree_class': {
+    ...             'tree_class__max_depth': [3, 5, 7],
+    ...             'tree_class__min_samples_split': [5, 10, 15],
+    ...             'tree_class__criterion': ['gini', 'entropy'],
+    ...             'tree_class__min_samples_leaf': [2, 4, 6]
+    ...         },
+    ...     },
+    ...     'cv': {
+    ...         'kfold_5': KFold(n_splits=5, shuffle=True, random_state=42)
+    ...     },
+    ...     'no_scale': ['tree_class'],
+    ...     'no_poly': ['knn_class', 'tree_class']
+    ... }
+
+Run a binary classification on 7 models, dynamically assembling the pipeline and
+performing a grid search of the hyper-parameters, all based on the configuration
+file defined above:
+
+    >>> results_df = compare_models(
+    ...
+    ...     # Data split and sampling
+    ...     x=X, y=y, test_size=0.25, stratify=None, under_sample=None,
+    ...     over_sample=None, svm_knn_resample=None,
+    ...
+    ...     # Models and pipeline steps
+    ...     imputer=None, transformers=None, scaler='stand', selector=None,
+    ...     models=['logreg', 'knn_class', 'svm_proba', 'tree_class',
+    ...     'forest_class', 'xgb_class', 'keras_class'], svm_proba=True,
+    ...
+    ...     # Grid search
+    ...     search_type='random', scorer='accuracy', grid_cv='kfold_5', verbose=1,
+    ...
+    ...     # Model evaluation and charts
+    ...     model_eval=True, plot_perf=True, plot_curve=True, fig_size=(12,6),
+    ...     legend_loc='lower left', rotation=45, threshold=0.5,
+    ...     class_map=class_map, pos_label=1, title='Breast Cancer',
+    ...
+    ...     # Config, preferences and notes
+    ...     config=my_config, class_weight=None, random_state=42, decimal=4,
+    ...     n_jobs=None, notes='Test Size=0.25, Threshold=0.50'
+    ... )  #doctest: +NORMALIZE_WHITESPACE
+
+![compare_models output 1 of 5](https://www.datawaza.com/en/latest/_static/compare_models_output_1.png)
+![compare_models output 2 of 5](https://www.datawaza.com/en/latest/_static/compare_models_output_2.png)
+![compare_models output 3 of 5](https://www.datawaza.com/en/latest/_static/compare_models_output_3.png)
+![compare_models output 4 of 5](https://www.datawaza.com/en/latest/_static/compare_models_output_4.png)
+![compare_models output 5 of 5](https://www.datawaza.com/en/latest/_static/compare_models_output_5.png)
+
 This was just a sample of some Datawaza tools. Download [userguide.ipynb](https://github.com/jbeno/datawaza/blob/main/docs/userguide.ipynb) and explore the full breadth of the library in your Jupyter environment.
```

#### html2text {}

```diff
@@ -1,39 +1,8 @@
-Metadata-Version: 2.1 Name: datawaza Version: 0.1.2 Summary: Datawaza is a
-collection of tools for data exploration, visualization, data cleaning,
-pipeline creation, model iteration, and evaluation. Home-page: https://
-datawaza.com Author: Jim Beno Author-email: jim@jimbeno.net Project-URL:
-Documentation, https://datawaza.com Project-URL: Source, https://github.com/
-jbeno/datawaza Keywords: data science,visualization,machine learning,data
-analysis Classifier: Development Status :: 3 - Alpha Classifier: Intended
-Audience :: Science/Research Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.10 Classifier: Operating System
-:: OS Independent Classifier: License :: OSI Approved :: GNU General Public
-License v3 (GPLv3) Classifier: Natural Language :: English Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Scientific/Engineering :: Visualization Classifier: Topic :: Scientific/
-Engineering :: Information Analysis Requires-Python: >=3.10 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: pandas~=1.2.1
-Requires-Dist: numpy~=1.26.2 Requires-Dist: matplotlib~=3.8.2 Requires-Dist:
-seaborn~=0.13.0 Requires-Dist: pytz~=2024.1 Requires-Dist: scikit-
-learn~=1.4.1.post1 Requires-Dist: category_encoders~=2.6.3 Requires-Dist:
-joblib~=1.3.2 Requires-Dist: setuptools~=69.1.1 Requires-Dist: typing~=3.7.4.3
-Requires-Dist: scipy~=1.11.4 Requires-Dist: cartopy~=0.22.0 Requires-Dist:
-geopandas~=0.14.3 Requires-Dist: statsmodels~=0.14.1 Requires-Dist:
-plotly~=5.19.0 Provides-Extra: dev Requires-Dist: pydata_sphinx_theme==0.15.2;
-extra == "dev" Requires-Dist: sphinx-design==0.5.0; extra == "dev" Requires-
-Dist: Sphinx==7.2.6; extra == "dev" Requires-Dist: sphinx-rtd-theme==2.0.0;
-extra == "dev" Requires-Dist: sphinxcontrib-applehelp==1.0.8; extra == "dev"
-Requires-Dist: sphinxcontrib-devhelp==1.0.6; extra == "dev" Requires-Dist:
-sphinxcontrib-htmlhelp==2.0.5; extra == "dev" Requires-Dist: sphinxcontrib-
-jquery==4.1; extra == "dev" Requires-Dist: sphinxcontrib-jsmath==1.0.1; extra
-== "dev" Requires-Dist: sphinxcontrib-qthelp==1.0.7; extra == "dev" Requires-
-Dist: sphinxcontrib-serializinghtml==1.1.10; extra == "dev" Requires-Dist:
-myst-parser==2.0.0; extra == "dev" Requires-Dist: sphinx-favicon==1.0.1; extra
-== "dev" Requires-Dist: nbsphinx==0.9.3; extra == "dev"
+
 [datawaza_logo_name_trans.svg]-------------------------------------- [![PyPI
 Version](https://img.shields.io/pypi/v/datawaza)](https://pypi.org/project/
 datawaza/) [![License](https://img.shields.io/github/license/jbeno/datawaza)]
 (https://github.com/jbeno/datawaza/blob/main/LICENSE) [![Last Commit](https://
 img.shields.io/github/last-commit/jbeno/datawaza)](https://github.com/jbeno/
 datawaza) [![Documentation Status](https://readthedocs.org/projects/datawaza/
 badge/?version=latest)](https://www.datawaza.com/en/latest/?badge=latest) [!
@@ -44,66 +13,66 @@
 exploration, visualization, data cleaning, pipeline creation, hyper-parameter
 searching, model iteration, and evaluation. It builds upon core libraries like
 [Pandas](https://pandas.pydata.org/), [Matplotlib](https://matplotlib.org/),
 [Seaborn](https://seaborn.pydata.org/), and [Scikit-Learn](https://scikit-
 learn.org/stable/).
      _[_h_t_t_p_s_:_/_/_w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/_e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_p_l_o_t___c_h_a_r_t_s_._p_n_g_]_[_h_t_t_p_s_:_/_/
  _w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/_e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_p_l_o_t___m_a_p___c_a_._p_n_g_]_[_h_t_t_p_s_:_/_/_w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/
+                    _e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_c_o_m_p_a_r_e___m_o_d_e_l_s___2_._p_n_g_]
+      _[_h_t_t_p_s_:_/_/_w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/_e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_p_l_o_t___c_o_r_r_._p_n_g_]_[_h_t_t_p_s_:_/_/
+      _w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/_e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_p_l_o_t___t_r_a_i_n___h_i_s_t_o_r_y_._p_n_g_]_[_h_t_t_p_s_:_/_/
+            _w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/_e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_i_t_e_r_a_t_e___m_o_d_e_l___1_._p_n_g_]
+   _[_h_t_t_p_s_:_/_/_w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/_e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_i_t_e_r_a_t_e___m_o_d_e_l___2_._p_n_g_]_[_h_t_t_p_s_:_/_/
+_w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/_e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_p_l_o_t___r_e_s_u_l_t_s_._p_n_g_]_[_h_t_t_p_s_:_/_/_w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/
                         _e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_p_l_o_t___3_d_._p_n_g_]
-   _[_h_t_t_p_s_:_/_/_w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/_e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_i_t_e_r_a_t_e___m_o_d_e_l___1_._p_n_g_]_[_h_t_t_p_s_:_/_/
-       _w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/_e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_i_t_e_r_a_t_e___m_o_d_e_l___2_._p_n_g_]_[_h_t_t_p_s_:_/_/
-             _w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/_e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_p_l_o_t___r_e_s_u_l_t_s_._p_n_g_]
-      _[_h_t_t_p_s_:_/_/_w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/_e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_g_e_t___c_o_r_r_._p_n_g_]_[_h_t_t_p_s_:_/_/
-   _w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/_e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_r_e_d_u_c_e___m_u_l_t_i_c_o_l_l_i_n_e_a_r_i_t_y_._p_n_g_]_[_h_t_t_p_s_:_/_/
-               _w_w_w_._d_a_t_a_w_a_z_a_._c_o_m_/_e_n_/_l_a_t_e_s_t_/___s_t_a_t_i_c_/_p_l_o_t___c_o_r_r_._p_n_g_]
 Installation ------------ The latest release can be found on [PyPI](https://
-pypi.org/project/datawaza/). See the [Change Log](CHANGELOG.md) for a history
-of changes. Install Datawaza with pip: pip install datawaza Documentation -----
--------- Online documentation is available at [Datawaza.com](https://
-datawaza.com). The [User Guide](https://www.datawaza.com/en/latest/
-userguide.html) is a Jupyter notebook that walks through how to use the
-Datawaza functions. It's probably the best place to start. There is also an API
-reference for the major modules: [Clean](https://www.datawaza.com/en/latest/
-clean.html), [Explore](https://www.datawaza.com/en/latest/explore.html),
-[Model](https://www.datawaza.com/en/latest/model.html), and [Tools](https://
-www.datawaza.com/en/latest/tools.html). Development ----------- The [Datawaza
-repo](https://github.com/jbeno/datawaza) is on GitHub. Please submit bugs that
-you encounter to the [Issue Tracker](https://github.com/jbeno/datawaza/issues).
-Contributions and ideas for enhancements are welcome! So far this is a solo
-effort, but I would love to collaborate. Dependencies ------------ Datawaza
-supports Python 3.10. It may support other versions, but these have not been
-tested yet. Due to the breadth of use cases, installation requires NumPy,
-Pandas, Matplotlib, Seaborn, Plotly, Scikit-Learn, SciPy, Cartopy, GeoPandas,
-StatsModels, and a few other supporting packages. See the [Requirements.txt]
-(https://github.com/jbeno/datawaza/blob/main/requirements.txt). What is Waza? -
------------- Waza (æ) means "technique" in Japanese. In martial arts like
-Aikido, it is paired with words like "suwari-waza" (sitting techniques) or
-"kaeshi-waza" (reversal techniques). So we've paired it with "data" to
-represent Data Science techniques: ãã¼ã¿æ "data-waza". Origin Story -----
--------- Most of these functions were created while I was pursuing a
-[Professional Certificate in Machine Learning & Artificial Intelligence](https:
-//em-executive.berkeley.edu/professional-certificate-machine-learning-
-artificial-intelligence) from U.C. Berkeley. With every assignment, I tried to
-simplify repetitive tasks and streamline my workflow. They served me well, and
-I hope you will find some value in them. Quick Start ----------- The [User
-Guide](https://www.datawaza.com/en/latest/userguide.html) will show you how to
-use Datawaza's functions in depth. Assuming you already have data loaded, here
-are some examples of what it can do: >>> import datawaza as dw Show the unique
-values of each variable below the threshold of n = 12: >>> dw.get_unique(df,
-12, count=True, percent=True) CATEGORICAL: Variables with unique values equal
-to or below: 12 job has 12 unique values: admin. 10422 25.3% blue-collar 9254
-22.47% technician 6743 16.37% services 3969 9.64% management 2924 7.1% retired
-1720 4.18% entrepreneur 1456 3.54% self-employed 1421 3.45% housemaid 1060
-2.57% unemployed 1014 2.46% student 875 2.12% unknown 330 0.8% marital has 4
-unique values: married 24928 60.52% single 11568 28.09% divorced 4612 11.2%
-unknown 80 0.19% Plot bar charts of categorical variables, dimensioned by the
-target variable: >>> dw.plot_charts(df, plot_type='cat', cat_cols=cat_columns,
-hue='y', rotation=90) ![plot_charts output](https://www.datawaza.com/en/latest/
-_static/plot_charts_output.png) Get the top positive and negative correlations
-with the target variable, and save to lists: >>> pos_features, neg_features =
+pypi.org/project/datawaza/). Install Datawaza with pip: pip install datawaza
+See the [Change Log](CHANGELOG.md) for a history of changes. Dependencies -----
+------- Datawaza supports Python 3.9 - 3.12. Because Cartopy does not support
+Python 3.8, and that's a dependency for `plot_map_ca`, 3.8 is not supported.
+Installation requires NumPy, Pandas, Matplotlib, Seaborn, Plotly, Scikit-Learn,
+SciPy, Cartopy, GeoPandas, StatsModels, TensorFlow, Keras, SciKeras (if
+utilizing KerasClassifier as a model), PyTorch, and a few other supporting
+packages. See the [Requirements.txt](https://github.com/jbeno/datawaza/blob/
+main/requirements.txt). Documentation ------------- Online documentation is
+available at [Datawaza.com](https://datawaza.com). The [User Guide](https://
+www.datawaza.com/en/latest/userguide.html) is a Jupyter notebook that walks
+through how to use the Datawaza functions. It's probably the best place to
+start. There is also an API reference for the major modules: [Clean](https://
+www.datawaza.com/en/latest/clean.html), [Explore](https://www.datawaza.com/en/
+latest/explore.html), [Model](https://www.datawaza.com/en/latest/model.html),
+and [Tools](https://www.datawaza.com/en/latest/tools.html). Development -------
+---- The [Datawaza repo](https://github.com/jbeno/datawaza) is on GitHub.
+Please submit bugs that you encounter to the [Issue Tracker](https://
+github.com/jbeno/datawaza/issues). Contributions and ideas for enhancements are
+welcome! What is Waza? ------------- Waza (æ) means "technique" in Japanese.
+In martial arts like Aikido, it is paired with words like "suwari-waza"
+(sitting techniques) or "kaeshi-waza" (reversal techniques). So we've paired it
+with "data" to represent Data Science techniques: ãã¼ã¿æ "data-waza".
+Origin Story ------------- Most of these functions were created while I was
+pursuing a [Professional Certificate](https://em-executive.berkeley.edu/
+professional-certificate-machine-learning-artificial-intelligence) in Machine
+Learning & Artificial Intelligence from U.C. Berkeley. With each assignment, I
+tried to simplify repetitive tasks and streamline my workflow. They served me
+well at the time, so perhaps they will be of value to others. Quick Start -----
+------ The [User Guide](https://www.datawaza.com/en/latest/userguide.html) will
+show you how to use Datawaza's functions in depth. Assuming you already have
+data loaded, here are some examples of what it can do: >>> import datawaza as
+dw Show the unique values of each variable below the threshold of n = 12: >>>
+dw.get_unique(df, 12, count=True, percent=True) CATEGORICAL: Variables with
+unique values equal to or below: 12 job has 12 unique values: admin. 10422
+25.3% blue-collar 9254 22.47% technician 6743 16.37% services 3969 9.64%
+management 2924 7.1% retired 1720 4.18% entrepreneur 1456 3.54% self-employed
+1421 3.45% housemaid 1060 2.57% unemployed 1014 2.46% student 875 2.12% unknown
+330 0.8% marital has 4 unique values: married 24928 60.52% single 11568 28.09%
+divorced 4612 11.2% unknown 80 0.19% Plot bar charts of categorical variables:
+>>> dw.plot_charts(df, plot_type='cat', cat_cols=cat_columns, rotation=90) !
+[plot_charts output](https://www.datawaza.com/en/latest/_static/
+plot_charts_output.png) Get the top positive and negative correlations with the
+target variable, and save to lists: >>> pos_features, neg_features =
 dw.get_corr(df_enc, n=10, var='subscribed_enc', return_arrays=True) Top 10
 positive correlations: Variable 1 Variable 2 Correlation 0 duration
 subscribed_enc 0.41 1 poutcome_success subscribed_enc 0.32 2
 previously_contacted subscribed_enc 0.32 3 pdays subscribed_enc 0.27 4 previous
 subscribed_enc 0.23 5 month_mar subscribed_enc 0.14 6 month_oct subscribed_enc
 0.14 7 month_sep subscribed_enc 0.12 8 no_default_1 subscribed_enc 0.10 9
 job_student subscribed_enc 0.09 Top 10 negative correlations: Variable 1
@@ -111,26 +80,73 @@
 subscribed_enc -0.31 2 emp.var.rate subscribed_enc -0.30 3 poutcome_nonexistent
 subscribed_enc -0.19 4 contact_telephone subscribed_enc -0.14 5 cons.price.idx
 subscribed_enc -0.14 6 month_may subscribed_enc -0.11 7 campaign subscribed_enc
 -0.07 8 job_blue-collar subscribed_enc -0.07 9 education_basic.9y
 subscribed_enc -0.05 Plot a chart showing the top correlations with the target
 variable: >>> dw.plot_corr(df_enc, 'subscribed_enc', n=16, size=(12,6),
 rotation=90) ![plot_corr output](https://www.datawaza.com/en/latest/_static/
-plot_corr_output.png) Run a model iteration, which dynamically assembles a
-pipeline and evaluates the model, including charts of residuals, predicted vs.
-actual, and coefficients: >>> results_df, iteration_6 = dw.iterate_model
-(X2_train, X2_test, y2_train, y2_test, ... transformers=['ohe', 'log',
-'poly3'], model='linreg', ... iteration='6', note='X2. Test size: 0.25,
+plot_corr_output.png) Run a regression model iteration, which dynamically
+assembles a pipeline and evaluates the model, including charts of residuals,
+predicted vs. actual, and coefficients: >>> results_df, iteration_6 =
+dw.iterate_model(X2_train, X2_test, y2_train, y2_test, ... transformers=['ohe',
+'log', 'poly3'], model='linreg', ... iteration='6', note='X2. Test size: 0.25,
 Pipeline: OHE > Log > Poly3 > LinReg', ... plot=True, lowess=True, coef=True,
 perm=True, vif=True, decimal=2, ... save=True, save_df=results_df,
 config=my_config) ![iterate_model output 1 of 3](https://www.datawaza.com/en/
 latest/_static/iterate_model_output_1.png) ![iterate_model output 2 of 3]
 (https://www.datawaza.com/en/latest/_static/iterate_model_output_2.png) !
 [iterate_model output 3 of 3](https://www.datawaza.com/en/latest/_static/
 iterate_model_output_3.png) Compare train/test scores across model iterations,
 and select the best result: >>> dw.plot_results(results_df, metrics=['Train
 MAE', 'Test MAE'], y_label='Mean Absolute Error', ... select_metric='Test MAE',
 select_criteria='min', decimal=0) ![plot_results output](https://
-www.datawaza.com/en/latest/_static/plot_results_output.png) This was just a
-sample of some Datawaza tools. Download [userguide.ipynb](https://github.com/
-jbeno/datawaza/blob/main/docs/userguide.ipynb) and explore the full breadth of
-the library in your Jupyter environment.
+www.datawaza.com/en/latest/_static/plot_results_output.png) Define a
+configuration file to compare multiple binary classification models: >>> # Set
+some variables referenced in the config >>> random_state = 42 >>> class_weight
+= None >>> max_iter = 10000 >>> >>> # Set column lists referenced in the config
+>>> num_columns = list(X.columns) >>> cat_columns = [] >>> >>> # Create a
+custom configuration file with 3 models and grid search params >>> my_config =
+{ ... 'models' : { ... 'logreg': LogisticRegression(max_iter=max_iter, ...
+random_state=random_state, class_weight=class_weight), ... 'knn_class':
+KNeighborsClassifier(), ... 'tree_class': DecisionTreeClassifier
+(random_state=random_state, ... class_weight=class_weight) ... }, ...
+'imputers': { ... 'simple_imputer': SimpleImputer() ... }, ... 'transformers':
+{ ... 'ohe': (OneHotEncoder(drop='if_binary', handle_unknown='ignore'), ...
+cat_columns) ... }, ... 'scalers': { ... 'stand': StandardScaler() ... }, ...
+'selectors': { ... 'sfs_logreg': SequentialFeatureSelector(LogisticRegression
+( ... max_iter=max_iter, random_state=random_state, ...
+class_weight=class_weight)) ... }, ... 'params' : { ... 'logreg': { ...
+'logreg__C': [0.0001, 0.001, 0.01, 0.1, 1, 10, 100], ... 'logreg__solver':
+['newton-cg', 'lbfgs', 'saga'] ... }, ... 'knn_class': { ...
+'knn_class__n_neighbors': [3, 5, 10, 15, 20, 25], ... 'knn_class__weights':
+['uniform', 'distance'], ... 'knn_class__metric': ['euclidean', 'manhattan']
+... }, ... 'tree_class': { ... 'tree_class__max_depth': [3, 5, 7], ...
+'tree_class__min_samples_split': [5, 10, 15], ... 'tree_class__criterion':
+['gini', 'entropy'], ... 'tree_class__min_samples_leaf': [2, 4, 6] ... }, ...
+}, ... 'cv': { ... 'kfold_5': KFold(n_splits=5, shuffle=True, random_state=42)
+... }, ... 'no_scale': ['tree_class'], ... 'no_poly': ['knn_class',
+'tree_class'] ... } Run a binary classification on 7 models, dynamically
+assembling the pipeline and performing a grid search of the hyper-parameters,
+all based on the configuration file defined above: >>> results_df =
+compare_models( ... ... # Data split and sampling ... x=X, y=y, test_size=0.25,
+stratify=None, under_sample=None, ... over_sample=None, svm_knn_resample=None,
+... ... # Models and pipeline steps ... imputer=None, transformers=None,
+scaler='stand', selector=None, ... models=['logreg', 'knn_class', 'svm_proba',
+'tree_class', ... 'forest_class', 'xgb_class', 'keras_class'], svm_proba=True,
+... ... # Grid search ... search_type='random', scorer='accuracy',
+grid_cv='kfold_5', verbose=1, ... ... # Model evaluation and charts ...
+model_eval=True, plot_perf=True, plot_curve=True, fig_size=(12,6), ...
+legend_loc='lower left', rotation=45, threshold=0.5, ... class_map=class_map,
+pos_label=1, title='Breast Cancer', ... ... # Config, preferences and notes ...
+config=my_config, class_weight=None, random_state=42, decimal=4, ...
+n_jobs=None, notes='Test Size=0.25, Threshold=0.50' ... ) #doctest:
++NORMALIZE_WHITESPACE ![compare_models output 1 of 5](https://www.datawaza.com/
+en/latest/_static/compare_models_output_1.png) ![compare_models output 2 of 5]
+(https://www.datawaza.com/en/latest/_static/compare_models_output_2.png) !
+[compare_models output 3 of 5](https://www.datawaza.com/en/latest/_static/
+compare_models_output_3.png) ![compare_models output 4 of 5](https://
+www.datawaza.com/en/latest/_static/compare_models_output_4.png) !
+[compare_models output 5 of 5](https://www.datawaza.com/en/latest/_static/
+compare_models_output_5.png) This was just a sample of some Datawaza tools.
+Download [userguide.ipynb](https://github.com/jbeno/datawaza/blob/main/docs/
+userguide.ipynb) and explore the full breadth of the library in your Jupyter
+environment.
```

### Comparing `datawaza-0.1.2/datawaza/__init__.py` & `datawaza-0.1.3/datawaza/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,39 +26,49 @@
     - :mod:`datawaza.model`: Utilities for model training, evaluation, and iteration.
     - :mod:`datawaza.tools`: Miscellaneous helper functions and utilities.
 """
 
 # Metadata
 __author__ = "Jim Beno"
 __email__ = "jim@jimbeno.net"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __license__ = "GNU GPLv3"
 
 from .explore import (get_outliers,
                       get_corr,
                       get_unique,
                       plot_charts,
                       plot_corr,
                       plot_3d,
-                      plot_map_ca)
+                      plot_map_ca,
+                      plot_scatt,
+                      print_ascii_image)
 
 from .clean import (convert_data_values,
                     convert_dtypes,
                     convert_time_values,
                     reduce_multicollinearity,
                     split_outliers)
 
 from .tools import (calc_pfi,
                     calc_vif,
                     check_for_duplicates,
+                    DebugPrinter,
                     extract_coef,
                     format_df,
                     log_transform,
+                    model_summary,
                     split_dataframe,
-                    thousand_dollars,
+                    dollars,
                     thousands,
                     LogTransformer)
 
-from .model import (create_pipeline,
+from .model import (compare_models,
+                    create_nn_binary,
+                    create_nn_multi,
+                    create_pipeline,
                     create_results_df,
+                    eval_model,
                     iterate_model,
-                    plot_results)
+                    plot_acf_residuals,
+                    plot_results,
+                    plot_train_history)
```

### Comparing `datawaza-0.1.2/datawaza/clean.py` & `datawaza-0.1.3/datawaza/clean.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     - :func:`~datawaza.clean.reduce_multicollinearity` - Reduce multicollinearity in a DataFrame by removing highly correlated features.
     - :func:`~datawaza.clean.split_outliers` - Split a DataFrame into two based on the presence of outliers.
 """
 
 # Metadata
 __author__ = "Jim Beno"
 __email__ = "jim@jimbeno.net"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __license__ = "GNU GPLv3"
 
 # Standard library imports
 import re
 
 # Data manipulation and analysis
 import numpy as np
```

### Comparing `datawaza-0.1.2/datawaza/data/cb_2018_us_county_5m.dbf` & `datawaza-0.1.3/datawaza/data/cb_2018_us_county_5m.dbf`

 * *Files identical despite different names*

### Comparing `datawaza-0.1.2/datawaza/data/cb_2018_us_county_5m.shp` & `datawaza-0.1.3/datawaza/data/cb_2018_us_county_5m.shp`

 * *Files identical despite different names*

### Comparing `datawaza-0.1.2/datawaza/data/cb_2018_us_county_5m.shp.ea.iso.xml` & `datawaza-0.1.3/datawaza/data/cb_2018_us_county_5m.shp.ea.iso.xml`

 * *Files identical despite different names*

### Comparing `datawaza-0.1.2/datawaza/data/cb_2018_us_county_5m.shp.iso.xml` & `datawaza-0.1.3/datawaza/data/cb_2018_us_county_5m.shp.iso.xml`

 * *Files identical despite different names*

### Comparing `datawaza-0.1.2/datawaza/data/cb_2018_us_county_5m.shx` & `datawaza-0.1.3/datawaza/data/cb_2018_us_county_5m.shx`

 * *Files identical despite different names*

### Comparing `datawaza-0.1.2/datawaza/explore.py` & `datawaza-0.1.3/datawaza/tools.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,1332 +1,1357 @@
-# explore.py – Explore module of Datawaza
+# tools.py – Tools module of Datawaza
 #
 # Datawaza  Copyright (C) 2024  Jim Beno
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details:
 # https://github.com/jbeno/datawaza/blob/main/LICENSE
 """
-This module provides tools to streamline exploratory data analysis.
-It contains functions to find unique values, plot distributions, detect outliers,
-extract the top correlations, plot correlations, plot 3D charts, and plot data
-on a map of California.
+This module provides helper tools used in data analysis, cleaning, and modeling.
+It contains functions to check for duplicates in lists, split a dataframe into two
+by numeric vs. categorical variables, format numbers on the axis of a chart,
+perform log transformations, calculate VIF and Feature Permutation Importance,
+and extract the coefficients from models that support them.
+
+Classes:
+    - :class:`~datawaza.tools.DebugPrinter` - Conditionally print debugging information during the execution of a script.
+        - :meth:`~datawaza.tools.DebugPrinter.print` - Print a message if debugging is enabled.
+        - :meth:`~datawaza.tools.DebugPrinter.set_debug` - Enable or disable debugging mode.
+    - :class:`~datawaza.tools.LogTransformer` - Apply logarithmic transformation to numerical features.
+        - :meth:`~datawaza.tools.LogTransformer.fit` - Fit the transformer to the input data.
+        - :meth:`~datawaza.tools.LogTransformer.transform` - Apply the logarithmic transformation to the input data.
+        - :meth:`~datawaza.tools.LogTransformer.get_feature_names_out` - Get the feature names after applying the transformation.
 
 Functions:
-    - :func:`~datawaza.explore.get_corr` - Display the top `n` positive and negative correlations with a target variable in a DataFrame.
-    - :func:`~datawaza.explore.get_outliers` - Detects and summarizes outliers for the specified numeric columns in a DataFrame, based on an IQR ratio.
-    - :func:`~datawaza.explore.get_unique` - Print the unique values of all variables below a threshold `n`, including counts and percentages.
-    - :func:`~datawaza.explore.plot_3d` - Create a 3D scatter plot using Plotly Express.
-    - :func:`~datawaza.explore.plot_charts` - Display multiple bar plots and histograms for categorical and/or continuous variables in a DataFrame, with an option to dimension by the specified `hue`.
-    - :func:`~datawaza.explore.plot_corr` - Plot the top `n` correlations of one variable against others in a DataFrame.
-    - :func:`~datawaza.explore.plot_map_ca` - Plot longitude and latitude data on a geographic map of California.
+    - :func:`~datawaza.tools.calc_pfi` - Calculate Permutation Feature Importance for a trained model.
+    - :func:`~datawaza.tools.calc_vif` - Calculate the Variance Inflation Factor (VIF) for each feature.
+    - :func:`~datawaza.tools.check_for_duplicates` - Check for duplicate items (ex: column names) across multiple lists.
+    - :func:`~datawaza.tools.extract_coef` - Extract feature names and coefficients from a trained model.
+    - :func:`~datawaza.tools.format_df` - Format columns of a DataFrame as either large or small numbers.
+    - :func:`~datawaza.tools.log_transform` - Apply a log transformation to specified columns in a DataFrame.
+    - :func:`~datawaza.tools.model_summary` - Create a DataFrame summary of a Keras model's architecture and parameters.
+    - :func:`~datawaza.tools.split_dataframe` - Split a DataFrame into categorical and numerical columns.
+    - :func:`~datawaza.tools.thousand_dollars` - Format a number as currency with thousands separators on a matplotlib chart axis.
+    - :func:`~datawaza.tools.thousands` - Format a number with thousands separators on a matplotlib chart axis.
 """
 
 # Metadata
 __author__ = "Jim Beno"
 __email__ = "jim@jimbeno.net"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __license__ = "GNU GPLv3"
 
 # Standard library imports
-import matplotlib.patheffects as pe
+import os
+import inspect
 
 # Data manipulation and analysis
 import numpy as np
 import pandas as pd
-from pandas import DataFrame
-import geopandas as gpd
 
 # Visualization libraries
 import matplotlib.pyplot as plt
-from matplotlib.ticker import FuncFormatter
 import seaborn as sns
-import plotly.express as px
 
-# Statistical and geographic mapping
-from scipy.stats import iqr
-import cartopy.crs as ccrs
-import cartopy.feature as cfeature
-
-# Miscellaneous imports
-from importlib.resources import path
-
-# Local Datawaza helper function imports
-from datawaza.tools import thousands
+# Machine Learning: Model selection and evaluation
+from sklearn.model_selection import GridSearchCV
+from sklearn.inspection import permutation_importance
+
+# Machine Learning: Pipeline and transformations
+from sklearn.pipeline import Pipeline
+from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.compose import ColumnTransformer
+from sklearn.preprocessing import StandardScaler
+
+# Machine Learning: Models
+from sklearn.linear_model import (
+    LogisticRegression, LogisticRegressionCV, PassiveAggressiveClassifier,
+    Perceptron, RidgeClassifier, RidgeClassifierCV, SGDClassifier, SGDOneClassSVM,
+    LinearRegression, Ridge, RidgeCV, SGDRegressor, ElasticNet, ElasticNetCV,
+    Lars, LarsCV, Lasso, LassoCV, LassoLars, LassoLarsCV, LassoLarsIC,
+    OrthogonalMatchingPursuit, OrthogonalMatchingPursuitCV, ARDRegression,
+    BayesianRidge, HuberRegressor, QuantileRegressor, RANSACRegressor,
+    TheilSenRegressor
+)
 
 # Typing imports
 from typing import Optional, Union, Tuple, List, Dict, Any
 
+# TensorFlow and Keras
+os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'  # Suppress TensorFlow warning on import
+import tensorflow as tf
+import keras as keras
+
 
 # Functions
-def get_corr(
-        df: DataFrame,
-        n: int = 5,
-        var: Optional[str] = None,
-        show_results: bool = True,
-        return_arrays: bool = False
-) -> Union[None, Tuple[np.ndarray, np.ndarray]]:
-    """
-    Display the top `n` positive and negative correlations with a target variable
-    in a DataFrame.
-
-    This function computes the correlation matrix for the provided DataFrame, and
-    identifies the top `n` positively and negatively correlated pairs of variables.
-    By default, it prints a summary of these correlations. Optionally, it can
-    return arrays of the variable names involved in these top correlations,
-    avoiding duplicates.
-
-    Use this to quickly identify the strongest correlations with a target variable.
-    You can also use this to reduce a DataFrame with a large number of features
-    down to just the top `n` correlated features. Extract the names of the top
-    correlated features into 2 separate arrays (one for positive, one for
-    negative). Concatenate those variable lists and append the target variable. Use
-    this concatenated array to create a new DataFrame.
+def calc_pfi(model,
+             X: pd.DataFrame,
+             y: pd.Series,
+             scoring: Any = None,
+             n_repeats: int = 10,
+             random_state: int = 42,
+             decimal: int = 2
+             ) -> pd.DataFrame:
+    """
+    Calculate Permutation Feature Importance for a trained model.
+
+    This function calculates the Permutation Feature Importance (PFI) for
+    each feature in the input dataset using a trained model. PFI measures
+    the importance of each feature by permuting its values and observing
+    the impact on the model's performance. Features with higher
+    permutation importance scores are considered more important for the
+    model's predictions.
+
+    The function returns a DataFrame with the feature names, mean
+    permutation importance scores, and standard deviations of the scores.
+    The DataFrame is sorted in descending order based on the mean scores.
+    It's just a wrapper around the Scikit-learn `permutation_importance`
+    function to display the results in a convenient format.
+
+    Use this function to identify the most important features for a
+    trained model and gain insights into the model's behavior.
 
     Parameters
     ----------
-    df : pandas.DataFrame
-        The DataFrame to analyze for correlations.
-    n : int, optional
-        The number of top positive and negative correlations to list. Default is 5.
-    var : str, optional
-        A specific variable of interest. If provided, the function will only
-        consider correlations involving this variable. Default is None.
-    show_results : bool, optional
-        Flag to indicate if the results should be printed. Default is True.
-    return_arrays : bool, optional
-        Flag to indicate if the function should return arrays of variable names
-        involved in the top correlations. Default is False.
+    model :
+        The trained model object. It should have a `predict` method.
+    X : pd.DataFrame
+        The input DataFrame containing the features used for prediction.
+    y : pd.Series
+        The target variable or labels corresponding to the input features.
+    scoring : Any, optional
+        Scorer to use. It can be a single string (see sklearn 'scoring_parameter') or
+        a callable that returns a single value. Default is None, which uses the
+        estimator's default scorer.
+    n_repeats : int, optional
+        The number of times to permute each feature. Higher values provide
+        more stable importance scores but increase computation time.
+        Default is 10.
+    random_state : int, optional
+        The random seed for reproducibility. Default is 42.
+    decimal : int, optional
+        The number of decimals to round to when displaying output.
+        Default is 2.
 
     Returns
     -------
-    tuple, optional
-        If `return_arrays` is set to True, the function returns a tuple containing
-        two arrays: (1) `positive_variables`: An array of variable names involved
-        in the top n positive correlations. (2) `negative_variables`: An array of
-        variable names involved in the top n negative correlations. If
-        `return_arrays` is False, the function returns nothing.
+    pd.DataFrame
+        A DataFrame with three columns: 'Feature' (feature names),
+        'Importance Mean' (mean permutation importance scores), and
+        'Importance Std' (standard deviations of the scores). The DataFrame is
+        sorted in descending order based on the 'Importance Mean' column.
 
     Examples
     --------
-    Prepare the data for the examples:
+    Prepare a sample dataset and train a model:
 
-    >>> np.random.seed(0)  # For reproducibility
-    >>> n_samples = 100
-    >>> # Create variables
-    >>> temp = np.linspace(10, 30, n_samples) + np.random.normal(0, 2, n_samples)
-    >>> sales = temp * 3 + np.random.normal(0, 10, n_samples)
-    >>> fuel = 100 - temp * 2 + np.random.normal(0, 5, n_samples)
-    >>> humidity = 70 - temp * 1.5 + np.random.normal(0, 4, n_samples)
-    >>> ac_units_sold = temp * 2 + np.random.normal(0, 15, n_samples)
-    >>> # Create DataFrame
-    >>> df = pd.DataFrame({'Temp': temp, 'Sales': sales, 'Fuel': fuel,
-    ...                    'Humidity': humidity, 'AC_Units_Sold': ac_units_sold})
-
-    Example 1: Print the top 'n' correlations, both positive and negative:
-
-    >>> get_corr(df, n=2, var='Temp')
-    Top 2 positive correlations:
-          Variable 1 Variable 2  Correlation
-    0          Sales       Temp         0.85
-    1  AC_Units_Sold       Temp         0.62
-    <BLANKLINE>
-    Top 2 negative correlations:
-      Variable 1 Variable 2  Correlation
-    0       Fuel       Temp        -0.92
-    1   Humidity       Temp        -0.92
+    >>> from sklearn.datasets import load_iris
+    >>> from sklearn.ensemble import RandomForestClassifier
+    >>> iris = load_iris()
+    >>> X = pd.DataFrame(iris.data, columns=iris.feature_names)
+    >>> y = pd.Series(iris.target)
+    >>> model = RandomForestClassifier(random_state=42)
+    >>> model.fit(X, y)
+    RandomForestClassifier(random_state=42)
+
+    Calculate Permutation Feature Importance:
+
+    >>> pfi_df = calc_pfi(model, X, y, decimal=4)
+    >>> pfi_df
+                 Feature Importance Mean Importance Std
+    2  petal length (cm)          0.2227         0.0243
+    3   petal width (cm)          0.1807         0.0212
+    0  sepal length (cm)          0.0147         0.0065
+    1   sepal width (cm)          0.0127         0.0047
+    """
+    # Calculate Permutation Feature Importance
+    r = permutation_importance(model, X, y, n_repeats=n_repeats, scoring=scoring,
+                               random_state=random_state)
+
+    # Create a DataFrame with feature names, mean scores, and std scores
+    pfi_df = pd.DataFrame({"Feature": X.columns,
+                           "Importance Mean": r.importances_mean,
+                           "Importance Std": r.importances_std})
+
+    # Sort the DataFrame by mean scores in descending order
+    pfi_sorted = pfi_df.sort_values(by="Importance Mean", ascending=False)
 
-    Example 2: Create arrays with the top correlated feature names:
+    # Format the PFI values for better readability
+    pfi_formatted = format_df(pfi_sorted, small_num_cols=['Importance Mean', 'Importance Std'], decimal=decimal)
 
-    >>> (top_pos, top_neg) = get_corr(df, n=1, var='Temp', show_results=False,
-    ...     return_arrays=True)
-    >>> print(top_pos)
-    ['Sales']
-    >>> print(top_neg)
-    ['Fuel']
+    return pfi_formatted
 
-    Example 3: Create a dataframe of top correlated features from those arrays:
 
-    >>> top_features = np.concatenate((top_pos, top_neg, ['Temp']))
-    >>> df_top_features = df[top_features]
-    >>> print(df_top_features[:2])
-           Sales       Fuel       Temp
-    0  59.415821  71.097881  13.528105
-    1  19.529413  76.798435  11.002335
+def calc_vif(X: pd.DataFrame,
+             num_columns: Optional[List[str]] = None,
+             decimal: int = 2
+             ) -> pd.DataFrame:
     """
-    pd.set_option('display.expand_frame_repr', False)
+    Calculate the Variance Inflation Factor (VIF) for each feature.
 
-    corr = round(df.corr(numeric_only=True), 2)
+    This function calculates the VIF for each feature in the input
+    dataset. VIF is a measure of multicollinearity, which indicates the
+    degree to which a feature can be explained by other features in the
+    dataset. A higher VIF value suggests higher multicollinearity, and a
+    VIF value exceeding 5 or 10 is often regarded as indicating severe
+    multicollinearity.
+
+    By default, VIF will be calculated for all numeric columns in the `X`
+    DataFrame. You can optionally specify columns with `num_columns`. You
+    can also control how many decimal places are shown with `decimal`.
+
+    The function also interprets the level of multicollinearity based on
+    the VIF values and assigns a corresponding category: "Extreme" (VIF
+    >= 100), "High" (10 <= VIF < 100), "Moderate" (5 <= VIF < 10), or
+    "Low" (VIF < 5).
 
-    # Unstack correlation matrix into a DataFrame
-    corr_df = corr.unstack().reset_index()
-    corr_df.columns = ['Variable 1', 'Variable 2', 'Correlation']
+    Use this function to identify features with high multicollinearity in
+    your dataset before performing further analysis or modeling.
 
-    # If a variable is specified, filter to correlations involving that variable
-    if var is not None:
-        corr_df = corr_df[(corr_df['Variable 1'] == var) | (corr_df['Variable 2'] == var)]
+    Parameters
+    ----------
+    X : pd.DataFrame
+        The input DataFrame containing the features to calculate VIF for.
+    num_columns : List[str], optional
+        List of column names to consider for VIF calculation. If
+        provided, only the specified numeric columns will be used. If
+        None (default), all numeric columns in the DataFrame will be
+        used.
+    decimal : int, optional
+        The number of decimals to round to when displaying output.
+        Default is 2.
 
-    # Remove self-correlations and duplicates
-    corr_df = corr_df[corr_df['Variable 1'] != corr_df['Variable 2']]
-    corr_df[['Variable 1', 'Variable 2']] = np.sort(corr_df[['Variable 1', 'Variable 2']], axis=1)
-    corr_df = corr_df.drop_duplicates(subset=['Variable 1', 'Variable 2'])
+    Returns
+    -------
+    pd.DataFrame
+        A DataFrame with three columns: 'Features' (feature names), 'VIF'
+        (VIF values), and 'Multicollinearity' (interpreted level of
+        multicollinearity). The DataFrame is sorted in descending order
+        based on the VIF values.
 
-    # Sort by absolute correlation value from highest to lowest
-    corr_df['AbsCorrelation'] = corr_df['Correlation'].abs()
-    corr_df = corr_df.sort_values(by='AbsCorrelation', ascending=False)
+    Examples
+    --------
+    Prepare a sample dataset for the examples:
+
+    >>> from sklearn.datasets import load_iris
+    >>> iris = load_iris()
+    >>> X = pd.DataFrame(iris.data, columns=iris.feature_names)
+    >>> num_columns = list(X.columns)
+
+    Example 1: Calculate VIF for all numeric features in the iris dataset:
+
+    >>> vif_df = calc_vif(X)
+    >>> vif_df
+                Features    VIF Multicollinearity
+    2  petal length (cm)  31.26              High
+    3   petal width (cm)  16.09              High
+    0  sepal length (cm)   7.07          Moderate
+    1   sepal width (cm)   2.10               Low
+
+    Example 2: Calculate VIF for specific numeric features, 4 decimals:
+
+    >>> vif_df = calc_vif(X, num_columns=num_columns, decimal=4)
+    >>> vif_df
+                Features      VIF Multicollinearity
+    2  petal length (cm)  31.2615              High
+    3   petal width (cm)  16.0902              High
+    0  sepal length (cm)   7.0727          Moderate
+    1   sepal width (cm)   2.1009               Low
+    """
+    from sklearn.linear_model import LinearRegression
 
-    # Drop the absolute value column
-    corr_df = corr_df.drop(columns='AbsCorrelation').reset_index(drop=True)
+    def interpret_vif(vif):
+        if vif >= 100:
+            return "Extreme"
+        elif vif >= 10:
+            return "High"
+        elif vif >= 5:
+            return "Moderate"
+        else:
+            return "Low"
 
-    # Get the first n positive and negative correlations
-    positive_corr = corr_df[corr_df['Correlation'] > 0].head(n).reset_index(drop=True)
-    negative_corr = corr_df[corr_df['Correlation'] < 0].head(n).reset_index(drop=True)
+    # Set a high threshold for very large VIFs
+    MAX_VIF = 1000
 
-    # Print the results
-    if show_results:
-        print("Top", n, "positive correlations:")
-        print(positive_corr)
-        print("\nTop", n, "negative correlations:")
-        print(negative_corr)
+    # If num_columns is not provided, select all numeric columns
+    if num_columns is None:
+        num_columns = X.select_dtypes(include=[np.number]).columns
 
-    # Return the arrays
-    if return_arrays:
-        # Remove target variable from the arrays
-        positive_variables = positive_corr[['Variable 1', 'Variable 2']].values.flatten()
-        positive_variables = positive_variables[positive_variables != var]
+    vif_dict = {}
 
-        negative_variables = negative_corr[['Variable 1', 'Variable 2']].values.flatten()
-        negative_variables = negative_variables[negative_variables != var]
+    for feature in num_columns:
+        other_features = [col for col in num_columns if col != feature]
 
-        return positive_variables, negative_variables
+        # Split the dataset, one independent variable against all others
+        X_other, y = X[other_features], X[feature]
 
+        # Fit the model and obtain R^2
+        r_squared = LinearRegression().fit(X_other, y).score(X_other, y)
 
-def get_outliers(
-        df: pd.DataFrame,
-        num_columns: List[str],
-        ratio: float = 1.5,
-        exclude_zeros: bool = False,
-        plot: bool = False,
-        width: int = 15,
-        height: int = 2
-) -> pd.DataFrame:
+        # Compute the VIF, with a check for r_squared close to 1
+        if 1 - r_squared < 1e-5:
+            vif = MAX_VIF
+        else:
+            vif = 1 / (1 - r_squared)
+
+        vif_dict[feature] = vif
+
+    # Create a DataFrame with VIF values
+    vif_df = pd.DataFrame({"Features": vif_dict.keys(), "VIF": vif_dict.values()})
+
+    # Flag severe multicollinearity
+    vif_df["Multicollinearity"] = vif_df["VIF"].apply(interpret_vif)
+
+    # Sort the DataFrame by VIF values in descending order
+    vif_sorted = vif_df.sort_values(by='VIF', ascending=False)
+
+    # Format the VIF values for better readability
+    vif_formatted = format_df(vif_sorted, small_num_cols=['VIF'], decimal=decimal)
+
+    return vif_formatted
+
+def check_for_duplicates(*lists: List[str],
+                         df: Optional[pd.DataFrame] = None) -> None:
     """
-    Detects and summarizes outliers for the specified numeric columns in a
-    DataFrame, based on an IQR ratio.
+    Check for duplicate items (ex: column names) across multiple lists.
 
-    This function identifies outliers using Tukey's method, where outliers are
-    considered to be those data points that fall below Q1 - `ratio` * IQR or above
-    Q3 + `ratio` * IQR. You can exclude zeros from the calculations, as they can
-    appear as outliers and skew your results. You can also change the default IQR
-    `ratio` of  1.5. If outliers are found, they will be summarized in the returned
-    DataFrame. In addition, the distributions of the variables with outliers can be
-    plotted as boxplots.
-
-    Use this function to identify outliers during the early stages of exploratory
-    data analysis. With one line, you can see: total non-null, total zero values,
-    zero percent, outlier count, outlier percent, skewness, and kurtosis. You can
-    also visually spot outliers outside of the whiskers in the boxplots. Then you
-    can decide how you want to handle the outliers (ex: log transform, drop, etc.)
+    This function takes an arbitrary number of lists and checks for duplicate items
+    across the lists, as well as items appearing more than once within each list.
+    It prints a summary of the items and the lists they appear in. Additionally, if
+    a DataFrame is provided, it checks for any columns in the DataFrame that are
+    missing from the lists and prints them.
+
+    Use this function when you are organizing columns in a large DataFrame into
+    lists that represent their variable type (ex: num_columns, cat_columns). This
+    helps to ensure you haven't duplicated a column accidentally. And the optional
+    DataFrame check helps you identify columns that haven't been assigned to a list
+    yet. This is really useful when you're dealing with a large dataset.
 
     Parameters
     ----------
-    df : DataFrame
-        The DataFrame to analyze for outliers.
-    num_columns : List[str]
-        List of column names in `df` to check for outliers. These should be names
-        of columns with numerical data.
-    ratio : float, optional
-        The multiplier for IQR to determine the threshold for outliers. Default
-        is 1.5.
-    exclude_zeros : bool, optional
-        If set to True, zeros are excluded from the outlier calculation. Default
-        is False.
-    plot : bool, optional
-        If set to True, box plots of outlier distributions are displayed. Default
-        is False.
-    width : int, optional
-        The width of the plot figure. This parameter only has an effect if `plot`
-        is True. Default is 15.
-    height : int, optional
-        The height of each subplot row. This parameter only has an effect if `plot`
-        is True. Default is 2.
+    *lists : List[str]
+        An arbitrary number of lists containing items (ex: column names) to check
+        for duplicates.
+    df : pd.DataFrame, optional
+        A DataFrame to check for missing columns that are not present in the lists.
+        Default is None.
 
     Returns
     -------
-    pd.DataFrame
-        A DataFrame summarizing the outliers found in each specified column,
-        including the number of non-null and zero values, percentage of zero
-        values, count of outliers, percentage of outliers, and measures of skewness
-        and kurtosis.
+    None
+        The function prints the duplicate items, the lists they appear in, and any
+        missing columns in the DataFrame (if provided).
 
     Examples
     --------
-    Prepare the data for the examples:
+    Prepare data for examples, with intentional duplicates:
 
-    >>> np.random.seed(0)  # For reproducibility
-    >>> pd.set_option('display.max_columns', None)  # For test consistency
-    >>> pd.set_option('display.width', None)  # For test consistency
-    >>> df = pd.DataFrame({
-    ...     'A': np.random.randn(100),
-    ...     'B': np.random.exponential(scale=2.0, size=100),
-    ...     'C': np.random.randn(100)
-    ... })
-    >>> df.at[2, 'A'] = 0; df.at[5, 'A'] = 0  # Assign some zeros
-    >>> df.at[3, 'B'] = np.nan; df.at[7, 'B'] = np.nan  # Assign some NaNs
-    >>> num_columns = ['A', 'B', 'C']  # Store numeric columns
-
-    Example 1: Create a dataframe that lists outlier statistics:
-
-    >>> outlier_summary = get_outliers(df, num_columns)
-    >>> print(outlier_summary)
-      Column  Total Non-Null  Total Zero  Zero Percent  Outlier Count  Outlier Percent  Skewness  Kurtosis
-    1      B              98           0           0.0              4             4.08      2.62     10.48
-    0      A             100           2           2.0              1             1.00      0.01     -0.25
-    2      C             100           0           0.0              1             1.00     -0.03      0.19
-
-    Example 2: Create a dataframe that lists outlier statistics, excluding zeros:
-
-    >>> outlier_summary = get_outliers(df, num_columns, exclude_zeros=True)
-    >>> print(outlier_summary)
-      Column  Total Non-Null  Total Zero  Zero Percent  Outlier Count  Outlier Percent  Skewness  Kurtosis
-    0      B              98           0           0.0              4             4.08      2.62     10.48
-    1      C             100           0           0.0              1             1.00     -0.03      0.19
-    """
-    outlier_data = []
-
-    for col in num_columns:
-        non_null_data = df[col].dropna()
-        if exclude_zeros:
-            non_null_data = non_null_data[non_null_data != 0]
+    >>> df = pd.DataFrame({'age': [], 'height': [], 'weight': [], 'gender': [],
+    ... 'city': [], 'country': []})
+    >>> num_cols = ['age', 'height', 'weight']
+    >>> cat_cols = ['gender', 'age', 'country', 'country']
+
+    Example 1: Check for duplicate column names in two lists:
+
+    >>> check_for_duplicates(num_cols, cat_cols)
+    Items appearing in more than one list, or more than once per list:
+    age (2): num_cols, cat_cols
+    country (2): cat_cols, cat_cols
+
+    Fix the duplicate column:
+
+    >>> cat_cols = ['gender', 'country']
+
+    Example 2: Check for duplicates, and look for missing columns in a DataFrame:
+
+    >>> check_for_duplicates(num_cols, cat_cols, df=df)
+    Items appearing in more than one list, or more than once per list:
+    None.
+    <BLANKLINE>
+    Columns in the dataframe missing from the lists:
+    city
+
+    Fix the missing column:
+
+    >>> cat_cols = ['gender', 'city', 'country']
+
+    Final check:
+
+    >>> check_for_duplicates(num_cols, cat_cols, df=df)
+    Items appearing in more than one list, or more than once per list:
+    None.
+    <BLANKLINE>
+    Columns in the dataframe missing from the lists:
+    None.
+    """
+    # Get the frame and local variables of the caller
+    caller_frame = inspect.currentframe().f_back
+    caller_locals = caller_frame.f_locals
+
+    # Create a dictionary to store the mapping of columns to the lists they appear in
+    column_lists_map = {}
+
+    # Iterate over each list passed as an argument
+    for lst in lists:
+        # Get the name of the list variable from the caller's local variables
+        list_name = [name for name, value in caller_locals.items() if value is lst][0]
+        # Iterate over each column in the current list
+        for column in lst:
+            if column not in column_lists_map:
+                # If the column is not in the map, add it with the current list name
+                column_lists_map[column] = [list_name]
+            else:
+                # Append the current list name, even if it exists, to check
+                # for duplicated items or column names within the same list
+                column_lists_map[column].append(list_name)
+
+    # Create a dictionary of duplicate columns and the lists they appear in
+    duplicates = {column: lists for column, lists in column_lists_map.items() if len(lists) > 1}
+
+    # Print the summary of duplicate columns
+    print("Items appearing in more than one list, or more than once per list:")
+    if duplicates:
+        for column, lists in duplicates.items():
+            print(f"{column} ({len(lists)}): {', '.join(lists)}")
+    else:
+        print("None.")
+
+    # If a DataFrame is passed, check for column names that are missing from the lists
+    if df is not None:
+        all_columns = column_lists_map.keys()
+        missing_columns = set(df.columns) - set(all_columns)
+        print("\nColumns in the dataframe missing from the lists:")
+        if missing_columns:
+            for column in missing_columns:
+                print(column)
         else:
-            non_null_data = non_null_data
+            print("None.")
 
-        if non_null_data.empty:
-            continue
 
-        Q1 = np.percentile(non_null_data, 25)
-        Q3 = np.percentile(non_null_data, 75)
-        IQR = iqr(non_null_data)
-
-        lower_bound = Q1 - ratio * IQR
-        upper_bound = Q3 + ratio * IQR
-
-        outliers = non_null_data[(non_null_data < lower_bound) | (non_null_data > upper_bound)]
-        outlier_count = outliers.count()
-        total_non_null = non_null_data.count()
-        total_zero = non_null_data[non_null_data == 0].count()
-        zero_percent = round((total_zero / total_non_null) * 100, 2)
-
-        if outlier_count > 0:
-            percentage = round((outlier_count / total_non_null) * 100, 2)
-            skewness = round(non_null_data.skew(), 2)
-            kurtosis = round(non_null_data.kurt(), 2)
-            outlier_data.append([col, total_non_null, total_zero, zero_percent, outlier_count, percentage, skewness, kurtosis])
-
-    outlier_df = pd.DataFrame(outlier_data, columns=['Column', 'Total Non-Null', 'Total Zero', 'Zero Percent', 'Outlier Count',
-                                                     'Outlier Percent', 'Skewness', 'Kurtosis'])
-    outlier_df = outlier_df.sort_values(by='Outlier Percent', ascending=False)
-
-    if plot:
-        plt.figure(figsize=(width, len(outlier_df) * height))
-        plot_index = 1
-
-        for index, row in outlier_df.iterrows():
-            plt.subplot(len(outlier_df) // 2 + len(outlier_df) % 2, 2, plot_index)
-            sns.boxplot(x=df[row['Column']], orient='h')
-            plt.title(f"{row['Column']}, Outliers: {row['Outlier Count']} ({row['Outlier Percent']}%)")
-
-            plot_index += 1
-
-        plt.tight_layout()
-        plt.show()
-
-    return outlier_df
-
-
-def get_unique(
-        df: DataFrame,
-        n: int = 20,
-        sort: str = 'count',
-        show_list: bool = True,
-        count: bool = True,
-        percent: bool = True,
-        plot: bool = False,
-        cont: bool = False,
-        strip: bool = False,
-        dropna: bool = False,
-        fig_size: Tuple[int, int] = (6, 4),
-        rotation: int = 45
-) -> None:
-    """
-    Print the unique values of all variables below a threshold `n`, including
-    counts and percentages.
-
-    This function examines the unique values of all the variables in a DataFrame.
-    If the number is below a threshold `n`, it will list their unique values. For
-    each value, it prints out the count and percentage of the dataset with that
-    value. You can change the sort, and there are options to strip single quotes
-    from the variable names, or exclude NaN values. You can optionally show
-    descriptive statistics for the continuous variables able the 'n' threshold, or
-    display simple plots.
-
-    Use this to quickly examine the features of your dataset at the beginning of
-    exploratory data analysis. Use `df.nunique()` to first determine how many
-    unique values each variable has, and identify a number that likely separates
-    the categorical from continuous numeric variables. Then run get_unique using
-    that number as `n` (this avoids iterating over continuous data).
+def extract_coef(
+        grid_or_pipe: Union[GridSearchCV, Pipeline],
+        X: pd.DataFrame,
+        format: bool = True,
+        decimal: int = 2,
+        debug: bool = False
+) -> pd.DataFrame:
+    """
+    Extract feature names and coefficients from a trained model.
+
+    This function traverses through the steps of a GridSearchCV or
+    Pipeline object and extracts the feature names and coefficients from
+    the final trained model. It attempts to handle transformations such as
+    ColumnTransformer and feature scaling steps. However, due to the complexity
+    of some transformations, and inconsistent support on tracking feature
+    names, the final output feature names may be different than the input.
+
+    Note: This function currently supports only single target regression
+    problems. It also checks against a list of known classes that support
+    coefficient extraction. This list may not be comprehensive.
 
     Parameters
     ----------
-    df : DataFrame
-        The dataframe that contains the variables you want to analyze.
-    n : int, optional
-        The maximum number of unique values to consider. This helps to avoid
-        iterating over continuous data. Default is 20.
-    sort : str, optional
-        Determines the sorting of unique values:
-        - 'name' - sorts alphabetically/numerically,
-        - 'count' - sorts by count of unique values (descending),
-        - 'percent' - sorts by percentage of each unique value (descending).
-        Default is 'count'.
-    show_list : bool, optional
-        If True, shows the list of unique values. Default is True.
-    count : bool, optional
-        If True, shows counts of each unique value. Default is False.
-    percent : bool, optional
-        If True, shows the percentage of each unique value. Default is False.
-    plot : bool, optional
-        If True, shows a basic chart for each variable. Default is False.
-    cont : bool, optional
-        If True, analyzes variables with unique values greater than 'n'
-        as continuous data. Default is False.
-    strip : bool, optional
-        If True, removes single quotes from the variable names. Default is False.
-    dropna : bool, optional
-        If True, excludes NaN values from unique value lists. Default is False.
-    fig_size : tuple, optional
-        Size of figure if plotting is enabled. Default is (6, 4).
-    rotation : int, optional
-        Rotation angle of X axis ticks if plotting is enabled. Default is 45.
+    grid_or_pipe : Union[GridSearchCV, Pipeline]
+        A trained GridSearchCV or Pipeline object containing the model.
+    X : pd.DataFrame
+        The input DataFrame used during training, to get the original
+        feature names.
+    format : bool, optional
+        Applies formatting to the results to make it easier to read, but
+        converts numbers to strings. Default is True.
+    decimal : int, optional
+        The number of decimals to round to when displaying output.
+        Default is 2.
+    debug : bool, optional
+        If True, print debugging information during the extraction
+        process. Default is False.
 
     Returns
     -------
-    None
-        The function prints the analysis directly.
+    pd.DataFrame
+        A DataFrame with two columns: 'Feature' (the names of the
+        selected features) and 'Coefficient' (the corresponding
+        coefficients of the features).
 
-    Examples
-    --------
-    Prepare the data for the examples:
+    Example
+    -------
+    Prepare sample data for the example:
 
-    >>> df = pd.DataFrame({'Animal': ["'Cat'", "'Dog'", "'Cat'", "'Mountain Lion'",
-    ...     "'Dog'", "'Dog'"],
-    ...     'Sex': ['Male', 'Female', 'Male', 'Male', 'Female', np.nan],
-    ...     'Weight': [6.5, 12.5, 7.7, 84.1, 22.3, 29.2]
-    ... })
+    >>> from sklearn.datasets import fetch_california_housing
+    >>> from sklearn.pipeline import Pipeline
+    >>> from sklearn.linear_model import Ridge
+    >>> from sklearn.preprocessing import StandardScaler
+    >>> X, y = fetch_california_housing(return_X_y=True)
+    >>> X = pd.DataFrame(X, columns=['MedInc', 'HouseAge', 'AveRooms',
+    ...                               'AveBedrms', 'Population', 'AveOccup',
+    ...                               'Latitude', 'Longitude'])
+
+    Create and fit a model pipeline:
+
+    >>> pipe = Pipeline([
+    ...     ('scaler', StandardScaler()),
+    ...     ('model', Ridge())
+    ... ])
+    >>> pipe.fit(X, y)
+    Pipeline(steps=[('scaler', StandardScaler()), ('model', Ridge())])
+
+    Example 1: Extract feature names and coefficients from the fitted model:
+
+    >>> extract_coef(pipe, X, decimal=4)
+          Feature Coefficient
+    0      MedInc      0.8296
+    1    HouseAge      0.1188
+    2    AveRooms     -0.2654
+    3   AveBedrms      0.3055
+    4  Population     -0.0045
+    5    AveOccup     -0.0393
+    6    Latitude     -0.8993
+    7   Longitude     -0.8699
+
+    Example 2: Extract feature names adn coefficients without formatting:
+
+    >>> extract_coef(pipe, X, format=False)
+          Feature Coefficient
+    0      MedInc    0.829593
+    1    HouseAge    0.118817
+    2    AveRooms   -0.265397
+    3   AveBedrms    0.305525
+    4  Population    -0.00448
+    5    AveOccup    -0.03933
+    6    Latitude   -0.899266
+    7   Longitude   -0.869916
+
+    Example 3: Extract coefficients from a grid search object:
+
+    >>> parameters = {'model__alpha': [1.0, 0.5]}
+    >>> grid = GridSearchCV(pipe, parameters)
+    >>> grid.fit(X, y)  #doctest: +NORMALIZE_WHITESPACE
+    GridSearchCV(estimator=Pipeline(steps=[('scaler', StandardScaler()),
+                                           ('model', Ridge())]),
+                 param_grid={'model__alpha': [1.0, 0.5]})
+    >>> extract_coef(grid, X)
+          Feature Coefficient
+    0      MedInc        0.83
+    1    HouseAge        0.12
+    2    AveRooms       -0.27
+    3   AveBedrms        0.31
+    4  Population       -0.00
+    5    AveOccup       -0.04
+    6    Latitude       -0.90
+    7   Longitude       -0.87
+    """
+    # List of classes that support the .coef_ attribute
+    SUPPORTED_COEF_CLASSES = (
+        LogisticRegression, LogisticRegressionCV, PassiveAggressiveClassifier,
+        Perceptron, RidgeClassifier, RidgeClassifierCV, SGDClassifier, SGDOneClassSVM,
+        LinearRegression, Ridge, RidgeCV, SGDRegressor, ElasticNet, ElasticNetCV,
+        Lars, LarsCV, Lasso, LassoCV, LassoLars, LassoLarsCV, LassoLarsIC,
+        OrthogonalMatchingPursuit, OrthogonalMatchingPursuitCV, ARDRegression,
+        BayesianRidge, HuberRegressor, QuantileRegressor, RANSACRegressor,
+        TheilSenRegressor
+    )
+
+    def supports_coef(estimator):
+        """Check if estimator supports .coef_"""
+        return isinstance(estimator, SUPPORTED_COEF_CLASSES)
+
+    # Determine the type of the passed object and set flags
+    if hasattr(grid_or_pipe, 'best_estimator_'):
+        estimator = grid_or_pipe.best_estimator_
+        is_grid = True
+        is_pipe = False
+        if debug:
+            print('Grid: ', is_grid)
+    else:
+        estimator = grid_or_pipe
+        is_pipe = True
+        is_grid = False
+        if debug:
+            print('Pipe: ', is_pipe)
+
+    # Initial setup
+    current_features = list(X.columns)
+    if debug:
+        print('current_features: ', current_features)
+    mapping = pd.DataFrame({
+        'feature_name': current_features,
+        'intermediate_name1': current_features,
+        'selected': [True] * len(current_features),
+        'coefficients': [None] * len(current_features)
+    })
+
+    for step_name, step_transformer in estimator.named_steps.items():
+        if debug:
+            print(f"Processing step: {step_name} in {step_transformer}")
+
+        # If transformer is a ColumnTransformer
+        if isinstance(step_transformer, ColumnTransformer):
+            new_features = []
+            for name, trans, columns in step_transformer.transformers_:
+                if hasattr(trans, 'get_feature_names_out'):
+                    try:
+                        if hasattr(trans, 'feature_names_in_'):
+                            out_features = trans.get_feature_names_out(trans.feature_names_in_)
+                        else:
+                            out_features = trans.get_feature_names_out(columns)
+                    except ValueError:
+                        out_features = [f"{name}_{i}" for i in range(trans.transform(X.iloc[:, columns].values).shape[1])]
+                else:
+                    out_features = columns
+                new_features.extend(out_features)
 
-    Example 1: Print unique values below a threshold of 3:
+            current_features = new_features
+            mapping = pd.DataFrame({
+                'feature_name': current_features,
+                'intermediate_name1': current_features,
+                'selected': [True] * len(current_features),
+                'coefficients': [None] * len(current_features)
+            })
+            if debug:
+                print("Mapping: ", mapping)
+
+        # Reduction
+        elif hasattr(step_transformer, 'get_support'):
+            mask = step_transformer.get_support()
+            mapping.loc[mapping['feature_name'].isin(current_features), 'selected'] = mask
+            current_features = mapping[mapping['selected']]['feature_name'].tolist()
+
+
+    # If there's a model with coefficients in this step, update coefficients
+    if supports_coef(step_transformer):
+        coefficients = step_transformer.coef_.ravel()
+        selected_rows = mapping[mapping['selected']].index
+        if debug:
+            print("Coefficients: ", coefficients)
+            print(f"Number of coefficients: {len(coefficients)}")  # Debugging
+            print(f"Number of selected rows: {len(selected_rows)}")  # Debugging
 
-    >>> get_unique(df, n=3)
-    <BLANKLINE>
-    CATEGORICAL: Variables with unique values equal to or below: 3
-    <BLANKLINE>
-    Animal has 3 unique values:
-    <BLANKLINE>
-        'Dog'               3   50.0%
-        'Cat'               2   33.33%
-        'Mountain Lion'     1   16.67%
-    <BLANKLINE>
-    Sex has 3 unique values:
-    <BLANKLINE>
-        Male         3   50.0%
-        Female       2   33.33%
-        nan          1   16.67%
+        if len(coefficients) == len(selected_rows):
+            mapping.loc[selected_rows, 'coefficients'] = coefficients.tolist()
+        else:
+            print(f"Mismatch in coefficients and selected rows for step: {step_name}")
+
+    # For transformers inside ColumnTransformer
+    if isinstance(step_transformer, ColumnTransformer):
+        if debug:
+            print("ColumnTransformer:", step_transformer)
+        transformers = step_transformer.transformers_
+        if debug:
+            print("Transformers: ", transformers)
+        new_features = []  # Collect new features from this step
+        for name, trans, columns in transformers:
+            # OneHotEncoder or similar expanding transformers
+            if hasattr(trans, 'get_feature_names_out'):
+                out_features = list(trans.get_feature_names_out(columns))
+                new_features.extend(out_features)
+                if debug:
+                    print("Out features: ", out_features)
+                    print("New features: ", new_features)
+            else:
+                new_features.extend(columns)
 
-    Example 2: Sort values by name, strip single quotes, drop NaN:
+        current_features = new_features
 
-    >>> get_unique(df, n=3, sort='name', strip=True, dropna=True)
-    <BLANKLINE>
-    CATEGORICAL: Variables with unique values equal to or below: 3
-    <BLANKLINE>
-    Animal has 3 unique values:
-    <BLANKLINE>
-        Cat                 2   33.33%
-        Dog                 3   50.0%
-        Mountain Lion       1   16.67%
-    <BLANKLINE>
-    Sex has 2 unique values:
-    <BLANKLINE>
-        Female       2   40.0%
-        Male         3   60.0%
-    """
-    # Calculate # of unique values for each variable in the dataframe
-    var_list = df.nunique(axis=0, dropna=dropna)
+        # Update mapping based on current_features
+        mapping = pd.DataFrame({
+            'feature_name': current_features,
+            'intermediate_name1': current_features,
+            'selected': [True] * len(current_features),
+            'coefficients': [None] * len(current_features)
+        })
+        if debug:
+            print("Mapping: ", mapping)
+    # Filtering the final selected features and their coefficients
+    final_data = mapping[mapping['selected']]
 
-    # Iterate through each categorical variable in the list below n
-    print(f"\nCATEGORICAL: Variables with unique values equal to or below: {n}")
-    for i in range(len(var_list)):
-        var_name = var_list.index[i]
-        unique_count = var_list.iloc[i]
-
-        # If unique value count is less than n, get the list of values, counts, percentages
-        if unique_count <= n:
-            number = df[var_name].value_counts(dropna=dropna)
-            if dropna:
-                total_count = df[var_name].dropna().shape[0]  # Count of non-NaN entries
-            else:
-                total_count = df[var_name].shape[0]  # Total entries, including NaN
-            perc = round(number / total_count * 100, 2)
-            orig = number.index
-            # Strip out the single quotes
-            name = [str(n) for n in number.index]
-            name = [n.strip('\'') for n in name]
-            # Store everything in dataframe uv for consistent access and sorting
-            uv = pd.DataFrame({'orig': orig, 'name': name, 'number': number, 'perc': perc})
-
-            # Sort the unique values by name or count, if specified
-            if sort == 'name':
-                uv = uv.sort_values(by='name', ascending=True)
-            elif sort == 'count':
-                uv = uv.sort_values(by='number', ascending=False)
-            elif sort == 'percent':
-                uv = uv.sort_values(by='perc', ascending=False)
-
-            # Print out the list of unique values for each variable
-            if show_list:
-                print(f"\n{var_name} has {unique_count} unique values:\n")
-                for w, x, y, z in uv.itertuples(index=False):
-                    # Decide on to use stripped name or not
-                    if strip:
-                        w = x
-                    # Put some spacing after the value names for readability
-                    w_str = str(w)
-                    w_pad_size = uv.name.str.len().max() + 7
-                    w_pad = w_str + " " * (w_pad_size - len(w_str))
-                    y_str = str(y)
-                    y_pad_max = uv.number.max()
-                    y_pad_max_str = str(y_pad_max)
-                    y_pad_size = len(y_pad_max_str) + 3
-                    y_pad = y_str + " " * (y_pad_size - len(y_str))
-                    if count and percent:
-                        print("    " + str(w_pad) + str(y_pad) + str(z) + "%")
-                    elif count:
-                        print("    " + str(w_pad) + str(y))
-                    elif percent:
-                        print("    " + str(w_pad) + str(z) + "%")
-                    else:
-                        print("    " + str(w))
-
-            # Plot countplot if plot=True
-            if plot:
-                print("\n")
-                plt.figure(figsize=fig_size)
-                if strip:
-                    if sort == 'count':
-                        sns.barplot(data=uv, x='name', y='number', order=uv.sort_values('number', ascending=False).name)
-                    else:
-                        sns.barplot(data=uv, x=uv.loc[0], y='number', order=uv.sort_values('name', ascending=True).name)
-                else:
-                    if sort == 'count':
-                        sns.barplot(data=uv, x='orig', y='number', order=uv.sort_values('number', ascending=False).orig)
-                    else:
-                        sns.barplot(data=uv, x='orig', y='number', order=uv.sort_values('orig', ascending=True).orig)
-                plt.title(var_name)
-                plt.xlabel('')
-                plt.ylabel('')
-                plt.xticks(rotation=rotation)
-                plt.grid(False)
-                plt.show()
-
-    if cont:
-        # Iterate through each continuous variable in the list above n
-        print(f"\nCONTINUOUS: Variables with unique values greater than: {n}")
-        for i in range(len(var_list)):
-            var_name = var_list.index[i]
-            unique_count = var_list.iloc[i]
-
-            if unique_count > n:
-                print(f"\n{var_name} has {unique_count} unique values:\n")
-                print(var_name)
-                print(df[var_name].describe())
-
-                # Plot countplot if plot=True
-                if plot:
-                    print("\n")
-                    plt.figure(figsize=fig_size)
-                    sns.histplot(data=df, x=var_name)
-                    plt.title(var_name)
-                    plt.xlabel('')
-                    plt.ylabel('')
-                    plt.xticks(rotation=rotation)
-                    plt.grid(False)
-                    plt.show()
+    # Rename the columns to "Feature" and "Coefficient"
+    final_data = final_data[['feature_name', 'coefficients']].rename(columns={'feature_name': 'Feature', 'coefficients': 'Coefficient'})
 
+    # Format the coefficient values for better readability
+    if format:
+        final_data = format_df(final_data, small_num_cols=['Coefficient'], decimal=decimal)
 
-from typing import List, Dict, Optional
+    return final_data
 
-def plot_3d(
+
+def format_df(
         df: pd.DataFrame,
-        x: str,
-        y: str,
-        z: str,
-        color: Optional[str] = None,
-        color_discrete_sequence: Optional[List[str]] = None,
-        color_discrete_map: Optional[Dict[str, str]] = None,
-        color_continuous_scale: Optional[List[str]] = None,
-        x_scale: str = 'linear',
-        y_scale: str = 'linear',
-        z_scale: str = 'linear',
-        height: int = 600,
-        width: int = 1000,
-        font_size: int = 10
-) -> None:
-    """
-    Create a 3D scatter plot using Plotly Express.
-
-    This function generates an interactive 3D scatter plot using the
-    Plotly Express library. It allows for customization of the `x`, `y`, and `z`
-    axes, as well as color coding of the points based on the column specified
-    for `color` (similar to the `hue` parameter in Seaborn). A `color_discrete_map`
-    dictionary can be passed to map specific values of the `color` column to
-    colors. Alternatively, you can just pass a `color_discrete_map` or
-    `color_continuous_scale` depending on the type of values in the `color`
-    column. Onlye 1 of these 3 coloring methods should be used at a time. The plot
-    can also be displayed with either a linear or logarithmic scale on each axis
-    by setting `x_scale`, `y_scale`, or `z_scale` from 'linear' to 'log'.
-
-    Use this function to visualize and explore relationships between three
-    variables in a dataset, with the option to color code the points based
-    on a fourth variable. It is a great way to visualize the top 3 principal
-    components, dimensioned by the target variable.
+        large_num_cols: Optional[List[str]] = None,
+        small_num_cols: Optional[List[str]] = None,
+        decimal: int = 2
+) -> pd.DataFrame:
+    """
+    Format columns of a DataFrame as either large or small numbers.
+
+    This function formats the specified columns in the input DataFrame.
+    Large numbers are formatted with commas as thousands separators and
+    no decimal places. Small numbers are formatted with a specified
+    number of decimal places (they will have commas as well). Use
+    `decimal` to define how many decimal places to display.
+
+    Use this function when you need to format specific columns in a
+    DataFrame for better readability or presentation purposes.
 
     Parameters
     ----------
     df : pd.DataFrame
-        The input DataFrame containing the data to be plotted.
-    x : str
-        The column name to be used for the x-axis.
-    y : str
-        The column name to be used for the y-axis.
-    z : str
-        The column name to be used for the z-axis.
-    color : str, optional
-        The column name to be used for color coding the points. Default is
-        None.
-    color_discrete_sequence : List[str], optional
-        Strings should define valid CSS-colors. When `color` is set and the values
-        in the corresponding column are not numeric, values in that column are
-        assigned colors by cycling through `color_discrete_sequence` in the order
-        described in `category_orders`. Various color sequences are available in
-        `plotly.express.colors.qualitative`. Default is None.
-    color_discrete_map : Dict[str, str], optional
-        String values should define valid CSS-colors. Used to assign specific
-        colors values in the `color` column. Default is None.
-    color_continuous_scale : List[str], optional
-        Strings should define valid CSS-colors. This list is used to build a
-        continuous color scale when the `color` column contains numeric data.
-        Various color scales are available in `plotly.express.colors.sequential`,
-        `plotly.express.colors.diverging`, and `plotly.express.colors.cyclical`.
-        Default is None.
-    x_scale : str, optional
-        The scale type for the X axis. Use 'log' for logarithmic scale.
-        Default is 'linear'.
-    y_scale : str, optional
-        The scale type for the Y axis. Use 'log' for logarithmic scale.
-        Default is 'linear'.
-    z_scale : str, optional
-        The scale type for the Z axis. Use 'log' for logarithmic scale.
-        Default is 'linear'.
-    height : int, optional
-        The height of the plot in pixels.
-        Default is 600.
-    width : int, optional
-        The width of the plot in pixels.
-        Default is 1000.
-    font_size : int, optional
-        The size of the font used in the plot.
-        Default is 10.
+        The input DataFrame containing the columns to be formatted.
+    large_num_cols : List[str], optional
+        List of column names containing large numbers to be formatted with
+        commas as thousands separators, no decimals. Default is None.
+    small_num_cols : List[str], optional
+        List of column names containing small numbers to be formatted with
+        a specified number of decimal places. Default is None.
+    decimal : int, optional
+        The number of decimal places to display for small numbers. Default
+        is 2.
 
     Returns
     -------
-    None
-        The function displays the interactive 3D scatter plot using Plotly
-        Express.
+    pd.DataFrame
+        A new DataFrame with the specified columns formatted.
 
     Examples
     --------
     Prepare the data for the examples:
 
     >>> df = pd.DataFrame({
-    ...     'X': [1, 2, 3, 4, 5],
-    ...     'Y': [2, 4, 6, 8, 10],
-    ...     'Z': [3, 6, 9, 12, 15],
-    ...     'Category': ['A', 'B', 'A', 'B', 'A'],
-    ...     'Continuous': [10, 20, 30, 40, 50]
+    ...     'A': [112345697, 28799522, 391039492, 10959013409, 3522343059],
+    ...     'B': [0.123401, 0.234501, 0.345601, 0.456701, 0.567801],
+    ...     'C': ['X', 'Y', 'Z', 'X', 'Y']
     ... })
+    >>> df
+                 A         B  C
+    0    112345697  0.123401  X
+    1     28799522  0.234501  Y
+    2    391039492  0.345601  Z
+    3  10959013409  0.456701  X
+    4   3522343059  0.567801  Y
+
+    Example 1: Format large numbers and small numbers with default decimal places:
+
+    >>> formatted_df = format_df(df, large_num_cols=['A'], small_num_cols=['B'])
+    >>> formatted_df
+                    A     B  C
+    0     112,345,697  0.12  X
+    1      28,799,522  0.23  Y
+    2     391,039,492  0.35  Z
+    3  10,959,013,409  0.46  X
+    4   3,522,343,059  0.57  Y
+
+    Example 2: Format small numbers with a specified number of decimal places:
+
+    >>> formatted_df = format_df(df, large_num_cols=['A'], small_num_cols=['B'],
+    ...                          decimal=4)
+    >>> formatted_df
+                    A       B  C
+    0     112,345,697  0.1234  X
+    1      28,799,522  0.2345  Y
+    2     391,039,492  0.3456  Z
+    3  10,959,013,409  0.4567  X
+    4   3,522,343,059  0.5678  Y
+    """
+    # Function to format a column
+    def format_columns(val, col_type):
+        # Check if value is NaN or not a numeric type; return as is if true
+        if pd.isna(val) or not isinstance(val, (int, float)):
+            return val
+        if col_type == "large":
+            return '{:,.0f}'.format(val)
+        elif col_type == "small":
+            return f'{{:,.{decimal}f}}'.format(val)
+
+    # Create a copy of the input DataFrame to avoid modifying the original
+    formatted_df = df.copy()
+
+    # Format columns with large numbers
+    if large_num_cols:
+        for col in large_num_cols:
+            formatted_df[col] = formatted_df[col].apply(
+                lambda x: format_columns(x, "large")
+            )
+
+    # Format columns with small numbers
+    if small_num_cols:
+        for col in small_num_cols:
+            formatted_df[col] = formatted_df[col].apply(
+                lambda x: format_columns(x, "small")
+            )
 
-    Example 1: Create a basic 3D scatter plot:
+    return formatted_df
 
-    >>> plot_3d(df, x='X', y='Y', z='Z')
 
-    Example 2: Create a 3D scatter plot with default color coding, and log scale
-    on the X axis:
+def log_transform(
+        df: pd.DataFrame,
+        columns: Optional[List[str]] = None
+) -> pd.DataFrame:
+    """
+    Apply a log transformation to specified columns in a DataFrame.
 
-    >>> plot_3d(df, x='X', y='Y', z='Z', color='Category', x_scale='log')
+    This function applies a log transformation (base e) to the specified
+    columns of the input DataFrame. The log-transformed columns are
+    appended to the DataFrame with the suffix '_log'. If a column
+    contains a negative value, a log transformation is not possible. In this
+    case, a warning message will be printed, and the function will continue
+    and try to transform additional columns.
 
-    Example 3: Create a 3D scatter plot with a discrete color palette:
-
-    >>> plot_3d(df, x='X', y='Y', z='Z', color='Category',
-    ...         color_discrete_sequence=px.colors.qualitative.Prism)
-
-    Example 4: Create a 3D scatter plot with a continuous color palette:
-
-    >>> plot_3d(df, x='X', y='Y', z='Z', color='Continuous',
-    ...         color_continuous_scale=px.colors.sequential.Viridis)
-
-    Example 5: Create a 3D scatter plot with a custom discrete color map,
-    and adjust the height and width:
-
-    >>> category_color_map = {'A': px.colors.qualitative.D3[0],
-    ...                       'B': px.colors.qualitative.D3[1]}
-    >>> plot_3d(df, x='X', y='Y', z='Z', color='Category',
-    ...         color_discrete_map=category_color_map,
-    ...         height=800, width=1200)
-    """
-    # Create the 3D scatter plot and set the title
-    if color is not None:
-        # Handle mappings of values in 'color' column to 'color_discrete_map'
-        if color_discrete_map is not None:
-            fig = px.scatter_3d(df, x=x, y=y, z=z,
-                                color=color,
-                                color_discrete_map=color_discrete_map,
-                                height=height,
-                                width=width)
-        # Handle a discrete color palette
-        elif color_discrete_sequence is not None:
-            fig = px.scatter_3d(df, x=x, y=y, z=z,
-                                color=color,
-                                color_discrete_sequence=color_discrete_sequence,
-                                height=height,
-                                width=width)
-        # Handle a continuous color palette
-        elif color_continuous_scale is not None:
-            fig = px.scatter_3d(df, x=x, y=y, z=z,
-                                color=color,
-                                color_continuous_scale=color_continuous_scale,
-                                height=height,
-                                width=width)
-        # Handle no specified palette
-        else:
-            fig = px.scatter_3d(df, x=x, y=y, z=z,
-                                color=color,
-                                height=height,
-                                width=width)
-        title_text = f"{x}, {y}, {z} by {color}"
-    # No color specified
-    else:
-        fig = px.scatter_3d(df, x=x, y=y, z=z,
-                            height=height,
-                            width=width)
-        title_text = f"{x}, {y}, {z}"
-
-    # Adjust the 3D perspective and plot styling
-    fig.update_layout(title={'text': title_text, 'y': 0.9, 'x': 0.5,
-                             'xanchor': 'center', 'yanchor': 'top'},
-                      showlegend=True,
-                      scene_camera=dict(up=dict(x=0, y=0, z=1),
-                                        center=dict(x=0, y=0, z=-0.1),
-                                        eye=dict(x=1.5, y=-1.4, z=0.5)),
-                      margin=dict(l=0, r=0, b=0, t=0),
-                      scene=dict(xaxis=dict(backgroundcolor='white',
-                                            color='black',
-                                            gridcolor='#f0f0f0',
-                                            title=x,
-                                            title_font=dict(size=font_size),
-                                            tickfont=dict(size=font_size),
-                                            type=x_scale),
-                                 yaxis=dict(backgroundcolor='white',
-                                            color='black',
-                                            gridcolor='#f0f0f0',
-                                            title=y,
-                                            title_font=dict(size=font_size),
-                                            tickfont=dict(size=font_size),
-                                            type=y_scale),
-                                 zaxis=dict(backgroundcolor='lightgrey',
-                                            color='black',
-                                            gridcolor='#f0f0f0',
-                                            title=z,
-                                            title_font=dict(size=font_size),
-                                            tickfont=dict(size=font_size),
-                                            type=z_scale)))
-
-    # Update the marker style
-    fig.update_traces(marker=dict(size=3, opacity=1,
-                                  line=dict(color='black', width=0.1)))
-
-    # Display the plot
-    fig.show()
-
-
-def plot_charts(df: pd.DataFrame,
-                plot_type: str = 'both',
-                n: int = 10,
-                ncols: int = 2,
-                fig_width: int = 15,
-                subplot_height: int = 4,
-                rotation: int = 0,
-                cat_cols: Optional[List[str]] = None,
-                cont_cols: Optional[List[str]] = None,
-                dtype_check: bool = True,
-                sample_size: Optional[Union[int, float]] = None,
-                random_state: int = 42,
-                hue: Optional[str] = None,
-                color_discrete_map: Optional[Dict] = None,
-                normalize: bool = False,
-                kde: bool = False,
-                multiple: str = 'layer',
-                log_scale: bool = False,
-                ignore_zero: bool = False) -> None:
-    """
-    Display multiple bar plots and histograms for categorical and/or continuous
-    variables in a DataFrame, with an option to dimension by the specified `hue`.
-
-    This function allows you to plot a large number of distributions with one line
-    of code. You choose which type of plots to create by setting `plot_type` to
-    `cat`, `cont`, or `both`. Categorical variables are plotted with
-    `sns.barplot` ordered by descending value counts for a clean appearance.
-    Continuous variables are plotted with `sns.histplot`. There are two approaches
-    to identifying categorical vs. continuous variables: (a) you can specify
-    `cat_cols` and `cont_cols` as lists of the respective column names, or (b) you
-    can specify `n` as the dividing line, and any variable with `n` or lower unique
-    values will be treated as categorical. In addition, you can enable
-    `dtype_check` on the continuous columns to only include columns of data type
-    `int64` or `float64`.
-
-    For each type of variable, it creates a subplot layout that has `ncols`
-    columns, and is `fig_width` wide. It calculates how many rows are required to
-    display all the plots, and each row is `subplot_height` high. Specify `hue` if
-    you want to dimension the plots by another variable. You can set
-    `color_discrete_map` to a color mapping dictionary for the values of the `hue`
-    variable. You can also customize some parameters of the plots, such as
-    `rotation` of the X axis tick labels. For categorical variables, you can
-    normalize the plots to show proportions instead of counts by setting
-    `normalize` to True.
-
-    For histograms, you can display KDE lines with `kde`, and change how the `hue`
-    variable appears by setting `multiple`. If you have a large amount of data that
-    is taking too long to process, you can take a random sample of your data by
-    setting `sample_size` to either a count or proportion. To handle skewed data,
-    you have two options: (a) you can enable log scale on the X axis with
-    `log_scale`, and (b) you can ignore zero values with `ignore_zero` (these can
-    sometimes dominate the left end of a chart).
-
-    Use this function to quickly visualize the distributions of your data during
-    exploratory data analysis. With one line, you can produce a comprehensive
-    series of plots that can help you spot issues that will require handling during
-    data cleaning. By setting `hue` to your target y variable, you might be able to
-    catch glimpses of potential correlations or relationships.
+    Use this function when you need to log-transform skewed columns in
+    a DataFrame to approximate a more normal distribution for modeling.
 
     Parameters
     ----------
     df : pd.DataFrame
-        The dataframe containing the variables to be analyzed.
-    plot_type : str, optional
-        The type of charts to plot: 'cat' for categorical, 'cont' for continuous,
-        or 'both'. Default is 'both'.
-    n : int, optional
-        Threshold for distinguishing between categorical (≤ n unique values) and
-        continuous (> n unique values) variables. Default is 10.
-    ncols : int, optional
-        The number of columns in the subplot grid. Default is 2.
-    fig_width : int, optional
-        The width of the entire plot figure (not individual subplots). Default 15.
-    subplot_height : int, optional
-        The height of each subplot. Default is 4.
-    rotation : int, optional
-        The rotation angle for x-axis labels. Default is 0.
-    cat_cols : List[str], optional
-        List of column names to treat as categorical variables. Inferred from
-        unique count if not provided.
-    cont_cols : List[str], optional
-        List of column names to treat as continuous variables. Inferred from unique
-        count if not provided.
-    dtype_check : bool, optional
-        If True, considers only numeric types for continuous variables. Default is
-        True.
-    sample_size : int or float, optional
-        If provided, indicates the fraction (if < 1) or number (if ≥ 1) of samples
-        to draw from the dataframe for histograms.
-    random_state : int, optional. Default is 42
-        Set random state for reproducibility if using sample_size to perform a
-        random sample for histograms.
-    hue : str, optional
-        Name of the column for hue-based dimensioning in the plots.
-    color_discrete_map : Dict, optional
-        A color mapping dictionary for the values in the 'hue' variable.
-    normalize : bool, optional
-        If True, normalizes categorical plots to show proportions instead of
-        counts. Default is False.
-    kde : bool, optional
-        If True, shows Kernel Density Estimate (KDE) line on continuous histograms.
-        Default is False.
-    multiple : str, optional
-        Method to handle the hue variable in countplots. Options are 'layer',
-        'dodge', 'stack', 'fill'. Default is 'layer'.
-    log_scale : bool, optional
-        If True, uses log scale for continuous histograms. Default is False.
-    ignore_zero : bool, optional
-        If True, ignores zero values in continuous histograms. Default is False.
+        The input DataFrame containing the columns to be log-transformed.
+    columns : List[str], optional
+        List of column names to be log-transformed. If None, all columns
+        in the DataFrame will be considered. Default is None.
 
     Returns
     -------
-    None
-        Creates and displays plots without returning any value.
+    pd.DataFrame
+        A new DataFrame with the log-transformed columns appended. The
+        log-transformed columns have the suffix '_log'.
 
     Examples
     --------
-    Prepare the data for the examples:
+    Prepare data for the examples:
 
     >>> df = pd.DataFrame({
-    ...     'Category A': np.random.choice(['A', 'B', 'C'], size=100),
-    ...     'Category B': np.random.choice(['D', 'E', 'F', 'G', 'H', 'I', 'J'],
-    ...                                    size=100),
-    ...     'Measure 1': np.random.randn(100),
-    ...     'Measure 2': np.random.exponential(scale=2.0, size=100),
-    ...     'Target': np.random.choice(['Yes', 'No'], size=100)
+    ...     'A': [1, 2, 3, 4, 5],
+    ...     'B': [10, 20, 30, 40, 50],
+    ...     'C': [100, 200, 300, 400, 500]
     ... })
-    >>> cat_cols = ['Category A', 'Category B', 'Target']
-    >>> num_cols = ['Measure 1', 'Measure 2']
 
-    Example 1: Plot both categorical and continuous variables based on a boundary
-    of `n` unique values:
+    Example 1: Log-transform all columns:
+
+    >>> df_log = log_transform(df)
+    >>> df_log
+       A   B    C     A_log     B_log     C_log
+    0  1  10  100  0.693147  2.397895  4.615121
+    1  2  20  200  1.098612  3.044522  5.303305
+    2  3  30  300  1.386294  3.433987  5.707110
+    3  4  40  400  1.609438  3.713572  5.993961
+    4  5  50  500  1.791759  3.931826  6.216606
+
+    Example 2: Log-transform specific columns:
+
+    >>> df_log = log_transform(df, columns=['A', 'C'])
+    >>> df_log
+       A   B    C     A_log     C_log
+    0  1  10  100  0.693147  4.615121
+    1  2  20  200  1.098612  5.303305
+    2  3  30  300  1.386294  5.707110
+    3  4  40  400  1.609438  5.993961
+    4  5  50  500  1.791759  6.216606
+
+    Example 3: Encounter an error with a negative value:
+
+    >>> df['D'] = [-1, 2, 3, 4, 5]
+    >>> df['E'] = [5, 4, 3, 2, 1]
+    >>> df_log = log_transform(df)
+    WARNING: Column 'D' has negative values and cannot be log-transformed.
+    >>> df_log
+       A   B    C  D  E     A_log     B_log     C_log     E_log
+    0  1  10  100 -1  5  0.693147  2.397895  4.615121  1.791759
+    1  2  20  200  2  4  1.098612  3.044522  5.303305  1.609438
+    2  3  30  300  3  3  1.386294  3.433987  5.707110  1.386294
+    3  4  40  400  4  2  1.609438  3.713572  5.993961  1.098612
+    4  5  50  500  5  1  1.791759  3.931826  6.216606  0.693147
+    """
+    # Create a copy of the input DataFrame to avoid modifying the original
+    df_log = df.copy(deep=True)
 
-    >>> plot_charts(df, n=7)
+    # If columns parameter is not provided, use all columns in the DataFrame
+    if columns is None:
+        columns = df.columns
+
+    # Initialize an empty list to store the names of log-transformed columns
+    log_columns = []
+
+    # Iterate over the specified columns and apply log transformation
+    for col in columns:
+        # Check if the column has negative values
+        if df[col].min() < 0:
+            print(f"WARNING: Column '{col}' has negative values and cannot be log-transformed.")
+            # Skip this iteration and go to the next column
+            continue
 
-    Example 2: Plot only categorical variables using a column list, dimensioned
-    by `hue`:
+        # Apply log transformation and append the transformed column
+        df_log[col + '_log'] = np.log1p(df[col])
+        log_columns.append(col + '_log')
 
-    >>> plot_charts(df, plot_type='cat', cat_cols=cat_cols, hue='Target')
+    return df_log
+
+
+def model_summary(
+        model: keras.Model
+) -> pd.DataFrame:
+    """
+    Create a DataFrame summary of a Keras model's architecture and parameters.
 
-    Example 3: Customize the subplot width, number of columns, and rotation of
-    the X axis tick labels:
+    This function takes a Keras model as input and returns a pandas DataFrame
+    containing a summary of the model's architecture, including the model name,
+    type, total parameters, trainable parameters, non-trainable parameters, layer
+    names, types, activations, output shapes, the number of parameters, and the
+    parameter sizes in bytes for each layer.
+
+    Use this function when you need to obtain a structured summary of a Keras
+    model's architecture and parameters for analysis, reporting, or
+    visualization purposes. This is also used to test some other functions
+    where the model.summary() output varies enough to fail the test cases.
 
-    >>> plot_charts(df, plot_type='both', n=7, fig_width=20, ncols=3, rotation=90)
+    Parameters
+    ----------
+    model : keras.Model
+        The Keras model for which to generate the summary.
 
-    Example 4: Plot only histograms dimensioned by hue (stacked values), with KDE
-    lines, and X axis in log scale:
+    Returns
+    -------
+    pd.DataFrame
+        A pandas DataFrame containing the model summary, with columns for layer
+        name, type, activation, output shape, number of parameters, and parameter
+        size in bytes. Additional rows are included to show the total, trainable,
+        and non-trainable parameters along with their byte sizes.
 
-    >>> plot_charts(df, plot_type='cont', cont_cols=num_cols, hue='Target',
-    ...             multiple='stack', kde=True, log_scale=True)
+    Examples
+    --------
+    >>> pd.set_option('display.max_columns', None)  # For test consistency
+    >>> pd.set_option('display.width', None)  # For test consistency
+    >>> model = keras.Sequential([
+    ...     keras.layers.Input(shape=(10,), name='Input'),
+    ...     keras.layers.Dense(64, activation='relu', name='Dense_1'),
+    ...     keras.layers.Dense(32, activation='relu', name='Dense_2'),
+    ...     keras.layers.Dense(1, activation='sigmoid', name='Dense_3'),
+    ... ], name='Sequential_Model')
+    >>> model.build()
+    >>> model_summary(model)  #doctest: +NORMALIZE_WHITESPACE
+            Item                  Name         Type Activation Output Shape  Parameters    Bytes
+    0      Model      Sequential_Model   Sequential       None         None         NaN      NaN
+    1      Input                 Input  KerasTensor       None   (None, 10)         0.0      0.0
+    2      Layer               Dense_1        Dense       relu   (None, 64)       704.0   2816.0
+    3      Layer               Dense_2        Dense       relu   (None, 32)      2080.0   8320.0
+    4      Layer               Dense_3        Dense    sigmoid    (None, 1)        33.0    132.0
+    5  Statistic          Total Params         None       None         None      2817.0  11268.0
+    6  Statistic      Trainable Params         None       None         None      2817.0  11268.0
+    7  Statistic  Non-Trainable Params         None       None         None         0.0      0.0
     """
-    # Function to sample the data
-    def get_sample(df, sample_size):
-        # If sample_size is less than 1, treat it as a fraction
-        if sample_size < 1:
-            df_sample = df.sample(frac=sample_size, random_state=random_state)
-        # If sample_size is greater than or equalt to 1, treat it as an exact sample count
-        elif sample_size >= 1:
-            # Convert floats to int
-            sample_size = int(sample_size)
-            df_sample = df.sample(n=sample_size, random_state=random_state)
-        else:
-            print(f'WARNING: Could not sample. get_sample() called, but sample_size = {sample_size}.')
-            df_sample = df
-        # Return a sampled dataframe
-        return df_sample
-
-    # Function to plot categorical variables as bar plots
-    def plot_categorical(df, cols, ncols, fig_width, subplot_height, rotation, sample_size, hue, color_discrete_map, normalize):
-        # If sample_size is defined, draw a sample
-        df = get_sample(df, sample_size) if sample_size else df
-
-        # Warn when we're asked to normalize but don't have hue
-        if normalize and not hue:
-            print(f"WARNING: Can't normalize without hue. normalize = {normalize}, hue = {hue}.")
-
-        # Calculate the number of charts to plot
-        nplots = len(cols)
-        nrows = nplots//ncols
-        if nplots % ncols:
-            nrows += 1
-
-        # Create the figure with subplots
-        fig, axs = plt.subplots(nrows=nrows, ncols=ncols, figsize=(fig_width, nrows*subplot_height), constrained_layout=True)
-        if isinstance(axs, np.ndarray):
-            if len(axs.shape) > 1:
-                axs = axs.ravel()
-        else:
-            axs = [axs]
+    if not model.built:
+        print("Model is not built. Please build the model by calling `model.build(input_shape)` or by running `model.fit()` with some data.")
+        return pd.DataFrame()  # Return an empty DataFrame if the model is not built
+
+    def format_size(num_params):
+        return num_params * 4  # Assuming parameters are float32, each taking 4 bytes
+
+    layers_summary = []
+
+    # Model row
+    layers_summary.append(["Model", model.name, model.__class__.__name__, None, None, None, None])
+
+    # Input layer(s)
+    for input_tensor in model.inputs:
+        layers_summary.append([
+            "Input", input_tensor.name.split(':')[0], input_tensor.__class__.__name__,
+            None, str(input_tensor.shape), 0, 0
+        ])
+
+    # Layers
+    for layer in model.layers:
+        activation = getattr(layer, 'activation', None)
+        activation_name = activation.__name__ if activation else None
+        try:
+            output_shape = str(layer.output.shape)
+        except AttributeError:
+            output_shape = 'Unavailable'
+        layers_summary.append([
+            "Layer", layer.name, layer.__class__.__name__, activation_name,
+            output_shape, layer.count_params(), format_size(layer.count_params())
+        ])
+
+    # Statistics
+    total_params = model.count_params()
+    trainable_params = sum(tf.size(w).numpy() for w in model.trainable_variables)
+    non_trainable_params = total_params - trainable_params
+
+    layers_summary.append(["Statistic", "Total Params", None, None, None, total_params, format_size(total_params)])
+    layers_summary.append(["Statistic", "Trainable Params", None, None, None, trainable_params, format_size(trainable_params)])
+    layers_summary.append(["Statistic", "Non-Trainable Params", None, None, None, non_trainable_params, format_size(non_trainable_params)])
 
-        # Iterate through each categorical column to plot
-        for i, col in enumerate(cols):
-            if normalize and hue:
-                # Normalize the counts, but only if hue is defined
-                df_copy = df.copy()
-                data = df_copy.groupby(col)[hue].value_counts(normalize=True).rename('proportion').reset_index()
-                sns.barplot(data=data, x=col, y='proportion', hue=hue, palette=color_discrete_map, ax=axs[i])
-                axs[i].set_ylabel('Proportion', fontsize=12)
-            else:
-                # Sort the DataFrame by the count of occurrences of each category
-                if hue:
-                    # Handle the case where the column is the same as the hue variable
-                    if col == hue:
-                        sorted_df = df[[hue]].groupby(hue).value_counts().reset_index()
-                    else:
-                        sorted_df = df[[col, hue]].groupby(hue).value_counts().reset_index()
-                else:
-                    sorted_df = df[col].value_counts().reset_index()
-                    sorted_df.columns = [col, 'count']
+    summary_df = pd.DataFrame(layers_summary, columns=["Item", "Name", "Type", "Activation", "Output Shape", "Parameters", "Bytes"])
 
-                # Convert the column to string type to prevent numerical sorting
-                sorted_df[col] = sorted_df[col].astype(str)
+    return summary_df
 
-                # Generate a color palette
-                if hue:
-                    # Generate a color palette to match the number of hue values
-                    num_hue_values = len(sorted_df[hue].value_counts())
-                    if num_hue_values > 10:
-                        colors = sns.color_palette("husl", num_hue_values)
-                    elif color_discrete_map:
-                        colors = color_discrete_map
-                    else:
-                        colors = sns.color_palette("tab10", num_hue_values)
-                else:
-                    # Generate a color palette to match the number of categories
-                    num_categories = sorted_df.shape[0]
-                    if num_categories > 10:
-                        colors = sns.color_palette("husl", num_categories)
-                    elif color_discrete_map:
-                        colors = color_discrete_map
-                    else:
-                        colors = sns.color_palette("tab10", num_categories)
-
-                # Plot the appropriate chart
-                if hue == None:
-                    sns.barplot(data=sorted_df, x=col, y='count', hue=col, legend=False, palette=colors, ax=axs[i])
-                else:
-                    sns.barplot(data=sorted_df, x=col, y='count', hue=hue, palette=colors, ax=axs[i])
-                axs[i].set_ylabel('Count', fontsize=12)
-                axs[i].yaxis.set_major_formatter(FuncFormatter(thousands))
-            axs[i].set_xlabel(' ', fontsize=12)
-            axs[i].set_title(col, fontsize=16, pad=10)
-            axs[i].tick_params(axis='x', rotation=rotation)
-
-        # Remove empty subplots
-        for empty_subplot in axs[nplots:]:
-            fig.delaxes(empty_subplot)
-
-    # Function to plot continuous variables as histograms
-    def plot_continuous(df, cols, ncols, fig_width, subplot_height, sample_size, hue,
-                        color_discrete_map, kde, multiple, log_scale, ignore_zero):
-        # If sample_size is defined, draw a sample
-        df = get_sample(df, sample_size) if sample_size else df
-
-        # Calculate the number of charts to plot
-        nplots = len(cols)
-        nrows = nplots//ncols
-        if nplots % ncols:
-            nrows += 1
-
-        # Create the figure with subplots
-        fig, axs = plt.subplots(nrows=nrows, ncols=ncols, figsize=(fig_width, nrows * subplot_height), constrained_layout=True)
-        if isinstance(axs, np.ndarray):
-            if len(axs.shape) > 1:
-                axs = axs.ravel()
-        else:
-            axs = [axs]
 
-        # Iterate through each continuous column to plot
-        for i, col in enumerate(cols):
-            if hue is not None:
-                if ignore_zero:
-                    # Optionally ignore zero values in case they dwarf the rest of the chart
-                    sns.histplot(data=df[df[col]>0], x=col, hue=hue, palette=color_discrete_map, ax=axs[i], kde=kde, multiple=multiple, log_scale=log_scale)
-                else:
-                    sns.histplot(data=df, x=col, hue=hue, palette=color_discrete_map, ax=axs[i], kde=kde, multiple=multiple, log_scale=log_scale)
-            else:
-                if ignore_zero:
-                    sns.histplot(data=df[df[col]>0], x=col, ax=axs[i])
-                else:
-                    sns.histplot(data=df, x=col, ax=axs[i])
-            axs[i].set_title(col, fontsize=16, pad=10)
-            axs[i].set_ylabel('Count', fontsize=12)
-            axs[i].yaxis.set_major_formatter(FuncFormatter(thousands))
-            axs[i].set_xlabel(' ', fontsize=12)
-            axs[i].tick_params(axis='x', rotation=rotation)
-
-        # Remove empty subplots
-        for empty_subplot in axs[nplots:]:
-            fig.delaxes(empty_subplot)
-
-    # Start by getting counts of unique values
-    unique_count = df.nunique()
-
-    # Plot the categorical columns, if selected
-    if plot_type == 'cat' or plot_type == 'both':
-        if cat_cols is None:
-            # If columns not specified, find them based on less than or equal to 'n' unique values
-            cat_cols = unique_count[unique_count <= n].index.tolist()
-            # if hue in cat_cols:
-            #     cat_cols.remove(hue)
-        plot_categorical(df, cat_cols, ncols, fig_width, subplot_height, rotation, sample_size, hue, color_discrete_map, normalize)
-
-    # Plot the continuous columns, if selected
-    if plot_type == 'cont' or plot_type == 'both':
-        if cont_cols is None:
-            # If columns not specified, find them based on greater than 'n' unique values
-            cont_cols = unique_count[unique_count > n].index.tolist()
-        # If data type check is requested, filter out anything not int or float
-        if dtype_check:
-            cont_cols = [col for col in cont_cols if df[col].dtype in ['int64', 'float64']]
-        plot_continuous(df, cont_cols, ncols, fig_width, subplot_height, sample_size, hue, color_discrete_map, kde, multiple, log_scale, ignore_zero)
-
-
-def plot_corr(df: pd.DataFrame,
-              column: str,
-              n: int,
-              method: str = 'pearson',
-              size: Tuple[int, int] = (15, 8),
-              rotation: int = 45,
-              palette: str = 'RdYlGn',
-              decimal: int = 2) -> None:
-    """
-    Plot the top `n` correlations of one variable against others in a DataFrame.
-
-    This function generates a barplot that visually represents the correlations of
-    a specified column with other numeric columns in a DataFrame. It displays both
-    the strength (height of the bars) and the nature (color) of the correlations
-    (positive or negative). The function computes correlations using the specified
-    method and presents the strongest positive and negative correlations up to the
-    number specified by `n`. Correlations are ordered from strongest to lowest,
-    from the outside in.
-
-    Use this to communicate the correlations of one particular variable (ex: target
-    y) in relation to others with a very clean design. It's much easier to scan
-    this correlation chart vs. trying to find the variable of interest in a
-    heatmap. The fixed Y axis scales, and Red-Yellow-Green color palette, ensure
-    the actual magnitudes of the positive or negative correlations are clear and
-    not misinterpreted.
+def split_dataframe(
+        df: pd.DataFrame,
+        n: int
+) -> Tuple[pd.DataFrame, pd.DataFrame]:
+    """
+    Split a DataFrame into categorical and numerical columns.
+
+    This function splits the input DataFrame into two separate DataFrames based on
+    the number of unique values in each column. Columns with `n` or fewer unique
+    values are considered categorical and are placed in `df_cat`, while columns
+    with more than `n` unique values are considered numerical and are placed in
+    `df_num`.
+
+    Use this function when you need to separate categorical and numerical columns
+    in a DataFrame for further analysis or processing.
 
     Parameters
     ----------
     df : pd.DataFrame
-        The DataFrame containing the variables for correlation analysis.
-    column : str
-        The name of the column to evaluate correlations against.
+        The DataFrame to split.
     n : int
-        The number of correlations to display, split evenly between positive and
-        negative correlations.
-    method : str, optional
-        The method of correlation calculation, as per `df.corr()` method options
-        ('pearson', 'kendall', 'spearman'). Default is 'pearson'.
-    size : Tuple[int, int], optional
-        The size of the resulting plot. Default is (15, 8).
-    rotation : int, optional
-        The rotation angle for x-axis labels. Default is 45 degrees.
-    palette : str, optional
-        The colormap for representing correlation values. Default is 'RdYlGn'.
-    decimal : int, optional
-        The number of decimal places for rounding correlation values. Default is 2.
+        The maximum number of unique values for a column to be considered
+        categorical.
 
     Returns
     -------
-    None
-        Displays the barplot but does not return any value.
+    Tuple[pd.DataFrame, pd.DataFrame]
+        A tuple containing two DataFrames:
+        - df_cat: Contains the categorical columns of `df`.
+        - df_num: Contains the numerical columns of `df`.
 
     Examples
     --------
-    >>> df = pd.DataFrame({
-    ...     'A': np.random.rand(50),
-    ...     'B': np.random.rand(50),
-    ...     'C': np.random.rand(50)
-    ... })
-    >>> plot_corr(df, 'A', n=4)
+    Prepare the data for the examples:
 
-    This will display a barplot of the top 2 positive and top 2 negative
-    correlations of column 'A' with columns 'B' and 'C'.
-    """
-    # Calculate correlations
-    corr = round(df.corr(method=method, numeric_only=True)[column].sort_values(), decimal)
+    >>> data = {
+    ...     'A': [5.1, 2.0, 3.2, 1.4, 7.2],
+    ...     'B': ['Yes', 'No', 'No', 'Yes', 'No'],
+    ...     'C': [10, 20, 30, 40, 50],
+    ...     'D': ['High', 'Low', 'High', 'Low', 'Low']
+    ... }
+    >>> df = pd.DataFrame(data)
+
+    Example 1: Split the DataFrame based on 2 unique values:
 
-    # Drop column from correlations (correlating with itself)
-    corr = corr.drop(column)
-
-    # Get the most negative and most positive correlations, sorted by absolute value
-    most_negative = corr.sort_values().head(n // 2)
-    most_positive = corr.sort_values().tail(n // 2)
-
-    # Concatenate these two series and sort the final series by correlation value
-    corr = pd.concat([most_negative, most_positive]).sort_values()
-    corr.dropna(inplace=True)
-
-    # Generate colors based on correlation values using a colormap
-    cmap = plt.get_cmap(palette)
-    colors = cmap((corr.values + 1) / 2)
-
-    # Plot the chart
-    plt.figure(figsize=size)
-    plt.axhline(y=0, color='lightgrey', alpha=0.8, linestyle='-')
-    bars = plt.bar(corr.index, corr.values, color=colors)
-
-    # Add value labels to the end of each bar
-    for bar in bars:
-        yval = bar.get_height()
-        if yval < 0:
-            plt.text(bar.get_x() + bar.get_width() / 3.0, yval - 0.05, yval, va='top', fontsize=9)
+    >>> df_cat, df_num = split_dataframe(df, n=2)
+    >>> df_cat
+         B     D
+    0  Yes  High
+    1   No   Low
+    2   No  High
+    3  Yes   Low
+    4   No   Low
+    >>> df_num
+         A   C
+    0  5.1  10
+    1  2.0  20
+    2  3.2  30
+    3  1.4  40
+    4  7.2  50
+    """
+    # Initialize the 2 dataframes
+    df_cat = pd.DataFrame()
+    df_num = pd.DataFrame()
+
+    # Check unique values of each column
+    for col in df.columns:
+        # If Less than or equal to n, add it to the categorical df
+        if df[col].nunique() <= n:
+            df_cat[col] = df[col]
+        # Otherwise add it to the numerical df
         else:
-            plt.text(bar.get_x() + bar.get_width() / 3.0, yval + 0.05, yval, va='bottom', fontsize=9)
+            df_num[col] = df[col]
 
-    plt.title('Correlation with ' + column, fontsize=20)
-    plt.ylabel('Correlation', fontsize=14)
-    plt.xlabel('Other Variables', fontsize=14)
-    plt.xticks(rotation=rotation)
-    plt.ylim(-1, 1)
-    plt.show()
+    # Return the 2 dataframes
+    return df_cat, df_num
 
 
-def plot_map_ca(
-        df: pd.DataFrame,
-        lon: str = 'Longitude',
-        lat: str = 'Latitude',
-        hue: Optional[str] = None,
-        size: Optional[str] = None,
-        size_range: Tuple[int, int] = (50, 200),
-        title: str = 'Geographic Chart',
-        dot_size: Optional[int] = None,
-        alpha: float = 0.8,
-        color_map: Optional[str] = None,
-        fig_size: Tuple[int, int] = (12, 12)
-) -> None:
-    """
-    Plot longitude and latitude data on a geographic map of California.
-
-    This function creates a geographic map of California using Cartopy and
-    overlays data points from a DataFrame. The map includes major cities, county
-    boundaries, and geographic terrain features. Specify the columns in the
-    dataframe that map to the longitude (`lon`) and the latitude (`lat`). Then
-    specify an optional `hue` column to see changes in this variable by color,
-    and/or a `size` column to see changes in this varible by dot size. So two
-    variables can be visualized at once.
-
-    A few parameters can be customized, such as the range of the dot sizes
-    (`size_range`) if you're using `size`. You can also just use `dot_size` to
-    specify a fixed size for all the dots on the map. The `alpha` transparency
-    can be adjusted, to make sure you at least have a chance of seeing dots of
-    a different color that may be covered up by the top-most layer. You can also
-    customize the `color_map` for the `hue` parameter.
-
-    Use this function to visualize geospatial data related to
-    California on a clean map.
-
-    Note: This function requires a few libraries to be installed: Cartopy,
-    Geopandas, and Matplotlib (pyplot and patheffects). In addition, it uses
-    the 2018 Census Bureau's 5-meter county map files, which can be found here:
-    https://www2.census.gov/geo/tiger/GENZ2018/shp/cb_2018_us_county_5m.zip
+def dollars(
+        x: float,
+        pos: int = 0
+) -> str:
+    """
+    Format a number as currency with thousands separators on a matplotlib chart
+    axis.
+
+    This function takes a numeric value `x` and formats it as a string with
+    thousands separators and a dollar sign prefix. The `pos` parameter is required
+    by the matplotlib library for tick formatting but is not used in this function.
+
+    Use this function when you need to display currency values in a more readable
+    format, particularly in the context of matplotlib or seaborn plots.
 
     Parameters
     ----------
-    df : pd.DataFrame
-        DataFrame containing the data to be plotted.
-    lon : str, optional
-        Column name in `df` representing the longitude coordinates.
-        Default is 'Longitude'.
-    lat : str, optional
-        Column name in `df` representing the latitude coordinates.
-        Default is 'Latitude'.
-    hue : str, optional
-        Column name in `df` for color-coding the points. Default is
-        None.
-    size : str, optional
-        Column name in `df` to scale the size of points. Default is
-        None.
-    size_range : Tuple[int, int], optional
-        Range of sizes if the `size` parameter is used. Default is
-        (50, 200).
-    title : str, optional
-        Title of the plot. Default is 'Geographic Chart'.
-    dot_size : int, optional
-        Size of all dots if you want them to be uniform. Default is
-        None.
-    alpha : float, optional
-        Transparency of the points. Default is 0.8.
-    color_map : colors.Colormap, optional
-        Colormap to be used if `hue` is specified. Default is None.
-    fig_size : Tuple[int, int], optional
-        Size of the figure. Default is (12, 12).
+    x : float
+        The number to format.
+    pos : int, optional
+        The position of the number. This parameter is not used in the function
+        but is required by matplotlib for tick formatting. Default is 0.
 
     Returns
     -------
-    None
+    str
+        The formatted number as a string with thousands separators and dollar sign.
 
     Examples
     --------
+    Example 1: Format a large currency value with default parameters:
+
+    >>> x = 1234567.89
+    >>> formatted_num = dollars(x)
+    >>> print(formatted_num)
+    $1,234,567
+
+    Example 2: Use the function for tick formatting in a seaborn scatterplot:
+
     >>> import pandas as pd
+    >>> import seaborn as sns
+    >>> import matplotlib.pyplot as plt
+    >>> from matplotlib.ticker import FuncFormatter
+
+    >>> # Create a sample DataFrame for plotting
     >>> data = {
-    ...     'longitude': [-122.23, -122.22, -122.24, -122.25, -122.25],
-    ...     'latitude': [37.88, 37.86, 37.85, 37.85, 37.85],
-    ...     'housing_median_age': [41.0, 21.0, 52.0, 52.0, 52.0],
-    ...     'total_rooms': [880.0, 7099.0, 1467.0, 1274.0, 1627.0],
-    ...     'total_bedrooms': [129.0, 1106.0, 190.0, 235.0, 280.0],
-    ...     'population': [322.0, 2401.0, 496.0, 558.0, 565.0],
-    ...     'households': [126.0, 1138.0, 177.0, 219.0, 259.0],
-    ...     'median_income': [8.3252, 8.3014, 7.2574, 5.6431, 3.8462],
-    ...     'median_house_value': [452600.0, 358500.0, 352100.0, 341300.0, 342200.0],
-    ...     'ocean_proximity': ['NEAR BAY', 'NEAR BAY', 'NEAR BAY', 'NEAR BAY', 'NEAR BAY']
+    ...     'housing_median_age': [41.0, 21.0, 52.0, 52.0, 52.0, 52.0, 52.0],
+    ...     'total_rooms': [880.0, 7099.0, 1467.0, 1274.0, 1627.0, 919.0, 2535.0],
+    ...     'median_house_value': [452600.0, 358500.0, 352100.0, 341300.0,
+    ...     342200.0, 269700.0, 299200.0]
     ... }
     >>> df = pd.DataFrame(data)
-    >>> plot_map_ca(df, lon='longitude', lat='latitude',
-    ...             hue='ocean_proximity', size='median_house_value',
-    ...             size_range=(100, 500), alpha=0.6,
-    ...             title='California Housing Data')
-    """
-    # Define the locations of major cities
-    large_ca_cities = {'Name': ['Fresno', 'Los Angeles', 'Sacramento', 'San Diego', 'San Francisco', 'San Jose'],
-                       'Latitude': [36.746842, 34.052233, 38.581572, 32.715328, 37.774931, 37.339386],
-                       'Longitude': [-119.772586, -118.243686, -121.494400, -117.157256, -122.419417, -121.894956],
-                       'County': ['Fresno', 'Los Angeles', 'Sacramento', 'San Diego', 'San Francisco', 'Santa Clara']}
-    df_large_cities = pd.DataFrame(large_ca_cities)
-
-    # Create a figure that utilizes Cartopy
-    fig = plt.figure(figsize=fig_size)
-    ax = plt.axes(projection=ccrs.PlateCarree())
-    ax.set_extent([-125, -114, 32, 42])
-
-    # Add geographic details
-    ax.add_feature(cfeature.LAND, facecolor='white')
-    ax.add_feature(cfeature.OCEAN, facecolor='lightgrey', alpha=0.5)
-    ax.add_feature(cfeature.COASTLINE)
-    ax.add_feature(cfeature.STATES)
-
-    # Add county boundaries
-    # Determine the path to the data file within the package
-    with path('datawaza.data', 'cb_2018_us_county_5m.shp') as data_path:
-        counties = gpd.read_file(str(data_path))
-    counties_ca = counties[counties['STATEFP'] == '06']
-    counties_ca = counties_ca.to_crs("EPSG:4326")
-    for geometry in counties_ca['geometry']:
-        ax.add_geometries([geometry], crs=ccrs.PlateCarree(), edgecolor='grey', alpha=0.3, facecolor='none')
-
-    # Draw the scatterplot of data
-    if dot_size:
-        ax.scatter(df[lon], df[lat], s=dot_size, cmap=color_map, alpha=alpha, transform=ccrs.PlateCarree())
-    else:
-        sns.scatterplot(data=df, x=lon, y=lat, hue=hue, size=size, alpha=alpha, ax=ax, palette=color_map, sizes=size_range)
 
-    # Add cities
-    ax.scatter(df_large_cities['Longitude'], df_large_cities['Latitude'], transform=ccrs.PlateCarree(), edgecolor='black')
-    for x, y, label in zip(df_large_cities['Longitude'], df_large_cities['Latitude'], df_large_cities['Name']):
-        text = ax.text(x + 0.05, y + 0.05, label, transform=ccrs.PlateCarree(), fontsize=12, ha='left', fontname='Arial')
-        text.set_path_effects([pe.withStroke(linewidth=3, foreground='white')])
-
-    # Finish up the chart
-    ax.set_title(title, fontsize=18, pad=15)
-    ax.set_xlabel('Longitude', fontsize=14, labelpad=15)
-    ax.set_ylabel('Latitude', fontsize=14)
-    ax.gridlines(draw_labels=True, color='lightgrey', alpha=0.5)
-    plt.show()
+    >>> plt.figure(figsize=(10, 6))  # doctest: +SKIP
+    >>> plt.title('Total Rooms vs. Median House Value', fontsize=18, pad=15)  # doctest: +SKIP
+    >>> sns.scatterplot(data=df, x='total_rooms', y='median_house_value')  # doctest: +SKIP
+    >>> plt.xlabel('Total Rooms', fontsize=14, labelpad=10)  # doctest: +SKIP
+    >>> plt.ylabel('Median House Value', fontsize=14)  # doctest: +SKIP
+    >>> plt.gca().yaxis.set_major_formatter(FuncFormatter(dollars))
+    >>> plt.show()  # Displays the plot (visual output not shown)  # doctest: +SKIP
+    """
+    s = '${:0,d}'.format(int(x))
+    return s
+
+
+def thousands(
+        x: float,
+        pos: int = 0
+) -> str:
+    """
+    Format a number with thousands separators on a matplotlib chart axis.
+
+    This function takes a numeric value `x` and formats it as a string with
+    thousands separators. The `pos` parameter is required by the matplotlib
+    library for tick formatting but is not used in this function.
+
+    Use this function when you need to display large numbers in a more readable
+    format, particularly in the context of matplotlib or seaborn plots.
+
+    Parameters
+    ----------
+    x : float
+        The number to format.
+    pos : int, optional
+        The position of the number. This parameter is not used in the function
+        but is required by matplotlib for tick formatting. Default is 0.
+
+    Returns
+    -------
+    str
+        The formatted number as a string with thousands separators.
+
+    Examples
+    --------
+    Example 1: Format a large number with default parameters:
+
+    >>> x = 1234567.89
+    >>> formatted_num = thousands(x)
+    >>> print(formatted_num)
+    1,234,567
+
+    Example 2: Use the function for tick formatting in a seaborn histogram plot:
+
+    >>> import pandas as pd
+    >>> import seaborn as sns
+    >>> import matplotlib.pyplot as plt
+    >>> from matplotlib.ticker import FuncFormatter
+
+    >>> # Create a sample DataFrame for plotting
+    >>> data = {
+    ...     'housing_median_age': [41.0, 21.0, 52.0, 52.0, 52.0, 52.0, 52.0],
+    ...     'total_rooms': [880.0, 7099.0, 1467.0, 1274.0, 1627.0, 919.0, 2535.0],
+    ...     'median_house_value': [452600.0, 358500.0, 352100.0, 341300.0,
+    ...     342200.0, 269700.0, 299200.0]
+    ... }
+    >>> df = pd.DataFrame(data)
+
+    >>> plt.figure(figsize=(10, 6))  # doctest: +SKIP
+    >>> plt.title('Total Rooms vs. Median House Value', fontsize=18, pad=15)  # doctest: +SKIP
+    >>> sns.scatterplot(data=df, x='total_rooms', y='median_house_value')  # doctest: +SKIP
+    >>> plt.xlabel('Total Rooms', fontsize=14, labelpad=10)  # doctest: +SKIP
+    >>> plt.ylabel('Median House Value', fontsize=14)  # doctest: +SKIP
+    >>> plt.gca().xaxis.set_major_formatter(FuncFormatter(thousands))
+    >>> plt.show()  # Displays the plot (visual output not shown)  # doctest: +SKIP
+    """
+    s = '{:0,d}'.format(int(x))
+    return s
+
+
+# Classes
+class DebugPrinter:
+    """
+    Conditionally print debugging information during the execution of a script.
+
+    This class provides a simple way to print debugging information during the
+    execution of a script. By setting the `debug` attribute to True, you can
+    enable or disable debugging output throughout the script. The `print()`
+    method works like the built-in `print()` function but only prints output
+    when debugging is enabled.
+
+    Use this class when you need to easily control and print debugging messages
+    in your script, allowing you to enable or disable debugging output as
+    needed. It allows you to avoid nesting a bunch of print statements
+    underneath an "if debug:" statement, and it's lighter weight than a full
+    logging setup.
+
+    Parameters
+    ----------
+    debug : bool, optional
+        Whether to enable debugging output. Default is False.
+
+    Examples
+    --------
+    Set some test variables for the examples:
+
+    >>> name = 'Setting'
+    >>> value = 10
+
+    Example 1: Create a DebugPrinter object and print a debug message:
+
+    >>> db = DebugPrinter(debug=True)
+    >>> db.print('This is a debug message.')
+    This is a debug message.
+
+    Example 2: Disable debugging and print a message that doesn't display:
+
+    >>> db.set_debug(False)
+    >>> db.print("This is a debug message that won't show.")
+
+    Example 3: Re-enable debug, and print a formatted message with variables:
+
+    >>> db.set_debug(True)
+    >>> db.print(f'This is a debug message. ({name}: {value})')
+    This is a debug message. (Setting: 10)
+    """
+
+    def __init__(
+            self,
+            debug: bool = False
+    ):
+        """
+        Initialize the DebugPrinter object with the specified debugging setting.
+        """
+        self.debug = debug
+
+    def print(self, *args, **kwargs):
+        """
+        Print debugging information if debugging is enabled.
+
+        Parameters
+        ----------
+        *args
+            Any number of positional arguments to print.
+        **kwargs
+            Any keyword arguments to pass to the built-in `print()` function.
+        """
+        if self.debug:
+            print(*args, **kwargs)
+
+    def set_debug(self, debug: bool):
+        """
+        Set the debugging setting to enable or disable debugging output.
+
+        Parameters
+        ----------
+        debug : bool
+            Whether to enable or disable debugging output.
+        """
+        self.debug = debug
+
+
+class LogTransformer(BaseEstimator, TransformerMixin):
+    """
+    Apply logarithmic transformation to numerical features.
+
+    This transformer applies a logarithmic transformation to the input
+    features using `np.log1p()`, which calculates the natural logarithm
+    of 1 plus the input values. It is useful for transforming skewed
+    distributions to be more approximately normal.
+
+    The transformer inherits from BaseEstimator and TransformerMixin
+    to ensure compatibility with scikit-learn pipelines and model
+    selection tools.
+
+    Examples
+    --------
+    >>> from sklearn.datasets import load_iris
+    >>> X, _ = load_iris(return_X_y=True)
+    >>> transformer = LogTransformer()
+    >>> X_transformed = transformer.fit_transform(X)
+    >>> transformer.get_feature_names_out(['sepal_length', 'sepal_width',
+    ...                                     'petal_length', 'petal_width'])
+    ['sepal_length_log', 'sepal_width_log', 'petal_length_log', 'petal_width_log']
+    """
+    def __init__(self):
+        pass
+
+    def fit(self, X, y=None):
+        """
+        Fit the transformer to the input data.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            The input data.
+        y : None
+            Ignored. This parameter exists only for compatibility with
+            scikit-learn pipelines.
+
+        Returns
+        -------
+        self : LogTransformer
+            The fitted transformer.
+        """
+        return self
+
+    def transform(self, X):
+        """
+        Apply the logarithmic transformation to the input data.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            The input data.
+
+        Returns
+        -------
+        X_transformed : array-like of shape (n_samples, n_features)
+            The transformed data.
+        """
+        return np.log1p(X)
+
+    def get_feature_names_out(self, input_features=None):
+        """
+        Get the feature names after applying the transformation.
+
+        Parameters
+        ----------
+        input_features : list of str, default=None
+            The input feature names. If None, the feature names will be
+            generated as 'x0', 'x1', etc.
+
+        Returns
+        -------
+        feature_names_out : list of str
+            The feature names after applying the transformation, suffixed
+            with '_log'.
+        """
+        return [f"{col}_log" for col in input_features]
+
```

### Comparing `datawaza-0.1.2/datawaza.egg-info/SOURCES.txt` & `datawaza-0.1.3/datawaza.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -13,8 +13,11 @@
 datawaza.egg-info/top_level.txt
 datawaza/data/cb_2018_us_county_5m.cpg
 datawaza/data/cb_2018_us_county_5m.dbf
 datawaza/data/cb_2018_us_county_5m.prj
 datawaza/data/cb_2018_us_county_5m.shp
 datawaza/data/cb_2018_us_county_5m.shp.ea.iso.xml
 datawaza/data/cb_2018_us_county_5m.shp.iso.xml
-datawaza/data/cb_2018_us_county_5m.shx
+datawaza/data/cb_2018_us_county_5m.shx
+datawaza/data/mnist_28x28_ch1_x0.pt
+datawaza/data/svhn_32x32_ch3_x0.pt
+datawaza/data/svhn_32x32_ch3_xhat0.pt
```

### Comparing `datawaza-0.1.2/setup.py` & `datawaza-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,55 +2,60 @@
 
 # Read the contents of the README file
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name = 'datawaza',
-    version = '0.1.2',
-    python_requires = '>=3.10',
+    version = '0.1.3',
+    python_requires = '>=3.9, <3.13',
     packages = find_packages(),
     package_data = {
-        # Specify files within the datawaza package
-        'datawaza': ['data/*.xml', 'data/*.dbf', 'data/*.shp', 'data/*.shx', 'data/*.cpg', 'data/*.prj'],
+        # Map files and sample PyTorch image tensors
+        'datawaza': ['data/*.xml', 'data/*.dbf', 'data/*.shp', 'data/*.shx', 'data/*.cpg', 'data/*.prj', 'data/*.pt'],
     },
     include_package_data=True,
     install_requires=[
-        'pandas~=1.2.1',
-        'numpy~=1.26.2',
-        'matplotlib~=3.8.2',
-        'seaborn~=0.13.0',
-        'pytz~=2024.1',
-        'scikit-learn~=1.4.1.post1',
-        'category_encoders~=2.6.3',
-        'joblib~=1.3.2',
-        'setuptools~=69.1.1',
-        'typing~=3.7.4.3',
-        'scipy~=1.11.4',
-        'cartopy~=0.22.0',
-        'geopandas~=0.14.3',
-        'statsmodels~=0.14.1',
-        'plotly~=5.19.0'
+        'pandas>=2.2.1',
+        'numpy>=1.26.2',
+        'matplotlib>=3.8.2',
+        'seaborn>=0.13.2',
+        'pytz>=2023.3',
+        'scikit-learn>=1.5.0',
+        'joblib>=1.3.2',
+        'setuptools>=69.1.1',
+        'typing>=3.7.4.3',
+        'scipy>=1.11.4',
+        'cartopy>=0.22.0',
+        'geopandas>=0.14.3',
+        'statsmodels>=0.14.1',
+        'plotly>=5.19.0',
+        'nbformat>=4.2.0',
+        'importlib_resources>=6.3.2; python_version<"3.10"',
+        'scikeras>=0.13.0',
+        'xgboost>=2.0.3',
+        'imbalanced-learn>=0.12.3',
+        'tensorflow>=2.16.1',
+        'keras>=3.2.0',
+        'torch>=2.1.0',
     ],
     extras_require = {
-        'dev': [
-            'pydata_sphinx_theme==0.15.2',
-            'sphinx-design==0.5.0',
-            'Sphinx==7.2.6',
-            'sphinx-rtd-theme==2.0.0',
-            'sphinxcontrib-applehelp==1.0.8',
-            'sphinxcontrib-devhelp==1.0.6',
-            'sphinxcontrib-htmlhelp==2.0.5',
-            'sphinxcontrib-jquery==4.1',
-            'sphinxcontrib-jsmath==1.0.1',
-            'sphinxcontrib-qthelp==1.0.7',
-            'sphinxcontrib-serializinghtml==1.1.10',
-            'myst-parser==2.0.0',
-            'sphinx-favicon==1.0.1',
-            'nbsphinx==0.9.3'
+        'doc': [
+            'pydata_sphinx_theme~=0.15.2',
+            'sphinx-design~=0.5.0',
+            'Sphinx~=7.2.6',
+            'myst-parser~=2.0.0',
+            'sphinx-favicon~=1.0.1',
+            'nbsphinx~=0.9.3',
+        ],
+        'test': [
+            'pytest>=8.1.1',
+            'pytest-cov>=4.1.0',
+            'coverage>=6.5.0',
+            'coveralls>=3.3.1',
         ]
     },
     author='Jim Beno',
     author_email='jim@jimbeno.net',
     description="Datawaza is a collection of tools for data exploration, visualization, data cleaning, pipeline creation, model iteration, and evaluation.",
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -60,15 +65,18 @@
         'Source': 'https://github.com/jbeno/datawaza'
     },
     keywords=['data science', 'visualization', 'machine learning', 'data analysis'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Operating System :: OS Independent',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Natural Language :: English',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Scientific/Engineering :: Visualization',
         'Topic :: Scientific/Engineering :: Information Analysis'
     ]
```

