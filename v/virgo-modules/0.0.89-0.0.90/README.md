# Comparing `tmp/virgo_modules-0.0.89.tar.gz` & `tmp/virgo_modules-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.89.tar", last modified: Wed May 29 16:18:05 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.90.tar", last modified: Thu May 30 14:59:17 2024, max compression
```

## Comparing `virgo_modules-0.0.89.tar` & `virgo_modules-0.0.90.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 16:18:05.185614 virgo_modules-0.0.89/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.89/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-05-29 16:18:05.170614 virgo_modules-0.0.89/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.89/README.md
--rw-rw-rw-   0        0        0       42 2024-05-29 16:18:05.185614 virgo_modules-0.0.89/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-05-29 16:16:25.000000 virgo_modules-0.0.89/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:18:04.999576 virgo_modules-0.0.89/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-05-29 16:18:05.068272 virgo_modules-0.0.89/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.89/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:18:05.147092 virgo_modules-0.0.89/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.89/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.89/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0    13732 2024-05-16 12:03:48.000000 virgo_modules-0.0.89/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.89/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    72244 2024-05-23 16:28:19.000000 virgo_modules-0.0.89/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   150133 2024-05-29 16:16:25.000000 virgo_modules-0.0.89/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:18:05.088964 virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-05-29 16:18:03.000000 virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-05-29 16:18:03.000000 virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 16:18:03.000000 virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-05-29 16:18:03.000000 virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-29 16:18:03.000000 virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 14:59:17.416336 virgo_modules-0.0.90/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.90/LICENSE
+-rw-rw-rw-   0        0        0     1411 2024-05-30 14:59:17.409335 virgo_modules-0.0.90/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.90/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-30 14:59:17.416336 virgo_modules-0.0.90/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-05-30 13:02:28.000000 virgo_modules-0.0.90/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:59:17.167623 virgo_modules-0.0.90/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-05-30 14:59:17.295839 virgo_modules-0.0.90/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.90/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:59:17.405050 virgo_modules-0.0.90/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.90/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.90/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0    14287 2024-05-30 13:29:15.000000 virgo_modules-0.0.90/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.90/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    72244 2024-05-23 16:28:19.000000 virgo_modules-0.0.90/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   150116 2024-05-30 14:56:36.000000 virgo_modules-0.0.90/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:59:17.377046 virgo_modules-0.0.90/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0     1411 2024-05-30 14:59:16.000000 virgo_modules-0.0.90/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-05-30 14:59:16.000000 virgo_modules-0.0.90/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 14:59:16.000000 virgo_modules-0.0.90/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-05-30 14:59:16.000000 virgo_modules-0.0.90/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-30 14:59:16.000000 virgo_modules-0.0.90/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.89/LICENSE` & `virgo_modules-0.0.90/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.89/PKG-INFO` & `virgo_modules-0.0.90/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo_modules
-Version: 0.0.89
+Version: 0.0.90
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.89/setup.py` & `virgo_modules-0.0.90/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.89",
+    version="0.0.90",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.89/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.90/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.89/virgo_app/virgo_modules/src/edge_utils.py` & `virgo_modules-0.0.90/virgo_app/virgo_modules/src/edge_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from feature_engine.selection import DropFeatures, DropCorrelatedFeatures
 from feature_engine.imputation import  MeanMedianImputer
 from virgo_modules.src.ticketer_source import FeatureSelector
 from feature_engine.discretisation import EqualWidthDiscretiser
 from feature_engine.datetime import DatetimeFeatures
 
-from .ticketer_source import VirgoWinsorizerFeature, InverseHyperbolicSine
+from .ticketer_source import VirgoWinsorizerFeature, InverseHyperbolicSine, FeaturesEntropy
 
 class produce_model_wrapper:
     """
     class that wraps a pipeline and a machine learning model. it also provides data spliting train/validation
 
     Attributes
     ----------
@@ -86,16 +86,16 @@
         Returns
         -------
         None
         """
         self.model = model
         self.pipe_transform = pipe
         self.pipeline = Pipeline([('pipe_transform',self.pipe_transform), ('model',self.model)])
-        self.features_to_model = self.pipe_transform.fit_transform(self.X_train).columns
         self.pipeline.fit(self.X_train, self.y_train)
+        self.features_to_model = self.pipeline[:-1].transform(self.X_train).columns
 
 class register_results():
     """
     class that collects model metrics
 
     Attributes
     ----------
@@ -213,14 +213,15 @@
 
 
 def data_processing_pipeline_classifier(
         features_base,features_to_drop = False, winsorizer_conf = False, discretize_columns = False,
         bins_discretize = 10, correlation = 0.85, fillna = True,
         invhypervolsin_features = False,
         date_features_list = False,
+        entropy_set_list = False,
         pipeline_order = 'selector//winzorizer//discretizer//median_inputer//drop//correlation'
         ):
 
     '''
     pipeline builder
 
             Parameters:
@@ -229,36 +230,46 @@
                     winsorizer_conf (dict): winsorising configuration dictionary
                     discretize_columns (list): feature list to discretize
                     bins_discretize (int): number of bins to discretize
                     correlation (float): correlation threshold to discard correlated features
                     fillna (boolean): if true to fill na features
                     invhypervolsin_features (list): list of features to apply inverse hyperbolic sine
                     date_features_list (list): list of features to compute from Date field. (list of features from feature_engine)
+                    entropy_set_list (list): list of dictionaries that contains features and targets to compute entropy
                     pipeline_order (str): custom pipeline order eg. selector//winzorizer//discretizer//median_inputer//drop//correlation
             Returns:
                     pipe (obj): pipeline object
     '''
     select_pipe = [('selector', FeatureSelector(features_base))] if features_base else []
     winzorizer_pipe = [('winzorized_features', VirgoWinsorizerFeature(winsorizer_conf))] if winsorizer_conf else []
     drop_pipe = [('drop_features' , DropFeatures(features_to_drop=features_to_drop))] if features_to_drop else []
     discretize = [('discretize',EqualWidthDiscretiser(discretize_columns, bins = bins_discretize ))] if discretize_columns else []
     drop_corr = [('drop_corr', DropCorrelatedFeatures(threshold=correlation, method = 'spearman'))] if correlation else []
     median_imputer_pipe = [('median_imputer', MeanMedianImputer())] if fillna else []
     invhypersin_pipe = [('invhypervolsin scaler', InverseHyperbolicSine(features = invhypervolsin_features))] if invhypervolsin_features else []
     datetimeFeatures_pipe = [('date features', DatetimeFeatures(features_to_extract = date_features_list, variables = 'Date', drop_original = False))] if date_features_list else []
-
+    
+    entropy_pipe = list()
+    if entropy_set_list:
+        for setx_ in entropy_set_list:
+            setx = setx_['set'].split('//')
+            target_ = setx_['target']
+            subpipe_name = '_'.join(setx) + 'entropy'
+            entropy_pipe.append((subpipe_name, FeaturesEntropy(features = setx, target = target_)))
+    
     pipe_dictionary = {
         'selector': select_pipe,
         'winzorizer':winzorizer_pipe,
         'drop':drop_pipe,
         'discretizer': discretize,
         'correlation': drop_corr,
         'median_inputer':median_imputer_pipe,
         'arcsinh_scaler': invhypersin_pipe,
         'date_features': datetimeFeatures_pipe,
+        'entropy_features' : entropy_pipe,
     }
 
     pipeline_steps = pipeline_order.split('//')
     ## validation
     for step in pipeline_steps:
         if step not in pipe_dictionary.keys():
             raise Exception(f'{step} step not in list of steps, the list is: {list(pipe_dictionary.keys())}')
```

### Comparing `virgo_modules-0.0.89/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.90/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.89/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.90/virgo_app/virgo_modules/src/re_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.89/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.90/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
     def fit(self, X, y=None):
         return self
 
     def transform(self, X, y=None):
         return X[self.columns]
 
-class features_entropy(BaseEstimator, TransformerMixin):
+class FeaturesEntropy(BaseEstimator, TransformerMixin):
     """
     Class that creates a feature that calculate entropy for a given feature classes, but it might get some leackeage in the training set.
     this class is compatible with scikitlearn pipeline
 
     Attributes
     ----------
     columns : list
@@ -189,16 +189,16 @@
         unique_dates.sort()
         
         total_length = len(unique_dates)
         cut = int(round(total_length*self.perc,0))
         train_dates = unique_dates[:cut]
         max_train_date = max(train_dates)
         
-        X_ = X[X['Date'] <= max_train_date]
-        df = pd.merge(X_, y, left_index=True, right_index=True, how = 'left').copy()
+        X_ = X[X['Date'] <= max_train_date].copy()
+        df = X_.join(y, how = 'left')
 
         column_list = [f'{self.feature_type}_signal_{colx}' for colx in self.features]
         
         df_aggr = (
             df
             .groupby(column_list, as_index = False)
             .apply(
@@ -237,20 +237,20 @@
         self.entropy_map = (
             df_aggr
             [column_list+['class_entropy']]
             .rename(columns = {'class_entropy': self.feature_name})
             .copy()
         )
         
-        del df, df_aggr
+        del df, df_aggr, X_
         return self
 
     def transform(self, X, y=None):
 
-        X = X.merge(self.entropy_map, on=self.column_list, how = 'left')
+        X = X.join(self.entropy_map.set_index(self.column_list), on=self.column_list, how = 'left')
         X[self.feature_name] = X[self.feature_name].fillna(self.default_null)
         return X
 
 def sharpe_ratio(return_series):
 
     '''
     calculate sharpe ratio for given array.
@@ -2594,17 +2594,16 @@
         Returns
         -------
         sample (float): sample size
         """
         self.model = model
         self.pipe_transform = pipe
         self.pipeline = Pipeline([('pipe_transform',self.pipe_transform), ('model',self.model)])
-        self.features_to_model = self.pipe_transform.fit_transform(self.X_train).columns
         self.pipeline.fit(self.X_train, self.y_train)
-
+        self.features_to_model = self.pipeline[:-1].transform(self.X_train).columns
 
 class hmm_feature_selector():
     """
     class that is going to train hmm models to perform feature selection
 
     Attributes
     ----------
```

### Comparing `virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/PKG-INFO` & `virgo_modules-0.0.90/virgo_app/virgo_modules.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo-modules
-Version: 0.0.89
+Version: 0.0.90
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.90/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

