# Comparing `tmp/pikobs-2.0.8.tar.gz` & `tmp/pikobs-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikobs-2.0.8.tar", last modified: Wed May 29 18:36:28 2024, max compression
+gzip compressed data, was "pikobs-2.0.9.tar", last modified: Wed May 29 18:47:25 2024, max compression
```

## Comparing `pikobs-2.0.8.tar` & `pikobs-2.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:36:28.708247 pikobs-2.0.8/
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)       40 2024-05-29 18:22:16.000000 pikobs-2.0.8/MANIFEST.in
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      261 2024-05-29 18:36:28.707973 pikobs-2.0.8/PKG-INFO
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:22:26.000000 pikobs-2.0.8/README.md
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)        6 2024-05-29 18:22:36.000000 pikobs-2.0.8/VERSION
-drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:36:28.687352 pikobs-2.0.8/pikobs/
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      140 2024-05-03 18:07:10.000000 pikobs-2.0.8/pikobs/__init__.py
-drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:36:28.689168 pikobs-2.0.8/pikobs/cardio/
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)       50 2024-05-01 13:40:01.000000 pikobs-2.0.8/pikobs/cardio/__init__.py
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)    15595 2024-05-17 14:19:09.000000 pikobs-2.0.8/pikobs/cardio/cardio.py
--rwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)    16748 2024-05-08 13:52:51.000000 pikobs-2.0.8/pikobs/cardio/cardio_plot.py
-drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:36:28.704581 pikobs-2.0.8/pikobs/configobs/
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      194 2024-05-06 15:28:28.000000 pikobs-2.0.8/pikobs/configobs/__init__.py
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      740 2024-04-30 18:54:05.000000 pikobs-2.0.8/pikobs/configobs/delete_folder.py
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)     5322 2024-05-10 20:31:10.000000 pikobs-2.0.8/pikobs/configobs/familyobs.py
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)     1189 2024-04-30 14:23:41.000000 pikobs-2.0.8/pikobs/configobs/flags_criteria.py
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)     4458 2024-04-30 14:09:27.000000 pikobs-2.0.8/pikobs/configobs/regionsobs.py
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      627 2024-05-29 13:39:37.000000 pikobs-2.0.8/pikobs/configobs/type_boxes.py
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)     4175 2024-05-10 20:04:43.000000 pikobs-2.0.8/pikobs/configobs/type_projection.py
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)     1712 2024-05-23 13:36:30.000000 pikobs-2.0.8/pikobs/configobs/type_varno.py
-drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:36:28.705231 pikobs-2.0.8/pikobs/profile/
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)       52 2024-05-02 22:38:20.000000 pikobs-2.0.8/pikobs/profile/__init__.py
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)    16591 2024-05-22 00:12:16.000000 pikobs-2.0.8/pikobs/profile/profile.py
--rwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)    15866 2024-05-08 17:58:27.000000 pikobs-2.0.8/pikobs/profile/profile_plot.py
-drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:36:28.706061 pikobs-2.0.8/pikobs/scatter/
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)       51 2024-04-30 18:24:53.000000 pikobs-2.0.8/pikobs/scatter/__init__.py
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)    17934 2024-05-29 16:40:05.000000 pikobs-2.0.8/pikobs/scatter/scatter.py
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)    14696 2024-05-29 18:19:17.000000 pikobs-2.0.8/pikobs/scatter/scatter_plot.py
-drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:36:28.706614 pikobs-2.0.8/pikobs/timeserie/
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)       56 2024-05-01 18:31:39.000000 pikobs-2.0.8/pikobs/timeserie/__init__.py
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)    15217 2024-05-08 13:27:23.000000 pikobs-2.0.8/pikobs/timeserie/timeserie.py
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)    14742 2024-05-03 13:09:35.000000 pikobs-2.0.8/pikobs/timeserie/timeserie_plot.py
-drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:36:28.707636 pikobs-2.0.8/pikobs/vdedr/
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)       48 2024-05-05 00:05:59.000000 pikobs-2.0.8/pikobs/vdedr/__init__.py
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)    16366 2024-05-06 14:54:47.000000 pikobs-2.0.8/pikobs/vdedr/vdedr.py
--rwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)    14412 2024-05-06 15:14:42.000000 pikobs-2.0.8/pikobs/vdedr/vdedr_plot.py
-drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:36:28.688628 pikobs-2.0.8/pikobs.egg-info/
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      261 2024-05-29 18:36:28.687637 pikobs-2.0.8/pikobs.egg-info/PKG-INFO
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      878 2024-05-29 18:36:28.687990 pikobs-2.0.8/pikobs.egg-info/SOURCES.txt
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)        1 2024-05-29 18:36:28.688211 pikobs-2.0.8/pikobs.egg-info/dependency_links.txt
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      162 2024-05-29 18:36:28.688438 pikobs-2.0.8/pikobs.egg-info/requires.txt
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)        7 2024-05-29 18:36:28.688665 pikobs-2.0.8/pikobs.egg-info/top_level.txt
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)       38 2024-05-29 18:36:28.708298 pikobs-2.0.8/setup.cfg
--rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      983 2024-05-29 18:36:25.000000 pikobs-2.0.8/setup.py
+drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:47:25.042323 pikobs-2.0.9/
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)       40 2024-05-29 18:22:16.000000 pikobs-2.0.9/MANIFEST.in
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      261 2024-05-29 18:47:25.042008 pikobs-2.0.9/PKG-INFO
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:22:26.000000 pikobs-2.0.9/README.md
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)        6 2024-05-29 18:43:26.000000 pikobs-2.0.9/VERSION
+drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:47:24.959832 pikobs-2.0.9/pikobs/
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      140 2024-05-03 18:07:10.000000 pikobs-2.0.9/pikobs/__init__.py
+drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:47:24.961668 pikobs-2.0.9/pikobs/cardio/
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)       50 2024-05-01 13:40:01.000000 pikobs-2.0.9/pikobs/cardio/__init__.py
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)    15595 2024-05-17 14:19:09.000000 pikobs-2.0.9/pikobs/cardio/cardio.py
+-rwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)    16748 2024-05-08 13:52:51.000000 pikobs-2.0.9/pikobs/cardio/cardio_plot.py
+drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:47:24.963452 pikobs-2.0.9/pikobs/configobs/
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      194 2024-05-06 15:28:28.000000 pikobs-2.0.9/pikobs/configobs/__init__.py
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      740 2024-04-30 18:54:05.000000 pikobs-2.0.9/pikobs/configobs/delete_folder.py
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)     5322 2024-05-10 20:31:10.000000 pikobs-2.0.9/pikobs/configobs/familyobs.py
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)     1189 2024-04-30 14:23:41.000000 pikobs-2.0.9/pikobs/configobs/flags_criteria.py
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)     4458 2024-04-30 14:09:27.000000 pikobs-2.0.9/pikobs/configobs/regionsobs.py
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      627 2024-05-29 13:39:37.000000 pikobs-2.0.9/pikobs/configobs/type_boxes.py
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)     4175 2024-05-10 20:04:43.000000 pikobs-2.0.9/pikobs/configobs/type_projection.py
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)     1712 2024-05-23 13:36:30.000000 pikobs-2.0.9/pikobs/configobs/type_varno.py
+drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:47:24.964588 pikobs-2.0.9/pikobs/profile/
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)       52 2024-05-02 22:38:20.000000 pikobs-2.0.9/pikobs/profile/__init__.py
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)    16591 2024-05-22 00:12:16.000000 pikobs-2.0.9/pikobs/profile/profile.py
+-rwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)    15866 2024-05-08 17:58:27.000000 pikobs-2.0.9/pikobs/profile/profile_plot.py
+drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:47:24.986138 pikobs-2.0.9/pikobs/scatter/
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)       51 2024-04-30 18:24:53.000000 pikobs-2.0.9/pikobs/scatter/__init__.py
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)    17934 2024-05-29 16:40:05.000000 pikobs-2.0.9/pikobs/scatter/scatter.py
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)    14696 2024-05-29 18:19:17.000000 pikobs-2.0.9/pikobs/scatter/scatter_plot.py
+drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:47:25.007484 pikobs-2.0.9/pikobs/timeserie/
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)       56 2024-05-01 18:31:39.000000 pikobs-2.0.9/pikobs/timeserie/__init__.py
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)    15217 2024-05-08 13:27:23.000000 pikobs-2.0.9/pikobs/timeserie/timeserie.py
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)    14742 2024-05-03 13:09:35.000000 pikobs-2.0.9/pikobs/timeserie/timeserie_plot.py
+drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:47:25.022422 pikobs-2.0.9/pikobs/vdedr/
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)       48 2024-05-05 00:05:59.000000 pikobs-2.0.9/pikobs/vdedr/__init__.py
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)    16366 2024-05-06 14:54:47.000000 pikobs-2.0.9/pikobs/vdedr/vdedr.py
+-rwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)    14412 2024-05-06 15:14:42.000000 pikobs-2.0.9/pikobs/vdedr/vdedr_plot.py
+drwxr-xr-x   0 dlo001   (67268) eccc_cmda (66068)        0 2024-05-29 18:47:24.960692 pikobs-2.0.9/pikobs.egg-info/
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      261 2024-05-29 18:47:24.960073 pikobs-2.0.9/pikobs.egg-info/PKG-INFO
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      878 2024-05-29 18:47:24.960236 pikobs-2.0.9/pikobs.egg-info/SOURCES.txt
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)        1 2024-05-29 18:47:24.960401 pikobs-2.0.9/pikobs.egg-info/dependency_links.txt
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      154 2024-05-29 18:47:24.960565 pikobs-2.0.9/pikobs.egg-info/requires.txt
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)        7 2024-05-29 18:47:24.960737 pikobs-2.0.9/pikobs.egg-info/top_level.txt
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)       38 2024-05-29 18:47:25.042377 pikobs-2.0.9/setup.cfg
+-rw-r--r--   0 dlo001   (67268) eccc_cmda (66068)      974 2024-05-29 18:44:27.000000 pikobs-2.0.9/setup.py
```

### Comparing `pikobs-2.0.8/pikobs/cardio/cardio.py` & `pikobs-2.0.9/pikobs/cardio/cardio.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/cardio/cardio_plot.py` & `pikobs-2.0.9/pikobs/cardio/cardio_plot.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/configobs/delete_folder.py` & `pikobs-2.0.9/pikobs/configobs/delete_folder.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/configobs/familyobs.py` & `pikobs-2.0.9/pikobs/configobs/familyobs.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/configobs/flags_criteria.py` & `pikobs-2.0.9/pikobs/configobs/flags_criteria.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/configobs/regionsobs.py` & `pikobs-2.0.9/pikobs/configobs/regionsobs.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/configobs/type_boxes.py` & `pikobs-2.0.9/pikobs/configobs/type_boxes.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/configobs/type_projection.py` & `pikobs-2.0.9/pikobs/configobs/type_projection.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/configobs/type_varno.py` & `pikobs-2.0.9/pikobs/configobs/type_varno.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/profile/profile.py` & `pikobs-2.0.9/pikobs/profile/profile.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/profile/profile_plot.py` & `pikobs-2.0.9/pikobs/profile/profile_plot.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/scatter/scatter.py` & `pikobs-2.0.9/pikobs/scatter/scatter.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/scatter/scatter_plot.py` & `pikobs-2.0.9/pikobs/scatter/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/timeserie/timeserie.py` & `pikobs-2.0.9/pikobs/timeserie/timeserie.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/timeserie/timeserie_plot.py` & `pikobs-2.0.9/pikobs/timeserie/timeserie_plot.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/vdedr/vdedr.py` & `pikobs-2.0.9/pikobs/vdedr/vdedr.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs/vdedr/vdedr_plot.py` & `pikobs-2.0.9/pikobs/vdedr/vdedr_plot.py`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/pikobs.egg-info/SOURCES.txt` & `pikobs-2.0.9/pikobs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pikobs-2.0.8/setup.py` & `pikobs-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,9 +19,9 @@
     author='David Lobon',
     author_email='dhlobon@gmail.com',
     description="pikobs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),    
     python_requires='>=3.8', 
-    install_requires=['matplotlib','numpy >= 1.17.0','cartopy>= 0.18.0', 'geopandas==0.10.0', 'earthpy==0.9.4', 'shapely==1.7.0',  'cartopy==0.18.0', 'h5py','packaging', 'pygrib', 'domutils' ,'dask==2022.9.1', 'scipy', 'pytz'],
+    install_requires=['matplotlib','numpy >= 1.17.0','cartopy', 'geopandas==0.10.0', 'earthpy==0.9.4', 'shapely==1.7.0',  'cartopy==0.18.0', 'h5py','packaging', 'pygrib', 'domutils' ,'dask==2022.9.1', 'scipy', 'pytz'],
 )
```

