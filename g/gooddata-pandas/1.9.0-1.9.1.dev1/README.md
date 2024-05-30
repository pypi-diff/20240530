# Comparing `tmp/gooddata-pandas-1.9.0.tar.gz` & `tmp/gooddata-pandas-1.9.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gooddata-pandas-1.9.0.tar", last modified: Thu Nov 16 13:25:00 2023, max compression
+gzip compressed data, was "gooddata-pandas-1.9.1.dev1.tar", last modified: Thu Dec 14 13:21:12 2023, max compression
```

## Comparing `gooddata-pandas-1.9.0.tar` & `gooddata-pandas-1.9.1.dev1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:25:00.094967 gooddata-pandas-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    77209 2023-11-16 13:24:41.000000 gooddata-pandas-1.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-16 13:24:41.000000 gooddata-pandas-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2023-11-16 13:25:00.094967 gooddata-pandas-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-11-16 13:24:41.000000 gooddata-pandas-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:25:00.094967 gooddata-pandas-1.9.0/gooddata_pandas/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-11-16 13:24:41.000000 gooddata-pandas-1.9.0/gooddata_pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-16 13:24:41.000000 gooddata-pandas-1.9.0/gooddata_pandas/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    18625 2023-11-16 13:24:41.000000 gooddata-pandas-1.9.0/gooddata_pandas/data_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2023-11-16 13:24:41.000000 gooddata-pandas-1.9.0/gooddata_pandas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2023-11-16 13:24:41.000000 gooddata-pandas-1.9.0/gooddata_pandas/good_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-16 13:24:41.000000 gooddata-pandas-1.9.0/gooddata_pandas/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    22864 2023-11-16 13:24:41.000000 gooddata-pandas-1.9.0/gooddata_pandas/result_convertor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2023-11-16 13:24:41.000000 gooddata-pandas-1.9.0/gooddata_pandas/series.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2023-11-16 13:24:41.000000 gooddata-pandas-1.9.0/gooddata_pandas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:25:00.094967 gooddata-pandas-1.9.0/gooddata_pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2023-11-16 13:25:00.000000 gooddata-pandas-1.9.0/gooddata_pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-11-16 13:25:00.000000 gooddata-pandas-1.9.0/gooddata_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 13:25:00.000000 gooddata-pandas-1.9.0/gooddata_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-16 13:25:00.000000 gooddata-pandas-1.9.0/gooddata_pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-16 13:25:00.000000 gooddata-pandas-1.9.0/gooddata_pandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 13:25:00.094967 gooddata-pandas-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-11-16 13:24:41.000000 gooddata-pandas-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:12.943474 gooddata-pandas-1.9.1.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    77209 2023-12-14 13:20:50.000000 gooddata-pandas-1.9.1.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-14 13:20:50.000000 gooddata-pandas-1.9.1.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2023-12-14 13:21:12.943474 gooddata-pandas-1.9.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-12-14 13:20:50.000000 gooddata-pandas-1.9.1.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:12.939474 gooddata-pandas-1.9.1.dev1/gooddata_pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2023-12-14 13:20:50.000000 gooddata-pandas-1.9.1.dev1/gooddata_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-14 13:20:50.000000 gooddata-pandas-1.9.1.dev1/gooddata_pandas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18625 2023-12-14 13:20:50.000000 gooddata-pandas-1.9.1.dev1/gooddata_pandas/data_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2023-12-14 13:20:50.000000 gooddata-pandas-1.9.1.dev1/gooddata_pandas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2023-12-14 13:20:50.000000 gooddata-pandas-1.9.1.dev1/gooddata_pandas/good_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-14 13:20:50.000000 gooddata-pandas-1.9.1.dev1/gooddata_pandas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    23035 2023-12-14 13:20:50.000000 gooddata-pandas-1.9.1.dev1/gooddata_pandas/result_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2023-12-14 13:20:50.000000 gooddata-pandas-1.9.1.dev1/gooddata_pandas/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2023-12-14 13:20:50.000000 gooddata-pandas-1.9.1.dev1/gooddata_pandas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:12.943474 gooddata-pandas-1.9.1.dev1/gooddata_pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2023-12-14 13:21:12.000000 gooddata-pandas-1.9.1.dev1/gooddata_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2023-12-14 13:21:12.000000 gooddata-pandas-1.9.1.dev1/gooddata_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 13:21:12.000000 gooddata-pandas-1.9.1.dev1/gooddata_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-14 13:21:12.000000 gooddata-pandas-1.9.1.dev1/gooddata_pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-14 13:21:12.000000 gooddata-pandas-1.9.1.dev1/gooddata_pandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 13:21:12.943474 gooddata-pandas-1.9.1.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2023-12-14 13:21:06.000000 gooddata-pandas-1.9.1.dev1/setup.py
```

### Comparing `gooddata-pandas-1.9.0/LICENSE.txt` & `gooddata-pandas-1.9.1.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.9.0/PKG-INFO` & `gooddata-pandas-1.9.1.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-pandas
-Version: 1.9.0
+Version: 1.9.1.dev1
 Summary: GoodData Cloud to pandas
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.9.0
+Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.9.1.dev1
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,pandas,series,data,frame,data_frame,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,30 +18,30 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: gooddata-sdk~=1.9.0
+Requires-Dist: gooddata-sdk~=1.9.1.dev1
 Requires-Dist: pandas<2.0.0,>=1.0.0
 
 # GoodData Pandas
 
 This package contains a thin layer that utilizes gooddata-sdk and allows you to conveniently create pandas series and
 data frames from the computations done against semantic model in your [GoodData.CN](https://www.gooddata.com/developers/cloud-native/) workspace.
 
 See [DOCUMENTATION](https://gooddata-pandas.readthedocs.io/en/latest/) for more details.
 
 ## Requirements
 
 -  GoodData.CN installation; either running on your cloud
    infrastructure or the free Community Edition running on your workstation
 
--  Python 3.7 or newer
+-  Python 3.8 or newer
 
 ## Installation
 
 Run the following command to install the `gooddata-pandas` package on your system:
 
     pip install gooddata-pandas
```

### Comparing `gooddata-pandas-1.9.0/README.md` & `gooddata-pandas-1.9.1.dev1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 See [DOCUMENTATION](https://gooddata-pandas.readthedocs.io/en/latest/) for more details.
 
 ## Requirements
 
 -  GoodData.CN installation; either running on your cloud
    infrastructure or the free Community Edition running on your workstation
 
--  Python 3.7 or newer
+-  Python 3.8 or newer
 
 ## Installation
 
 Run the following command to install the `gooddata-pandas` package on your system:
 
     pip install gooddata-pandas
```

### Comparing `gooddata-pandas-1.9.0/gooddata_pandas/data_access.py` & `gooddata-pandas-1.9.1.dev1/gooddata_pandas/data_access.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.9.0/gooddata_pandas/dataframe.py` & `gooddata-pandas-1.9.1.dev1/gooddata_pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.9.0/gooddata_pandas/good_pandas.py` & `gooddata-pandas-1.9.1.dev1/gooddata_pandas/good_pandas.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.9.0/gooddata_pandas/result_convertor.py` & `gooddata-pandas-1.9.1.dev1/gooddata_pandas/result_convertor.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         grand_total_headers (Tuple[Optional[_DataHeaders], Optional[_DataHeaders]]):
             Per-dimension grand total headers.
     """
 
     data: List[_DataArray]
     data_headers: Tuple[_DataHeaders, Optional[_DataHeaders]]
     grand_totals: Tuple[Optional[List[_DataArray]], Optional[List[_DataArray]]]
-    grand_total_headers: Tuple[Optional[_DataHeaders], Optional[_DataHeaders]]
+    grand_total_headers: Tuple[Optional[List[Dict[str, _DataHeaders]]], Optional[List[Dict[str, _DataHeaders]]]]
 
 
 @define
 class _AccumulatedData:
     """
     Utility class to offload code from the function that extracts all data and headers for a
     particular paged result. The method drives the paging and calls out to this class to accumulate
@@ -46,15 +46,17 @@
         grand_totals (List[Optional[List[_DataArray]]]): Holds the grand total data arrays.
         grand_totals_headers (List[Optional[_DataHeaders]]): Holds the headers for grand total data arrays.
     """
 
     data: List[_DataArray] = field(init=False, factory=list)
     data_headers: List[Optional[_DataHeaders]] = field(init=False, factory=lambda: [None, None])
     grand_totals: List[Optional[List[_DataArray]]] = field(init=False, factory=lambda: [None, None])
-    grand_totals_headers: List[Optional[_DataHeaders]] = field(init=False, factory=lambda: [None, None])
+    grand_totals_headers: List[Optional[List[Dict[str, _DataHeaders]]]] = field(
+        init=False, factory=lambda: [None, None]
+    )
 
     def accumulate_data(self, from_result: ExecutionResult) -> None:
         """
         Accumulate data from the ExecutionResult.
 
         If the result is one-dimensional, the data is a single array, so this adds the elements of that array
         into 'data'. If it's two-dimensional, the data is an array of arrays, so this adds as many arrays as
@@ -115,14 +117,22 @@
 
         # get dimension indexes mapping from response like {"dim1": 0, "dim0": 1}
         dim_idx_dict = {dim["localIdentifier"]: idx for idx, dim in enumerate(response.dimensions)}
 
         for grand_total in grand_totals:
             # 2-dim results have always 1-dim grand totals (3-dim results have 2-dim gt but DataFrame stores 2D only)
             dims = grand_total["totalDimensions"]
+
+            # if dims are empty then data contain total of column and row grandtotals so extend existing data array
+            if len(dims) == 0:
+                grand_totals_item = cast(List[_DataArray], self.grand_totals[0])
+                for total_idx, total_data in enumerate(grand_total["data"]):
+                    grand_totals_item[total_idx].extend(total_data)
+                continue
+
             assert len(dims) == 1, "Only 2-dimensional results are supported"
             dim_idx = dim_idx_dict[dims[0]]
             # the dimension id specified on the grand total says from what dimension were
             # the grand totals calculated (1 for column totals or 0 for row totals);
             #
             # the grand totals themselves should, however be placed in the opposite dimension:
             #
@@ -130,19 +140,15 @@
             # row totals are extra columns at the right 'edge' of the data
             opposite_dim = 1 if dim_idx == 0 else 0
 
             if self.grand_totals[opposite_dim] is None:
                 # grand totals not initialized yet; initialize both data and headers by making
                 # a shallow copy from the results
                 self.grand_totals[opposite_dim] = grand_total["data"][:]
-                # TODO: row total measure headers are currently not supported (only aggregation info w/o measure label)
-                #       measure header defs are under ["headerGroups"][>0]
-                self.grand_totals_headers[opposite_dim] = grand_total["dimensionHeaders"][0]["headerGroups"][0][
-                    "headers"
-                ][:]
+                self.grand_totals_headers[opposite_dim] = grand_total["dimensionHeaders"][0]["headerGroups"]
             elif paging_dim != opposite_dim:
                 # grand totals are already initialized and the code is paging in the direction that reveals
                 # additional grand total values; append them accordingly; no need to consider total headers:
                 # that is because only the grand total data is subject to paging
                 grand_totals_item = cast(List[_DataArray], self.grand_totals[opposite_dim])
                 if opposite_dim == 0:
                     # have column totals and paging 'to the right'; totals for the new columns are revealed so
@@ -442,18 +448,16 @@
     """
     headers: Tuple[_DataHeaders, Optional[_DataHeaders]] = extract.data_headers
 
     for dim_idx, grand_total_headers in enumerate(extract.grand_total_headers):
         if grand_total_headers is None:
             continue
         header = cast(List[List[Any]], headers[dim_idx])
-        header[0].extend(grand_total_headers)
-        padding = [None] * len(grand_total_headers)
-        for other_headers in header[1:]:
-            other_headers.extend(padding)
+        for level, grand_total_header in enumerate(grand_total_headers):
+            header[level].extend(grand_total_header["headers"])
 
     return headers
 
 
 def convert_execution_response_to_dataframe(
     execution_response: BareExecutionResponse,
     result_cache_metadata: ResultCacheMetadata,
```

### Comparing `gooddata-pandas-1.9.0/gooddata_pandas/series.py` & `gooddata-pandas-1.9.1.dev1/gooddata_pandas/series.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.9.0/gooddata_pandas/utils.py` & `gooddata-pandas-1.9.1.dev1/gooddata_pandas/utils.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.9.0/gooddata_pandas.egg-info/PKG-INFO` & `gooddata-pandas-1.9.1.dev1/gooddata_pandas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-pandas
-Version: 1.9.0
+Version: 1.9.1.dev1
 Summary: GoodData Cloud to pandas
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.9.0
+Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.9.1.dev1
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,pandas,series,data,frame,data_frame,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,30 +18,30 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: gooddata-sdk~=1.9.0
+Requires-Dist: gooddata-sdk~=1.9.1.dev1
 Requires-Dist: pandas<2.0.0,>=1.0.0
 
 # GoodData Pandas
 
 This package contains a thin layer that utilizes gooddata-sdk and allows you to conveniently create pandas series and
 data frames from the computations done against semantic model in your [GoodData.CN](https://www.gooddata.com/developers/cloud-native/) workspace.
 
 See [DOCUMENTATION](https://gooddata-pandas.readthedocs.io/en/latest/) for more details.
 
 ## Requirements
 
 -  GoodData.CN installation; either running on your cloud
    infrastructure or the free Community Edition running on your workstation
 
--  Python 3.7 or newer
+-  Python 3.8 or newer
 
 ## Installation
 
 Run the following command to install the `gooddata-pandas` package on your system:
 
     pip install gooddata-pandas
```

### Comparing `gooddata-pandas-1.9.0/setup.py` & `gooddata-pandas-1.9.1.dev1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 REQUIRES = [
-    "gooddata-sdk~=1.9.0",
+    "gooddata-sdk~=1.9.1.dev1",
     "pandas>=1.0.0,<2.0.0",
 ]
 
 setup(
     name="gooddata-pandas",
     description="GoodData Cloud to pandas",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.9.0",
+    version="1.9.1.dev1",
     author="GoodData",
     author_email="support@gooddata.com",
     license="MIT",
     license_file="LICENSE.txt",
     license_files=("LICENSE.txt",),
     install_requires=REQUIRES,
     packages=find_packages(exclude=["tests*"]),
     python_requires=">=3.8.0",
     project_urls={
-        "Documentation": "https://gooddata-pandas.readthedocs.io/en/v1.9.0",
+        "Documentation": "https://gooddata-pandas.readthedocs.io/en/v1.9.1.dev1",
         "Source": "https://github.com/gooddata/gooddata-python-sdk",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
```

