# Comparing `tmp/tidypath-1.3.8.tar.gz` & `tmp/tidypath-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidypath-1.3.8.tar", last modified: Fri May  3 15:45:12 2024, max compression
+gzip compressed data, was "tidypath-1.3.9.tar", last modified: Thu May 30 13:41:36 2024, max compression
```

## Comparing `tidypath-1.3.8.tar` & `tidypath-1.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-05-03 15:45:12.172061 tidypath-1.3.8/
--rwxr-xr-x   0 userx     (1000) wheel      (998)    35149 2023-06-08 21:46:44.000000 tidypath-1.3.8/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     3682 2024-05-03 15:45:12.172061 tidypath-1.3.8/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)     2804 2023-06-08 21:46:44.000000 tidypath-1.3.8/README.md
--rwxr-xr-x   0 userx     (1000) wheel      (998)      106 2024-05-03 15:45:12.172061 tidypath-1.3.8/setup.cfg
--rwxr-xr-x   0 userx     (1000) wheel      (998)     1161 2024-05-03 15:44:54.000000 tidypath-1.3.8/setup.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-05-03 15:45:12.172061 tidypath-1.3.8/tidypath/
--rwxr-xr-x   0 userx     (1000) wheel      (998)      371 2023-09-01 13:40:54.000000 tidypath-1.3.8/tidypath/__init__.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     1629 2023-06-08 21:46:44.000000 tidypath-1.3.8/tidypath/_helper.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     4998 2024-02-21 23:01:12.000000 tidypath-1.3.8/tidypath/config.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)    14688 2024-05-03 15:44:47.000000 tidypath-1.3.8/tidypath/decorators.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     6165 2023-07-01 08:06:57.000000 tidypath-1.3.8/tidypath/fmt.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     5197 2023-06-08 21:46:44.000000 tidypath-1.3.8/tidypath/inspection.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)    14158 2024-02-14 00:36:13.000000 tidypath-1.3.8/tidypath/paths.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     9844 2023-06-08 21:46:44.000000 tidypath-1.3.8/tidypath/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-05-03 15:45:12.172061 tidypath-1.3.8/tidypath.egg-info/
--rwxr-xr-x   0 userx     (1000) wheel      (998)     3682 2024-05-03 15:45:12.000000 tidypath-1.3.8/tidypath.egg-info/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)      358 2024-05-03 15:45:12.000000 tidypath-1.3.8/tidypath.egg-info/SOURCES.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2024-05-03 15:45:12.000000 tidypath-1.3.8/tidypath.egg-info/dependency_links.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)       63 2024-05-03 15:45:12.000000 tidypath-1.3.8/tidypath.egg-info/requires.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        9 2024-05-03 15:45:12.000000 tidypath-1.3.8/tidypath.egg-info/top_level.txt
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-30 13:41:36.139047 tidypath-1.3.9/
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)    35149 2023-09-08 10:22:16.000000 tidypath-1.3.9/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2024-05-30 13:41:36.139047 tidypath-1.3.9/PKG-INFO
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     2804 2023-09-08 10:22:16.000000 tidypath-1.3.9/README.md
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)      106 2024-05-30 13:41:36.143047 tidypath-1.3.9/setup.cfg
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     1161 2024-05-30 13:41:15.000000 tidypath-1.3.9/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-30 13:41:36.131047 tidypath-1.3.9/tidypath/
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)      371 2023-09-08 10:22:16.000000 tidypath-1.3.9/tidypath/__init__.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     1629 2023-09-08 10:22:16.000000 tidypath-1.3.9/tidypath/_helper.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     4998 2024-04-05 11:52:19.000000 tidypath-1.3.9/tidypath/config.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)    14770 2024-05-30 13:41:07.000000 tidypath-1.3.9/tidypath/decorators.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     6165 2023-09-08 10:22:17.000000 tidypath-1.3.9/tidypath/fmt.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     5197 2023-09-08 10:22:17.000000 tidypath-1.3.9/tidypath/inspection.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)    14158 2024-04-05 11:52:19.000000 tidypath-1.3.9/tidypath/paths.py
+-rwxr-xr-x   0 jorgemedina  (1236) users      (100)     9844 2023-09-08 10:22:17.000000 tidypath-1.3.9/tidypath/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-30 13:41:36.139047 tidypath-1.3.9/tidypath.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2024-05-30 13:41:35.000000 tidypath-1.3.9/tidypath.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      358 2024-05-30 13:41:36.000000 tidypath-1.3.9/tidypath.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-05-30 13:41:35.000000 tidypath-1.3.9/tidypath.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       63 2024-05-30 13:41:35.000000 tidypath-1.3.9/tidypath.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        9 2024-05-30 13:41:35.000000 tidypath-1.3.9/tidypath.egg-info/top_level.txt
```

### Comparing `tidypath-1.3.8/LICENSE.md` & `tidypath-1.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.8/PKG-INFO` & `tidypath-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.3.8
+Version: 1.3.9
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidypath-1.3.8/README.md` & `tidypath-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.8/setup.py` & `tidypath-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tidypath',
-    version='1.3.8',
+    version='1.3.9',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=['tidypath'],
     url='https://github.com/medinajorge/tidypath',
     download_url='https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz',
     description="Automatically store/load data in a tidy, efficient way.",
     long_description=open('README.md').read(),
```

### Comparing `tidypath-1.3.8/tidypath/_helper.py` & `tidypath-1.3.9/tidypath/_helper.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.8/tidypath/config.py` & `tidypath-1.3.9/tidypath/config.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.8/tidypath/decorators.py` & `tidypath-1.3.9/tidypath/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,18 +111,19 @@
                 filename = os.path.basename(saving_path)
                 if len(filename) > max_str_length:
                     saving_path = hash_path(saving_path)
                     warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
                 return saving_path
 
             result = None
-            def compute_and_save(result, ext, saving_path):
+            def compute(result, ext, saving_path):
                 if result is None:
                     result = func(*args, **kwargs)
-                getattr(storage, f"save_{ext}")(result, saving_path, **save_opts)
+                if save:
+                    getattr(storage, f"save_{ext}")(result, saving_path, **save_opts)
                 return result
 
             if isinstance(ext, str):
                 ext = [ext]
             for ext_i in ext:
                 saving_path = get_saving_path(ext_i)
                 if skip_computation and not Path(saving_path).exists():
@@ -133,27 +134,27 @@
                         result = getattr(storage, f"load_{ext_i}")(saving_path, **load_opts)
                     except EOFError or LZMAError or _lzma.LZMAError:
                         if skip_computation:
                             warnings.warn("Corrupted file. Skipping computation ...", RuntimeWarning)
                             return SavedataSkippedComputation()
                         else:
                             warnings.warn("Corrupted file. Recomputing and storing ...", RuntimeWarning)
-                            result = compute_and_save(result, ext_i, saving_path)
+                            result = compute(result, ext_i, saving_path)
                     except KeyboardInterrupt:
                         raise KeyboardInterrupt
                     except Exception as e:
                         print(e)
                         if skip_computation:
                             warnings.warn("Corrupted file. Skipping computation ...", RuntimeWarning)
                             return SavedataSkippedComputation()
                         else:
                             warnings.warn("Corrupted file. Recomputing and storing ...", RuntimeWarning)
-                            result = compute_and_save(result, ext_i, saving_path)
+                            result = compute(result, ext_i, saving_path)
                 else:
-                    result = compute_and_save(result, ext_i, saving_path)
+                    result = compute(result, ext_i, saving_path)
             return result
 
         wrapper.__signature__ = merge_wrapper_signatures(wrapper, ["overwrite", "keys", "save", "funcname_in_filename", "skip_computation", "ext"])
         wrapper.__out__ = "data"
         return wrapper
 
     if func is None:
@@ -228,35 +229,36 @@
                         warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
                     return saving_path
 
                 if is_mpl_axes:
                     fig = fig.get_figure()
                 is_mpl = isinstance(fig, mpl_figure)
 
-                if isinstance(ext, str):
-                    ext = [ext]
-                for ext_i in ext:
-                    saving_path = get_saving_path(ext_i)
-                    if not Path(saving_path).exists() or overwrite:
-                        if is_mpl:
-                            fig.savefig(saving_path, format=ext_i, **{**mpl_save_defaults, **save_opts})
-                        elif isinstance(fig, plotly_figure):
-                            if ext_i == "html":
-                                fig.write_html(saving_path, **save_opts)
+                if save:
+                    if isinstance(ext, str):
+                        ext = [ext]
+                    for ext_i in ext:
+                        saving_path = get_saving_path(ext_i)
+                        if not Path(saving_path).exists() or overwrite:
+                            if is_mpl:
+                                fig.savefig(saving_path, format=ext_i, **{**mpl_save_defaults, **save_opts})
+                            elif isinstance(fig, plotly_figure):
+                                if ext_i == "html":
+                                    fig.write_html(saving_path, **save_opts)
+                                else:
+                                    fig.write_image(saving_path, format=ext_i, **save_opts)
                             else:
-                                fig.write_image(saving_path, format=ext_i, **save_opts)
-                        else:
-                            raise TypeError(f"fig type '{type(fig)}' not valid. Available: 'matplotlib.figure.Figure', 'matplotlib.axes._subplots.AxesSubplot', 'plotly.grap_objs._figure.Figure'.")
+                                raise TypeError(f"fig type '{type(fig)}' not valid. Available: 'matplotlib.figure.Figure', 'matplotlib.axes._subplots.AxesSubplot', 'plotly.grap_objs._figure.Figure'.")
 
-                if is_mpl:
-                    plt.close(fig)
 
                 if return_fig:
                     return fig
                 else:
+                    if is_mpl:
+                        plt.close(fig)
                     return
             elif fig is None or math.isnan(fig):
                 warnings.warn("Expected output figure (plotly or matplotlib) and received None or NaN.", RuntimeWarning)
             else:
                 warnings.warn("Expected output figure (plotly, matplotlib) or a flag for figure error computation (None, NaN), but received {}".format(type(fig)), RuntimeWarning)
 
         wrapper.__signature__ = merge_wrapper_signatures(wrapper, ["overwrite", "keys", "save", "funcname_in_filename", "return_fig", "ext"])
```

### Comparing `tidypath-1.3.8/tidypath/fmt.py` & `tidypath-1.3.9/tidypath/fmt.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.8/tidypath/inspection.py` & `tidypath-1.3.9/tidypath/inspection.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.8/tidypath/paths.py` & `tidypath-1.3.9/tidypath/paths.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.8/tidypath/storage.py` & `tidypath-1.3.9/tidypath/storage.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.8/tidypath.egg-info/PKG-INFO` & `tidypath-1.3.9/tidypath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.3.8
+Version: 1.3.9
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

