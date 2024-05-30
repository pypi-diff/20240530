# Comparing `tmp/primap2-0.9.7.tar.gz` & `tmp/primap2-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primap2-0.9.7.tar", last modified: Wed May 10 09:55:47 2023, max compression
+gzip compressed data, was "primap2-0.9.8.tar", last modified: Mon Dec  4 10:40:09 2023, max compression
```

## Comparing `primap2-0.9.7.tar` & `primap2-0.9.8.tar`

### file list

```diff
@@ -1,133 +1,136 @@
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.825400 primap2-0.9.7/.github/
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.825400 primap2-0.9.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      671 2023-03-31 17:51:36.000000 primap2-0.9.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      548 2023-03-31 17:51:36.000000 primap2-0.9.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      364 2023-03-31 17:51:36.000000 primap2-0.9.7/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.825400 primap2-0.9.7/.github/workflows/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      955 2023-04-24 13:56:22.000000 primap2-0.9.7/.github/workflows/ci.yml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1340 2023-04-28 09:36:40.000000 primap2-0.9.7/.gitignore
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1197 2023-05-10 09:45:31.000000 primap2-0.9.7/.pre-commit-config.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      406 2023-04-28 09:36:40.000000 primap2-0.9.7/.readthedocs.yml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      173 2023-04-28 09:36:40.000000 primap2-0.9.7/AUTHORS.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5678 2023-05-10 09:46:07.000000 primap2-0.9.7/CHANGELOG.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1608 2023-03-31 17:51:36.000000 primap2-0.9.7/CONTRIBUTING.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11357 2023-03-31 17:51:36.000000 primap2-0.9.7/LICENSE
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2880 2023-05-10 09:55:38.000000 primap2-0.9.7/Makefile
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8917 2023-05-10 09:55:47.829400 primap2-0.9.7/PKG-INFO
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2284 2023-05-10 09:49:45.000000 primap2-0.9.7/README.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      167 2023-03-31 17:51:36.000000 primap2-0.9.7/TODO.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      130 2023-03-31 17:51:36.000000 primap2-0.9.7/codecov.yml
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.825400 primap2-0.9.7/docs/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      620 2023-04-04 07:09:04.000000 primap2-0.9.7/docs/Makefile
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.825400 primap2-0.9.7/docs/_static/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       28 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/_static/custom.css
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1796 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/api.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/changelog.rst
--rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5210 2023-04-24 13:56:22.000000 primap2-0.9.7/docs/conf.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      356 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/credits.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8297 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_format_details.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14060 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_format_examples.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3891 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading.rst
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/docs/data_reading_writing_examples/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      105 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading_writing_examples/.gitignore
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    33106 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading_writing_examples/FAOstat.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    44497 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading_writing_examples/PRIMAP-hist.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      199 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading_writing_examples/test_csv_data_long.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      432 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading_writing_examples/test_csv_data_sec_cat.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1201 2023-04-28 07:59:57.000000 primap2-0.9.7/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      332 2023-04-28 07:59:57.000000 primap2-0.9.7/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5669 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading_writing_examples/test_data_long.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5774 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading_writing_examples/test_data_wide.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1538 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/datalad.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    19051 2023-04-28 09:36:09.000000 primap2-0.9.7/docs/development.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      436 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/index.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1106 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/installation.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4579 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/interchange_format_details.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11376 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/interchange_format_examples.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      769 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/make.bat
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    15032 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/minimal_ds.nc
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   543680 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/opulent_ds.nc
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      292 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/pm2io.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/readme.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      111 2023-04-04 07:21:47.000000 primap2-0.9.7/docs/requirements.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    28635 2023-04-04 07:21:47.000000 primap2-0.9.7/docs/usage.ipynb
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/licenses/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      565 2023-03-31 17:51:36.000000 primap2-0.9.7/licenses/pint_xarray_license
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      565 2023-03-31 17:51:36.000000 primap2-0.9.7/licenses/xarray_license
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       64 2023-03-31 17:51:36.000000 primap2-0.9.7/mypy.ini
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2261 2023-04-04 07:21:47.000000 primap2-0.9.7/primap-stubs.patch
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/primap2/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      304 2023-05-10 09:45:47.000000 primap2-0.9.7/primap2/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      327 2023-04-25 14:13:52.000000 primap2-0.9.7/primap2/_accessor_base.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21858 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/_aggregate.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9076 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/_alias_selection.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18227 2023-05-10 09:15:27.000000 primap2-0.9.7/primap2/_data_format.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    12288 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/_downscale.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9246 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/_merge.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2720 2023-04-25 13:24:13.000000 primap2-0.9.7/primap2/_metadata.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5656 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/_overview.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    23888 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/_setters.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      423 2023-04-25 13:05:58.000000 primap2-0.9.7/primap2/_types.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11482 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/_units.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1508 2023-04-25 13:14:07.000000 primap2-0.9.7/primap2/accessors.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/primap2/pm2io/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6332 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/pm2io/_GHG_inventory_reading.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      728 2023-05-10 09:15:27.000000 primap2-0.9.7/primap2/pm2io/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    13487 2023-04-25 15:48:53.000000 primap2-0.9.7/primap2/pm2io/_conversion.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    61245 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/pm2io/_data_reading.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    13953 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/pm2io/_interchange_format.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/primap2/tests/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       79 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1640 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/conftest.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/primap2/tests/data/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2999 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21056 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.nc
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      701 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      199 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/long.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       84 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/long_no_time.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       87 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_csv_data.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      113 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_csv_data_category_name.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      109 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_csv_data_category_name_fill_cat_code.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      231 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_csv_data_category_name_long.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      432 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_csv_data_sec_cat.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      434 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_csv_data_sec_cat_strings.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14880 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_from_interchange_format_output.nc
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      198 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_read_wide_csv_file_no_sec_cats.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      224 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_read_wide_csv_file_no_sec_cats_cat_name.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      446 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_read_wide_csv_file_output.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      492 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_read_wide_csv_file_output_entity_def.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      328 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_read_wide_csv_file_output_unit_def.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    90672 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_sum_skip_allna_inhomogeneous_result.nc
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6126 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/examples.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11731 2023-05-10 09:45:31.000000 primap2-0.9.7/primap2/tests/test_aggregate.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2988 2023-04-28 08:57:53.000000 primap2-0.9.7/primap2/tests/test_alias_selection.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5501 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/test_conversion.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11752 2023-05-10 09:15:27.000000 primap2-0.9.7/primap2/tests/test_data_format.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    37510 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/tests/test_data_reading.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6827 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/test_downscale.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1737 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/test_interchange_format.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3597 2023-04-04 07:21:47.000000 primap2-0.9.7/primap2/tests/test_merge.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1384 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/test_metadata.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6107 2023-04-28 08:58:51.000000 primap2-0.9.7/primap2/tests/test_overview.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    17597 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/tests/test_setters.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2621 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/test_units.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1911 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/tests/utils.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/primap2.egg-info/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8917 2023-05-10 09:55:47.000000 primap2-0.9.7/primap2.egg-info/PKG-INFO
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3607 2023-05-10 09:55:47.000000 primap2-0.9.7/primap2.egg-info/SOURCES.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-05-10 09:55:47.000000 primap2-0.9.7/primap2.egg-info/dependency_links.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      415 2023-05-10 09:55:47.000000 primap2-0.9.7/primap2.egg-info/requires.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        8 2023-05-10 09:55:47.000000 primap2-0.9.7/primap2.egg-info/top_level.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      322 2023-04-28 09:36:40.000000 primap2-0.9.7/pyproject.toml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-03-31 17:51:36.000000 primap2-0.9.7/requirements.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-03-31 17:51:36.000000 primap2-0.9.7/requirements_dev.txt
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/rosetta/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4711 2023-03-31 17:51:36.000000 primap2-0.9.7/rosetta/combine_rows-set.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1696 2023-05-10 09:55:47.829400 primap2-0.9.7/setup.cfg
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-03-31 17:51:36.000000 primap2-0.9.7/setup.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1315 2023-05-10 09:45:47.000000 primap2-0.9.7/tbump.toml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      379 2023-04-24 13:56:22.000000 primap2-0.9.7/tox.ini
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      706 2023-03-31 17:51:36.000000 primap2-0.9.7/update_changelog.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1147 2023-03-31 17:51:36.000000 primap2-0.9.7/update_citation_info.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-12-04 10:40:09.590957 primap2-0.9.8/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      387 2023-11-14 15:48:17.000000 primap2-0.9.8/.check_python_version.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-12-04 10:40:09.582956 primap2-0.9.8/.github/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-12-04 10:40:09.582956 primap2-0.9.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      671 2023-03-31 17:51:36.000000 primap2-0.9.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      548 2023-03-31 17:51:36.000000 primap2-0.9.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      364 2023-03-31 17:51:36.000000 primap2-0.9.8/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-12-04 10:40:09.582956 primap2-0.9.8/.github/workflows/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      955 2023-11-14 15:48:17.000000 primap2-0.9.8/.github/workflows/ci.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1340 2023-11-14 15:48:17.000000 primap2-0.9.8/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1192 2023-12-04 10:13:38.000000 primap2-0.9.8/.pre-commit-config.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      383 2023-11-14 15:48:17.000000 primap2-0.9.8/.readthedocs.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      173 2023-11-14 15:48:17.000000 primap2-0.9.8/AUTHORS.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6014 2023-12-04 10:16:56.000000 primap2-0.9.8/CHANGELOG.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1608 2023-03-31 17:51:36.000000 primap2-0.9.8/CONTRIBUTING.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11357 2023-03-31 17:51:36.000000 primap2-0.9.8/LICENSE
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3046 2023-11-14 15:48:17.000000 primap2-0.9.8/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    10690 2023-12-04 10:40:09.590957 primap2-0.9.8/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2285 2023-12-04 10:39:50.000000 primap2-0.9.8/README.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      167 2023-03-31 17:51:36.000000 primap2-0.9.8/TODO.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      130 2023-03-31 17:51:36.000000 primap2-0.9.8/codecov.yml
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-12-04 10:40:09.586956 primap2-0.9.8/docs/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      620 2023-04-04 07:09:04.000000 primap2-0.9.8/docs/Makefile
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-12-04 10:40:09.586956 primap2-0.9.8/docs/_static/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       28 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/_static/custom.css
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1796 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/api.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/changelog.rst
+-rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5210 2023-11-14 15:48:17.000000 primap2-0.9.8/docs/conf.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      356 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/credits.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8297 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/data_format_details.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14060 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/data_format_examples.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3891 2023-11-14 15:47:31.000000 primap2-0.9.8/docs/data_reading.rst
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-12-04 10:40:09.586956 primap2-0.9.8/docs/data_reading_writing_examples/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      105 2023-11-14 15:47:31.000000 primap2-0.9.8/docs/data_reading_writing_examples/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    33106 2023-11-14 15:47:31.000000 primap2-0.9.8/docs/data_reading_writing_examples/FAOstat.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    44497 2023-11-14 15:47:31.000000 primap2-0.9.8/docs/data_reading_writing_examples/PRIMAP-hist.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      199 2023-11-14 15:47:31.000000 primap2-0.9.8/docs/data_reading_writing_examples/test_csv_data_long.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      432 2023-11-14 15:47:31.000000 primap2-0.9.8/docs/data_reading_writing_examples/test_csv_data_sec_cat.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1201 2023-11-14 15:47:31.000000 primap2-0.9.8/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      332 2023-11-14 15:47:31.000000 primap2-0.9.8/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5669 2023-11-14 15:47:31.000000 primap2-0.9.8/docs/data_reading_writing_examples/test_data_long.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5774 2023-11-14 15:47:31.000000 primap2-0.9.8/docs/data_reading_writing_examples/test_data_wide.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1538 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/datalad.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18725 2023-11-14 15:48:17.000000 primap2-0.9.8/docs/development.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      436 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/index.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1106 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/installation.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4579 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/interchange_format_details.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11376 2023-11-14 15:47:31.000000 primap2-0.9.8/docs/interchange_format_examples.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      769 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/make.bat
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    15032 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/minimal_ds.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   543680 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/opulent_ds.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      292 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/pm2io.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-03-31 17:51:36.000000 primap2-0.9.8/docs/readme.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      111 2023-11-14 15:47:31.000000 primap2-0.9.8/docs/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    29565 2023-11-14 15:48:17.000000 primap2-0.9.8/docs/usage.ipynb
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-12-04 10:40:09.586956 primap2-0.9.8/licenses/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      565 2023-03-31 17:51:36.000000 primap2-0.9.8/licenses/pint_xarray_license
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      565 2023-03-31 17:51:36.000000 primap2-0.9.8/licenses/xarray_license
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       64 2023-03-31 17:51:36.000000 primap2-0.9.8/mypy.ini
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2261 2023-12-04 10:13:38.000000 primap2-0.9.8/primap-stubs.patch
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-12-04 10:40:09.586956 primap2-0.9.8/primap2/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      304 2023-12-04 10:16:31.000000 primap2-0.9.8/primap2/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      327 2023-04-25 14:13:52.000000 primap2-0.9.8/primap2/_accessor_base.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    25451 2023-12-04 10:13:38.000000 primap2-0.9.8/primap2/_aggregate.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9113 2023-12-04 10:13:38.000000 primap2-0.9.8/primap2/_alias_selection.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18227 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/_data_format.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    15168 2023-12-04 10:13:38.000000 primap2-0.9.8/primap2/_downscale.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9327 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/_merge.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2720 2023-04-25 13:24:13.000000 primap2-0.9.8/primap2/_metadata.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5656 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/_overview.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    23888 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/_setters.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      423 2023-04-25 13:05:58.000000 primap2-0.9.8/primap2/_types.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11482 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/_units.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1508 2023-12-04 10:13:38.000000 primap2-0.9.8/primap2/accessors.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-12-04 10:40:09.586956 primap2-0.9.8/primap2/pm2io/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6332 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/pm2io/_GHG_inventory_reading.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      728 2023-05-10 09:15:27.000000 primap2-0.9.8/primap2/pm2io/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    13515 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/pm2io/_conversion.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    65653 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/pm2io/_data_reading.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    13950 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/pm2io/_interchange_format.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-12-04 10:40:09.586956 primap2-0.9.8/primap2/tests/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       79 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1626 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/tests/conftest.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-12-04 10:40:09.586956 primap2-0.9.8/primap2/tests/data/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2999 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21056 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      701 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      199 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/long.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       84 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/long_no_time.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       87 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/test_csv_data.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      113 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/test_csv_data_category_name.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      109 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/test_csv_data_category_name_fill_cat_code.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      231 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/test_csv_data_category_name_long.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      432 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/test_csv_data_sec_cat.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      434 2023-11-14 15:47:31.000000 primap2-0.9.8/primap2/tests/data/test_csv_data_sec_cat_strings.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      164 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/tests/data/test_csv_data_unit_harmonization.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14880 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/test_from_interchange_format_output.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      198 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/test_read_wide_csv_file_no_sec_cats.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      224 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/test_read_wide_csv_file_no_sec_cats_cat_name.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      446 2023-11-14 15:47:31.000000 primap2-0.9.8/primap2/tests/data/test_read_wide_csv_file_output.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      492 2023-11-14 15:47:31.000000 primap2-0.9.8/primap2/tests/data/test_read_wide_csv_file_output_entity_def.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      328 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/test_read_wide_csv_file_output_unit_def.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      298 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/tests/data/test_read_wide_csv_file_output_unit_harm.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    90672 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/data/test_sum_skip_allna_inhomogeneous_result.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6126 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/examples.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    13328 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/tests/test_aggregate.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2988 2023-04-28 08:57:53.000000 primap2-0.9.8/primap2/tests/test_alias_selection.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5501 2023-11-14 15:47:31.000000 primap2-0.9.8/primap2/tests/test_conversion.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11752 2023-05-10 09:15:27.000000 primap2-0.9.8/primap2/tests/test_data_format.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    38578 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/tests/test_data_reading.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     7276 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/tests/test_downscale.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1737 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/test_interchange_format.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3597 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/tests/test_merge.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1384 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/test_metadata.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6058 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/tests/test_overview.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    17597 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/tests/test_setters.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2621 2023-03-31 17:51:36.000000 primap2-0.9.8/primap2/tests/test_units.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1911 2023-11-14 15:48:17.000000 primap2-0.9.8/primap2/tests/utils.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-12-04 10:40:09.586956 primap2-0.9.8/primap2.egg-info/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    10690 2023-12-04 10:40:09.000000 primap2-0.9.8/primap2.egg-info/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3752 2023-12-04 10:40:09.000000 primap2-0.9.8/primap2.egg-info/SOURCES.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-12-04 10:40:09.000000 primap2-0.9.8/primap2.egg-info/dependency_links.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      415 2023-12-04 10:40:09.000000 primap2-0.9.8/primap2.egg-info/requires.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        8 2023-12-04 10:40:09.000000 primap2-0.9.8/primap2.egg-info/top_level.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      322 2023-11-14 15:48:17.000000 primap2-0.9.8/pyproject.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-03-31 17:51:36.000000 primap2-0.9.8/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-03-31 17:51:36.000000 primap2-0.9.8/requirements_dev.txt
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-12-04 10:40:09.586956 primap2-0.9.8/rosetta/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4711 2023-03-31 17:51:36.000000 primap2-0.9.8/rosetta/combine_rows-set.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1696 2023-12-04 10:40:09.590957 primap2-0.9.8/setup.cfg
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-03-31 17:51:36.000000 primap2-0.9.8/setup.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1315 2023-12-04 10:16:31.000000 primap2-0.9.8/tbump.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      379 2023-11-14 15:48:17.000000 primap2-0.9.8/tox.ini
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      706 2023-03-31 17:51:36.000000 primap2-0.9.8/update_changelog.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1147 2023-03-31 17:51:36.000000 primap2-0.9.8/update_citation_info.py
```

### Comparing `primap2-0.9.7/.github/ISSUE_TEMPLATE/bug_report.md` & `primap2-0.9.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/.github/ISSUE_TEMPLATE/feature_request.md` & `primap2-0.9.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/.github/workflows/ci.yml` & `primap2-0.9.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/.gitignore` & `primap2-0.9.8/.gitignore`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/.pre-commit-config.yaml` & `primap2-0.9.8/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: 'v4.4.0'
+    rev: 'v4.5.0'
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
       - id: check-ast
       - id: fix-byte-order-marker
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: detect-private-key
       - id: mixed-line-ending
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: 'v0.0.265'
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: 'v0.1.6'
     hooks:
       - id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
   - repo: https://github.com/psf/black
-    rev: '23.3.0'
+    rev: '23.11.0'
     hooks:
       - id: black
   - repo: https://github.com/keewis/blackdoc
-    rev: v0.3.8
+    rev: v0.3.9
     hooks:
       - id: blackdoc
   - repo: https://github.com/PyCQA/doc8
     rev: 'v1.1.1'
     hooks:
       - id: doc8
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: '1.7.0'
+    rev: '1.7.1'
     hooks:
       - id: nbqa-black
         args: [ --nbqa-mutate, --line-length=75 ]
       - id: nbqa-check-ast
   - repo: https://github.com/asottile/blacken-docs
-    rev: '1.13.0'
+    rev: '1.16.0'
     hooks:
       - id: blacken-docs
```

### Comparing `primap2-0.9.7/CHANGELOG.rst` & `primap2-0.9.8/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 =========
 Changelog
 =========
 
+0.9.8
+-----
+* add additional control over nan treatment to downscaling functionality
+* Allow kwargs in gas basket summation
+* use min_count=1 as default in pr.sum
+* fix error message for 0-dimensional arrays in pr.merge
+* fix building the documentation on readthedocs.org
+* Modify unit harmonization to return native units if possible
+
 0.9.7
 -----
 * Fix the test suite to work with Pint release 0.21.
 
 0.9.6
 -----
 * Add dependency on openscm_units > 0.5.1 for compatibility with latest pandas.
```

### Comparing `primap2-0.9.7/CONTRIBUTING.rst` & `primap2-0.9.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/LICENSE` & `primap2-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/Makefile` & `primap2-0.9.8/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.PHONY: clean clean-test clean-pyc clean-build docs help virtual-environment install-pre-commit stubs update-venv README.rst
+.PHONY: clean clean-test clean-pyc clean-build docs help virtual-environment install-pre-commit stubs update-venv README.rst check-python-version
 .DEFAULT_GOAL := help
 
 define PRINT_HELP_PYSCRIPT
 import re, sys
 
 for line in sys.stdin:
 	match = re.match(r'^([a-zA-Z_-]+):.*?## (.*)$$', line)
@@ -68,21 +68,23 @@
 
 install: clean ## install the package to the active Python's site-packages
 	python setup.py install
 
 virtual-environment: venv ## setup a virtual environment for development
 
 venv: requirements_dev.txt setup.cfg
+	[ -d venv ] || python3 .check_python_version.py
 	[ -d venv ] || python3 -m venv venv
 	venv/bin/python -m pip install --upgrade pip wheel
 	venv/bin/python -m pip install --upgrade -e .[dev]
 	touch venv
 
-update-venv:
+update-venv: ## update all packages in the development environment
 	[ -d venv ] || python3 -m venv venv
+	venv/bin/python .check_python_version.py
 	venv/bin/python -m pip install --upgrade pip wheel
 	venv/bin/python -m pip install --upgrade --upgrade-strategy eager -e .[dev]
 	touch venv
 
 install-pre-commit: update-venv ## install the pre-commit hooks
 	venv/bin/pre-commit install
```

### Comparing `primap2-0.9.7/README.rst` & `primap2-0.9.8/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 Apache License, Version 2.0 as well. The full text of the xarray copyright statement is
 included in the licenses directory.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger and Johannes Gütschow. (2023-05-10).
-pik-primap/primap2: PRIMAP2 Version 0.9.7.
-Zenodo. https://doi.org/10.5281/zenodo.7919586
+Mika Pflüger and Johannes Gütschow. (2023-12-04).
+pik-primap/primap2: PRIMAP2 Version 0.9.8.
+Zenodo. https://doi.org/10.5281/zenodo.10254997
```

### Comparing `primap2-0.9.7/docs/Makefile` & `primap2-0.9.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/api.rst` & `primap2-0.9.8/docs/api.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/conf.py` & `primap2-0.9.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/data_format_details.rst` & `primap2-0.9.8/docs/data_format_details.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/data_format_examples.ipynb` & `primap2-0.9.8/docs/data_format_examples.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/data_reading.rst` & `primap2-0.9.8/docs/data_reading.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/data_reading_writing_examples/FAOstat.ipynb` & `primap2-0.9.8/docs/data_reading_writing_examples/FAOstat.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/data_reading_writing_examples/PRIMAP-hist.ipynb` & `primap2-0.9.8/docs/data_reading_writing_examples/PRIMAP-hist.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.csv` & `primap2-0.9.8/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.csv`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/data_reading_writing_examples/test_data_long.ipynb` & `primap2-0.9.8/docs/data_reading_writing_examples/test_data_long.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/data_reading_writing_examples/test_data_wide.ipynb` & `primap2-0.9.8/docs/data_reading_writing_examples/test_data_wide.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/datalad.rst` & `primap2-0.9.8/docs/datalad.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/development.rst` & `primap2-0.9.8/docs/development.rst`

 * *Files 3% similar despite different names*

```diff
@@ -359,27 +359,23 @@
    to ``Numpy``.
 4. If you want to run tests in pycharm instead of the terminal using ``make test``,
    you can add a configuration at
    ``Run | Edit configurations | + | python tests | pytest``.
    Afterwards, you can run the tests by selecting this configuration at the top right
    bar and clicking on the "run" or "run with coverage" icons.
 5. If you want to run the ``black`` code formatter from PyCharm, look at their
-   `howto <https://black.readthedocs.io/en/stable/editor_integration.html#pycharm-intellij-idea>`_.
+   `howto <https://black.readthedocs.io/en/stable/integrations/editors.html#pycharm-intellij-idea>`_.
 6. A couple of plugins can be useful in PyCharm for PRIMAP2 development:
 
    * `Makefile support <https://plugins.jetbrains.com/plugin/9333-makefile-language>`_
       to run Makefile targets directly from PyCharm
    * `CSV Plugin <https://plugins.jetbrains.com/plugin/10037-csv-plugin>`_
       to view and edit CSV files
    * `Matlab support <https://plugins.jetbrains.com/plugin/10941-matlab-support>`_
       to quickly view .m files without starting matlab
-   * `Diff/patch file support <https://plugins.jetbrains.com/plugin/11957-diff--patch-file-support>`_
-      for syntax highlighting of patch files (currently only used for stub generation)
-   * `Requirements <https://plugins.jetbrains.com/plugin/10837-requirements>`_
-      for managing requirements_dev.txt from within PyCharm
    * `Toml <https://plugins.jetbrains.com/plugin/8195-toml>`_
       for editing pyproject.toml
    * `.ignore <https://plugins.jetbrains.com/plugin/7495--ignore>`_
       for better support of ``.gitignore``
 
 Deploying
 ---------
```

### Comparing `primap2-0.9.7/docs/installation.rst` & `primap2-0.9.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/interchange_format_details.rst` & `primap2-0.9.8/docs/interchange_format_details.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/interchange_format_examples.ipynb` & `primap2-0.9.8/docs/interchange_format_examples.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/make.bat` & `primap2-0.9.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/minimal_ds.nc` & `primap2-0.9.8/docs/minimal_ds.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/opulent_ds.nc` & `primap2-0.9.8/docs/opulent_ds.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/docs/usage.ipynb` & `primap2-0.9.8/docs/usage.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9980695576970595%*

 * *Differences: {"'cells'": "{47: {'source': {insert: [(8, 'while ignoring only those categories which are missing "*

 * *            "completely.\\n'), (9, 'It is also possible to ignore NA values (i.e. treating them as "*

 * *            "0) in sums using \\n'), (10, 'the `skipna` parameter. \\n'), (11, 'When using "*

 * *            "`skipna`, the `min_count` parameter governs how many non-NA vales are \\n'), (12, "*

 * *            "'needed in a sum for the result to be non-NA. The default value is `skipna=1`. \\n'), "*

 * *            "(13, ' […]*

```diff
@@ -816,15 +816,24 @@
                 "\n",
                 "xarray provides robust functions for aggregation (`sum`) and filling of\n",
                 "missing information (`fillna`).\n",
                 "PRIMAP2 adds functions which fill or skip missing information based on if the\n",
                 "information is missing at all points along certain axes, for example for\n",
                 "a whole time series.\n",
                 "This makes it possible to, for example, evaluate the sum of sub-categories\n",
-                "while ignoring only those categories which are missing completely."
+                "while ignoring only those categories which are missing completely.\n",
+                "It is also possible to ignore NA values (i.e. treating them as 0) in sums using \n",
+                "the `skipna` parameter. \n",
+                "When using `skipna`, the `min_count` parameter governs how many non-NA vales are \n",
+                "needed in a sum for the result to be non-NA. The default value is `skipna=1`. \n",
+                "This is helpful if you want to e.g. sum all subsectors and for some countries \n",
+                "or gases some of the subsectors have NA values because there is no data. To avoid\n",
+                "NA timeseries if a single sector is NA you use `skipna`. In other cases, e.g. when \n",
+                "checking if data coverage is complete `skipna` is not used, so any NA value in the \n",
+                "source data results in NA in the summed data and is not hidden. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "pycharm": {
@@ -861,14 +870,25 @@
                 "da.pr.sum(dim=\"area\", skipna_evaluation_dims=\"time\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "da.pr.sum(dim=\"area\", skipna=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
                 "# compare this to the result of the standard xarray sum:\n",
```

### Comparing `primap2-0.9.7/licenses/pint_xarray_license` & `primap2-0.9.8/licenses/pint_xarray_license`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/licenses/xarray_license` & `primap2-0.9.8/licenses/xarray_license`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap-stubs.patch` & `primap2-0.9.8/primap-stubs.patch`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/_aggregate.py` & `primap2-0.9.8/primap2/_aggregate.py`

 * *Files 7% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         self,
         dim: Optional[DimOrDimsT] = None,
         *,
         reduce_to_dim: Optional[DimOrDimsT] = None,
         skipna: Optional[bool] = None,
         skipna_evaluation_dims: Optional[DimOrDimsT] = None,
         keep_attrs: bool = True,
-        **kwargs,
+        min_count: Optional[int] = None,
     ) -> xr.DataArray:
         """Reduce this DataArray's data by applying `sum` along some dimension(s).
 
         By default, works like da.sum(), but has additional features:
 
         1. Dimension aliases can be used instead of full dimension names everywhere.
         2. Instead of specifying the dimension(s) to reduce via ``dim``, you can specify
@@ -128,14 +128,17 @@
            `sum` will be applied along all other dimensions.
         3. You can specify ``skipna_evaluation_dims`` to skip NA values only if all
            values along the given dimension(s) are NA. Example: If you have a data array
            with the dimensions ``time`` and ``position``, summing over ``time`` with the
            evaluation dimension ``position`` will skip only those values where all
            values with the same ``position`` are NA.
 
+        ``skipna`` and ``min_count`` work like in the :py:func:`xr.sum` function. The behaviour
+        of primap1 is reproduced by ``skipna=True, min_count=1``.
+
         Parameters
         ----------
         dim: str or list of str, optional
           Dimension(s) over which to apply `sum`. Only one of ``dim`` and
           ``reduce_to_dim`` arguments can be supplied. If neither is supplied, then
           the sum is calculated over all dimensions.
         reduce_to_dim: str or list of str, optional
@@ -151,16 +154,24 @@
           Dimension(s) to evaluate along to determine if values should be skipped.
           Only one of ``skipna`` and ``skipna_evaluation_dims`` can be supplied.
           If all values along the specified dimensions are NA, the values are skipped,
           other NA values are not skipped and will lead to NA in the corresponding
           result.
         keep_attrs: bool, optional
           Keep the attr metadata (default True).
-        **kwargs: dict
-          Additional keyword arguments are passed directly to xarray's da.sum().
+        min_count: int (default None, but set to 1 if skipna=True)
+          The minimal number of non-NA values in a sum that is necessary for a non-NA
+          result. This only has an effect if ``skipna=True``. As an example: you sum data
+          for a region for a certain sector, gas and year. If ``skipna=False``,
+          all countries in the region need to have non-NA data for that sector, gas,
+          year combination. If ``skipna=True`` and ``min_count=1`` then one country with
+          non-NA data is enough for a non-NA result. All NA values will be treated as
+          zero. If ``min_count=0`` all NA values will be treated as zero
+          also if there is no single non-NA value in the data that is to be summed.
+
 
         Returns
         -------
         summed : xr.DataArray
         """
         dim = self._reduce_dim(dim, reduce_to_dim)
 
@@ -171,16 +182,21 @@
             )
 
         if skipna_evaluation_dims is not None:
             skipna = False
             da = self.fill_all_na(dim=skipna_evaluation_dims, value=0)
         else:
             da = self._da
+            if skipna:
+                if min_count is None:
+                    min_count = 1
 
-        return da.sum(dim=dim, skipna=skipna, keep_attrs=keep_attrs, **kwargs)
+        return da.sum(
+            dim=dim, skipna=skipna, keep_attrs=keep_attrs, min_count=min_count
+        )
 
     @alias_dims(["dim"])
     def fill_all_na(self, dim: Union[Iterable[Hashable], str], value=0) -> xr.DataArray:
         """Fill NA values only where all values along the specified dimension(s) are NA.
 
         Example: having a data array with dimensions ``time`` and ``position``,
         filling it along ``time`` will only fill those values where all points that
@@ -336,15 +352,15 @@
         self,
         dim: Optional[DimOrDimsT] = None,
         *,
         reduce_to_dim: Optional[DimOrDimsT] = None,
         skipna: Optional[bool] = None,
         skipna_evaluation_dims: Optional[DimOrDimsT] = None,
         keep_attrs: bool = True,
-        **kwargs,
+        min_count: Optional[int] = None,
     ) -> DatasetOrDataArray:
         """Reduce this Dataset's data by applying `sum` along some dimension(s).
 
         By default, works like ds.sum(), but has additional features:
 
         1. Dimension aliases can be used instead of full dimension names everywhere.
         2. Instead of specifying the dimension(s) to reduce via ``dim``, you can specify
@@ -355,14 +371,17 @@
            with the dimensions ``time`` and ``position``, summing over ``time`` with the
            evaluation dimension ``position`` will skip only those values where all
            values with the same ``position`` are NA.
         4. If you specify ``entity`` in "dim", the Dataset is converted to a DataArray
            and summed along the data variables (which will only work if the units of
            the DataArrays are compatible).
 
+        ``skipna`` and ``min_count`` work like in the :py:func:`xr.sum` function. The behaviour
+        of primap1 is reproduced by ``skipna=True, min_count=1``.
+
         Parameters
         ----------
         dim: str or list of str, optional
           Dimension(s) over which to apply `sum`. Only one of ``dim`` and
           ``reduce_to_dim`` arguments can be supplied. If neither is supplied, then
           the sum is calculated over all dimensions. Use "entity" to convert to a
           DataArray and sum along the data variables.
@@ -380,16 +399,23 @@
           Dimension(s) to evaluate along to determine if values should be skipped.
           Only one of ``skipna`` and ``skipna_evaluation_dims`` can be supplied.
           If all values along the specified dimensions are NA, the values are skipped,
           other NA values are not skipped and will lead to NA in the corresponding
           result.
         keep_attrs: bool, optional
           Keep the attr metadata (default True).
-        **kwargs: dict
-          Additional keyword arguments are passed directly to xarray's da.sum().
+        min_count: int (default None, but set to 1 if skipna=True)
+          The minimal number of non-NA values in a sum that is necessary for a non-NA
+          result. This only has an effect if ``skipna=True``. As an example: you sum data
+          for a region for a certain sector, gas and year. If ``skipna=False``,
+          all countries in the region need to have non-NA data for that sector, gas,
+          year combination. If ``skipna=True`` and ``min_count=1`` then one country with
+          non-NA data is enough for a non-NA result. All NA values will be treated as
+          zero. If ``min_count=0`` all NA values will be treated as zero
+          also if there is no single non-NA value in the data that is to be summed.
 
         Returns
         -------
         summed : xr.DataArray
         """
         dim = self._reduce_dim(dim, reduce_to_dim)
 
@@ -400,38 +426,46 @@
             )
 
         if skipna_evaluation_dims is not None:
             skipna = False
             ds = self.fill_all_na(dim=skipna_evaluation_dims, value=0)
         else:
             ds = self._ds
+            if skipna:
+                if min_count is None:
+                    min_count = 1
 
         if dim is not None and "entity" in dim:
             ndim = set(dim) - {"entity"}
 
-            ds = ds.sum(dim=ndim, skipna=skipna, keep_attrs=keep_attrs, **kwargs)
+            ds = ds.sum(
+                dim=ndim, skipna=skipna, keep_attrs=keep_attrs, min_count=min_count
+            )
 
             if not ds.pr._all_vars_all_dimensions():
                 raise NotImplementedError(
                     "Summing along the entity dimension is only supported "
                     "when all entities share the dimensions remaining after summing."
                 )
             return ds.to_array("entity").sum(
-                dim="entity", skipna=skipna, keep_attrs=keep_attrs, **kwargs
+                dim="entity", skipna=skipna, keep_attrs=keep_attrs, min_count=min_count
             )
         else:
-            return ds.sum(dim=dim, skipna=skipna, keep_attrs=keep_attrs, **kwargs)
+            return ds.sum(
+                dim=dim, skipna=skipna, keep_attrs=keep_attrs, min_count=min_count
+            )
 
     def gas_basket_contents_sum(
         self,
         *,
         basket: str,
         basket_contents: Sequence[str],
         skipna: Optional[bool] = None,
         skipna_evaluation_dims: Optional[DimOrDimsT] = None,
+        min_count: Optional[int] = None,
     ) -> xr.DataArray:
         """The sum of gas basket contents converted using the global warming potential
         of the gas basket.
 
         Parameters
         ----------
         basket: str
@@ -446,14 +480,23 @@
           implemented (object, datetime64 or timedelta64).
         skipna_evaluation_dims: str or list of str, optional
           Dimension(s) to evaluate along to determine if values should be skipped.
           Only one of ``skipna`` and ``skipna_evaluation_dims`` can be supplied.
           If all values along the specified dimensions are NA, the values are skipped,
           other NA values are not skipped and will lead to NA in the corresponding
           result.
+        min_count: int (default None, but set to 1 if skipna=True)
+          The minimal number of non-NA values in a sum that is necessary for a non-NA
+          result. This only has an effect if ``skipna=True``. As an example: you sum data
+          for a region for a certain sector, gas and year. If ``skipna=False``,
+          all countries in the region need to have non-NA data for that sector, gas,
+          year combination. If ``skipna=True`` and ``min_count=1`` then one country with
+          non-NA data is enough for a non-NA result. All NA values will be treated as
+          zero. If ``min_count=0`` all NA values will be treated as zero
+          also if there is no single non-NA value in the data that is to be summed.
 
         Returns
         -------
         summed : xr.DataArray
         """
 
         basket_contents_converted = xr.Dataset()
@@ -462,28 +505,30 @@
             da: xr.DataArray = self._ds[var]
             basket_contents_converted[var] = da.pr.convert_to_gwp_like(like=basket_da)
 
         da = basket_contents_converted.pr.sum(
             dim="entity",
             skipna_evaluation_dims=skipna_evaluation_dims,
             skipna=skipna,
+            min_count=min_count,
         )
         da.attrs["gwp_context"] = basket_da.attrs["gwp_context"]
         da.attrs["entity"] = basket_da.attrs["entity"]
         da.name = basket_da.name
         return da
 
     def fill_na_gas_basket_from_contents(
         self,
         *,
         basket: str,
         basket_contents: Sequence[str],
         sel: Optional[Mapping[Hashable, Sequence]] = None,
         skipna: Optional[bool] = None,
         skipna_evaluation_dims: Optional[DimOrDimsT] = None,
+        min_count: Optional[int] = None,
     ) -> xr.DataArray:
         """Fill NA values in a gas basket using the sum of its contents.
 
         To calculate the sum of the gas basket contents, the global warming potential
         context defined on the gas basket will be used.
 
         Parameters
@@ -504,21 +549,31 @@
           implemented (object, datetime64 or timedelta64).
         skipna_evaluation_dims: str or list of str, optional
           Dimension(s) to evaluate along to determine if values should be skipped.
           Only one of ``skipna`` and ``skipna_evaluation_dims`` can be supplied.
           If all values along the specified dimensions are NA, the values are skipped,
           other NA values are not skipped and will lead to NA in the corresponding
           result.
+        min_count: int (default None, but set to 1 if skipna=True)
+          The minimal number of non-NA values in a sum that is necessary for a non-NA
+          result. This only has an effect if ``skipna=True``. As an example: you sum data
+          for a region for a certain sector, gas and year. If ``skipna=False``,
+          all countries in the region need to have non-NA data for that sector, gas,
+          year combination. If ``skipna=True`` and ``min_count=1`` then one country with
+          non-NA data is enough for a non-NA result. All NA values will be treated as
+          zero. If ``min_count=0`` all NA values will be treated as zero
+          also if there is no single non-NA value in the data that is to be summed.
 
         Returns
         -------
         filled : xr.DataArray
         """
         ds_sel = select_no_scalar_dimension(self._ds, sel)
         return self._ds[basket].fillna(
             ds_sel.pr.gas_basket_contents_sum(
                 basket=basket,
                 basket_contents=basket_contents,
                 skipna_evaluation_dims=skipna_evaluation_dims,
                 skipna=skipna,
+                min_count=min_count,
             )
         )
```

### Comparing `primap2-0.9.7/primap2/_alias_selection.py` & `primap2-0.9.8/primap2/_alias_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             except AttributeError:
                 obj = self._ds
             translations = obj.pr.dim_alias_translations
             dims = set(obj.dims).union(set(additional_allowed_values))
 
             # translate kwargs
             for arg_to_alias in args_to_alias:
-                if arg_to_alias in kwargs:
+                if arg_to_alias in kwargs and kwargs[arg_to_alias] is not None:
                     kwargs[arg_to_alias] = alias(
                         kwargs[arg_to_alias], translations, dims
                     )
 
             # translate args
             args_translated = []
             for i, arg in enumerate(args):
```

### Comparing `primap2-0.9.7/primap2/_data_format.py` & `primap2-0.9.8/primap2/_data_format.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/_downscale.py` & `primap2-0.9.8/primap2/_downscale.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Hashable, Sequence
-from typing import Optional
+from typing import Optional, Union
 
 import xarray as xr
 
 from ._accessor_base import BaseDataArrayAccessor, BaseDatasetAccessor
 from ._aggregate import select_no_scalar_dimension
 from ._units import ureg
 
@@ -13,15 +13,17 @@
         self,
         *,
         dim: Hashable,
         basket: Hashable,
         basket_contents: Sequence[Hashable],
         check_consistency: bool = True,
         sel: Optional[dict[Hashable, Sequence]] = None,
-        skipna_evaluation_dims: Sequence[Hashable] = tuple(),
+        skipna_evaluation_dims: Union[None, Sequence[Hashable]] = None,
+        skipna: bool = True,
+        tolerance: float = 0.01,
     ) -> xr.DataArray:
         """Downscale timeseries along a dimension using a basket defined on a
         broader timeseries.
 
         This is useful if you have data for many points in time for a total, for example
         the entire Energy sector, and higher-resolution data (e.g. fossil and non-fossil
         energies separately) for only a few points in time. In the example, the Energy
@@ -51,32 +53,52 @@
         sel: Selection dict, optional
           If the downscaling should only be done on a subset of the Dataset while
           retaining all other values unchanged, give a selection dictionary. The
           downscaling will be done on ``ds.loc[sel]``.
         skipna_evaluation_dims: list of str, optional
           Dimensions which should be evaluated to determine if NA values should be
           skipped entirely if missing fully. By default, no NA values are skipped.
+        skipna: bool, default True
+          If true it will be passed on to xarray's ds.sum function with min_count=1
+          for the calculation of the basket.
+          The effect is that NA values in a sum will be ignored and treated as zero
+          in the sum unless all values are NA which results in NA.
+        tolerance: float
+          If given it overrides the default tolerance for deviations of sums of
+          individual timeseries to given aggregate timeseries. Default is 0.01 (1%)
 
         Returns
         -------
         downscaled: xr.DataArray
         """
         da_sel = select_no_scalar_dimension(self._da, sel)
 
         basket_contents_da = da_sel.loc[{dim: basket_contents}]
         basket_da = da_sel.loc[{dim: basket}]
 
+        if skipna_evaluation_dims is not None:
+            if skipna:
+                raise ValueError(
+                    "Only one of 'skipna' and 'skipna_evaluation_dims' may be supplied, not"
+                    " both."
+                )
+            else:
+                skipna = None
+
         basket_sum = basket_contents_da.pr.sum(
-            dim=dim, skipna_evaluation_dims=skipna_evaluation_dims
+            dim=dim,
+            skipna=skipna,
+            min_count=1,
+            skipna_evaluation_dims=skipna_evaluation_dims,
         )
 
         if check_consistency:
             deviation: xr.DataArray = abs(basket_da / basket_sum - 1)
-            devmax = deviation.max()
-            if devmax > 0.01:
+            devmax = float(deviation.max().pint.dequantify().data)
+            if devmax > tolerance:
                 raise ValueError(
                     f"Sum of the basket_contents {basket_contents!r} deviates"
                     f" {devmax * 100} % from the basket"
                     f" {basket!r}, which is more than the allowed 1 %. "
                     "To continue regardless, set check_consistency=False."
                 )
 
@@ -100,15 +122,17 @@
         self,
         *,
         dim: Hashable,
         basket: Hashable,
         basket_contents: Sequence[Hashable],
         check_consistency: bool = True,
         sel: Optional[dict[Hashable, Sequence]] = None,
-        skipna_evaluation_dims: Sequence[Hashable] = tuple(),
+        skipna_evaluation_dims: Optional[Sequence[Hashable]] = None,
+        skipna: bool = True,
+        tolerance: float = 0.01,
     ) -> xr.Dataset:
         """Downscale timeseries along a dimension using a basket defined on a
         broader timeseries.
 
         This is useful if you have data for many points in time for a total, for example
         the entire Energy sector, and higher-resolution data (e.g. fossil and non-fossil
         energies separately) for only a few points in time. In the example, the Energy
@@ -138,14 +162,22 @@
         sel: Selection dict, optional
           If the downscaling should only be done on a subset of the Dataset while
           retaining all other values unchanged, give a selection dictionary. The
           downscaling will be done on ``ds.loc[sel]``.
         skipna_evaluation_dims: list of str, optional
           Dimensions which should be evaluated to determine if NA values should be
           skipped entirely if missing fully. By default, no NA values are skipped.
+        skipna: bool, default True
+          If true it will be passed on to xarray's ds.sum function with min_count=1 for
+          the calculation of the basket.
+          The effect is that NA values in a sum will be ignored and treated as zero
+          in the sum unless all values are NA which results in NA.
+        tolerance: float
+          If given it overrides the default tolerance for deviations of sums of
+          individual timeseries to given aggregate timeseries. Default is 0.01 (1%)
 
         Notes
         -----
         To downscale along the entity dimension, i.e. to downscale gases, see
         :py:meth:`downscale_gas_timeseries`, which handles gwp conversions
         appropriately.
 
@@ -154,22 +186,34 @@
         downscaled: xr.Dataset
         """
         ds_sel = select_no_scalar_dimension(self._ds, sel)
 
         basket_contents_ds = ds_sel.loc[{dim: basket_contents}]
         basket_ds = ds_sel.loc[{dim: basket}]
 
+        if skipna_evaluation_dims is not None:
+            if skipna:
+                raise ValueError(
+                    "Only one of 'skipna' and 'skipna_evaluation_dims' may be supplied, not"
+                    " both."
+                )
+            else:
+                skipna = None
+
         basket_sum = basket_contents_ds.pr.sum(
-            dim=dim, skipna_evaluation_dims=skipna_evaluation_dims
+            dim=dim,
+            skipna=skipna,
+            min_count=1,
+            skipna_evaluation_dims=skipna_evaluation_dims,
         )
 
         if check_consistency:
             deviation = abs(basket_ds / basket_sum - 1)
             devmax = deviation.to_array().max()
-            if devmax > 0.01:
+            if devmax > tolerance:
                 raise ValueError(
                     f"Sum of the basket_contents {basket_contents!r} deviates"
                     f" {devmax * 100} % from the basket"
                     f" {basket!r}, which is more than the allowed 1 %. "
                     "To continue regardless, set check_consistency=False."
                 )
 
@@ -190,15 +234,17 @@
     def downscale_gas_timeseries(
         self,
         *,
         basket: Hashable,
         basket_contents: Sequence[Hashable],
         check_consistency: bool = True,
         sel: Optional[dict[Hashable, Sequence]] = None,
-        skipna_evaluation_dims: Sequence[Hashable] = tuple(),
+        skipna_evaluation_dims: Optional[Sequence[Hashable]] = None,
+        skipna: bool = True,
+        tolerance: float = 0.01,
     ) -> xr.Dataset:
         """Downscale a gas basket defined on a broader timeseries to its contents
         known on fewer time points.
 
         This is useful if you have data for many points in time for a gas basket, for
         example KYOTOGHG, and higher-resolution data (e.g. the individual green house
         gases included in KYOTOGHG) for only a few points in time.
@@ -226,39 +272,60 @@
         sel: Selection dict, optional
           If the downscaling should only be done on a subset of the Dataset while
           retaining all other values unchanged, give a selection dictionary. The
           downscaling will be done on ``ds.loc[sel]``.
         skipna_evaluation_dims: list of str, optional
           Dimensions which should be evaluated to determine if NA values should be
           skipped entirely if missing fully. By default, no NA values are skipped.
+        skipna: bool, optional
+          If true it will be passed on to xarray's ds.sum function with min_count=1 for
+          the calculation of the basket.
+          The effect is that NA values in a sum will be ignored and treated as zero
+          in the sum unless all values are NA which results in NA.
+        tolerance: float
+          If given it overrides the default tolerance for deviations of sums of
+          individual timeseries to given aggregate timeseries. Default is 0.01 (1%)
 
         Returns
         -------
         downscaled: xr.Dataset
         """
         ds_sel = select_no_scalar_dimension(self._ds, sel)
 
         basket_contents_converted = xr.Dataset()
         da_basket = ds_sel[basket]
         for var in basket_contents:
             da: xr.DataArray = ds_sel[var]
             basket_contents_converted[var] = da.pr.convert_to_gwp_like(like=da_basket)
 
+        if skipna_evaluation_dims is not None:
+            if skipna:
+                raise ValueError(
+                    "Only one of 'skipna' and 'skipna_evaluation_dims' may be supplied, not"
+                    " both."
+                )
+            else:
+                skipna = None
+
         basket_sum = basket_contents_converted.pr.sum(
-            dim="entity", skipna_evaluation_dims=skipna_evaluation_dims
+            dim="entity",
+            skipna=skipna,
+            min_count=1,
+            skipna_evaluation_dims=skipna_evaluation_dims,
         )
 
         if check_consistency:
             deviation = abs(da_basket / basket_sum - 1)
             devmax = deviation.max().item()
-            if devmax > 0.01:
+            if devmax > tolerance:
                 raise ValueError(
                     f"Sum of the basket_contents {basket_contents!r} deviates"
                     f" {devmax * 100} % from the basket"
                     f" {basket!r}, which is more than the allowed 1 %. "
+                    f" {deviation}"
                     "To continue regardless, set check_consistency=False."
                 )
 
         # inter- and extrapolate
         shares = (
             (basket_contents_converted / basket_sum)
             .pint.to({x: "" for x in basket_contents_converted.keys()})
```

### Comparing `primap2-0.9.7/primap2/_merge.py` & `primap2-0.9.8/primap2/_merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,22 +87,19 @@
 
     Strategy:
     * remove all length-1 dimensions and put them in description
     * convert the rest into a pandas dataframe for nice printing
     """
     scalar_dims = [dim for dim in da_error.dims if len(da_error[dim]) == 1]
     scalar_dims_str = ", ".join(f"{dim}={da_error[dim].item()}" for dim in scalar_dims)
-
-    errors_str = (
-        da_error.squeeze(drop=True)
-        .pint.dequantify()
-        .to_dataframe()
-        .dropna()
-        .to_string()
-    )
+    da_error_dequ = da_error.squeeze(drop=True).pint.dequantify()
+    if np.ndim(da_error_dequ.data) == 0:
+        errors_str = str(da_error_dequ.data)
+    else:
+        errors_str = da_error_dequ.to_dataframe().dropna().to_string()
 
     return (
         f"pr.merge error: found discrepancies larger than tolerance "
         f"({tolerance * 100:.2f}%) for {scalar_dims_str}:\n"
         f"shown are relative discrepancies.\n" + errors_str
     )
```

### Comparing `primap2-0.9.7/primap2/_metadata.py` & `primap2-0.9.8/primap2/_metadata.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/_overview.py` & `primap2-0.9.8/primap2/_overview.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/_setters.py` & `primap2-0.9.8/primap2/_setters.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/_units.py` & `primap2-0.9.8/primap2/_units.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/accessors.py` & `primap2-0.9.8/primap2/accessors.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/pm2io/_GHG_inventory_reading.py` & `primap2-0.9.8/primap2/pm2io/_GHG_inventory_reading.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/pm2io/__init__.py` & `primap2-0.9.8/primap2/pm2io/__init__.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/pm2io/_conversion.py` & `primap2-0.9.8/primap2/pm2io/_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,14 +339,15 @@
     # define the mapping of PRIMAP GWP specifications to PRIMAP2 GWP specification
     # no GWP given will be mapped to SAR
     gwp_mapping = {
         "SAR": "SARGWP100",
         "AR4": "AR4GWP100",
         "AR5": "AR5GWP100",
         "AR5CCF": "AR5CCFGWP100",  # not sure if implemented in scmdata units
+        "AR6": "AR6GWP100",
     }
 
     # build regexp to match the GWP conversion variables
     regexp_str = "("
     for current_entity in entities_gwp:
         regexp_str = regexp_str + current_entity + "|"
     regexp_str = regexp_str[0:-1] + ")"
```

### Comparing `primap2-0.9.7/primap2/pm2io/_data_reading.py` & `primap2-0.9.8/primap2/pm2io/_data_reading.py`

 * *Files 4% similar despite different names*

```diff
@@ -1342,15 +1342,15 @@
     """Parse a string code and return 0 or np.nan based on rules to interpret
     the codes."""
     code = code.strip()
     if code in _special_codes:
         return _special_codes[code]
 
     parts = code.split(",")
-    parts = [x.replace(".", "").strip() for x in parts]
+    parts = [x.replace(".", "").strip().upper() for x in parts]
     if "IE" in parts or "NO" in parts:
         return 0
     if "NE" in parts or "NA" in parts:
         return np.nan
     raise ValueError(f"Could not parse code: {code!r}.")
 
 
@@ -1386,78 +1386,119 @@
     """Replace str values indicating not-a-number by float NaN."""
     for col in columns:
         data[col] = data[col].replace(na_repl_dict)
         data[col] = pd.to_numeric(data[col], errors="coerce")
         data[col] = data[col].astype("float64", copy=False, errors="ignore")
 
 
-def preferred_unit(entity: str, units: list[str], gwp_to_use: Union[None, str]) -> str:
+def preferred_unit(entity: str, units: dict[str, str]) -> Union[str, None]:
     """Choose the preferred unit for the given entity.
 
     In general, "Gg <substance> / year" will be preferred if it is compatible with the
     given input units. Otherwise, the first unit from units will be preferred.
 
     Parameters
     ----------
     entity: str
         Basic entity, e.g. a gas.
-    units: list of str
-        Units which are in use for the entity.
-    gwp_to_use: str, optional
-        Global warming potential specification which will be used for the conversion.
-        By specifying the gwp_to_use, you can make sure that it will be possible to
+    units: dict of str, str
+        Keys are the units which are in use for the entity and values the global
+        warming potential specifications which will be used for the conversion.
+        By specifying the gwp_context to use, you can make sure that it will be possible to
         convert from the input units to the output unit with the given gwp.
+        If not applicable for a unit use None
 
     Returns
     -------
     preferred_unit: str
         The best unit for the given entity and units.
 
     Examples
     --------
-    >>> preferred_unit("CO2", ["kt CO2 / yr", "mg CO2 / s"], None)
+    >>> preferred_unit("CO2", {"kt CO2 / yr": None, "mg CO2 / s": None})
     'Gg CO2 / yr'
-    >>> preferred_unit("CH4", ["kt CO2 / yr"], "AR4GWP100")
+    >>> preferred_unit("CH4", {"kt CO2 / yr": "AR4GWP100"})
     'Gg CH4 / yr'
-    >>> preferred_unit("CH4", ["kt CO2 / yr", "Mg CO2 / yr"], None)
-    'kt CO2 / yr'
-    """
-    unit_fallback = units[0]
-    conversion_contexts = []
-    if gwp_to_use:
-        conversion_contexts.append(gwp_to_use)
+    >>> preferred_unit("CH4", {"kt CO2 / yr": None, "Mg CH4 / yr": None})
+    None
+    >>> preferred_unit("CH4", {"kt CO2 / yr": "AR4GWP100", "Gg CO2 / yr": "SARGWP100"})
+    'Gg CH4 / yr'
+    >>> preferred_unit(
+    ...     "KYOTOGHG", {"kt CO2 / yr": "AR4GWP100", "Gg CO2 / yr": "SARGWP100"}
+    ... )
 
-    # check if conversion to native unit is possible
+    """
+    unit_fallback = next(iter(units.keys()))
+    context_fallback = units[unit_fallback]
+    # check if all can be converted to native or fallback units
+    native_conv = []
+    fb_conv = []
     native_unit = "Gg " + entity + " / yr"
-    try:
-        # print(f"Testing conversion from {ureg[unit_fallback].units} to "
-        #       f"{ureg[native_unit].units} for {entity}.")
-        if ureg(unit_fallback).is_compatible_with(
-            ureg[native_unit], *conversion_contexts
-        ):
-            return native_unit
-    except pint.UndefinedUnitError:
-        # we have a gas basket or something unknown, so no conversion to native unit
-        # print(f"Exception occurred for entity {entity}")
-        pass
-
-    return unit_fallback
+    for unit in units.keys():
+        conversion_contexts = []
+        if units[unit] is not None:
+            conversion_contexts.append(units[unit])
+
+        # check if conversion to native unit is possible
+        try:
+            # print(f"Testing conversion from {ureg[unit_fallback].units} to "
+            #       f"{ureg[native_unit].units} for {entity}.")
+            if ureg(unit).is_compatible_with(ureg[native_unit], *conversion_contexts):
+                native_conv.append(True)
+            else:
+                native_conv.append(False)
+        except pint.UndefinedUnitError:
+            # we have a gas basket or something unknown, so no conversion to native unit
+            # print(f"Exception occurred for entity {entity}")
+            native_conv.append(False)
+            pass
+
+        # check if conversion to fallback unit is possible
+        if units[unit] != context_fallback:
+            fb_conv.append(False)
+            pass
+        else:
+            try:
+                # print(f"Testing conversion from {ureg[unit_fallback].units} to "
+                #       f"{ureg[native_unit].units} for {entity}.")
+                if ureg(unit).is_compatible_with(
+                    ureg[unit_fallback], *conversion_contexts
+                ):
+                    fb_conv.append(True)
+                else:
+                    fb_conv.append(False)
+            except pint.UndefinedUnitError:
+                # we have a gas basket or something unknown, so no conversion to native
+                # unit
+                # print(f"Exception occurred for entity {entity}")
+                fb_conv.append(False)
+                pass
+
+    if all(native_conv):
+        # print(f"converting {entity} to native unit {native_unit}")
+        return native_unit
+    elif all(fb_conv):
+        # print(f"converting {entity} to fallback unit {unit_fallback}")
+        return unit_fallback
+    else:
+        return None
 
 
 def harmonize_units(
     data: pd.DataFrame,
     *,
     unit_col: Union[None, str] = None,
     attrs: Union[None, dict] = None,
     dimensions: Iterable[str],
 ) -> None:
     """Harmonize the units of the input data.
 
-    For each entity, convert all time series to the same unit (the unit that occurs
-    first). Units must already be in PRIMAP2 style.
+    For each entity, convert all time series to the same unit (the native unit or
+    the unit that occurs first if conversion to the native unit is not possible). Units
+    must already be in PRIMAP2 style.
 
     As unit handling is tricky and with new units new problem occur this function has a
     lot of (currently commented) debug output
 
     Parameters
     ----------
     data: pd.DataFrame
@@ -1486,72 +1527,113 @@
         entity_col = dim_aliases.get("entity", "entity")
     else:
         entity_col = "entity"
 
     if unit_col is None:
         unit_col = dim_aliases.get("unit", "unit")
 
+    # find basic entities for all entities and make a list
     entities = data[entity_col].unique()
+    basic_entities = {}
+
     # print(entities)
     for entity in entities:
         # check if GWP given in entity
+        # print(f"entity: {entity}")
         gwp_match = re.findall(r"\(([A-Z0-9]*)\)$", entity)
         if gwp_match:
             gwp_to_use = gwp_match[0]
-            basic_entity = re.findall(r"^[^()\s]*", entity)
+            basic_entity = re.findall(r"^[^\(\)\s]*", entity)
             basic_entity = basic_entity[0]
         else:
             gwp_to_use = None
             basic_entity = entity
+        # print(f"gwp: {gwp_to_use}")
         # print(f"basic_entity: {basic_entity}")
-        # get all units for this entity
-        data_this_entity = data.loc[data[entity_col] == entity]
-        units_this_entity = data_this_entity[unit_col].unique()
-
-        if len(units_this_entity) > 1 or gwp_to_use:
-            # need unit conversion.
-            unit_to = preferred_unit(basic_entity, units_this_entity, gwp_to_use)
+        if basic_entity in basic_entities.keys():
+            basic_entities[basic_entity][entity] = gwp_to_use
+        else:
+            basic_entities[basic_entity] = {entity: gwp_to_use}
 
-            # if len(units_this_entity) > 1:
+    for basic_entity in basic_entities:
+        # print(f"basic_entity: {basic_entity}")
+        # print(f"entities: {basic_entities[basic_entity]}")
+        # get all units for this entity
+        data_this_basic_entity = data.loc[
+            data[entity_col].isin(basic_entities[basic_entity])
+        ]
+        units_this_basic_entity = data_this_basic_entity[unit_col].unique()
+        unit_gwp_this_basic_entity = {}
+        gwp_conversion_this_basic_entity = False
+        for entity in basic_entities[basic_entity].keys():
+            data_this_entity = data_this_basic_entity.loc[data[entity_col] == entity]
+            units_this_entity = data_this_entity[unit_col].unique()
             for unit in units_this_entity:
-                if unit != unit_to:
-                    # print(f"Working on unit {unit}")
-                    unit_pint = ureg[unit]
-                    # could add a try except block here to throw and log an error or
-                    # add error info in DF instead of crashing
-                    if gwp_to_use:
-                        with ureg.context(gwp_to_use):
-                            unit_pint = unit_pint.to(unit_to)
-                    else:
-                        unit_pint = unit_pint.to(unit_to)
-                    # print(f"Pint unit is {unit_pint}")
-                    factor = unit_pint.magnitude
-                    # print(f"Converting with factor {factor} to unit {unit_to}")
-                    mask = (data[entity_col] == entity) & (data[unit_col] == unit)
-                    # print(data.loc[mask, data_cols])
-                    try:
-                        data.loc[mask, data_cols] *= factor
-                    except TypeError:
-                        # print(data.loc[mask, data_cols])
-                        strs = find_str_values_in_data(data, data_cols)
-                        logger.error(
-                            f"The following string values are present and can "
-                            f"not be converted during unit conversion: {strs}."
-                        )
-                        raise ValueError(
-                            f"String values {strs} prevent unit conversion."
-                        ) from None
-
-                    data.loc[mask, unit_col] = unit_to
-
-            if gwp_to_use and unit_to not in units_this_entity:
-                # entity was converted
-                entity_mask = data[entity_col] == entity
-                # print(f"Changing entity from {entity} to {basic_entity}")
-                data.loc[entity_mask, entity_col] = basic_entity
+                unit_gwp_this_basic_entity[unit] = basic_entities[basic_entity][entity]
+            if basic_entities[basic_entity][entity] is not None:
+                gwp_conversion_this_basic_entity = True
+
+            if len(units_this_basic_entity) > 1 or gwp_conversion_this_basic_entity:
+                # need unit conversion.
+                # determine unit to convert all units to. If none is found no conversion
+                # is carried out at all
+                unit_to = preferred_unit(basic_entity, unit_gwp_this_basic_entity)
+                # print(f"basic_entity: {basic_entity}, unit_to: {unit_to}")
+                if unit_to is not None:
+                    # print(f"unit conversion for {basic_entity}, "
+                    #      f"{basic_entities[basic_entity]}")
+                    for entity in basic_entities[basic_entity]:
+                        data_this_entity = data.loc[data[entity_col] == entity]
+                        units_this_entity = data_this_entity[unit_col].unique()
+
+                        for unit in units_this_entity:
+                            if unit != unit_to:
+                                # print(f"Working on unit {unit}")
+                                unit_pint = ureg[unit]
+                                # could add a try except block here to throw and log an
+                                # error or add error info in DF instead of crashing
+                                gwp_this_entity = basic_entities[basic_entity][entity]
+                                if gwp_this_entity:
+                                    with ureg.context(gwp_this_entity):
+                                        unit_pint = unit_pint.to(unit_to)
+                                else:
+                                    unit_pint = unit_pint.to(unit_to)
+                                # print(f"Pint unit is {unit_pint}")
+                                factor = unit_pint.magnitude
+                                # print(f"Converting with factor {factor} to unit
+                                # {unit_to}")
+                                mask = (data[entity_col] == entity) & (
+                                    data[unit_col] == unit
+                                )
+                                # print(data.loc[mask, data_cols])
+                                try:
+                                    data.loc[mask, data_cols] *= factor
+                                except TypeError:
+                                    # print(data.loc[mask, data_cols])
+                                    strs = find_str_values_in_data(data, data_cols)
+                                    logger.error(
+                                        f"The following string values are present and "
+                                        f"can not be converted during unit conversion: "
+                                        f"{strs}."
+                                    )
+                                    raise ValueError(
+                                        f"String values {strs} prevent unit conversion."
+                                    ) from None
+
+                                data.loc[mask, unit_col] = unit_to
+
+                        # if entity differs from basic entity and the units are not
+                        # compatible we had GWP conversion and have to adapt the entity
+                        if (entity != basic_entity) and not ureg(
+                            unit
+                        ).is_compatible_with(ureg[unit_to]):
+                            # entity was converted
+                            entity_mask = data[entity_col] == entity
+                            # print(f"Changing entity from {entity} to {basic_entity}")
+                            data.loc[entity_mask, entity_col] = basic_entity
 
 
 def sort_columns_and_rows(
     data: pd.DataFrame,
     dimensions: Iterable[str],
 ) -> tuple[pd.DataFrame, list[str]]:
     """Sort the data.
```

### Comparing `primap2-0.9.7/primap2/pm2io/_interchange_format.py` & `primap2-0.9.8/primap2/pm2io/_interchange_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
 
     # check resulting shape to estimate memory consumption
     dim_lens = {dim: len(np.unique(data_xr[dim].dropna("index"))) for dim in index_cols}
     dim_lens["time"] = len(time_cols)
     shapes = []
     for _, dims in dimensions.items():
         shapes.append([dim_lens[dim] for dim in dims if dim != "unit"])
-    array_size = sum(np.product(shape) for shape in shapes)
+    array_size = sum(np.prod(shape) for shape in shapes)
     logger.debug(f"Expected array shapes: {shapes}, resulting in size {array_size:,}.")
     if array_size > max_array_size:
         logger.error(
             f"Set with {len(shapes)} entities and a total of {len(index_cols)} "
             f"dimensions will have a size of {array_size:,} "
             f"due to the shapes {shapes}. Aborting to avoid out-of-memory errors. To "
             f"continue, raise max_array_size (currently {max_array_size:,})."
```

### Comparing `primap2-0.9.7/primap2/tests/conftest.py` & `primap2-0.9.8/primap2/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import primap2  # noqa: F401
 
 from . import examples
 
 
 # monkey-patch caplog to work wit loguru
-# see https://loguru.readthedocs.io/en/stable/resources/migration.html#making-things-work-with-pytest-and-caplog  # noqa: E501
+# see https://loguru.readthedocs.io/en/stable/resources/migration.html#making-things-work-with-pytest-and-caplog
 @pytest.fixture
 def caplog(caplog):
     class PropogateHandler(logging.Handler):
         def emit(self, record):
             logging.getLogger(record.name).handle(record)
 
     handler_id = logger.add(PropogateHandler(), format="{message} {extra}")
```

### Comparing `primap2-0.9.7/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.csv` & `primap2-0.9.8/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.csv`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.nc` & `primap2-0.9.8/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.yaml` & `primap2-0.9.8/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.yaml`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/tests/data/test_from_interchange_format_output.nc` & `primap2-0.9.8/primap2/tests/data/test_from_interchange_format_output.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/tests/data/test_sum_skip_allna_inhomogeneous_result.nc` & `primap2-0.9.8/primap2/tests/data/test_sum_skip_allna_inhomogeneous_result.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/tests/examples.py` & `primap2-0.9.8/primap2/tests/examples.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/tests/test_aggregate.py` & `primap2-0.9.8/primap2/tests/test_aggregate.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 """Tests for _aggregate.py"""
 
 import pathlib
 
 import numpy as np
 import pytest
 import xarray as xr
-import xarray.testing
 
 import primap2
 from primap2 import ureg
 
 from . import examples
 from .utils import assert_equal
 
@@ -65,15 +64,15 @@
     ds = xr.Dataset({"1": da, "2": da.copy()})
     dsf = ds.pr.fill_all_na(dim="b", value=0)
     assert np.allclose(dsf["1"], a_expected, equal_nan=True)
     assert np.allclose(dsf["2"], a_expected, equal_nan=True)
 
 
 class TestSum:
-    def test_skipna(self):
+    def test_skipna_evaluation_dims(self):
         coords = [("a", [1, 2]), ("b", [1, 2]), ("c", [1, 2, 3])]
         da = xr.DataArray(
             data=[
                 [[np.nan, np.nan, np.nan], [np.nan, 1, 2]],
                 [[np.nan, np.nan, np.nan], [np.nan, 1, 2]],
             ],
             coords=coords,
@@ -97,14 +96,59 @@
             {
                 "1": b_expected,
                 "2": b_expected,
             }
         )
         xr.testing.assert_identical(dss, dss_expected)
 
+    def test_skipna(self):
+        coords = [("a", [1, 2]), ("b", [1, 2]), ("c", [1, 2, 3])]
+        da = xr.DataArray(
+            data=[
+                [[np.nan, np.nan, np.nan], [np.nan, 1, 2]],
+                [[np.nan, np.nan, np.nan], [np.nan, 1, 2]],
+            ],
+            coords=coords,
+        )
+
+        b0 = da.pr.sum(dim="b", skipna=True, min_count=0)
+        b0_expected = xr.DataArray(
+            data=[[0, 1, 2], [0, 1, 2]], coords=[coords[0], coords[2]]
+        )
+        assert np.allclose(b0, b0_expected, equal_nan=True)
+
+        b1 = da.pr.sum(dim="b", skipna=True, min_count=1)
+        b1_expected = xr.DataArray(
+            data=[[np.nan, 1, 2], [np.nan, 1, 2]], coords=[coords[0], coords[2]]
+        )
+        assert np.allclose(b1, b1_expected, equal_nan=True)
+
+        b2 = da.pr.sum(dim="b", skipna=True, min_count=2)
+        b2_expected = xr.DataArray(
+            data=[[np.nan, np.nan, np.nan], [np.nan, np.nan, np.nan]],
+            coords=[coords[0], coords[2]],
+        )
+        assert np.allclose(b2, b2_expected, equal_nan=True)
+
+        bdef = da.pr.sum(dim="b", skipna=True)
+        assert np.allclose(bdef, b1_expected, equal_nan=True)
+
+        ds = xr.Dataset({"1": da, "2": da.copy()})
+        dss1 = ds.pr.sum(dim="b", skipna=True, min_count=1)
+        dss1_expected = xr.Dataset(
+            {
+                "1": b1_expected,
+                "2": b1_expected,
+            }
+        )
+        xr.testing.assert_identical(dss1, dss1_expected)
+
+        dssdef = ds.pr.sum(dim="b", skipna=True)
+        xr.testing.assert_identical(dssdef, dss1_expected)
+
     def test_inhomogeneous_regression(self, opulent_ds: xr.Dataset):
         ds = opulent_ds
         dss = ds.pr.loc[{"category": ["1", "2", "3", "4", "5"]}].pr.sum("category")
         xr.testing.assert_identical(dss["population"], ds["population"])
         actual = dss["CO2"]
         expected = (
             ds["CO2"]
```

### Comparing `primap2-0.9.7/primap2/tests/test_alias_selection.py` & `primap2-0.9.8/primap2/tests/test_alias_selection.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/tests/test_conversion.py` & `primap2-0.9.8/primap2/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/tests/test_data_format.py` & `primap2-0.9.8/primap2/tests/test_data_format.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/tests/test_data_reading.py` & `primap2-0.9.8/primap2/tests/test_data_reading.py`

 * *Files 2% similar despite different names*

```diff
@@ -563,14 +563,42 @@
             filter_keep=filter_keep,
             filter_remove=filter_remove,
         )
         df_result.to_csv(tmp_path / "test.csv")
         df_result = pd.read_csv(tmp_path / "test.csv", index_col=0)
         pd.testing.assert_frame_equal(df_result, df_expected, check_column_type=False)
 
+    def test_unit_harmonization(
+        self,
+        tmp_path,
+        coords_cols,
+        coords_defaults,
+        coords_terminologies,
+        coords_value_mapping,
+    ):
+        file_input = DATA_PATH / "test_csv_data_unit_harmonization.csv"
+        file_expected = DATA_PATH / "test_read_wide_csv_file_output_unit_harm.csv"
+        df_expected = pd.read_csv(file_expected, index_col=0)
+
+        del coords_cols["sec_cats__Class"]
+        del coords_defaults["sec_cats__Type"]
+        del coords_terminologies["sec_cats__Class"]
+        del coords_terminologies["sec_cats__Type"]
+
+        df_result = pm2io.read_wide_csv_file_if(
+            file_input,
+            coords_cols=coords_cols,
+            coords_defaults=coords_defaults,
+            coords_terminologies=coords_terminologies,
+            coords_value_mapping=coords_value_mapping,
+        )
+        df_result.to_csv(tmp_path / "test.csv")
+        df_result = pd.read_csv(tmp_path / "test.csv", index_col=0)
+        pd.testing.assert_frame_equal(df_result, df_expected, check_column_type=False)
+
     def test_function_mapping(
         self,
         tmp_path,
         coords_cols,
         coords_defaults,
         coords_terminologies,
         coords_value_mapping,
```

### Comparing `primap2-0.9.7/primap2/tests/test_downscale.py` & `primap2-0.9.8/primap2/tests/test_downscale.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 """Tests for _downscale.py"""
 
 import numpy as np
 import pytest
 import xarray as xr
-import xarray.testing
 
 from primap2 import ureg
 
 from .utils import allclose, assert_equal
 
 
 def test_downscale_gas_timeseries(empty_ds):
@@ -33,14 +32,25 @@
     expected["CH4"][:] = 1 * ureg("Gg CH4 / year")
     expected["CO2"].loc[{"time": "2020"}] = 2 * ureg("Gg CO2 / year")
     expected["SF6"].loc[{"time": "2020"}] = 2 * ureg("Gg SF6 / year")
     expected["CH4"].loc[{"time": "2020"}] = 2 * ureg("Gg CH4 / year")
 
     xr.testing.assert_identical(downscaled, expected)
 
+    with pytest.raises(
+        ValueError,
+        match="Only one of 'skipna' and 'skipna_evaluation_dims' may be supplied, not both.",
+    ):
+        empty_ds.pr.downscale_gas_timeseries(
+            basket="KYOTOGHG (AR4GWP100)",
+            basket_contents=["CO2", "SF6", "CH4"],
+            skipna_evaluation_dims=["time"],
+            skipna=True,
+        )
+
     empty_ds["SF6"].loc[{"time": "2002"}] = 2 * ureg("Gg SF6 / year")
 
     with pytest.raises(
         ValueError, match="To continue regardless, set check_consistency=False"
     ):
         empty_ds.pr.downscale_gas_timeseries(
             basket="KYOTOGHG (AR4GWP100)", basket_contents=["CO2", "SF6", "CH4"]
@@ -108,27 +118,31 @@
     )
 
     downscaled_ds = ds.pr.downscale_timeseries(
         dim="area (ISO3)", basket="CAMB", basket_contents=["COL", "ARG", "MEX", "BOL"]
     )
     assert_equal(downscaled_ds["CO2"], expected, equal_nan=True, atol=0.01)
 
-    da.loc[{"area (ISO3)": "BOL", "time": "2002"}] = 2 * ureg("Gg CO2 / year")
     with pytest.raises(
-        ValueError, match="To continue regardless, set check_consistency=False"
+        ValueError,
+        match="Only one of 'skipna' and 'skipna_evaluation_dims' may be supplied, not both.",
     ):
-        da.pr.downscale_timeseries(
+        ds.pr.downscale_timeseries(
             dim="area (ISO3)",
             basket="CAMB",
             basket_contents=["COL", "ARG", "MEX", "BOL"],
+            skipna_evaluation_dims=["time"],
+            skipna=True,
         )
+
+    da.loc[{"area (ISO3)": "BOL", "time": "2002"}] = 2 * ureg("Gg CO2 / year")
     with pytest.raises(
         ValueError, match="To continue regardless, set check_consistency=False"
     ):
-        ds.pr.downscale_timeseries(
+        da.pr.downscale_timeseries(
             dim="area (ISO3)",
             basket="CAMB",
             basket_contents=["COL", "ARG", "MEX", "BOL"],
         )
 
     downscaled = da.pr.downscale_timeseries(
         dim="area (ISO3)",
```

### Comparing `primap2-0.9.7/primap2/tests/test_interchange_format.py` & `primap2-0.9.8/primap2/tests/test_interchange_format.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/tests/test_merge.py` & `primap2-0.9.8/primap2/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/tests/test_metadata.py` & `primap2-0.9.8/primap2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/tests/test_overview.py` & `primap2-0.9.8/primap2/tests/test_overview.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     da.pr.loc[{"product": "milk"}] = np.nan
 
     expected = pd.DataFrame(
         index=da.pr["animal"].values,
         columns=da.pr["product"].values,
         data=np.zeros((len(da.pr["animal"]), len(da.pr["product"])), dtype=np.int32),
     )
-    expected[:] = np.product(da.shape) // np.product(expected.shape)
+    expected[:] = np.prod(da.shape) // np.prod(expected.shape)
     expected.loc[:, "milk"] = 0
     expected.index.name = "animal (FAOSTAT)"
     expected.columns.name = "product (FAOSTAT)"
 
     pd.testing.assert_frame_equal(
         expected.astype(np.int32), da.pr.coverage("animal", "product").astype(np.int32)
     )
@@ -119,18 +119,16 @@
     ds["CO2"].pr.loc[{"product": "milk"}] = np.nan
 
     expected = pd.DataFrame(
         index=ds.pr["product"].values,
         columns=ds.pr["animal"].values,
         data=np.zeros((len(ds.pr["product"]), len(ds.pr["animal"])), dtype=int),
     )
-    expected[:] = np.product(ds["CO2"].shape) // np.product(expected.shape) * 4
-    expected.loc["milk", :] = (
-        np.product(ds["CO2"].shape) // np.product(expected.shape) * 3
-    )
+    expected[:] = np.prod(ds["CO2"].shape) // np.prod(expected.shape) * 4
+    expected.loc["milk", :] = np.prod(ds["CO2"].shape) // np.prod(expected.shape) * 3
     expected.index.name = "product (FAOSTAT)"
     expected.columns.name = "animal (FAOSTAT)"
     expected.name = "coverage"
 
     pd.testing.assert_frame_equal(expected, ds.pr.coverage("product", "animal"))
     pd.testing.assert_frame_equal(expected.T, ds.pr.coverage("animal", "product"))
 
@@ -140,17 +138,17 @@
     ds["CO2"].pr.loc[{"product": "milk"}] = np.nan
 
     expected = pd.DataFrame(
         index=list(ds.keys()),
         columns=ds.pr["area"].values,
         data=np.zeros((len(ds), len(ds.pr["area"].values)), dtype=int),
     )
-    expected[:] = np.product(ds["CO2"].shape)
-    expected.loc["population", :] = np.product(ds["population"].shape)
-    expected.loc["CO2", :] = np.product(ds["CO2"].shape) - np.product(
+    expected[:] = np.prod(ds["CO2"].shape)
+    expected.loc["population", :] = np.prod(ds["population"].shape)
+    expected.loc["CO2", :] = np.prod(ds["CO2"].shape) - np.prod(
         ds["CO2"].pr.loc[{"product": "milk"}].shape
     )
     expected = expected // len(ds.pr["area"].values)
     expected.name = "coverage"
     expected.index.name = "entity"
     expected.columns.name = "area (ISO3)"
 
@@ -172,15 +170,15 @@
     entites_expected = [x for x in ds.keys() if x != "population"]
 
     expected = pd.DataFrame(
         index=ds.pr["product"].values,
         columns=entites_expected,
         data=np.zeros((len(ds.pr["product"]), len(entites_expected)), dtype=int),
     )
-    expected[:] = np.product(ds["CO2"].shape) // len(ds.pr["product"])
+    expected[:] = np.prod(ds["CO2"].shape) // len(ds.pr["product"])
     expected.loc["milk", "CO2"] = 0
     expected.index.name = "product (FAOSTAT)"
     expected.columns.name = "entity"
 
     pd.testing.assert_frame_equal(expected, ds.pr.coverage("product", "entity"))
     pd.testing.assert_frame_equal(expected.T, ds.pr.coverage("entity", "product"))
```

### Comparing `primap2-0.9.7/primap2/tests/test_setters.py` & `primap2-0.9.8/primap2/tests/test_setters.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/tests/test_units.py` & `primap2-0.9.8/primap2/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2/tests/utils.py` & `primap2-0.9.8/primap2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/primap2.egg-info/SOURCES.txt` & `primap2-0.9.8/primap2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.check_python_version.py
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
@@ -104,15 +105,17 @@
 primap2/tests/data/long_no_time.csv
 primap2/tests/data/test_csv_data.csv
 primap2/tests/data/test_csv_data_category_name.csv
 primap2/tests/data/test_csv_data_category_name_fill_cat_code.csv
 primap2/tests/data/test_csv_data_category_name_long.csv
 primap2/tests/data/test_csv_data_sec_cat.csv
 primap2/tests/data/test_csv_data_sec_cat_strings.csv
+primap2/tests/data/test_csv_data_unit_harmonization.csv
 primap2/tests/data/test_from_interchange_format_output.nc
 primap2/tests/data/test_read_wide_csv_file_no_sec_cats.csv
 primap2/tests/data/test_read_wide_csv_file_no_sec_cats_cat_name.csv
 primap2/tests/data/test_read_wide_csv_file_output.csv
 primap2/tests/data/test_read_wide_csv_file_output_entity_def.csv
 primap2/tests/data/test_read_wide_csv_file_output_unit_def.csv
+primap2/tests/data/test_read_wide_csv_file_output_unit_harm.csv
 primap2/tests/data/test_sum_skip_allna_inhomogeneous_result.nc
 rosetta/combine_rows-set.ipynb
```

### Comparing `primap2-0.9.7/rosetta/combine_rows-set.ipynb` & `primap2-0.9.8/rosetta/combine_rows-set.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/setup.cfg` & `primap2-0.9.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = primap2
-version = 0.9.7
+version = 0.9.8
 author = Mika Pflüger
 author_email = mika.pflueger@climate-resource.com
 description = The next generation of the PRIMAP climate policy analysis suite.
 long_description = file: README.rst, CHANGELOG.rst
 long_description_content_type = text/x-rst
 url = https://github.com/pik-primap/primap2
 project_urls =
```

### Comparing `primap2-0.9.7/tbump.toml` & `primap2-0.9.8/tbump.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/pik-primap/primap2/"
 
 [version]
-current = "0.9.7"
+current = "0.9.8"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `primap2-0.9.7/update_changelog.py` & `primap2-0.9.8/update_changelog.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.7/update_citation_info.py` & `primap2-0.9.8/update_citation_info.py`

 * *Files identical despite different names*

