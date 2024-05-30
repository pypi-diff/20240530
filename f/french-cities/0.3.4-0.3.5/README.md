# Comparing `tmp/french_cities-0.3.4.tar.gz` & `tmp/french_cities-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "french_cities-0.3.4.tar", max compression
+gzip compressed data, was "french_cities-0.3.5.tar", max compression
```

## Comparing `french_cities-0.3.4.tar` & `french_cities-0.3.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10260 2024-05-29 20:17:27.103324 french_cities-0.3.4/README.fr.md
--rw-r--r--   0        0        0     8729 2024-05-29 20:17:27.103324 french_cities-0.3.4/README.md
--rw-r--r--   0        0        0      477 2024-05-29 20:17:27.103324 french_cities-0.3.4/french_cities/__init__.py
--rw-r--r--   0        0        0    31689 2024-05-29 20:17:27.103324 french_cities-0.3.4/french_cities/city_finder.py
--rw-r--r--   0        0        0    11143 2024-05-29 20:17:27.103324 french_cities-0.3.4/french_cities/departement_finder.py
--rw-r--r--   0        0        0      805 2024-05-29 20:17:27.103324 french_cities-0.3.4/french_cities/utils.py
--rw-r--r--   0        0        0     8302 2024-05-29 20:17:27.103324 french_cities-0.3.4/french_cities/vintage.py
--rw-r--r--   0        0        0     1358 2024-05-29 20:17:27.103324 french_cities-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    20579 1970-01-01 00:00:00.000000 french_cities-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    10260 2024-05-30 20:24:14.879881 french_cities-0.3.5/README.fr.md
+-rw-r--r--   0        0        0     8729 2024-05-30 20:24:14.879881 french_cities-0.3.5/README.md
+-rw-r--r--   0        0        0      477 2024-05-30 20:24:14.883881 french_cities-0.3.5/french_cities/__init__.py
+-rw-r--r--   0        0        0    31806 2024-05-30 20:24:14.883881 french_cities-0.3.5/french_cities/city_finder.py
+-rw-r--r--   0        0        0    11143 2024-05-30 20:24:14.883881 french_cities-0.3.5/french_cities/departement_finder.py
+-rw-r--r--   0        0        0      805 2024-05-30 20:24:14.883881 french_cities-0.3.5/french_cities/utils.py
+-rw-r--r--   0        0        0     8302 2024-05-30 20:24:14.883881 french_cities-0.3.5/french_cities/vintage.py
+-rw-r--r--   0        0        0     1358 2024-05-30 20:24:14.883881 french_cities-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0    20579 1970-01-01 00:00:00.000000 french_cities-0.3.5/PKG-INFO
```

### Comparing `french_cities-0.3.4/README.fr.md` & `french_cities-0.3.5/README.fr.md`

 * *Files identical despite different names*

### Comparing `french_cities-0.3.4/README.md` & `french_cities-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `french_cities-0.3.4/french_cities/city_finder.py` & `french_cities-0.3.5/french_cities/city_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,16 @@
             df.loc[ix, postcode] = df.loc[ix, postcode].str.zfill(5)
     except KeyError:
         pass
 
     components_kept = list(
         {field for test_cols, _ in to_test_ok for field in test_cols}
     )
+    for f in components_kept:
+        df[f] = df[f].replace("", np.nan)
 
     addresses = df.loc[:, components_kept + ["candidat_0"]].drop_duplicates()
 
     # Add dep recognition if not already there, just to check the result's
     # coherence (and NOT to compute city recognition using it!)
     if not dep:
         dep = "dep"
@@ -560,15 +562,15 @@
             cdist(
                 look_for.loc[ix1, "city_cleaned"],
                 df.loc[ix2, "TITLE_SHORT"],
                 score_cutoff=80,
                 workers=-1,
             ),
             index=ix1,
-            columns=df.loc[ix2, "CODE"],
+            columns=df.loc[ix2, ["TITLE_SHORT", "CODE"]],
         ).replace(0, np.nan)
 
         try:
             results.append(
                 pd.Series(
                     match_.dropna(how="all", axis=1)
                     .dropna(how="all")
@@ -576,15 +578,15 @@
                     index=ix1,
                 )
             )
         except ValueError:
             continue
 
     results = pd.concat(results, ignore_index=False).sort_index()
-
+    results = results.str[1]
     try:
         year = int(year)
     except ValueError:
         year = date.today().year
     results = set_vintage(results.to_frame("CODE"), year, "CODE")
 
     results = look_for.join(results)
```

### Comparing `french_cities-0.3.4/french_cities/departement_finder.py` & `french_cities-0.3.5/french_cities/departement_finder.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.3.4/french_cities/utils.py` & `french_cities-0.3.5/french_cities/utils.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.3.4/french_cities/vintage.py` & `french_cities-0.3.5/french_cities/vintage.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.3.4/pyproject.toml` & `french_cities-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "french-cities"
-version = "0.3.4"
+version = "0.3.5"
 description = "Toolbox on french cities: set vintage, find departments, find cities..."
 authors = ["thomas.grandjean <thomas.grandjean@developpement-durable.gouv.fr>"]
 license = "GPL-3.0-or-later"
 readme = ["README.md", "README.fr.md"]
 homepage = "https://github.com/tgrandje/french-cities/"
 repository = "https://github.com/tgrandje/french-cities/"
 documentation = "https://github.com/tgrandje/french-cities/"
```

### Comparing `french_cities-0.3.4/PKG-INFO` & `french_cities-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: french-cities
-Version: 0.3.4
+Version: 0.3.5
 Summary: Toolbox on french cities: set vintage, find departments, find cities...
 Home-page: https://github.com/tgrandje/french-cities/
 License: GPL-3.0-or-later
 Keywords: france,cities
 Author: thomas.grandjean
 Author-email: thomas.grandjean@developpement-durable.gouv.fr
 Requires-Python: >=3.9,<4.0
```

