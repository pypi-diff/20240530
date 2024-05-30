# Comparing `tmp/virgo_modules-0.0.88.tar.gz` & `tmp/virgo_modules-0.0.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.88.tar", last modified: Thu May 23 16:45:38 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.89.tar", last modified: Wed May 29 16:18:05 2024, max compression
```

## Comparing `virgo_modules-0.0.88.tar` & `virgo_modules-0.0.89.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 16:45:38.887897 virgo_modules-0.0.88/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.88/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-05-23 16:45:38.882897 virgo_modules-0.0.88/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.88/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 16:45:38.887897 virgo_modules-0.0.88/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-05-23 16:27:32.000000 virgo_modules-0.0.88/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:45:38.800904 virgo_modules-0.0.88/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-05-23 16:45:38.824897 virgo_modules-0.0.88/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.88/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:45:38.878899 virgo_modules-0.0.88/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.88/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.88/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0    13732 2024-05-16 12:03:48.000000 virgo_modules-0.0.88/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.88/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    72244 2024-05-23 16:28:19.000000 virgo_modules-0.0.88/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   146629 2024-05-23 16:27:32.000000 virgo_modules-0.0.88/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:45:38.849900 virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-05-23 16:45:38.000000 virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-05-23 16:45:38.000000 virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:45:38.000000 virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-05-23 16:45:38.000000 virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 16:45:38.000000 virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 16:18:05.185614 virgo_modules-0.0.89/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.89/LICENSE
+-rw-rw-rw-   0        0        0     1411 2024-05-29 16:18:05.170614 virgo_modules-0.0.89/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.89/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 16:18:05.185614 virgo_modules-0.0.89/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-05-29 16:16:25.000000 virgo_modules-0.0.89/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:18:04.999576 virgo_modules-0.0.89/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-05-29 16:18:05.068272 virgo_modules-0.0.89/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.89/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:18:05.147092 virgo_modules-0.0.89/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.89/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.89/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0    13732 2024-05-16 12:03:48.000000 virgo_modules-0.0.89/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.89/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    72244 2024-05-23 16:28:19.000000 virgo_modules-0.0.89/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   150133 2024-05-29 16:16:25.000000 virgo_modules-0.0.89/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:18:05.088964 virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0     1411 2024-05-29 16:18:03.000000 virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-05-29 16:18:03.000000 virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 16:18:03.000000 virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-05-29 16:18:03.000000 virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-29 16:18:03.000000 virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.88/LICENSE` & `virgo_modules-0.0.89/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.88/PKG-INFO` & `virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: virgo_modules
-Version: 0.0.88
+Name: virgo-modules
+Version: 0.0.89
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.88/setup.py` & `virgo_modules-0.0.89/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.88",
+    version="0.0.89",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.88/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.89/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.88/virgo_app/virgo_modules/src/edge_utils.py` & `virgo_modules-0.0.89/virgo_app/virgo_modules/src/edge_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.88/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.89/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.88/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.89/virgo_app/virgo_modules/src/re_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.88/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.89/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,117 @@
 
     def fit(self, X, y=None):
         return self
 
     def transform(self, X, y=None):
         return X[self.columns]
 
+class features_entropy(BaseEstimator, TransformerMixin):
+    """
+    Class that creates a feature that calculate entropy for a given feature classes, but it might get some leackeage in the training set.
+    this class is compatible with scikitlearn pipeline
+
+    Attributes
+    ----------
+    columns : list
+        list of features to select
+    entropy_map: pd.DataFrame
+        dataframe of the map with the entropies per class
+    perc: float
+        percentage of the dates using for calculate the entropy map
+    
+    Methods
+    -------
+    fit(additional="", X=DataFrame, y=None):
+        fit transformation.
+    transform(X=DataFrame, y=None):
+        apply feature transformation
+    """
+    
+    def __init__(self, features, target, feature_name = None, feature_type = 'discrete', perc = 0.5, default_null = 0.99):
+        
+        self.features = features
+        self.feature_type = feature_type
+        self.target = target
+        self.perc = perc
+        self.default_null = default_null
+        
+        if not feature_name:
+            self.feature_name = '_'.join(features)
+            self.feature_name = self.feature_name + '_' + target + '_' + feature_type
+        else:
+            self.feature_name = feature_name
+            
+    def fit(self, X, y=None):
+
+        unique_dates = list(X['Date'].unique())
+        unique_dates.sort()
+        
+        total_length = len(unique_dates)
+        cut = int(round(total_length*self.perc,0))
+        train_dates = unique_dates[:cut]
+        max_train_date = max(train_dates)
+        
+        X_ = X[X['Date'] <= max_train_date]
+        df = pd.merge(X_, y, left_index=True, right_index=True, how = 'left').copy()
+
+        column_list = [f'{self.feature_type}_signal_{colx}' for colx in self.features]
+        
+        df_aggr = (
+            df
+            .groupby(column_list, as_index = False)
+            .apply(
+                lambda x: pd.Series(
+                    dict(
+                        counts = x[self.target].count(),
+                        trues=(x[self.target] == 1).sum(),
+                        falses=(x[self.target] == 0).sum(),
+                    )
+                )
+            )
+            .assign(
+                trues_rate=lambda x: x['trues'] / x['counts']
+            )
+            .assign(
+                falses_rate=lambda x: x['falses'] / x['counts']
+            )
+            .assign(
+                log2_trues = lambda x: np.log2(1/x['trues_rate'])
+            )
+            .assign(
+                log2_falses = lambda x: np.log2(1/x['falses_rate'])
+            )
+            .assign(
+                comp1 = lambda x: x['trues_rate']*x['log2_trues']
+            )
+            .assign(
+                comp2 = lambda x: x['falses_rate']*x['log2_falses']
+            )
+            .assign(
+                class_entropy = lambda x: np.round(x['comp1']+x['comp2'],3)
+            )
+        )
+        
+        self.column_list = column_list
+        self.entropy_map = (
+            df_aggr
+            [column_list+['class_entropy']]
+            .rename(columns = {'class_entropy': self.feature_name})
+            .copy()
+        )
+        
+        del df, df_aggr
+        return self
+
+    def transform(self, X, y=None):
+
+        X = X.merge(self.entropy_map, on=self.column_list, how = 'left')
+        X[self.feature_name] = X[self.feature_name].fillna(self.default_null)
+        return X
+
 def sharpe_ratio(return_series):
 
     '''
     calculate sharpe ratio for given array.
 
             Parameters:
                     return_series (pd.series): pandas series of the asset returns
```

### Comparing `virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/PKG-INFO` & `virgo_modules-0.0.89/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: virgo-modules
-Version: 0.0.88
+Name: virgo_modules
+Version: 0.0.89
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.89/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

