# Comparing `tmp/kedro-datasets-3.0.0.tar.gz` & `tmp/kedro_datasets-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-datasets-3.0.0.tar", last modified: Wed Apr 10 14:53:32 2024, max compression
+gzip compressed data, was "kedro_datasets-3.0.1.tar", last modified: Thu May 30 12:11:09 2024, max compression
```

## Comparing `kedro-datasets-3.0.0.tar` & `kedro_datasets-3.0.1.tar`

### file list

```diff
@@ -1,124 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.348596 kedro-datasets-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20534 2024-04-10 14:53:32.348596 kedro-datasets-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.304596 kedro-datasets-3.0.0/kedro_datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.304596 kedro-datasets-3.0.0/kedro_datasets/api/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/api/api_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.304596 kedro-datasets-3.0.0/kedro_datasets/biosequence/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/biosequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/biosequence/biosequence_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.304596 kedro-datasets-3.0.0/kedro_datasets/dask/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/dask/parquet_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.304596 kedro-datasets-3.0.0/kedro_datasets/databricks/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17369 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/databricks/managed_table_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.304596 kedro-datasets-3.0.0/kedro_datasets/email/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/email/message_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/geopandas/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/geopandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/geopandas/geojson_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/holoviews/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/holoviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/holoviews/holoviews_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/huggingface/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/huggingface/hugging_face_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/huggingface/transformer_pipeline_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/ibis/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/ibis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/ibis/table_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/json/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/json/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/matlab/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/matlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/matlab/matlab_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/matplotlib/matplotlib_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/netcdf/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/netcdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/netcdf/netcdf_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/networkx/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/networkx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/networkx/gml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/networkx/graphml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/networkx/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.312596 kedro-datasets-3.0.0/kedro_datasets/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10244 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/deltatable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/feather_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11823 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/gbq_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/generic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/hdf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/parquet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    22978 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/sql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/xml_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.312596 kedro-datasets-3.0.0/kedro_datasets/partitions/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/partitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10453 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/partitions/incremental_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14010 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/partitions/partitioned_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.312596 kedro-datasets-3.0.0/kedro_datasets/pickle/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pickle/pickle_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.312596 kedro-datasets-3.0.0/kedro_datasets/pillow/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pillow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pillow/image_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/plotly/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/plotly/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/plotly/plotly_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/polars/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/polars/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/polars/eager_polars_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/polars/lazy_polars_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/redis/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/redis/redis_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/snowflake/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8737 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/snowflake/snowpark_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/spark/deltatable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    16981 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/spark/spark_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/spark/spark_hive_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/spark/spark_jdbc_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/spark/spark_streaming_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/svmlight/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/svmlight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/svmlight/svmlight_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/text/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/text/text_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.320596 kedro-datasets-3.0.0/kedro_datasets/tracking/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/tracking/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/tracking/metrics_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.320596 kedro-datasets-3.0.0/kedro_datasets/video/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/video/video_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.320596 kedro-datasets-3.0.0/kedro_datasets/yaml/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/yaml/yaml_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.320596 kedro-datasets-3.0.0/kedro_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20534 2024-04-10 14:53:32.000000 kedro-datasets-3.0.0/kedro_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-10 14:53:32.000000 kedro-datasets-3.0.0/kedro_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:53:32.000000 kedro-datasets-3.0.0/kedro_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-10 14:53:32.000000 kedro-datasets-3.0.0/kedro_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 14:53:32.000000 kedro-datasets-3.0.0/kedro_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:53:32.348596 kedro-datasets-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.355745 kedro_datasets-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22134 2024-05-30 12:11:09.355745 kedro_datasets-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.311745 kedro_datasets-3.0.1/kedro_datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.311745 kedro_datasets-3.0.1/kedro_datasets/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/api/api_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.311745 kedro_datasets-3.0.1/kedro_datasets/biosequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/biosequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/biosequence/biosequence_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.311745 kedro_datasets-3.0.1/kedro_datasets/dask/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/dask/parquet_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.311745 kedro_datasets-3.0.1/kedro_datasets/databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17576 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/databricks/managed_table_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.311745 kedro_datasets-3.0.1/kedro_datasets/email/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/email/message_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.311745 kedro_datasets-3.0.1/kedro_datasets/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/geopandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/geopandas/geojson_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.315745 kedro_datasets-3.0.1/kedro_datasets/holoviews/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/holoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/holoviews/holoviews_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.315745 kedro_datasets-3.0.1/kedro_datasets/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/huggingface/hugging_face_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/huggingface/transformer_pipeline_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.315745 kedro_datasets-3.0.1/kedro_datasets/ibis/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/ibis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/ibis/table_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.315745 kedro_datasets-3.0.1/kedro_datasets/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/json/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.315745 kedro_datasets-3.0.1/kedro_datasets/matlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/matlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/matlab/matlab_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.315745 kedro_datasets-3.0.1/kedro_datasets/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/matplotlib/matplotlib_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.315745 kedro_datasets-3.0.1/kedro_datasets/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/netcdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/netcdf/netcdf_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.315745 kedro_datasets-3.0.1/kedro_datasets/networkx/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/networkx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/networkx/gml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/networkx/graphml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/networkx/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.319745 kedro_datasets-3.0.1/kedro_datasets/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pandas/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pandas/deltatable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pandas/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pandas/feather_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pandas/gbq_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pandas/generic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pandas/hdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pandas/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pandas/parquet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23067 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pandas/sql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pandas/xml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.319745 kedro_datasets-3.0.1/kedro_datasets/partitions/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/partitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/partitions/incremental_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14038 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/partitions/partitioned_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.319745 kedro_datasets-3.0.1/kedro_datasets/pickle/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pickle/pickle_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.319745 kedro_datasets-3.0.1/kedro_datasets/pillow/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pillow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/pillow/image_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.319745 kedro_datasets-3.0.1/kedro_datasets/plotly/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/plotly/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/plotly/plotly_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.323745 kedro_datasets-3.0.1/kedro_datasets/polars/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/polars/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/polars/eager_polars_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/polars/lazy_polars_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.323745 kedro_datasets-3.0.1/kedro_datasets/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/redis/redis_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.323745 kedro_datasets-3.0.1/kedro_datasets/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/snowflake/snowpark_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.323745 kedro_datasets-3.0.1/kedro_datasets/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/spark/deltatable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/spark/spark_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/spark/spark_hive_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/spark/spark_jdbc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/spark/spark_streaming_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.323745 kedro_datasets-3.0.1/kedro_datasets/svmlight/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/svmlight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/svmlight/svmlight_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.323745 kedro_datasets-3.0.1/kedro_datasets/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/tensorflow/tensorflow_model_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.323745 kedro_datasets-3.0.1/kedro_datasets/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/text/text_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.327745 kedro_datasets-3.0.1/kedro_datasets/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/tracking/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/tracking/metrics_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.327745 kedro_datasets-3.0.1/kedro_datasets/video/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/video/video_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.327745 kedro_datasets-3.0.1/kedro_datasets/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets/yaml/yaml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.327745 kedro_datasets-3.0.1/kedro_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22134 2024-05-30 12:11:09.000000 kedro_datasets-3.0.1/kedro_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-30 12:11:09.000000 kedro_datasets-3.0.1/kedro_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 12:11:09.000000 kedro_datasets-3.0.1/kedro_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-30 12:11:09.000000 kedro_datasets-3.0.1/kedro_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 12:11:09.000000 kedro_datasets-3.0.1/kedro_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:09.327745 kedro_datasets-3.0.1/kedro_datasets_experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/kedro_datasets_experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-05-30 12:11:01.000000 kedro_datasets-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 12:11:09.355745 kedro_datasets-3.0.1/setup.cfg
```

### Comparing `kedro-datasets-3.0.0/PKG-INFO` & `kedro_datasets-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-datasets
-Version: 3.0.0
+Version: 3.0.1
 Summary: Kedro-Datasets is where you can find all of Kedro's data connectors.
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: >=3.9
@@ -14,15 +14,15 @@
 Provides-Extra: pandas-base
 Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-base"
 Provides-Extra: spark-base
 Requires-Dist: pyspark<4.0,>=2.2; extra == "spark-base"
 Provides-Extra: hdfs-base
 Requires-Dist: hdfs<3.0,>=2.5.8; extra == "hdfs-base"
 Provides-Extra: s3fs-base
-Requires-Dist: s3fs<2024.1,>=2021.4; extra == "s3fs-base"
+Requires-Dist: s3fs>=2021.04; extra == "s3fs-base"
 Provides-Extra: polars-base
 Requires-Dist: polars>=0.18.0; extra == "polars-base"
 Provides-Extra: plotly-base
 Requires-Dist: plotly<6.0,>=4.8.0; extra == "plotly-base"
 Provides-Extra: delta-base
 Requires-Dist: delta-spark~=1.2.1; extra == "delta-base"
 Provides-Extra: networkx-base
@@ -242,55 +242,51 @@
 Requires-Dist: kedro-datasets[video-videodataset]; extra == "video"
 Provides-Extra: yaml-yamldataset
 Requires-Dist: kedro-datasets[pandas-base]; extra == "yaml-yamldataset"
 Requires-Dist: PyYAML<7.0,>=4.2; extra == "yaml-yamldataset"
 Provides-Extra: yaml
 Requires-Dist: kedro-datasets[yaml-yamldataset]; extra == "yaml"
 Provides-Extra: docs
-Requires-Dist: docutils==0.16; extra == "docs"
-Requires-Dist: sphinx~=5.3.0; extra == "docs"
-Requires-Dist: sphinx_rtd_theme==1.2.0; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints==1.20.2; extra == "docs"
-Requires-Dist: sphinx_copybutton==0.3.1; extra == "docs"
-Requires-Dist: sphinx-notfound-page; extra == "docs"
+Requires-Dist: kedro-sphinx-theme==2024.4.0; extra == "docs"
 Requires-Dist: ipykernel<7.0,>=5.3; extra == "docs"
-Requires-Dist: sphinxcontrib-mermaid~=0.7.1; extra == "docs"
-Requires-Dist: myst-parser~=1.0.0; extra == "docs"
-Requires-Dist: Jinja2<3.1.0; extra == "docs"
+Requires-Dist: Jinja2<3.2.0; extra == "docs"
 Provides-Extra: test
 Requires-Dist: adlfs~=2023.1; extra == "test"
 Requires-Dist: bandit<2.0,>=1.6.2; extra == "test"
 Requires-Dist: behave==1.2.6; extra == "test"
 Requires-Dist: biopython~=1.73; extra == "test"
 Requires-Dist: blacken-docs==1.9.2; extra == "test"
 Requires-Dist: black~=22.0; extra == "test"
 Requires-Dist: cloudpickle<=2.0.0; extra == "test"
 Requires-Dist: compress-pickle[lz4]~=2.1.0; extra == "test"
-Requires-Dist: coverage[toml]; extra == "test"
+Requires-Dist: coverage>=7.2.0; extra == "test"
 Requires-Dist: dask[complete]>=2021.10; extra == "test"
 Requires-Dist: delta-spark<3.0,>=1.0; extra == "test"
 Requires-Dist: deltalake>=0.10.0; extra == "test"
 Requires-Dist: dill~=0.3.1; extra == "test"
 Requires-Dist: filelock<4.0,>=3.4.0; extra == "test"
 Requires-Dist: gcsfs<2023.3,>=2023.1; extra == "test"
 Requires-Dist: geopandas<1.0,>=0.6.0; extra == "test"
 Requires-Dist: hdfs<3.0,>=2.5.8; extra == "test"
 Requires-Dist: holoviews>=1.13.0; extra == "test"
+Requires-Dist: h5netcdf>=1.2.0; extra == "test"
 Requires-Dist: ibis-framework[duckdb,examples]; extra == "test"
 Requires-Dist: import-linter[toml]==1.2.6; extra == "test"
 Requires-Dist: ipython<8.0,>=7.31.1; extra == "test"
 Requires-Dist: Jinja2<3.1.0; extra == "test"
 Requires-Dist: joblib>=0.14; extra == "test"
 Requires-Dist: jupyterlab>=3.0; extra == "test"
 Requires-Dist: jupyter~=1.0; extra == "test"
 Requires-Dist: lxml~=4.6; extra == "test"
 Requires-Dist: matplotlib<3.4,>=3.0.3; python_version < "3.10" and extra == "test"
 Requires-Dist: matplotlib<3.6,>=3.5; python_version >= "3.10" and extra == "test"
 Requires-Dist: memory_profiler<1.0,>=0.50.0; extra == "test"
 Requires-Dist: moto==5.0.0; extra == "test"
+Requires-Dist: mypy~=1.0; extra == "test"
+Requires-Dist: netcdf4>=1.6.4; extra == "test"
 Requires-Dist: networkx~=2.4; extra == "test"
 Requires-Dist: opencv-python~=4.5.5.64; extra == "test"
 Requires-Dist: openpyxl<4.0,>=3.0.3; extra == "test"
 Requires-Dist: pandas-gbq>=0.12.0; extra == "test"
 Requires-Dist: pandas>=2.0; extra == "test"
 Requires-Dist: Pillow~=9.0; extra == "test"
 Requires-Dist: plotly<6.0,>=4.8.0; extra == "test"
@@ -306,16 +302,16 @@
 Requires-Dist: pytest-mock<2.0,>=1.7.1; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=2.2.1; extra == "test"
 Requires-Dist: pytest~=7.2; extra == "test"
 Requires-Dist: redis~=4.1; extra == "test"
 Requires-Dist: requests-mock~=1.6; extra == "test"
 Requires-Dist: requests~=2.20; extra == "test"
 Requires-Dist: ruff~=0.0.290; extra == "test"
-Requires-Dist: s3fs<2024.1,>=2021.04; extra == "test"
-Requires-Dist: snowflake-snowpark-python~=1.0; python_version == "3.9" and extra == "test"
+Requires-Dist: s3fs>=2021.04; extra == "test"
+Requires-Dist: snowflake-snowpark-python~=1.0; python_version < "3.11" and extra == "test"
 Requires-Dist: scikit-learn<2,>=1.0.2; extra == "test"
 Requires-Dist: scipy>=1.7.3; extra == "test"
 Requires-Dist: packaging; extra == "test"
 Requires-Dist: SQLAlchemy>=1.2; extra == "test"
 Requires-Dist: tables>=3.8.0; platform_system == "Windows" and extra == "test"
 Requires-Dist: tables~=3.6; platform_system != "Windows" and extra == "test"
 Requires-Dist: tensorflow-macos~=2.0; (platform_system == "Darwin" and platform_machine == "arm64") and extra == "test"
@@ -323,36 +319,68 @@
 Requires-Dist: triad<1.0,>=0.6.7; extra == "test"
 Requires-Dist: trufflehog~=2.1; extra == "test"
 Requires-Dist: xarray>=2023.1.0; extra == "test"
 Requires-Dist: xlsxwriter~=1.0; extra == "test"
 Requires-Dist: datasets; extra == "test"
 Requires-Dist: huggingface_hub; extra == "test"
 Requires-Dist: transformers[torch]; extra == "test"
+Requires-Dist: types-cachetools; extra == "test"
+Requires-Dist: types-PyYAML; extra == "test"
+Requires-Dist: types-redis; extra == "test"
+Requires-Dist: types-requests; extra == "test"
+Requires-Dist: types-decorator; extra == "test"
+Requires-Dist: types-six; extra == "test"
+Requires-Dist: types-tabulate; extra == "test"
+Provides-Extra: experimental
 Provides-Extra: all
 Requires-Dist: kedro-datasets[docs,test]; extra == "all"
 
 # Kedro-Datasets
 
 <!-- Note that the contents of this file are also used in the documentation, see docs/source/index.md -->
 
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://pypi.org/project/kedro-datasets/)
+[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg)](https://pypi.org/project/kedro-datasets/)
 [![PyPI Version](https://badge.fury.io/py/kedro-datasets.svg)](https://pypi.org/project/kedro-datasets/)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
 
 Welcome to `kedro_datasets`, the home of Kedro's data connectors. Here you will find `AbstractDataset` implementations powering Kedro's DataCatalog created by QuantumBlack and external contributors.
 
 ## Installation
 
 `kedro-datasets` is a Python plugin. To install it:
 
 ```bash
 pip install kedro-datasets
 ```
 
+### Install dependencies at a group-level
+
+Datasets are organised into groups e.g. `pandas`, `spark` and `pickle`. Each group has a collection of datasets, e.g.`pandas.CSVDataset`, `pandas.ParquetDataset` and more. You can install dependencies for an entire group of dependencies as follows:
+
+```bash
+pip install "kedro-datasets[<group>]"
+```
+
+This installs Kedro-Datasets and dependencies related to the dataset group. An example of this could be a workflow that depends on the data types in `pandas`. Run `pip install 'kedro-datasets[pandas]'` to install Kedro-Datasets and the dependencies for the datasets in the [`pandas` group](https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets/kedro_datasets/pandas).
+
+### Install dependencies at a type-level
+
+To limit installation to dependencies specific to a dataset:
+
+```bash
+pip install "kedro-datasets[<group>-<dataset>]"
+```
+
+For example, your workflow might require the `pandas.ExcelDataset`, so to install its dependencies, run `pip install "kedro-datasets[pandas-exceldataset]"`.
+
+```{note}
+From `kedro-datasets` version 3.0.0 onwards, the names of the optional dataset-level dependencies have been normalised to follow [PEP 685](https://peps.python.org/pep-0685/). The '.' character has been replaced with a '-' character and the names are in lowercase. For example, if you had `kedro-datasets[pandas.ExcelDataset]` in your requirements file, it would have to be changed to `kedro-datasets[pandas-exceldataset]`.
+```
+
 ## What `AbstractDataset` implementations are supported?
 
 We support a range of data connectors, including CSV, Excel, Parquet, Feather, HDF5, JSON, Pickle, SQL Tables, SQL Queries, Spark DataFrames and more. We even allow support for working with images.
 
 These data connectors are supported with the APIs of `pandas`, `spark`, `networkx`, `matplotlib`, `yaml` and more.
 
 [The Data Catalog](https://docs.kedro.org/en/stable/data/data_catalog.html) allows you to work with a range of file formats on local file systems, network file systems, cloud object stores, and Hadoop.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/_typing.py` & `kedro_datasets-3.0.1/kedro_datasets/_typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 `_typing.py` defines custom data types for Kedro-viz integration. It uses NewType from the typing module.
 These types are used to facilitate data rendering in the Kedro-viz front-end.
 """
 
 from typing import NewType
 
 TablePreview = NewType("TablePreview", dict)
-ImagePreview = NewType("ImagePreview", bytes)
+ImagePreview = NewType("ImagePreview", str)
 PlotlyPreview = NewType("PlotlyPreview", dict)
-JSONPreview = NewType("JSONPreview", dict)
+JSONPreview = NewType("JSONPreview", str)
 
 
 # experiment tracking datasets types
 MetricsTrackingPreview = NewType("MetricsTrackingPreview", dict)
 JSONTrackingPreview = NewType("JSONTrackingPreview", dict)
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/api/api_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/api/api_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """``APIDataset`` loads the data from HTTP(S) APIs.
 It uses the python requests library: https://requests.readthedocs.io/en/latest/
 """
+from __future__ import annotations
 
 import json as json_  # make pylint happy
 from copy import deepcopy
-from typing import Any, Union
+from typing import Any
 
 import requests
 from kedro.io.core import AbstractDataset, DatasetError
 from requests import Session, sessions
 from requests.auth import AuthBase
 
 
@@ -57,15 +58,15 @@
 
     .. code-block:: pycon
 
         >>> example_table = '{"col1":["val1", "val2"], "col2":["val3", "val4"]}'
         >>>
         >>> dataset = APIDataset(
         ...     method="POST",
-        ...     url="https://httpbin.org/post",
+        ...     url="https://dummyjson.com/products/add",
         ...     save_args={"chunk_size": 1},
         ... )
         >>> dataset.save(example_table)
 
     On initialisation, we can specify all the necessary parameters in the save args
     dictionary. The default HTTP(S) method is POST but PUT is also supported. Two
     important parameters to keep in mind are timeout and chunk_size. `timeout` defines
@@ -89,18 +90,18 @@
     }
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         url: str,
         method: str = "GET",
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        credentials: Union[tuple[str, str], list[str], AuthBase] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        credentials: tuple[str, str] | list[str] | AuthBase | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``APIDataset`` to fetch data from an API endpoint.
 
         Args:
             url: The API URL endpoint.
             method: The method of the request. GET, POST, PUT are the only supported
                 methods
@@ -215,15 +216,15 @@
         except requests.exceptions.HTTPError as exc:
             raise DatasetError("Failed to send data", exc) from exc
 
         except OSError as exc:
             raise DatasetError("Failed to connect to the remote server") from exc
         return response
 
-    def _save(self, data: Any) -> requests.Response:
+    def _save(self, data: Any) -> requests.Response:  # type: ignore[override]
         if self._request_args["method"] in ["PUT", "POST"]:
             if isinstance(data, list):
                 return self._execute_save_with_chunks(json_data=data)
 
             return self._execute_save_request(json_data=data)
 
         raise DatasetError("Use PUT or POST methods for save")
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/biosequence/biosequence_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/biosequence/biosequence_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """BioSequenceDataset loads and saves data to/from bio-sequence objects to
 file.
 """
+from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 from Bio import SeqIO
@@ -44,19 +45,19 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """
         Creates a new instance of ``BioSequenceDataset`` pointing
         to a concrete filepath.
 
         Args:
             filepath: Filepath in POSIX format to sequence file prefixed with a protocol like
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/dask/parquet_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/dask/parquet_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """``ParquetDataset`` is a data set used to load and save data to parquet files using Dask
 dataframe"""
+from __future__ import annotations
 
 from copy import deepcopy
 from typing import Any
 
 import dask.dataframe as dd
 import fsspec
 import triad
@@ -80,19 +81,19 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {"write_index": False}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``ParquetDataset`` pointing to concrete
         parquet files.
 
         Args:
             filepath: Filepath in POSIX format to a parquet file
                 parquet collection or the directory of a multipart parquet.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/databricks/managed_table_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/databricks/managed_table_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """``ManagedTableDataset`` implementation to access managed delta tables
 in Databricks.
 """
+from __future__ import annotations
 
 import logging
 import re
 from dataclasses import dataclass
-from typing import Any, Optional, Union
+from typing import Any
 
 import pandas as pd
 from kedro.io.core import (
     AbstractVersionedDataset,
     DatasetError,
     Version,
     VersionNotFoundError,
@@ -28,22 +29,22 @@
     """Stores the definition of a managed table"""
 
     # regex for tables, catalogs and schemas
     _NAMING_REGEX = r"\b[0-9a-zA-Z_-]{1,}\b"
     _VALID_WRITE_MODES = ["overwrite", "upsert", "append"]
     _VALID_DATAFRAME_TYPES = ["spark", "pandas"]
     database: str
-    catalog: Optional[str]
+    catalog: str | None
     table: str
-    write_mode: Union[str, None]
+    write_mode: str | None
     dataframe_type: str
-    primary_key: Optional[str]
-    owner_group: str
-    partition_columns: Union[str, list[str]]
-    json_schema: StructType
+    primary_key: str | list[str] | None
+    owner_group: str | None
+    partition_columns: str | list[str] | None
+    json_schema: dict[str, Any] | None = None
 
     def __post_init__(self):
         """Run validation methods if declared.
         The validation method can be a simple check
         that raises DatasetError.
         The validation is performed by calling a function named:
             `validate_<field_name>(self, value) -> raises DatasetError`
@@ -116,28 +117,28 @@
         if self.primary_key is None or len(self.primary_key) == 0:
             if self.write_mode == "upsert":
                 raise DatasetError(
                     f"`primary_key` must be provided for"
                     f"`write_mode` {self.write_mode}"
                 )
 
-    def full_table_location(self) -> str:
+    def full_table_location(self) -> str | None:
         """Returns the full table location
 
         Returns:
-            str: table location in the format catalog.database.table
+            str | None : table location in the format catalog.database.table or None if database and table aren't defined
         """
         full_table_location = None
         if self.catalog and self.database and self.table:
             full_table_location = f"`{self.catalog}`.`{self.database}`.`{self.table}`"
         elif self.database and self.table:
             full_table_location = f"`{self.database}`.`{self.table}`"
         return full_table_location
 
-    def schema(self) -> StructType:
+    def schema(self) -> StructType | None:
         """Returns the Spark schema of the table if it exists
 
         Returns:
             StructType:
         """
         schema = None
         try:
@@ -213,25 +214,25 @@
     # using ``ThreadRunner`` instead
     _SINGLE_PROCESS = True
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         table: str,
-        catalog: str = None,
+        catalog: str | None = None,
         database: str = "default",
-        write_mode: Union[str, None] = None,
+        write_mode: str | None = None,
         dataframe_type: str = "spark",
-        primary_key: Optional[Union[str, list[str]]] = None,
-        version: Version = None,
+        primary_key: str | list[str] | None = None,
+        version: Version | None = None,
         # the following parameters are used by project hooks
         # to create or update table properties
-        schema: dict[str, Any] = None,
-        partition_columns: list[str] = None,
-        owner_group: str = None,
+        schema: dict[str, Any] | None = None,
+        partition_columns: list[str] | None = None,
+        owner_group: str | None = None,
     ) -> None:
         """Creates a new instance of ``ManagedTableDataset``.
 
         Args:
             table: the name of the table
             catalog: the name of the catalog in Unity.
                 Defaults to None.
@@ -272,20 +273,20 @@
             partition_columns=partition_columns,
             json_schema=schema,
         )
 
         self._version = version
 
         super().__init__(
-            filepath=None,
+            filepath=None,  # type: ignore[arg-type]
             version=version,
-            exists_function=self._exists,
+            exists_function=self._exists,  # type: ignore[arg-type]
         )
 
-    def _load(self) -> Union[DataFrame, pd.DataFrame]:
+    def _load(self) -> DataFrame | pd.DataFrame:
         """Loads the version of data in the format defined in the init
         (spark|pandas dataframe)
 
         Raises:
             VersionNotFoundError: if the version defined in
             the init doesn't exist
 
@@ -313,30 +314,30 @@
         """Saves the data to the table by appending it
         to the location defined in the init
 
         Args:
             data (DataFrame): the Spark dataframe to append to the table
         """
         data.write.format("delta").mode("append").saveAsTable(
-            self._table.full_table_location()
+            self._table.full_table_location() or ""
         )
 
     def _save_overwrite(self, data: DataFrame) -> None:
         """Overwrites the data in the table with the data provided.
         (this is the default save mode)
 
         Args:
             data (DataFrame): the Spark dataframe to overwrite the table with.
         """
         delta_table = data.write.format("delta")
         if self._table.write_mode == "overwrite":
             delta_table = delta_table.mode("overwrite").option(
                 "overwriteSchema", "true"
             )
-        delta_table.saveAsTable(self._table.full_table_location())
+        delta_table.saveAsTable(self._table.full_table_location() or "")
 
     def _save_upsert(self, update_data: DataFrame) -> None:
         """Upserts the data by joining on primary_key columns or column.
         If table doesn't exist at save, the data is inserted to a new table.
 
         Args:
             update_data (DataFrame): the Spark dataframe to upsert
@@ -369,31 +370,32 @@
             _get_spark().conf.set("whereExpr", where_expr)
             upsert_sql = """MERGE INTO ${fullTableAddress} base USING update ON ${whereExpr}
                 WHEN MATCHED THEN UPDATE SET * WHEN NOT MATCHED THEN INSERT *"""
             _get_spark().sql(upsert_sql)
         else:
             self._save_append(update_data)
 
-    def _save(self, data: Union[DataFrame, pd.DataFrame]) -> None:
+    def _save(self, data: DataFrame | pd.DataFrame) -> None:
         """Saves the data based on the write_mode and dataframe_type in the init.
         If write_mode is pandas, Spark dataframe is created first.
         If schema is provided, data is matched to schema before saving
         (columns will be sorted and truncated).
 
         Args:
             data (Any): Spark or pandas dataframe to save to the table location
         """
         if self._table.write_mode is None:
             raise DatasetError(
                 "'save' can not be used in read-only mode. "
                 "Change 'write_mode' value to `overwrite`, `upsert` or `append`."
             )
         # filter columns specified in schema and match their ordering
-        if self._table.schema():
-            cols = self._table.schema().fieldNames()
+        schema = self._table.schema()
+        if schema:
+            cols = schema.fieldNames()
             if self._table.dataframe_type == "pandas":
                 data = _get_spark().createDataFrame(
                     data.loc[:, cols], schema=self._table.schema()
                 )
             else:
                 data = data.select(*cols)
         elif self._table.dataframe_type == "pandas":
@@ -401,15 +403,15 @@
         if self._table.write_mode == "overwrite":
             self._save_overwrite(data)
         elif self._table.write_mode == "upsert":
             self._save_upsert(data)
         elif self._table.write_mode == "append":
             self._save_append(data)
 
-    def _describe(self) -> dict[str, str]:
+    def _describe(self) -> dict[str, str | list | None]:
         """Returns a description of the instance of ManagedTableDataset
 
         Returns:
             Dict[str, str]: Dict with the details of the dataset
         """
         return {
             "catalog": self._table.catalog,
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/email/message_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/email/message_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``EmailMessageDataset`` loads/saves an email message from/to a file
 using an underlying filesystem (e.g.: local, S3, GCS). It uses the
 ``email`` package in the standard library to manage email messages.
 """
+from __future__ import annotations
 
 from copy import deepcopy
 from email.generator import Generator
 from email.message import Message
 from email.parser import Parser
 from email.policy import default
 from pathlib import PurePosixPath
@@ -55,20 +56,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``EmailMessageDataset`` pointing to a concrete text file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a text file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/geopandas/geojson_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/geopandas/geojson_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """GeoJSONDataset loads and saves data to a local geojson file. The
 underlying functionality is supported by geopandas, so it supports all
 allowed geopandas (pandas) options for loading and saving geosjon files.
 """
+from __future__ import annotations
 
 import copy
 from pathlib import PurePosixPath
 from typing import Any, Union
 
 import fsspec
 import geopandas as gpd
@@ -51,20 +52,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS = {"driver": "GeoJSON"}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``GeoJSONDataset`` pointing to a concrete GeoJSON file
         on a specific filesystem fsspec.
 
         Args:
 
             filepath: Filepath in POSIX format to a GeoJSON file prefixed with a protocol like
@@ -121,15 +122,15 @@
         if save_args is not None:
             self._save_args.update(save_args)
 
         _fs_open_args_save.setdefault("mode", "wb")
         self._fs_open_args_load = _fs_open_args_load
         self._fs_open_args_save = _fs_open_args_save
 
-    def _load(self) -> Union[gpd.GeoDataFrame, dict[str, gpd.GeoDataFrame]]:
+    def _load(self) -> gpd.GeoDataFrame | dict[str, gpd.GeoDataFrame]:
         load_path = get_filepath_str(self._get_load_path(), self._protocol)
         with self._fs.open(load_path, **self._fs_open_args_load) as fs_file:
             return gpd.read_file(fs_file, **self._load_args)
 
     def _save(self, data: gpd.GeoDataFrame) -> None:
         save_path = get_filepath_str(self._get_save_path(), self._protocol)
         with self._fs.open(save_path, **self._fs_open_args_save) as fs_file:
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/holoviews/holoviews_writer.py` & `kedro_datasets-3.0.1/kedro_datasets/holoviews/holoviews_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """``HoloviewsWriter`` saves Holoviews objects as image file(s) to an underlying
 filesystem (e.g. local, S3, GCS)."""
+from __future__ import annotations
 
 import io
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, NoReturn, TypeVar
 
 import fsspec
@@ -40,19 +41,19 @@
 
     DEFAULT_SAVE_ARGS: dict[str, Any] = {"fmt": "png"}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        fs_args: dict[str, Any] = None,
-        credentials: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        metadata: dict[str, Any] = None,
+        fs_args: dict[str, Any] | None = None,
+        credentials: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``HoloviewsWriter``.
 
         Args:
             filepath: Filepath in POSIX format to a text file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
                 The prefix should be any protocol supported by ``fsspec``.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/huggingface/hugging_face_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/huggingface/hugging_face_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     """
 
     def __init__(
         self,
         *,
         dataset_name: str,
-        dataset_kwargs: dict[Any] | None = None,
+        dataset_kwargs: dict[str, Any] | None = None,
     ):
         self.dataset_name = dataset_name
         self._dataset_kwargs = dataset_kwargs or {}
 
     def _load(self):
         return load_dataset(self.dataset_name, **self._dataset_kwargs)
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/huggingface/transformer_pipeline_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/huggingface/transformer_pipeline_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,26 +25,28 @@
          model_name: Twitter/twhin-bert-base
 
     Example usage for the :doc:`Python API <kedro:data/advanced_data_catalog_usage>`:
 
     .. code-block:: pycon
 
        >>> from kedro_datasets.huggingface import HFTransformerPipelineDataset
-       >>> dataset = HFTransformerPipelineDataset(task="text-classification", model_name="prajjwal1/bert-tiny")
+       >>> dataset = HFTransformerPipelineDataset(
+       ...     task="text-classification", model_name="prajjwal1/bert-tiny"
+       ... )
        >>> model = dataset.load()
        >>> assert model("Hello world")[0]["label"].startswith("LABEL_")
 
     """
 
     def __init__(
         self,
         *,
         task: str | None = None,
         model_name: str | None = None,
-        pipeline_kwargs: dict[t.Any] | None = None,
+        pipeline_kwargs: dict[str, t.Any] | None = None,
     ):
         if task is None and model_name is None:
             raise ValueError("At least 'task' or 'model_name' are needed")
         self._task = task if task else None
         self._model_name = model_name
         self._pipeline_kwargs = pipeline_kwargs or {}
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/ibis/table_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/ibis/table_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,16 @@
 
         cls = type(self)
         key = hashable(self._connection_config)
         if key not in cls._connections:
             import ibis
 
             config = deepcopy(self._connection_config)
-            backend = getattr(ibis, config.pop("backend"))
+            backend_attr = config.pop("backend") if config else None
+            backend = getattr(ibis, backend_attr)
             cls._connections[key] = backend.connect(**config)
 
         return cls._connections[key]
 
     def _load(self) -> ir.Table:
         if self._filepath is not None:
             if self._file_format is None:
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/json/json_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/json/json_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``JSONDataset`` loads/saves data from/to a JSON file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses native json to handle the JSON file.
 """
+from __future__ import annotations
 
 import json
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
@@ -55,19 +56,19 @@
 
     DEFAULT_SAVE_ARGS: dict[str, Any] = {"indent": 2}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``JSONDataset`` pointing to a concrete JSON file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a JSON file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
@@ -168,8 +169,8 @@
         Generate a preview of the JSON dataset with a specified number of items.
 
         Returns:
             A string representing the JSON data for previewing.
         """
         data = self._load()
 
-        return json.dumps(data)
+        return JSONPreview(json.dumps(data))
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/matlab/matlab_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/matlab/matlab_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """``MatlabDataset`` loads/saves data from/to a Matlab file using an underlying
 filesystem ?(e.g.: local, S3, GCS)?. The underlying functionality is supported by
 the specified backend library passed in (defaults to the ``matlab`` library), so it
 supports all allowed options for loading and saving matlab files.
 """
+from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 import numpy as np
@@ -53,19 +54,19 @@
     """
 
     DEFAULT_SAVE_ARGS: dict[str, Any] = {"indent": 2}
 
     def __init__(  # noqa = PLR0913
         self,
         filepath: str,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of MatlabDataSet to load and save data from/to a MATLAB file.
 
         Args:
             filepath: Filepath in POSIX format to a Matlab file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
                 The prefix should be any protocol supported by ``fsspec``.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/matplotlib/matplotlib_writer.py` & `kedro_datasets-3.0.1/kedro_datasets/matplotlib/matplotlib_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """``MatplotlibWriter`` saves one or more Matplotlib objects as image
 files to an underlying filesystem (e.g. local, S3, GCS)."""
+from __future__ import annotations
 
 import base64
 import io
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, NoReturn, Union
 from warnings import warn
@@ -13,22 +14,21 @@
 from kedro.io.core import (
     AbstractVersionedDataset,
     DatasetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
+from matplotlib.figure import Figure
 
 from kedro_datasets._typing import ImagePreview
 
 
 class MatplotlibWriter(
-    AbstractVersionedDataset[
-        Union[plt.figure, list[plt.figure], dict[str, plt.figure]], NoReturn
-    ]
+    AbstractVersionedDataset[Union[Figure, list[Figure], dict[str, Figure]], NoReturn]
 ):
     """``MatplotlibWriter`` saves one or more Matplotlib objects as
     image files to an underlying filesystem (e.g. local, S3, GCS).
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog_yaml_examples.html>`_:
@@ -117,20 +117,20 @@
 
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        fs_args: dict[str, Any] = None,
-        credentials: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
+        fs_args: dict[str, Any] | None = None,
+        credentials: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
         overwrite: bool = False,
-        metadata: dict[str, Any] = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``MatplotlibWriter``.
 
         Args:
             filepath: Filepath in POSIX format to save Matplotlib objects to, prefixed with a
                 protocol like `s3://`. If prefix is not provided, `file` protocol (local filesystem)
                 will be used. The prefix should be any protocol supported by ``fsspec``.
@@ -199,17 +199,15 @@
             "save_args": self._save_args,
             "version": self._version,
         }
 
     def _load(self) -> NoReturn:
         raise DatasetError(f"Loading not supported for '{self.__class__.__name__}'")
 
-    def _save(
-        self, data: Union[plt.figure, list[plt.figure], dict[str, plt.figure]]
-    ) -> None:
+    def _save(self, data: Figure | (list[Figure] | dict[str, Figure])) -> None:
         save_path = self._get_save_path()
 
         if isinstance(data, (list, dict)) and self._overwrite and self._exists():
             self._fs.rm(get_filepath_str(save_path, self._protocol), recursive=True)
 
         if isinstance(data, list):
             for index, plot in enumerate(data):
@@ -225,15 +223,15 @@
             full_key_path = get_filepath_str(save_path, self._protocol)
             self._save_to_fs(full_key_path=full_key_path, plot=data)
 
         plt.close("all")
 
         self._invalidate_cache()
 
-    def _save_to_fs(self, full_key_path: str, plot: plt.figure):
+    def _save_to_fs(self, full_key_path: str, plot: Figure):
         bytes_buffer = io.BytesIO()
         plot.savefig(bytes_buffer, **self._save_args)
 
         with self._fs.open(full_key_path, **self._fs_open_args_save) as fs_file:
             fs_file.write(bytes_buffer.getvalue())
 
     def _exists(self) -> bool:
@@ -255,8 +253,8 @@
 
         Returns:
             str: A base64 encoded string representing the matplotlib plot image.
         """
         load_path = get_filepath_str(self._get_load_path(), self._protocol)
         with self._fs.open(load_path, mode="rb") as img_file:
             base64_bytes = base64.b64encode(img_file.read())
-        return base64_bytes.decode("utf-8")
+        return ImagePreview(base64_bytes.decode("utf-8"))
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/netcdf/netcdf_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/netcdf/netcdf_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """NetCDFDataset loads and saves data to a local netcdf (.nc) file."""
 
+from __future__ import annotations
+
 import logging
 from copy import deepcopy
 from glob import glob
 from pathlib import Path, PurePosixPath
 from typing import Any
 
 import fsspec
@@ -51,34 +53,34 @@
 
         >>> from kedro_datasets.netcdf import NetCDFDataset
         >>> import xarray as xr
         >>> ds = xr.DataArray(
         ...     [0, 1, 2], dims=["x"], coords={"x": [0, 1, 2]}, name="data"
         ... ).to_dataset()
         >>> dataset = NetCDFDataset(
-        ...     filepath="path/to/folder",
+        ...     filepath=tmp_path / "data.nc",
         ...     save_args={"mode": "w"},
         ... )
         >>> dataset.save(ds)
         >>> reloaded = dataset.load()
     """
 
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa
         self,
         *,
         filepath: str,
-        temppath: str = None,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        credentials: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        temppath: str | None = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        credentials: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ):
         """Creates a new instance of ``NetCDFDataset`` pointing to a concrete NetCDF
         file on a specific filesystem
 
         Args:
             filepath: Filepath in POSIX format to a NetCDF file prefixed with a
                 protocol like `s3://`. If prefix is not provided, `file` protocol
@@ -136,45 +138,50 @@
         # Determine if multiple NetCDF files are being loaded in.
         self._is_multifile = (
             True if "*" in str(PurePosixPath(self._filepath).stem) else False
         )
 
     def _load(self) -> xr.Dataset:
         load_path = self._filepath
+        multi_load_path = load_path
 
         # If NetCDF(s) are on any type of remote storage, need to sync to local to open.
         # Kerchunk could be implemented here in the future for direct remote reading.
         if self._protocol != "file":
             logger.info("Syncing remote NetCDF file to local storage.")
 
             if self._is_multifile:
-                load_path = sorted(self._fs.glob(load_path))
+                multi_load_path = sorted(self._fs.glob(load_path))  # type: ignore[assignment]
 
             self._fs.get(load_path, f"{self._temppath}/")
-            load_path = f"{self._temppath}/{self._filepath.stem}.nc"
+            load_path = f"{self._temppath}/{str(Path(self._filepath).stem)}.nc"
 
-        if self._is_multifile:
-            data = xr.open_mfdataset(str(load_path), **self._load_args)
+        if self._is_multifile and multi_load_path:
+            data = xr.open_mfdataset(multi_load_path, **self._load_args)
         else:
             data = xr.open_dataset(load_path, **self._load_args)
 
         return data
 
     def _save(self, data: xr.Dataset):
         if self._is_multifile:
             raise DatasetError(
                 "Globbed multifile datasets with '*' in filepath cannot be saved. "
                 + "Create an alternate NetCDFDataset with a single .nc output file."
             )
         else:
-            save_path = self._filepath
-            bytes_buffer = data.to_netcdf(**self._save_args)
-
-            with self._fs.open(save_path, mode="wb") as fs_file:
-                fs_file.write(bytes_buffer)
+            if self._protocol == "file":
+                data.to_netcdf(path=self._filepath, **self._save_args)
+            else:
+                if self._temppath is None:
+                    raise DatasetError("_temppath should have been set in __init__")
+                temp_save_path = self._temppath / PurePosixPath(self._filepath).name
+                data.to_netcdf(path=str(temp_save_path), **self._save_args)
+                # Sync to remote storage
+                self._fs.put_file(str(temp_save_path), self._filepath)
 
             self._invalidate_cache()
 
     def _describe(self) -> dict[str, Any]:
         return dict(
             filepath=self._filepath,
             protocol=self._protocol,
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/networkx/gml_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/networkx/gml_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """NetworkX ``GMLDataset`` loads and saves graphs to a graph modelling language (GML)
 file using an underlying filesystem (e.g.: local, S3, GCS). NetworkX is used to
 create GML data.
 """
+from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 import networkx
@@ -40,20 +41,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``GMLDataset``.
 
         Args:
             filepath: Filepath in POSIX format to the NetworkX GML file.
             load_args: Arguments passed on to ``networkx.read_gml``.
                 See the details in
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/networkx/graphml_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/networkx/graphml_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """NetworkX ``GraphMLDataset`` loads and saves graphs to a GraphML file using an underlying
 filesystem (e.g.: local, S3, GCS). NetworkX is used to create GraphML data.
 """
+from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 import networkx
@@ -39,20 +40,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``GraphMLDataset``.
 
         Args:
             filepath: Filepath in POSIX format to the NetworkX GraphML file.
             load_args: Arguments passed on to ``networkx.read_graphml``.
                 See the details in
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/networkx/json_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/networkx/json_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``JSONDataset`` loads and saves graphs to a JSON file using an underlying
 filesystem (e.g.: local, S3, GCS). NetworkX is used to create JSON data.
 """
+from __future__ import annotations
 
 import json
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
@@ -40,20 +41,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``JSONDataset``.
 
         Args:
             filepath: Filepath in POSIX format to the NetworkX graph JSON file.
             load_args: Arguments passed on to ``networkx.node_link_graph``.
                 See the details in
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/pandas/__init__.py` & `kedro_datasets-3.0.1/kedro_datasets/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-3.0.0/kedro_datasets/pandas/csv_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/pandas/csv_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``CSVDataset`` loads/saves data from/to a CSV file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses pandas to handle the CSV file.
 """
+from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any
 
@@ -71,20 +72,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {"index": False}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``CSVDataset`` pointing to a concrete CSV file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a CSV file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
@@ -205,11 +206,11 @@
             nrows: The number of rows to include in the preview. Defaults to 5.
 
         Returns:
             dict: A dictionary containing the data in a split format.
         """
         # Create a copy so it doesn't contaminate the original dataset
         dataset_copy = self._copy()
-        dataset_copy._load_args["nrows"] = nrows
+        dataset_copy._load_args["nrows"] = nrows  # type: ignore[attr-defined]
         data = dataset_copy.load()
 
         return data.to_dict(orient="split")
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/pandas/deltatable_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/pandas/deltatable_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """``DeltaTableDataset`` loads/saves delta tables from/to a filesystem (e.g.: local,
 S3, GCS), Databricks unity catalog and AWS Glue catalog respectively. It handles
 load and save using a pandas dataframe.
 """
+from __future__ import annotations
 
 from copy import deepcopy
-from typing import Any, Optional
+from typing import Any
 
 import pandas as pd
 from deltalake import DataCatalog, DeltaTable, Metadata
 from deltalake.exceptions import TableNotFoundError
 from deltalake.writer import write_deltalake
 from kedro.io.core import AbstractDataset, DatasetError
 
@@ -83,23 +84,23 @@
 
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {"mode": DEFAULT_WRITE_MODE}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
-        filepath: Optional[str] = None,
-        catalog_type: Optional[DataCatalog] = None,
-        catalog_name: Optional[str] = None,
-        database: Optional[str] = None,
-        table: Optional[str] = None,
-        load_args: Optional[dict[str, Any]] = None,
-        save_args: Optional[dict[str, Any]] = None,
-        credentials: Optional[dict[str, Any]] = None,
-        fs_args: Optional[dict[str, Any]] = None,
+        filepath: str | None = None,
+        catalog_type: DataCatalog | None = None,
+        catalog_name: str | None = None,
+        database: str | None = None,
+        table: str | None = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``DeltaTableDataset``
 
         Args:
             filepath (str): Filepath to a delta lake file with the following accepted protocol:
                 ``S3``: `s3://<bucket>/<path>`, `s3a://<bucket>/<path>`
                 ``Azure``: `az://<container>/<path>`, `adl://<container>/<path>`,
@@ -137,15 +138,15 @@
         self._table = table
         self._fs_args = deepcopy(fs_args) or {}
         self._credentials = deepcopy(credentials) or {}
 
         # DeltaTable cannot be instantiated from an empty directory
         # for the first time creation from filepath, we need to delay the instantiation
         self.is_empty_dir: bool = False
-        self._delta_table: Optional[DeltaTable] = None
+        self._delta_table: DeltaTable | None = None
 
         self._load_args = deepcopy(self.DEFAULT_LOAD_ARGS)
         if load_args:
             self._load_args.update(load_args)
 
         self._save_args = deepcopy(self.DEFAULT_SAVE_ARGS)
         if save_args:
@@ -175,78 +176,78 @@
                     storage_options=self.fs_args,
                     version=self._version,
                 )
             except TableNotFoundError:
                 self.is_empty_dir = True
         else:
             self._delta_table = DeltaTable.from_data_catalog(
-                data_catalog=DataCatalog[self._catalog_type],
+                data_catalog=DataCatalog[self._catalog_type],  # type: ignore[misc]
                 data_catalog_id=self._catalog_name,
-                database_name=self._database,
-                table_name=self._table,
+                database_name=self._database or "",
+                table_name=self._table or "",
             )
 
     @property
     def fs_args(self) -> dict[str, Any]:
         """Appends and returns filesystem credentials to fs_args."""
         fs_args = deepcopy(self._fs_args)
         fs_args.update(self._credentials)
         return fs_args
 
     @property
-    def schema(self) -> dict[str, Any]:
+    def schema(self) -> str:
         """Returns the schema of the DeltaTableDataset as a dictionary."""
-        return self._delta_table.schema().json()
+        return self._delta_table.schema().to_json() if self._delta_table else ""
 
     @property
-    def metadata(self) -> Metadata:
+    def metadata(self) -> Metadata | None:
         """Returns the metadata of the DeltaTableDataset as a dictionary.
         Metadata contains the following:
         1. A unique id
         2. A name, if provided
         3. A description, if provided
         4. The list of partition_columns.
         5. The created_time of the table
         6. A map of table configuration. This includes fields such as delta.appendOnly,
         which if true indicates the table is not meant to have data deleted from it.
 
         Returns: Metadata object containing the above metadata attributes.
         """
-        return self._delta_table.metadata()
+        return self._delta_table.metadata() if self._delta_table else None
 
     @property
-    def history(self) -> list[dict[str, Any]]:
+    def history(self) -> list[dict[str, Any]] | None:
         """Returns the history of actions on DeltaTableDataset as a list of dictionaries."""
-        return self._delta_table.history()
+        return self._delta_table.history() if self._delta_table else None
 
-    def get_loaded_version(self) -> int:
+    def get_loaded_version(self) -> int | None:
         """Returns the version of the DeltaTableDataset that is currently loaded."""
-        return self._delta_table.version()
+        return self._delta_table.version() if self._delta_table else None
 
     def _load(self) -> pd.DataFrame:
-        return self._delta_table.to_pandas()
+        return self._delta_table.to_pandas() if self._delta_table else None
 
     def _save(self, data: pd.DataFrame) -> None:
         if self.is_empty_dir:
             # first time creation of delta table
             write_deltalake(
-                self._filepath,
+                self._filepath or "",
                 data,
                 storage_options=self.fs_args,
                 **self._save_args,
             )
             self.is_empty_dir = False
             self._delta_table = DeltaTable(
-                table_uri=self._filepath,
+                table_uri=self._filepath or "",
                 storage_options=self.fs_args,
                 version=self._version,
             )
         else:
             write_deltalake(
-                self._delta_table,
+                self._delta_table or "",
                 data,
                 storage_options=self.fs_args,
                 **self._save_args,
             )
 
     def _describe(self) -> dict[str, Any]:
         return {
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/pandas/excel_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/pandas/excel_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``ExcelDataset`` loads/saves data from/to a Excel file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses pandas to handle the Excel file.
 """
+from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any, Union
 
@@ -112,20 +113,20 @@
     DEFAULT_SAVE_ARGS = {"index": False}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
         engine: str = "openpyxl",
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``ExcelDataset`` pointing to a concrete Excel file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a Excel file prefixed with a protocol like
                 `s3://`. If prefix is not provided, `file` protocol (local filesystem) will be used.
@@ -212,29 +213,29 @@
             "protocol": self._protocol,
             "load_args": self._load_args,
             "save_args": self._save_args,
             "writer_args": self._writer_args,
             "version": self._version,
         }
 
-    def _load(self) -> Union[pd.DataFrame, dict[str, pd.DataFrame]]:
+    def _load(self) -> pd.DataFrame | dict[str, pd.DataFrame]:
         load_path = str(self._get_load_path())
         if self._protocol == "file":
             # file:// protocol seems to misbehave on Windows
             # (<urlopen error file not on local host>),
             # so we don't join that back to the filepath;
             # storage_options also don't work with local paths
             return pd.read_excel(load_path, **self._load_args)
 
         load_path = f"{self._protocol}{PROTOCOL_DELIMITER}{load_path}"
         return pd.read_excel(
             load_path, storage_options=self._storage_options, **self._load_args
         )
 
-    def _save(self, data: Union[pd.DataFrame, dict[str, pd.DataFrame]]) -> None:
+    def _save(self, data: pd.DataFrame | dict[str, pd.DataFrame]) -> None:
         output = BytesIO()
         save_path = get_filepath_str(self._get_save_path(), self._protocol)
 
         with pd.ExcelWriter(output, **self._writer_args) as writer:
             if isinstance(data, dict):
                 for sheet_name, sheet_data in data.items():
                     sheet_data.to_excel(
@@ -273,11 +274,11 @@
             nrows: The number of rows to include in the preview. Defaults to 5.
 
         Returns:
             dict: A dictionary containing the data in a split format.
         """
         # Create a copy so it doesn't contaminate the original dataset
         dataset_copy = self._copy()
-        dataset_copy._load_args["nrows"] = nrows
+        dataset_copy._load_args["nrows"] = nrows  # type: ignore[attr-defined]
         data = dataset_copy.load()
 
         return data.to_dict(orient="split")
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/pandas/feather_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/pandas/feather_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``FeatherDataset`` is a data set used to load and save data to feather files
 using an underlying filesystem (e.g.: local, S3, GCS). The underlying functionality
 is supported by pandas, so it supports all operations the pandas supports.
 """
+from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any
 
@@ -69,20 +70,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``FeatherDataset`` pointing to a concrete
         filepath.
 
         Args:
             filepath: Filepath in POSIX format to a feather file prefixed with a protocol like
                 `s3://`. If prefix is not provided, `file` protocol (local filesystem) will be used.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/pandas/gbq_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/pandas/gbq_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """``GBQTableDataset`` loads and saves data from/to Google BigQuery. It uses pandas-gbq
 to read and write from/to BigQuery table.
 """
 
+from __future__ import annotations
+
 import copy
 from pathlib import PurePosixPath
-from typing import Any, NoReturn, Union
+from typing import Any, NoReturn
 
 import fsspec
 import pandas as pd
 from google.cloud import bigquery
 from google.cloud.exceptions import NotFound
 from google.oauth2.credentials import Credentials
 from kedro.io.core import (
@@ -66,19 +68,19 @@
     DEFAULT_SAVE_ARGS: dict[str, Any] = {"progress_bar": False}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         dataset: str,
         table_name: str,
-        project: str = None,
-        credentials: Union[dict[str, Any], Credentials] = None,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        project: str | None = None,
+        credentials: dict[str, Any] | Credentials | None = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``GBQTableDataset``.
 
         Args:
             dataset: Google BigQuery dataset.
             table_name: Google BigQuery table name.
             project: Google BigQuery Account project ID.
@@ -208,21 +210,21 @@
         >>> sql_data = dataset.load()
     """
 
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
-        sql: str = None,
-        project: str = None,
-        credentials: Union[dict[str, Any], Credentials] = None,
-        load_args: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        filepath: str = None,
-        metadata: dict[str, Any] = None,
+        sql: str | None = None,
+        project: str | None = None,
+        credentials: dict[str, Any] | Credentials | None = None,
+        load_args: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        filepath: str | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``GBQQueryDataset``.
 
         Args:
             sql: The sql query statement.
             project: Google BigQuery Account project ID.
                 Optional when available from the environment.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/pandas/generic_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/pandas/generic_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``GenericDataset`` loads/saves data from/to a data file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses pandas to handle the
 type of read/write target.
 """
+from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 import pandas as pd
@@ -88,20 +89,20 @@
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
         file_format: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ):
         """Creates a new instance of ``GenericDataset`` pointing to a concrete data file
         on a specific filesystem. The appropriate pandas load/save methods are
         dynamically identified by string matching on a best effort basis.
 
         Args:
             filepath: Filepath in POSIX format to a file prefixed with a protocol like `s3://`.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/pandas/hdf_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/pandas/hdf_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``HDFDataset`` loads/saves data from/to a hdf file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses pandas.HDFStore to handle the hdf file.
 """
+from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import PurePosixPath
 from threading import Lock
 from typing import Any
 
 import fsspec
@@ -61,20 +62,20 @@
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
         key: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``HDFDataset`` pointing to a concrete hdf file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a hdf file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/pandas/json_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/pandas/json_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``JSONDataset`` loads/saves data from/to a JSON file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses pandas to handle the JSON file.
 """
+from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any
 
@@ -66,20 +67,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``JSONDataset`` pointing to a concrete JSON file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a JSON file prefixed with a protocol like `s3://`.
                 If prefix is not provided `file` protocol (local filesystem) will be used.
@@ -200,14 +201,14 @@
             nrows: Number of rows to include in the preview. Defaults to 5.
 
         Returns:
             dict: A dictionary in a split format for preview, if possible.
         """
         # Create a copy, so it doesn't contaminate the original dataset
         dataset_copy = self._copy()
-        dataset_copy._load_args.setdefault("lines", True)
-        dataset_copy._load_args["nrows"] = nrows
+        dataset_copy._load_args.setdefault("lines", True)  # type: ignore[attr-defined]
+        dataset_copy._load_args["nrows"] = nrows  # type: ignore[attr-defined]
         preview_df = dataset_copy._load()
 
         preview_dict = preview_df.to_dict(orient="split")
 
         return preview_dict
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/pandas/parquet_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/pandas/parquet_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``ParquetDataset`` loads/saves data from/to a Parquet file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses pandas to handle the Parquet file.
 """
+from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import Path, PurePosixPath
 from typing import Any
 
@@ -77,20 +78,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``ParquetDataset`` pointing to a concrete Parquet file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a Parquet file prefixed with a protocol like
                 `s3://`. If prefix is not provided, `file` protocol (local filesystem) will be used.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/pandas/sql_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/pandas/sql_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,17 +159,17 @@
     engines: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         table_name: str,
         credentials: dict[str, Any],
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new ``SQLTableDataset``.
 
         Args:
             table_name: The table name to load or save data to. It
                 overwrites name in ``save_args`` and ``table_name``
                 parameters in ``load_args``.
@@ -289,15 +289,15 @@
         """
 
         table_name = self._load_args["table_name"]
 
         metadata = MetaData()
         table_ref = Table(table_name, metadata, autoload_with=self.engine)
 
-        query = select(table_ref).limit(nrows)
+        query = select(table_ref).limit(nrows)  # type: ignore[arg-type]
 
         with self.engine.connect() as conn:
             result = conn.execute(query)
             data_preview = pd.DataFrame(result.fetchall(), columns=result.keys())
 
         preview_data = data_preview.to_dict(orient="split")
         return preview_data
@@ -428,21 +428,21 @@
 
     # using Any because of Sphinx but it should be
     # sqlalchemy.engine.Engine or sqlalchemy.engine.base.Engine
     engines: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
-        sql: str = None,
-        credentials: dict[str, Any] = None,
-        load_args: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        filepath: str = None,
+        sql: str | None = None,
+        credentials: dict[str, Any] | None = None,
+        load_args: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        filepath: str | None = None,
         execution_options: dict[str, Any] | None = None,
-        metadata: dict[str, Any] = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new ``SQLQueryDataset``.
 
         Args:
             sql: The sql query statement.
             credentials: A dictionary with a ``SQLAlchemy`` connection string.
                 Users are supposed to provide the connection string 'con'
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/pandas/xml_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/pandas/xml_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``XMLDataset`` loads/saves data from/to a XML file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses pandas to handle the XML file.
 """
+from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any
 
@@ -47,20 +48,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {"index": False}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``XMLDataset`` pointing to a concrete XML file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a XML file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/partitions/incremental_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/partitions/incremental_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,18 +66,18 @@
         self,
         *,
         path: str,
         dataset: str | type[AbstractDataset] | dict[str, Any],
         checkpoint: str | dict[str, Any] | None = None,
         filepath_arg: str = "filepath",
         filename_suffix: str = "",
-        credentials: dict[str, Any] = None,
-        load_args: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        credentials: dict[str, Any] | None = None,
+        load_args: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``IncrementalDataset``.
 
         Args:
             path: Path to the folder containing partitioned data.
                 If path starts with the protocol (e.g., ``s3://``) then the
                 corresponding ``fsspec`` concrete filesystem implementation will
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/partitions/partitioned_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/partitions/partitioned_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,19 +143,19 @@
     def __init__(  # noqa: PLR0913
         self,
         *,
         path: str,
         dataset: str | type[AbstractDataset] | dict[str, Any],
         filepath_arg: str = "filepath",
         filename_suffix: str = "",
-        credentials: dict[str, Any] = None,
-        load_args: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
+        credentials: dict[str, Any] | None = None,
+        load_args: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
         overwrite: bool = False,
-        metadata: dict[str, Any] = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``PartitionedDataset``.
 
         Args:
             path: Path to the folder containing partitioned data.
                 If path starts with the protocol (e.g., ``s3://``) then the
                 corresponding ``fsspec`` concrete filesystem implementation will
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/pickle/pickle_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/pickle/pickle_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """``PickleDataset`` loads/saves data from/to a Pickle file using an underlying
 filesystem (e.g.: local, S3, GCS). The underlying functionality is supported by
 the specified backend library passed in (defaults to the ``pickle`` library), so it
 supports all allowed options for loading and saving pickle files.
 """
+from __future__ import annotations
 
 import importlib
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
@@ -75,20 +76,20 @@
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
         backend: str = "pickle",
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``PickleDataset`` pointing to a concrete Pickle
         file on a specific filesystem. ``PickleDataset`` supports custom backends to
         serialise/deserialise objects.
 
         Example backends that are compatible (non-exhaustive):
             * `pickle`
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/pillow/image_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/pillow/image_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``ImageDataset`` loads/saves image data as `numpy` from an underlying
 filesystem (e.g.: local, S3, GCS). It uses Pillow to handle image file.
 """
+from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 from kedro.io.core import (
@@ -45,19 +46,19 @@
 
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``ImageDataset`` pointing to a concrete image file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to an image file prefixed with a protocol like
                 `s3://`. If prefix is not provided, `file` protocol (local filesystem) will be used.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/plotly/json_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/plotly/json_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``JSONDataset`` loads/saves a plotly figure from/to a JSON file using an underlying
 filesystem (e.g.: local, S3, GCS).
 """
+from __future__ import annotations
 
 import json
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Union
 
 import fsspec
@@ -57,20 +58,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``JSONDataset`` pointing to a concrete JSON file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a JSON file prefixed with a protocol like `s3://`.
                 If prefix is not provided `file` protocol (local filesystem) will be used.
@@ -139,15 +140,15 @@
             "filepath": self._filepath,
             "protocol": self._protocol,
             "load_args": self._load_args,
             "save_args": self._save_args,
             "version": self._version,
         }
 
-    def _load(self) -> Union[go.Figure, go.FigureWidget]:
+    def _load(self) -> go.Figure | go.FigureWidget:
         load_path = get_filepath_str(self._get_load_path(), self._protocol)
 
         with self._fs.open(load_path, **self._fs_open_args_load) as fs_file:
             # read_json doesn't work correctly with file handler, so we have to read
             # the file, decode it manually and pass to the low-level from_json instead.
             return pio.from_json(str(fs_file.read(), "utf-8"), **self._load_args)
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/plotly/plotly_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/plotly/plotly_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``PlotlyDataset`` generates a plot from a pandas DataFrame and saves it to a JSON
 file using an underlying filesystem (e.g.: local, S3, GCS). It loads the JSON into a
 plotly figure.
 """
+from __future__ import annotations
 
 import json
 from copy import deepcopy
 from typing import Any
 
 import pandas as pd
 import plotly.express as px
@@ -70,20 +71,20 @@
     """
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
         plotly_args: dict[str, Any],
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``PlotlyDataset`` pointing to a concrete JSON file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a JSON file prefixed with a protocol like `s3://`.
                 If prefix is not provided `file` protocol (local filesystem) will be used.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/polars/__init__.py` & `kedro_datasets-3.0.1/kedro_datasets/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-3.0.0/kedro_datasets/polars/csv_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/polars/csv_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``CSVDataset`` loads/saves data from/to a CSV file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses polars to handle the CSV file.
 """
+from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any
 
@@ -67,20 +68,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {"rechunk": True}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``CSVDataset`` pointing to a concrete CSV file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a CSV file prefixed with a protocol
                 `s3://`.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/polars/eager_polars_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/polars/eager_polars_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``EagerPolarsDataset`` loads/saves data from/to a data file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses polars to handle the
 type of read/write target.
 """
+from __future__ import annotations
 
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
@@ -50,27 +51,27 @@
         >>> dataset = EagerPolarsDataset(filepath=tmp_path / "test.parquet", file_format="parquet")
         >>> dataset.save(data)
         >>> reloaded = dataset.load()
         >>> assert data.frame_equal(reloaded)
 
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS = {}  # type: dict[str, Any]
+    DEFAULT_SAVE_ARGS = {}  # type: dict[str, Any]
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
         file_format: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
     ):
         """Creates a new instance of ``EagerPolarsDataset`` pointing to a concrete data file
         on a specific filesystem. The appropriate polars load/save methods are dynamically
         identified by string matching on a best effort basis.
 
         Args:
             filepath: Filepath in POSIX format to a file prefixed with a protocol like
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/polars/lazy_polars_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/polars/lazy_polars_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """``LazyPolarsDataset`` loads/saves data from/to a data file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses polars to handle the
 type of read/write target.
 """
+from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
-from typing import Any, ClassVar, Optional, Union
+from typing import Any, ClassVar, Union
 
 import fsspec
 import polars as pl
 import pyarrow.dataset as ds
 from kedro.io.core import (
     AbstractVersionedDataset,
     DatasetError,
@@ -75,20 +76,20 @@
     DEFAULT_SAVE_ARGS: ClassVar[dict[str, Any]] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
         file_format: str,
-        load_args: Optional[dict[str, Any]] = None,
-        save_args: Optional[dict[str, Any]] = None,
-        version: Version = None,
-        credentials: Optional[dict[str, Any]] = None,
-        fs_args: Optional[dict[str, Any]] = None,
-        metadata: Optional[dict[str, Any]] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``LazyPolarsDataset`` pointing to a concrete
         data file on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a file prefixed with a protocol like
                 `s3://`.
@@ -191,23 +192,23 @@
 
     def _load(self) -> pl.LazyFrame:
         load_path = str(self._get_load_path())
 
         if self._protocol == "file":
             # With local filesystems, we can use Polar's build-in I/O method:
             load_method = getattr(pl, f"scan_{self._file_format}", None)
-            return load_method(load_path, **self._load_args)
+            return load_method(load_path, **self._load_args)  # type: ignore[misc]
 
         # For object storage, we use pyarrow for I/O:
         dataset = ds.dataset(
             load_path, filesystem=self._fs, format=self._file_format, **self._load_args
         )
         return pl.scan_pyarrow_dataset(dataset)
 
-    def _save(self, data: Union[pl.DataFrame, pl.LazyFrame]) -> None:
+    def _save(self, data: pl.DataFrame | pl.LazyFrame) -> None:
         save_path = get_filepath_str(self._get_save_path(), self._protocol)
 
         collected_data = None
         if isinstance(data, pl.LazyFrame):
             collected_data = data.collect()
         else:
             collected_data = data
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/redis/redis_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/redis/redis_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``PickleDataset`` loads/saves data from/to a Redis database. The underlying
 functionality is supported by the redis library, so it supports all allowed
 options for instantiating the redis app ``from_url`` and setting a value."""
+from __future__ import annotations
 
 import importlib
 import os
 from copy import deepcopy
 from typing import Any
 
 import redis
@@ -60,19 +61,19 @@
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         key: str,
         backend: str = "pickle",
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        credentials: dict[str, Any] = None,
-        redis_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        credentials: dict[str, Any] | None = None,
+        redis_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``PickleDataset``. This loads/saves data from/to
         a Redis database while deserialising/serialising. Supports custom backends to
         serialise/deserialise objects.
 
         Example backends that are compatible (non-exhaustive):
             * `pickle`
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/snowflake/snowpark_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/snowflake/snowpark_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """``AbstractDataset`` implementation to access Snowflake using Snowpark dataframes
 """
+from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from typing import Any
 
 import snowflake.snowpark as sp
 from kedro.io.core import AbstractDataset, DatasetError
@@ -101,20 +102,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         table_name: str,
-        schema: str = None,
-        database: str = None,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        credentials: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        schema: str | None = None,
+        database: str | None = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        credentials: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``SnowparkTableDataset``.
 
         Args:
             table_name: The table name to load or save data to.
             schema: Name of the schema where ``table_name`` is.
                 Optional as can be provided as part of ``credentials``
@@ -210,15 +211,15 @@
         return session
 
     @property
     def _session(self) -> sp.Session:
         return self._get_session(self._connection_parameters)
 
     def _load(self) -> sp.DataFrame:
-        table_name = [
+        table_name: list = [
             self._database,
             self._schema,
             self._table_name,
         ]
 
         sp_df = self._session.table(".".join(table_name))
         return sp_df
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/spark/__init__.py` & `kedro_datasets-3.0.1/kedro_datasets/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-3.0.0/kedro_datasets/spark/deltatable_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/spark/deltatable_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``AbstractDataset`` implementation to access DeltaTables using
 ``delta-spark``.
 """
+from __future__ import annotations
 
 from pathlib import PurePosixPath
 from typing import Any, NoReturn
 
 from delta.tables import DeltaTable
 from kedro.io.core import AbstractDataset, DatasetError
 from pyspark.sql.utils import AnalysisException
@@ -63,15 +64,17 @@
 
     # this dataset cannot be used with ``ParallelRunner``,
     # therefore it has the attribute ``_SINGLE_PROCESS = True``
     # for parallelism within a Spark pipeline please consider
     # using ``ThreadRunner`` instead
     _SINGLE_PROCESS = True
 
-    def __init__(self, *, filepath: str, metadata: dict[str, Any] = None) -> None:
+    def __init__(
+        self, *, filepath: str, metadata: dict[str, Any] | None = None
+    ) -> None:
         """Creates a new instance of ``DeltaTableDataset``.
 
         Args:
             filepath: Filepath in POSIX format to a Spark dataframe. When using Databricks
                 and working with data written to mount path points,
                 specify ``filepath``s for (versioned) ``SparkDataset``s
                 starting with ``/dbfs/mnt``.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/spark/spark_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/spark/spark_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,19 +264,19 @@
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
         file_format: str = "parquet",
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``SparkDataset``.
 
         Args:
             filepath: Filepath in POSIX format to a Spark dataframe. When using Databricks
                 specify ``filepath``s starting with ``/dbfs/``.
             file_format: File format used during load and save
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/spark/spark_hive_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/spark/spark_hive_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``AbstractDataset`` implementation to access Spark dataframes using
 ``pyspark`` on Apache Hive.
 """
+from __future__ import annotations
 
 import pickle
 from copy import deepcopy
 from typing import Any
 
 from kedro.io.core import AbstractDataset, DatasetError
 from pyspark.sql import DataFrame, Window
@@ -71,17 +72,17 @@
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         database: str,
         table: str,
         write_mode: str = "errorifexists",
-        table_pk: list[str] = None,
-        save_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        table_pk: list[str] | None = None,
+        save_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``SparkHiveDataset``.
 
         Args:
             database: The name of the hive database.
             table: The name of the table within the database.
             write_mode: ``insert``, ``upsert`` or ``overwrite`` are supported.
@@ -134,15 +135,15 @@
             "table": self._table,
             "write_mode": self._write_mode,
             "table_pk": self._table_pk,
             "partition_by": self._save_args.get("partitionBy"),
             "format": self._format,
         }
 
-    def _create_hive_table(self, data: DataFrame, mode: str = None):
+    def _create_hive_table(self, data: DataFrame, mode: str | None = None):
         _mode: str = mode or self._write_mode
         data.write.saveAsTable(
             self._full_table_address,
             mode=_mode,
             format=self._format,
             **self._save_args,
         )
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/spark/spark_jdbc_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/spark/spark_jdbc_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """SparkJDBCDataset to load and save a PySpark DataFrame via JDBC."""
+from __future__ import annotations
 
 from copy import deepcopy
 from typing import Any
 
 from kedro.io.core import AbstractDataset, DatasetError
 from pyspark.sql import DataFrame
 
@@ -70,18 +71,18 @@
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         url: str,
         table: str,
-        credentials: dict[str, Any] = None,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        credentials: dict[str, Any] | None = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new ``SparkJDBCDataset``.
 
         Args:
             url: A JDBC URL of the form ``jdbc:subprotocol:subname``.
             table: The name of the table to load or save data to.
             credentials: A dictionary of JDBC database connection arguments.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/spark/spark_streaming_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/spark/spark_streaming_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """SparkStreamingDataset to load and save a PySpark Streaming DataFrame."""
+from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 from kedro.io.core import AbstractDataset
 from pyspark.sql import DataFrame
@@ -34,24 +35,24 @@
             checkpoint: data/04_checkpoint/raw_new_inventory
             header: True
           load_args:
             schema:
                 filepath: data/01_raw/schema/inventory_schema.json
     """
 
-    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
-    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_LOAD_ARGS = {}  # type: dict[str, Any]
+    DEFAULT_SAVE_ARGS = {}  # type: dict[str, Any]
 
     def __init__(
         self,
         *,
         filepath: str = "",
         file_format: str = "",
-        save_args: dict[str, Any] = None,
-        load_args: dict[str, Any] = None,
+        save_args: dict[str, Any] | None = None,
+        load_args: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of SparkStreamingDataset.
 
         Args:
             filepath: Filepath in POSIX format to a Spark dataframe. When using Databricks
                 specify ``filepath``s starting with ``/dbfs/``. For message brokers such as
                 Kafka and all filepath is not required.
@@ -124,22 +125,25 @@
     def _save(self, data: DataFrame) -> None:
         """Saves pyspark dataframe.
         Args:
             data: PySpark streaming dataframe for saving
         """
         save_path = _strip_dbfs_prefix(self._fs_prefix + str(self._filepath))
         output_constructor = data.writeStream.format(self._file_format)
-
+        output_mode = (
+            self._save_args.pop("output_mode", None) if self._save_args else None
+        )
+        checkpoint = (
+            self._save_args.pop("checkpoint", None) if self._save_args else None
+        )
         (
-            output_constructor.option(
-                "checkpointLocation", self._save_args.pop("checkpoint")
-            )
+            output_constructor.option("checkpointLocation", checkpoint)
             .option("path", save_path)
-            .outputMode(self._save_args.pop("output_mode"))
-            .options(**self._save_args)
+            .outputMode(output_mode)
+            .options(**self._save_args or {})
             .start()
         )
 
     def _exists(self) -> bool:
         load_path = _strip_dbfs_prefix(self._fs_prefix + str(self._filepath))
 
         try:
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/svmlight/svmlight_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/svmlight/svmlight_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """``SVMLightDataset`` loads/saves data from/to a svmlight/libsvm file using an
 underlying filesystem (e.g.: local, S3, GCS). It uses sklearn functions
 ``dump_svmlight_file`` to save and ``load_svmlight_file`` to load a file.
 """
+from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import PurePosixPath
-from typing import Any, Optional, Union
+from typing import Any, Union
 
 import fsspec
 from kedro.io.core import (
     AbstractVersionedDataset,
     DatasetError,
     Version,
     get_filepath_str,
@@ -91,20 +92,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Optional[Version] = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of SVMLightDataset to load/save data from a svmlight/libsvm file.
 
         Args:
             filepath: Filepath in POSIX format to a text file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
                 The prefix should be any protocol supported by ``fsspec``.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/tensorflow/tensorflow_model_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``TensorFlowModelDataset`` is a dataset implementation which can save and load
 TensorFlow models.
 """
+from __future__ import annotations
 
 import copy
 import tempfile
 from pathlib import PurePath, PurePosixPath
 from typing import Any
 
 import fsspec
@@ -70,20 +71,20 @@
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] | None = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``TensorFlowModelDataset``.
 
         Args:
             filepath: Filepath in POSIX format to a TensorFlow model directory prefixed with a
                 protocol like `s3://`. If prefix is not provided `file` protocol (local filesystem)
                 will be used. The prefix should be any protocol supported by ``fsspec``.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/text/text_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/text/text_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``TextDataset`` loads/saves data from/to a text file using an underlying
 filesystem (e.g.: local, S3, GCS).
 """
+from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 from kedro.io.core import (
@@ -47,18 +48,18 @@
 
     """
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``TextDataset`` pointing to a concrete text file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a text file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/tracking/json_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/tracking/json_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,13 +44,13 @@
     """
 
     versioned = True
 
     def _load(self) -> NoReturn:
         raise DatasetError(f"Loading not supported for '{self.__class__.__name__}'")
 
-    def preview(self) -> JSONTrackingPreview:
+    def preview(self) -> JSONTrackingPreview:  # type: ignore[override]
         "Load the JSON tracking dataset used in Kedro-viz experiment tracking."
         load_path = get_filepath_str(self._get_load_path(), self._protocol)
 
         with self._fs.open(load_path, **self._fs_open_args_load) as fs_file:
-            return json.load(fs_file)
+            return JSONTrackingPreview(json.load(fs_file))
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/tracking/metrics_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/tracking/metrics_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,13 +64,13 @@
         save_path = get_filepath_str(self._get_save_path(), self._protocol)
 
         with self._fs.open(save_path, **self._fs_open_args_save) as fs_file:
             json.dump(data, fs_file, **self._save_args)
 
         self._invalidate_cache()
 
-    def preview(self) -> MetricsTrackingPreview:
+    def preview(self) -> MetricsTrackingPreview:  # type: ignore[override]
         "Load the Metrics tracking dataset used in Kedro-viz experiment tracking"
         load_path = get_filepath_str(self._get_load_path(), self._protocol)
 
         with self._fs.open(load_path, **self._fs_open_args_load) as fs_file:
             return json.load(fs_file)
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/video/video_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/video/video_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """``VideoDataset`` loads/saves video data from an underlying
 filesystem (e.g.: local, S3, GCS). It uses OpenCV VideoCapture to read
 and decode videos and OpenCV VideoWriter to encode and write video.
 """
+from __future__ import annotations
 
 import itertools
 import tempfile
 from collections import abc
 from collections.abc import Generator, Sequence
 from copy import deepcopy
 from pathlib import Path, PurePosixPath
-from typing import Any, Optional, Union
+from typing import Any
 
 import cv2
 import fsspec
 import numpy as np
 import PIL.Image
 from kedro.io.core import AbstractDataset, get_protocol_and_path
 
@@ -21,17 +22,17 @@
 class SlicedVideo:
     """A representation of slices of other video types"""
 
     def __init__(self, video, slice_indexes):
         self.video = video
         self.indexes = range(*slice_indexes.indices(len(video)))
 
-    def __getitem__(self, index: Union[int, slice]) -> PIL.Image.Image:
+    def __getitem__(self, index: int | slice) -> PIL.Image.Image:
         if isinstance(index, slice):
-            return SlicedVideo(self, index)
+            return SlicedVideo(self, index)  # type: ignore
         return self.video[self.indexes[index]]
 
     def __len__(self) -> int:
         return len(self.indexes)
 
     def __getattr__(self, item):
         return getattr(self.video, item)
@@ -57,15 +58,15 @@
     def size(self) -> tuple[int, int]:
         """Get the resolution of the video"""
         raise NotImplementedError()
 
     def __len__(self) -> int:
         return self._n_frames
 
-    def __getitem__(self, index: Union[int, slice]):
+    def __getitem__(self, index: int | slice):
         """Get a frame from the video"""
         raise NotImplementedError()
 
 
 class FileVideo(AbstractVideo):
     """A video object read from a file"""
 
@@ -85,15 +86,15 @@
 
     @property
     def size(self) -> tuple[int, int]:
         width = int(self._cap.get(cv2.CAP_PROP_FRAME_WIDTH))
         height = int(self._cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
         return width, height
 
-    def __getitem__(self, index: Union[int, slice]):
+    def __getitem__(self, index: int | slice):
         if isinstance(index, slice):
             return SlicedVideo(self, index)
 
         if index < 0:
             index += len(self)
         if index >= len(self):
             raise IndexError()
@@ -147,15 +148,15 @@
     def fps(self) -> float:
         return self._fps
 
     @property
     def size(self) -> tuple[int, int]:
         return self._size
 
-    def __getitem__(self, index: Union[int, slice]):
+    def __getitem__(self, index: int | slice):
         if isinstance(index, slice):
             return SlicedVideo(self, index)
         return self._frames[index]
 
 
 class GeneratorVideo(AbstractVideo):
     """A video object with frames yielded by a generator"""
@@ -182,15 +183,15 @@
     def fps(self) -> float:
         return self._fps
 
     @property
     def size(self) -> tuple[int, int]:
         return self._size
 
-    def __getitem__(self, index: Union[int, slice]):
+    def __getitem__(self, index: int | slice):
         raise NotImplementedError("Underlying video is a generator")
 
     def __next__(self):
         return next(self._gen)
 
     def __iter__(self):
         return self
@@ -267,18 +268,18 @@
 
     """
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        fourcc: Optional[str] = "mp4v",
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        fourcc: str | None = "mp4v",
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of VideoDataset to load / save video data for given filepath.
 
         Args:
             filepath: The location of the video file to load / save data.
             fourcc: The codec to use when writing video, note that depending on how opencv is
                 installed there might be more or less codecs avaiable. If set to None, the
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets/yaml/yaml_dataset.py` & `kedro_datasets-3.0.1/kedro_datasets/yaml/yaml_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``YAMLDataset`` loads/saves data from/to a YAML file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses PyYAML to handle the YAML file.
 """
+from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 import yaml
@@ -50,19 +51,19 @@
 
     DEFAULT_SAVE_ARGS: dict[str, Any] = {"default_flow_style": False}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
-        save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        save_args: dict[str, Any] | None = None,
+        version: Version | None = None,
+        credentials: dict[str, Any] | None = None,
+        fs_args: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Creates a new instance of ``YAMLDataset`` pointing to a concrete YAML file
         on a specific filesystem.
 
         Args:
             filepath: Filepath in POSIX format to a YAML file prefixed with a protocol like `s3://`.
                 If prefix is not provided, `file` protocol (local filesystem) will be used.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets.egg-info/PKG-INFO` & `kedro_datasets-3.0.1/kedro_datasets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-datasets
-Version: 3.0.0
+Version: 3.0.1
 Summary: Kedro-Datasets is where you can find all of Kedro's data connectors.
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: >=3.9
@@ -14,15 +14,15 @@
 Provides-Extra: pandas-base
 Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-base"
 Provides-Extra: spark-base
 Requires-Dist: pyspark<4.0,>=2.2; extra == "spark-base"
 Provides-Extra: hdfs-base
 Requires-Dist: hdfs<3.0,>=2.5.8; extra == "hdfs-base"
 Provides-Extra: s3fs-base
-Requires-Dist: s3fs<2024.1,>=2021.4; extra == "s3fs-base"
+Requires-Dist: s3fs>=2021.04; extra == "s3fs-base"
 Provides-Extra: polars-base
 Requires-Dist: polars>=0.18.0; extra == "polars-base"
 Provides-Extra: plotly-base
 Requires-Dist: plotly<6.0,>=4.8.0; extra == "plotly-base"
 Provides-Extra: delta-base
 Requires-Dist: delta-spark~=1.2.1; extra == "delta-base"
 Provides-Extra: networkx-base
@@ -242,55 +242,51 @@
 Requires-Dist: kedro-datasets[video-videodataset]; extra == "video"
 Provides-Extra: yaml-yamldataset
 Requires-Dist: kedro-datasets[pandas-base]; extra == "yaml-yamldataset"
 Requires-Dist: PyYAML<7.0,>=4.2; extra == "yaml-yamldataset"
 Provides-Extra: yaml
 Requires-Dist: kedro-datasets[yaml-yamldataset]; extra == "yaml"
 Provides-Extra: docs
-Requires-Dist: docutils==0.16; extra == "docs"
-Requires-Dist: sphinx~=5.3.0; extra == "docs"
-Requires-Dist: sphinx_rtd_theme==1.2.0; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints==1.20.2; extra == "docs"
-Requires-Dist: sphinx_copybutton==0.3.1; extra == "docs"
-Requires-Dist: sphinx-notfound-page; extra == "docs"
+Requires-Dist: kedro-sphinx-theme==2024.4.0; extra == "docs"
 Requires-Dist: ipykernel<7.0,>=5.3; extra == "docs"
-Requires-Dist: sphinxcontrib-mermaid~=0.7.1; extra == "docs"
-Requires-Dist: myst-parser~=1.0.0; extra == "docs"
-Requires-Dist: Jinja2<3.1.0; extra == "docs"
+Requires-Dist: Jinja2<3.2.0; extra == "docs"
 Provides-Extra: test
 Requires-Dist: adlfs~=2023.1; extra == "test"
 Requires-Dist: bandit<2.0,>=1.6.2; extra == "test"
 Requires-Dist: behave==1.2.6; extra == "test"
 Requires-Dist: biopython~=1.73; extra == "test"
 Requires-Dist: blacken-docs==1.9.2; extra == "test"
 Requires-Dist: black~=22.0; extra == "test"
 Requires-Dist: cloudpickle<=2.0.0; extra == "test"
 Requires-Dist: compress-pickle[lz4]~=2.1.0; extra == "test"
-Requires-Dist: coverage[toml]; extra == "test"
+Requires-Dist: coverage>=7.2.0; extra == "test"
 Requires-Dist: dask[complete]>=2021.10; extra == "test"
 Requires-Dist: delta-spark<3.0,>=1.0; extra == "test"
 Requires-Dist: deltalake>=0.10.0; extra == "test"
 Requires-Dist: dill~=0.3.1; extra == "test"
 Requires-Dist: filelock<4.0,>=3.4.0; extra == "test"
 Requires-Dist: gcsfs<2023.3,>=2023.1; extra == "test"
 Requires-Dist: geopandas<1.0,>=0.6.0; extra == "test"
 Requires-Dist: hdfs<3.0,>=2.5.8; extra == "test"
 Requires-Dist: holoviews>=1.13.0; extra == "test"
+Requires-Dist: h5netcdf>=1.2.0; extra == "test"
 Requires-Dist: ibis-framework[duckdb,examples]; extra == "test"
 Requires-Dist: import-linter[toml]==1.2.6; extra == "test"
 Requires-Dist: ipython<8.0,>=7.31.1; extra == "test"
 Requires-Dist: Jinja2<3.1.0; extra == "test"
 Requires-Dist: joblib>=0.14; extra == "test"
 Requires-Dist: jupyterlab>=3.0; extra == "test"
 Requires-Dist: jupyter~=1.0; extra == "test"
 Requires-Dist: lxml~=4.6; extra == "test"
 Requires-Dist: matplotlib<3.4,>=3.0.3; python_version < "3.10" and extra == "test"
 Requires-Dist: matplotlib<3.6,>=3.5; python_version >= "3.10" and extra == "test"
 Requires-Dist: memory_profiler<1.0,>=0.50.0; extra == "test"
 Requires-Dist: moto==5.0.0; extra == "test"
+Requires-Dist: mypy~=1.0; extra == "test"
+Requires-Dist: netcdf4>=1.6.4; extra == "test"
 Requires-Dist: networkx~=2.4; extra == "test"
 Requires-Dist: opencv-python~=4.5.5.64; extra == "test"
 Requires-Dist: openpyxl<4.0,>=3.0.3; extra == "test"
 Requires-Dist: pandas-gbq>=0.12.0; extra == "test"
 Requires-Dist: pandas>=2.0; extra == "test"
 Requires-Dist: Pillow~=9.0; extra == "test"
 Requires-Dist: plotly<6.0,>=4.8.0; extra == "test"
@@ -306,16 +302,16 @@
 Requires-Dist: pytest-mock<2.0,>=1.7.1; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=2.2.1; extra == "test"
 Requires-Dist: pytest~=7.2; extra == "test"
 Requires-Dist: redis~=4.1; extra == "test"
 Requires-Dist: requests-mock~=1.6; extra == "test"
 Requires-Dist: requests~=2.20; extra == "test"
 Requires-Dist: ruff~=0.0.290; extra == "test"
-Requires-Dist: s3fs<2024.1,>=2021.04; extra == "test"
-Requires-Dist: snowflake-snowpark-python~=1.0; python_version == "3.9" and extra == "test"
+Requires-Dist: s3fs>=2021.04; extra == "test"
+Requires-Dist: snowflake-snowpark-python~=1.0; python_version < "3.11" and extra == "test"
 Requires-Dist: scikit-learn<2,>=1.0.2; extra == "test"
 Requires-Dist: scipy>=1.7.3; extra == "test"
 Requires-Dist: packaging; extra == "test"
 Requires-Dist: SQLAlchemy>=1.2; extra == "test"
 Requires-Dist: tables>=3.8.0; platform_system == "Windows" and extra == "test"
 Requires-Dist: tables~=3.6; platform_system != "Windows" and extra == "test"
 Requires-Dist: tensorflow-macos~=2.0; (platform_system == "Darwin" and platform_machine == "arm64") and extra == "test"
@@ -323,36 +319,68 @@
 Requires-Dist: triad<1.0,>=0.6.7; extra == "test"
 Requires-Dist: trufflehog~=2.1; extra == "test"
 Requires-Dist: xarray>=2023.1.0; extra == "test"
 Requires-Dist: xlsxwriter~=1.0; extra == "test"
 Requires-Dist: datasets; extra == "test"
 Requires-Dist: huggingface_hub; extra == "test"
 Requires-Dist: transformers[torch]; extra == "test"
+Requires-Dist: types-cachetools; extra == "test"
+Requires-Dist: types-PyYAML; extra == "test"
+Requires-Dist: types-redis; extra == "test"
+Requires-Dist: types-requests; extra == "test"
+Requires-Dist: types-decorator; extra == "test"
+Requires-Dist: types-six; extra == "test"
+Requires-Dist: types-tabulate; extra == "test"
+Provides-Extra: experimental
 Provides-Extra: all
 Requires-Dist: kedro-datasets[docs,test]; extra == "all"
 
 # Kedro-Datasets
 
 <!-- Note that the contents of this file are also used in the documentation, see docs/source/index.md -->
 
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://pypi.org/project/kedro-datasets/)
+[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg)](https://pypi.org/project/kedro-datasets/)
 [![PyPI Version](https://badge.fury.io/py/kedro-datasets.svg)](https://pypi.org/project/kedro-datasets/)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
 
 Welcome to `kedro_datasets`, the home of Kedro's data connectors. Here you will find `AbstractDataset` implementations powering Kedro's DataCatalog created by QuantumBlack and external contributors.
 
 ## Installation
 
 `kedro-datasets` is a Python plugin. To install it:
 
 ```bash
 pip install kedro-datasets
 ```
 
+### Install dependencies at a group-level
+
+Datasets are organised into groups e.g. `pandas`, `spark` and `pickle`. Each group has a collection of datasets, e.g.`pandas.CSVDataset`, `pandas.ParquetDataset` and more. You can install dependencies for an entire group of dependencies as follows:
+
+```bash
+pip install "kedro-datasets[<group>]"
+```
+
+This installs Kedro-Datasets and dependencies related to the dataset group. An example of this could be a workflow that depends on the data types in `pandas`. Run `pip install 'kedro-datasets[pandas]'` to install Kedro-Datasets and the dependencies for the datasets in the [`pandas` group](https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets/kedro_datasets/pandas).
+
+### Install dependencies at a type-level
+
+To limit installation to dependencies specific to a dataset:
+
+```bash
+pip install "kedro-datasets[<group>-<dataset>]"
+```
+
+For example, your workflow might require the `pandas.ExcelDataset`, so to install its dependencies, run `pip install "kedro-datasets[pandas-exceldataset]"`.
+
+```{note}
+From `kedro-datasets` version 3.0.0 onwards, the names of the optional dataset-level dependencies have been normalised to follow [PEP 685](https://peps.python.org/pep-0685/). The '.' character has been replaced with a '-' character and the names are in lowercase. For example, if you had `kedro-datasets[pandas.ExcelDataset]` in your requirements file, it would have to be changed to `kedro-datasets[pandas-exceldataset]`.
+```
+
 ## What `AbstractDataset` implementations are supported?
 
 We support a range of data connectors, including CSV, Excel, Parquet, Feather, HDF5, JSON, Pickle, SQL Tables, SQL Queries, Spark DataFrames and more. We even allow support for working with images.
 
 These data connectors are supported with the APIs of `pandas`, `spark`, `networkx`, `matplotlib`, `yaml` and more.
 
 [The Data Catalog](https://docs.kedro.org/en/stable/data/data_catalog.html) allows you to work with a range of file formats on local file systems, network file systems, cloud object stores, and Hadoop.
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets.egg-info/SOURCES.txt` & `kedro_datasets-3.0.1/kedro_datasets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -83,8 +83,9 @@
 kedro_datasets/text/text_dataset.py
 kedro_datasets/tracking/__init__.py
 kedro_datasets/tracking/json_dataset.py
 kedro_datasets/tracking/metrics_dataset.py
 kedro_datasets/video/__init__.py
 kedro_datasets/video/video_dataset.py
 kedro_datasets/yaml/__init__.py
-kedro_datasets/yaml/yaml_dataset.py
+kedro_datasets/yaml/yaml_dataset.py
+kedro_datasets_experimental/__init__.py
```

### Comparing `kedro-datasets-3.0.0/kedro_datasets.egg-info/requires.txt` & `kedro_datasets-3.0.1/kedro_datasets.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,24 +29,19 @@
 [databricks-managedtabledataset]
 kedro-datasets[delta-base,pandas-base,spark-base]
 
 [delta-base]
 delta-spark~=1.2.1
 
 [docs]
-docutils==0.16
-sphinx~=5.3.0
-sphinx_rtd_theme==1.2.0
-sphinx-autodoc-typehints==1.20.2
-sphinx_copybutton==0.3.1
-sphinx-notfound-page
+kedro-sphinx-theme==2024.4.0
 ipykernel<7.0,>=5.3
-sphinxcontrib-mermaid~=0.7.1
-myst-parser~=1.0.0
-Jinja2<3.1.0
+Jinja2<3.2.0
+
+[experimental]
 
 [geopandas]
 kedro-datasets[geopandas-geojsondataset]
 
 [geopandas-geojsondataset]
 geopandas<1.0,>=0.6.0
 pyproj~=3.0
@@ -292,15 +287,15 @@
 [redis]
 kedro-datasets[redis-pickledataset]
 
 [redis-pickledataset]
 redis~=4.1
 
 [s3fs-base]
-s3fs<2024.1,>=2021.4
+s3fs>=2021.04
 
 [snowflake]
 kedro-datasets[snowflake-snowparktabledataset]
 
 [snowflake-snowparktabledataset]
 snowflake-snowpark-python~=1.0
 
@@ -346,34 +341,37 @@
 bandit<2.0,>=1.6.2
 behave==1.2.6
 biopython~=1.73
 blacken-docs==1.9.2
 black~=22.0
 cloudpickle<=2.0.0
 compress-pickle[lz4]~=2.1.0
-coverage[toml]
+coverage>=7.2.0
 dask[complete]>=2021.10
 delta-spark<3.0,>=1.0
 deltalake>=0.10.0
 dill~=0.3.1
 filelock<4.0,>=3.4.0
 gcsfs<2023.3,>=2023.1
 geopandas<1.0,>=0.6.0
 hdfs<3.0,>=2.5.8
 holoviews>=1.13.0
+h5netcdf>=1.2.0
 ibis-framework[duckdb,examples]
 import-linter[toml]==1.2.6
 ipython<8.0,>=7.31.1
 Jinja2<3.1.0
 joblib>=0.14
 jupyterlab>=3.0
 jupyter~=1.0
 lxml~=4.6
 memory_profiler<1.0,>=0.50.0
 moto==5.0.0
+mypy~=1.0
+netcdf4>=1.6.4
 networkx~=2.4
 opencv-python~=4.5.5.64
 openpyxl<4.0,>=3.0.3
 pandas-gbq>=0.12.0
 pandas>=2.0
 Pillow~=9.0
 plotly<6.0,>=4.8.0
@@ -385,26 +383,33 @@
 pytest-mock<2.0,>=1.7.1
 pytest-xdist[psutil]~=2.2.1
 pytest~=7.2
 redis~=4.1
 requests-mock~=1.6
 requests~=2.20
 ruff~=0.0.290
-s3fs<2024.1,>=2021.04
+s3fs>=2021.04
 scikit-learn<2,>=1.0.2
 scipy>=1.7.3
 packaging
 SQLAlchemy>=1.2
 triad<1.0,>=0.6.7
 trufflehog~=2.1
 xarray>=2023.1.0
 xlsxwriter~=1.0
 datasets
 huggingface_hub
 transformers[torch]
+types-cachetools
+types-PyYAML
+types-redis
+types-requests
+types-decorator
+types-six
+types-tabulate
 
 [test:platform_system != "Darwin" or platform_machine != "arm64"]
 tensorflow~=2.0
 
 [test:platform_system != "Windows"]
 tables~=3.6
 
@@ -416,16 +421,14 @@
 
 [test:python_version < "3.10"]
 matplotlib<3.4,>=3.0.3
 
 [test:python_version < "3.11"]
 pyarrow>=1.0
 pyspark<3.4,>=3.0
-
-[test:python_version == "3.9"]
 snowflake-snowpark-python~=1.0
 
 [test:python_version >= "3.10"]
 matplotlib<3.6,>=3.5
 
 [test:python_version >= "3.11"]
 pyarrow>=7.0
```

### Comparing `kedro-datasets-3.0.0/pyproject.toml` & `kedro_datasets-3.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 dynamic = ["readme", "version"]
 
 [project.optional-dependencies]
 pandas-base = ["pandas>=1.3, <3.0",]
 spark-base = ["pyspark>=2.2, <4.0",]
 hdfs-base = ["hdfs>=2.5.8, <3.0",]
-s3fs-base = ["s3fs>=2021.4, <2024.1",]  # Upper bound set arbitrarily, to be reassessed in early 2024
+s3fs-base = ["s3fs>=2021.04",]
 polars-base = ["polars>=0.18.0",]
 plotly-base = ["plotly>=4.8.0, <6.0"]
 delta-base = ["delta-spark~=1.2.1",]
 networkx-base = ["networkx~=2.4"]
 
 # Individual Datasets
 api-apidataset = ["requests~=2.20"]
@@ -160,64 +160,59 @@
 
 video-videodataset = ["opencv-python~=4.5.5.64"]
 video = ["kedro-datasets[video-videodataset]"]
 
 yaml-yamldataset = ["kedro-datasets[pandas-base]", "PyYAML>=4.2, <7.0"]
 yaml = ["kedro-datasets[yaml-yamldataset]"]
 
+# Experimental Datasets
+
+
 # Docs requirements
 docs = [
-    # docutils>=0.17 changed the HTML
-    # see https://github.com/readthedocs/sphinx_rtd_theme/issues/1115
-    "docutils==0.16",
-    "sphinx~=5.3.0",
-    "sphinx_rtd_theme==1.2.0",
-    # Regression on sphinx-autodoc-typehints 1.21
-    # that creates some problematic docstrings
-    "sphinx-autodoc-typehints==1.20.2",
-    "sphinx_copybutton==0.3.1",
-    "sphinx-notfound-page",
+    "kedro-sphinx-theme==2024.4.0",
     "ipykernel>=5.3, <7.0",
-    "sphinxcontrib-mermaid~=0.7.1",
-    "myst-parser~=1.0.0",
-    "Jinja2<3.1.0",
+    "Jinja2<3.2.0",
 ]
 
 # Test requirements
 test = [
     "adlfs~=2023.1",
     "bandit>=1.6.2, <2.0",
     "behave==1.2.6",
     "biopython~=1.73",
     "blacken-docs==1.9.2",
     "black~=22.0",
     "cloudpickle<=2.0.0",
     "compress-pickle[lz4]~=2.1.0",
-    "coverage[toml]",
+    "coverage>=7.2.0",
     "dask[complete]>=2021.10",
     "delta-spark>=1.0, <3.0",
     "deltalake>=0.10.0",
     "dill~=0.3.1",
     "filelock>=3.4.0, <4.0",
     "gcsfs>=2023.1, <2023.3",
     "geopandas>=0.6.0, <1.0",
     "hdfs>=2.5.8, <3.0",
     "holoviews>=1.13.0",
+    "h5netcdf>=1.2.0",
     "ibis-framework[duckdb,examples]",
     "import-linter[toml]==1.2.6",
     "ipython>=7.31.1, <8.0",
     "Jinja2<3.1.0",
     "joblib>=0.14",
     "jupyterlab>=3.0",
     "jupyter~=1.0",
     "lxml~=4.6",
     "matplotlib>=3.0.3, <3.4; python_version < '3.10'",  # 3.4.0 breaks holoviews
     "matplotlib>=3.5, <3.6; python_version >= '3.10'",
     "memory_profiler>=0.50.0, <1.0",
     "moto==5.0.0",
+    "mypy~=1.0",
+    "netcdf4>=1.6.4",
     "networkx~=2.4",
     "opencv-python~=4.5.5.64",
     "openpyxl>=3.0.3, <4.0",
     "pandas-gbq>=0.12.0",
     "pandas>=2.0",
     "Pillow~=9.0",
     "plotly>=4.8.0, <6.0",
@@ -233,16 +228,16 @@
     "pytest-mock>=1.7.1, <2.0",
     "pytest-xdist[psutil]~=2.2.1",
     "pytest~=7.2",
     "redis~=4.1",
     "requests-mock~=1.6",
     "requests~=2.20",
     "ruff~=0.0.290",
-    "s3fs>=2021.04, <2024.1",
-    "snowflake-snowpark-python~=1.0; python_version == '3.9'",
+    "s3fs>=2021.04",
+    "snowflake-snowpark-python~=1.0; python_version < '3.11'",
     "scikit-learn>=1.0.2,<2",
     "scipy>=1.7.3",
     "packaging",
     "SQLAlchemy>=1.2",
     "tables>=3.8.0; platform_system == 'Windows'",  # Import issues with python 3.8 with pytables pinning to 3.8.0 fixes this https://github.com/PyTables/PyTables/issues/933#issuecomment-1555917593
     "tables~=3.6; platform_system != 'Windows'",
     "tensorflow-macos~=2.0; platform_system == 'Darwin' and platform_machine == 'arm64'",
@@ -251,20 +246,30 @@
     "trufflehog~=2.1",
     "xarray>=2023.1.0",
     "xlsxwriter~=1.0",
     # huggingface
     "datasets",
     "huggingface_hub",
     "transformers[torch]",
+    # mypy related dependencies
+    "types-cachetools",
+    "types-PyYAML",
+    "types-redis",
+    "types-requests",
+    "types-decorator",
+    "types-six",
+    "types-tabulate",
 ]
 
+# Experimental dataset requirements
+experimental = []
+
 # All requirements
 all = ["kedro-datasets[test,docs]"]
 
-
 [project.urls]
 Source = "https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets"
 Documentation = "https://docs.kedro.org"
 Tracker = "https://github.com/kedro-org/kedro-plugins/issues"
 
 [tool.setuptools.packages.find]
 include = ["kedro_datasets*"]
@@ -274,15 +279,15 @@
 version = {attr = "kedro_datasets.__version__"}
 
 [tool.coverage.report]
 fail_under = 100
 show_missing = true
 # temporarily ignore kedro_datasets/__init__.py in coverage report
 omit = ["tests/*", "kedro_datasets/holoviews/*", "kedro_datasets/netcdf/*", "kedro_datasets/snowflake/*", "kedro_datasets/tensorflow/*", "kedro_datasets/__init__.py", "kedro_datasets/conftest.py", "kedro_datasets/databricks/*"]
-exclude_lines = ["pragma: no cover", "raise NotImplementedError", "if TYPE_CHECKING:"]
+exclude_also = ["raise NotImplementedError", "if TYPE_CHECKING:"]
 
 [tool.pytest.ini_options]
 addopts = """
 --cov-report xml:coverage.xml \
 --cov-report term-missing \
 --cov kedro_datasets \
 --cov tests \
@@ -304,7 +309,10 @@
     "T201", # Print Statement
 ]
 ignore = ["E501"]  # Black takes care of line-too-long
 
 [tool.ruff.per-file-ignores]
 "{tests,docs}/*" = ["PLR2004", "PLR0913", "T201"]
 "*/{__init__.py}" = ["F821"] # temporarily ignore ruff undefined name errors for dataset aliases
+
+[tool.mypy]
+ignore_missing_imports = true
```

