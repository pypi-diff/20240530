# Comparing `tmp/dvcx-0.85.0.tar.gz` & `tmp/dvcx-0.85.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.85.0.tar", last modified: Mon May 27 15:29:15 2024, max compression
+gzip compressed data, was "dvcx-0.85.1.tar", last modified: Thu May 30 03:40:38 2024, max compression
```

## Comparing `dvcx-0.85.0.tar` & `dvcx-0.85.1.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.335796 dvcx-0.85.0/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-27 15:29:07.000000 dvcx-0.85.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 15:29:07.000000 dvcx-0.85.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.291796 dvcx-0.85.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.291796 dvcx-0.85.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-27 15:29:07.000000 dvcx-0.85.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-27 15:29:07.000000 dvcx-0.85.0/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-27 15:29:07.000000 dvcx-0.85.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-27 15:29:07.000000 dvcx-0.85.0/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-27 15:29:07.000000 dvcx-0.85.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.291796 dvcx-0.85.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-27 15:29:07.000000 dvcx-0.85.0/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-27 15:29:07.000000 dvcx-0.85.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-27 15:29:07.000000 dvcx-0.85.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-27 15:29:07.000000 dvcx-0.85.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-27 15:29:07.000000 dvcx-0.85.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-27 15:29:07.000000 dvcx-0.85.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.291796 dvcx-0.85.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-27 15:29:07.000000 dvcx-0.85.0/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 15:29:07.000000 dvcx-0.85.0/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-27 15:29:07.000000 dvcx-0.85.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-27 15:29:07.000000 dvcx-0.85.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-27 15:29:07.000000 dvcx-0.85.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.291796 dvcx-0.85.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-27 15:29:07.000000 dvcx-0.85.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-27 15:29:07.000000 dvcx-0.85.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-27 15:29:07.000000 dvcx-0.85.0/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-27 15:29:15.335796 dvcx-0.85.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-27 15:29:07.000000 dvcx-0.85.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.291796 dvcx-0.85.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-27 15:29:07.000000 dvcx-0.85.0/docs/cv_intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-27 15:29:07.000000 dvcx-0.85.0/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.295796 dvcx-0.85.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/llm-claude-aggregate-query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/llm-claude-simple-query.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/llm-claude.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.295796 dvcx-0.85.0/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.299796 dvcx-0.85.0/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.299796 dvcx-0.85.0/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-27 15:29:07.000000 dvcx-0.85.0/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-27 15:29:07.000000 dvcx-0.85.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-27 15:29:07.000000 dvcx-0.85.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:29:15.335796 dvcx-0.85.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.283796 dvcx-0.85.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.303796 dvcx-0.85.0/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-27 15:29:15.000000 dvcx-0.85.0/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.303796 dvcx-0.85.0/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73432 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.307796 dvcx-0.85.0/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.307796 dvcx-0.85.0/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46164 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24923 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    31653 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    16157 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.311796 dvcx-0.85.0/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/feature_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/vfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.315796 dvcx-0.85.0/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    61693 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/query/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/query/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.315796 dvcx-0.85.0/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.315796 dvcx-0.85.0/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.315796 dvcx-0.85.0/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.315796 dvcx-0.85.0/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.315796 dvcx-0.85.0/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-27 15:29:07.000000 dvcx-0.85.0/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.331796 dvcx-0.85.0/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-27 15:29:15.000000 dvcx-0.85.0/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-27 15:29:15.000000 dvcx-0.85.0/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:29:15.000000 dvcx-0.85.0/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 15:29:15.000000 dvcx-0.85.0/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-27 15:29:15.000000 dvcx-0.85.0/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 15:29:15.000000 dvcx-0.85.0/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.319796 dvcx-0.85.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.319796 dvcx-0.85.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16373 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.319796 dvcx-0.85.0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35240 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   112436 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    29281 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/func/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.319796 dvcx-0.85.0/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/scripts/name_len_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/scripts/name_len_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/test_cli_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/test_query_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.327796 dvcx-0.85.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.327796 dvcx-0.85.0/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/lib/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/lib/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/lib/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.327796 dvcx-0.85.0/tests/unit/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:15.331796 dvcx-0.85.0/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/sql/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_dataset_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-27 15:29:07.000000 dvcx-0.85.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.359616 dvcx-0.85.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-30 03:40:30.000000 dvcx-0.85.1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-30 03:40:30.000000 dvcx-0.85.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.311616 dvcx-0.85.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.311616 dvcx-0.85.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.311616 dvcx-0.85.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-30 03:40:30.000000 dvcx-0.85.1/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-30 03:40:30.000000 dvcx-0.85.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-30 03:40:30.000000 dvcx-0.85.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.311616 dvcx-0.85.1/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 03:40:30.000000 dvcx-0.85.1/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-30 03:40:30.000000 dvcx-0.85.1/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-30 03:40:30.000000 dvcx-0.85.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-30 03:40:30.000000 dvcx-0.85.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-30 03:40:30.000000 dvcx-0.85.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.311616 dvcx-0.85.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-30 03:40:30.000000 dvcx-0.85.1/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-30 03:40:30.000000 dvcx-0.85.1/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-30 03:40:30.000000 dvcx-0.85.1/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-30 03:40:38.355616 dvcx-0.85.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-30 03:40:30.000000 dvcx-0.85.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.311616 dvcx-0.85.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-30 03:40:30.000000 dvcx-0.85.1/docs/cv_intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-30 03:40:30.000000 dvcx-0.85.1/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.315616 dvcx-0.85.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/llm-claude-aggregate-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/llm-claude-simple-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/llm-claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.315616 dvcx-0.85.1/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.319616 dvcx-0.85.1/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.319616 dvcx-0.85.1/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-30 03:40:30.000000 dvcx-0.85.1/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-30 03:40:30.000000 dvcx-0.85.1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-30 03:40:30.000000 dvcx-0.85.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:40:38.359616 dvcx-0.85.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.303616 dvcx-0.85.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.323616 dvcx-0.85.1/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-30 03:40:38.000000 dvcx-0.85.1/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.323616 dvcx-0.85.1/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73445 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.323616 dvcx-0.85.1/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.327616 dvcx-0.85.1/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46118 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10884 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24815 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31653 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16157 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.331616 dvcx-0.85.1/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/feature_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/vfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.331616 dvcx-0.85.1/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61615 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.335616 dvcx-0.85.1/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.335616 dvcx-0.85.1/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.335616 dvcx-0.85.1/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.335616 dvcx-0.85.1/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.335616 dvcx-0.85.1/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-30 03:40:30.000000 dvcx-0.85.1/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.351616 dvcx-0.85.1/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-30 03:40:38.000000 dvcx-0.85.1/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-30 03:40:38.000000 dvcx-0.85.1/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:40:38.000000 dvcx-0.85.1/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 03:40:38.000000 dvcx-0.85.1/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-30 03:40:38.000000 dvcx-0.85.1/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 03:40:38.000000 dvcx-0.85.1/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.339616 dvcx-0.85.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.339616 dvcx-0.85.1/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16373 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.339616 dvcx-0.85.1/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35240 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112436 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29281 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/func/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.343616 dvcx-0.85.1/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/scripts/name_len_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/scripts/name_len_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/test_cli_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/test_query_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.347616 dvcx-0.85.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.347616 dvcx-0.85.1/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.351616 dvcx-0.85.1/tests/unit/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:38.351616 dvcx-0.85.1/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_dataset_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-30 03:40:30.000000 dvcx-0.85.1/tests/utils.py
```

### Comparing `dvcx-0.85.0/.cruft.json` & `dvcx-0.85.1/.cruft.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'fd347ad0bc86b4bf8ef5b6cba47cad02fbcb89c3'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "de956df5482ba686b8c4a4f2c53052da59e18d4c",
+    "commit": "fd347ad0bc86b4bf8ef5b6cba47cad02fbcb89c3",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/iterative/py-template",
             "author": "Dmitry Petrov",
             "copyright_year": "2022",
             "development_status": "Development Status :: 2 - Pre-Alpha",
             "docs": "False",
```

### Comparing `dvcx-0.85.0/.github/workflows/benchmarks.yml` & `dvcx-0.85.1/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/.github/workflows/release.yml` & `dvcx-0.85.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/.github/workflows/tests.yml` & `dvcx-0.85.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/.gitignore` & `dvcx-0.85.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/.pre-commit-config.yaml` & `dvcx-0.85.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,21 @@
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: ['--fix=lf']
       - id: sort-simple-yaml
       - id: trailing-whitespace
         exclude: '^LICENSES/'
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.4.5'
+    rev: 'v0.4.6'
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.5
+    rev: v2.3.0
     hooks:
       - id: codespell
         additional_dependencies: ["tomli"]
   - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
     rev: v2.13.0
     hooks:
       - id: pretty-format-toml
```

### Comparing `dvcx-0.85.0/CODE_OF_CONDUCT.rst` & `dvcx-0.85.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/CONTRIBUTING.rst` & `dvcx-0.85.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/LICENSE` & `dvcx-0.85.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/LICENSES/Apache-2.0.txt` & `dvcx-0.85.1/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/LICENSES/BSD-3-Clause.txt` & `dvcx-0.85.1/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/LICENSES/Python-2.0.txt` & `dvcx-0.85.1/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/PKG-INFO` & `dvcx-0.85.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.85.0
+Version: 0.85.1
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.85.0/README.rst` & `dvcx-0.85.1/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/docs/cv_intro.md` & `dvcx-0.85.1/docs/cv_intro.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/docs/udfs.md` & `dvcx-0.85.1/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/blip2_image_desc_lib.py` & `dvcx-0.85.1/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/clip.py` & `dvcx-0.85.1/examples/clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/common_sql_functions.py` & `dvcx-0.85.1/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/dir_expansion.py` & `dvcx-0.85.1/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/hf_pipeline.py` & `dvcx-0.85.1/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/llava2_image_desc_lib.py` & `dvcx-0.85.1/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/llm-claude-aggregate-query.py` & `dvcx-0.85.1/examples/llm-claude-aggregate-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/llm-claude-simple-query.py` & `dvcx-0.85.1/examples/llm-claude-simple-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/llm-claude.py` & `dvcx-0.85.1/examples/llm-claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/loader.py` & `dvcx-0.85.1/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/neurips/README` & `dvcx-0.85.1/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/neurips/distance_to_query.py` & `dvcx-0.85.1/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/neurips/llm_chat.py` & `dvcx-0.85.1/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/neurips/single_query.py` & `dvcx-0.85.1/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/neurips/text_loaders.py` & `dvcx-0.85.1/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/openai_image_desc_lib.py` & `dvcx-0.85.1/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/openimage-detect.py` & `dvcx-0.85.1/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/pose_detection.py` & `dvcx-0.85.1/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/torch-loader.py` & `dvcx-0.85.1/examples/torch-loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/udfs/batching.py` & `dvcx-0.85.1/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/udfs/image_transformation.py` & `dvcx-0.85.1/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/udfs/parallel.py` & `dvcx-0.85.1/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/udfs/simple.py` & `dvcx-0.85.1/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/udfs/stateful.py` & `dvcx-0.85.1/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/udfs/stateful_similarity.py` & `dvcx-0.85.1/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/unstructured-text.py` & `dvcx-0.85.1/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/wds.py` & `dvcx-0.85.1/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/wds_filtered.py` & `dvcx-0.85.1/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/wds_meta.py` & `dvcx-0.85.1/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/zalando/zalando_clip.py` & `dvcx-0.85.1/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.85.1/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/noxfile.py` & `dvcx-0.85.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/pyproject.toml` & `dvcx-0.85.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
 warn_unreachable = true
 ignore_missing_imports = true
 disable_error_code = "annotation-unchecked"
 files = ["src", "tests"]
 
 [tool.codespell]
 ignore-words-list = " "
+skip = "CODE_OF_CONDUCT.rst"
 
 [tool.ruff]
 output-format = "full"
 show-fixes = true
 
 [tool.ruff.lint]
 ignore = [
```

### Comparing `dvcx-0.85.0/src/dvcx/asyn.py` & `dvcx-0.85.1/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/cache.py` & `dvcx-0.85.1/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/catalog/catalog.py` & `dvcx-0.85.1/src/dvcx/catalog/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -601,14 +601,15 @@
         }
 
     def copy(self, cache=True, db=True):
         result = copy(self)
         if not db:
             result.id_generator = None
             result.metastore = None
+            result._warehouse = None
             result.warehouse = None
         return result
 
     @classmethod
     def generate_query_dataset_name(cls) -> str:
         return f"{QUERY_DATASET_PREFIX}_{uuid4().hex}"
 
@@ -688,15 +689,15 @@
             storage = source_metastore.get_storage(client.uri)
             source_metastore.init_partial_id(client.uri)
             partial_id = source_metastore.get_next_partial_id(client.uri)
 
             source_metastore = self.metastore.clone(
                 uri=client.uri, partial_id=partial_id
             )
-            source_metastore.init(client.uri, partial_id)
+            source_metastore.init(client.uri)
 
             source_warehouse = self.warehouse.clone()
             dataset = self.create_dataset(storage_dataset_name, listing=True)
 
             return (
                 Listing(storage, source_metastore, source_warehouse, client, dataset),
                 path,
@@ -737,15 +738,15 @@
             )
 
             return lst, path
 
         source_metastore.init_partial_id(client.uri)
         partial_id = source_metastore.get_next_partial_id(client.uri)
 
-        source_metastore.init(client.uri, partial_id)
+        source_metastore.init(client.uri)
         source_metastore = self.metastore.clone(uri=client.uri, partial_id=partial_id)
 
         source_warehouse = self.warehouse.clone()
 
         dataset = self.create_dataset(storage_dataset_name, listing=True)
 
         lst = Listing(storage, source_metastore, source_warehouse, client, dataset)
```

### Comparing `dvcx-0.85.0/src/dvcx/catalog/datasource.py` & `dvcx-0.85.1/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/catalog/loader.py` & `dvcx-0.85.1/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/cli.py` & `dvcx-0.85.1/src/dvcx/cli.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/cli_utils.py` & `dvcx-0.85.1/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/client/azure.py` & `dvcx-0.85.1/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/client/fileslice.py` & `dvcx-0.85.1/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/client/fsspec.py` & `dvcx-0.85.1/src/dvcx/client/fsspec.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/client/gcs.py` & `dvcx-0.85.1/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/client/local.py` & `dvcx-0.85.1/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/client/s3.py` & `dvcx-0.85.1/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/config.py` & `dvcx-0.85.1/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/data_storage/db_engine.py` & `dvcx-0.85.1/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/data_storage/id_generator.py` & `dvcx-0.85.1/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/data_storage/metastore.py` & `dvcx-0.85.1/src/dvcx/data_storage/metastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,17 @@
         use_new_connection: bool = False,
     ) -> "AbstractMetastore":
         """Clones AbstractMetastore implementation for some Storage input.
         Setting use_new_connection will always use a new database connection.
         New connections should only be used if needed due to errors with
         closed connections."""
 
-    def init(self, uri: StorageURI, partial_id: int) -> None:
-        """Initialize metastore."""
+    @abstractmethod
+    def init(self, uri: StorageURI) -> None:
+        """Initialize partials table for given storage uri."""
 
     def close(self) -> None:
         """Closes any active database or HTTP connections."""
 
     def cleanup_temp_tables(self, temp_table_names: list[str]):
         """Cleanup temp tables."""
 
@@ -380,14 +381,18 @@
         id_generator: "AbstractIDGenerator",
         uri: StorageURI = StorageURI(""),
         partial_id: Optional[int] = None,
     ):
         self.id_generator = id_generator
         super().__init__(uri, partial_id)
 
+    @abstractmethod
+    def init(self, uri: StorageURI) -> None:
+        """Initialize partials table for given storage uri."""
+
     def close(self) -> None:
         """Closes any active database connections."""
         self.db.close()
 
     def cleanup_temp_tables(self, temp_table_names: list[str]):
         """Cleanup temp tables."""
         self.id_generator.delete_uris(temp_table_names)
@@ -580,68 +585,68 @@
 
     @abstractmethod
     def _storages_insert(self): ...
 
     def _storages_select(self, *columns):
         if not columns:
             return self._storages.select()
-        return select(*columns).select_from(self._storages)
+        return select(*columns)
 
     def _storages_update(self):
         return self._storages.update()
 
     def _storages_delete(self):
         return self._storages.delete()
 
     @abstractmethod
     def _partials_insert(self): ...
 
     def _partials_select(self, *columns):
         if not columns:
             return self._partials.select()
-        return select(*columns).select_from(self._partials)
+        return select(*columns)
 
     def _partials_update(self):
         return self._partials.update()
 
     @abstractmethod
     def _datasets_insert(self): ...
 
     def _datasets_select(self, *columns):
         if not columns:
             return self._datasets.select()
-        return select(*columns).select_from(self._datasets)
+        return select(*columns)
 
     def _datasets_update(self):
         return self._datasets.update()
 
     def _datasets_delete(self):
         return self._datasets.delete()
 
     @abstractmethod
     def _datasets_versions_insert(self): ...
 
     def _datasets_versions_select(self, *columns):
         if not columns:
             return self._datasets_versions.select()
-        return select(*columns).select_from(self._datasets_versions)
+        return select(*columns)
 
     def _datasets_versions_update(self):
         return self._datasets_versions.update()
 
     def _datasets_versions_delete(self):
         return self._datasets_versions.delete()
 
     @abstractmethod
     def _datasets_dependencies_insert(self): ...
 
     def _datasets_dependencies_select(self, *columns):
         if not columns:
             return self._datasets_dependencies.select()
-        return select(*columns).select_from(self._datasets_dependencies)
+        return select(*columns)
 
     def _datasets_dependencies_update(self):
         return self._datasets_dependencies.update()
 
     def _datasets_dependencies_delete(self):
         return self._datasets_dependencies.delete()
 
@@ -898,15 +903,14 @@
         # This SQL statement finds all entries that are
         # prefixes of the given prefix, matching this or parent directories
         # that are indexed.
         dir_prefix = posixpath.join(prefix, "")
         p = self._partials_table(uri)
         expire_values = self.db.execute(
             select(p.c.expires, p.c.partial_id, p.c.path_str)
-            .select_from(p)
             .where(
                 p.c.path_str == func.substr(dir_prefix, 1, func.length(p.c.path_str))
             )
             .order_by(p.c.expires.desc())
         )
         for expires, partial_id, path_str in expire_values:
             if not is_expired(expires):
@@ -917,15 +921,15 @@
 
     def get_last_partial_path(self, uri: StorageURI) -> Optional[str]:
         """Returns last partial path for given storage."""
         p = self._partials_table(uri)
         if not self.db.has_table(p.name):
             raise StorageNotFoundError(f"Storage {uri} partials are not found.")
         last_partial = self.db.execute(
-            select(p.c.path_str).select_from(p).order_by(p.c.timestamp.desc()).limit(1)
+            select(p.c.path_str).order_by(p.c.timestamp.desc()).limit(1)
         )
         for (path_str,) in last_partial:
             return path_str
         return None
 
     #
     # Datasets
@@ -1291,23 +1295,23 @@
 
         dataset_version = dataset.get_version(version)
 
         select_cols = self._dataset_dependencies_select_columns()
 
         query = (
             self._datasets_dependencies_select(*select_cols)
-            .where(
-                (dd.c.source_dataset_id == dataset.id)
-                & (dd.c.source_dataset_version_id == dataset_version.id)
-            )
             .select_from(
                 dd.join(d, dd.c.dataset_id == d.c.id, isouter=True)
                 .join(s, dd.c.bucket_id == s.c.id, isouter=True)
                 .join(dv, dd.c.dataset_version_id == dv.c.id, isouter=True)
             )
+            .where(
+                (dd.c.source_dataset_id == dataset.id)
+                & (dd.c.source_dataset_version_id == dataset_version.id)
+            )
         )
         if version:
             dataset_version = dataset.get_version(version)
             query = query.where(dd.c.source_dataset_version_id == dataset_version.id)
 
         return [self.dependency_class.parse(*r) for r in self.db.execute(query)]
```

### Comparing `dvcx-0.85.0/src/dvcx/data_storage/schema.py` & `dvcx-0.85.1/src/dvcx/data_storage/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         """
         return query
 
     def select(self, *columns):
         if not columns:
             query = self.table.select()
         else:
-            query = sa.select(*columns).select_from(self.table)
+            query = sa.select(*columns)
         return self.apply_conditions(query)
 
     def insert(self):
         return self.table.insert()
 
     def update(self):
         return self.apply_conditions(self.table.update())
```

### Comparing `dvcx-0.85.0/src/dvcx/data_storage/serializer.py` & `dvcx-0.85.1/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/data_storage/sqlite.py` & `dvcx-0.85.1/src/dvcx/data_storage/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,19 +316,15 @@
                 .on_conflict_do_update(
                     index_elements=["uri"],
                     set_={"last_id": self._table.c.last_id + count},
                 )
             )
             self._db.execute(stmt_ins, conn=conn)
 
-            stmt_sel = (
-                select(self._table.c.last_id)
-                .select_from(self._table)
-                .where(self._table.c.uri == uri)
-            )
+            stmt_sel = select(self._table.c.last_id).where(self._table.c.uri == uri)
             last_id = self._db.execute(stmt_sel, conn=conn).fetchone()[0]
 
         return range(last_id - count + 1, last_id + 1)
 
 
 class SQLiteMetastore(AbstractDBMetastore):
     """
@@ -426,15 +422,15 @@
         self.db.create_table(self._datasets, if_not_exists=True)
         self.default_table_names.append(self._datasets.name)
         self.db.create_table(self._datasets_versions, if_not_exists=True)
         self.default_table_names.append(self._datasets_versions.name)
         self.db.create_table(self._datasets_dependencies, if_not_exists=True)
         self.default_table_names.append(self._datasets_dependencies.name)
 
-    def init(self, uri: StorageURI, partial_id: int) -> None:
+    def init(self, uri: StorageURI) -> None:
         if not uri:
             raise ValueError("uri for init() cannot be empty")
         partials_table = self._partials_table(uri)
         self.db.create_table(partials_table, if_not_exists=True)
 
     @classmethod
     def _buckets_columns(cls) -> list["SchemaItem"]:
```

### Comparing `dvcx-0.85.0/src/dvcx/data_storage/warehouse.py` & `dvcx-0.85.1/src/dvcx/data_storage/warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/dataset.py` & `dvcx-0.85.1/src/dvcx/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/error.py` & `dvcx-0.85.1/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/cached_stream.py` & `dvcx-0.85.1/src/dvcx/lib/cached_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self.cached_file = None
 
         self.temp_file = None
         self.temp_file_pos = 0
 
     def __enter__(self):
         if os.path.exists(self.target_path):
-            self.cached_file = open(self.target_path, mode=self.mode)  # noqa: SIM115
+            self.cached_file = open(self.target_path, mode=self.mode)
             return self.cached_file
 
         tmp_dir = self.catalog.cache.tmp_dir
         if not os.path.exists(tmp_dir):
             os.makedirs(tmp_dir)
         self.temp_file = tempfile.NamedTemporaryFile(
             prefix=str(self.uid.get_hash()), dir=tmp_dir, delete=False
@@ -103,15 +103,15 @@
         self.cached_file = None
 
     def get_path_in_cache(self):
         return self.catalog.cache.path_from_checksum(self.uid.get_hash())
 
     def __enter__(self):
         self.client.download(self.uid)
-        self.cached_file = open(self.get_path_in_cache(), self.mode)  # noqa: SIM115
+        self.cached_file = open(self.get_path_in_cache(), self.mode)
         return self.cached_file
 
     def __exit__(self, *args):
         self.cached_file.close()
 
 
 class PreDownloadStream(PreCachedStream):
```

### Comparing `dvcx-0.85.0/src/dvcx/lib/claude.py` & `dvcx-0.85.1/src/dvcx/lib/claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/dataset.py` & `dvcx-0.85.1/src/dvcx/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/feature.py` & `dvcx-0.85.1/src/dvcx/lib/feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/feature_types.py` & `dvcx-0.85.1/src/dvcx/lib/feature_types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/feature_udf.py` & `dvcx-0.85.1/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/file.py` & `dvcx-0.85.1/src/dvcx/lib/file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.85.1/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.85.1/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.85.1/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/image.py` & `dvcx-0.85.1/src/dvcx/lib/image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/image_transform.py` & `dvcx-0.85.1/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.85.1/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/pytorch.py` & `dvcx-0.85.1/src/dvcx/lib/pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/reader.py` & `dvcx-0.85.1/src/dvcx/lib/reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/text.py` & `dvcx-0.85.1/src/dvcx/lib/text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/udf.py` & `dvcx-0.85.1/src/dvcx/lib/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/unstructured.py` & `dvcx-0.85.1/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/utils.py` & `dvcx-0.85.1/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/webdataset.py` & `dvcx-0.85.1/src/dvcx/lib/webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.85.1/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.85.1/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/listing.py` & `dvcx-0.85.1/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/node.py` & `dvcx-0.85.1/src/dvcx/node.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/nodes_fetcher.py` & `dvcx-0.85.1/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/nodes_thread_pool.py` & `dvcx-0.85.1/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/progress.py` & `dvcx-0.85.1/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/query/batch.py` & `dvcx-0.85.1/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/query/builtins.py` & `dvcx-0.85.1/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/query/dataset.py` & `dvcx-0.85.1/src/dvcx/query/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,15 @@
         insert_q = temp_table.insert().from_select(
             source_query.selected_columns, diff_q
         )
 
         self.catalog.warehouse.db.execute(insert_q)
 
         def q(*columns):
-            return sqlalchemy.select(*columns).select_from(temp_table)
+            return sqlalchemy.select(*columns)
 
         return step_result(q, temp_table.c)
 
 
 @frozen
 class Subtract(DatasetDiffOperation):
     """
@@ -622,15 +622,14 @@
         if self.partition_by is not None:
             partition_tbl = self.create_partitions_table(query)
             temp_tables.append(partition_tbl.name)
 
             subq = query.subquery()
             query = (
                 sqlalchemy.select(*subq.c)
-                .select_from(subq)
                 .outerjoin(partition_tbl, partition_tbl.c.id == subq.c.id)
                 .add_columns(*partition_columns())
             )
 
         query, tables = self.process_input_query(query)
         for t in tables:
             temp_tables.append(t.name)
@@ -679,15 +678,15 @@
         )
         return table
 
     def process_input_query(self, query: Select) -> tuple[Select, list["Table"]]:
         if os.getenv("DVCX_DISABLE_QUERY_CACHE", "") not in ("", "0"):
             return query, []
         table = self.create_pre_udf_table(query)
-        q: Select = sqlalchemy.select(*table.c).select_from(table)
+        q: Select = sqlalchemy.select(*table.c)
         if query._order_by_clauses:
             # we are adding ordering only if it's explicitly added by user in
             # query part before adding signals
             q = q.order_by(table.c.id)
         return q, [table]
 
     def create_result_query(
```

### Comparing `dvcx-0.85.0/src/dvcx/query/dispatch.py` & `dvcx-0.85.1/src/dvcx/query/dispatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,14 +345,15 @@
             for p in pool:
                 p.join()
 
 
 class WorkerCallback(Callback):
     def __init__(self, queue: multiprocess.Queue):
         self.queue = queue
+        super().__init__()
 
     def relative_update(self, inc: int = 1) -> None:
         put_into_queue(self.queue, {"status": NOTIFY_STATUS, "downloaded": inc})
 
 
 @attrs.define
 class UDFWorker:
```

### Comparing `dvcx-0.85.0/src/dvcx/query/params.py` & `dvcx-0.85.1/src/dvcx/query/params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/query/schema.py` & `dvcx-0.85.1/src/dvcx/query/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/query/session.py` & `dvcx-0.85.1/src/dvcx/query/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     def get(
         cls, session: Optional["Session"] = None, catalog: Optional["Catalog"] = None
     ) -> "Session":
         """Creates a Session() object from a catalog.
 
         Parameters:
             `session` (Session): Optional Session(). If not provided a new session will
-                    be created. It's needed mostly for simplie API purpuses.
+                    be created. It's needed mostly for simplie API purposes.
             `catalog` (Catalog): Optional catalog. By default a new catalog is created.
         """
         if session:
             return session
 
         if cls.GLOBAL_SESSION is None:
             cls.GLOBAL_SESSION_CTX = Session(cls.GLOBAL_SESSION_NAME, catalog)
```

### Comparing `dvcx-0.85.0/src/dvcx/query/udf.py` & `dvcx-0.85.1/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/remote/studio.py` & `dvcx-0.85.1/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/sql/default/base.py` & `dvcx-0.85.1/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/sql/functions/array.py` & `dvcx-0.85.1/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/sql/functions/path.py` & `dvcx-0.85.1/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/sql/selectable.py` & `dvcx-0.85.1/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/sql/sqlite/base.py` & `dvcx-0.85.1/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/sql/sqlite/types.py` & `dvcx-0.85.1/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/sql/types.py` & `dvcx-0.85.1/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/sql/utils.py` & `dvcx-0.85.1/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/storage.py` & `dvcx-0.85.1/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx/utils.py` & `dvcx-0.85.1/src/dvcx/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.85.1/src/dvcx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.85.0
+Version: 0.85.1
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.85.0/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.85.1/src/dvcx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/src/dvcx.egg-info/requires.txt` & `dvcx-0.85.1/src/dvcx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/benchmarks/conftest.py` & `dvcx-0.85.1/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/conftest.py` & `dvcx-0.85.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/data.py` & `dvcx-0.85.1/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/func/test_catalog.py` & `dvcx-0.85.1/tests/func/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/func/test_client.py` & `dvcx-0.85.1/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/func/test_dataset_query.py` & `dvcx-0.85.1/tests/func/test_dataset_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/func/test_datasets.py` & `dvcx-0.85.1/tests/func/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/func/test_ls.py` & `dvcx-0.85.1/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/func/test_pull.py` & `dvcx-0.85.1/tests/func/test_pull.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/func/test_pytorch.py` & `dvcx-0.85.1/tests/func/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/func/test_query.py` & `dvcx-0.85.1/tests/func/test_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/scripts/name_len_normal.py` & `dvcx-0.85.1/tests/scripts/name_len_normal.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/scripts/name_len_slow.py` & `dvcx-0.85.1/tests/scripts/name_len_slow.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/test_cli_e2e.py` & `dvcx-0.85.1/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/test_query_e2e.py` & `dvcx-0.85.1/tests/test_query_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/lib/test_cached_stream.py` & `dvcx-0.85.1/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/lib/test_feature.py` & `dvcx-0.85.1/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/lib/test_feature_udf.py` & `dvcx-0.85.1/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/lib/test_file.py` & `dvcx-0.85.1/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/lib/test_image.py` & `dvcx-0.85.1/tests/unit/lib/test_image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/lib/test_reader.py` & `dvcx-0.85.1/tests/unit/lib/test_reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/lib/test_text.py` & `dvcx-0.85.1/tests/unit/lib/test_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/lib/test_webdataset.py` & `dvcx-0.85.1/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.85.1/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/sql/test_array.py` & `dvcx-0.85.1/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/sql/test_conditional.py` & `dvcx-0.85.1/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/sql/test_path.py` & `dvcx-0.85.1/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/sql/test_selectable.py` & `dvcx-0.85.1/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/sql/test_string.py` & `dvcx-0.85.1/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_asyn.py` & `dvcx-0.85.1/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_cache.py` & `dvcx-0.85.1/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_catalog.py` & `dvcx-0.85.1/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_catalog_loader.py` & `dvcx-0.85.1/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_cli_parsing.py` & `dvcx-0.85.1/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_client.py` & `dvcx-0.85.1/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_client_s3.py` & `dvcx-0.85.1/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_data_storage.py` & `dvcx-0.85.1/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_database_engine.py` & `dvcx-0.85.1/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_dataset.py` & `dvcx-0.85.1/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_dataset_row.py` & `dvcx-0.85.1/tests/unit/test_dataset_row.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_dispatch.py` & `dvcx-0.85.1/tests/unit/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_fileslice.py` & `dvcx-0.85.1/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_id_generator.py` & `dvcx-0.85.1/tests/unit/test_id_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 
 from dvcx.data_storage.serializer import deserialize
 from dvcx.data_storage.sqlite import SQLiteDatabaseEngine, SQLiteIDGenerator
 
 
 def get_rows(id_generator):
     uris = id_generator.db.execute(
-        select(id_generator._table.c.uri, id_generator._table.c.last_id).select_from(
-            id_generator._table
-        )
+        select(id_generator._table.c.uri, id_generator._table.c.last_id)
     ).fetchall()
     return set(uris)
 
 
 def test_init(sqlite_db):
     id_generator = SQLiteIDGenerator(sqlite_db)
     assert id_generator.db == sqlite_db
```

### Comparing `dvcx-0.85.0/tests/unit/test_listing.py` & `dvcx-0.85.1/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_metastore.py` & `dvcx-0.85.1/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_query_params.py` & `dvcx-0.85.1/tests/unit/test_query_params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_serializer.py` & `dvcx-0.85.1/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_session.py` & `dvcx-0.85.1/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_storage.py` & `dvcx-0.85.1/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_udf.py` & `dvcx-0.85.1/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_utils.py` & `dvcx-0.85.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/unit/test_warehouse.py` & `dvcx-0.85.1/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.85.0/tests/utils.py` & `dvcx-0.85.1/tests/utils.py`

 * *Files identical despite different names*

