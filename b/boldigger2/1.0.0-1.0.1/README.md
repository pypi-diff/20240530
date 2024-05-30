# Comparing `tmp/boldigger2-1.0.0.tar.gz` & `tmp/boldigger2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boldigger2-1.0.0.tar", last modified: Wed May 29 17:23:25 2024, max compression
+gzip compressed data, was "boldigger2-1.0.1.tar", last modified: Wed May 29 18:52:59 2024, max compression
```

## Comparing `boldigger2-1.0.0.tar` & `boldigger2-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 17:23:25.944136 boldigger2-1.0.0/
--rw-rw-rw-   0        0        0     1093 2024-05-29 03:47:00.000000 boldigger2-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0    10616 2024-05-29 17:23:25.943138 boldigger2-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     9684 2024-05-29 17:22:57.000000 boldigger2-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 17:23:25.926192 boldigger2-1.0.0/boldigger2/
--rw-rw-rw-   0        0        0        0 2024-05-29 03:44:28.000000 boldigger2-1.0.0/boldigger2/__init__.py
--rw-rw-rw-   0        0        0     1602 2024-05-21 05:50:28.000000 boldigger2-1.0.0/boldigger2/__main__.py
--rw-rw-rw-   0        0        0    12036 2024-05-29 03:46:11.000000 boldigger2-1.0.0/boldigger2/additional_data_download.py
--rw-rw-rw-   0        0        0    10838 2024-05-29 03:51:42.000000 boldigger2-1.0.0/boldigger2/digger_hit.py
--rw-rw-rw-   0        0        0    21740 2024-05-29 03:46:11.000000 boldigger2-1.0.0/boldigger2/id_engine_coi.py
--rw-rw-rw-   0        0        0     2516 2024-05-29 03:46:11.000000 boldigger2-1.0.0/boldigger2/login.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:23:25.942140 boldigger2-1.0.0/boldigger2.egg-info/
--rw-rw-rw-   0        0        0    10616 2024-05-29 17:23:25.000000 boldigger2-1.0.0/boldigger2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2024-05-29 17:23:25.000000 boldigger2-1.0.0/boldigger2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 17:23:25.000000 boldigger2-1.0.0/boldigger2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-29 17:23:25.000000 boldigger2-1.0.0/boldigger2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      203 2024-05-29 17:23:25.000000 boldigger2-1.0.0/boldigger2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-29 17:23:25.000000 boldigger2-1.0.0/boldigger2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2024-05-29 03:59:19.000000 boldigger2-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-29 17:23:25.944136 boldigger2-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1292 2024-05-29 04:04:05.000000 boldigger2-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:52:59.149010 boldigger2-1.0.1/
+-rw-rw-rw-   0        0        0     1093 2024-05-29 03:47:00.000000 boldigger2-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    10833 2024-05-29 18:52:59.148013 boldigger2-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9928 2024-05-29 18:51:46.000000 boldigger2-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 18:52:59.131070 boldigger2-1.0.1/boldigger2/
+-rw-rw-rw-   0        0        0        0 2024-05-29 03:44:28.000000 boldigger2-1.0.1/boldigger2/__init__.py
+-rw-rw-rw-   0        0        0     1602 2024-05-21 05:50:28.000000 boldigger2-1.0.1/boldigger2/__main__.py
+-rw-rw-rw-   0        0        0    12036 2024-05-29 03:46:11.000000 boldigger2-1.0.1/boldigger2/additional_data_download.py
+-rw-rw-rw-   0        0        0    10838 2024-05-29 03:51:42.000000 boldigger2-1.0.1/boldigger2/digger_hit.py
+-rw-rw-rw-   0        0        0    21740 2024-05-29 03:46:11.000000 boldigger2-1.0.1/boldigger2/id_engine_coi.py
+-rw-rw-rw-   0        0        0     2516 2024-05-29 03:46:11.000000 boldigger2-1.0.1/boldigger2/login.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:52:59.147017 boldigger2-1.0.1/boldigger2.egg-info/
+-rw-rw-rw-   0        0        0    10833 2024-05-29 18:52:59.000000 boldigger2-1.0.1/boldigger2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2024-05-29 18:52:59.000000 boldigger2-1.0.1/boldigger2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:52:59.000000 boldigger2-1.0.1/boldigger2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-29 18:52:59.000000 boldigger2-1.0.1/boldigger2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      192 2024-05-29 18:52:59.000000 boldigger2-1.0.1/boldigger2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 18:52:59.000000 boldigger2-1.0.1/boldigger2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2024-05-29 03:59:19.000000 boldigger2-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:52:59.149010 boldigger2-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1269 2024-05-29 18:52:50.000000 boldigger2-1.0.1/setup.py
```

### Comparing `boldigger2-1.0.0/LICENSE.txt` & `boldigger2-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `boldigger2-1.0.0/PKG-INFO` & `boldigger2-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: boldigger2
-Version: 1.0.0
+Version: 1.0.1
 Summary: An even better python package to query different databases of boldsystems.org
 Home-page: https://github.com/DominikBuchner/BOLDigger
 Author: Dominik Buchner
 Author-email: dominik.buchner524@googlemail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4>=4.12.3
-Requires-Dist: Bio>=1.7.0
 Requires-Dist: biopython>=1.79
 Requires-Dist: joblib>=1.1.0
 Requires-Dist: more_itertools>=10.2.0
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: Requests>=2.32.2
 Requires-Dist: requests_html>=0.10.0
@@ -52,14 +51,15 @@
 - **Simplified Arguments**: The `identify` function in BOLDigger2 only accepts a single argument: the path to the FASTA file to be identified. It saves all results in the same folder.
 - **Efficient Data Storage**: BOLDigger2 saves the top 100 hits in a separate file, leading to much faster processing times. All outputs will also be saved in .hdf and .parquet format to facilitate subsequent processing for large tables.
 - **Additional Data Fields**: The top hits in BOLDigger2 will contain additional data fields, such as the number of records supporting the selected top hit, the taxonomic level used for the top hit, and all BINS the selected hit belongs to if it is a species-level hit.
 - **Additional flag**: BOLDigger2 exchanged flag 5. If the top hit is represented by multiple BINS flag 5 is used. The API verification module from BOLDigger is no longer needed.
 - **Adjusted Species-Level Threshold**: BOLDigger2 accepts hits with a similarity of >= 97% as species-level records. This decision aligns with the 3% OTU clustering threshold commonly used in DNA metabarcoding.
 - **Increased process safety**: BOLDigger2 can be stopped at any point in the processing and will simply continue where it was stopped. BOLDigger2 will no longer alter the provided FASTA file. BOLDigger2 accepts both common FASTA formats.
 - **Dynamic downloads**: BOLDigger2 will automatically adjust the number of sequences per query to the BOLD database. If the connection times out the query size will be reduced, if the request is successful, the query size will be increased.
+- **Improved error handling**: Broken records in the BOLD database are now detected and directly reported as a "BrokenRecord" in addition to "NoMatches". If the BOLD website is not accessible, BOLDigger2 will simply wait until it is up again.
 
 ## Installation and Usage
 
 BOLDigger2 requires Python version 3.9 or higher and can be easily installed using pip in any command line:
 
 `pip install boldigger2`
```

### Comparing `boldigger2-1.0.0/README.md` & `boldigger2-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 - **Simplified Arguments**: The `identify` function in BOLDigger2 only accepts a single argument: the path to the FASTA file to be identified. It saves all results in the same folder.
 - **Efficient Data Storage**: BOLDigger2 saves the top 100 hits in a separate file, leading to much faster processing times. All outputs will also be saved in .hdf and .parquet format to facilitate subsequent processing for large tables.
 - **Additional Data Fields**: The top hits in BOLDigger2 will contain additional data fields, such as the number of records supporting the selected top hit, the taxonomic level used for the top hit, and all BINS the selected hit belongs to if it is a species-level hit.
 - **Additional flag**: BOLDigger2 exchanged flag 5. If the top hit is represented by multiple BINS flag 5 is used. The API verification module from BOLDigger is no longer needed.
 - **Adjusted Species-Level Threshold**: BOLDigger2 accepts hits with a similarity of >= 97% as species-level records. This decision aligns with the 3% OTU clustering threshold commonly used in DNA metabarcoding.
 - **Increased process safety**: BOLDigger2 can be stopped at any point in the processing and will simply continue where it was stopped. BOLDigger2 will no longer alter the provided FASTA file. BOLDigger2 accepts both common FASTA formats.
 - **Dynamic downloads**: BOLDigger2 will automatically adjust the number of sequences per query to the BOLD database. If the connection times out the query size will be reduced, if the request is successful, the query size will be increased.
+- **Improved error handling**: Broken records in the BOLD database are now detected and directly reported as a "BrokenRecord" in addition to "NoMatches". If the BOLD website is not accessible, BOLDigger2 will simply wait until it is up again.
 
 ## Installation and Usage
 
 BOLDigger2 requires Python version 3.9 or higher and can be easily installed using pip in any command line:
 
 `pip install boldigger2`
```

### Comparing `boldigger2-1.0.0/boldigger2/__main__.py` & `boldigger2-1.0.1/boldigger2/__main__.py`

 * *Files identical despite different names*

### Comparing `boldigger2-1.0.0/boldigger2/additional_data_download.py` & `boldigger2-1.0.1/boldigger2/additional_data_download.py`

 * *Files identical despite different names*

### Comparing `boldigger2-1.0.0/boldigger2/digger_hit.py` & `boldigger2-1.0.1/boldigger2/digger_hit.py`

 * *Files identical despite different names*

### Comparing `boldigger2-1.0.0/boldigger2/id_engine_coi.py` & `boldigger2-1.0.1/boldigger2/id_engine_coi.py`

 * *Files identical despite different names*

### Comparing `boldigger2-1.0.0/boldigger2/login.py` & `boldigger2-1.0.1/boldigger2/login.py`

 * *Files identical despite different names*

### Comparing `boldigger2-1.0.0/boldigger2.egg-info/PKG-INFO` & `boldigger2-1.0.1/boldigger2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: boldigger2
-Version: 1.0.0
+Version: 1.0.1
 Summary: An even better python package to query different databases of boldsystems.org
 Home-page: https://github.com/DominikBuchner/BOLDigger
 Author: Dominik Buchner
 Author-email: dominik.buchner524@googlemail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4>=4.12.3
-Requires-Dist: Bio>=1.7.0
 Requires-Dist: biopython>=1.79
 Requires-Dist: joblib>=1.1.0
 Requires-Dist: more_itertools>=10.2.0
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: Requests>=2.32.2
 Requires-Dist: requests_html>=0.10.0
@@ -52,14 +51,15 @@
 - **Simplified Arguments**: The `identify` function in BOLDigger2 only accepts a single argument: the path to the FASTA file to be identified. It saves all results in the same folder.
 - **Efficient Data Storage**: BOLDigger2 saves the top 100 hits in a separate file, leading to much faster processing times. All outputs will also be saved in .hdf and .parquet format to facilitate subsequent processing for large tables.
 - **Additional Data Fields**: The top hits in BOLDigger2 will contain additional data fields, such as the number of records supporting the selected top hit, the taxonomic level used for the top hit, and all BINS the selected hit belongs to if it is a species-level hit.
 - **Additional flag**: BOLDigger2 exchanged flag 5. If the top hit is represented by multiple BINS flag 5 is used. The API verification module from BOLDigger is no longer needed.
 - **Adjusted Species-Level Threshold**: BOLDigger2 accepts hits with a similarity of >= 97% as species-level records. This decision aligns with the 3% OTU clustering threshold commonly used in DNA metabarcoding.
 - **Increased process safety**: BOLDigger2 can be stopped at any point in the processing and will simply continue where it was stopped. BOLDigger2 will no longer alter the provided FASTA file. BOLDigger2 accepts both common FASTA formats.
 - **Dynamic downloads**: BOLDigger2 will automatically adjust the number of sequences per query to the BOLD database. If the connection times out the query size will be reduced, if the request is successful, the query size will be increased.
+- **Improved error handling**: Broken records in the BOLD database are now detected and directly reported as a "BrokenRecord" in addition to "NoMatches". If the BOLD website is not accessible, BOLDigger2 will simply wait until it is up again.
 
 ## Installation and Usage
 
 BOLDigger2 requires Python version 3.9 or higher and can be easily installed using pip in any command line:
 
 `pip install boldigger2`
```

### Comparing `boldigger2-1.0.0/setup.py` & `boldigger2-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="boldigger2",
-    version="1.0.0",
+    version="1.0.1",
     author="Dominik Buchner",
     author_email="dominik.buchner524@googlemail.com",
     description="An even better python package to query different databases of boldsystems.org",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DominikBuchner/BOLDigger",
     packages=setuptools.find_packages(),
     license="MIT",
     install_requires=[
         "beautifulsoup4>=4.12.3",
-        "Bio>=1.7.0",
         "biopython>=1.79",
         "joblib>=1.1.0",
         "more_itertools>=10.2.0",
         "numpy>=1.26.4",
         "pandas>=2.2.2",
         "Requests>=2.32.2",
         "requests_html>=0.10.0",
```

