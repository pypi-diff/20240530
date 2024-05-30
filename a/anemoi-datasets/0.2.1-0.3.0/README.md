# Comparing `tmp/anemoi_datasets-0.2.1.tar.gz` & `tmp/anemoi_datasets-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemoi_datasets-0.2.1.tar", last modified: Fri May 17 10:22:11 2024, max compression
+gzip compressed data, was "anemoi_datasets-0.3.0.tar", last modified: Thu May 30 19:12:39 2024, max compression
```

## Comparing `anemoi_datasets-0.2.1.tar` & `anemoi_datasets-0.3.0.tar`

### file list

```diff
@@ -1,284 +1,286 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.033925 anemoi_datasets-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:10.981925 anemoi_datasets-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:10.989925 anemoi_datasets-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:10.989925 anemoi_datasets-0.2.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/.vscode/spellright.dict
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-05-17 10:22:11.033925 anemoi_datasets-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:10.989925 anemoi_datasets-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:10.989925 anemoi_datasets-0.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:10.989925 anemoi_datasets-0.2.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/_templates/.gitkeep
--rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/apply-fmt.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:10.993925 anemoi_datasets-0.2.1/docs/building/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:10.993925 anemoi_datasets-0.2.1/docs/building/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/filters/empty.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/filters/noop.rst
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/filters/rename.rst
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/filters/rotate_winds.rst
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/filters/select.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/filters/unrotate_winds.rst
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/filters.rst
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/handling-missing-dates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/handling-missing-values.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/naming-variables.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/operations.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:10.997925 anemoi_datasets-0.2.1/docs/building/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/accumulations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/accumulations1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/accumulations2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/forcings.rst
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/forcings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/grib.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/hindcasts.rst
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/mars.rst
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/mars1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/mars2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/netcdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/netcdf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/opendap.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/opendap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/recentre.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:10.997925 anemoi_datasets-0.2.1/docs/building/sources/yaml/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/yaml/grib1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/yaml/grib2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/yaml/grib3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/yaml/grib4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources/yaml/perturbations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/sources.rst
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/statistics.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/syntax.rst
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/syntax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:10.997925 anemoi_datasets-0.2.1/docs/building/yaml/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/yaml/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/yaml/building1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/yaml/building1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/yaml/building2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/yaml/building2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/yaml/building3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/yaml/building3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/yaml/concat.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/yaml/hindcasts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/yaml/input.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/yaml/missing_dates.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/yaml/nan.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/building/yaml/pipe.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/check-index.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.001925 anemoi_datasets-0.2.1/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/cli/compare.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/cli/copy.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/cli/create.rst
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/cli/inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/cli/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    58982 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/images.pptx
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/overview_.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.001925 anemoi_datasets-0.2.1/docs/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)   106709 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/schemas/matrix.excalidraw
--rw-r--r--   0 runner    (1001) docker     (127)    53069 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/schemas/matrix.png
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/schemas/overview.excalidraw
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/schemas/overview.png
--rw-r--r--   0 runner    (1001) docker     (127)    42125 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/schemas/recipe.excalidraw
--rw-r--r--   0 runner    (1001) docker     (127)    43845 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/schemas/recipe.png
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/test.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.001925 anemoi_datasets-0.2.1/docs/using/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.009925 anemoi_datasets-0.2.1/docs/using/code/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/area1_.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/area2_.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/chain_.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/combine_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/concat1.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/cutout_.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/drop_.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/end_.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/ensembles1_.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/frequency_.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/grids1_.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/join1.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/matching0_.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/matching1_.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/matching2_.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/matching3_.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/matching4_.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/misc1.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/misc2.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/missing_.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/open_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/open_combine1_.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/open_combine2_.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/open_complex.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/open_dict_.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/open_first_.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/open_list_.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/open_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/open_other.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/open_path.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/open_yaml_.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/rename_.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/reorder1_.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/reorder2_.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/select1_.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/select2_.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/shuffle_.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/some_attributes_.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/start_.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/statistics_.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/subset_example.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/thinning_.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/zip1_.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/code/zip2_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/combining.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/configuration.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/grids.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.013925 anemoi_datasets-0.2.1/docs/using/images/
--rw-r--r--   0 runner    (1001) docker     (127)   108038 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/images/area-1.png
--rw-r--r--   0 runner    (1001) docker     (127)    40564 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/images/concat.png
--rw-r--r--   0 runner    (1001) docker     (127)   141221 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/images/cutout-1.png
--rw-r--r--   0 runner    (1001) docker     (127)   122139 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/images/cutout-2.png
--rw-r--r--   0 runner    (1001) docker     (127)   129758 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/images/cutout-3.png
--rw-r--r--   0 runner    (1001) docker     (127)   151858 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/images/cutout-4.png
--rw-r--r--   0 runner    (1001) docker     (127)    38066 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/images/join.png
--rw-r--r--   0 runner    (1001) docker     (127)    36070 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/images/overlay.png
--rw-r--r--   0 runner    (1001) docker     (127)   109206 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/images/thinning-after.png
--rw-r--r--   0 runner    (1001) docker     (127)   141221 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/images/thinning-before.png
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/matching.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/methods.rst
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/miscellaneous.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/opening.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/other.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/selecting.rst
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/statistics.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/docs/using/subsetting.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:22:11.033925 anemoi_datasets-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:10.985925 anemoi_datasets-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:10.985925 anemoi_datasets-0.2.1/src/anemoi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.013925 anemoi_datasets-0.2.1/src/anemoi/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 10:22:10.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.013925 anemoi_datasets-0.2.1/src/anemoi/datasets/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/commands/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/commands/copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/commands/create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.013925 anemoi_datasets-0.2.1/src/anemoi/datasets/commands/inspect/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/commands/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/commands/inspect/zarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/commands/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.017925 anemoi_datasets-0.2.1/src/anemoi/datasets/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/compute/recentre.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.017925 anemoi_datasets-0.2.1/src/anemoi/datasets/create/
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.017925 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.017925 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/filters/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/filters/noop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/filters/rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/filters/rotate_winds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/filters/unrotate_winds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.021925 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/accumulations.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/forcings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/grib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13042 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/hindcasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/mars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/opendap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/recentre.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/tendencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    27888 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/input.py
--rw-r--r--   0 runner    (1001) docker     (127)    28611 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/loaders.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3682 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/size.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.021925 anemoi_datasets-0.2.1/src/anemoi/datasets/create/statistics/
--rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/statistics/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/create/zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.025925 anemoi_datasets-0.2.1/src/anemoi/datasets/data/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/debug.css
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/forewards.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/join.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/masked.py
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10869 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/stores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/data/unchecked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.025925 anemoi_datasets-0.2.1/src/anemoi/datasets/dates/
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/dates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/dates/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/grids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.025925 anemoi_datasets-0.2.1/src/anemoi/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/src/anemoi/datasets/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.029925 anemoi_datasets-0.2.1/src/anemoi_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-05-17 10:22:10.000000 anemoi_datasets-0.2.1/src/anemoi_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-17 10:22:10.000000 anemoi_datasets-0.2.1/src/anemoi_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:22:10.000000 anemoi_datasets-0.2.1/src/anemoi_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 10:22:10.000000 anemoi_datasets-0.2.1/src/anemoi_datasets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-17 10:22:10.000000 anemoi_datasets-0.2.1/src/anemoi_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 10:22:10.000000 anemoi_datasets-0.2.1/src/anemoi_datasets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.029925 anemoi_datasets-0.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.029925 anemoi_datasets-0.2.1/tests/create/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/create/concat.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/create/data_sources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/create/join.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/create/missing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/create/nan.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/create/pipe.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/create/recentre.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     7695 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/create/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/create-perturbations-full.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/create-shift.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/test_chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)    36578 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tests/test_indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.029925 anemoi_datasets-0.2.1/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tools/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.029925 anemoi_datasets-0.2.1/tools/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tools/examples/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tools/examples/an-oper-2023-2023-2p5-6h-v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:11.029925 anemoi_datasets-0.2.1/tools/grids/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tools/grids/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tools/grids/grids.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tools/grids/grids1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-17 10:22:01.000000 anemoi_datasets-0.2.1/tools/grids/grids2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.507383 anemoi_datasets-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.459382 anemoi_datasets-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.467383 anemoi_datasets-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.467383 anemoi_datasets-0.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/.vscode/spellright.dict
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-05-30 19:12:39.507383 anemoi_datasets-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.467383 anemoi_datasets-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.467383 anemoi_datasets-0.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.467383 anemoi_datasets-0.3.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/_templates/.gitkeep
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/apply-fmt.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.471382 anemoi_datasets-0.3.0/docs/building/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.471382 anemoi_datasets-0.3.0/docs/building/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/filters/empty.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/filters/noop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/filters/rename.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/filters/rotate_winds.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/filters/select.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/filters/unrotate_winds.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/filters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/handling-missing-dates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/handling-missing-values.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/naming-variables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/operations.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.471382 anemoi_datasets-0.3.0/docs/building/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/accumulations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/accumulations1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/accumulations2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/forcings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/forcings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/grib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/hindcasts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/mars.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/mars1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/mars2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/netcdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/netcdf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/opendap.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/opendap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/recentre.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.475382 anemoi_datasets-0.3.0/docs/building/sources/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/yaml/grib1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/yaml/grib2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/yaml/grib3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/yaml/grib4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/yaml/hindcasts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources/yaml/recentre.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/sources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/statistics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/syntax.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/syntax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.475382 anemoi_datasets-0.3.0/docs/building/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/yaml/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/yaml/building1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/yaml/building1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/yaml/building2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/yaml/building2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/yaml/building3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/yaml/building3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/yaml/concat.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/yaml/hindcasts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/yaml/input.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/yaml/missing_dates.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/yaml/nan.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/building/yaml/pipe.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/check-index.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.475382 anemoi_datasets-0.3.0/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/cli/compare.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/cli/copy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/cli/create.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/cli/inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/cli/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/cli/scan.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58982 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/images.pptx
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/overview_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.479383 anemoi_datasets-0.3.0/docs/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   106709 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/schemas/matrix.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)    53069 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/schemas/matrix.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/schemas/overview.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/schemas/overview.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42125 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/schemas/recipe.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)    43845 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/schemas/recipe.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.479383 anemoi_datasets-0.3.0/docs/using/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.487383 anemoi_datasets-0.3.0/docs/using/code/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/area1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/area2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/chain_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/combine_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/concat1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/cutout_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/drop_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/end_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/ensembles1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/frequency_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/grids1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/join1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/matching0_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/matching1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/matching2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/matching3_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/matching4_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/misc1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/misc2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/missing_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/open_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/open_combine1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/open_combine2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/open_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/open_dict_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/open_first_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/open_list_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/open_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/open_other.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/open_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/open_yaml_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/rename_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/reorder1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/reorder2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/select1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/select2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/shuffle_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/some_attributes_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/start_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/statistics_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/subset_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/thinning_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/zip1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/code/zip2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/combining.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/configuration.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/grids.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.487383 anemoi_datasets-0.3.0/docs/using/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   108038 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/images/area-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40564 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/images/concat.png
+-rw-r--r--   0 runner    (1001) docker     (127)   141221 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/images/cutout-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   122139 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/images/cutout-2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   129758 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/images/cutout-3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   151858 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/images/cutout-4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38066 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/images/join.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36070 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/images/overlay.png
+-rw-r--r--   0 runner    (1001) docker     (127)   109206 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/images/thinning-after.png
+-rw-r--r--   0 runner    (1001) docker     (127)   141221 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/images/thinning-before.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/matching.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/methods.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/miscellaneous.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/opening.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/other.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/selecting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/statistics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/docs/using/subsetting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 19:12:39.507383 anemoi_datasets-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.463382 anemoi_datasets-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.463382 anemoi_datasets-0.3.0/src/anemoi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.491383 anemoi_datasets-0.3.0/src/anemoi/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 19:12:39.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.491383 anemoi_datasets-0.3.0/src/anemoi/datasets/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/commands/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/commands/copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/commands/create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.491383 anemoi_datasets-0.3.0/src/anemoi/datasets/commands/inspect/
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/commands/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/commands/inspect/zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/commands/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.491383 anemoi_datasets-0.3.0/src/anemoi/datasets/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/compute/recentre.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.491383 anemoi_datasets-0.3.0/src/anemoi/datasets/create/
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.491383 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.495383 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/filters/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/filters/noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/filters/rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/filters/rotate_winds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/filters/unrotate_winds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.495383 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/accumulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/forcings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/grib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13042 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/hindcasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/mars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/opendap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/recentre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/tendencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27888 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/loaders.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3682 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.495383 anemoi_datasets-0.3.0/src/anemoi/datasets/create/statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/statistics/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/create/zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.499383 anemoi_datasets-0.3.0/src/anemoi/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/debug.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/forewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/masked.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/data/unchecked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.499383 anemoi_datasets-0.3.0/src/anemoi/datasets/dates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/dates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/dates/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/grids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.499383 anemoi_datasets-0.3.0/src/anemoi/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/src/anemoi/datasets/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.503383 anemoi_datasets-0.3.0/src/anemoi_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-05-30 19:12:39.000000 anemoi_datasets-0.3.0/src/anemoi_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-30 19:12:39.000000 anemoi_datasets-0.3.0/src/anemoi_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:12:39.000000 anemoi_datasets-0.3.0/src/anemoi_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 19:12:39.000000 anemoi_datasets-0.3.0/src/anemoi_datasets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-30 19:12:39.000000 anemoi_datasets-0.3.0/src/anemoi_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 19:12:39.000000 anemoi_datasets-0.3.0/src/anemoi_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.503383 anemoi_datasets-0.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.503383 anemoi_datasets-0.3.0/tests/create/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/create/concat.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/create/data_sources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/create/join.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/create/missing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/create/nan.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/create/pipe.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/create/recentre.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7695 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/create/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/create-perturbations-full.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/create-shift.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/test_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36569 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tests/test_indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.503383 anemoi_datasets-0.3.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tools/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.503383 anemoi_datasets-0.3.0/tools/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tools/examples/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tools/examples/an-oper-2023-2023-2p5-6h-v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:12:39.503383 anemoi_datasets-0.3.0/tools/grids/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tools/grids/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tools/grids/grids.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tools/grids/grids1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-30 19:12:30.000000 anemoi_datasets-0.3.0/tools/grids/grids2.yaml
```

### Comparing `anemoi_datasets-0.2.1/.github/workflows/python-publish.yml` & `anemoi_datasets-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/.gitignore` & `anemoi_datasets-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/.pre-commit-config.yaml` & `anemoi_datasets-0.3.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,27 @@
       stages: [commit]
       language: python
       entry: jupyter nbconvert --ClearOutputPreprocessor.enabled=True --inplace
       additional_dependencies: [jupyter]
 
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.4.0
+  rev: v4.6.0
   hooks:
   - id: check-yaml # Check YAML files for syntax errors only
     args: [--unsafe, --allow-multiple-documents]
   - id: debug-statements # Check for debugger imports and py37+ breakpoint()
   - id: end-of-file-fixer # Ensure files end in a newline
   - id: trailing-whitespace # Trailing whitespace checker
-#  - id: no-commit-to-branch # Prevent committing to main / master
+  - id: no-commit-to-branch # Prevent committing to main / master
   - id: check-added-large-files # Check for large files added to git
   - id: check-merge-conflict # Check for files that contain merge conflict
 
 - repo: https://github.com/psf/black-pre-commit-mirror
-  rev: 24.1.1
+  rev: 24.4.2
   hooks:
     - id: black
       args: [--line-length=120]
 
 - repo: https://github.com/pycqa/isort
   rev: 5.13.2
   hooks:
@@ -37,34 +37,45 @@
     args:
     - -l 120
     - --force-single-line-imports
     - --profile black
 
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.3.0
+  rev: v0.4.6
   hooks:
   - id: ruff
     exclude: '(dev/.*|.*_)\.py$'
     args:
     - --line-length=120
     - --fix
     - --exit-non-zero-on-fix
     - --preview
 
-
 - repo: https://github.com/sphinx-contrib/sphinx-lint
   rev: v0.9.1
   hooks:
     - id: sphinx-lint
 
 # For now, we use it. But it does not support a lot of sphinx features
 - repo: https://github.com/dzhu/rstfmt
   rev: v0.0.14
   hooks:
     - id: rstfmt
+      exclude: 'cli/.*' # Because we use argparse
 
 - repo: https://github.com/b8raoult/pre-commit-docconvert
   rev: "0.1.4"
   hooks:
   - id: docconvert
     args: ["numpy"]
+
+- repo: https://github.com/b8raoult/optional-dependencies-all
+  rev: "0.0.2"
+  hooks:
+  - id: optional-dependencies-all
+    args: ["--inplace", "--all-key", "all", "--exclude-keys", "dev,docs"]
+
+- repo: https://github.com/tox-dev/pyproject-fmt
+  rev: "2.1.3"
+  hooks:
+    - id: pyproject-fmt
```

### Comparing `anemoi_datasets-0.2.1/LICENSE` & `anemoi_datasets-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/PKG-INFO` & `anemoi_datasets-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-datasets
-Version: 0.2.1
+Version: 0.3.0
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,64 +201,73 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Project-URL: Homepage, https://github.com/ecmwf/anemoi-datasets/
 Project-URL: Documentation, https://anemoi-datasets.readthedocs.io/
-Project-URL: Repository, https://github.com/ecmwf/anemoi-datasets/
+Project-URL: Homepage, https://github.com/ecmwf/anemoi-datasets/
 Project-URL: Issues, https://github.com/ecmwf/anemoi-datasets/issues
-Keywords: tools,datasets,ai
+Project-URL: Repository, https://github.com/ecmwf/anemoi-datasets/
+Keywords: ai,datasets,tools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: anemoi-utils[provenance]>=0.1.7
-Requires-Dist: zarr<=2.17.0
-Requires-Dist: pyyaml
+Requires-Dist: anemoi-utils[provenance]>=0.3
 Requires-Dist: numpy
-Requires-Dist: tqdm
+Requires-Dist: pyyaml
 Requires-Dist: semantic-version
-Provides-Extra: remote
-Requires-Dist: boto3; extra == "remote"
-Requires-Dist: requests; extra == "remote"
-Requires-Dist: s3fs; extra == "remote"
-Provides-Extra: create
-Requires-Dist: climetlab>=0.22.1; extra == "create"
-Requires-Dist: earthkit-meteo; extra == "create"
-Requires-Dist: pyproj; extra == "create"
-Requires-Dist: ecmwflibs>=0.6.3; extra == "create"
-Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx_rtd_theme; extra == "docs"
-Requires-Dist: nbsphinx; extra == "docs"
-Requires-Dist: pandoc; extra == "docs"
+Requires-Dist: tqdm
+Requires-Dist: zarr<=2.17
 Provides-Extra: all
+Requires-Dist: anemoi-utils[provenance]>=0.3; extra == "all"
 Requires-Dist: boto3; extra == "all"
-Requires-Dist: requests; extra == "all"
-Requires-Dist: s3fs; extra == "all"
 Requires-Dist: climetlab>=0.22.1; extra == "all"
 Requires-Dist: earthkit-meteo; extra == "all"
-Requires-Dist: pyproj; extra == "all"
 Requires-Dist: ecmwflibs>=0.6.3; extra == "all"
+Requires-Dist: numpy; extra == "all"
+Requires-Dist: pyproj; extra == "all"
+Requires-Dist: pyyaml; extra == "all"
+Requires-Dist: requests; extra == "all"
+Requires-Dist: s3fs; extra == "all"
+Requires-Dist: semantic-version; extra == "all"
+Requires-Dist: tqdm; extra == "all"
+Requires-Dist: zarr<=2.17; extra == "all"
+Provides-Extra: create
+Requires-Dist: climetlab>=0.22.1; extra == "create"
+Requires-Dist: earthkit-meteo; extra == "create"
+Requires-Dist: ecmwflibs>=0.6.3; extra == "create"
+Requires-Dist: pyproj; extra == "create"
 Provides-Extra: dev
 Requires-Dist: boto3; extra == "dev"
-Requires-Dist: requests; extra == "dev"
-Requires-Dist: s3fs; extra == "dev"
 Requires-Dist: climetlab>=0.22.1; extra == "dev"
 Requires-Dist: earthkit-meteo; extra == "dev"
-Requires-Dist: pyproj; extra == "dev"
 Requires-Dist: ecmwflibs>=0.6.3; extra == "dev"
-Requires-Dist: sphinx; extra == "dev"
-Requires-Dist: sphinx_rtd_theme; extra == "dev"
 Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: pandoc; extra == "dev"
+Requires-Dist: pyproj; extra == "dev"
+Requires-Dist: requests; extra == "dev"
+Requires-Dist: s3fs; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: sphinx-argparse; extra == "dev"
+Requires-Dist: sphinx-rtd-theme; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: pandoc; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-argparse; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Provides-Extra: remote
+Requires-Dist: boto3; extra == "remote"
+Requires-Dist: requests; extra == "remote"
+Requires-Dist: s3fs; extra == "remote"
```

### Comparing `anemoi_datasets-0.2.1/README.md` & `anemoi_datasets-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/Makefile` & `anemoi_datasets-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/_static/logo.png` & `anemoi_datasets-0.3.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/_static/style.css` & `anemoi_datasets-0.3.0/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/building/handling-missing-dates.rst` & `anemoi_datasets-0.3.0/docs/building/handling-missing-dates.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/building/handling-missing-values.rst` & `anemoi_datasets-0.3.0/docs/building/handling-missing-values.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #########################
  Handling missing values
 #########################
 
-When handling data for machine learning models, missing values (NaNs)
+When handling data for machine learning models, missing values (`NaNs`)
 can pose a challenge, as models require complete data to operate
 effectively and may crash otherwise. Ideally, we anticipate having
-complete data in all fields. However, there are scenarios where NaNs
-naturally occur, such as with variables only relevant on land or at sea
-(such as sea surface temperature (`sst`), for example). In such cases,
-the default behavior is to reject data with NaNs as invalid. To
-accommodate NaNs and accurately compute statistics based on them, you
-can include the `allow_nans` key in the configuration. Here's an example
-of how to implement it:
+complete data in all fields.
+
+However, there are scenarios where `NaNs` naturally occur, such as with
+variables only relevant on land or at sea. This happens for sea surface
+temperature (`sst`), for example. In such cases, the default behavior is
+to reject data with `NaNs` as invalid. To accommodate `NaNs` and
+accurately compute statistics based on them, you can include the
+``allow_nans`` key in the configuration.
+
+Here's an example of how to implement it:
 
 .. literalinclude:: yaml/nan.yaml
    :language: yaml
```

### Comparing `anemoi_datasets-0.2.1/docs/building/introduction.rst` & `anemoi_datasets-0.3.0/docs/building/introduction.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/building/operations.rst` & `anemoi_datasets-0.3.0/docs/building/operations.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/building/sources/accumulations.rst` & `anemoi_datasets-0.3.0/docs/building/sources/accumulations.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 others are accumulated since the last time step (e.g. ERA5).
 
 The `accumulations` has some of that knowledge built-in. If the source
 dataset is unknown, the package assumes that the fields to use are
 accumulated since the beginning of the forecast, over a 6h period.
 
 The user can specify the desired accumulation period with the
-``accumulation_period`` parameter. If its value is a single interger,
-the source will attempt to accumulate the variables over that period.
-This does not always mean that the data used is accumulated from the
+``accumulation_period`` parameter. If its value is a single integer, the
+source will attempt to accumulate the variables over that period. This
+does not always mean that the data used is accumulated from the
 beginning of the forecast, but the most recent data available will be
 used:
 
 -  For ECMWF operational forecasts, the data is accumulated from the
    beginning of the forecast. So if the accumulation period is 6h, for
    the date 2020-01-01 00:00, the source will use the forecast [1]_ of
    2019-12-31 18:00 and the step 6h.
@@ -40,21 +40,21 @@
    for the date for the date 2020-01-01 13:00 the source will use the
    forecast of 2020-01-01 06:00 and the step 1-2h, 2-3h, 3-4h, 4-5h,
    5-6h and 6-7h.
 
 If the of ``accumulation_period`` value is a pair of integers `[step1,
 step2]`, the algorithm is different. The source will compute the
 accumulation between the `step1` and `step2` previous forecast that
-valiate at the given date at `step2`. For example, if the accumulation
+validate at the given date at `step2`. For example, if the accumulation
 period is `[6, 12]`, and the valid date is 2020-10-10 18:00, the source
 will use the forecast of 2020-10-10 06:00 and the steps 6h and 12h.
 
 Please note that ``accumulation_period=6`` and ``accumulation_period=[0,
 6]`` are not equivalent. In the first case, the source can use return an
-accumulation bwteen step 1h and step 7h if it is the most appropriate
+accumulation between step 1h and step 7h if it is the most appropriate
 data available, while in the second case, the source will always return
 the accumulation between step 0h and step 6h, if available.
 
 .. literalinclude:: accumulations1.yaml
    :language: yaml
 
 or:
```

### Comparing `anemoi_datasets-0.2.1/docs/building/sources/forcings.rst` & `anemoi_datasets-0.3.0/docs/building/sources/forcings.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/building/sources/grib.rst` & `anemoi_datasets-0.3.0/docs/building/sources/grib.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/building/sources/hindcasts.rst` & `anemoi_datasets-0.3.0/docs/building/sources/hindcasts.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/building/sources/mars.rst` & `anemoi_datasets-0.3.0/docs/building/sources/mars.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/building/sources/recentre.rst` & `anemoi_datasets-0.3.0/docs/building/sources/recentre.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/building/statistics.rst` & `anemoi_datasets-0.3.0/docs/building/statistics.rst`

 * *Files 26% similar despite different names*

```diff
@@ -4,27 +4,62 @@
  Gathering statistics
 ######################
 
 *Anemoi* will collect statistics about each variables in the dataset as
 it is created. These statistics are intended to be used to normalise the
 data during training.
 
+The statistics are stored in the :doc:`statistics attribute
+<../using/statistics>` of the dataset. The computed statistics include
+`minimum, maximum, mean, standard deviation`.
+
+************************
+ Statistics dates range
+************************
+
 By defaults, the statistics are not computed on the whole dataset, but
-on a subset of dates. The subset is defined using the following
-algorithm:
+on a subset of dates. This usually is done to avoid any data leakage
+from the validation and test sets to the training set.
+
+The dates subset used to compute the statistics is defined using the
+following algorithm:
 
    -  If the dataset covers 20 years or more, the last 3 years are
       excluded.
    -  If the dataset covers 10 years or more, the last year is excluded.
    -  Otherwise, 80% of the dataset is used.
 
-You can override this behaviour by setting the `start` or `end`
-parameters in the `statistics` config.
+You can override this behaviour by setting either the `start` parameter
+or the `end` parameters in the `statistics` config.
+
+Example configuration gathering statistics from 2000 to 2020 :
 
 .. code:: yaml
 
    statistics:
        start: 2000
        end: 2020
 
-..
-   TODO: List the statistics that are computed
+Example configuration gathering statistics from the beginning of the
+dataset period to 2020 :
+
+.. code:: yaml
+
+   statistics:
+       end: 2020
+
+Example configuration gathering statistics using only 2020 data :
+
+.. code:: yaml
+
+   statistics:
+       start: 2020
+       end: 2020
+
+**************************
+ Data with missing values
+**************************
+
+If the dataset contains missing values (known as `NaNs`), an error will
+be raised when trying to compute the statistics. To allow `NaNs` in the
+dataset, you can set the `allow_nans` as described :doc:`here
+</building/handling-missing-values>`.
```

### Comparing `anemoi_datasets-0.2.1/docs/building/yaml/building1.txt` & `anemoi_datasets-0.3.0/docs/building/yaml/building1.txt`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/building/yaml/building2.txt` & `anemoi_datasets-0.3.0/docs/building/yaml/building2.txt`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/building/yaml/building3.txt` & `anemoi_datasets-0.3.0/docs/building/yaml/building3.txt`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/conf.py` & `anemoi_datasets-0.3.0/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.join(os.path.abspath('.'), 'src'))
 
 import datetime
 import os
+import sys
 
 read_the_docs_build = os.environ.get("READTHEDOCS", None) == "True"
 
-# top = os.path.realpath(os.path.dirname(os.path.dirname(__file__)))
-# sys.path.insert(0, top)
+sys.path.insert(0, os.path.join(os.path.abspath(".."), "src"))
 
 
 source_suffix = ".rst"
 master_doc = "index"
 pygments_style = "sphinx"
 html_theme_options = {"logo_only": True}
 html_logo = "_static/logo.png"
@@ -41,28 +41,36 @@
     years = "2024"
 else:
     years = "2024-%s" % (year,)
 
 copyright = "%s, ECMWF" % (years,)
 
 
-release = "0.1.0"
+try:
+    from anemoi.datasets._version import __version__
+
+    release = __version__
+except ImportError:
+    release = "0.0.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.todo",
     "sphinx_rtd_theme",
     "nbsphinx",
     "sphinx.ext.graphviz",
     "sphinx.ext.intersphinx",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.napoleon",
+    "sphinxarg.ext",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 # templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
@@ -108,7 +116,9 @@
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 html_css_files = ["style.css"]
 
 
 todo_include_todos = not read_the_docs_build
+
+autodoc_member_order = "bysource"  # Keep file order
```

### Comparing `anemoi_datasets-0.2.1/docs/images.pptx` & `anemoi_datasets-0.3.0/docs/images.pptx`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/index.rst` & `anemoi_datasets-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/installing.rst` & `anemoi_datasets-0.3.0/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/overview.rst` & `anemoi_datasets-0.3.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/schemas/matrix.excalidraw` & `anemoi_datasets-0.3.0/docs/schemas/matrix.excalidraw`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/schemas/matrix.png` & `anemoi_datasets-0.3.0/docs/schemas/matrix.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/schemas/overview.excalidraw` & `anemoi_datasets-0.3.0/docs/schemas/overview.excalidraw`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/schemas/overview.png` & `anemoi_datasets-0.3.0/docs/schemas/overview.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/schemas/recipe.excalidraw` & `anemoi_datasets-0.3.0/docs/schemas/recipe.excalidraw`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/schemas/recipe.png` & `anemoi_datasets-0.3.0/docs/schemas/recipe.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/test.ipynb` & `anemoi_datasets-0.3.0/docs/test.ipynb`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/combining.rst` & `anemoi_datasets-0.3.0/docs/using/combining.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/configuration.rst` & `anemoi_datasets-0.3.0/docs/using/configuration.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/grids.rst` & `anemoi_datasets-0.3.0/docs/using/grids.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/images/area-1.png` & `anemoi_datasets-0.3.0/docs/using/images/area-1.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/images/concat.png` & `anemoi_datasets-0.3.0/docs/using/images/concat.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/images/cutout-1.png` & `anemoi_datasets-0.3.0/docs/using/images/cutout-1.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/images/cutout-2.png` & `anemoi_datasets-0.3.0/docs/using/images/cutout-2.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/images/cutout-3.png` & `anemoi_datasets-0.3.0/docs/using/images/cutout-3.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/images/cutout-4.png` & `anemoi_datasets-0.3.0/docs/using/images/cutout-4.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/images/join.png` & `anemoi_datasets-0.3.0/docs/using/images/join.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/images/overlay.png` & `anemoi_datasets-0.3.0/docs/using/images/overlay.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/images/thinning-after.png` & `anemoi_datasets-0.3.0/docs/using/images/thinning-after.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/images/thinning-before.png` & `anemoi_datasets-0.3.0/docs/using/images/thinning-before.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/introduction.rst` & `anemoi_datasets-0.3.0/docs/using/introduction.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/matching.rst` & `anemoi_datasets-0.3.0/docs/using/matching.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/methods.rst` & `anemoi_datasets-0.3.0/docs/using/methods.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/miscellaneous.rst` & `anemoi_datasets-0.3.0/docs/using/miscellaneous.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/opening.rst` & `anemoi_datasets-0.3.0/docs/using/opening.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/other.rst` & `anemoi_datasets-0.3.0/docs/using/other.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/selecting.rst` & `anemoi_datasets-0.3.0/docs/using/selecting.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/docs/using/subsetting.rst` & `anemoi_datasets-0.3.0/docs/using/subsetting.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/__init__.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/commands/compare.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/commands/compare.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/commands/copy.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/commands/copy.py`

 * *Files 21% similar despite different names*

```diff
@@ -37,211 +37,269 @@
     s3://ml-datasets/stable/aifs-ea-an-oper-0001-mars-o96-1979-2022-1h-v3.zarr
 
 zinfo https://object-store.os-api.cci1.ecmwf.int/
     ml-datasets/stable/aifs-ea-an-oper-0001-mars-o96-1979-2022-1h-v3.zarr
 """
 
 
-class CopyMixin:
-    internal = True
-    timestamp = True
+class Copier:
+    def __init__(self, source, target, transfers, block_size, overwrite, resume, progress, nested, rechunk, **kwargs):
+        self.source = source
+        self.target = target
+        self.transfers = transfers
+        self.block_size = block_size
+        self.overwrite = overwrite
+        self.resume = resume
+        self.progress = progress
+        self.nested = nested
+        self.rechunk = rechunk
 
-    def add_arguments(self, command_parser):
-        command_parser.add_argument("--transfers", type=int, default=8)
-        command_parser.add_argument("--block-size", type=int, default=100)
-        command_parser.add_argument("--overwrite", action="store_true")
-        command_parser.add_argument("--progress", action="store_true")
-        command_parser.add_argument("--nested", action="store_true", help="Use ZARR's nested directpry backend.")
-        command_parser.add_argument(
-            "--rechunk",
-            nargs="+",
-            help="Rechunk given array.",
-            metavar="array=i,j,k,l",
-        )
-        command_parser.add_argument("source")
-        command_parser.add_argument("target")
+        self.rechunking = rechunk.split(",") if rechunk else []
 
     def _store(self, path, nested=False):
         if nested:
             import zarr
 
             return zarr.storage.NestedDirectoryStore(path)
         return path
 
-    def copy_chunk(self, n, m, source, target, block_size, _copy, progress):
+    def copy_chunk(self, n, m, source, target, _copy, progress):
         if _copy[n:m].all():
             LOG.info(f"Skipping {n} to {m}")
             return None
 
-        for i in tqdm.tqdm(
-            range(n, m),
-            desc=f"Copying {n} to {m}",
-            leave=False,
-            disable=not isatty and not progress,
-        ):
-            target[i] = source[i]
+        if self.block_size % self.data_chunks[0] == 0:
+            target[slice(n, m)] = source[slice(n, m)]
+        else:
+            LOG.warning(
+                f"Block size ({self.block_size}) is not a multiple of target chunk size ({self.data_chunks[0]}). Slow copy expected."
+            )
+            if self.transfers > 1:
+                # race condition, different threads might copy the same data to the same chunk
+                raise NotImplementedError(
+                    "Block size is not a multiple of target chunk size. Parallel copy not supported."
+                )
+            for i in tqdm.tqdm(
+                range(n, m),
+                desc=f"Copying {n} to {m}",
+                leave=False,
+                disable=not isatty and not progress,
+            ):
+                target[i] = source[i]
+
         return slice(n, m)
 
-    def copy_data(self, source, target, transfers, block_size, _copy, progress, rechunking):
+    def parse_rechunking(self, rechunking, source_data):
+        shape = source_data.shape
+        chunks = list(source_data.chunks)
+        for i, c in enumerate(rechunking):
+            if not c:
+                continue
+            elif c == "full":
+                chunks[i] = shape[i]
+            c = int(c)
+            c = min(c, shape[i])
+            chunks[i] = c
+        chunks = tuple(chunks)
+
+        if chunks != source_data.chunks:
+            LOG.info(f"Rechunking data from {source_data.chunks} to {chunks}")
+            # if self.transfers > 1:
+            #    raise NotImplementedError("Rechunking with multiple transfers is not implemented")
+        return chunks
+
+    def copy_data(self, source, target, _copy, progress):
         LOG.info("Copying data")
         source_data = source["data"]
 
-        chunks = list(source_data.chunks)
-        if "data" in rechunking:
-            assert len(chunks) == len(rechunking["data"]), (chunks, rechunking["data"])
-            for i, c in enumerate(rechunking["data"]):
-                if c != -1:
-                    chunks[i] = c
+        self.data_chunks = self.parse_rechunking(self.rechunking, source_data)
 
         target_data = (
             target["data"]
             if "data" in target
             else target.create_dataset(
                 "data",
                 shape=source_data.shape,
-                chunks=chunks,
+                chunks=self.data_chunks,
                 dtype=source_data.dtype,
             )
         )
 
-        executor = ThreadPoolExecutor(max_workers=transfers)
+        executor = ThreadPoolExecutor(max_workers=self.transfers)
         tasks = []
         n = 0
         while n < target_data.shape[0]:
             tasks.append(
                 executor.submit(
                     self.copy_chunk,
                     n,
-                    min(n + block_size, target_data.shape[0]),
+                    min(n + self.block_size, target_data.shape[0]),
                     source_data,
                     target_data,
-                    block_size,
                     _copy,
                     progress,
                 )
             )
-            n += block_size
+            n += self.block_size
 
         for future in tqdm.tqdm(as_completed(tasks), total=len(tasks), smoothing=0):
             copied = future.result()
             if copied is not None:
                 _copy[copied] = True
                 target["_copy"] = _copy
 
         target["_copy"] = _copy
 
         LOG.info("Copied data")
 
-    def copy_array(self, name, source, target, transfers, block_size, _copy, progress, rechunking):
+    def copy_array(self, name, source, target, _copy, progress):
         for k, v in source.attrs.items():
             target.attrs[k] = v
 
         if name == "_copy":
             return
 
         if name == "data":
-            self.copy_data(source, target, transfers, block_size, _copy, progress, rechunking)
+            self.copy_data(source, target, _copy, progress)
             return
 
         LOG.info(f"Copying {name}")
         target[name] = source[name]
         LOG.info(f"Copied {name}")
 
-    def copy_group(self, source, target, transfers, block_size, _copy, progress, rechunking):
+    def copy_group(self, source, target, _copy, progress):
         import zarr
 
         for k, v in source.attrs.items():
             target.attrs[k] = v
 
         for name in sorted(source.keys()):
             if isinstance(source[name], zarr.hierarchy.Group):
                 group = target[name] if name in target else target.create_group(name)
                 self.copy_group(
                     source[name],
                     group,
-                    transfers,
-                    block_size,
                     _copy,
                     progress,
-                    rechunking,
                 )
             else:
                 self.copy_array(
                     name,
                     source,
                     target,
-                    transfers,
-                    block_size,
                     _copy,
                     progress,
-                    rechunking,
                 )
 
-    def copy(self, source, target, transfers, block_size, progress, rechunking):
+    def copy(self, source, target, progress):
         import zarr
 
         if "_copy" not in target:
             target["_copy"] = zarr.zeros(
                 source["data"].shape[0],
                 dtype=bool,
             )
         _copy = target["_copy"]
         _copy_np = _copy[:]
 
-        self.copy_group(source, target, transfers, block_size, _copy_np, progress, rechunking)
+        self.copy_group(source, target, _copy_np, progress)
         del target["_copy"]
 
-    def run(self, args):
+    def run(self):
         import zarr
 
         # base, ext = os.path.splitext(os.path.basename(args.source))
         # assert ext == ".zarr", ext
         # assert "." not in base, base
-        LOG.info(f"Copying {args.source} to {args.target}")
+        LOG.info(f"Copying {self.source} to {self.target}")
 
-        rechunking = {}
-        if args.rechunk:
-            for r in args.rechunk:
-                k, v = r.split("=")
-                if k != "data":
-                    raise ValueError(f"Only rechunking data is supported: {k}")
-                values = v.split(",")
-                values = [-1 if x == "" else x for x in values]
-                values = tuple(int(x) for x in values)
-                rechunking[k] = values
-            for k, v in rechunking.items():
-                LOG.info(f"Rechunking {k} to {v}")
+        def target_exists():
+            try:
+                zarr.open(self._store(self.target), mode="r")
+                return True
+            except ValueError:
+                return False
 
-        try:
-            target = zarr.open(self._store(args.target, args.nested), mode="r")
+        def target_finished():
+            target = zarr.open(self._store(self.target), mode="r")
             if "_copy" in target:
                 done = sum(1 if x else 0 for x in target["_copy"])
                 todo = len(target["_copy"])
                 LOG.info(
                     "Resuming copy, done %s out or %s, %s%%",
                     done,
                     todo,
                     int(done / todo * 100 + 0.5),
                 )
+                return False
             elif "sums" in target and "data" in target:  # sums is copied last
-                LOG.error("Target already exists")
-                return
-        except ValueError as e:
-            LOG.info(f"Target does not exist: {e}")
-            pass
-
-        source = zarr.open(self._store(args.source), mode="r")
-        if args.overwrite:
-            target = zarr.open(self._store(args.target, args.nested), mode="w")
-        else:
-            try:
-                target = zarr.open(self._store(args.target, args.nested), mode="w+")
-            except ValueError:
-                target = zarr.open(self._store(args.target, args.nested), mode="w")
-        self.copy(source, target, args.transfers, args.block_size, args.progress, rechunking)
+                return True
+            return False
+
+        def open_target():
+
+            if not target_exists():
+                return zarr.open(self._store(self.target, self.nested), mode="w")
+
+            if self.overwrite:
+                LOG.error("Target already exists, overwriting.")
+                return zarr.open(self._store(self.target, self.nested), mode="w")
+
+            if self.resume:
+                if target_finished():
+                    LOG.error("Target already exists and is finished.")
+                    sys.exit(0)
+
+                LOG.error("Target already exists, resuming copy.")
+                return zarr.open(self._store(self.target, self.nested), mode="w+")
+
+            LOG.error("Target already exists, use either --overwrite or --resume.")
+            sys.exit(1)
+
+        target = open_target()
+
+        assert target is not None, target
+
+        source = zarr.open(self._store(self.source), mode="r")
+        self.copy(source, target, self.progress)
+
+
+class CopyMixin:
+    internal = True
+    timestamp = True
+
+    def add_arguments(self, command_parser):
+        group = command_parser.add_mutually_exclusive_group()
+        group.add_argument(
+            "--overwrite",
+            action="store_true",
+            help="Overwrite existing dataset. This will delete the target dataset if it already exists. Cannot be used with --resume.",
+        )
+        group.add_argument(
+            "--resume", action="store_true", help="Resume copying an existing dataset. Cannot be used with --overwrite."
+        )
+        command_parser.add_argument("--transfers", type=int, default=8, help="Number of parallel transfers.")
+        command_parser.add_argument(
+            "--progress", action="store_true", help="Force show progress bar, even if not in an interactive shell."
+        )
+        command_parser.add_argument("--nested", action="store_true", help="Use ZARR's nested directpry backend.")
+        command_parser.add_argument(
+            "--rechunk", help="Rechunk the target data array. Rechunk size should be a diviser of the block size."
+        )
+        command_parser.add_argument(
+            "--block-size",
+            type=int,
+            default=100,
+            help="For optimisation purposes, data is transfered by blocks. Default is 100.",
+        )
+        command_parser.add_argument("source", help="Source location.")
+        command_parser.add_argument("target", help="Target location.")
+
+    def run(self, args):
+        Copier(**vars(args)).run()
 
 
 class Copy(CopyMixin, Command):
-    pass
+    """Copy a dataset from one location to another."""
 
 
 command = Copy
```

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/commands/inspect/__init__.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/commands/inspect/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,24 +7,20 @@
 
 
 import os
 
 from .. import Command
 from .zarr import InspectZarr
 
-# from .checkpoint import InspectCheckpoint
-
 
 class Inspect(Command, InspectZarr):
-    # class Inspect(Command, InspectCheckpoint, InspectZarr):
-    """Inspect a checkpoint or zarr file."""
+    """Inspect a zarr dataset."""
 
     def add_arguments(self, command_parser):
         # g = command_parser.add_mutually_exclusive_group()
-        # g.add_argument("--inspect", action="store_true", help="Inspect weights")
         command_parser.add_argument("path", metavar="PATH", nargs="+")
         command_parser.add_argument("--detailed", action="store_true")
         # command_parser.add_argument("--probe", action="store_true")
         command_parser.add_argument("--progress", action="store_true")
         command_parser.add_argument("--statistics", action="store_true")
         command_parser.add_argument("--size", action="store_true", help="Print size")
```

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/commands/inspect/zarr.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/commands/inspect/zarr.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/commands/scan.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/commands/scan.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/compute/recentre.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/compute/recentre.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/__init__.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,24 @@
         self,
         path,
         config=None,
         cache=None,
         print=print,
         statistics_tmp=None,
         overwrite=False,
+        test=None,
         **kwargs,
     ):
         self.path = path  # Output path
         self.config = config
         self.cache = cache
         self.print = print
         self.statistics_tmp = statistics_tmp
         self.overwrite = overwrite
+        self.test = test
 
     def init(self, check_name=False):
         # check path
         _, ext = os.path.splitext(self.path)
         assert ext != "zarr", f"Unsupported extension={ext}"
         from .loaders import InitialiserLoader
 
@@ -39,14 +41,15 @@
 
         with self._cache_context():
             obj = InitialiserLoader.from_config(
                 path=self.path,
                 config=self.config,
                 statistics_tmp=self.statistics_tmp,
                 print=self.print,
+                test=self.test,
             )
             obj.initialise(check_name=check_name)
 
     def load(self, parts=None):
         from .loaders import ContentLoader
 
         with self._cache_context():
```

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/check.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/check.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/chunks.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/chunks.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/config.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/config.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/__init__.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/filters/empty.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/filters/empty.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/filters/rename.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/filters/rename.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/filters/rotate_winds.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/filters/rotate_winds.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/filters/unrotate_winds.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/filters/unrotate_winds.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/accumulations.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/accumulations.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/constants.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/constants.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/forcings.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/forcings.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/grib.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/grib.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/hindcasts.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/hindcasts.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/mars.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/mars.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/netcdf.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/netcdf.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/opendap.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/opendap.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/recentre.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/recentre.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/source.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/source.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/functions/sources/tendencies.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/functions/sources/tendencies.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/input.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/input.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/loaders.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from anemoi.datasets.data.misc import as_first_date
 from anemoi.datasets.data.misc import as_last_date
 from anemoi.datasets.dates.groups import Groups
 
 from .check import DatasetName
 from .check import check_data_values
 from .chunks import ChunkFilter
+from .config import DictObj
 from .config import build_output
 from .config import loader_config
 from .input import build_input
 from .statistics import Summary
 from .statistics import TmpStatistics
 from .statistics import check_variance
 from .statistics import compute_statistics
@@ -51,14 +52,16 @@
         np.seterr(all="raise", under="warn")
 
         assert isinstance(path, str), path
 
         self.path = path
         self.kwargs = kwargs
         self.print = print
+        if "test" in kwargs:
+            self.test = kwargs["test"]
 
     @classmethod
     def from_config(cls, *, config, path, print=print, **kwargs):
         # config is the path to the config file or a dict with the config
         assert isinstance(config, dict) or isinstance(config, str), config
         return cls(config=config, path=path, print=print, **kwargs)
 
@@ -153,15 +156,43 @@
 class InitialiserLoader(Loader):
     def __init__(self, config, **kwargs):
         super().__init__(**kwargs)
         self.main_config = loader_config(config)
 
         self.tmp_statistics.delete()
 
+        if self.test:
+
+            def test_dates(cfg, n=4):
+                LOG.warn("Running in test mode. Changing the list of dates to use only 4.")
+                groups = Groups(**cfg)
+                dates = groups.dates
+                return dict(start=dates[0], end=dates[n - 1], frequency=dates.frequency, group_by=n)
+
+            self.main_config.dates = test_dates(self.main_config.dates)
+
+            def set_to_test_mode(obj):
+                if isinstance(obj, (list, tuple)):
+                    for v in obj:
+                        set_to_test_mode(v)
+                    return
+                if isinstance(obj, (dict, DictObj)):
+                    if "grid" in obj:
+                        obj["grid"] = "20./20."
+                        LOG.warn(f"Running in test mode. Setting grid to {obj['grid']}")
+                    if "number" in obj:
+                        obj["number"] = obj["number"][0:3]
+                        LOG.warn(f"Running in test mode. Setting number to {obj['number']}")
+                    for k, v in obj.items():
+                        set_to_test_mode(v)
+
+            set_to_test_mode(self.main_config)
+
         LOG.info(self.main_config.dates)
+
         self.groups = Groups(**self.main_config.dates)
 
         self.output = build_output(self.main_config.output, parent=self)
         self.input = self.build_input()
 
         LOG.info(self.input)
         all_dates = self.groups.dates
```

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/patch.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/patch.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/persistent.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/persistent.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,15 @@
 
 class PersistentDict:
     version = 3
 
     # Used in parrallel, during data loading,
     # to write data in pickle files.
     def __init__(self, directory, create=True):
-        """dirname: str
-        The directory where the data will be stored.
-        """
+        """dirname: str The directory where the data will be stored."""
         self.dirname = directory
         self.name, self.ext = os.path.splitext(os.path.basename(self.dirname))
         if create:
             self.create()
 
     def create(self):
         os.makedirs(self.dirname, exist_ok=True)
```

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/size.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/size.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/statistics/__init__.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/statistics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 from ..check import check_data_values
 from .summary import Summary
 
 LOG = logging.getLogger(__name__)
 
 
 def default_statistics_dates(dates):
-    """
-    Calculate default statistics dates based on the given list of dates.
+    """Calculate default statistics dates based on the given list of dates.
 
     Args:
         dates (list): List of datetime objects representing dates.
 
     Returns:
         tuple: A tuple containing the default start and end dates.
+
     """
 
     def to_datetime(d):
         if isinstance(d, np.datetime64):
             return d.tolist()
         assert isinstance(d, datetime.datetime), d
         return d
```

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/statistics/summary.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/statistics/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 
 from ..check import StatisticsValueError
 from ..check import check_data_values
 from ..check import check_stats
 
 
 class Summary(dict):
-    """This class is used to store the summary statistics of a dataset.
-    It can be saved and loaded from a json file.
-    And does some basic checks on the data.
-    """
+    """This class is used to store the summary statistics of a dataset. It can be saved and loaded from a json file. And does some basic checks on the data."""
 
     STATS_NAMES = [
         "minimum",
         "maximum",
         "mean",
         "stdev",
         "has_nans",
```

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/template.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/template.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/utils.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/utils.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/writer.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 
 LOG = logging.getLogger(__name__)
 
 
 class ViewCacheArray:
     """A class that provides a caching mechanism for writing to a NumPy-like array.
 
-    The is initialized with a NumPy-like array, a shape and a list to reindex the first dimension.
-    The array is used to store the final data, while the cache is used to temporarily
-    store the data before flushing it to the array.
+    The is initialized with a NumPy-like array, a shape and a list to reindex the first
+    dimension. The array is used to store the final data, while the cache is used to
+    temporarily store the data before flushing it to the array.
 
     The `flush` method copies the contents of the cache to the final array.
+
     """
 
     def __init__(self, array, *, shape, indexes):
         assert len(indexes) == shape[0], (len(indexes), shape[0])
         self.array = array
         self.dtype = array.dtype
         self.cache = np.full(shape, np.nan, dtype=self.dtype)
```

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/create/zarr.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/create/zarr.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/__init__.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/concat.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/concat.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/dataset.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/dataset.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/debug.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/debug.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/ensemble.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/ensemble.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/forewards.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/forewards.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/grids.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/grids.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/indexing.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/indexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,17 +115,15 @@
 
         return i
 
     return tuple(_(i) for i in index)
 
 
 def expand_list_indexing(method):
-    """Allows to use slices, lists, and tuples to select data from the dataset.
-    Zarr does not support indexing with lists/arrays directly, so we need to implement it ourselves.
-    """
+    """Allows to use slices, lists, and tuples to select data from the dataset. Zarr does not support indexing with lists/arrays directly, so we need to implement it ourselves."""
 
     @wraps(method)
     def wrapper(self, index):
         if not isinstance(index, tuple):
             return method(self, index)
 
         if not any(isinstance(i, (list, tuple)) for i in index):
```

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/join.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/join.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/masked.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/masked.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/misc.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/misc.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/select.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/select.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/statistics.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/statistics.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/stores.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/stores.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,15 @@
         raise NotImplementedError()
 
     def __iter__(self):
         raise NotImplementedError()
 
 
 class HTTPStore(ReadOnlyStore):
-    """We write our own HTTPStore because the one used by zarr (fsspec) does not play
-    well with fork() and multiprocessing.
-    """
+    """We write our own HTTPStore because the one used by zarr (fsspec) does not play well with fork() and multiprocessing."""
 
     def __init__(self, url):
         self.url = url
 
     def __getitem__(self, key):
         import requests
 
@@ -55,17 +53,15 @@
             raise KeyError(key)
 
         r.raise_for_status()
         return r.content
 
 
 class S3Store(ReadOnlyStore):
-    """We write our own S3Store because the one used by zarr (fsspec) does not play well
-    with fork() and multiprocessing.
-    """
+    """We write our own S3Store because the one used by zarr (fsspec) does not play well with fork() and multiprocessing."""
 
     def __init__(self, url):
         import boto3
 
         self.bucket, self.key = url[5:].split("/", 1)
 
         # TODO: get the profile name from the url
```

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/subset.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/subset.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/data/unchecked.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/data/unchecked.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,15 @@
 
     def __call__(self, method):
         name = method.__name__
         check = self.check
 
         @wraps(method)
         def wrapper(obj):
-            """
-            This is a decorator that checks the compatibility of the datasets
-            before calling the method. If the datasets are compatible, it
-            will return the result of the method, otherwise it will raise an
-            exception.
-            """
+            """This is a decorator that checks the compatibility of the datasets before calling the method. If the datasets are compatible, it will return the result of the method, otherwise it will raise an exception."""
 
             for d in obj.datasets[1:]:
                 getattr(obj, check)(obj.datasets[0], d)
 
             return getattr(Combined, name).__get__(obj)
 
         return wrapper
```

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/dates/__init__.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/dates/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/dates/groups.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/dates/groups.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi/datasets/grids.py` & `anemoi_datasets-0.3.0/src/anemoi/datasets/grids.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/src/anemoi_datasets.egg-info/PKG-INFO` & `anemoi_datasets-0.3.0/src/anemoi_datasets.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-datasets
-Version: 0.2.1
+Version: 0.3.0
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,64 +201,73 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Project-URL: Homepage, https://github.com/ecmwf/anemoi-datasets/
 Project-URL: Documentation, https://anemoi-datasets.readthedocs.io/
-Project-URL: Repository, https://github.com/ecmwf/anemoi-datasets/
+Project-URL: Homepage, https://github.com/ecmwf/anemoi-datasets/
 Project-URL: Issues, https://github.com/ecmwf/anemoi-datasets/issues
-Keywords: tools,datasets,ai
+Project-URL: Repository, https://github.com/ecmwf/anemoi-datasets/
+Keywords: ai,datasets,tools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: anemoi-utils[provenance]>=0.1.7
-Requires-Dist: zarr<=2.17.0
-Requires-Dist: pyyaml
+Requires-Dist: anemoi-utils[provenance]>=0.3
 Requires-Dist: numpy
-Requires-Dist: tqdm
+Requires-Dist: pyyaml
 Requires-Dist: semantic-version
-Provides-Extra: remote
-Requires-Dist: boto3; extra == "remote"
-Requires-Dist: requests; extra == "remote"
-Requires-Dist: s3fs; extra == "remote"
-Provides-Extra: create
-Requires-Dist: climetlab>=0.22.1; extra == "create"
-Requires-Dist: earthkit-meteo; extra == "create"
-Requires-Dist: pyproj; extra == "create"
-Requires-Dist: ecmwflibs>=0.6.3; extra == "create"
-Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx_rtd_theme; extra == "docs"
-Requires-Dist: nbsphinx; extra == "docs"
-Requires-Dist: pandoc; extra == "docs"
+Requires-Dist: tqdm
+Requires-Dist: zarr<=2.17
 Provides-Extra: all
+Requires-Dist: anemoi-utils[provenance]>=0.3; extra == "all"
 Requires-Dist: boto3; extra == "all"
-Requires-Dist: requests; extra == "all"
-Requires-Dist: s3fs; extra == "all"
 Requires-Dist: climetlab>=0.22.1; extra == "all"
 Requires-Dist: earthkit-meteo; extra == "all"
-Requires-Dist: pyproj; extra == "all"
 Requires-Dist: ecmwflibs>=0.6.3; extra == "all"
+Requires-Dist: numpy; extra == "all"
+Requires-Dist: pyproj; extra == "all"
+Requires-Dist: pyyaml; extra == "all"
+Requires-Dist: requests; extra == "all"
+Requires-Dist: s3fs; extra == "all"
+Requires-Dist: semantic-version; extra == "all"
+Requires-Dist: tqdm; extra == "all"
+Requires-Dist: zarr<=2.17; extra == "all"
+Provides-Extra: create
+Requires-Dist: climetlab>=0.22.1; extra == "create"
+Requires-Dist: earthkit-meteo; extra == "create"
+Requires-Dist: ecmwflibs>=0.6.3; extra == "create"
+Requires-Dist: pyproj; extra == "create"
 Provides-Extra: dev
 Requires-Dist: boto3; extra == "dev"
-Requires-Dist: requests; extra == "dev"
-Requires-Dist: s3fs; extra == "dev"
 Requires-Dist: climetlab>=0.22.1; extra == "dev"
 Requires-Dist: earthkit-meteo; extra == "dev"
-Requires-Dist: pyproj; extra == "dev"
 Requires-Dist: ecmwflibs>=0.6.3; extra == "dev"
-Requires-Dist: sphinx; extra == "dev"
-Requires-Dist: sphinx_rtd_theme; extra == "dev"
 Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: pandoc; extra == "dev"
+Requires-Dist: pyproj; extra == "dev"
+Requires-Dist: requests; extra == "dev"
+Requires-Dist: s3fs; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: sphinx-argparse; extra == "dev"
+Requires-Dist: sphinx-rtd-theme; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: pandoc; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-argparse; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Provides-Extra: remote
+Requires-Dist: boto3; extra == "remote"
+Requires-Dist: requests; extra == "remote"
+Requires-Dist: s3fs; extra == "remote"
```

### Comparing `anemoi_datasets-0.2.1/src/anemoi_datasets.egg-info/SOURCES.txt` & `anemoi_datasets-0.3.0/src/anemoi_datasets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,16 @@
 docs/building/sources/opendap.rst
 docs/building/sources/opendap.yaml
 docs/building/sources/recentre.rst
 docs/building/sources/yaml/grib1.yaml
 docs/building/sources/yaml/grib2.yaml
 docs/building/sources/yaml/grib3.yaml
 docs/building/sources/yaml/grib4.yaml
-docs/building/sources/yaml/perturbations.yaml
+docs/building/sources/yaml/hindcasts.yaml
+docs/building/sources/yaml/recentre.yaml
 docs/building/yaml/Makefile
 docs/building/yaml/building1.txt
 docs/building/yaml/building1.yaml
 docs/building/yaml/building2.txt
 docs/building/yaml/building2.yaml
 docs/building/yaml/building3.txt
 docs/building/yaml/building3.yaml
@@ -70,14 +71,15 @@
 docs/building/yaml/nan.yaml
 docs/building/yaml/pipe.yaml
 docs/cli/compare.rst
 docs/cli/copy.rst
 docs/cli/create.rst
 docs/cli/inspect.rst
 docs/cli/introduction.rst
+docs/cli/scan.rst
 docs/schemas/matrix.excalidraw
 docs/schemas/matrix.png
 docs/schemas/overview.excalidraw
 docs/schemas/overview.png
 docs/schemas/recipe.excalidraw
 docs/schemas/recipe.png
 docs/using/combining.rst
```

### Comparing `anemoi_datasets-0.2.1/tests/create/concat.yaml` & `anemoi_datasets-0.3.0/tests/create/concat.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/tests/create/join.yaml` & `anemoi_datasets-0.3.0/tests/create/join.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/tests/create/pipe.yaml` & `anemoi_datasets-0.3.0/tests/create/pipe.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/tests/create/recentre.yaml` & `anemoi_datasets-0.3.0/tests/create/recentre.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/tests/create/test_create.py` & `anemoi_datasets-0.3.0/tests/create/test_create.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/tests/create-perturbations-full.yaml` & `anemoi_datasets-0.3.0/tests/create-perturbations-full.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/tests/create-shift.yaml` & `anemoi_datasets-0.3.0/tests/create-shift.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/tests/test_chunks.py` & `anemoi_datasets-0.3.0/tests/test_chunks.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/tests/test_data.py` & `anemoi_datasets-0.3.0/tests/test_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,17 +38,15 @@
                 return func(*args, **kwargs)
 
     return wrapper
 
 
 @cache
 def _(date, var, k=0, e=0, values=VALUES):
-    """Create a simple array of values based on the date and variable name, ensemble,
-    grid and a few other parameters.
-    """
+    """Create a simple array of values based on the date and variable name, ensemble, grid and a few other parameters."""
     d = date.year * 10000 + date.month * 100 + date.day
     v = ord(var) - ord("a") + 1
     assert 0 <= k <= 9
     assert 0 <= e <= 9
 
     return np.array([d * 100 + v + k / 10.0 + w / 100.0 + e / 1000.0 for w in range(values)])
```

### Comparing `anemoi_datasets-0.2.1/tests/test_dates.py` & `anemoi_datasets-0.3.0/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/tests/test_indexing.py` & `anemoi_datasets-0.3.0/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/tools/examples/an-oper-2023-2023-2p5-6h-v1.yaml` & `anemoi_datasets-0.3.0/tools/examples/an-oper-2023-2023-2p5-6h-v1.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/tools/grids/grids.ipynb` & `anemoi_datasets-0.3.0/tools/grids/grids.ipynb`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/tools/grids/grids1.yaml` & `anemoi_datasets-0.3.0/tools/grids/grids1.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.2.1/tools/grids/grids2.yaml` & `anemoi_datasets-0.3.0/tools/grids/grids2.yaml`

 * *Files identical despite different names*

