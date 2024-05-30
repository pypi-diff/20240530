# Comparing `tmp/neurocaps-0.9.4.post1.tar.gz` & `tmp/neurocaps-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.9.4.post1.tar", last modified: Wed May 29 01:05:21 2024, max compression
+gzip compressed data, was "neurocaps-0.9.5.tar", last modified: Thu May 30 18:29:22 2024, max compression
```

## Comparing `neurocaps-0.9.4.post1.tar` & `neurocaps-0.9.5.tar`

### file list

```diff
@@ -1,40 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.143163 neurocaps-0.9.4.post1/
--rw-rw-rw-   0        0        0     1077 2024-04-28 16:38:21.000000 neurocaps-0.9.4.post1/LICENSE.md
--rw-rw-rw-   0        0        0    17016 2024-05-29 01:05:21.143163 neurocaps-0.9.4.post1/PKG-INFO
--rw-rw-rw-   0        0        0    15453 2024-05-28 18:55:10.000000 neurocaps-0.9.4.post1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.086144 neurocaps-0.9.4.post1/neurocaps/
--rw-rw-rw-   0        0        0       72 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.116421 neurocaps-0.9.4.post1/neurocaps/_utils/
--rw-rw-rw-   0        0        0      363 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.119165 neurocaps-0.9.4.post1/neurocaps/_utils/_cap_internals/
--rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_cap_internals/__init__.py
--rw-rw-rw-   0        0        0     2531 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-rw-rw-   0        0        0      184 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
-drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.126961 neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/
--rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-rw-rw-   0        0        0     2187 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
--rw-rw-rw-   0        0        0     5777 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-rw-rw-   0        0        0     8190 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-rw-rw-   0        0        0     2680 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.131695 neurocaps-0.9.4.post1/neurocaps/analysis/
--rw-rw-rw-   0        0        0      139 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/analysis/__init__.py
--rw-rw-rw-   0        0        0    72959 2024-05-28 18:55:10.000000 neurocaps-0.9.4.post1/neurocaps/analysis/cap.py
--rw-rw-rw-   0        0        0     4791 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/analysis/merge.py
--rw-rw-rw-   0        0        0     1626 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/analysis/standardize.py
-drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.133604 neurocaps-0.9.4.post1/neurocaps/extraction/
--rw-rw-rw-   0        0        0       87 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/extraction/__init__.py
--rw-rw-rw-   0        0        0    33356 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/extraction/timeseriesextractor.py
-drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.140702 neurocaps-0.9.4.post1/neurocaps.egg-info/
--rw-rw-rw-   0        0        0    17016 2024-05-29 01:05:21.000000 neurocaps-0.9.4.post1/neurocaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2024-05-29 01:05:21.000000 neurocaps-0.9.4.post1/neurocaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 01:05:21.000000 neurocaps-0.9.4.post1/neurocaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      150 2024-05-29 01:05:21.000000 neurocaps-0.9.4.post1/neurocaps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-29 01:05:21.000000 neurocaps-0.9.4.post1/neurocaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1731 2024-05-29 00:57:01.000000 neurocaps-0.9.4.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-29 01:05:21.143163 neurocaps-0.9.4.post1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.140702 neurocaps-0.9.4.post1/tests/
--rw-rw-rw-   0        0        0     6471 2024-05-02 14:49:04.000000 neurocaps-0.9.4.post1/tests/test_CAP.py
--rw-rw-rw-   0        0        0     4687 2024-05-25 04:47:35.000000 neurocaps-0.9.4.post1/tests/test_TimeseriesExtractor.py
--rw-rw-rw-   0        0        0     1077 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/tests/test_TimeseriesExtractor_additional.py
--rw-rw-rw-   0        0        0     1931 2024-05-02 14:49:04.000000 neurocaps-0.9.4.post1/tests/test_merge_dicts.py
--rw-rw-rw-   0        0        0      691 2024-05-14 02:35:32.000000 neurocaps-0.9.4.post1/tests/test_standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.563119 neurocaps-0.9.5/
+-rw-rw-rw-   0        0        0     1077 2024-05-29 20:07:23.000000 neurocaps-0.9.5/LICENSE.md
+-rw-rw-rw-   0        0        0       11 2024-05-29 20:41:29.000000 neurocaps-0.9.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    18746 2024-05-30 18:29:22.563119 neurocaps-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0    17191 2024-05-30 18:27:19.000000 neurocaps-0.9.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.486673 neurocaps-0.9.5/neurocaps/
+-rw-rw-rw-   0        0        0       72 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.523719 neurocaps-0.9.5/neurocaps/_utils/
+-rw-rw-rw-   0        0        0      363 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.534387 neurocaps-0.9.5/neurocaps/_utils/_cap_internals/
+-rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.5/neurocaps/_utils/_cap_internals/__init__.py
+-rw-rw-rw-   0        0        0     2531 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-rw-rw-   0        0        0      184 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.542200 neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-rw-rw-   0        0        0     2187 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
+-rw-rw-rw-   0        0        0     5777 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-rw-rw-   0        0        0     8190 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-rw-rw-   0        0        0     2680 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.549153 neurocaps-0.9.5/neurocaps/analysis/
+-rw-rw-rw-   0        0        0      139 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/analysis/__init__.py
+-rw-rw-rw-   0        0        0    75038 2024-05-30 17:55:51.000000 neurocaps-0.9.5/neurocaps/analysis/cap.py
+-rw-rw-rw-   0        0        0     4791 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/analysis/merge.py
+-rw-rw-rw-   0        0        0     1626 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/analysis/standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.549153 neurocaps-0.9.5/neurocaps/extraction/
+-rw-rw-rw-   0        0        0       87 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/extraction/__init__.py
+-rw-rw-rw-   0        0        0    33356 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/extraction/timeseriesextractor.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.563119 neurocaps-0.9.5/neurocaps.egg-info/
+-rw-rw-rw-   0        0        0    18746 2024-05-30 18:29:22.000000 neurocaps-0.9.5/neurocaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      955 2024-05-30 18:29:22.000000 neurocaps-0.9.5/neurocaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 18:29:22.000000 neurocaps-0.9.5/neurocaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2024-05-30 18:29:22.000000 neurocaps-0.9.5/neurocaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-30 18:29:22.000000 neurocaps-0.9.5/neurocaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1725 2024-05-30 07:32:22.000000 neurocaps-0.9.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 18:29:22.563119 neurocaps-0.9.5/setup.cfg
```

### Comparing `neurocaps-0.9.4.post1/LICENSE.md` & `neurocaps-0.9.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4.post1/PKG-INFO` & `neurocaps-0.9.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.4.post1
+Version: 0.9.5
 Summary: Co-activation Patterns (CAPs) Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Project-URL: Issues, https://github.com/donishadsmith/neurocaps/issues
 Project-URL: Changelog, https://github.com/donishadsmith/neurocaps/blob/main/CHANGELOG.md
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
@@ -115,17 +115,17 @@
 - **Saving Timeseries:** Save the nested dictionary containing timeseries as a pickle file.
 - **Visualization:** Visualize the timeseries of a Schaefer, AAL, or Custom parcellation node or region/network in a specific subject's run, with options to save the plots.
 - **Parallel Processing:** Use parallel processing by specifying the number of CPU cores in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with TimeseriesExtractor.`get_bold()` to extract session 1 and 2 BOLD timeseries from 105 subjects from resting-state data (single run containing 360 volumes) and two task datasets (three runs containing 200 volumes each and two runs containing 200 volumes) reduced processing time from 5 hours 48 minutes to 1 hour 26 minutes (using 10 cores).
 
 **Main features for `CAP` includes:**
 - **Optimal Cluster Size Identification:** Perform the silhouette or elbow method to identify the optimal cluster size, saving the optimal model as an attribute.
 - **Grouping:** Perform CAPs analysis independently on groups of subject IDs. K-means clustering, silhouette and elbow methods, and plotting are done for each group when specified.
-- **CAP Visualization:** Visualize the CAPs as outer products or heatmaps, with options to use subplots to reduce the number of individual plots. You can save and use the plots. Refer to the docstring for the `caps2plot()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
-- **Surface Plot Visualization:** Convert the atlas used for parcellation to a stat map projected onto a surface plot. Refer to the docstring for the `caps2surf()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
-- **Correlation Matrix Creation:** Create a correlation matrix from CAPs. Refer to the docstring for the `caps2corr()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **CAP Visualization:** Visualize the CAPs as outer products or heatmaps, with options to use subplots to reduce the number of individual plots, as well as save. Refer to the docstring for the `caps2plot()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **Surface Plot Visualization:** Convert the atlas used for parcellation to a stat map projected onto a surface plot with options to customize and save plots. Refer to the docstring for the `caps2surf()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **Correlation Matrix Creation:** Create a correlation matrix from CAPs with options to customize and save plots. Refer to the docstring for the `caps2corr()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
 - **CAP Metrics Calculation:** Calculate CAP metrics as described in  [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2]:
     - *Temporal Fraction:* The proportion of total volumes spent in a single CAP over all volumes in a run.
     - *Persistence:* The average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time).
     - *Counts:* The frequency of each CAP observed in a run.
     - *Transition Frequency:* The number of switches between different CAPs across the entire run.
 
 **Additionally, the `neurocaps.analysis` submodule contains two additional functions:**
@@ -177,27 +177,34 @@
 cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
                     n_clusters=6)
 
 cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
                       standardize = True)
 
 # Visualize CAPs
+# You can use seaborn's premade palettes as strings or generate your own custom palettes
+# Using seaborn's diverging_palette function, matplotlib's LinearSegmentedColormap, 
+# or other Classes or functions compatable with seaborn
+
 cap_analysis.caps2plot(visual_scope="regions", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3, sharey=True, 
-                            subplots=True)
+                            subplots=True, cmap="coolwarm")
+# Create the colormap
+import seaborn as sns
+palette = sns.diverging_palette(260, 10, s=80, l=55, n=256, as_cmap=True)
 
 cap_analysis.caps2plot(visual_scope="nodes", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3,sharey=True, 
                             subplots=True, xlabel_rotation=90, tight_layout=False, 
-                            hspace = 0.4)
+                            hspace = 0.4, cmap=palette)
 
 ```
 **Plot Outputs:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/e1ab0f55-0c4c-4701-8f3a-838c2470d44d)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/43e46a0a-8721-4df9-88fa-04758a34142e)
 
 ```python
 
 # Get CAP metrics
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
                                          return_df=True, output_dir=output_dir,
                                          metrics=["temporal fraction", "persistence"],
@@ -218,25 +225,46 @@
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
 # Create surface plots of CAPs; there will be as many plots as CAPs
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
-cap_analysis.caps2surf(fwhm=2)
+cap_analysis.caps2surf(fwhm=2, cmap="cold_hot", layout="row",  size=(500, 100), zoom=1, cbar_location="bottom")
+
+#You can also generate your own colormaps using matplotlib's LinearSegmentedColormap
+
+# Create the colormap
+from matplotlib.colors import LinearSegmentedColormap
+colors = ["#1bfffe", "#00ccff", "#0099ff", "#0066ff", "#0033ff", "#c4c4c4",
+          "#ff6666", "#ff3333", "#FF0000","#ffcc00","#FFFF00"]
+custom_cmap = LinearSegmentedColormap.from_list("custom_cold_hot", colors, N=256)
+cap_analysis.caps2surf(fwhm=2, cmap=custom_cmap, size=(500, 100), layout="row")
 ```
-**Plot Output:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
+**Partial Plot Outputs:** (*Note*: one image will be generated per CAP)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/fadc946a-214b-4fbf-8316-2f32ab0b026e)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/8207914a-6bf0-47a9-8be8-3504d0a56516)
+
 
 ```python
 # Create correlation matrix
-cap_analysis.caps2corr(annot=True)
+cap_analysis.caps2corr(annot=True ,figsize=(6,4),cmap="coolwarm")
+
+# You can use seaborn's premade palettes as strings or generate your own custom palettes
+# Using seaborn's diverging_palette function, matplotlib's LinearSegmentedColormap, 
+# or other Classes or functions compatable with seaborn
+
+# Create the colormap
+import seaborn as sns
+palette = sns.diverging_palette(260, 10, s=80, l=55, n=256, as_cmap=True)
+cap_analysis.caps2corr(annot=True, ,figsize=(6,4), cmap=palette)
 ```
 **Plot Output:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/81620b36-55b0-4c83-be51-95d3f5280fa9)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/57a2ce81-13d3-40d0-93e7-0ca910f7b0be)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/9a8329df-65c7-4ad0-8b81-edc73f2d960d)
 
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single-subject open dataset to test the `TimeseriesExtractor` function on GitHub Actions. The open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. was also utilized. This data was obtained from the OpenfMRI database, accession number ds000031. 
 
 Modifications to the data included:
 
 - Truncating the preprocessed BOLD data and confounds from 448 timepoints to 40 timepoints.
```

### Comparing `neurocaps-0.9.4.post1/README.md` & `neurocaps-0.9.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -78,17 +78,17 @@
 - **Saving Timeseries:** Save the nested dictionary containing timeseries as a pickle file.
 - **Visualization:** Visualize the timeseries of a Schaefer, AAL, or Custom parcellation node or region/network in a specific subject's run, with options to save the plots.
 - **Parallel Processing:** Use parallel processing by specifying the number of CPU cores in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with TimeseriesExtractor.`get_bold()` to extract session 1 and 2 BOLD timeseries from 105 subjects from resting-state data (single run containing 360 volumes) and two task datasets (three runs containing 200 volumes each and two runs containing 200 volumes) reduced processing time from 5 hours 48 minutes to 1 hour 26 minutes (using 10 cores).
 
 **Main features for `CAP` includes:**
 - **Optimal Cluster Size Identification:** Perform the silhouette or elbow method to identify the optimal cluster size, saving the optimal model as an attribute.
 - **Grouping:** Perform CAPs analysis independently on groups of subject IDs. K-means clustering, silhouette and elbow methods, and plotting are done for each group when specified.
-- **CAP Visualization:** Visualize the CAPs as outer products or heatmaps, with options to use subplots to reduce the number of individual plots. You can save and use the plots. Refer to the docstring for the `caps2plot()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
-- **Surface Plot Visualization:** Convert the atlas used for parcellation to a stat map projected onto a surface plot. Refer to the docstring for the `caps2surf()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
-- **Correlation Matrix Creation:** Create a correlation matrix from CAPs. Refer to the docstring for the `caps2corr()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **CAP Visualization:** Visualize the CAPs as outer products or heatmaps, with options to use subplots to reduce the number of individual plots, as well as save. Refer to the docstring for the `caps2plot()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **Surface Plot Visualization:** Convert the atlas used for parcellation to a stat map projected onto a surface plot with options to customize and save plots. Refer to the docstring for the `caps2surf()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **Correlation Matrix Creation:** Create a correlation matrix from CAPs with options to customize and save plots. Refer to the docstring for the `caps2corr()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
 - **CAP Metrics Calculation:** Calculate CAP metrics as described in  [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2]:
     - *Temporal Fraction:* The proportion of total volumes spent in a single CAP over all volumes in a run.
     - *Persistence:* The average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time).
     - *Counts:* The frequency of each CAP observed in a run.
     - *Transition Frequency:* The number of switches between different CAPs across the entire run.
 
 **Additionally, the `neurocaps.analysis` submodule contains two additional functions:**
@@ -140,27 +140,34 @@
 cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
                     n_clusters=6)
 
 cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
                       standardize = True)
 
 # Visualize CAPs
+# You can use seaborn's premade palettes as strings or generate your own custom palettes
+# Using seaborn's diverging_palette function, matplotlib's LinearSegmentedColormap, 
+# or other Classes or functions compatable with seaborn
+
 cap_analysis.caps2plot(visual_scope="regions", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3, sharey=True, 
-                            subplots=True)
+                            subplots=True, cmap="coolwarm")
+# Create the colormap
+import seaborn as sns
+palette = sns.diverging_palette(260, 10, s=80, l=55, n=256, as_cmap=True)
 
 cap_analysis.caps2plot(visual_scope="nodes", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3,sharey=True, 
                             subplots=True, xlabel_rotation=90, tight_layout=False, 
-                            hspace = 0.4)
+                            hspace = 0.4, cmap=palette)
 
 ```
 **Plot Outputs:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/e1ab0f55-0c4c-4701-8f3a-838c2470d44d)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/43e46a0a-8721-4df9-88fa-04758a34142e)
 
 ```python
 
 # Get CAP metrics
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
                                          return_df=True, output_dir=output_dir,
                                          metrics=["temporal fraction", "persistence"],
@@ -181,25 +188,46 @@
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
 # Create surface plots of CAPs; there will be as many plots as CAPs
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
-cap_analysis.caps2surf(fwhm=2)
+cap_analysis.caps2surf(fwhm=2, cmap="cold_hot", layout="row",  size=(500, 100), zoom=1, cbar_location="bottom")
+
+#You can also generate your own colormaps using matplotlib's LinearSegmentedColormap
+
+# Create the colormap
+from matplotlib.colors import LinearSegmentedColormap
+colors = ["#1bfffe", "#00ccff", "#0099ff", "#0066ff", "#0033ff", "#c4c4c4",
+          "#ff6666", "#ff3333", "#FF0000","#ffcc00","#FFFF00"]
+custom_cmap = LinearSegmentedColormap.from_list("custom_cold_hot", colors, N=256)
+cap_analysis.caps2surf(fwhm=2, cmap=custom_cmap, size=(500, 100), layout="row")
 ```
-**Plot Output:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
+**Partial Plot Outputs:** (*Note*: one image will be generated per CAP)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/fadc946a-214b-4fbf-8316-2f32ab0b026e)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/8207914a-6bf0-47a9-8be8-3504d0a56516)
+
 
 ```python
 # Create correlation matrix
-cap_analysis.caps2corr(annot=True)
+cap_analysis.caps2corr(annot=True ,figsize=(6,4),cmap="coolwarm")
+
+# You can use seaborn's premade palettes as strings or generate your own custom palettes
+# Using seaborn's diverging_palette function, matplotlib's LinearSegmentedColormap, 
+# or other Classes or functions compatable with seaborn
+
+# Create the colormap
+import seaborn as sns
+palette = sns.diverging_palette(260, 10, s=80, l=55, n=256, as_cmap=True)
+cap_analysis.caps2corr(annot=True, ,figsize=(6,4), cmap=palette)
 ```
 **Plot Output:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/81620b36-55b0-4c83-be51-95d3f5280fa9)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/57a2ce81-13d3-40d0-93e7-0ca910f7b0be)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/9a8329df-65c7-4ad0-8b81-edc73f2d960d)
 
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single-subject open dataset to test the `TimeseriesExtractor` function on GitHub Actions. The open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. was also utilized. This data was obtained from the OpenfMRI database, accession number ds000031. 
 
 Modifications to the data included:
 
 - Truncating the preprocessed BOLD data and confounds from 448 timepoints to 40 timepoints.
@@ -219,8 +247,8 @@
 
 [^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
 
 [^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
 
 [^5]: Huang CC, Rolls ET, Feng J, Lin CP. An extended Human Connectome Project multimodal parcellation atlas of the human cortex and subcortical areas. Brain Struct Funct. 2022 Apr;227(3):763-778. Epub 2021 Nov 17. doi: 10.1007/s00429-021-02421-6
 
-[^6]: Huang CC, Rolls ET, Hsu CH, Feng J, Lin CP. Extensive Cortical Connectivity of the Human Hippocampal Memory System: Beyond the "What" and "Where" Dual Stream Model. Cerebral Cortex. 2021 May 19;bhab113. doi: 10.1093/cercor/bhab113.
+[^6]: Huang CC, Rolls ET, Hsu CH, Feng J, Lin CP. Extensive Cortical Connectivity of the Human Hippocampal Memory System: Beyond the "What" and "Where" Dual Stream Model. Cerebral Cortex. 2021 May 19;bhab113. doi: 10.1093/cercor/bhab113.
```

### Comparing `neurocaps-0.9.4.post1/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.9.5/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py` & `neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4.post1/neurocaps/analysis/cap.py` & `neurocaps-0.9.5/neurocaps/analysis/cap.py`

 * *Files 3% similar despite different names*

```diff
@@ -330,16 +330,21 @@
                 Rotation angle for x-axis labels.
             - "ylabel_rotation": int, default=0
                 Rotation angle for y-axis labels.
             - "annot": bool, default=False
                 Add values to cells on the outer product heatmap at the region level only.
             - "linewidths": float, default=0
                 Padding between each cell in the plot.
-            - "cmap": str, default="coolwarm"
-                Color map for the cells in the plot.
+            - "cmap": str, Class, or function, default="coolwarm"
+                Color map for the cells in the plot. For this parameter, you can use premade color palettes or create custom ones.
+                Below is a list of valid options:
+                - Strings to call seaborn's premade palettes. Refer to seaborn's documentation for valid options.
+                - Seaborn's diverging_palette function to generate custom palettes.
+                - Matplotlib's LinearSegmentedColormap to generate custom palettes.
+                - Other classes or functions compatible with seaborn.
     
          Notes
         -----
         If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. Also, this function assumes that the background label is "zero". Do not add a a background label, in the "nodes" or "networks" key,
         the zero index should correspond the first id that is not zero.
 
         Custom Key Structure:
@@ -873,16 +878,21 @@
                 Rotation angle for x-axis labels.
             - "ylabel_rotation": int, default=0
                 Rotation angle for y-axis labels.
             - "annot": bool, default=False
                 Add values to each cell.
             - "linewidths": float, default=0
                 Padding between each cell in the plot.
-            - "cmap": str, default="coolwarm"
-                Color map for the cells in the plot.
+            - "cmap": str, Class, or function, default="coolwarm"
+                Color map for the cells in the plot. For this parameter, you can use premade color palettes or create custom ones.
+                Below is a list of valid options:
+                - Strings to call seaborn's premade palettes. Refer to seaborn's documentation for valid options.
+                - Seaborn's diverging_palette function to generate custom palettes.
+                - Matplotlib's LinearSegmentedColormap to generate custom palettes.
+                - Other classes or functions compatible with seaborn.
         """
         import matplotlib.pyplot as plt, os, pandas as pd
         from seaborn import heatmap
 
         if not hasattr(self,"_caps"):
             raise AttributeError("Cannot plot caps since `self._caps` attribute does not exist. Run `self.get_caps()` first.")
         
@@ -951,16 +961,19 @@
             If True, saves the statistical map for each CAP for all groups as a Nifti1Image if `output_dir` is provided.
         **kwargs : dict
             Additional parameters to pass to modify certain plot parameters. Options include:
             - "dpi": int, default=300
                 Dots per inch for the plot.
             - "title_pad": int, default=-3
                 Padding for the plot title.
-            - "cmap": str, default="cold_hot"
-                Colormap to be used for the plot.
+            - "cmap": str or Class, default="cold_hot"
+                Colormap to be used for the plot. For this parameter, you can use premade color palettes or create custom ones.
+                Below is a list of valid options:
+                - Strings to call nilearn's _cmap_d fuction. Refer to documention for nilearn's _cmap_d for valid palettes.
+                - Matplotlib's LinearSegmentedColormap to generate custom colormaps.
             - "cbar_location": str, default="bottom"
                 Location of the colorbar.
             - "cbar_draw_border": bool, default=False
                 Whether to draw a border around the colorbar.
             - "cbar_aspect": int, default=20
                 Aspect ratio of the colorbar.
             - "cbar_shrink": float, default=0.2
@@ -987,14 +1000,16 @@
                 Views to be displayed in the plot.
             - "brightness": float, default=0.5
                 Brightness level of the plot.
             - "figsize": tuple or None, default=None
                 Size of the figure.
             - "scale": tuple, default=(2, 2)
                 Scale factors for the plot.
+            - "surface": str, default="inflated"
+                The surface atlas that is used for plotting. Options are "inflated" or "veryinflated"
 
             Please refer to surfplot's documentation for specifics: 
             https://surfplot.readthedocs.io/en/latest/generated/surfplot.plotting.Plot.html#surfplot.plotting.Plot.
 
         Returns
         -------
         Nifti1Image
@@ -1036,14 +1051,15 @@
                          size = kwargs["size"] if kwargs and "size" in kwargs.keys() else (500,400),
                          layout = kwargs["layout"] if kwargs and "layout" in kwargs.keys() else "grid",
                          zoom = kwargs["zoom"] if kwargs and "zoom" in kwargs.keys() else 1.5,
                          views = kwargs["views"] if kwargs and "views" in kwargs.keys() else ["lateral", "medial"],
                          brightness = kwargs["brightness"] if kwargs and "brightness" in kwargs.keys() else 0.5,
                          figsize = kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else None,
                          scale = kwargs["scale"] if kwargs and "scale" in kwargs.keys() else (2,2),
+                         surface = kwargs["surface"] if kwargs and "surface" in kwargs.keys() else "inflated"
                          )
         
         if kwargs:
             invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
             if len(invalid_kwargs.keys()) > 0:
                 print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
 
@@ -1060,31 +1076,36 @@
                 # Add smoothing to stat map to help mitigate potential coverage issues 
                 if fwhm != None:
                     stat_map = image.smooth_img(stat_map, fwhm=fwhm)
 
                 # Code slightly adapted from surfplot example 2
                 gii_lh, gii_rh = mni152_to_fslr(stat_map, method=method, fslr_density=fslr_density)
                 surfaces = fetch_fslr()
-                lh, rh = surfaces['inflated']
+                if plot_dict["surface"] not in ["inflated", "veryinflated"]:
+                    warnings.warn(f"{plot_dict['surface']} is an invalid option for `surface`. Available options include 'inflated' or 'verinflated'. Defaulting to 'inflated'")
+                    plot_dict["surface"] = "inflated"
+                lh, rh = surfaces[plot_dict["surface"]]
                 lh = str(lh) if not isinstance(lh, str) else lh
                 rh = str(rh) if not isinstance(rh, str) else rh
                 sulc_lh, sulc_rh = surfaces['sulc']
                 sulc_lh = str(sulc_lh) if not isinstance(sulc_lh, str) else sulc_lh
                 sulc_rh = str(sulc_rh) if not isinstance(sulc_rh, str) else sulc_rh
                 p = Plot(lh, rh, size=plot_dict["size"], layout=plot_dict["layout"], zoom=plot_dict["zoom"],
                          views=plot_dict["views"], brightness=plot_dict["brightness"])
 
                 # Add base layer
                 p.add_layer({"left": sulc_lh, "right": sulc_rh}, cmap="binary_r", cbar=False)
 
                 plot_min = -1 if round(atlas_fdata.min()) == 0 else round(atlas_fdata.min())
                 plot_max = 1 if round(atlas_fdata.max()) == 0 else round(atlas_fdata.max())
-
+                
+                # Check cmap
+                cmap = _cmap_d[plot_dict["cmap"]] if isinstance(plot_dict["cmap"],str) else plot_dict["cmap"]
                 # Add stat map layer
-                p.add_layer({"left": gii_lh, "right": gii_rh}, cmap=_cmap_d[plot_dict["cmap"]], 
+                p.add_layer({"left": gii_lh, "right": gii_rh}, cmap=cmap, 
                             alpha=plot_dict["cbar_alpha"], color_range=(plot_min,plot_max))
 
                 # Color bar
                 kws = dict(location=plot_dict["cbar_location"], draw_border=plot_dict["cbar_draw_border"], aspect=plot_dict["cbar_aspect"], shrink=plot_dict["cbar_shrink"],
                         decimals=plot_dict["cbar_decimals"], pad=plot_dict["cbar_pad"], fraction=plot_dict["cbar_fraction"], n_ticks=plot_dict["cbar_n_ticks"], 
                         fontsize=plot_dict["cbar_fontsize"])
                 fig = p.build(cbar_kws=kws, figsize=plot_dict["figsize"], scale=plot_dict["scale"])
```

### Comparing `neurocaps-0.9.4.post1/neurocaps/analysis/merge.py` & `neurocaps-0.9.5/neurocaps/analysis/merge.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4.post1/neurocaps/analysis/standardize.py` & `neurocaps-0.9.5/neurocaps/analysis/standardize.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4.post1/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.9.5/neurocaps/extraction/timeseriesextractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4.post1/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.9.5/neurocaps.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.4.post1
+Version: 0.9.5
 Summary: Co-activation Patterns (CAPs) Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Project-URL: Issues, https://github.com/donishadsmith/neurocaps/issues
 Project-URL: Changelog, https://github.com/donishadsmith/neurocaps/blob/main/CHANGELOG.md
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
@@ -115,17 +115,17 @@
 - **Saving Timeseries:** Save the nested dictionary containing timeseries as a pickle file.
 - **Visualization:** Visualize the timeseries of a Schaefer, AAL, or Custom parcellation node or region/network in a specific subject's run, with options to save the plots.
 - **Parallel Processing:** Use parallel processing by specifying the number of CPU cores in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with TimeseriesExtractor.`get_bold()` to extract session 1 and 2 BOLD timeseries from 105 subjects from resting-state data (single run containing 360 volumes) and two task datasets (three runs containing 200 volumes each and two runs containing 200 volumes) reduced processing time from 5 hours 48 minutes to 1 hour 26 minutes (using 10 cores).
 
 **Main features for `CAP` includes:**
 - **Optimal Cluster Size Identification:** Perform the silhouette or elbow method to identify the optimal cluster size, saving the optimal model as an attribute.
 - **Grouping:** Perform CAPs analysis independently on groups of subject IDs. K-means clustering, silhouette and elbow methods, and plotting are done for each group when specified.
-- **CAP Visualization:** Visualize the CAPs as outer products or heatmaps, with options to use subplots to reduce the number of individual plots. You can save and use the plots. Refer to the docstring for the `caps2plot()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
-- **Surface Plot Visualization:** Convert the atlas used for parcellation to a stat map projected onto a surface plot. Refer to the docstring for the `caps2surf()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
-- **Correlation Matrix Creation:** Create a correlation matrix from CAPs. Refer to the docstring for the `caps2corr()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **CAP Visualization:** Visualize the CAPs as outer products or heatmaps, with options to use subplots to reduce the number of individual plots, as well as save. Refer to the docstring for the `caps2plot()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **Surface Plot Visualization:** Convert the atlas used for parcellation to a stat map projected onto a surface plot with options to customize and save plots. Refer to the docstring for the `caps2surf()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **Correlation Matrix Creation:** Create a correlation matrix from CAPs with options to customize and save plots. Refer to the docstring for the `caps2corr()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
 - **CAP Metrics Calculation:** Calculate CAP metrics as described in  [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2]:
     - *Temporal Fraction:* The proportion of total volumes spent in a single CAP over all volumes in a run.
     - *Persistence:* The average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time).
     - *Counts:* The frequency of each CAP observed in a run.
     - *Transition Frequency:* The number of switches between different CAPs across the entire run.
 
 **Additionally, the `neurocaps.analysis` submodule contains two additional functions:**
@@ -177,27 +177,34 @@
 cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
                     n_clusters=6)
 
 cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
                       standardize = True)
 
 # Visualize CAPs
+# You can use seaborn's premade palettes as strings or generate your own custom palettes
+# Using seaborn's diverging_palette function, matplotlib's LinearSegmentedColormap, 
+# or other Classes or functions compatable with seaborn
+
 cap_analysis.caps2plot(visual_scope="regions", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3, sharey=True, 
-                            subplots=True)
+                            subplots=True, cmap="coolwarm")
+# Create the colormap
+import seaborn as sns
+palette = sns.diverging_palette(260, 10, s=80, l=55, n=256, as_cmap=True)
 
 cap_analysis.caps2plot(visual_scope="nodes", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3,sharey=True, 
                             subplots=True, xlabel_rotation=90, tight_layout=False, 
-                            hspace = 0.4)
+                            hspace = 0.4, cmap=palette)
 
 ```
 **Plot Outputs:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/e1ab0f55-0c4c-4701-8f3a-838c2470d44d)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/43e46a0a-8721-4df9-88fa-04758a34142e)
 
 ```python
 
 # Get CAP metrics
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
                                          return_df=True, output_dir=output_dir,
                                          metrics=["temporal fraction", "persistence"],
@@ -218,25 +225,46 @@
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
 # Create surface plots of CAPs; there will be as many plots as CAPs
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
-cap_analysis.caps2surf(fwhm=2)
+cap_analysis.caps2surf(fwhm=2, cmap="cold_hot", layout="row",  size=(500, 100), zoom=1, cbar_location="bottom")
+
+#You can also generate your own colormaps using matplotlib's LinearSegmentedColormap
+
+# Create the colormap
+from matplotlib.colors import LinearSegmentedColormap
+colors = ["#1bfffe", "#00ccff", "#0099ff", "#0066ff", "#0033ff", "#c4c4c4",
+          "#ff6666", "#ff3333", "#FF0000","#ffcc00","#FFFF00"]
+custom_cmap = LinearSegmentedColormap.from_list("custom_cold_hot", colors, N=256)
+cap_analysis.caps2surf(fwhm=2, cmap=custom_cmap, size=(500, 100), layout="row")
 ```
-**Plot Output:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
+**Partial Plot Outputs:** (*Note*: one image will be generated per CAP)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/fadc946a-214b-4fbf-8316-2f32ab0b026e)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/8207914a-6bf0-47a9-8be8-3504d0a56516)
+
 
 ```python
 # Create correlation matrix
-cap_analysis.caps2corr(annot=True)
+cap_analysis.caps2corr(annot=True ,figsize=(6,4),cmap="coolwarm")
+
+# You can use seaborn's premade palettes as strings or generate your own custom palettes
+# Using seaborn's diverging_palette function, matplotlib's LinearSegmentedColormap, 
+# or other Classes or functions compatable with seaborn
+
+# Create the colormap
+import seaborn as sns
+palette = sns.diverging_palette(260, 10, s=80, l=55, n=256, as_cmap=True)
+cap_analysis.caps2corr(annot=True, ,figsize=(6,4), cmap=palette)
 ```
 **Plot Output:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/81620b36-55b0-4c83-be51-95d3f5280fa9)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/57a2ce81-13d3-40d0-93e7-0ca910f7b0be)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/9a8329df-65c7-4ad0-8b81-edc73f2d960d)
 
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single-subject open dataset to test the `TimeseriesExtractor` function on GitHub Actions. The open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. was also utilized. This data was obtained from the OpenfMRI database, accession number ds000031. 
 
 Modifications to the data included:
 
 - Truncating the preprocessed BOLD data and confounds from 448 timepoints to 40 timepoints.
```

### Comparing `neurocaps-0.9.4.post1/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.9.5/neurocaps.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE.md
+MANIFEST.in
 README.md
 pyproject.toml
 neurocaps/__init__.py
 neurocaps.egg-info/PKG-INFO
 neurocaps.egg-info/SOURCES.txt
 neurocaps.egg-info/dependency_links.txt
 neurocaps.egg-info/requires.txt
@@ -17,13 +18,8 @@
 neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
 neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
 neurocaps/analysis/__init__.py
 neurocaps/analysis/cap.py
 neurocaps/analysis/merge.py
 neurocaps/analysis/standardize.py
 neurocaps/extraction/__init__.py
-neurocaps/extraction/timeseriesextractor.py
-tests/test_CAP.py
-tests/test_TimeseriesExtractor.py
-tests/test_TimeseriesExtractor_additional.py
-tests/test_merge_dicts.py
-tests/test_standardize.py
+neurocaps/extraction/timeseriesextractor.py
```

### Comparing `neurocaps-0.9.4.post1/pyproject.toml` & `neurocaps-0.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,108 +2,107 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6e65 7572 6f63 6170 7322 0d0a 7665   "neurocaps"..ve
-00000080: 7273 696f 6e20 3d20 2230 2e39 2e34 2e70  rsion = "0.9.4.p
-00000090: 6f73 7431 220d 0a6c 6963 656e 7365 203d  ost1"..license =
-000000a0: 207b 7465 7874 203d 2022 4d49 5420 4c69   {text = "MIT Li
-000000b0: 6365 6e73 6522 7d0d 0a61 7574 686f 7273  cense"}..authors
-000000c0: 203d 205b 7b6e 616d 6520 3d20 2244 6f6e   = [{name = "Don
-000000d0: 6973 6861 2053 6d69 7468 222c 2065 6d61  isha Smith", ema
-000000e0: 696c 203d 2022 646f 6e69 7368 6173 6d69  il = "donishasmi
-000000f0: 7468 406f 7574 6c6f 6f6b 2e63 6f6d 227d  th@outlook.com"}
-00000100: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
-00000110: 2022 436f 2d61 6374 6976 6174 696f 6e20   "Co-activation 
-00000120: 5061 7474 6572 6e73 2028 4341 5073 2920  Patterns (CAPs) 
-00000130: 5079 7468 6f6e 2070 6163 6b61 6765 220d  Python package".
-00000140: 0a72 6561 646d 6520 3d20 2252 4541 444d  .readme = "READM
-00000150: 452e 6d64 220d 0a72 6571 7569 7265 732d  E.md"..requires-
-00000160: 7079 7468 6f6e 203d 2022 3e3d 332e 392e  python = ">=3.9.
-00000170: 3022 0d0a 6b65 7977 6f72 6473 203d 205b  0"..keywords = [
-00000180: 2270 7974 686f 6e22 2c20 2243 6f2d 4163  "python", "Co-Ac
-00000190: 7469 7661 7469 6f6e 2050 6174 7465 726e  tivation Pattern
-000001a0: 7322 2c20 2243 4150 7322 2c20 226e 6575  s", "CAPs", "neu
-000001b0: 726f 696d 6167 696e 6722 2c20 2266 6d72  roimaging", "fmr
-000001c0: 6922 2c20 2264 6663 222c 2022 6479 6e61  i", "dfc", "dyna
-000001d0: 6d69 6320 6675 6e63 7469 6f6e 616c 2063  mic functional c
-000001e0: 6f6e 6e65 6374 6976 6974 7922 2c20 2266  onnectivity", "f
-000001f0: 4d52 4950 7265 7022 5d0d 0a63 6c61 7373  MRIPrep"]..class
-00000200: 6966 6965 7273 203d 205b 0d0a 2020 2020  ifiers = [..    
-00000210: 2249 6e74 656e 6465 6420 4175 6469 656e  "Intended Audien
-00000220: 6365 203a 3a20 4564 7563 6174 696f 6e22  ce :: Education"
-00000230: 2c0d 0a20 2020 2022 496e 7465 6e64 6564  ,..    "Intended
-00000240: 2041 7564 6965 6e63 6520 3a3a 2053 6369   Audience :: Sci
-00000250: 656e 6365 2f52 6573 6561 7263 6822 2c0d  ence/Research",.
-00000260: 0a20 2020 2022 546f 7069 6320 3a3a 2053  .    "Topic :: S
-00000270: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
-00000280: 6572 696e 6722 2c0d 0a20 2020 2022 4c69  ering",..    "Li
-00000290: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-000002a0: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
-000002b0: 656e 7365 222c 0d0a 2020 2020 2250 726f  ense",..    "Pro
-000002c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002e0: 2e39 222c 0d0a 2020 2020 2250 726f 6772  .9",..    "Progr
-000002f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000300: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000310: 3022 2c0d 0a20 2020 2022 5072 6f67 7261  0",..    "Progra
-00000320: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000330: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
-00000340: 222c 0d0a 2020 2020 2250 726f 6772 616d  ",..    "Program
-00000350: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000360: 2050 7974 686f 6e20 3a3a 2033 2e31 3222   Python :: 3.12"
-00000370: 2c0d 0a20 2020 2022 4f70 6572 6174 696e  ,..    "Operatin
-00000380: 6720 5379 7374 656d 203a 3a20 4d61 634f  g System :: MacO
-00000390: 5320 3a3a 204d 6163 4f53 2058 222c 0d0a  S :: MacOS X",..
-000003a0: 2020 2020 224f 7065 7261 7469 6e67 2053      "Operating S
-000003b0: 7973 7465 6d20 3a3a 2050 4f53 4958 203a  ystem :: POSIX :
-000003c0: 3a20 4c69 6e75 7822 2c0d 0a20 2020 2022  : Linux",..    "
-000003d0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-000003e0: 203a 3a20 4d69 6372 6f73 6f66 7420 3a3a   :: Microsoft ::
-000003f0: 2057 696e 646f 7773 203a 3a20 5769 6e64   Windows :: Wind
-00000400: 6f77 7320 3131 222c 0d0a 2020 2020 2244  ows 11",..    "D
-00000410: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
-00000420: 7320 3a3a 2034 202d 2042 6574 6122 0d0a  s :: 4 - Beta"..
-00000430: 5d0d 0a64 6570 656e 6465 6e63 6965 7320  ]..dependencies 
-00000440: 3d20 5b22 6e75 6d70 7922 2c0d 0a20 2020  = ["numpy",..   
-00000450: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
-00000460: 6e64 6173 222c 0d0a 2020 2020 2020 2020  ndas",..        
-00000470: 2020 2020 2020 2020 226d 6174 706c 6f74          "matplot
-00000480: 6c69 6222 2c0d 0a20 2020 2020 2020 2020  lib",..         
-00000490: 2020 2020 2020 2022 7365 6162 6f72 6e22         "seaborn"
-000004a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000004b0: 2020 2022 6b6e 6565 6422 2c0d 0a20 2020     "kneed",..   
-000004c0: 2020 2020 2020 2020 2020 2020 2022 6e69               "ni
-000004d0: 6261 6265 6c22 2c0d 0a20 2020 2020 2020  babel",..       
-000004e0: 2020 2020 2020 2020 2022 6e69 6c65 6172           "nilear
-000004f0: 6e3e 3d30 2e31 302e 312c 2021 3d30 2e31  n>=0.10.1, !=0.1
-00000500: 302e 3322 2c0d 0a20 2020 2020 2020 2020  0.3",..         
-00000510: 2020 2020 2020 2022 7363 696b 6974 2d6c         "scikit-l
-00000520: 6561 726e 3e3d 312e 342e 3022 2c0d 0a20  earn>=1.4.0",.. 
-00000530: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000540: 7375 7266 706c 6f74 222c 0d0a 2020 2020  surfplot",..    
-00000550: 2020 2020 2020 2020 2020 2020 226e 6575              "neu
-00000560: 726f 6d61 7073 222c 0d0a 2020 2020 2020  romaps",..      
-00000570: 2020 2020 2020 2020 2020 2270 7962 6964            "pybid
-00000580: 733b 2070 6c61 7466 6f72 6d5f 7379 7374  s; platform_syst
-00000590: 656d 2021 3d20 2757 696e 646f 7773 2722  em != 'Windows'"
-000005a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000005b0: 2020 5d0d 0a0d 0a5b 7072 6f6a 6563 742e    ]....[project.
-000005c0: 7572 6c73 5d0d 0a48 6f6d 6570 6167 6520  urls]..Homepage 
-000005d0: 3d20 2268 7474 7073 3a2f 2f67 6974 6875  = "https://githu
-000005e0: 622e 636f 6d2f 646f 6e69 7368 6164 736d  b.com/donishadsm
-000005f0: 6974 682f 6e65 7572 6f63 6170 7322 2020  ith/neurocaps"  
-00000600: 0d0a 4973 7375 6573 203d 2022 6874 7470  ..Issues = "http
-00000610: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-00000620: 6f6e 6973 6861 6473 6d69 7468 2f6e 6575  onishadsmith/neu
-00000630: 726f 6361 7073 2f69 7373 7565 7322 2020  rocaps/issues"  
-00000640: 0d0a 4368 616e 6765 6c6f 6720 3d20 2268  ..Changelog = "h
-00000650: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000660: 6d2f 646f 6e69 7368 6164 736d 6974 682f  m/donishadsmith/
-00000670: 6e65 7572 6f63 6170 732f 626c 6f62 2f6d  neurocaps/blob/m
-00000680: 6169 6e2f 4348 414e 4745 4c4f 472e 6d64  ain/CHANGELOG.md
-00000690: 220d 0a0d 0a5b 746f 6f6c 2e64 6973 7475  "....[tool.distu
-000006a0: 7469 6c73 2e62 6469 7374 5f77 6865 656c  tils.bdist_wheel
-000006b0: 5d0d 0a75 6e69 7665 7273 616c 203d 2074  ]..universal = t
-000006c0: 7275 65                                  rue
+00000080: 7273 696f 6e20 3d20 2230 2e39 2e35 220d  rsion = "0.9.5".
+00000090: 0a6c 6963 656e 7365 203d 207b 7465 7874  .license = {text
+000000a0: 203d 2022 4d49 5420 4c69 6365 6e73 6522   = "MIT License"
+000000b0: 7d0d 0a61 7574 686f 7273 203d 205b 7b6e  }..authors = [{n
+000000c0: 616d 6520 3d20 2244 6f6e 6973 6861 2053  ame = "Donisha S
+000000d0: 6d69 7468 222c 2065 6d61 696c 203d 2022  mith", email = "
+000000e0: 646f 6e69 7368 6173 6d69 7468 406f 7574  donishasmith@out
+000000f0: 6c6f 6f6b 2e63 6f6d 227d 5d0d 0a64 6573  look.com"}]..des
+00000100: 6372 6970 7469 6f6e 203d 2022 436f 2d61  cription = "Co-a
+00000110: 6374 6976 6174 696f 6e20 5061 7474 6572  ctivation Patter
+00000120: 6e73 2028 4341 5073 2920 5079 7468 6f6e  ns (CAPs) Python
+00000130: 2070 6163 6b61 6765 220d 0a72 6561 646d   package"..readm
+00000140: 6520 3d20 2252 4541 444d 452e 6d64 220d  e = "README.md".
+00000150: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
+00000160: 203d 2022 3e3d 332e 392e 3022 0d0a 6b65   = ">=3.9.0"..ke
+00000170: 7977 6f72 6473 203d 205b 2270 7974 686f  ywords = ["pytho
+00000180: 6e22 2c20 2243 6f2d 4163 7469 7661 7469  n", "Co-Activati
+00000190: 6f6e 2050 6174 7465 726e 7322 2c20 2243  on Patterns", "C
+000001a0: 4150 7322 2c20 226e 6575 726f 696d 6167  APs", "neuroimag
+000001b0: 696e 6722 2c20 2266 6d72 6922 2c20 2264  ing", "fmri", "d
+000001c0: 6663 222c 2022 6479 6e61 6d69 6320 6675  fc", "dynamic fu
+000001d0: 6e63 7469 6f6e 616c 2063 6f6e 6e65 6374  nctional connect
+000001e0: 6976 6974 7922 2c20 2266 4d52 4950 7265  ivity", "fMRIPre
+000001f0: 7022 5d0d 0a63 6c61 7373 6966 6965 7273  p"]..classifiers
+00000200: 203d 205b 0d0a 2020 2020 2249 6e74 656e   = [..    "Inten
+00000210: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00000220: 4564 7563 6174 696f 6e22 2c0d 0a20 2020  Education",..   
+00000230: 2022 496e 7465 6e64 6564 2041 7564 6965   "Intended Audie
+00000240: 6e63 6520 3a3a 2053 6369 656e 6365 2f52  nce :: Science/R
+00000250: 6573 6561 7263 6822 2c0d 0a20 2020 2022  esearch",..    "
+00000260: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
+00000270: 6669 632f 456e 6769 6e65 6572 696e 6722  fic/Engineering"
+00000280: 2c0d 0a20 2020 2022 4c69 6365 6e73 6520  ,..    "License 
+00000290: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+000002a0: 3a3a 204d 4954 204c 6963 656e 7365 222c  :: MIT License",
+000002b0: 0d0a 2020 2020 2250 726f 6772 616d 6d69  ..    "Programmi
+000002c0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002d0: 7974 686f 6e20 3a3a 2033 2e39 222c 0d0a  ython :: 3.9",..
+000002e0: 2020 2020 2250 726f 6772 616d 6d69 6e67      "Programming
+000002f0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000300: 686f 6e20 3a3a 2033 2e31 3022 2c0d 0a20  hon :: 3.10",.. 
+00000310: 2020 2022 5072 6f67 7261 6d6d 696e 6720     "Programming 
+00000320: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000330: 6f6e 203a 3a20 332e 3131 222c 0d0a 2020  on :: 3.11",..  
+00000340: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
+00000350: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000360: 6e20 3a3a 2033 2e31 3222 2c0d 0a20 2020  n :: 3.12",..   
+00000370: 2022 4f70 6572 6174 696e 6720 5379 7374   "Operating Syst
+00000380: 656d 203a 3a20 4d61 634f 5320 3a3a 204d  em :: MacOS :: M
+00000390: 6163 4f53 2058 222c 0d0a 2020 2020 224f  acOS X",..    "O
+000003a0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000003b0: 3a3a 2050 4f53 4958 203a 3a20 4c69 6e75  :: POSIX :: Linu
+000003c0: 7822 2c0d 0a20 2020 2022 4f70 6572 6174  x",..    "Operat
+000003d0: 696e 6720 5379 7374 656d 203a 3a20 4d69  ing System :: Mi
+000003e0: 6372 6f73 6f66 7420 3a3a 2057 696e 646f  crosoft :: Windo
+000003f0: 7773 203a 3a20 5769 6e64 6f77 7320 3131  ws :: Windows 11
+00000400: 222c 0d0a 2020 2020 2244 6576 656c 6f70  ",..    "Develop
+00000410: 6d65 6e74 2053 7461 7475 7320 3a3a 2034  ment Status :: 4
+00000420: 202d 2042 6574 6122 0d0a 5d0d 0a64 6570   - Beta"..]..dep
+00000430: 656e 6465 6e63 6965 7320 3d20 5b22 6e75  endencies = ["nu
+00000440: 6d70 7922 2c0d 0a20 2020 2020 2020 2020  mpy",..         
+00000450: 2020 2020 2020 2022 7061 6e64 6173 222c         "pandas",
+00000460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000470: 2020 226d 6174 706c 6f74 6c69 6222 2c0d    "matplotlib",.
+00000480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000490: 2022 7365 6162 6f72 6e22 2c0d 0a20 2020   "seaborn",..   
+000004a0: 2020 2020 2020 2020 2020 2020 2022 6b6e               "kn
+000004b0: 6565 6422 2c0d 0a20 2020 2020 2020 2020  eed",..         
+000004c0: 2020 2020 2020 2022 6e69 6261 6265 6c22         "nibabel"
+000004d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000004e0: 2020 2022 6e69 6c65 6172 6e3e 3d30 2e31     "nilearn>=0.1
+000004f0: 302e 312c 2021 3d30 2e31 302e 3322 2c0d  0.1, !=0.10.3",.
+00000500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000510: 2022 7363 696b 6974 2d6c 6561 726e 3e3d   "scikit-learn>=
+00000520: 312e 342e 3022 2c0d 0a20 2020 2020 2020  1.4.0",..       
+00000530: 2020 2020 2020 2020 2022 7375 7266 706c           "surfpl
+00000540: 6f74 222c 0d0a 2020 2020 2020 2020 2020  ot",..          
+00000550: 2020 2020 2020 226e 6575 726f 6d61 7073        "neuromaps
+00000560: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000570: 2020 2020 2270 7962 6964 733b 2070 6c61      "pybids; pla
+00000580: 7466 6f72 6d5f 7379 7374 656d 2021 3d20  tform_system != 
+00000590: 2757 696e 646f 7773 2722 0d0a 2020 2020  'Windows'"..    
+000005a0: 2020 2020 2020 2020 2020 2020 5d0d 0a0d              ]...
+000005b0: 0a5b 7072 6f6a 6563 742e 7572 6c73 5d0d  .[project.urls].
+000005c0: 0a48 6f6d 6570 6167 6520 3d20 2268 7474  .Homepage = "htt
+000005d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000005e0: 646f 6e69 7368 6164 736d 6974 682f 6e65  donishadsmith/ne
+000005f0: 7572 6f63 6170 7322 2020 0d0a 4973 7375  urocaps"  ..Issu
+00000600: 6573 203d 2022 6874 7470 733a 2f2f 6769  es = "https://gi
+00000610: 7468 7562 2e63 6f6d 2f64 6f6e 6973 6861  thub.com/donisha
+00000620: 6473 6d69 7468 2f6e 6575 726f 6361 7073  dsmith/neurocaps
+00000630: 2f69 7373 7565 7322 2020 0d0a 4368 616e  /issues"  ..Chan
+00000640: 6765 6c6f 6720 3d20 2268 7474 7073 3a2f  gelog = "https:/
+00000650: 2f67 6974 6875 622e 636f 6d2f 646f 6e69  /github.com/doni
+00000660: 7368 6164 736d 6974 682f 6e65 7572 6f63  shadsmith/neuroc
+00000670: 6170 732f 626c 6f62 2f6d 6169 6e2f 4348  aps/blob/main/CH
+00000680: 414e 4745 4c4f 472e 6d64 220d 0a0d 0a5b  ANGELOG.md"....[
+00000690: 746f 6f6c 2e64 6973 7475 7469 6c73 2e62  tool.distutils.b
+000006a0: 6469 7374 5f77 6865 656c 5d0d 0a75 6e69  dist_wheel]..uni
+000006b0: 7665 7273 616c 203d 2074 7275 65         versal = true
```

