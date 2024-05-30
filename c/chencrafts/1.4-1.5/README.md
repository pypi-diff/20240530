# Comparing `tmp/chencrafts-1.4.tar.gz` & `tmp/chencrafts-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chencrafts-1.4.tar", last modified: Thu May 16 20:46:42 2024, max compression
+gzip compressed data, was "chencrafts-1.5.tar", last modified: Thu May 30 01:23:29 2024, max compression
```

## Comparing `chencrafts-1.4.tar` & `chencrafts-1.5.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:46:42.509821 chencrafts-1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:46:42.497820 chencrafts-1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:46:42.501820 chencrafts-1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-16 20:46:38.000000 chencrafts-1.4/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-16 20:46:38.000000 chencrafts-1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-16 20:46:38.000000 chencrafts-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 20:46:38.000000 chencrafts-1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-16 20:46:42.509821 chencrafts-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-16 20:46:38.000000 chencrafts-1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:46:42.501820 chencrafts-1.4/chencrafts/
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:46:42.505821 chencrafts-1.4/chencrafts/bsqubits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:46:42.505821 chencrafts-1.4/chencrafts/bsqubits/QEC_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/bsqubits/QEC_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38778 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/bsqubits/QEC_graph/cat_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/bsqubits/QEC_graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/bsqubits/QEC_graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/bsqubits/QEC_graph/node.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/bsqubits/QEC_graph/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/bsqubits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/bsqubits/batched_custom_sweeps.py
--rw-r--r--   0 runner    (1001) docker     (127)     9917 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/bsqubits/cat_ideal.py
--rw-r--r--   0 runner    (1001) docker     (127)    19213 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/bsqubits/cat_real.py
--rw-r--r--   0 runner    (1001) docker     (127)    31255 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/bsqubits/derive_var.py
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/bsqubits/error_rates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/bsqubits/pulse_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26739 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/bsqubits/systems.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:46:42.505821 chencrafts-1.4/chencrafts/cqed/
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/block_diag.py
--rw-r--r--   0 runner    (1001) docker     (127)    28529 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/crit_photon_num.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:46:42.509821 chencrafts-1.4/chencrafts/cqed/custom_sweeps/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/custom_sweeps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/custom_sweeps/crit_photon_num.py
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/custom_sweeps/decoherence.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/custom_sweeps/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/custom_sweeps/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/decoherence.py
--rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/flexible_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)    12715 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/mode_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/pulses.py
--rw-r--r--   0 runner    (1001) docker     (127)    14020 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/qt_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/scq_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/spec_poly_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/special_states.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/cqed/symbolic_bosons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:46:42.509821 chencrafts-1.4/chencrafts/projects/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    78060 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/projects/fluxonium_tunable_coupler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/projects/protomon_disorder.py
--rw-r--r--   0 runner    (1001) docker     (127)    36649 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/projects/protomon_full_disorder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:46:42.509821 chencrafts-1.4/chencrafts/toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/toolbox/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/toolbox/gadgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    41421 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/toolbox/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/toolbox/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/toolbox/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-16 20:46:38.000000 chencrafts-1.4/chencrafts/toolbox/useless.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-16 20:46:42.000000 chencrafts-1.4/chencrafts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:46:42.509821 chencrafts-1.4/chencrafts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-16 20:46:42.000000 chencrafts-1.4/chencrafts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-16 20:46:42.000000 chencrafts-1.4/chencrafts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:46:42.000000 chencrafts-1.4/chencrafts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-16 20:46:42.000000 chencrafts-1.4/chencrafts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 20:46:42.000000 chencrafts-1.4/chencrafts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-16 20:46:38.000000 chencrafts-1.4/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-16 20:46:38.000000 chencrafts-1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:46:42.509821 chencrafts-1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:46:42.509821 chencrafts-1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-16 20:46:38.000000 chencrafts-1.4/tests/test_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:23:29.786979 chencrafts-1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:23:29.774979 chencrafts-1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:23:29.774979 chencrafts-1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-30 01:23:22.000000 chencrafts-1.5/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-30 01:23:22.000000 chencrafts-1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-30 01:23:22.000000 chencrafts-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-30 01:23:22.000000 chencrafts-1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-30 01:23:29.786979 chencrafts-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-30 01:23:22.000000 chencrafts-1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:23:29.774979 chencrafts-1.5/chencrafts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:23:29.778979 chencrafts-1.5/chencrafts/bsqubits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:23:29.778979 chencrafts-1.5/chencrafts/bsqubits/QEC_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/QEC_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38778 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/QEC_graph/cat_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/QEC_graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/QEC_graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/QEC_graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/QEC_graph/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/batched_custom_sweeps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/batched_sweeps_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/cat_ideal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19213 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/cat_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31255 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/derive_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/error_rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/pulse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26739 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/bsqubits/systems.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:23:29.782979 chencrafts-1.5/chencrafts/cqed/
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/block_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28529 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/crit_photon_num.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:23:29.782979 chencrafts-1.5/chencrafts/cqed/custom_sweeps/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/custom_sweeps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/custom_sweeps/crit_photon_num.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/custom_sweeps/decoherence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/custom_sweeps/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/custom_sweeps/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/decoherence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11410 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/flexible_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/floquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/mode_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/pulses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14020 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/qt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/scq_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/spec_poly_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/special_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/cqed/symbolic_bosons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:23:29.782979 chencrafts-1.5/chencrafts/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78060 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/projects/fluxonium_tunable_coupler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/projects/protomon_disorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36649 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/projects/protomon_full_disorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:23:29.782979 chencrafts-1.5/chencrafts/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/toolbox/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/toolbox/gadgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41421 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/toolbox/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/toolbox/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/toolbox/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-30 01:23:22.000000 chencrafts-1.5/chencrafts/toolbox/useless.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-30 01:23:29.000000 chencrafts-1.5/chencrafts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:23:29.782979 chencrafts-1.5/chencrafts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-30 01:23:29.000000 chencrafts-1.5/chencrafts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-30 01:23:29.000000 chencrafts-1.5/chencrafts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 01:23:29.000000 chencrafts-1.5/chencrafts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 01:23:29.000000 chencrafts-1.5/chencrafts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 01:23:29.000000 chencrafts-1.5/chencrafts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-30 01:23:22.000000 chencrafts-1.5/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-30 01:23:22.000000 chencrafts-1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 01:23:29.786979 chencrafts-1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:23:29.782979 chencrafts-1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-30 01:23:22.000000 chencrafts-1.5/tests/test_optimization.py
```

### Comparing `chencrafts-1.4/.github/workflows/publish_to_pypi.yml` & `chencrafts-1.5/.github/workflows/publish_to_pypi.yml`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
     - name: Sign the dists with Sigstore
-      uses: sigstore/gh-action-sigstore-python@v1.2.3
+      uses: sigstore/gh-action-sigstore-python@v2.1.1
       with:
         inputs: >-
           ./dist/*.tar.gz
           ./dist/*.whl
     - name: Create GitHub Release
       env:
         GITHUB_TOKEN: ${{ github.token }}
```

### Comparing `chencrafts-1.4/LICENSE` & `chencrafts-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/PKG-INFO` & `chencrafts-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chencrafts
-Version: 1.4
+Version: 1.5
 Summary: A personal toolbox for superconducting qubits and quantum mechanics.
 Author-email: Danyang Chen <DanyangChen2026@u.northwestern.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2024 and later, Danyang Chen
         All rights reserved.
```

### Comparing `chencrafts-1.4/README.md` & `chencrafts-1.5/README.md`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/__init__.py` & `chencrafts-1.5/chencrafts/__init__.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/bsqubits/QEC_graph/__init__.py` & `chencrafts-1.5/chencrafts/bsqubits/QEC_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/bsqubits/QEC_graph/cat_tree.py` & `chencrafts-1.5/chencrafts/bsqubits/QEC_graph/cat_tree.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/bsqubits/QEC_graph/edge.py` & `chencrafts-1.5/chencrafts/bsqubits/QEC_graph/edge.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/bsqubits/QEC_graph/graph.py` & `chencrafts-1.5/chencrafts/bsqubits/QEC_graph/graph.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/bsqubits/QEC_graph/node.py` & `chencrafts-1.5/chencrafts/bsqubits/QEC_graph/node.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/bsqubits/__init__.py` & `chencrafts-1.5/chencrafts/bsqubits/__init__.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/bsqubits/batched_custom_sweeps.py` & `chencrafts-1.5/chencrafts/bsqubits/batched_custom_sweeps.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
     - swept parameters
     - sweep[<name>]
     - kwargs[<name>] (kwargs of this function)
     """
     # some parameters for use
     qubit_dim = sweep.hilbertspace.subsystem_dims[qubit_mode_idx]
     params = kwargs | sweep.parameters.meshgrid_by_name() 
-
     
     # cavity relaxation
     sweep.store_data(
         kappa_s = PI2 * sweep["omega_s_GHz"] / params["Q_s"]
     )
     sweep.store_data(
         n_th_s = n_th(sweep["omega_s_GHz"], params["temp_s"], params["n_th_base"])
```

### Comparing `chencrafts-1.4/chencrafts/bsqubits/cat_ideal.py` & `chencrafts-1.5/chencrafts/bsqubits/cat_ideal.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,18 +66,23 @@
 
     return _res_qubit_tensor(res_oprt, qubit_oprt, res_mode_idx)
     
 def _qubit_proj(
     res_dim: int, qubit_dim: int,
     res_mode_idx: Literal[0, 1] = 0,
     qubit_state: int = 0,
+    qubit_state_2: int | None = None,
 ) -> qt.Qobj:
     """For qubit measurement"""
     res_oprt = qt.qeye(res_dim)
-    qubit_oprt = qt.projection(qubit_dim, qubit_state, qubit_state)
+    
+    if qubit_state_2 is not None:
+        qubit_oprt = qt.projection(qubit_dim, qubit_state, qubit_state_2)
+    else:
+        qubit_oprt = qt.projection(qubit_dim, qubit_state, qubit_state)
 
     return _res_qubit_tensor(res_oprt, qubit_oprt, res_mode_idx)
 
 def _res_rotation(
     res_dim: int, qubit_dim: int,
     res_mode_idx: Literal[0, 1] = 0,
     angle: float = np.pi / 2,
```

### Comparing `chencrafts-1.4/chencrafts/bsqubits/cat_real.py` & `chencrafts-1.5/chencrafts/bsqubits/cat_real.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/bsqubits/derive_var.py` & `chencrafts-1.5/chencrafts/bsqubits/derive_var.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/bsqubits/error_rates.py` & `chencrafts-1.5/chencrafts/bsqubits/error_rates.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/bsqubits/pulse_utils.py` & `chencrafts-1.5/chencrafts/bsqubits/pulse_utils.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/bsqubits/systems.py` & `chencrafts-1.5/chencrafts/bsqubits/systems.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/cqed/__init__.py` & `chencrafts-1.5/chencrafts/cqed/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,25 +51,30 @@
 
 from chencrafts.cqed.mode_assignment import (
     label_convert,
     organize_dressed_esys,
     single_mode_dressed_esys,
     two_mode_dressed_esys,
     dressed_state_component,
+    branch_analysis,
 )
 
 from chencrafts.cqed.special_states import (
     coherent,
     cat,
 )
 
 from chencrafts.cqed.flexible_sweep import (
     FlexibleSweep,
 )
 
+from chencrafts.cqed.floquet import (
+    FloquetBasis,
+)
+
 from chencrafts.cqed.spec_poly_fit import (
     spec_poly_fit,
 )
 
 from chencrafts.cqed.crit_photon_num import (
     n_crit_by_diag,
     n_crit_by_1st_pert,
@@ -128,20 +133,23 @@
     "purcell_factor",
 
     "label_convert",
     "organize_dressed_esys",
     "single_mode_dressed_esys",
     "two_mode_dressed_esys",
     "dressed_state_component",
+    "branch_analysis",
 
     "coherent",
     "cat",
 
     "FlexibleSweep",
 
+    "FloquetBasis",
+
     "spec_poly_fit",
 
     "n_crit_by_diag",
     "n_crit_by_1st_pert",
     "n_crit_by_diag_subspace",
     "n_crit_by_diag_subspace_w_hilbertspace",
```

### Comparing `chencrafts-1.4/chencrafts/cqed/block_diag.py` & `chencrafts-1.5/chencrafts/cqed/block_diag.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/cqed/crit_photon_num.py` & `chencrafts-1.5/chencrafts/cqed/crit_photon_num.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/cqed/custom_sweeps/crit_photon_num.py` & `chencrafts-1.5/chencrafts/cqed/custom_sweeps/crit_photon_num.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/cqed/custom_sweeps/decoherence.py` & `chencrafts-1.5/chencrafts/cqed/custom_sweeps/decoherence.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/cqed/custom_sweeps/utils.py` & `chencrafts-1.5/chencrafts/cqed/custom_sweeps/utils.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/cqed/decoherence.py` & `chencrafts-1.5/chencrafts/cqed/decoherence.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/cqed/flexible_sweep.py` & `chencrafts-1.5/chencrafts/cqed/flexible_sweep.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 
 from scqubits.core.hilbert_space import HilbertSpace
 from scqubits.core.param_sweep import ParameterSweep, StateLabel
 from scqubits.core.namedslots_array import NamedSlotsNdarray, Parameters
 from scqubits.core.storage import SpectrumData
 
 from chencrafts.cqed.scq_helper import meshgrid_by_name
+from chencrafts.cqed.mode_assignment import branch_analysis
 
 import numpy as np
 from warnings import warn
 
-from typing import Dict, List, Tuple, Callable, Any, Literal
+from typing import Dict, List, Tuple, Callable, Any, Literal, Optional
 
 class FlexibleSweep():   
     """
     FlexibleSweep is a wrapper of scq.ParameterSweep. 
         - It allows for flexible parameter sweeping by defining fixed and swept 
             parameters. 
         - It will take `update_hilbertspace_by_keyword` as an input of the sweep
     """
     def __init__(
         self,
         hilbertspace: HilbertSpace,
         para: Dict[str, float] = {"dummy": 0.0},    # a dummy parameter
         swept_para: Dict[str, List[float] | np.ndarray] = {"dummy": [0.0]},   # a dummy parameter
         update_hilbertspace_by_keyword: Callable | None = None,
-        evals_count: int = 4,
+        evals_count: Optional[int] = None,
         num_cpus: int = 1,
         subsys_update_info: Dict[str, Any] = {},
         default_update_info: List | Literal["all"] | None = "all",
         **kwargs,
     ):
         """
         FlexibleSweep is a wrapper of scq.ParameterSweep. 
@@ -82,14 +83,15 @@
         self._complete_param_dict = self._get_complete_param_dict()
         _parameters = self._order_swept_para()
         self._swept_para_meshgrids = meshgrid_by_name(_parameters)
         self.dims = _parameters.counts
         self.hilbertspace = hilbertspace
         self._subsys_update_info = self._all_subsys_update_info(subsys_update_info, default_update_info)
         self._update_hilbertspace_by_keyword = update_hilbertspace_by_keyword
+        evals_count = evals_count if evals_count is not None else self.hilbertspace.dimension
 
         # ParameterSweep
         self.sweep = ParameterSweep(
             hilbertspace=self.hilbertspace,
             paramvals_by_name=self._complete_param_dict,
             update_hilbertspace=self._build_update_hilbertspace_func(),
             evals_count=evals_count,
@@ -267,8 +269,21 @@
     def dressed_indices(self, bare_indices: Tuple[int, ...]) -> np.ndarray:
         """
         A wrapper of scq.ParameterSweep.dressed_indices. It helps to to ravel
         the bare indices.
         """
         raveled_idx = np.ravel_multi_index(bare_indices, self.hilbertspace.subsystem_dims)
         return self["dressed_indices"][..., raveled_idx]
-    
+    
+    def branch_analysis(self, mode_priority: Optional[List[int]] = None):
+        branch_indices = branch_analysis(
+            self.sweep, mode_priority
+        )
+        self.sweep.store_data(
+            dressed_indices = branch_indices.reshape(1, -1)
+        )
+        (
+            self.sweep._data["lamb"],
+            self.sweep._data["chi"],
+            self.sweep._data["kerr"],
+            self.sweep._data["chi_prime"],      # only in Danyang's branch of scqubits
+        ) = self.sweep._dispersive_coefficients()
```

### Comparing `chencrafts-1.4/chencrafts/cqed/mode_assignment.py` & `chencrafts-1.5/chencrafts/cqed/mode_assignment.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import numpy as np
 import qutip as qt
 
 from scqubits.core.hilbert_space import HilbertSpace
+from scqubits.core.spec_lookup import MixinCompatible, SpectrumLookupMixin
+from scqubits.core.namedslots_array import NamedSlotsNdarray
 
 from warnings import warn
-from typing import List, Tuple, Any, overload
+import itertools
+from typing import List, Tuple, Any, overload, Optional
 
 @overload
 def label_convert(
     idx: Tuple[int, ...] | List[int],
     h_space: HilbertSpace | None = None, 
     dims: Tuple[int, ...] | List[int] | None = None
 ) -> np.intp:
@@ -331,7 +334,209 @@
         prob_list.append(prob)
 
     if truncate is not None:
         bare_label_list = bare_label_list[:truncate]
         prob_list = prob_list[:truncate]
 
     return bare_label_list, prob_list
+
+def _single_branch_analysis(
+    self: SpectrumLookupMixin,   # hilbertspace
+    mode_priority: List[int],
+    recusion_depth: int,
+    init_drs_idx: int, init_state: qt.Qobj, 
+    remaining_drs_indices: List[int], remaining_evecs: List[qt.Qobj], 
+):
+    """
+    Perform a single branch analysis according to Dumas et al. (2024). This 
+    is a core function to be run recursively.
+
+    In a nutshell, the function will:
+    1. Start from the "ground" state / starting point the branch, find
+    all of the branch states
+    2. Remove the found states from the remaining candidates
+    3. [If at the end of the depth-first search] Return the branch states
+    4. [If not at the end] For each branch state, use it as an init state to 
+    start such search again, which will return a (nested) list of branch 
+    states. Combine the list of branch states and return a nested list of
+    those states
+
+    In such way, the function will recursively go through this multi-dimensional
+    Hilbert space and assign the eigenstates to their labels.
+
+    Parameters
+    ----------
+    self:
+        SpectrumLookupMixin object, could be a `ParameterSweep` object or 
+        `HilbertSpace` object.
+    mode_priority:
+        A permutation of the mode indices. 
+        It represents the depth of the mode labels to be traversed. The later
+        the mode appears in the list, the deeper it is in the recursion.
+        For the last mode in the list, its states will be organized in a 
+        single branch - the innermost part of the nested list. 
+    recusion_depth:
+        The current depth of the recursion. It should be 0 at the beginning.
+    init_drs_idx:
+        The dressed index of the initial state of this branch.
+    init_state:
+        The initial state of this branch.
+    remaining_drs_indices:
+        The list of the remaining dressed indices to be assigned.
+    remaining_evecs:
+        The list of the remaining eigenstates to be assigned.
+    
+    Returns
+    -------
+    branch_drs_indices, branch_states
+        The (nested) list of the branch states and their dressed indices.
+    """
+
+    hspace = self.hilbertspace
+    mode_index = mode_priority[recusion_depth]
+    mode = hspace.subsystem_list[mode_index]
+    terminate_branch_length = hspace.subsystem_dims[mode_index]
+
+    # photon addition operator
+    if mode in hspace.osc_subsys_list:
+        excite_op = hspace.annihilate(mode).dag()
+    else:
+        # for this moment, have the same operator for both cases
+        excite_op = hspace.annihilate(mode).dag()
+
+    # loop over and find all states that matches the excited initial state
+    current_state = init_state
+    current_drs_idx = init_drs_idx
+    branch_drs_indices = []
+    branch_states = []
+    while True:
+        if recusion_depth == len(mode_priority) - 1:
+            # we are at the end of the depth-first search:
+            # just add the state to the branch
+            branch_drs_indices.append(current_drs_idx)
+            branch_states.append(current_state)
+        else:
+            # continue the depth-first search:
+            # recursively call the function and append all the branch states
+            (
+                _branch_drs_indices, _branch_states
+            ) = _single_branch_analysis(
+                self, 
+                mode_priority, 
+                recusion_depth + 1,
+                current_drs_idx,
+                current_state, 
+                remaining_drs_indices,
+                remaining_evecs, 
+            )
+            branch_drs_indices.append(_branch_drs_indices)
+            branch_states.append(_branch_states)
+
+        # if the branch is long enough, terminate the loop
+        if len(branch_states) == terminate_branch_length:
+            break
+
+        # find the closest state to the excited current state
+        if len(remaining_evecs) == 0:
+            raise ValueError(
+                "No more states to assign. It's likely that the eignestates "
+                "are not complete. Please try obtain a complete set of "
+                "eigenstates using generate_lookup."
+            )
+
+        excited_state = (excite_op * current_state).unit()
+        overlaps = [np.abs(excited_state.overlap(evec)) for evec in remaining_evecs]
+        max_overlap_index = np.argmax(overlaps)
+
+        current_state = remaining_evecs[max_overlap_index]
+        current_drs_idx = remaining_drs_indices[max_overlap_index]
+
+        # remove the state from the remaining states
+        remaining_evecs.pop(max_overlap_index)
+        remaining_drs_indices.pop(max_overlap_index)
+
+    return branch_drs_indices, branch_states
+
+def generate_branch_analysis(
+    self: SpectrumLookupMixin,   # hilbertspace
+    param_indices: Tuple[int, ...],
+    mode_priority: Optional[List[int]] = None,
+    transpose: bool = False,
+):
+    """
+    Perform a full branch analysis according to Dumas et al. (2024) for 
+    a single parameter point. This
+    function will organize the eigenstates into a multi-dimensional array
+    according to the mode_priority. 
+
+    Parameters
+    ----------
+    self:
+        SpectrumLookupMixin object, could be a `ParameterSweep` object or 
+        `HilbertSpace` object.
+    param_indices:
+        The indices of the parameter sweep to be analyzed.
+    mode_priority:
+        A permutation of the mode indices. 
+        It represents the depth of the mode labels to be traversed. The later
+        the mode appears in the list, the deeper it is in the recursion.
+        For the last mode in the list, its states will be organized in a 
+        single branch - the innermost part of the nested list.
+    transpose:
+        If True, the returned array will be transposed according to the
+        mode_priority. 
+
+    Returns
+    -------
+    branch_drs_indices
+        The multi-dimensional array of the dressed indices organized by 
+        the mode_priority. If the dimensions of the subsystems are
+        D0, D1 and D2, the returned array will have the shape (D0, D1, D2).
+        If transposed is True, the array will be transposed according to
+        the mode_priority.
+    """
+    if mode_priority is None:
+        mode_priority = list(range(self.hilbertspace.subsystem_count))
+    
+    # branch_states = np.ndarray(self.hilbertspace.subsystem_dims, dtype=object)
+    # branch_drs_indices = np.ndarray(self.hilbertspace.subsystem_dims, dtype=int)
+
+    evecs = self._data["evecs"][param_indices]
+    init_state = evecs[0]
+    remaining_evecs = list(evecs[1:])
+    remaining_drs_indices = list(range(1, self.hilbertspace.dimension))
+
+    branch_drs_indices, _ = _single_branch_analysis(
+        self, mode_priority, 
+        0, 
+        0, init_state,
+        remaining_drs_indices, remaining_evecs
+    )
+    branch_drs_indices = np.array(branch_drs_indices)
+
+    if not transpose:
+        reversed_permutation = np.argsort(mode_priority)
+        return np.transpose(
+            branch_drs_indices, reversed_permutation
+        )
+
+    return branch_drs_indices
+
+def branch_analysis(
+    self: SpectrumLookupMixin,   # hilbertspace
+    mode_priority: Optional[List[int]] = None,
+    transpose: bool = False,
+) -> NamedSlotsNdarray:
+    """
+    """
+    dressed_indices = np.empty(shape=self._parameters.counts, dtype=object)
+
+    param_indices = itertools.product(*map(range, self._parameters.counts))
+    for index in param_indices:
+        dressed_indices[index] = generate_branch_analysis(
+            self, index, mode_priority, transpose,
+        )
+    dressed_indices = np.asarray(dressed_indices[:].tolist())
+
+    parameter_dict = self._parameters.ordered_dict.copy()
+    return NamedSlotsNdarray(dressed_indices, parameter_dict)
+
```

### Comparing `chencrafts-1.4/chencrafts/cqed/pulses.py` & `chencrafts-1.5/chencrafts/cqed/pulses.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/cqed/qt_helper.py` & `chencrafts-1.5/chencrafts/cqed/qt_helper.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/cqed/scq_helper.py` & `chencrafts-1.5/chencrafts/cqed/scq_helper.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/cqed/spec_poly_fit.py` & `chencrafts-1.5/chencrafts/cqed/spec_poly_fit.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/cqed/special_states.py` & `chencrafts-1.5/chencrafts/cqed/special_states.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/cqed/symbolic_bosons.py` & `chencrafts-1.5/chencrafts/cqed/symbolic_bosons.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/projects/fluxonium_tunable_coupler.py` & `chencrafts-1.5/chencrafts/projects/fluxonium_tunable_coupler.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/projects/protomon_disorder.py` & `chencrafts-1.5/chencrafts/projects/protomon_disorder.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/projects/protomon_full_disorder.py` & `chencrafts-1.5/chencrafts/projects/protomon_full_disorder.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/settings.py` & `chencrafts-1.5/chencrafts/settings.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/toolbox/__init__.py` & `chencrafts-1.5/chencrafts/toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/toolbox/data_processing.py` & `chencrafts-1.5/chencrafts/toolbox/data_processing.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/toolbox/gadgets.py` & `chencrafts-1.5/chencrafts/toolbox/gadgets.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/toolbox/optimize.py` & `chencrafts-1.5/chencrafts/toolbox/optimize.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/toolbox/plot.py` & `chencrafts-1.5/chencrafts/toolbox/plot.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/toolbox/save.py` & `chencrafts-1.5/chencrafts/toolbox/save.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts/toolbox/useless.py` & `chencrafts-1.5/chencrafts/toolbox/useless.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/chencrafts.egg-info/PKG-INFO` & `chencrafts-1.5/chencrafts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chencrafts
-Version: 1.4
+Version: 1.5
 Summary: A personal toolbox for superconducting qubits and quantum mechanics.
 Author-email: Danyang Chen <DanyangChen2026@u.northwestern.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2024 and later, Danyang Chen
         All rights reserved.
```

### Comparing `chencrafts-1.4/chencrafts.egg-info/SOURCES.txt` & `chencrafts-1.5/chencrafts.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 chencrafts.egg-info/PKG-INFO
 chencrafts.egg-info/SOURCES.txt
 chencrafts.egg-info/dependency_links.txt
 chencrafts.egg-info/requires.txt
 chencrafts.egg-info/top_level.txt
 chencrafts/bsqubits/__init__.py
 chencrafts/bsqubits/batched_custom_sweeps.py
+chencrafts/bsqubits/batched_sweeps_recipe.py
 chencrafts/bsqubits/cat_ideal.py
 chencrafts/bsqubits/cat_real.py
 chencrafts/bsqubits/derive_var.py
 chencrafts/bsqubits/error_rates.py
 chencrafts/bsqubits/pulse_utils.py
 chencrafts/bsqubits/systems.py
 chencrafts/bsqubits/QEC_graph/__init__.py
@@ -30,14 +31,15 @@
 chencrafts/bsqubits/QEC_graph/node.py
 chencrafts/bsqubits/QEC_graph/settings.py
 chencrafts/cqed/__init__.py
 chencrafts/cqed/block_diag.py
 chencrafts/cqed/crit_photon_num.py
 chencrafts/cqed/decoherence.py
 chencrafts/cqed/flexible_sweep.py
+chencrafts/cqed/floquet.py
 chencrafts/cqed/mode_assignment.py
 chencrafts/cqed/pulses.py
 chencrafts/cqed/qt_helper.py
 chencrafts/cqed/scq_helper.py
 chencrafts/cqed/spec_poly_fit.py
 chencrafts/cqed/special_states.py
 chencrafts/cqed/symbolic_bosons.py
```

### Comparing `chencrafts-1.4/pyproject.toml` & `chencrafts-1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chencrafts-1.4/tests/test_optimization.py` & `chencrafts-1.5/tests/test_optimization.py`

 * *Files identical despite different names*

