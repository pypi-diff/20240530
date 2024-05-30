# Comparing `tmp/didtool-0.1.2-py3-none-any.whl.zip` & `tmp/didtool-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,29 +1,30 @@
-Zip file size: 43734 bytes, number of entries: 27
+Zip file size: 44262 bytes, number of entries: 28
+-rw-r--r--  2.0 unx     6148 b- defN 23-May-05 02:21 .DS_Store
 -rw-r--r--  2.0 unx      747 b- defN 21-Mar-10 08:09 didtool/__init__.py
--rw-r--r--  2.0 unx    14678 b- defN 21-Dec-09 10:41 didtool/cut.py
+-rw-r--r--  2.0 unx    14681 b- defN 24-May-30 08:37 didtool/cut.py
 -rw-r--r--  2.0 unx     2586 b- defN 21-Mar-10 07:36 didtool/encoder.py
 -rw-r--r--  2.0 unx      737 b- defN 20-Jun-24 02:23 didtool/logger.py
 -rw-r--r--  2.0 unx    23162 b- defN 21-Dec-09 10:41 didtool/metric.py
--rw-r--r--  2.0 unx    25734 b- defN 21-Dec-09 10:41 didtool/model.py
+-rw-r--r--  2.0 unx    25975 b- defN 24-May-30 08:37 didtool/model.py
 -rw-r--r--  2.0 unx    10015 b- defN 21-Dec-09 10:41 didtool/scorecard.py
--rw-r--r--  2.0 unx    16133 b- defN 21-Apr-08 12:03 didtool/selector.py
+-rw-r--r--  2.0 unx    16274 b- defN 24-May-30 08:37 didtool/selector.py
 -rw-r--r--  2.0 unx     4199 b- defN 21-Dec-23 03:21 didtool/split.py
--rw-r--r--  2.0 unx     3543 b- defN 21-Dec-09 02:41 didtool/stats.py
+-rw-r--r--  2.0 unx     3543 b- defN 24-May-22 14:48 didtool/stats.py
 -rw-r--r--  2.0 unx    19779 b- defN 21-Dec-09 02:42 didtool/transformer.py
 -rw-r--r--  2.0 unx     1833 b- defN 21-Dec-09 10:41 didtool/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Dec-09 02:49 tests/__init__.py
 -rw-r--r--  2.0 unx     3114 b- defN 21-Dec-09 06:48 tests/cut_test.py
 -rw-r--r--  2.0 unx     1839 b- defN 21-Dec-09 10:41 tests/encoder_test.py
 -rw-r--r--  2.0 unx     1669 b- defN 21-Dec-09 02:57 tests/metric_test.py
 -rw-r--r--  2.0 unx     7854 b- defN 21-Dec-09 03:25 tests/model_test.py
 -rw-r--r--  2.0 unx     1196 b- defN 21-Dec-09 03:38 tests/scorecard_test.py
 -rw-r--r--  2.0 unx     5528 b- defN 21-Dec-09 03:09 tests/selector_test.py
 -rw-r--r--  2.0 unx     1360 b- defN 21-Dec-09 03:09 tests/split_test.py
 -rw-r--r--  2.0 unx     2762 b- defN 21-Dec-09 03:09 tests/stats_test.py
 -rw-r--r--  2.0 unx    15002 b- defN 21-Dec-09 10:41 tests/transformer_test.py
--rw-r--r--  2.0 unx     1066 b- defN 21-Dec-23 04:18 didtool-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1014 b- defN 21-Dec-23 04:18 didtool-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Dec-23 04:18 didtool-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 21-Dec-23 04:18 didtool-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2054 b- defN 21-Dec-23 04:18 didtool-0.1.2.dist-info/RECORD
-27 files, 167710 bytes uncompressed, 40518 bytes compressed:  75.8%
+-rw-r--r--  2.0 unx     1066 b- defN 24-May-30 08:38 didtool-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      998 b- defN 24-May-30 08:38 didtool-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 08:38 didtool-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-May-30 08:38 didtool-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2119 b- defN 24-May-30 08:38 didtool-0.1.3.dist-info/RECORD
+28 files, 174292 bytes uncompressed, 40952 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -1,7 +1,10 @@
+Filename: .DS_Store
+Comment: 
+
 Filename: didtool/__init__.py
 Comment: 
 
 Filename: didtool/cut.py
 Comment: 
 
 Filename: didtool/encoder.py
@@ -60,23 +63,23 @@
 
 Filename: tests/stats_test.py
 Comment: 
 
 Filename: tests/transformer_test.py
 Comment: 
 
-Filename: didtool-0.1.2.dist-info/LICENSE
+Filename: didtool-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: didtool-0.1.2.dist-info/METADATA
+Filename: didtool-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: didtool-0.1.2.dist-info/WHEEL
+Filename: didtool-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: didtool-0.1.2.dist-info/top_level.txt
+Filename: didtool-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: didtool-0.1.2.dist-info/RECORD
+Filename: didtool-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## didtool/cut.py

```diff
@@ -133,15 +133,15 @@
          of `x`.
 
     bins : numpy.ndarray
         The computed or specified bins. Only returned when `return_bins=True`.
     """
     x = to_ndarray(x)
     target = to_ndarray(target)
-    mask = np.isnan(x)
+    mask = pd.isnull(x)
 
     tree = DecisionTreeClassifier(
         min_samples_leaf=min_bin,
         max_leaf_nodes=n_bins,
     )
     # only use non-nan values to fit decision tree
     tree.fit(x[~mask].reshape((-1, 1)), target[~mask])
@@ -190,15 +190,15 @@
          of `x`.
 
     bins : numpy.ndarray
         The computed or specified bins. Only returned when `return_bins=True`.
     """
     x = to_ndarray(x)
     target = to_ndarray(target)
-    mask = np.isnan(x)
+    mask = pd.isnull(x)
     min_child_samples = math.ceil(min_bin * len(x))
 
     tree = lightgbm.LGBMClassifier(
         n_estimators=1,
         num_leaves=n_bins,
         min_child_samples=min_child_samples,
         random_state=27
@@ -268,15 +268,15 @@
     return:
         out:分箱后结果
         bins:分箱界限
     """
     # 去除nan，单独分箱
     x = to_ndarray(x)
     target = to_ndarray(target)
-    mask = np.isnan(x)
+    mask = pd.isnull(x)
     df = pd.DataFrame({'feature': x[~mask], 'label': target[~mask]})
 
     # 对变量按属性值从小到大排序
     df.sort_values(by='feature', ascending=True, inplace=True)
     # 计算每一个属性值对应的卡方统计量等信息
     df['count_1'] = df['label']
     df['count_0'] = 1 - df['label']
```

## didtool/model.py

```diff
@@ -176,21 +176,24 @@
             train_data[self.feature_names])
         trans_val_data = self.pipeline[0].transform(
             val_data[self.feature_names])
         eval_set = [
             (trans_train_data, train_data[self.target]),
             (trans_val_data, val_data[self.target])
         ]
+
+        # 使用 early_stopping 回调函数
+        early_stopping_callback = lgb.early_stopping(stopping_rounds=early_stopping_rounds, verbose=verbose)
+
         self.pipeline[-1].fit(
             trans_train_data,
             train_data[self.target],
-            early_stopping_rounds=early_stopping_rounds,
             eval_set=eval_set,
             eval_metric=eval_metric,
-            verbose=verbose
+            callbacks=[early_stopping_callback]
         )
 
         imp_score = self.model.feature_importances_
         self.importance_df = pd.DataFrame({
             'feature': self.feature_names,
             'importance': imp_score}
         ).sort_values(by='importance', ascending=False)
@@ -541,21 +544,23 @@
                 train_k[self.feature_names])
             trans_val_k = self.pipelines[k][0].transform(
                 val_k[self.feature_names])
             eval_set = [
                 (trans_train_k, train_k[self.target]),
                 (trans_val_k, val_k[self.target])
             ]
+
+            # 使用 early_stopping 回调函数
+            early_stopping_callback = lgb.early_stopping(stopping_rounds=early_stopping_rounds, verbose=verbose)
             self.pipelines[k][-1].fit(
                 trans_train_k,
                 train_k[self.target],
-                early_stopping_rounds=early_stopping_rounds,
                 eval_set=eval_set,
                 eval_metric=eval_metric,
-                verbose=verbose
+                callbacks=[early_stopping_callback]
             )
 
             # append feature importance of model k
             imp_score = self.models[k].feature_importances_
             df_imp = pd.DataFrame({
                 'feature': self.feature_names,
                 'importance': imp_score}
```

## didtool/selector.py

```diff
@@ -236,18 +236,21 @@
                                        random_state=i)
 
             train_features, valid_features, train_labels, valid_labels = \
                 train_test_split(self.data, self.label,
                                  test_size=0.2, stratify=self.label,
                                  random_state=i)
 
+            # 使用 early_stopping 回调函数
+            early_stopping_callback = lgb.early_stopping(stopping_rounds=20, verbose=False)
+
             # Train the model with early stopping
             model.fit(train_features, train_labels, eval_metric='logloss',
                       eval_set=[(valid_features, valid_labels)],
-                      early_stopping_rounds=20, verbose=-1)
+                      callbacks=[early_stopping_callback])
 
             # Clean up memory
             gc.enable()
             del train_features, train_labels, valid_features, valid_labels
             gc.collect()
 
             # Record the feature importances
```

## Comparing `didtool-0.1.2.dist-info/LICENSE` & `didtool-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `didtool-0.1.2.dist-info/METADATA` & `didtool-0.1.3.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: didtool
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tool set for feature engineering & modeling
 Home-page: https://github.com/dustless/didtool
 Author: dustless
 Author-email: wuchenghui927@126.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: seaborn (>=0.10.1)
 Requires-Dist: scikit-learn (>=0.24.1)
-Requires-Dist: lightgbm (>=3.1.0)
+Requires-Dist: lightgbm (>=4.3.0)
 Requires-Dist: sklearn2pmml (>=0.65.0)
 Requires-Dist: bayesian-optimization (==1.2.0)
-Requires-Dist: pandas
-Requires-Dist: numpy
+Requires-Dist: pandas (>=1.5.3)
+Requires-Dist: numpy (>=1.20.3)
 
 # didtool
 [![pipeline status](http://icode.wejoydata.com/did/common/didtool/badges/master/pipeline.svg)](http://icode.wejoydata.com/did/common/didtool/-/commits/master)
 
 ## Install
 ```
 pip install didtool
 ```
 or 
 ```
 python setup.py bdist_wheel
 cd dist/
 pip install didtool-{version}-py3-none-any.whl
 ```
-
-
```

## Comparing `didtool-0.1.2.dist-info/RECORD` & `didtool-0.1.3.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
+.DS_Store,sha256=DAcAGpeeXf6O4S9jL7W9K0hZnsTZpOqvYHlc00ayTwk,6148
 didtool/__init__.py,sha256=-ER5R6Lr-CQ2OdFmmwzQCklx0kOvKZYkMFyEy_E7oN4,747
-didtool/cut.py,sha256=ojt23qSpbVwvGM21mxa1HAjrJZ-PC42qOogDk-TfaaU,14678
+didtool/cut.py,sha256=CNv-B0c6XTQYuIRvhCJ_3wjtumVQBWylLzDWIHlXBi0,14681
 didtool/encoder.py,sha256=deb5YLKyr6v50TLVHUtpz0JOCshm6fdiN9CNmlELLW0,2586
 didtool/logger.py,sha256=qImCDgYW8cs2E88HCa2DVk7BiXsRt3liNXXTo0dVfkw,737
 didtool/metric.py,sha256=no3eoL0qjyarSAAnGLcTfQg8Q_EaVeNaPRQepjlgOro,23162
-didtool/model.py,sha256=2l5GHQcrJ6rj16nqojuyEyo0uEXOqLfkPK_FRre3_5Y,25734
+didtool/model.py,sha256=8Y6sVpcgTbVvvdjNHuC5DaJh7WWMQTDfudekl0OIBE4,25975
 didtool/scorecard.py,sha256=ir0Fpu1wBijw6MDAnKHvM9yAXpBs7cTx5-Lr4lWgLc8,10015
-didtool/selector.py,sha256=73G2PPS6Z0ANJturWjx5hpsSakfwqb8cqnyqnrAjWjQ,16133
+didtool/selector.py,sha256=fXCBsyAPXCIQ27_wcIS4OF1NwOeSQ9lNOCcgOVqaKWU,16274
 didtool/split.py,sha256=M0S8w_ChbLKlwdHeJYQn3RCqN8dGFmQLKA2olbs2xdQ,4199
 didtool/stats.py,sha256=Nx6NNGzxG9ZRzsAENyxcGd0IKkfNwt-7eGRYAx47xUM,3543
 didtool/transformer.py,sha256=CquBEXi8oN4cy-G78Z6vnUEcU6YnAayrXg2orISQfwg,19779
 didtool/utils.py,sha256=-TU-p327iGnSgw4LNdeMdyzYt3nOUNtN2SC-CUXGw3E,1833
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/cut_test.py,sha256=EEbyv4ZzbZZlA80QAtdg98HNRRgryaQk_xRJRojNUYw,3114
 tests/encoder_test.py,sha256=IvnELDk9YOQDTGD_bgtalOmalxy3YS5KaxvaWv2TCpE,1839
 tests/metric_test.py,sha256=JzGI_Ur5iUmMK7QG5RVAfSfNuyzhXSeIoasu3RlLBqM,1669
 tests/model_test.py,sha256=t-MLs60D8ngf4VvEq1R9jr7sXAKMk4Zc4H07dUWzgVA,7854
 tests/scorecard_test.py,sha256=NYWBwik7en-sKUj-w-tqUl4YzR_PbVGcw9ntnvW0MR4,1196
 tests/selector_test.py,sha256=95ESE1uDR9RQh5FlrftEvAniSxjEvFkmRj2gZsRzkOE,5528
 tests/split_test.py,sha256=6k-7CblTqghFx5yl-a3w1UxhQtukhIC2MyBtopNHPZg,1360
 tests/stats_test.py,sha256=YazQU4eWNE20AevkTcQAtHEAUVmyoVui4mB9iNy1h0Y,2762
 tests/transformer_test.py,sha256=-SbaZ15qP1sBCm4rj6JB1Pi_RVV4fg2UqIMNdLqVHnA,15002
-didtool-0.1.2.dist-info/LICENSE,sha256=ezEI3E-qHJQB4adzrnhwcUbRZ3FFEpwqC7GuGugGYaQ,1066
-didtool-0.1.2.dist-info/METADATA,sha256=DVB7E4GAxM9eJuq3o9AlkDbTBNl8aPN_xqVSADrVeGU,1014
-didtool-0.1.2.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
-didtool-0.1.2.dist-info/top_level.txt,sha256=sIlVblI47yPn7YnXOzSHEmUccSLmKy0QRD88tKZSpcM,14
-didtool-0.1.2.dist-info/RECORD,,
+didtool-0.1.3.dist-info/LICENSE,sha256=ezEI3E-qHJQB4adzrnhwcUbRZ3FFEpwqC7GuGugGYaQ,1066
+didtool-0.1.3.dist-info/METADATA,sha256=65-IvGlQfjdPwMyz_W3jNgtspXy7MjlybdLDRPKcCXY,998
+didtool-0.1.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+didtool-0.1.3.dist-info/top_level.txt,sha256=sIlVblI47yPn7YnXOzSHEmUccSLmKy0QRD88tKZSpcM,14
+didtool-0.1.3.dist-info/RECORD,,
```

