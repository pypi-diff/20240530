# Comparing `tmp/gooddata-dbt-1.9.0.tar.gz` & `tmp/gooddata-dbt-1.9.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gooddata-dbt-1.9.0.tar", last modified: Thu Nov 16 13:25:00 2023, max compression
+gzip compressed data, was "gooddata-dbt-1.9.1.dev1.tar", last modified: Thu Dec 14 13:21:12 2023, max compression
```

## Comparing `gooddata-dbt-1.9.0.tar` & `gooddata-dbt-1.9.1.dev1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:25:00.421404 gooddata-dbt-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    54841 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2023-11-16 13:25:00.421404 gooddata-dbt-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:25:00.417404 gooddata-dbt-1.9.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      261 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/bin/gooddata-dbt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:25:00.417404 gooddata-dbt-1.9.0/gooddata_dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:25:00.421404 gooddata-dbt-1.9.0/gooddata_dbt/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/dbt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13038 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/dbt/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/dbt/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/dbt/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6479 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/dbt/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    19839 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/dbt/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)    17438 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/dbt_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:25:00.421404 gooddata-dbt-1.9.0/gooddata_dbt/gooddata/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/gooddata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/gooddata/api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/gooddata/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/sdk_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/gooddata_dbt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:25:00.417404 gooddata-dbt-1.9.0/gooddata_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2023-11-16 13:25:00.000000 gooddata-dbt-1.9.0/gooddata_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-11-16 13:25:00.000000 gooddata-dbt-1.9.0/gooddata_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 13:25:00.000000 gooddata-dbt-1.9.0/gooddata_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-11-16 13:25:00.000000 gooddata-dbt-1.9.0/gooddata_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-16 13:25:00.000000 gooddata-dbt-1.9.0/gooddata_dbt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 13:25:00.421404 gooddata-dbt-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:25:00.421404 gooddata-dbt-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-11-16 13:24:42.000000 gooddata-dbt-1.9.0/tests/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:12.674155 gooddata-dbt-1.9.1.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    54841 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2023-12-14 13:21:12.674155 gooddata-dbt-1.9.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:12.670155 gooddata-dbt-1.9.1.dev1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/bin/gooddata-dbt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:12.674155 gooddata-dbt-1.9.1.dev1/gooddata_dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:12.674155 gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13038 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19839 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17438 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:12.674155 gooddata-dbt-1.9.1.dev1/gooddata_dbt/gooddata/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/gooddata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/gooddata/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/gooddata/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/sdk_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:12.674155 gooddata-dbt-1.9.1.dev1/gooddata_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2023-12-14 13:21:12.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2023-12-14 13:21:12.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 13:21:12.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-14 13:21:12.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-14 13:21:12.000000 gooddata-dbt-1.9.1.dev1/gooddata_dbt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 13:21:12.674155 gooddata-dbt-1.9.1.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2023-12-14 13:21:05.000000 gooddata-dbt-1.9.1.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:12.674155 gooddata-dbt-1.9.1.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-12-14 13:20:50.000000 gooddata-dbt-1.9.1.dev1/tests/test_tables.py
```

### Comparing `gooddata-dbt-1.9.0/LICENSE.txt` & `gooddata-dbt-1.9.1.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/PKG-INFO` & `gooddata-dbt-1.9.1.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gooddata-dbt
-Version: 1.9.0
+Version: 1.9.1.dev1
 Summary: dbt plugin for GoodData
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -15,18 +15,18 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: gooddata-sdk~=1.9.0
+Requires-Dist: gooddata-sdk~=1.9.1.dev1
 Requires-Dist: pyyaml>=5.1
-Requires-Dist: attrs==21.4.0
-Requires-Dist: cattrs==22.1.0
+Requires-Dist: attrs<=23.1.0,>=21.4.0
+Requires-Dist: cattrs<=23.2.3,>=22.1.0
 Requires-Dist: requests~=2.31.0
 Requires-Dist: tabulate~=0.8.10
 
 # gooddata-dbt
 GoodData plugin for dbt. Reads dbt models and profiles, generates GoodData semantic model.
 
 ## Install
```

#### html2text {}

```diff
@@ -1,52 +1,52 @@
-Metadata-Version: 2.1 Name: gooddata-dbt Version: 1.9.0 Summary: dbt plugin for
-GoodData Author: GoodData Author-email: support@gooddata.com License: MIT
-Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Database Classifier: Topic ::
-Scientific/Engineering Classifier: Topic :: Software Development Classifier:
-Typing :: Typed Requires-Python: >=3.8.0 Description-Content-Type: text/
-markdown License-File: LICENSE.txt Requires-Dist: gooddata-sdk~=1.9.0 Requires-
-Dist: pyyaml>=5.1 Requires-Dist: attrs==21.4.0 Requires-Dist: cattrs==22.1.0
-Requires-Dist: requests~=2.31.0 Requires-Dist: tabulate~=0.8.10 # gooddata-dbt
-GoodData plugin for dbt. Reads dbt models and profiles, generates GoodData
-semantic model. ## Install ```shell pip install gooddata-dbt # Or add the
-corresponding line to requirements.txt # Or install specific version pip
-install gooddata-dbt==1.0.0 ``` ## Configuration, parametrization Create
-`gooddata.yaml` file to configure so-called data products and environments.
-Check [gooddata_example.yml](gooddata_example.yml) file for more details.
-Parametrization of each execution can be done using environment variables /
-tool arguments. Use main --help and --help for each use case to learn more.
-Alternatively, you can configure everything with environment variables. You can
-directly set env variables in a shell session, or store them to .env file(s).
-We provide the following example: - [.env.dev](.env.dev) - [.env.custom.dev]
-(.env.custom.dev) is loaded from the above file and contains sensitive
-variables. Add `.env.custom.*` to .gitignore! Then load .env files: ```bash
-source .env.local ``` ## Use cases ```shell gooddata-dbt --help ``` The plugin
-provides the following use cases: - provision_workspaces - Provisions
-workspaces to GoodData based on gooddata.yaml file - register_data_sources -
-Registers data source in GoodData for each relevant dbt profile - deploy_ldm -
-Reads dbt models and profiles - Scans data source (connection props from dbt
-profiles) through GoodData to get column data types (optional in dbt) -
-Generates GoodData LDM(Logical Data Model) from dbt models. Can utilize custom
-gooddata-specific metadata, more below - upload_notification - Invalidates
-caches for data source - deploy_analytics - Reads content of `gooddata_layout`
-folder and deploys analytics model to GoodData - store_analytics - Reads
-analytics model from GoodData instance and stores it to disk to
-`gooddata_layout` folder - test_insights - Lists all insights(reports) from
-GoodData instance, and executes each report to validate it ## Custom metadata
-in dbt models (optional) If you want to generate optimal LDM from dbt models,
-sometimes you need to specify semantic metadata in dbt models. In general, all
-GoodData metadata must be put to dbt models under `meta` key, except
-descriptions. ### Titles, descriptions dbt supports only `description` field.
-For now, gooddata-dbt generates GoodData title/description from dbt
-description. Can be specified for both tables and columns. ### Model ID Per
-table, you can specify `model_id`. When deploying models/analytics, you can
-include any subset of model_ids. ```yaml models: - name: xxx meta: gooddata:
-model_id: my_id ``` ### GoodData entities By default, gooddata-dbt generates
-GoodData entities based on the following rules: - data type = NUMERIC (decimal
-number) - fact - data_type = DATE/TIMESTAMP/TIMESTAMPTZ - date dimension -
-other data types = attributes To override the default, specify custom GoodData
-meta this way: ```yaml columns: - name: xxxx meta: gooddata: ldm_type: fact/
-attribute/label/date/reference/primary_key referenced_table:
+Metadata-Version: 2.1 Name: gooddata-dbt Version: 1.9.1.dev1 Summary: dbt
+plugin for GoodData Author: GoodData Author-email: support@gooddata.com
+License: MIT Classifier: Development Status :: 4 - Beta Classifier: Environment
+:: Console Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Database
+Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Software
+Development Classifier: Typing :: Typed Requires-Python: >=3.8.0 Description-
+Content-Type: text/markdown License-File: LICENSE.txt Requires-Dist: gooddata-
+sdk~=1.9.1.dev1 Requires-Dist: pyyaml>=5.1 Requires-Dist:
+attrs<=23.1.0,>=21.4.0 Requires-Dist: cattrs<=23.2.3,>=22.1.0 Requires-Dist:
+requests~=2.31.0 Requires-Dist: tabulate~=0.8.10 # gooddata-dbt GoodData plugin
+for dbt. Reads dbt models and profiles, generates GoodData semantic model. ##
+Install ```shell pip install gooddata-dbt # Or add the corresponding line to
+requirements.txt # Or install specific version pip install gooddata-dbt==1.0.0
+``` ## Configuration, parametrization Create `gooddata.yaml` file to configure
+so-called data products and environments. Check [gooddata_example.yml]
+(gooddata_example.yml) file for more details. Parametrization of each execution
+can be done using environment variables / tool arguments. Use main --help and -
+-help for each use case to learn more. Alternatively, you can configure
+everything with environment variables. You can directly set env variables in a
+shell session, or store them to .env file(s). We provide the following example:
+- [.env.dev](.env.dev) - [.env.custom.dev](.env.custom.dev) is loaded from the
+above file and contains sensitive variables. Add `.env.custom.*` to .gitignore!
+Then load .env files: ```bash source .env.local ``` ## Use cases ```shell
+gooddata-dbt --help ``` The plugin provides the following use cases: -
+provision_workspaces - Provisions workspaces to GoodData based on gooddata.yaml
+file - register_data_sources - Registers data source in GoodData for each
+relevant dbt profile - deploy_ldm - Reads dbt models and profiles - Scans data
+source (connection props from dbt profiles) through GoodData to get column data
+types (optional in dbt) - Generates GoodData LDM(Logical Data Model) from dbt
+models. Can utilize custom gooddata-specific metadata, more below -
+upload_notification - Invalidates caches for data source - deploy_analytics -
+Reads content of `gooddata_layout` folder and deploys analytics model to
+GoodData - store_analytics - Reads analytics model from GoodData instance and
+stores it to disk to `gooddata_layout` folder - test_insights - Lists all
+insights(reports) from GoodData instance, and executes each report to validate
+it ## Custom metadata in dbt models (optional) If you want to generate optimal
+LDM from dbt models, sometimes you need to specify semantic metadata in dbt
+models. In general, all GoodData metadata must be put to dbt models under
+`meta` key, except descriptions. ### Titles, descriptions dbt supports only
+`description` field. For now, gooddata-dbt generates GoodData title/description
+from dbt description. Can be specified for both tables and columns. ### Model
+ID Per table, you can specify `model_id`. When deploying models/analytics, you
+can include any subset of model_ids. ```yaml models: - name: xxx meta:
+gooddata: model_id: my_id ``` ### GoodData entities By default, gooddata-dbt
+generates GoodData entities based on the following rules: - data type = NUMERIC
+(decimal number) - fact - data_type = DATE/TIMESTAMP/TIMESTAMPTZ - date
+dimension - other data types = attributes To override the default, specify
+custom GoodData meta this way: ```yaml columns: - name: xxxx meta: gooddata:
+ldm_type: fact/attribute/label/date/reference/primary_key referenced_table:
```

### Comparing `gooddata-dbt-1.9.0/README.md` & `gooddata-dbt-1.9.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/gooddata_dbt/args.py` & `gooddata-dbt-1.9.1.dev1/gooddata_dbt/args.py`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/gooddata_dbt/dbt/base.py` & `gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt/base.py`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/gooddata_dbt/dbt/cloud.py` & `gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt/cloud.py`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/gooddata_dbt/dbt/environment.py` & `gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt/environment.py`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/gooddata_dbt/dbt/metrics.py` & `gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt/metrics.py`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/gooddata_dbt/dbt/profiles.py` & `gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt/profiles.py`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/gooddata_dbt/dbt/tables.py` & `gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt/tables.py`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/gooddata_dbt/dbt_plugin.py` & `gooddata-dbt-1.9.1.dev1/gooddata_dbt/dbt_plugin.py`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/gooddata_dbt/gooddata/api_wrapper.py` & `gooddata-dbt-1.9.1.dev1/gooddata_dbt/gooddata/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/gooddata_dbt/gooddata/config.py` & `gooddata-dbt-1.9.1.dev1/gooddata_dbt/gooddata/config.py`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/gooddata_dbt/sdk_wrapper.py` & `gooddata-dbt-1.9.1.dev1/gooddata_dbt/sdk_wrapper.py`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/gooddata_dbt/utils.py` & `gooddata-dbt-1.9.1.dev1/gooddata_dbt/utils.py`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/gooddata_dbt.egg-info/PKG-INFO` & `gooddata-dbt-1.9.1.dev1/gooddata_dbt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gooddata-dbt
-Version: 1.9.0
+Version: 1.9.1.dev1
 Summary: dbt plugin for GoodData
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -15,18 +15,18 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: gooddata-sdk~=1.9.0
+Requires-Dist: gooddata-sdk~=1.9.1.dev1
 Requires-Dist: pyyaml>=5.1
-Requires-Dist: attrs==21.4.0
-Requires-Dist: cattrs==22.1.0
+Requires-Dist: attrs<=23.1.0,>=21.4.0
+Requires-Dist: cattrs<=23.2.3,>=22.1.0
 Requires-Dist: requests~=2.31.0
 Requires-Dist: tabulate~=0.8.10
 
 # gooddata-dbt
 GoodData plugin for dbt. Reads dbt models and profiles, generates GoodData semantic model.
 
 ## Install
```

#### html2text {}

```diff
@@ -1,52 +1,52 @@
-Metadata-Version: 2.1 Name: gooddata-dbt Version: 1.9.0 Summary: dbt plugin for
-GoodData Author: GoodData Author-email: support@gooddata.com License: MIT
-Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Database Classifier: Topic ::
-Scientific/Engineering Classifier: Topic :: Software Development Classifier:
-Typing :: Typed Requires-Python: >=3.8.0 Description-Content-Type: text/
-markdown License-File: LICENSE.txt Requires-Dist: gooddata-sdk~=1.9.0 Requires-
-Dist: pyyaml>=5.1 Requires-Dist: attrs==21.4.0 Requires-Dist: cattrs==22.1.0
-Requires-Dist: requests~=2.31.0 Requires-Dist: tabulate~=0.8.10 # gooddata-dbt
-GoodData plugin for dbt. Reads dbt models and profiles, generates GoodData
-semantic model. ## Install ```shell pip install gooddata-dbt # Or add the
-corresponding line to requirements.txt # Or install specific version pip
-install gooddata-dbt==1.0.0 ``` ## Configuration, parametrization Create
-`gooddata.yaml` file to configure so-called data products and environments.
-Check [gooddata_example.yml](gooddata_example.yml) file for more details.
-Parametrization of each execution can be done using environment variables /
-tool arguments. Use main --help and --help for each use case to learn more.
-Alternatively, you can configure everything with environment variables. You can
-directly set env variables in a shell session, or store them to .env file(s).
-We provide the following example: - [.env.dev](.env.dev) - [.env.custom.dev]
-(.env.custom.dev) is loaded from the above file and contains sensitive
-variables. Add `.env.custom.*` to .gitignore! Then load .env files: ```bash
-source .env.local ``` ## Use cases ```shell gooddata-dbt --help ``` The plugin
-provides the following use cases: - provision_workspaces - Provisions
-workspaces to GoodData based on gooddata.yaml file - register_data_sources -
-Registers data source in GoodData for each relevant dbt profile - deploy_ldm -
-Reads dbt models and profiles - Scans data source (connection props from dbt
-profiles) through GoodData to get column data types (optional in dbt) -
-Generates GoodData LDM(Logical Data Model) from dbt models. Can utilize custom
-gooddata-specific metadata, more below - upload_notification - Invalidates
-caches for data source - deploy_analytics - Reads content of `gooddata_layout`
-folder and deploys analytics model to GoodData - store_analytics - Reads
-analytics model from GoodData instance and stores it to disk to
-`gooddata_layout` folder - test_insights - Lists all insights(reports) from
-GoodData instance, and executes each report to validate it ## Custom metadata
-in dbt models (optional) If you want to generate optimal LDM from dbt models,
-sometimes you need to specify semantic metadata in dbt models. In general, all
-GoodData metadata must be put to dbt models under `meta` key, except
-descriptions. ### Titles, descriptions dbt supports only `description` field.
-For now, gooddata-dbt generates GoodData title/description from dbt
-description. Can be specified for both tables and columns. ### Model ID Per
-table, you can specify `model_id`. When deploying models/analytics, you can
-include any subset of model_ids. ```yaml models: - name: xxx meta: gooddata:
-model_id: my_id ``` ### GoodData entities By default, gooddata-dbt generates
-GoodData entities based on the following rules: - data type = NUMERIC (decimal
-number) - fact - data_type = DATE/TIMESTAMP/TIMESTAMPTZ - date dimension -
-other data types = attributes To override the default, specify custom GoodData
-meta this way: ```yaml columns: - name: xxxx meta: gooddata: ldm_type: fact/
-attribute/label/date/reference/primary_key referenced_table:
+Metadata-Version: 2.1 Name: gooddata-dbt Version: 1.9.1.dev1 Summary: dbt
+plugin for GoodData Author: GoodData Author-email: support@gooddata.com
+License: MIT Classifier: Development Status :: 4 - Beta Classifier: Environment
+:: Console Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Database
+Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Software
+Development Classifier: Typing :: Typed Requires-Python: >=3.8.0 Description-
+Content-Type: text/markdown License-File: LICENSE.txt Requires-Dist: gooddata-
+sdk~=1.9.1.dev1 Requires-Dist: pyyaml>=5.1 Requires-Dist:
+attrs<=23.1.0,>=21.4.0 Requires-Dist: cattrs<=23.2.3,>=22.1.0 Requires-Dist:
+requests~=2.31.0 Requires-Dist: tabulate~=0.8.10 # gooddata-dbt GoodData plugin
+for dbt. Reads dbt models and profiles, generates GoodData semantic model. ##
+Install ```shell pip install gooddata-dbt # Or add the corresponding line to
+requirements.txt # Or install specific version pip install gooddata-dbt==1.0.0
+``` ## Configuration, parametrization Create `gooddata.yaml` file to configure
+so-called data products and environments. Check [gooddata_example.yml]
+(gooddata_example.yml) file for more details. Parametrization of each execution
+can be done using environment variables / tool arguments. Use main --help and -
+-help for each use case to learn more. Alternatively, you can configure
+everything with environment variables. You can directly set env variables in a
+shell session, or store them to .env file(s). We provide the following example:
+- [.env.dev](.env.dev) - [.env.custom.dev](.env.custom.dev) is loaded from the
+above file and contains sensitive variables. Add `.env.custom.*` to .gitignore!
+Then load .env files: ```bash source .env.local ``` ## Use cases ```shell
+gooddata-dbt --help ``` The plugin provides the following use cases: -
+provision_workspaces - Provisions workspaces to GoodData based on gooddata.yaml
+file - register_data_sources - Registers data source in GoodData for each
+relevant dbt profile - deploy_ldm - Reads dbt models and profiles - Scans data
+source (connection props from dbt profiles) through GoodData to get column data
+types (optional in dbt) - Generates GoodData LDM(Logical Data Model) from dbt
+models. Can utilize custom gooddata-specific metadata, more below -
+upload_notification - Invalidates caches for data source - deploy_analytics -
+Reads content of `gooddata_layout` folder and deploys analytics model to
+GoodData - store_analytics - Reads analytics model from GoodData instance and
+stores it to disk to `gooddata_layout` folder - test_insights - Lists all
+insights(reports) from GoodData instance, and executes each report to validate
+it ## Custom metadata in dbt models (optional) If you want to generate optimal
+LDM from dbt models, sometimes you need to specify semantic metadata in dbt
+models. In general, all GoodData metadata must be put to dbt models under
+`meta` key, except descriptions. ### Titles, descriptions dbt supports only
+`description` field. For now, gooddata-dbt generates GoodData title/description
+from dbt description. Can be specified for both tables and columns. ### Model
+ID Per table, you can specify `model_id`. When deploying models/analytics, you
+can include any subset of model_ids. ```yaml models: - name: xxx meta:
+gooddata: model_id: my_id ``` ### GoodData entities By default, gooddata-dbt
+generates GoodData entities based on the following rules: - data type = NUMERIC
+(decimal number) - fact - data_type = DATE/TIMESTAMP/TIMESTAMPTZ - date
+dimension - other data types = attributes To override the default, specify
+custom GoodData meta this way: ```yaml columns: - name: xxxx meta: gooddata:
+ldm_type: fact/attribute/label/date/reference/primary_key referenced_table:
```

### Comparing `gooddata-dbt-1.9.0/gooddata_dbt.egg-info/SOURCES.txt` & `gooddata-dbt-1.9.1.dev1/gooddata_dbt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gooddata-dbt-1.9.0/setup.py` & `gooddata-dbt-1.9.1.dev1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 REQUIRES = [
-    "gooddata-sdk~=1.9.0",
+    "gooddata-sdk~=1.9.1.dev1",
     "pyyaml>=5.1",
-    "attrs==21.4.0",
-    "cattrs==22.1.0",
+    "attrs>=21.4.0,<=23.1.0",
+    "cattrs>=22.1.0,<=23.2.3",
     "requests~=2.31.0",
     "tabulate~=0.8.10",
 ]
 
 setup(
     name="gooddata-dbt",
     description="dbt plugin for GoodData",
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
```

### Comparing `gooddata-dbt-1.9.0/tests/test_tables.py` & `gooddata-dbt-1.9.1.dev1/tests/test_tables.py`

 * *Files identical despite different names*

