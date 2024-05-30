# Comparing `tmp/neurocarto-0.0.1.tar.gz` & `tmp/neurocarto-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocarto-0.0.1.tar", last modified: Wed May 22 11:44:31 2024, max compression
+gzip compressed data, was "neurocarto-0.0.2.tar", last modified: Thu May 30 10:32:59 2024, max compression
```

## Comparing `neurocarto-0.0.1.tar` & `neurocarto-0.0.2.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.464270 neurocarto-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-22 11:44:26.000000 neurocarto-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-22 11:44:31.464270 neurocarto-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-22 11:44:26.000000 neurocarto-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-22 11:44:26.000000 neurocarto-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 11:44:26.000000 neurocarto-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:44:31.464270 neurocarto-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.448269 neurocarto-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.452270 neurocarto-0.0.1/src/neurocarto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    26678 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/main_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/main_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    19276 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.456270 neurocarto-0.0.1/src/neurocarto/probe_npx/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15643 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/desp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/npx.py
--rw-r--r--   0 runner    (1001) docker     (127)    25808 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/select_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/select_weaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/select_weaker_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/stat.py
--rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11716 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.456270 neurocarto-0.0.1/src/neurocarto/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/_atlas_brain_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/atlas_brain.py
--rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/atlas_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/atlas_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/bokeh_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/bokeh_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.460270 neurocarto-0.0.1/src/neurocarto/util/edit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14208 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/atlas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/checking.py
--rw-r--r--   0 runner    (1001) docker     (127)     9238 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/moving.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/probe.py
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/surrounding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/probe_coor.py
--rw-r--r--   0 runner    (1001) docker     (127)    59633 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/util_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/util_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.464270 neurocarto-0.0.1/src/neurocarto/views/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25781 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/atlas.py
--rw-r--r--   0 runner    (1001) docker     (127)    26276 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (127)    22668 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/blueprint_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/data_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/image_npy.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/image_plt.matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/image_plt.py
--rw-r--r--   0 runner    (1001) docker     (127)    18870 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/probe.py
--rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/view_efficient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.464270 neurocarto-0.0.1/src/neurocarto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-22 11:44:31.000000 neurocarto-0.0.1/src/neurocarto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-22 11:44:31.000000 neurocarto-0.0.1/src/neurocarto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:44:31.000000 neurocarto-0.0.1/src/neurocarto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 11:44:31.000000 neurocarto-0.0.1/src/neurocarto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 11:44:31.000000 neurocarto-0.0.1/src/neurocarto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 11:44:31.000000 neurocarto-0.0.1/src/neurocarto.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.464270 neurocarto-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-22 11:44:26.000000 neurocarto-0.0.1/tests/test_electrode_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-05-22 11:44:26.000000 neurocarto-0.0.1/tests/test_npx_probe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-22 11:44:26.000000 neurocarto-0.0.1/tests/test_probe_oper.py
--rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-22 11:44:26.000000 neurocarto-0.0.1/tests/test_util_blueprint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:32:59.427060 neurocarto-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-30 10:32:55.000000 neurocarto-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-30 10:32:59.427060 neurocarto-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-30 10:32:55.000000 neurocarto-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-30 10:32:55.000000 neurocarto-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 10:32:55.000000 neurocarto-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:32:59.427060 neurocarto-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:32:59.411060 neurocarto-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:32:59.415060 neurocarto-0.0.2/src/neurocarto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26678 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/main_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/main_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19276 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:32:59.419060 neurocarto-0.0.2/src/neurocarto/probe_npx/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe_npx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15657 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe_npx/desp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe_npx/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe_npx/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe_npx/npx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25808 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe_npx/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe_npx/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe_npx/select_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe_npx/select_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe_npx/select_weaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe_npx/select_weaker_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe_npx/stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe_npx/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11716 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/probe_npx/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:32:59.419060 neurocarto-0.0.2/src/neurocarto/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/_atlas_brain_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/atlas_brain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/atlas_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/atlas_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/bokeh_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/bokeh_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:32:59.423060 neurocarto-0.0.2/src/neurocarto/util/edit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16883 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14208 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9238 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/moving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/edit/surrounding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/probe_coor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60442 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/util_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/util_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:32:59.427060 neurocarto-0.0.2/src/neurocarto/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25781 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26276 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22668 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/blueprint_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/data_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/image_npy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/image_plt.matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/image_plt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-30 10:32:55.000000 neurocarto-0.0.2/src/neurocarto/views/view_efficient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:32:59.427060 neurocarto-0.0.2/src/neurocarto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-30 10:32:59.000000 neurocarto-0.0.2/src/neurocarto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-30 10:32:59.000000 neurocarto-0.0.2/src/neurocarto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:32:59.000000 neurocarto-0.0.2/src/neurocarto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 10:32:59.000000 neurocarto-0.0.2/src/neurocarto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 10:32:59.000000 neurocarto-0.0.2/src/neurocarto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 10:32:59.000000 neurocarto-0.0.2/src/neurocarto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:32:59.427060 neurocarto-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-30 10:32:55.000000 neurocarto-0.0.2/tests/test_electrode_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-05-30 10:32:55.000000 neurocarto-0.0.2/tests/test_npx_probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-30 10:32:55.000000 neurocarto-0.0.2/tests/test_probe_oper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-30 10:32:55.000000 neurocarto-0.0.2/tests/test_util_blueprint.py
```

### Comparing `neurocarto-0.0.1/LICENSE` & `neurocarto-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/PKG-INFO` & `neurocarto-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocarto
-Version: 0.0.1
+Version: 0.0.2
 Summary: A web-interface channelmap editor for Neuropixels probe familiy
 Author-email: Ta-Shun Su <antoniost29@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, AntonioST
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `neurocarto-0.0.1/README.md` & `neurocarto-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/pyproject.toml` & `neurocarto-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # https://packaging.python.org/en/latest/tutorials/packaging-projects/
 # https://packaging.python.org/en/latest/guides/writing-pyproject-toml
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 
 [project]
 name = 'neurocarto'
-version = '0.0.1'
+version = '0.0.2'
 authors = [
     { name = "Ta-Shun Su", email = "antoniost29@gmail.com" },
 ]
 description = "A web-interface channelmap editor for Neuropixels probe familiy"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
```

### Comparing `neurocarto-0.0.1/src/neurocarto/config.py` & `neurocarto-0.0.2/src/neurocarto/config.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/files.py` & `neurocarto-0.0.2/src/neurocarto/files.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/main_app.py` & `neurocarto-0.0.2/src/neurocarto/main_app.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/main_index.py` & `neurocarto-0.0.2/src/neurocarto/main_index.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/probe.py` & `neurocarto-0.0.2/src/neurocarto/probe.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/probe_npx/desp.py` & `neurocarto-0.0.2/src/neurocarto/probe_npx/desp.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
         :param shank_width_scale:
         :param label_axis:
         :param kwargs:
         :see: {ProbePlotElectrodeProtocol}, {plot_electrode_block()}, {plot_probe_shape()}
         """
         from .plot import plot_electrode_block, plot_probe_shape
 
-        plot_electrode_block(ax, chmap, data, electrode_unit='raw', shank_width_scale=shank_width_scale, **kwargs)
+        plot_electrode_block(ax, chmap, data, electrode_unit='raw', shank_width_scale=shank_width_scale, sparse=False, **kwargs)
         plot_probe_shape(ax, chmap, color=probe_color, shank_width_scale=shank_width_scale, label_axis=label_axis, **kwargs)
 
         if not label_axis:
             ax.set_xlabel(None)
             ax.set_xticks([])
             ax.set_xticklabels([])
             ax.set_ylabel(None)
```

### Comparing `neurocarto-0.0.1/src/neurocarto/probe_npx/io.py` & `neurocarto-0.0.2/src/neurocarto/probe_npx/io.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/probe_npx/npx.py` & `neurocarto-0.0.2/src/neurocarto/probe_npx/npx.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/probe_npx/plot.py` & `neurocarto-0.0.2/src/neurocarto/probe_npx/plot.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/probe_npx/select.py` & `neurocarto-0.0.2/src/neurocarto/probe_npx/select.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/probe_npx/select_default.py` & `neurocarto-0.0.2/src/neurocarto/probe_npx/select_default.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/probe_npx/select_weaker.py` & `neurocarto-0.0.2/src/neurocarto/probe_npx/select_weaker.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/probe_npx/select_weaker_debug.py` & `neurocarto-0.0.2/src/neurocarto/probe_npx/select_weaker_debug.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/probe_npx/stat.py` & `neurocarto-0.0.2/src/neurocarto/probe_npx/stat.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,29 +86,30 @@
     if channelmap is None:
         channelmap = bp.channelmap
 
     if blueprint is None:
         blueprint = bp._blueprint
 
     electrode = npx_request_electrode(bp, blueprint)
+    total = channelmap.probe_type.n_channels
+    unused = total - len(channelmap)
     channel = 0
     excluded = 0
-    total = channelmap.probe_type.n_channels
 
     selected = blueprint[bp.selected_electrodes(channelmap)]
     for category, count in zip(*np.unique(selected, return_counts=True)):
         match category:
             case NpxProbeDesp.CATE_SET | NpxProbeDesp.CATE_FULL | NpxProbeDesp.CATE_HALF | NpxProbeDesp.CATE_QUARTER:
                 channel += count
             case NpxProbeDesp.CATE_EXCLUDED:
                 excluded += count
 
     ae = 0 if electrode == 0 else max(channel / electrode, 0)
     ce = 0 if ae == 0 else min(ae, 1 / ae)
-    ex = (total - excluded) / total
+    ex = (total - excluded - unused) / total
     return ae, ce * ex
 
 
 class ElectrodeProbability(NamedTuple):
     sample_times: int
     """number of sample times"""
     summation: NDArray[np.int_]
@@ -199,15 +200,15 @@
         for t in chmap.electrodes:
             mat[t.shank, t.column, t.row] += 1
 
         if probe.is_valid(chmap):
             complete += 1
 
         bp.set_blueprint(blueprint)
-        channel_efficiency.append(npx_channel_efficiency(bp)[1])
+        channel_efficiency.append(npx_channel_efficiency(bp, chmap)[1])
 
     return ElectrodeProbability(sample_times, mat, complete, np.array(channel_efficiency))
 
 
 def _npx_electrode_probability_n(probe: NpxProbeDesp, chmap: ChannelMap, blueprint: list[NpxElectrodeDesp],
                                  selector: ElectrodeSelector,
                                  sample_times: int,
```

### Comparing `neurocarto-0.0.1/src/neurocarto/probe_npx/utils.py` & `neurocarto-0.0.2/src/neurocarto/probe_npx/utils.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/probe_npx/views.py` & `neurocarto-0.0.2/src/neurocarto/probe_npx/views.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/_atlas_brain_type.py` & `neurocarto-0.0.2/src/neurocarto/util/_atlas_brain_type.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/atlas_brain.py` & `neurocarto-0.0.2/src/neurocarto/util/atlas_brain.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/atlas_slice.py` & `neurocarto-0.0.2/src/neurocarto/util/atlas_slice.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/atlas_struct.py` & `neurocarto-0.0.2/src/neurocarto/util/atlas_struct.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/bokeh_app.py` & `neurocarto-0.0.2/src/neurocarto/util/bokeh_app.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/bokeh_util.py` & `neurocarto-0.0.2/src/neurocarto/util/bokeh_util.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/debug.py` & `neurocarto-0.0.2/src/neurocarto/util/debug.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/edit/_actions.py` & `neurocarto-0.0.2/src/neurocarto/util/edit/_actions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Literal
 
 import numpy as np
-
 from neurocarto.probe_npx import NpxProbeDesp, utils
 from neurocarto.util.edit.checking import use_probe, use_view
 from neurocarto.util.util_blueprint import BlueprintFunctions
 
 if TYPE_CHECKING:
     from neurocarto.util.probe_coor import ProbeCoordinate
     from neurocarto.views.atlas import Label
@@ -33,35 +32,84 @@
     :param bp:
     :param row: (int=0) start row in um.
     """
     bp.set_channelmap(utils.npx24_stripe(row, um=True))
 
 
 @use_probe(NpxProbeDesp, 24)
-def npx24_half_density(bp: BlueprintFunctions, shank: int | list[int] = 0, row: int = 0):
+def npx24_half_density(bp: BlueprintFunctions, shank: int | list[int] | Literal['selected'] = 0, row: int = 0):
     """
     Make a channelmap for 4-shank Neuropixels probe that uniformly distributes channels in *half* density.
 
     :param bp:
-    :param shank: (int|[int, int]=0) on which shank/s.
+    :param shank: (int|[int, int]|'selected'=0) on which shank/s.
+        Use 'select' for selected electrodes.
     :param row: (int=0) start row in um.
     """
-    bp.set_channelmap(utils.npx24_half_density(shank, row, um=True))
+    match shank:
+        case 'selected':
+            if len(electrodes := bp.captured_electrodes(all=True)) < 4:
+                bp.log_message('need capture more electrodes')
+                return
+
+            # npx 24 arrange electrode in S-R-C ordering
+            match row % 2:
+                case 0:
+                    mask = (electrodes % 4 == 0) | (electrodes % 4 == 3)
+                case 1:
+                    mask = (electrodes % 4 == 1) | (electrodes % 4 == 2)
+                case _:
+                    raise RuntimeError('unreachable')
+
+            bp.add_electrodes(electrodes[mask])
+            bp.clear_capture_electrode()
+
+        case int() | [int(), int()] | (int(), int()):
+            bp.set_channelmap(utils.npx24_half_density(shank, row, um=True))
+        case _:
+            raise ValueError()
 
 
 @use_probe(NpxProbeDesp, 24)
-def npx24_quarter_density(bp: BlueprintFunctions, shank: int | list[int] | None = None, row: int = 0):
+def npx24_quarter_density(bp: BlueprintFunctions, shank: int | list[int] | Literal['selected'] | None = None, row: int = 0):
     """
     Make a channelmap for 4-shank Neuropixels probe that uniformly distributes channels in *quarter* density.
 
     :param bp:
-    :param shank: (int|[int, int]=None) on which shank/s. use ``None`` for four shanks.
+    :param shank: (int|[int, int]|'selected'=None) on which shank/s.
+        Use 'select' for selected electrodes.
+        Use ``None`` for four shanks.
     :param row: (int=0) start row in um.
     """
-    bp.set_channelmap(utils.npx24_quarter_density(shank, row, um=True))
+    match shank:
+        case 'selected':
+            if len(electrodes := bp.captured_electrodes(all=True)) < 8:
+                bp.log_message('need capture more electrodes')
+                return
+
+            # npx 24 arrange electrode in S-R-C ordering
+            match row % 4:
+                case 0:
+                    mask = (electrodes % 8 == 0) | (electrodes % 8 == 5)
+                case 1:
+                    mask = (electrodes % 8 == 1) | (electrodes % 8 == 4)
+                case 2:
+                    mask = (electrodes % 8 == 2) | (electrodes % 8 == 7)
+                case 3:
+                    mask = (electrodes % 8 == 3) | (electrodes % 8 == 6)
+                case _:
+                    raise RuntimeError('unreachable')
+
+            bp.add_electrodes(electrodes[mask])
+            bp.clear_capture_electrode()
+
+        case None | int() | [int(), int()] | (int(), int()):
+            bp.set_channelmap(utils.npx24_quarter_density(shank, row, um=True))
+        case _:
+            raise ValueError()
 
 
 @use_probe(NpxProbeDesp, 24)
 def npx24_one_eighth_density(bp: BlueprintFunctions, row: int = 0):
     """
     Make a channelmap for 4-shank Neuropixels probe that uniformly distributes channels in *one-eighth* density.
 
@@ -413,14 +461,15 @@
     X = NpxProbeDesp.CATE_EXCLUDED
 
     bp.log_message(f'min={np.nanmin(data)}, max={np.nanmax(data)}')
 
     data = bp.interpolate_nan(data)
     bp.draw(data)
 
+    bp.clear_blueprint()
     bp[np.isnan(data)] = X
     bp.reduce(X, 20, bi=False)
     bp.fill(X, gap=None, threshold=10, unset=True)
 
     bp[data >= threshold] = F
 
     bp.fill(F, gap=None)
```

### Comparing `neurocarto-0.0.1/src/neurocarto/util/edit/actions.py` & `neurocarto-0.0.2/src/neurocarto/util/edit/actions.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/edit/atlas.py` & `neurocarto-0.0.2/src/neurocarto/util/edit/atlas.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/edit/category.py` & `neurocarto-0.0.2/src/neurocarto/util/edit/category.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/edit/checking.py` & `neurocarto-0.0.2/src/neurocarto/util/edit/checking.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/edit/clustering.py` & `neurocarto-0.0.2/src/neurocarto/util/edit/clustering.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/edit/data.py` & `neurocarto-0.0.2/src/neurocarto/util/edit/data.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/edit/debug.py` & `neurocarto-0.0.2/src/neurocarto/util/edit/debug.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/edit/moving.py` & `neurocarto-0.0.2/src/neurocarto/util/edit/moving.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/edit/optimize.py` & `neurocarto-0.0.2/src/neurocarto/util/edit/optimize.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/edit/plot.py` & `neurocarto-0.0.2/src/neurocarto/util/edit/plot.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/edit/probe.py` & `neurocarto-0.0.2/src/neurocarto/util/edit/probe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 import textwrap
 from typing import Any, Literal
 
 import numpy as np
-from numpy.typing import NDArray
-
 from neurocarto.probe import ProbeDesp, ElectrodeDesp, M
 from neurocarto.util.util_blueprint import BlueprintFunctions
 from neurocarto.util.utils import SPHINX_BUILD, doc_link
 from neurocarto.views.base import ControllerView
+from numpy.typing import NDArray
 
 if SPHINX_BUILD:
     ProbeView = 'neurocarto.views.probe.ProbeView'
 
 __all__ = [
     'new_channelmap',
     'capture_electrode',
+    'clear_capture_electrode',
     'captured_electrodes',
     'set_state_for_captured',
     'set_category_for_captured',
     'refresh_selection',
     'select_electrodes',
 ]
 
@@ -59,23 +59,32 @@
         case _:
             raise ValueError(f'unknown mode "{mode}"')
 
     captured = [electrodes[it] for it in captured]
 
     view = controller.get_app().probe_view
     if state is None:
-        view.set_captured_electrodes(captured)
+        view.set_capture_electrodes(captured)
     else:
         for s in state:
             try:
                 data = view.data_electrodes[s]
             except KeyError:
                 pass
             else:
-                view.set_captured_electrodes(captured, data)
+                view.set_capture_electrodes(captured, data)
+
+
+@doc_link(DOC=textwrap.dedent(BlueprintFunctions.clear_capture_electrode.__doc__))
+def clear_capture_electrode(controller: ControllerView):
+    """
+    {DOC}
+    :see: {BlueprintFunctions#clear_capture_electrode()}
+    """
+    controller.get_app().probe_view.clear_capture_electrode()
 
 
 @doc_link(DOC=textwrap.dedent(BlueprintFunctions.captured_electrodes.__doc__))
 def captured_electrodes(controller: ControllerView, all=False) -> NDArray[np.int_]:
     """
     {DOC}
     :see: {BlueprintFunctions#captured_electrodes()}
```

### Comparing `neurocarto-0.0.1/src/neurocarto/util/edit/script.py` & `neurocarto-0.0.2/src/neurocarto/util/edit/script.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/edit/surrounding.py` & `neurocarto-0.0.2/src/neurocarto/util/edit/surrounding.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/probe_coor.py` & `neurocarto-0.0.2/src/neurocarto/util/probe_coor.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/util_blueprint.py` & `neurocarto-0.0.2/src/neurocarto/util/util_blueprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 import functools
 import sys
 from collections.abc import Callable, Sequence
 from pathlib import Path
 from typing import TYPE_CHECKING, overload, Generic, Final, Any, Literal
 
 import numpy as np
-from numpy.typing import NDArray
-
 from neurocarto.probe import ProbeDesp, M, E, get_probe_desp
-from neurocarto.util.edit.checking import use_probe
+from neurocarto.util.edit.checking import use_probe, use_view
 from neurocarto.util.utils import doc_link, SPHINX_BUILD
 from neurocarto.views.base import ControllerView, V
+from numpy.typing import NDArray
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 if TYPE_CHECKING:
@@ -39,15 +38,15 @@
     ELECTRODES = list[E]
 
 
     class BLUEPRINT:
         """Prevent sphinx from printing BLUEPRINT as ``ndarray[int64]``"""
         pass
 
-__all__ = ['BlueprintFunctions', 'ClusteringEdges', 'blueprint_function', 'use_probe']
+__all__ = ['BlueprintFunctions', 'ClusteringEdges', 'blueprint_function', 'use_probe', 'use_view']
 
 
 def maybe_blueprint(self: BlueprintFunctions, a):
     """
     Is *a* a blueprint?
 
     :param self:
@@ -125,14 +124,15 @@
     .. hlist::
         :columns: 2
 
         * {#blueprint()}
         * {#new_blueprint()}
         * {#blueprint_changed}
         * {#set_blueprint()}
+        * {#clear_blueprint()}
         * {#apply_blueprint()}
         * {#from_blueprint()}
         * {#index_blueprint()}
         * {#load_blueprint()}
         * {#save_blueprint()}
         * {#set()}
         * {#unset()}
@@ -167,14 +167,15 @@
 
     Call methods from {ProbeView}.
 
     .. hlist::
         :columns: 2
 
         * {#capture_electrode()}
+        * {#clear_capture_electrode()}
         * {#captured_electrodes()}
         * {#set_state_for_captured()}
         * {#set_category_for_captured()}
         * {#refresh_selection()}
 
     **Atlas Brain image view functions**
 
@@ -378,18 +379,20 @@
         """
         if (channelmap := self.channelmap) is None:
             raise RuntimeError('probe missing')
 
         electrodes = self.electrodes
         if isinstance(e, (int, np.integer)):
             es = [electrodes[int(e)]]
+        elif len(e) == 0:  # empty array
+            return
         elif isinstance(e, (list, tuple)):
             es = [electrodes[int(it)] for it in e]
         else:
-            es = [electrodes[int(it)] for it in np.arange((len(electrodes)))[e]]
+            es = [electrodes[int(it)] for it in np.arange(len(electrodes))[e]]
 
         for t in es:
             self.probe.add_electrode(channelmap, t, overwrite=overwrite)
 
     @doc_link()
     def del_electrodes(self, e: int | list[int] | NDArray[np.int_] | NDArray[np.bool_]):
         """
@@ -401,18 +404,20 @@
         """
         if (channelmap := self.channelmap) is None:
             raise RuntimeError('probe missing')
 
         electrodes = self.electrodes
         if isinstance(e, (int, np.integer)):
             es = [electrodes[int(e)]]
+        elif len(e) == 0:  # empty array
+            return
         elif isinstance(e, (list, tuple)):
             es = [electrodes[int(it)] for it in e]
         else:
-            es = [electrodes[int(it)] for it in np.arange((len(electrodes)))[e]]
+            es = [electrodes[int(it)] for it in np.arange(len(electrodes))[e]]
 
         for t in es:
             self.probe.del_electrode(channelmap, t)
 
     @doc_link()
     def selected_electrodes(self, chmap=None) -> NDArray[np.int_]:
         """
@@ -518,14 +523,25 @@
 
         if len(blueprint) != len(self.s):
             raise ValueError()
 
         self._blueprint = blueprint
         self._blueprint_changed = True
 
+    def clear_blueprint(self) -> BLUEPRINT:
+        """
+        unset blueprint.
+
+        :return: previous blueprint before clearing
+        """
+        ret = self.blueprint()
+        self._blueprint = self.new_blueprint()
+        self._blueprint_changed = True
+        return ret
+
     @doc_link()
     def apply_blueprint(self, electrodes: ELECTRODES = None, blueprint: BLUEPRINT = None) -> ELECTRODES:
         """
         Apply blueprint back to electrode list.
 
         :param electrodes: electrode list
         :param blueprint:
@@ -1274,14 +1290,25 @@
         :see: {ProbeView#set_captured_electrodes()}
         """
         from .edit.probe import capture_electrode
         if (controller := self._controller) is not None:
             capture_electrode(self, controller, index, state, mode)
 
     @doc_link()
+    def clear_capture_electrode(self):
+        """
+        clear capturing.
+
+        :see: {ProbeView#clear_capture_electrode()}
+        """
+        from .edit.probe import clear_capture_electrode
+        if (controller := self._controller) is not None:
+            clear_capture_electrode(controller)
+
+    @doc_link()
     def captured_electrodes(self, all=False) -> NDArray[np.int_]:
         """
         get captured electrodes.
 
         :param all: capture excluded electrodes?
         :return: index of captured electrodes.
         :see: {ProbeView#get_captured_electrodes_index()}
```

### Comparing `neurocarto-0.0.1/src/neurocarto/util/util_numpy.py` & `neurocarto-0.0.2/src/neurocarto/util/util_numpy.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/util/utils.py` & `neurocarto-0.0.2/src/neurocarto/util/utils.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/views/atlas.py` & `neurocarto-0.0.2/src/neurocarto/views/atlas.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/views/base.py` & `neurocarto-0.0.2/src/neurocarto/views/base.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/views/blueprint.py` & `neurocarto-0.0.2/src/neurocarto/views/blueprint.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/views/blueprint_script.py` & `neurocarto-0.0.2/src/neurocarto/views/blueprint_script.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/views/data.py` & `neurocarto-0.0.2/src/neurocarto/views/data.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/views/data_density.py` & `neurocarto-0.0.2/src/neurocarto/views/data_density.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/views/image.py` & `neurocarto-0.0.2/src/neurocarto/views/image.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/views/image_npy.py` & `neurocarto-0.0.2/src/neurocarto/views/image_npy.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/views/image_plt.py` & `neurocarto-0.0.2/src/neurocarto/views/image_plt.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/views/probe.py` & `neurocarto-0.0.2/src/neurocarto/views/probe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from __future__ import annotations
 
 from collections.abc import Iterable
 from typing import Any, TypedDict, Generic, TYPE_CHECKING
 
 from bokeh.models import ColumnDataSource, GlyphRenderer, tools, UIElement, Div
-from typing_extensions import Required
-
 from neurocarto.config import CartoConfig
 from neurocarto.probe import ProbeDesp, M, E
 from neurocarto.util.bokeh_app import run_timeout
 from neurocarto.util.bokeh_util import as_callback
 from neurocarto.util.debug import TimeMarker
 from neurocarto.util.utils import doc_link
 from neurocarto.views.base import Figure, ViewBase, RecordView, RecordStep
+from typing_extensions import Required
 
 if TYPE_CHECKING:
     from bokeh.server.callbacks import TimeoutCallback
 
 __all__ = ['ProbeView']
 
 
@@ -287,28 +286,35 @@
             selected_index = d.selected.indices
             if reset:
                 d.selected.indices = []
 
             e = d.data['e']
             return [e[it] for it in selected_index]
 
-    def set_captured_electrodes(self, electrodes: list[int] | list[E], d: ColumnDataSource = None):
+    def set_capture_electrodes(self, electrodes: list[int] | list[E], d: ColumnDataSource = None):
         if d is None:
             for data in self.data_electrodes.values():
-                self.set_captured_electrodes(electrodes, data)
+                self.set_capture_electrodes(electrodes, data)
         else:
             i = set([
                 it if isinstance(it, int) else self._e2i[it]
                 for it in electrodes
             ])
 
             e = d.data['e']
             s = [ii for ii, ie in enumerate(e) if ie in i]
             d.selected.indices = s
 
+    def clear_capture_electrode(self, d: ColumnDataSource = None):
+        if d is None:
+            for data in self.data_electrodes.values():
+                self.clear_capture_electrode(data)
+        else:
+            d.selected.indices = []
+
     _captured_electrodes: list[E] = []
     _captured_callback: TimeoutCallback | None = None
 
     def _on_capture(self, state: int):
         selected = self.get_captured_electrodes(self.data_electrodes[state])
         self._captured_electrodes.extend(selected)
         if self._captured_callback is None:
```

### Comparing `neurocarto-0.0.1/src/neurocarto/views/record.py` & `neurocarto-0.0.2/src/neurocarto/views/record.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/views/utils.py` & `neurocarto-0.0.2/src/neurocarto/views/utils.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto/views/view_efficient.py` & `neurocarto-0.0.2/src/neurocarto/views/view_efficient.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/src/neurocarto.egg-info/PKG-INFO` & `neurocarto-0.0.2/src/neurocarto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocarto
-Version: 0.0.1
+Version: 0.0.2
 Summary: A web-interface channelmap editor for Neuropixels probe familiy
 Author-email: Ta-Shun Su <antoniost29@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, AntonioST
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `neurocarto-0.0.1/src/neurocarto.egg-info/SOURCES.txt` & `neurocarto-0.0.2/src/neurocarto.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 src/neurocarto/probe_npx/desp.py
 src/neurocarto/probe_npx/io.py
 src/neurocarto/probe_npx/meta.py
 src/neurocarto/probe_npx/npx.py
 src/neurocarto/probe_npx/plot.py
 src/neurocarto/probe_npx/select.py
 src/neurocarto/probe_npx/select_default.py
+src/neurocarto/probe_npx/select_random.py
 src/neurocarto/probe_npx/select_weaker.py
 src/neurocarto/probe_npx/select_weaker_debug.py
 src/neurocarto/probe_npx/stat.py
 src/neurocarto/probe_npx/utils.py
 src/neurocarto/probe_npx/views.py
 src/neurocarto/util/__init__.py
 src/neurocarto/util/_atlas_brain_type.py
```

### Comparing `neurocarto-0.0.1/tests/test_electrode_select.py` & `neurocarto-0.0.2/tests/test_electrode_select.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/tests/test_npx_probe.py` & `neurocarto-0.0.2/tests/test_npx_probe.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/tests/test_probe_oper.py` & `neurocarto-0.0.2/tests/test_probe_oper.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.1/tests/test_util_blueprint.py` & `neurocarto-0.0.2/tests/test_util_blueprint.py`

 * *Files identical despite different names*

