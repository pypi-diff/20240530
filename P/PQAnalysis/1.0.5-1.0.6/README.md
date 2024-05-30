# Comparing `tmp/pqanalysis-1.0.5.tar.gz` & `tmp/pqanalysis-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqanalysis-1.0.5.tar", last modified: Sun May 26 21:50:39 2024, max compression
+gzip compressed data, was "pqanalysis-1.0.6.tar", last modified: Thu May 30 19:25:07 2024, max compression
```

## Comparing `pqanalysis-1.0.5.tar` & `pqanalysis-1.0.6.tar`

### file list

```diff
@@ -1,457 +1,459 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:39.003466 pqanalysis-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/.docstr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.911464 pqanalysis-1.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.923465 pqanalysis-1.0.5/.github/.pylint_cache/
--rw-r--r--   0 runner    (1001) docker     (127)    16870 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/.github/.pylint_cache/PQAnalysis_1.stats
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.923465 pqanalysis-1.0.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.923465 pqanalysis-1.0.5/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/.github/scripts/parse_pylint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.923465 pqanalysis-1.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22319 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/.style.yapf
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-26 21:50:39.003466 pqanalysis-1.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.923465 pqanalysis-1.0.5/PQAnalysis/
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-26 21:50:38.000000 pqanalysis-1.0.5/PQAnalysis/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.927465 pqanalysis-1.0.5/PQAnalysis/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.927465 pqanalysis-1.0.5/PQAnalysis/analysis/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/analysis/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/analysis/rdf/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/analysis/rdf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/analysis/rdf/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/analysis/rdf/rdf_input_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/analysis/rdf/rdf_output_file_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.927465 pqanalysis-1.0.5/PQAnalysis/atomic_system/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/atomic_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/atomic_system/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/atomic_system/_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/atomic_system/_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/atomic_system/_standard_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    23524 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/atomic_system/atomic_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/atomic_system/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.931465 pqanalysis-1.0.5/PQAnalysis/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/cli/_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/cli/_cli_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/cli/add_molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/cli/build_nep_traj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/cli/continue_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/cli/gen2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/cli/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/cli/rst2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/cli/traj2box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/cli/traj2qmcfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/cli/xyz2gen.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.931465 pqanalysis-1.0.5/PQAnalysis/core/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.931465 pqanalysis-1.0.5/PQAnalysis/core/atom/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/core/atom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/core/atom/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/core/atom/element.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.931465 pqanalysis-1.0.5/PQAnalysis/core/cell/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/core/cell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/core/cell/_standard_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/core/cell/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/core/residue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.931465 pqanalysis-1.0.5/PQAnalysis/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/grammar/PQ_inputGrammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/grammar/inputGrammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/grammar/rules.lark
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/grammar/selection.lark
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/grammar/terminals.lark
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.935465 pqanalysis-1.0.5/PQAnalysis/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/box_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/conversion_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/energy_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.935465 pqanalysis-1.0.5/PQAnalysis/io/gen_file/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/gen_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/gen_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/gen_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/gen_file/gen_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/gen_file/gen_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/info_file_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.935465 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/input_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.935465 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq/output_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.939465 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/moldescriptor_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.939465 pqanalysis-1.0.5/PQAnalysis/io/nep/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/nep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/nep/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    37872 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/nep/nep_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.939465 pqanalysis-1.0.5/PQAnalysis/io/restart_file/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/restart_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/restart_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/restart_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/restart_file/restart_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/restart_file/restart_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.939465 pqanalysis-1.0.5/PQAnalysis/io/topology_file/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/topology_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/topology_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/topology_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13349 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/topology_file/topology_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/topology_file/topology_file_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.943465 pqanalysis-1.0.5/PQAnalysis/io/traj_file/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/traj_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/traj_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/traj_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/traj_file/frame_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/traj_file/trajectory_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/traj_file/trajectory_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.943465 pqanalysis-1.0.5/PQAnalysis/io/virial/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/virial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/virial/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/virial/virial_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/io/write_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.943465 pqanalysis-1.0.5/PQAnalysis/physical_data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/physical_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/physical_data/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/physical_data/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.943465 pqanalysis-1.0.5/PQAnalysis/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/tools/add_molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/tools/traj_to_com_traj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.943465 pqanalysis-1.0.5/PQAnalysis/topology/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/topology/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.947465 pqanalysis-1.0.5/PQAnalysis/topology/bonded_topology/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/topology/bonded_topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/topology/bonded_topology/_topology_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/topology/bonded_topology/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/topology/bonded_topology/bond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/topology/bonded_topology/bonded_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/topology/bonded_topology/dihedral.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/topology/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23565 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/topology/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/topology/shake_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)    18809 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/topology/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.947465 pqanalysis-1.0.5/PQAnalysis/traj/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/traj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/traj/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/traj/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/traj/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    12838 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/traj/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/type_checking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.947465 pqanalysis-1.0.5/PQAnalysis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/utils/custom_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/PQAnalysis/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.999466 pqanalysis-1.0.5/PQAnalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-26 21:50:38.000000 pqanalysis-1.0.5/PQAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-05-26 21:50:38.000000 pqanalysis-1.0.5/PQAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:50:38.000000 pqanalysis-1.0.5/PQAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-26 21:50:38.000000 pqanalysis-1.0.5/PQAnalysis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-26 21:50:38.000000 pqanalysis-1.0.5/PQAnalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 21:50:38.000000 pqanalysis-1.0.5/PQAnalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.947465 pqanalysis-1.0.5/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.947465 pqanalysis-1.0.5/benchmarks/core/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/benchmarks/core/benchmark_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/benchmarks/core/benchmark_traj_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/benchmarks/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.947465 pqanalysis-1.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/autodoc.sh
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.947465 pqanalysis-1.0.5/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.915464 pqanalysis-1.0.5/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.947465 pqanalysis-1.0.5/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.951465 pqanalysis-1.0.5/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/_templates/package.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.971465 pqanalysis-1.0.5/docs/source/code/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.analysis.rdf.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.analysis.rdf.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.analysis.rdf.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.analysis.rdf.rdf_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.analysis.rdf.rdf_output_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.analysis.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.atomic_system.atomic_system.rst
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.atomic_system.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.atomic_system.rst
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.cli.add_molecules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.cli.build_nep_traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.cli.continue_input.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.cli.gen2xyz.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.cli.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.cli.rst2xyz.rst
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.cli.traj2box.rst
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.cli.traj2qmcfc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.cli.xyz2gen.rst
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.core.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.core.atom.atom.rst
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.core.atom.element.rst
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.core.atom.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.core.cell.cell.rst
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.core.cell.rst
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.core.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.core.residue.rst
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.box_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.conversion_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.energy_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.gen_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.gen_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.gen_file.gen_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.gen_file.gen_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.gen_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.info_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.input_file_reader.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.input_file_reader.pq.output_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.input_file_reader.pq.pq_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.input_file_reader.pq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.moldescriptor_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.nep.nep_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.nep.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.restart_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.restart_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.restart_file.restart_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.restart_file.restart_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.restart_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.rst
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.topology_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.topology_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.topology_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.topology_file.topology_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.traj_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.traj_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.traj_file.frame_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.traj_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.traj_file.trajectory_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.traj_file.trajectory_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.virial.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.virial.rst
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.virial.virial_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.write_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.physical_data.energy.rst
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.physical_data.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.physical_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.tools.add_molecule.rst
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.tools.traj_to_com_traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.topology.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.topology.bonded_topology.angle.rst
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.topology.bonded_topology.bond.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.topology.bonded_topology.bonded_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.topology.bonded_topology.dihedral.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.topology.bonded_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.topology.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.topology.selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.topology.shake_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.topology.topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.traj.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.traj.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.traj.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.traj.trajectory.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.type_checking.rst
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.types.rst
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.utils.common.rst
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.utils.custom_logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.utils.decorators.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.utils.files.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.utils.random.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/PQAnalysis.utils.units.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/code/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.971465 pqanalysis-1.0.5/docs/source/developerGuide/
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/developerGuide/developerGuide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.971465 pqanalysis-1.0.5/docs/source/logo/
--rw-r--r--   0 runner    (1001) docker     (127)   204575 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/logo/PQAnalysis.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.971465 pqanalysis-1.0.5/docs/source/userGuide/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/userGuide/inputFile.rst
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/docs/source/userGuide/userGuide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.915464 pqanalysis-1.0.5/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.975466 pqanalysis-1.0.5/examples/traj2box/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/examples/traj2box/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/examples/traj2box/acof_triclinic.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/examples/traj2box/acof_triclinic_2.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.975466 pqanalysis-1.0.5/examples/traj2comtraj/
--rw-r--r--   0 runner    (1001) docker     (127)  2600700 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/examples/traj2comtraj/umcm-9-md-01.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/pytest.sh
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-26 21:50:39.003466 pqanalysis-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.979466 pqanalysis-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.979466 pqanalysis-1.0.5/tests/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.979466 pqanalysis-1.0.5/tests/analysis/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/analysis/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/analysis/rdf/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/analysis/rdf/test_rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/analysis/rdf/test_rdfInputFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/analysis/rdf/test_rdfOutputFileReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.979466 pqanalysis-1.0.5/tests/atomicSystem/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/atomicSystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24372 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/atomicSystem/test_atomic_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/atomicSystem/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/atomicSystem/test_positions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.983466 pqanalysis-1.0.5/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/cli/test_continue_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/cli/test_rst2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/cli/test_traj2box.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/cli/test_traj2qmcfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.983466 pqanalysis-1.0.5/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.983466 pqanalysis-1.0.5/tests/core/atom/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/core/atom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/core/atom/test_atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/core/atom/test_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/core/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/core/test_residue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.919464 pqanalysis-1.0.5/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.983466 pqanalysis-1.0.5/tests/data/inputFileReader/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.987466 pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/n_not_matching.in
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/no_output_files.in
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/no_start_file.in
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/run-08.in
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/run-08.rpmd.in
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/run-09.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/run-10.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/inputFileReader/input.in
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/inputFileReader/input_PQ.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.987466 pqanalysis-1.0.5/tests/data/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/rdf/input.in
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/rdf/required_keys_not_given.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.987466 pqanalysis-1.0.5/tests/data/readEnergyFile/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/readEnergyFile/md-01.en
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/readEnergyFile/md-01.info
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/readEnergyFile/md-01_noinfo.en
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.987466 pqanalysis-1.0.5/tests/data/readInfoFile/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/readInfoFile/md-01.info
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/readInfoFile/md-01.qmcfc.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.987466 pqanalysis-1.0.5/tests/data/readMoldescriptor/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/readMoldescriptor/moldescriptor.dat
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/readMoldescriptor/moldescriptor_withError.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.987466 pqanalysis-1.0.5/tests/data/readRestartFile/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/readRestartFile/md-01.rst
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/readRestartFile/moldescriptor.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.987466 pqanalysis-1.0.5/tests/data/rst2xyz/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/rst2xyz/md-01.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.987466 pqanalysis-1.0.5/tests/data/traj2box/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/traj2box/box.dat
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/traj2box/box.vmd.xyz
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/traj2box/test.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.991466 pqanalysis-1.0.5/tests/data/traj2qmcfc/
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/traj2qmcfc/acof_triclinic.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/traj2qmcfc/acof_triclinic_2.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  2301740 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/data/traj2qmcfc/traj.qmcfc.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.995466 pqanalysis-1.0.5/tests/io/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.995466 pqanalysis-1.0.5/tests/io/inputFileReader/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.995466 pqanalysis-1.0.5/tests/io/inputFileReader/PQ/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/inputFileReader/PQ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.999466 pqanalysis-1.0.5/tests/io/inputFileReader/PQAnalysis/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/inputFileReader/PQAnalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/inputFileReader/PQAnalysis/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/inputFileReader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/inputFileReader/test_inputDictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/inputFileReader/test_inputFileParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/inputFileReader/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/inputFileReader/test_visitors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/test_boxWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/test_energyFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/test_frameReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/test_infoFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/test_moldescriptorReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/test_restartReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/test_restartWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    23202 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/test_trajectoryReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/test_trajectoryWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/io/test_write_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.999466 pqanalysis-1.0.5/tests/physicalData/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/physicalData/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/physicalData/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/test_formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.999466 pqanalysis-1.0.5/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/tools/test_traj_to_com_traj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.999466 pqanalysis-1.0.5/tests/topology/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/topology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.999466 pqanalysis-1.0.5/tests/topology/bonded_topology/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/topology/bonded_topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/topology/bonded_topology/test_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/topology/bonded_topology/test_bond.py
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/topology/bonded_topology/test_bondedTopology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/topology/bonded_topology/test_dihedral.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/topology/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/topology/test_selectionTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/topology/test_shakeTopology.py
--rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/topology/test_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.999466 pqanalysis-1.0.5/tests/traj/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/traj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/traj/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/traj/test_trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:50:38.999466 pqanalysis-1.0.5/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/utils/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-26 21:50:23.000000 pqanalysis-1.0.5/tests/utils/test_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.199953 pqanalysis-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/.docstr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.111953 pqanalysis-1.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.123953 pqanalysis-1.0.6/.github/.pylint_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)    16993 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/.github/.pylint_cache/PQAnalysis_1.stats
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.123953 pqanalysis-1.0.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.123953 pqanalysis-1.0.6/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/.github/scripts/parse_pylint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.123953 pqanalysis-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22319 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-30 19:25:07.199953 pqanalysis-1.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.123953 pqanalysis-1.0.6/PQAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 19:25:06.000000 pqanalysis-1.0.6/PQAnalysis/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.123953 pqanalysis-1.0.6/PQAnalysis/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.127953 pqanalysis-1.0.6/PQAnalysis/analysis/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/analysis/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/analysis/rdf/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/analysis/rdf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/analysis/rdf/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/analysis/rdf/rdf_input_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/analysis/rdf/rdf_output_file_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.127953 pqanalysis-1.0.6/PQAnalysis/atomic_system/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/atomic_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/atomic_system/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/atomic_system/_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/atomic_system/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/atomic_system/_standard_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/atomic_system/atomic_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/atomic_system/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.127953 pqanalysis-1.0.6/PQAnalysis/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/cli/_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/cli/_cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/cli/add_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/cli/build_nep_traj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/cli/continue_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/cli/gen2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/cli/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/cli/rst2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/cli/traj2box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/cli/traj2qmcfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/cli/xyz2gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.131953 pqanalysis-1.0.6/PQAnalysis/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.131953 pqanalysis-1.0.6/PQAnalysis/core/atom/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/core/atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/core/atom/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/core/atom/element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.131953 pqanalysis-1.0.6/PQAnalysis/core/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/core/cell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/core/cell/_standard_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/core/cell/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/core/residue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.131953 pqanalysis-1.0.6/PQAnalysis/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/grammar/PQ_inputGrammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/grammar/inputGrammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/grammar/rules.lark
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/grammar/selection.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/grammar/terminals.lark
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.135953 pqanalysis-1.0.6/PQAnalysis/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/box_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/conversion_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/energy_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.135953 pqanalysis-1.0.6/PQAnalysis/io/gen_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/gen_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/gen_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/gen_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/gen_file/gen_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/gen_file/gen_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/info_file_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.135953 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/input_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.135953 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq/output_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.135953 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/moldescriptor_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.135953 pqanalysis-1.0.6/PQAnalysis/io/nep/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/nep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/nep/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37872 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/nep/nep_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.139953 pqanalysis-1.0.6/PQAnalysis/io/restart_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/restart_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/restart_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/restart_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/restart_file/restart_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/restart_file/restart_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.139953 pqanalysis-1.0.6/PQAnalysis/io/topology_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/topology_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/topology_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/topology_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13349 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/topology_file/topology_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/topology_file/topology_file_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.139953 pqanalysis-1.0.6/PQAnalysis/io/traj_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/traj_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/traj_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/traj_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/traj_file/frame_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/traj_file/trajectory_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/traj_file/trajectory_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.139953 pqanalysis-1.0.6/PQAnalysis/io/virial/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/virial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/virial/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/virial/virial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/io/write_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.139953 pqanalysis-1.0.6/PQAnalysis/physical_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/physical_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/physical_data/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/physical_data/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.143953 pqanalysis-1.0.6/PQAnalysis/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/tools/add_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/tools/traj_to_com_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.143953 pqanalysis-1.0.6/PQAnalysis/topology/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/topology/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.143953 pqanalysis-1.0.6/PQAnalysis/topology/bonded_topology/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/topology/bonded_topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/topology/bonded_topology/_topology_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/topology/bonded_topology/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/topology/bonded_topology/bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/topology/bonded_topology/bonded_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/topology/bonded_topology/dihedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/topology/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23565 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/topology/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/topology/shake_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18809 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/topology/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.143953 pqanalysis-1.0.6/PQAnalysis/traj/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/traj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/traj/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/traj/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/traj/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/traj/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/type_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.147953 pqanalysis-1.0.6/PQAnalysis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/utils/custom_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/PQAnalysis/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.195953 pqanalysis-1.0.6/PQAnalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-30 19:25:07.000000 pqanalysis-1.0.6/PQAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15124 2024-05-30 19:25:07.000000 pqanalysis-1.0.6/PQAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:25:07.000000 pqanalysis-1.0.6/PQAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-30 19:25:07.000000 pqanalysis-1.0.6/PQAnalysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-30 19:25:07.000000 pqanalysis-1.0.6/PQAnalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 19:25:07.000000 pqanalysis-1.0.6/PQAnalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.147953 pqanalysis-1.0.6/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.147953 pqanalysis-1.0.6/benchmarks/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/benchmarks/core/benchmark_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/benchmarks/core/benchmark_traj_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/benchmarks/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.147953 pqanalysis-1.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/autodoc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.147953 pqanalysis-1.0.6/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.115953 pqanalysis-1.0.6/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.147953 pqanalysis-1.0.6/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.147953 pqanalysis-1.0.6/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/_templates/package.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.167953 pqanalysis-1.0.6/docs/source/code/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.analysis.rdf.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.analysis.rdf.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.analysis.rdf.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.analysis.rdf.rdf_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.analysis.rdf.rdf_output_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.analysis.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.atomic_system.atomic_system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.atomic_system.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.atomic_system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.cli.add_molecules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.cli.build_nep_traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.cli.continue_input.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.cli.gen2xyz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.cli.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.cli.rst2xyz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.cli.traj2box.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.cli.traj2qmcfc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.cli.xyz2gen.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.core.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.core.atom.atom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.core.atom.element.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.core.atom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.core.cell.cell.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.core.cell.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.core.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.core.residue.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.box_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.conversion_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.energy_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.gen_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.gen_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.gen_file.gen_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.gen_file.gen_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.gen_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.info_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.input_file_reader.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.input_file_reader.pq.output_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.input_file_reader.pq.pq_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.input_file_reader.pq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.moldescriptor_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.nep.nep_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.nep.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.restart_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.restart_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.restart_file.restart_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.restart_file.restart_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.restart_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.topology_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.topology_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.topology_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.topology_file.topology_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.traj_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.traj_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.traj_file.frame_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.traj_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.traj_file.trajectory_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.traj_file.trajectory_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.virial.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.virial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.virial.virial_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.write_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.physical_data.energy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.physical_data.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.physical_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.tools.add_molecule.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.tools.traj_to_com_traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.topology.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.topology.bonded_topology.angle.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.topology.bonded_topology.bond.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.topology.bonded_topology.bonded_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.topology.bonded_topology.dihedral.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.topology.bonded_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.topology.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.topology.selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.topology.shake_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.topology.topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.traj.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.traj.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.traj.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.traj.trajectory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.type_checking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.utils.common.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.utils.custom_logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.utils.decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.utils.files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.utils.random.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/PQAnalysis.utils.units.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/code/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.167953 pqanalysis-1.0.6/docs/source/developerGuide/
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/developerGuide/developerGuide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.167953 pqanalysis-1.0.6/docs/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   204575 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/logo/PQAnalysis.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.167953 pqanalysis-1.0.6/docs/source/userGuide/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/userGuide/inputFile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/docs/source/userGuide/userGuide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.115953 pqanalysis-1.0.6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.171953 pqanalysis-1.0.6/examples/traj2box/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/examples/traj2box/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/examples/traj2box/acof_triclinic.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/examples/traj2box/acof_triclinic_2.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.171953 pqanalysis-1.0.6/examples/traj2comtraj/
+-rw-r--r--   0 runner    (1001) docker     (127)  2600700 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/examples/traj2comtraj/umcm-9-md-01.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-30 19:25:07.199953 pqanalysis-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.175953 pqanalysis-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.175953 pqanalysis-1.0.6/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.175953 pqanalysis-1.0.6/tests/analysis/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/analysis/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/analysis/rdf/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/analysis/rdf/test_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/analysis/rdf/test_rdfInputFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/analysis/rdf/test_rdfOutputFileReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.175953 pqanalysis-1.0.6/tests/atomicSystem/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/atomicSystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25879 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/atomicSystem/test_atomic_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/atomicSystem/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/atomicSystem/test_positions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.175953 pqanalysis-1.0.6/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/cli/test_continue_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/cli/test_rst2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/cli/test_traj2box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/cli/test_traj2qmcfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.179953 pqanalysis-1.0.6/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.179953 pqanalysis-1.0.6/tests/core/atom/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/core/atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/core/atom/test_atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/core/atom/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/core/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/core/test_residue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.119953 pqanalysis-1.0.6/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.179953 pqanalysis-1.0.6/tests/data/inputFileReader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.179953 pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/n_not_matching.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/no_output_files.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/no_start_file.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/run-08.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/run-08.rpmd.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/run-09.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/run-10.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/inputFileReader/input.in
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/inputFileReader/input_PQ.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.179953 pqanalysis-1.0.6/tests/data/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/rdf/input.in
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/rdf/required_keys_not_given.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.179953 pqanalysis-1.0.6/tests/data/readEnergyFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/readEnergyFile/md-01.en
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/readEnergyFile/md-01.info
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/readEnergyFile/md-01_noinfo.en
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.183953 pqanalysis-1.0.6/tests/data/readInfoFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/readInfoFile/md-01.info
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/readInfoFile/md-01.qmcfc.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.183953 pqanalysis-1.0.6/tests/data/readMoldescriptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/readMoldescriptor/moldescriptor.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/readMoldescriptor/moldescriptor_withError.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.183953 pqanalysis-1.0.6/tests/data/readRestartFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/readRestartFile/md-01.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/readRestartFile/moldescriptor.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.183953 pqanalysis-1.0.6/tests/data/rst2xyz/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/rst2xyz/md-01.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.183953 pqanalysis-1.0.6/tests/data/traj2box/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/traj2box/box.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/traj2box/box.vmd.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/traj2box/test.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.187953 pqanalysis-1.0.6/tests/data/traj2qmcfc/
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/traj2qmcfc/acof_triclinic.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/traj2qmcfc/acof_triclinic_2.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  2301740 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/data/traj2qmcfc/traj.qmcfc.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.191954 pqanalysis-1.0.6/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.191954 pqanalysis-1.0.6/tests/io/inputFileReader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.191954 pqanalysis-1.0.6/tests/io/inputFileReader/PQ/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/inputFileReader/PQ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.191954 pqanalysis-1.0.6/tests/io/inputFileReader/PQAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/inputFileReader/PQAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/inputFileReader/PQAnalysis/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/inputFileReader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/inputFileReader/test_inputDictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/inputFileReader/test_inputFileParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/inputFileReader/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/inputFileReader/test_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/test_boxWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/test_energyFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/test_frameReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/test_infoFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/test_moldescriptorReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/test_restartReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/test_restartWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23202 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/test_trajectoryReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/test_trajectoryWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/io/test_write_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.191954 pqanalysis-1.0.6/tests/physicalData/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/physicalData/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/physicalData/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/test_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.191954 pqanalysis-1.0.6/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/tools/test_traj_to_com_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.195953 pqanalysis-1.0.6/tests/topology/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/topology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.195953 pqanalysis-1.0.6/tests/topology/bonded_topology/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/topology/bonded_topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/topology/bonded_topology/test_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/topology/bonded_topology/test_bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/topology/bonded_topology/test_bondedTopology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/topology/bonded_topology/test_dihedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/topology/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/topology/test_selectionTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/topology/test_shakeTopology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/topology/test_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.195953 pqanalysis-1.0.6/tests/traj/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/traj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/traj/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/traj/test_trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:25:07.195953 pqanalysis-1.0.6/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/utils/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/utils/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-30 19:24:54.000000 pqanalysis-1.0.6/tests/utils/test_math.py
```

### Comparing `pqanalysis-1.0.5/.codecov.yml` & `pqanalysis-1.0.6/.codecov.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/.github/.pylint_cache/PQAnalysis_1.stats` & `pqanalysis-1.0.6/.github/.pylint_cache/PQAnalysis_1.stats`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 95db 4100 0000 0000 008c 1870 796c  ....A........pyl
+00000000: 8004 9556 4200 0000 0000 008c 1870 796c  ...VB........pyl
 00000010: 696e 742e 7574 696c 732e 6c69 6e74 6572  int.utils.linter
 00000020: 7374 6174 7394 8c0b 4c69 6e74 6572 5374  stats...LinterSt
 00000030: 6174 7394 9394 2981 947d 9428 8c09 6261  ats...)..}.(..ba
 00000040: 645f 6e61 6d65 7394 7d94 288c 0861 7267  d_names.}.(..arg
 00000050: 756d 656e 7494 4b00 8c04 6174 7472 944b  ument.K...attr.K
 00000060: 008c 056b 6c61 7373 944b 008c 0f63 6c61  ...klass.K...cla
 00000070: 7373 5f61 7474 7269 6275 7465 944b 008c  ss_attribute.K..
@@ -10,1046 +10,1054 @@
 00000090: 0563 6f6e 7374 944b 0c8c 0969 6e6c 696e  .const.K...inlin
 000000a0: 6576 6172 944b 008c 0866 756e 6374 696f  evar.K...functio
 000000b0: 6e94 4b00 8c06 6d65 7468 6f64 944b 028c  n.K...method.K..
 000000c0: 066d 6f64 756c 6594 4b01 8c08 7661 7269  .module.K...vari
 000000d0: 6162 6c65 944b 008c 0774 7970 6576 6172  able.K...typevar
 000000e0: 944b 008c 0974 7970 6561 6c69 6173 944b  .K...typealias.K
 000000f0: 0075 8c09 6279 5f6d 6f64 756c 6594 7d94  .u..by_module.}.
-00000100: 288c 312f 686f 6d65 2f72 756e 6e65 722f  (.1/home/runner/
-00000110: 776f 726b 2f50 5141 6e61 6c79 7369 732f  work/PQAnalysis/
-00000120: 5051 416e 616c 7973 6973 2f2e 7079 6c69  PQAnalysis/.pyli
-00000130: 6e74 7263 947d 9428 8c0a 636f 6e76 656e  ntrc.}.(..conven
-00000140: 7469 6f6e 944b 008c 0565 7272 6f72 944b  tion.K...error.K
-00000150: 008c 0566 6174 616c 944b 008c 0469 6e66  ...fatal.K...inf
-00000160: 6f94 4b00 8c08 7265 6661 6374 6f72 944b  o.K...refactor.K
-00000170: 008c 0973 7461 7465 6d65 6e74 944b 008c  ...statement.K..
-00000180: 0777 6172 6e69 6e67 944b 0075 8c0c 436f  .warning.K.u..Co
-00000190: 6d6d 616e 6420 6c69 6e65 947d 9428 6818  mmand line.}.(h.
-000001a0: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
-000001b0: 4b00 681d 4b00 681e 4b00 758c 2243 6f6d  K.h.K.h.K.u."Com
-000001c0: 6d61 6e64 206c 696e 6520 6f72 2063 6f6e  mand line or con
-000001d0: 6669 6775 7261 7469 6f6e 2066 696c 6594  figuration file.
-000001e0: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-000001f0: 1b4b 0068 1c4b 0068 1d4b 0068 1e4b 0075  .K.h.K.h.K.h.K.u
-00000200: 8c0a 5051 416e 616c 7973 6973 947d 9428  ..PQAnalysis.}.(
-00000210: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-00000220: 681c 4b00 681d 4b1c 681e 4b01 758c 1850  h.K.h.K.h.K.u..P
-00000230: 5141 6e61 6c79 7369 732e 7479 7065 5f63  QAnalysis.type_c
-00000240: 6865 636b 696e 6794 7d94 2868 184b 0068  hecking.}.(h.K.h
-00000250: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
-00000260: 1d4b 3768 1e4b 0075 8c11 5051 416e 616c  .K7h.K.u..PQAnal
-00000270: 7973 6973 2e63 6f6e 6669 6794 7d94 2868  ysis.config.}.(h
-00000280: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-00000290: 1c4b 0068 1d4b 0668 1e4b 0075 8c10 5051  .K.h.K.h.K.u..PQ
-000002a0: 416e 616c 7973 6973 2e74 7970 6573 947d  Analysis.types.}
-000002b0: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-000002c0: 4b00 681c 4b00 681d 4b0e 681e 4b00 758c  K.h.K.h.K.h.K.u.
-000002d0: 1550 5141 6e61 6c79 7369 732e 6578 6365  .PQAnalysis.exce
-000002e0: 7074 696f 6e73 947d 9428 6818 4b00 6819  ptions.}.(h.K.h.
-000002f0: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
-00000300: 4b11 681e 4b00 758c 1250 5141 6e61 6c79  K.h.K.u..PQAnaly
-00000310: 7369 732e 666f 726d 6174 7394 7d94 2868  sis.formats.}.(h
-00000320: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-00000330: 1c4b 0068 1d4b 1468 1e4b 0075 8c17 5051  .K.h.K.h.K.u..PQ
-00000340: 416e 616c 7973 6973 2e74 6f70 6f6c 6f67  Analysis.topolog
-00000350: 792e 6170 6994 7d94 2868 184b 0068 194b  y.api.}.(h.K.h.K
-00000360: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
-00000370: 1168 1e4b 0075 8c1c 5051 416e 616c 7973  .h.K.u..PQAnalys
-00000380: 6973 2e74 6f70 6f6c 6f67 792e 746f 706f  is.topology.topo
-00000390: 6c6f 6779 947d 9428 6818 4b00 6819 4b00  logy.}.(h.K.h.K.
-000003a0: 681a 4b00 681b 4b00 681c 4b02 681d 4b9f  h.K.h.K.h.K.h.K.
-000003b0: 681e 4b00 758c 1d50 5141 6e61 6c79 7369  h.K.u..PQAnalysi
-000003c0: 732e 746f 706f 6c6f 6779 2e73 656c 6563  s.topology.selec
-000003d0: 7469 6f6e 947d 9428 6818 4b00 6819 4b00  tion.}.(h.K.h.K.
-000003e0: 681a 4b00 681b 4b00 681c 4b01 681d 4b92  h.K.h.K.h.K.h.K.
-000003f0: 681e 4b00 758c 1c50 5141 6e61 6c79 7369  h.K.u..PQAnalysi
-00000400: 732e 746f 706f 6c6f 6779 2e5f 5f69 6e69  s.topology.__ini
-00000410: 745f 5f94 7d94 2868 184b 0068 194b 0068  t__.}.(h.K.h.K.h
-00000420: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0768  .K.h.K.h.K.h.K.h
-00000430: 1e4b 0275 8c22 5051 416e 616c 7973 6973  .K.u."PQAnalysis
-00000440: 2e74 6f70 6f6c 6f67 792e 7368 616b 655f  .topology.shake_
-00000450: 746f 706f 6c6f 6779 947d 9428 6818 4b00  topology.}.(h.K.
-00000460: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
-00000470: 681d 4b2f 681e 4b00 758c 1e50 5141 6e61  h.K/h.K.u..PQAna
-00000480: 6c79 7369 732e 746f 706f 6c6f 6779 2e65  lysis.topology.e
-00000490: 7863 6570 7469 6f6e 7394 7d94 2868 184b  xceptions.}.(h.K
-000004a0: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-000004b0: 0068 1d4b 0568 1e4b 0075 8c33 5051 416e  .h.K.h.K.u.3PQAn
-000004c0: 616c 7973 6973 2e74 6f70 6f6c 6f67 792e  alysis.topology.
-000004d0: 626f 6e64 6564 5f74 6f70 6f6c 6f67 792e  bonded_topology.
-000004e0: 626f 6e64 6564 5f74 6f70 6f6c 6f67 7994  bonded_topology.
-000004f0: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00000500: 1b4b 0068 1c4b 0168 1d4b 2468 1e4b 0075  .K.h.K.h.K$h.K.u
-00000510: 8c38 5051 416e 616c 7973 6973 2e74 6f70  .8PQAnalysis.top
-00000520: 6f6c 6f67 792e 626f 6e64 6564 5f74 6f70  ology.bonded_top
-00000530: 6f6c 6f67 792e 5f74 6f70 6f6c 6f67 795f  ology._topology_
-00000540: 7072 6f70 6572 7469 6573 947d 9428 6818  properties.}.(h.
-00000550: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
-00000560: 4b00 681d 4b2e 681e 4b00 758c 2c50 5141  K.h.K.h.K.u.,PQA
-00000570: 6e61 6c79 7369 732e 746f 706f 6c6f 6779  nalysis.topology
-00000580: 2e62 6f6e 6465 645f 746f 706f 6c6f 6779  .bonded_topology
-00000590: 2e5f 5f69 6e69 745f 5f94 7d94 2868 184b  .__init__.}.(h.K
-000005a0: 0168 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-000005b0: 0068 1d4b 0068 1e4b 0075 8c29 5051 416e  .h.K.h.K.u.)PQAn
-000005c0: 616c 7973 6973 2e74 6f70 6f6c 6f67 792e  alysis.topology.
-000005d0: 626f 6e64 6564 5f74 6f70 6f6c 6f67 792e  bonded_topology.
-000005e0: 616e 676c 6594 7d94 2868 184b 0068 194b  angle.}.(h.K.h.K
-000005f0: 0068 1a4b 0068 1b4b 0068 1c4b 0168 1d4b  .h.K.h.K.h.K.h.K
-00000600: 1068 1e4b 0075 8c2c 5051 416e 616c 7973  .h.K.u.,PQAnalys
-00000610: 6973 2e74 6f70 6f6c 6f67 792e 626f 6e64  is.topology.bond
-00000620: 6564 5f74 6f70 6f6c 6f67 792e 6469 6865  ed_topology.dihe
-00000630: 6472 616c 947d 9428 6818 4b00 6819 4b00  dral.}.(h.K.h.K.
-00000640: 681a 4b00 681b 4b00 681c 4b02 681d 4b12  h.K.h.K.h.K.h.K.
-00000650: 681e 4b00 758c 2850 5141 6e61 6c79 7369  h.K.u.(PQAnalysi
-00000660: 732e 746f 706f 6c6f 6779 2e62 6f6e 6465  s.topology.bonde
-00000670: 645f 746f 706f 6c6f 6779 2e62 6f6e 6494  d_topology.bond.
-00000680: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00000690: 1b4b 0068 1c4b 0168 1d4b 1068 1e4b 0075  .K.h.K.h.K.h.K.u
-000006a0: 8c1d 5051 416e 616c 7973 6973 2e74 6f6f  ..PQAnalysis.too
-000006b0: 6c73 2e61 6464 5f6d 6f6c 6563 756c 6594  ls.add_molecule.
-000006c0: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-000006d0: 1b4b 0068 1c4b 0468 1d4b 5268 1e4b 0075  .K.h.K.h.KRh.K.u
-000006e0: 8c19 5051 416e 616c 7973 6973 2e74 6f6f  ..PQAnalysis.too
-000006f0: 6c73 2e5f 5f69 6e69 745f 5f94 7d94 2868  ls.__init__.}.(h
-00000700: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-00000710: 1c4b 0068 1d4b 0168 1e4b 0075 8c21 5051  .K.h.K.h.K.u.!PQ
-00000720: 416e 616c 7973 6973 2e74 6f6f 6c73 2e74  Analysis.tools.t
-00000730: 7261 6a5f 746f 5f63 6f6d 5f74 7261 6a94  raj_to_com_traj.
-00000740: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00000750: 1b4b 0068 1c4b 0068 1d4b 0c68 1e4b 0275  .K.h.K.h.K.h.K.u
-00000760: 8c2d 5051 416e 616c 7973 6973 2e61 746f  .-PQAnalysis.ato
-00000770: 6d69 635f 7379 7374 656d 2e5f 7374 616e  mic_system._stan
-00000780: 6461 7264 5f70 726f 7065 7274 6965 7394  dard_properties.
+00000100: 288c 272f 686f 6d65 2f6a 6167 2f70 726f  (.'/home/jag/pro
+00000110: 6a65 6374 732f 7071 616e 616c 7973 6973  jects/pqanalysis
+00000120: 2f2e 7079 6c69 6e74 7263 947d 9428 8c0a  /.pylintrc.}.(..
+00000130: 636f 6e76 656e 7469 6f6e 944b 008c 0565  convention.K...e
+00000140: 7272 6f72 944b 008c 0566 6174 616c 944b  rror.K...fatal.K
+00000150: 008c 0469 6e66 6f94 4b00 8c08 7265 6661  ...info.K...refa
+00000160: 6374 6f72 944b 008c 0973 7461 7465 6d65  ctor.K...stateme
+00000170: 6e74 944b 008c 0777 6172 6e69 6e67 944b  nt.K...warning.K
+00000180: 0075 8c0c 436f 6d6d 616e 6420 6c69 6e65  .u..Command line
+00000190: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+000001a0: 681b 4b00 681c 4b00 681d 4b00 681e 4b00  h.K.h.K.h.K.h.K.
+000001b0: 758c 2243 6f6d 6d61 6e64 206c 696e 6520  u."Command line 
+000001c0: 6f72 2063 6f6e 6669 6775 7261 7469 6f6e  or configuration
+000001d0: 2066 696c 6594 7d94 2868 184b 0068 194b   file.}.(h.K.h.K
+000001e0: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
+000001f0: 0068 1e4b 0075 8c0a 5051 416e 616c 7973  .h.K.u..PQAnalys
+00000200: 6973 947d 9428 6818 4b00 6819 4b01 681a  is.}.(h.K.h.K.h.
+00000210: 4b00 681b 4b00 681c 4b00 681d 4b1c 681e  K.h.K.h.K.h.K.h.
+00000220: 4b01 758c 1550 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
+00000230: 6578 6365 7074 696f 6e73 947d 9428 6818  exceptions.}.(h.
+00000240: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
+00000250: 4b00 681d 4b11 681e 4b00 758c 1150 5141  K.h.K.h.K.u..PQA
+00000260: 6e61 6c79 7369 732e 636f 6e66 6967 947d  nalysis.config.}
+00000270: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+00000280: 4b00 681c 4b00 681d 4b06 681e 4b00 758c  K.h.K.h.K.h.K.u.
+00000290: 1250 5141 6e61 6c79 7369 732e 666f 726d  .PQAnalysis.form
+000002a0: 6174 7394 7d94 2868 184b 0068 194b 0068  ats.}.(h.K.h.K.h
+000002b0: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 1468  .K.h.K.h.K.h.K.h
+000002c0: 1e4b 0075 8c10 5051 416e 616c 7973 6973  .K.u..PQAnalysis
+000002d0: 2e74 7970 6573 947d 9428 6818 4b00 6819  .types.}.(h.K.h.
+000002e0: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
+000002f0: 4b0f 681e 4b00 758c 1850 5141 6e61 6c79  K.h.K.u..PQAnaly
+00000300: 7369 732e 7479 7065 5f63 6865 636b 696e  sis.type_checkin
+00000310: 6794 7d94 2868 184b 0068 194b 0068 1a4b  g.}.(h.K.h.K.h.K
+00000320: 0068 1b4b 0068 1c4b 0068 1d4b 3768 1e4b  .h.K.h.K.h.K7h.K
+00000330: 0075 8c16 5051 416e 616c 7973 6973 2e75  .u..PQAnalysis.u
+00000340: 7469 6c73 2e66 696c 6573 947d 9428 6818  tils.files.}.(h.
+00000350: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
+00000360: 4b00 681d 4b0a 681e 4b00 758c 1650 5141  K.h.K.h.K.u..PQA
+00000370: 6e61 6c79 7369 732e 7574 696c 732e 756e  nalysis.utils.un
+00000380: 6974 7394 7d94 2868 184b 0068 194b 0068  its.}.(h.K.h.K.h
+00000390: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0768  .K.h.K.h.K.h.K.h
+000003a0: 1e4b 0075 8c19 5051 416e 616c 7973 6973  .K.u..PQAnalysis
+000003b0: 2e75 7469 6c73 2e5f 5f69 6e69 745f 5f94  .utils.__init__.
+000003c0: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+000003d0: 1b4b 0068 1c4b 0068 1d4b 0268 1e4b 0075  .K.h.K.h.K.h.K.u
+000003e0: 8c17 5051 416e 616c 7973 6973 2e75 7469  ..PQAnalysis.uti
+000003f0: 6c73 2e63 6f6d 6d6f 6e94 7d94 2868 184b  ls.common.}.(h.K
+00000400: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
+00000410: 0068 1d4b 0968 1e4b 0075 8c1f 5051 416e  .h.K.h.K.u..PQAn
+00000420: 616c 7973 6973 2e75 7469 6c73 2e63 7573  alysis.utils.cus
+00000430: 746f 6d5f 6c6f 6767 696e 6794 7d94 2868  tom_logging.}.(h
+00000440: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+00000450: 1c4b 0068 1d4b 6568 1e4b 0075 8c15 5051  .K.h.Keh.K.u..PQ
+00000460: 416e 616c 7973 6973 2e75 7469 6c73 2e6d  Analysis.utils.m
+00000470: 6174 6894 7d94 2868 184b 0068 194b 0068  ath.}.(h.K.h.K.h
+00000480: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0768  .K.h.K.h.K.h.K.h
+00000490: 1e4b 0075 8c1b 5051 416e 616c 7973 6973  .K.u..PQAnalysis
+000004a0: 2e75 7469 6c73 2e64 6563 6f72 6174 6f72  .utils.decorator
+000004b0: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
+000004c0: 0068 1b4b 0068 1c4b 0068 1d4b 2068 1e4b  .h.K.h.K.h.K h.K
+000004d0: 0075 8c17 5051 416e 616c 7973 6973 2e75  .u..PQAnalysis.u
+000004e0: 7469 6c73 2e72 616e 646f 6d94 7d94 2868  tils.random.}.(h
+000004f0: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+00000500: 1c4b 0068 1d4b 0668 1e4b 0075 8c1c 5051  .K.h.K.h.K.u..PQ
+00000510: 416e 616c 7973 6973 2e61 6e61 6c79 7369  Analysis.analysi
+00000520: 732e 5f5f 696e 6974 5f5f 947d 9428 6818  s.__init__.}.(h.
+00000530: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
+00000540: 4b00 681d 4b01 681e 4b00 758c 2250 5141  K.h.K.h.K.u."PQA
+00000550: 6e61 6c79 7369 732e 616e 616c 7973 6973  nalysis.analysis
+00000560: 2e72 6466 2e65 7863 6570 7469 6f6e 7394  .rdf.exceptions.
+00000570: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00000580: 1b4b 0068 1c4b 0068 1d4b 0968 1e4b 0075  .K.h.K.h.K.h.K.u
+00000590: 8c2e 5051 416e 616c 7973 6973 2e61 6e61  ..PQAnalysis.ana
+000005a0: 6c79 7369 732e 7264 662e 7264 665f 6f75  lysis.rdf.rdf_ou
+000005b0: 7470 7574 5f66 696c 655f 7772 6974 6572  tput_file_writer
+000005c0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+000005d0: 681b 4b00 681c 4b00 681d 4b33 681e 4b00  h.K.h.K.h.K3h.K.
+000005e0: 758c 1b50 5141 6e61 6c79 7369 732e 616e  u..PQAnalysis.an
+000005f0: 616c 7973 6973 2e72 6466 2e72 6466 947d  alysis.rdf.rdf.}
+00000600: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+00000610: 4b00 681c 4b03 681d 4b9a 681e 4b00 758c  K.h.K.h.K.h.K.u.
+00000620: 2d50 5141 6e61 6c79 7369 732e 616e 616c  -PQAnalysis.anal
+00000630: 7973 6973 2e72 6466 2e72 6466 5f69 6e70  ysis.rdf.rdf_inp
+00000640: 7574 5f66 696c 655f 7265 6164 6572 947d  ut_file_reader.}
+00000650: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+00000660: 4b00 681c 4b00 681d 4b18 681e 4b00 758c  K.h.K.h.K.h.K.u.
+00000670: 1b50 5141 6e61 6c79 7369 732e 616e 616c  .PQAnalysis.anal
+00000680: 7973 6973 2e72 6466 2e61 7069 947d 9428  ysis.rdf.api.}.(
+00000690: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+000006a0: 681c 4b00 681d 4b1e 681e 4b00 758c 2050  h.K.h.K.h.K.u. P
+000006b0: 5141 6e61 6c79 7369 732e 616e 616c 7973  QAnalysis.analys
+000006c0: 6973 2e72 6466 2e5f 5f69 6e69 745f 5f94  is.rdf.__init__.
+000006d0: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+000006e0: 1b4b 0068 1c4b 0068 1d4b 0568 1e4b 0075  .K.h.K.h.K.h.K.u
+000006f0: 8c19 5051 416e 616c 7973 6973 2e74 6f6f  ..PQAnalysis.too
+00000700: 6c73 2e5f 5f69 6e69 745f 5f94 7d94 2868  ls.__init__.}.(h
+00000710: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+00000720: 1c4b 0068 1d4b 0168 1e4b 0075 8c21 5051  .K.h.K.h.K.u.!PQ
+00000730: 416e 616c 7973 6973 2e74 6f6f 6c73 2e74  Analysis.tools.t
+00000740: 7261 6a5f 746f 5f63 6f6d 5f74 7261 6a94  raj_to_com_traj.
+00000750: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00000760: 1b4b 0068 1c4b 0068 1d4b 0c68 1e4b 0275  .K.h.K.h.K.h.K.u
+00000770: 8c1d 5051 416e 616c 7973 6973 2e74 6f6f  ..PQAnalysis.too
+00000780: 6c73 2e61 6464 5f6d 6f6c 6563 756c 6594  ls.add_molecule.
 00000790: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-000007a0: 1b4b 0068 1c4b 0268 1d4b 4468 1e4b 0075  .K.h.K.h.KDh.K.u
-000007b0: 8c24 5051 416e 616c 7973 6973 2e61 746f  .$PQAnalysis.ato
-000007c0: 6d69 635f 7379 7374 656d 2e5f 7072 6f70  mic_system._prop
-000007d0: 6572 7469 6573 947d 9428 6818 4b00 6819  erties.}.(h.K.h.
-000007e0: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
-000007f0: 4b26 681e 4b00 758c 2350 5141 6e61 6c79  K&h.K.u.#PQAnaly
-00000800: 7369 732e 6174 6f6d 6963 5f73 7973 7465  sis.atomic_syste
-00000810: 6d2e 5f70 6f73 6974 696f 6e73 947d 9428  m._positions.}.(
-00000820: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-00000830: 681c 4b00 681d 4b19 681e 4b00 758c 2650  h.K.h.K.h.K.u.&P
-00000840: 5141 6e61 6c79 7369 732e 6174 6f6d 6963  QAnalysis.atomic
-00000850: 5f73 7973 7465 6d2e 6174 6f6d 6963 5f73  _system.atomic_s
-00000860: 7973 7465 6d94 7d94 2868 184b 0068 194b  ystem.}.(h.K.h.K
-00000870: 0068 1a4b 0068 1b4b 0068 1c4b 0668 1d4b  .h.K.h.K.h.K.h.K
-00000880: 8a68 1e4b 0175 8c24 5051 416e 616c 7973  .h.K.u.$PQAnalys
-00000890: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
-000008a0: 2e5f 6465 636f 7261 746f 7273 947d 9428  ._decorators.}.(
-000008b0: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-000008c0: 681c 4b00 681d 4b18 681e 4b00 758c 2150  h.K.h.K.h.K.u.!P
-000008d0: 5141 6e61 6c79 7369 732e 6174 6f6d 6963  QAnalysis.atomic
-000008e0: 5f73 7973 7465 6d2e 5f5f 696e 6974 5f5f  _system.__init__
-000008f0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00000900: 681b 4b00 681c 4b00 681d 4b02 681e 4b00  h.K.h.K.h.K.h.K.
-00000910: 758c 2350 5141 6e61 6c79 7369 732e 6174  u.#PQAnalysis.at
-00000920: 6f6d 6963 5f73 7973 7465 6d2e 6578 6365  omic_system.exce
-00000930: 7074 696f 6e73 947d 9428 6818 4b00 6819  ptions.}.(h.K.h.
-00000940: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
-00000950: 4b12 681e 4b00 758c 1c50 5141 6e61 6c79  K.h.K.u..PQAnaly
-00000960: 7369 732e 616e 616c 7973 6973 2e5f 5f69  sis.analysis.__i
-00000970: 6e69 745f 5f94 7d94 2868 184b 0068 194b  nit__.}.(h.K.h.K
-00000980: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
-00000990: 0168 1e4b 0075 8c1b 5051 416e 616c 7973  .h.K.u..PQAnalys
-000009a0: 6973 2e61 6e61 6c79 7369 732e 7264 662e  is.analysis.rdf.
-000009b0: 6170 6994 7d94 2868 184b 0068 194b 0068  api.}.(h.K.h.K.h
-000009c0: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 1e68  .K.h.K.h.K.h.K.h
-000009d0: 1e4b 0075 8c2e 5051 416e 616c 7973 6973  .K.u..PQAnalysis
-000009e0: 2e61 6e61 6c79 7369 732e 7264 662e 7264  .analysis.rdf.rd
-000009f0: 665f 6f75 7470 7574 5f66 696c 655f 7772  f_output_file_wr
-00000a00: 6974 6572 947d 9428 6818 4b00 6819 4b00  iter.}.(h.K.h.K.
-00000a10: 681a 4b00 681b 4b00 681c 4b00 681d 4b33  h.K.h.K.h.K.h.K3
-00000a20: 681e 4b00 758c 2d50 5141 6e61 6c79 7369  h.K.u.-PQAnalysi
-00000a30: 732e 616e 616c 7973 6973 2e72 6466 2e72  s.analysis.rdf.r
-00000a40: 6466 5f69 6e70 7574 5f66 696c 655f 7265  df_input_file_re
-00000a50: 6164 6572 947d 9428 6818 4b00 6819 4b00  ader.}.(h.K.h.K.
-00000a60: 681a 4b00 681b 4b00 681c 4b00 681d 4b18  h.K.h.K.h.K.h.K.
-00000a70: 681e 4b00 758c 2050 5141 6e61 6c79 7369  h.K.u. PQAnalysi
-00000a80: 732e 616e 616c 7973 6973 2e72 6466 2e5f  s.analysis.rdf._
-00000a90: 5f69 6e69 745f 5f94 7d94 2868 184b 0068  _init__.}.(h.K.h
-00000aa0: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
-00000ab0: 1d4b 0568 1e4b 0075 8c1b 5051 416e 616c  .K.h.K.u..PQAnal
-00000ac0: 7973 6973 2e61 6e61 6c79 7369 732e 7264  ysis.analysis.rd
-00000ad0: 662e 7264 6694 7d94 2868 184b 0068 194b  f.rdf.}.(h.K.h.K
-00000ae0: 0068 1a4b 0068 1b4b 0068 1c4b 0368 1d4b  .h.K.h.K.h.K.h.K
-00000af0: 9a68 1e4b 0075 8c22 5051 416e 616c 7973  .h.K.u."PQAnalys
-00000b00: 6973 2e61 6e61 6c79 7369 732e 7264 662e  is.analysis.rdf.
-00000b10: 6578 6365 7074 696f 6e73 947d 9428 6818  exceptions.}.(h.
-00000b20: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
-00000b30: 4b00 681d 4b09 681e 4b00 758c 1150 5141  K.h.K.h.K.u..PQA
-00000b40: 6e61 6c79 7369 732e 696f 2e61 7069 947d  nalysis.io.api.}
-00000b50: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-00000b60: 4b00 681c 4b00 681d 4b11 681e 4b00 758c  K.h.K.h.K.h.K.u.
-00000b70: 1250 5141 6e61 6c79 7369 732e 696f 2e62  .PQAnalysis.io.b
-00000b80: 6173 6594 7d94 2868 184b 0068 194b 0068  ase.}.(h.K.h.K.h
-00000b90: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 3268  .K.h.K.h.K.h.K2h
-00000ba0: 1e4b 0075 8c18 5051 416e 616c 7973 6973  .K.u..PQAnalysis
-00000bb0: 2e69 6f2e 626f 785f 7772 6974 6572 947d  .io.box_writer.}
-00000bc0: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-00000bd0: 4b00 681c 4b00 681d 4b2c 681e 4b00 758c  K.h.K.h.K,h.K.u.
-00000be0: 2250 5141 6e61 6c79 7369 732e 696f 2e6d  "PQAnalysis.io.m
-00000bf0: 6f6c 6465 7363 7269 7074 6f72 5f72 6561  oldescriptor_rea
-00000c00: 6465 7294 7d94 2868 184b 0068 194b 0068  der.}.(h.K.h.K.h
-00000c10: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 3968  .K.h.K.h.K.h.K9h
-00000c20: 1e4b 0275 8c20 5051 416e 616c 7973 6973  .K.u. PQAnalysis
-00000c30: 2e69 6f2e 656e 6572 6779 5f66 696c 655f  .io.energy_file_
-00000c40: 7265 6164 6572 947d 9428 6818 4b00 6819  reader.}.(h.K.h.
-00000c50: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
-00000c60: 4b2e 681e 4b00 758c 1650 5141 6e61 6c79  K.h.K.u..PQAnaly
-00000c70: 7369 732e 696f 2e5f 5f69 6e69 745f 5f94  sis.io.__init__.
-00000c80: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00000c90: 1b4b 0068 1c4b 0068 1d4b 1a68 1e4b 0075  .K.h.K.h.K.h.K.u
-00000ca0: 8c17 5051 416e 616c 7973 6973 2e69 6f2e  ..PQAnalysis.io.
-00000cb0: 7772 6974 655f 6170 6994 7d94 2868 184b  write_api.}.(h.K
-00000cc0: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-00000cd0: 0068 1d4b 1468 1e4b 0175 8c1e 5051 416e  .h.K.h.K.u..PQAn
-00000ce0: 616c 7973 6973 2e69 6f2e 696e 666f 5f66  alysis.io.info_f
-00000cf0: 696c 655f 7265 6164 6572 947d 9428 6818  ile_reader.}.(h.
-00000d00: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
-00000d10: 4b01 681d 4b37 681e 4b00 758c 1c50 5141  K.h.K7h.K.u..PQA
-00000d20: 6e61 6c79 7369 732e 696f 2e63 6f6e 7665  nalysis.io.conve
-00000d30: 7273 696f 6e5f 6170 6994 7d94 2868 184b  rsion_api.}.(h.K
-00000d40: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-00000d50: 0068 1d4b 2768 1e4b 0075 8c18 5051 416e  .h.K'h.K.u..PQAn
-00000d60: 616c 7973 6973 2e69 6f2e 6578 6365 7074  alysis.io.except
-00000d70: 696f 6e73 947d 9428 6818 4b00 6819 4b00  ions.}.(h.K.h.K.
-00000d80: 681a 4b00 681b 4b00 681c 4b00 681d 4b06  h.K.h.K.h.K.h.K.
-00000d90: 681e 4b00 758c 1550 5141 6e61 6c79 7369  h.K.u..PQAnalysi
-00000da0: 732e 696f 2e66 6f72 6d61 7473 947d 9428  s.io.formats.}.(
-00000db0: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-00000dc0: 681c 4b01 681d 4b51 681e 4b00 758c 2850  h.K.h.KQh.K.u.(P
-00000dd0: 5141 6e61 6c79 7369 732e 696f 2e69 6e70  QAnalysis.io.inp
-00000de0: 7574 5f66 696c 655f 7265 6164 6572 2e5f  ut_file_reader._
-00000df0: 5f69 6e69 745f 5f94 7d94 2868 184b 0068  _init__.}.(h.K.h
-00000e00: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
-00000e10: 1d4b 0468 1e4b 0075 8c2a 5051 416e 616c  .K.h.K.u.*PQAnal
-00000e20: 7973 6973 2e69 6f2e 696e 7075 745f 6669  ysis.io.input_fi
-00000e30: 6c65 5f72 6561 6465 722e 6578 6365 7074  le_reader.except
-00000e40: 696f 6e73 947d 9428 6818 4b00 6819 4b00  ions.}.(h.K.h.K.
-00000e50: 681a 4b00 681b 4b00 681c 4b00 681d 4b0e  h.K.h.K.h.K.h.K.
-00000e60: 681e 4b00 758c 2750 5141 6e61 6c79 7369  h.K.u.'PQAnalysi
-00000e70: 732e 696f 2e69 6e70 7574 5f66 696c 655f  s.io.input_file_
-00000e80: 7265 6164 6572 2e66 6f72 6d61 7473 947d  reader.formats.}
-00000e90: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-00000ea0: 4b00 681c 4b00 681d 4b0f 681e 4b00 758c  K.h.K.h.K.h.K.u.
-00000eb0: 3150 5141 6e61 6c79 7369 732e 696f 2e69  1PQAnalysis.io.i
-00000ec0: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
-00000ed0: 2e69 6e70 7574 5f66 696c 655f 7061 7273  .input_file_pars
-00000ee0: 6572 947d 9428 6818 4b00 6819 4b00 681a  er.}.(h.K.h.K.h.
-00000ef0: 4b00 681b 4b00 681c 4b01 681d 4b7e 681e  K.h.K.h.K.h.K~h.
-00000f00: 4b00 758c 3250 5141 6e61 6c79 7369 732e  K.u.2PQAnalysis.
-00000f10: 696f 2e69 6e70 7574 5f66 696c 655f 7265  io.input_file_re
-00000f20: 6164 6572 2e70 715f 616e 616c 7973 6973  ader.pq_analysis
-00000f30: 2e5f 7061 7273 6594 7d94 2868 184b 0068  ._parse.}.(h.K.h
-00000f40: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0168  .K.h.K.h.K.h.K.h
-00000f50: 1d4b 4468 1e4b 0075 8c37 5051 416e 616c  .KDh.K.u.7PQAnal
-00000f60: 7973 6973 2e69 6f2e 696e 7075 745f 6669  ysis.io.input_fi
-00000f70: 6c65 5f72 6561 6465 722e 7071 5f61 6e61  le_reader.pq_ana
-00000f80: 6c79 7369 732e 5f66 696c 655f 6d69 7869  lysis._file_mixi
-00000f90: 6e94 7d94 2868 184b 0068 194b 0068 1a4b  n.}.(h.K.h.K.h.K
-00000fa0: 0068 1b4b 0068 1c4b 0068 1d4b 0d68 1e4b  .h.K.h.K.h.K.h.K
-00000fb0: 0075 8c3c 5051 416e 616c 7973 6973 2e69  .u.<PQAnalysis.i
-00000fc0: 6f2e 696e 7075 745f 6669 6c65 5f72 6561  o.input_file_rea
-00000fd0: 6465 722e 7071 5f61 6e61 6c79 7369 732e  der.pq_analysis.
-00000fe0: 5f70 6f73 6974 696f 6e73 5f6d 6978 696e  _positions_mixin
-00000ff0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00001000: 681b 4b00 681c 4b00 681d 4b0b 681e 4b00  h.K.h.K.h.K.h.K.
-00001010: 758c 3450 5141 6e61 6c79 7369 732e 696f  u.4PQAnalysis.io
-00001020: 2e69 6e70 7574 5f66 696c 655f 7265 6164  .input_file_read
-00001030: 6572 2e70 715f 616e 616c 7973 6973 2e5f  er.pq_analysis._
-00001040: 5f69 6e69 745f 5f94 7d94 2868 184b 0068  _init__.}.(h.K.h
-00001050: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
-00001060: 1d4b 0168 1e4b 0075 8c3c 5051 416e 616c  .K.h.K.u.<PQAnal
-00001070: 7973 6973 2e69 6f2e 696e 7075 745f 6669  ysis.io.input_fi
-00001080: 6c65 5f72 6561 6465 722e 7071 5f61 6e61  le_reader.pq_ana
-00001090: 6c79 7369 732e 5f73 656c 6563 7469 6f6e  lysis._selection
-000010a0: 5f6d 6978 696e 947d 9428 6818 4b00 6819  _mixin.}.(h.K.h.
-000010b0: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
-000010c0: 4b0c 681e 4b00 758c 4850 5141 6e61 6c79  K.h.K.u.HPQAnaly
-000010d0: 7369 732e 696f 2e69 6e70 7574 5f66 696c  sis.io.input_fil
-000010e0: 655f 7265 6164 6572 2e70 715f 616e 616c  e_reader.pq_anal
-000010f0: 7973 6973 2e70 7161 6e61 6c79 7369 735f  ysis.pqanalysis_
-00001100: 696e 7075 745f 6669 6c65 5f72 6561 6465  input_file_reade
-00001110: 7294 7d94 2868 184b 0068 194b 0068 1a4b  r.}.(h.K.h.K.h.K
-00001120: 0068 1b4b 0068 1c4b 0068 1d4b 3b68 1e4b  .h.K.h.K.h.K;h.K
-00001130: 0075 8c2f 5051 416e 616c 7973 6973 2e69  .u./PQAnalysis.i
-00001140: 6f2e 696e 7075 745f 6669 6c65 5f72 6561  o.input_file_rea
-00001150: 6465 722e 7071 2e6f 7574 7075 745f 6669  der.pq.output_fi
-00001160: 6c65 7394 7d94 2868 184b 0068 194b 0068  les.}.(h.K.h.K.h
-00001170: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 3268  .K.h.K.h.K.h.K2h
-00001180: 1e4b 0075 8c37 5051 416e 616c 7973 6973  .K.u.7PQAnalysis
-00001190: 2e69 6f2e 696e 7075 745f 6669 6c65 5f72  .io.input_file_r
-000011a0: 6561 6465 722e 7071 2e70 715f 696e 7075  eader.pq.pq_inpu
-000011b0: 745f 6669 6c65 5f72 6561 6465 7294 7d94  t_file_reader.}.
-000011c0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-000011d0: 0068 1c4b 0168 1d4b 5868 1e4b 0075 8c2b  .h.K.h.KXh.K.u.+
-000011e0: 5051 416e 616c 7973 6973 2e69 6f2e 696e  PQAnalysis.io.in
-000011f0: 7075 745f 6669 6c65 5f72 6561 6465 722e  put_file_reader.
-00001200: 7071 2e5f 5f69 6e69 745f 5f94 7d94 2868  pq.__init__.}.(h
-00001210: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-00001220: 1c4b 0068 1d4b 0168 1e4b 0075 8c1e 5051  .K.h.K.h.K.u..PQ
-00001230: 416e 616c 7973 6973 2e69 6f2e 7265 7374  Analysis.io.rest
-00001240: 6172 745f 6669 6c65 2e61 7069 947d 9428  art_file.api.}.(
-00001250: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-00001260: 681c 4b00 681d 4b08 681e 4b00 758c 2950  h.K.h.K.h.K.u.)P
-00001270: 5141 6e61 6c79 7369 732e 696f 2e72 6573  QAnalysis.io.res
-00001280: 7461 7274 5f66 696c 652e 7265 7374 6172  tart_file.restar
-00001290: 745f 7265 6164 6572 947d 9428 6818 4b00  t_reader.}.(h.K.
-000012a0: 6819 4b00 681a 4b00 681b 4b00 681c 4b01  h.K.h.K.h.K.h.K.
-000012b0: 681d 4b49 681e 4b00 758c 2350 5141 6e61  h.KIh.K.u.#PQAna
-000012c0: 6c79 7369 732e 696f 2e72 6573 7461 7274  lysis.io.restart
-000012d0: 5f66 696c 652e 5f5f 696e 6974 5f5f 947d  _file.__init__.}
-000012e0: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-000012f0: 4b00 681c 4b00 681d 4b02 681e 4b00 758c  K.h.K.h.K.h.K.u.
-00001300: 2550 5141 6e61 6c79 7369 732e 696f 2e72  %PQAnalysis.io.r
-00001310: 6573 7461 7274 5f66 696c 652e 6578 6365  estart_file.exce
-00001320: 7074 696f 6e73 947d 9428 6818 4b00 6819  ptions.}.(h.K.h.
-00001330: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
-00001340: 4b03 681e 4b00 758c 2950 5141 6e61 6c79  K.h.K.u.)PQAnaly
-00001350: 7369 732e 696f 2e72 6573 7461 7274 5f66  sis.io.restart_f
-00001360: 696c 652e 7265 7374 6172 745f 7772 6974  ile.restart_writ
-00001370: 6572 947d 9428 6818 4b00 6819 4b00 681a  er.}.(h.K.h.K.h.
-00001380: 4b00 681b 4b00 681c 4b00 681d 4b3d 681e  K.h.K.h.K.h.K=h.
-00001390: 4b00 758c 1b50 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
-000013a0: 696f 2e74 7261 6a5f 6669 6c65 2e61 7069  io.traj_file.api
-000013b0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-000013c0: 681b 4b00 681c 4b00 681d 4b13 681e 4b00  h.K.h.K.h.K.h.K.
-000013d0: 758c 2950 5141 6e61 6c79 7369 732e 696f  u.)PQAnalysis.io
-000013e0: 2e74 7261 6a5f 6669 6c65 2e74 7261 6a65  .traj_file.traje
-000013f0: 6374 6f72 795f 7265 6164 6572 947d 9428  ctory_reader.}.(
+000007a0: 1b4b 0068 1c4b 0468 1d4b 5268 1e4b 0075  .K.h.K.h.KRh.K.u
+000007b0: 8c12 5051 416e 616c 7973 6973 2e63 6c69  ..PQAnalysis.cli
+000007c0: 2e72 6466 947d 9428 6818 4b00 6819 4b00  .rdf.}.(h.K.h.K.
+000007d0: 681a 4b00 681b 4b00 681c 4b00 681d 4b1f  h.K.h.K.h.K.h.K.
+000007e0: 681e 4b00 758c 1d50 5141 6e61 6c79 7369  h.K.u..PQAnalysi
+000007f0: 732e 636c 692e 6275 696c 645f 6e65 705f  s.cli.build_nep_
+00000800: 7472 616a 947d 9428 6818 4b00 6819 4b00  traj.}.(h.K.h.K.
+00000810: 681a 4b00 681b 4b00 681c 4b00 681d 4b1f  h.K.h.K.h.K.h.K.
+00000820: 681e 4b00 758c 1650 5141 6e61 6c79 7369  h.K.u..PQAnalysi
+00000830: 732e 636c 692e 7879 7a32 6765 6e94 7d94  s.cli.xyz2gen.}.
+00000840: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+00000850: 0068 1c4b 0068 1d4b 1b68 1e4b 0075 8c18  .h.K.h.K.h.K.u..
+00000860: 5051 416e 616c 7973 6973 2e63 6c69 2e5f  PQAnalysis.cli._
+00000870: 636c 695f 6261 7365 947d 9428 6818 4b00  cli_base.}.(h.K.
+00000880: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
+00000890: 681d 4b05 681e 4b00 758c 1750 5141 6e61  h.K.h.K.u..PQAna
+000008a0: 6c79 7369 732e 636c 692e 7472 616a 3262  lysis.cli.traj2b
+000008b0: 6f78 947d 9428 6818 4b00 6819 4b00 681a  ox.}.(h.K.h.K.h.
+000008c0: 4b00 681b 4b00 681c 4b00 681d 4b1a 681e  K.h.K.h.K.h.K.h.
+000008d0: 4b00 758c 1c50 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
+000008e0: 636c 692e 6164 645f 6d6f 6c65 6375 6c65  cli.add_molecule
+000008f0: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
+00000900: 0068 1b4b 0068 1c4b 0068 1d4b 2868 1e4b  .h.K.h.K.h.K(h.K
+00000910: 0075 8c17 5051 416e 616c 7973 6973 2e63  .u..PQAnalysis.c
+00000920: 6c69 2e5f 5f69 6e69 745f 5f94 7d94 2868  li.__init__.}.(h
+00000930: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+00000940: 1c4b 0068 1d4b 0268 1e4b 0075 8c1d 5051  .K.h.K.h.K.u..PQ
+00000950: 416e 616c 7973 6973 2e63 6c69 2e63 6f6e  Analysis.cli.con
+00000960: 7469 6e75 655f 696e 7075 7494 7d94 2868  tinue_input.}.(h
+00000970: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+00000980: 1c4b 0068 1d4b 1a68 1e4b 0075 8c16 5051  .K.h.K.h.K.u..PQ
+00000990: 416e 616c 7973 6973 2e63 6c69 2e72 7374  Analysis.cli.rst
+000009a0: 3278 797a 947d 9428 6818 4b00 6819 4b00  2xyz.}.(h.K.h.K.
+000009b0: 681a 4b00 681b 4b00 681c 4b00 681d 4b1b  h.K.h.K.h.K.h.K.
+000009c0: 681e 4b00 758c 1650 5141 6e61 6c79 7369  h.K.u..PQAnalysi
+000009d0: 732e 636c 692e 6765 6e32 7879 7a94 7d94  s.cli.gen2xyz.}.
+000009e0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+000009f0: 0068 1c4b 0068 1d4b 1b68 1e4b 0075 8c13  .h.K.h.K.h.K.u..
+00000a00: 5051 416e 616c 7973 6973 2e63 6c69 2e6d  PQAnalysis.cli.m
+00000a10: 6169 6e94 7d94 2868 184b 0068 194b 0068  ain.}.(h.K.h.K.h
+00000a20: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 1c68  .K.h.K.h.K.h.K.h
+00000a30: 1e4b 0075 8c1f 5051 416e 616c 7973 6973  .K.u..PQAnalysis
+00000a40: 2e63 6c69 2e5f 6172 6775 6d65 6e74 5f70  .cli._argument_p
+00000a50: 6172 7365 7294 7d94 2868 184b 0068 194b  arser.}.(h.K.h.K
+00000a60: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
+00000a70: 3368 1e4b 0075 8c19 5051 416e 616c 7973  3h.K.u..PQAnalys
+00000a80: 6973 2e63 6c69 2e74 7261 6a32 716d 6366  is.cli.traj2qmcf
+00000a90: 6394 7d94 2868 184b 0068 194b 0068 1a4b  c.}.(h.K.h.K.h.K
+00000aa0: 0068 1b4b 0068 1c4b 0068 1d4b 1968 1e4b  .h.K.h.K.h.K.h.K
+00000ab0: 0075 8c23 5051 416e 616c 7973 6973 2e70  .u.#PQAnalysis.p
+00000ac0: 6879 7369 6361 6c5f 6461 7461 2e65 7863  hysical_data.exc
+00000ad0: 6570 7469 6f6e 7394 7d94 2868 184b 0068  eptions.}.(h.K.h
+00000ae0: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
+00000af0: 1d4b 0568 1e4b 0075 8c1f 5051 416e 616c  .K.h.K.u..PQAnal
+00000b00: 7973 6973 2e70 6879 7369 6361 6c5f 6461  ysis.physical_da
+00000b10: 7461 2e65 6e65 7267 7994 7d94 2868 184b  ta.energy.}.(h.K
+00000b20: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
+00000b30: 0068 1d4b 3e68 1e4b 0075 8c21 5051 416e  .h.K>h.K.u.!PQAn
+00000b40: 616c 7973 6973 2e70 6879 7369 6361 6c5f  alysis.physical_
+00000b50: 6461 7461 2e5f 5f69 6e69 745f 5f94 7d94  data.__init__.}.
+00000b60: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+00000b70: 0068 1c4b 0068 1d4b 0268 1e4b 0075 8c23  .h.K.h.K.h.K.u.#
+00000b80: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
+00000b90: 635f 7379 7374 656d 2e65 7863 6570 7469  c_system.excepti
+00000ba0: 6f6e 7394 7d94 2868 184b 0068 194b 0068  ons.}.(h.K.h.K.h
+00000bb0: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 1268  .K.h.K.h.K.h.K.h
+00000bc0: 1e4b 0075 8c24 5051 416e 616c 7973 6973  .K.u.$PQAnalysis
+00000bd0: 2e61 746f 6d69 635f 7379 7374 656d 2e5f  .atomic_system._
+00000be0: 6465 636f 7261 746f 7273 947d 9428 6818  decorators.}.(h.
+00000bf0: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
+00000c00: 4b00 681d 4b18 681e 4b00 758c 2650 5141  K.h.K.h.K.u.&PQA
+00000c10: 6e61 6c79 7369 732e 6174 6f6d 6963 5f73  nalysis.atomic_s
+00000c20: 7973 7465 6d2e 6174 6f6d 6963 5f73 7973  ystem.atomic_sys
+00000c30: 7465 6d94 7d94 2868 184b 0068 194b 0068  tem.}.(h.K.h.K.h
+00000c40: 1a4b 0068 1b4b 0068 1c4b 0668 1d4b a568  .K.h.K.h.K.h.K.h
+00000c50: 1e4b 0175 8c21 5051 416e 616c 7973 6973  .K.u.!PQAnalysis
+00000c60: 2e61 746f 6d69 635f 7379 7374 656d 2e5f  .atomic_system._
+00000c70: 5f69 6e69 745f 5f94 7d94 2868 184b 0068  _init__.}.(h.K.h
+00000c80: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
+00000c90: 1d4b 0268 1e4b 0075 8c24 5051 416e 616c  .K.h.K.u.$PQAnal
+00000ca0: 7973 6973 2e61 746f 6d69 635f 7379 7374  ysis.atomic_syst
+00000cb0: 656d 2e5f 7072 6f70 6572 7469 6573 947d  em._properties.}
+00000cc0: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+00000cd0: 4b00 681c 4b00 681d 4b28 681e 4b00 758c  K.h.K.h.K(h.K.u.
+00000ce0: 2350 5141 6e61 6c79 7369 732e 6174 6f6d  #PQAnalysis.atom
+00000cf0: 6963 5f73 7973 7465 6d2e 5f70 6f73 6974  ic_system._posit
+00000d00: 696f 6e73 947d 9428 6818 4b00 6819 4b00  ions.}.(h.K.h.K.
+00000d10: 681a 4b00 681b 4b00 681c 4b00 681d 4b19  h.K.h.K.h.K.h.K.
+00000d20: 681e 4b00 758c 2d50 5141 6e61 6c79 7369  h.K.u.-PQAnalysi
+00000d30: 732e 6174 6f6d 6963 5f73 7973 7465 6d2e  s.atomic_system.
+00000d40: 5f73 7461 6e64 6172 645f 7072 6f70 6572  _standard_proper
+00000d50: 7469 6573 947d 9428 6818 4b00 6819 4b00  ties.}.(h.K.h.K.
+00000d60: 681a 4b00 681b 4b00 681c 4b02 681d 4b44  h.K.h.K.h.K.h.KD
+00000d70: 681e 4b00 758c 1a50 5141 6e61 6c79 7369  h.K.u..PQAnalysi
+00000d80: 732e 7472 616a 2e65 7863 6570 7469 6f6e  s.traj.exception
+00000d90: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
+00000da0: 0068 1b4b 0068 1c4b 0068 1d4b 0768 1e4b  .h.K.h.K.h.K.h.K
+00000db0: 0075 8c17 5051 416e 616c 7973 6973 2e74  .u..PQAnalysis.t
+00000dc0: 7261 6a2e 666f 726d 6174 7394 7d94 2868  raj.formats.}.(h
+00000dd0: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+00000de0: 1c4b 0168 1d4b 2d68 1e4b 0075 8c13 5051  .K.h.K-h.K.u..PQ
+00000df0: 416e 616c 7973 6973 2e74 7261 6a2e 6170  Analysis.traj.ap
+00000e00: 6994 7d94 2868 184b 0068 194b 0068 1a4b  i.}.(h.K.h.K.h.K
+00000e10: 0068 1b4b 0068 1c4b 0068 1d4b 0868 1e4b  .h.K.h.K.h.K.h.K
+00000e20: 0075 8c1a 5051 416e 616c 7973 6973 2e74  .u..PQAnalysis.t
+00000e30: 7261 6a2e 7472 616a 6563 746f 7279 947d  raj.trajectory.}
+00000e40: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+00000e50: 4b00 681c 4b00 681d 4b66 681e 4b00 758c  K.h.K.h.Kfh.K.u.
+00000e60: 1850 5141 6e61 6c79 7369 732e 7472 616a  .PQAnalysis.traj
+00000e70: 2e5f 5f69 6e69 745f 5f94 7d94 2868 184b  .__init__.}.(h.K
+00000e80: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
+00000e90: 0068 1d4b 0468 1e4b 0075 8c1a 5051 416e  .h.K.h.K.u..PQAn
+00000ea0: 616c 7973 6973 2e63 6f72 652e 6578 6365  alysis.core.exce
+00000eb0: 7074 696f 6e73 947d 9428 6818 4b00 6819  ptions.}.(h.K.h.
+00000ec0: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
+00000ed0: 4b10 681e 4b00 758c 1350 5141 6e61 6c79  K.h.K.u..PQAnaly
+00000ee0: 7369 732e 636f 7265 2e61 7069 947d 9428  sis.core.api.}.(
+00000ef0: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+00000f00: 681c 4b00 681d 4b09 681e 4b01 758c 1750  h.K.h.K.h.K.u..P
+00000f10: 5141 6e61 6c79 7369 732e 636f 7265 2e72  QAnalysis.core.r
+00000f20: 6573 6964 7565 947d 9428 6818 4b00 6819  esidue.}.(h.K.h.
+00000f30: 4b00 681a 4b00 681b 4b00 681c 4b02 681d  K.h.K.h.K.h.K.h.
+00000f40: 4b50 681e 4b00 758c 1850 5141 6e61 6c79  KPh.K.u..PQAnaly
+00000f50: 7369 732e 636f 7265 2e5f 5f69 6e69 745f  sis.core.__init_
+00000f60: 5f94 7d94 2868 184b 0068 194b 0068 1a4b  _.}.(h.K.h.K.h.K
+00000f70: 0068 1b4b 0068 1c4b 0068 1d4b 0568 1e4b  .h.K.h.K.h.K.h.K
+00000f80: 0075 8c1d 5051 416e 616c 7973 6973 2e63  .u..PQAnalysis.c
+00000f90: 6f72 652e 6174 6f6d 2e5f 5f69 6e69 745f  ore.atom.__init_
+00000fa0: 5f94 7d94 2868 184b 0068 194b 0068 1a4b  _.}.(h.K.h.K.h.K
+00000fb0: 0068 1b4b 0068 1c4b 0068 1d4b 0268 1e4b  .h.K.h.K.h.K.h.K
+00000fc0: 0075 8c19 5051 416e 616c 7973 6973 2e63  .u..PQAnalysis.c
+00000fd0: 6f72 652e 6174 6f6d 2e61 746f 6d94 7d94  ore.atom.atom.}.
+00000fe0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+00000ff0: 0068 1c4b 0068 1d4b 3968 1e4b 0075 8c1c  .h.K.h.K9h.K.u..
+00001000: 5051 416e 616c 7973 6973 2e63 6f72 652e  PQAnalysis.core.
+00001010: 6174 6f6d 2e65 6c65 6d65 6e74 947d 9428  atom.element.}.(
+00001020: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+00001030: 681c 4b00 681d 4b34 681e 4b00 758c 1950  h.K.h.K4h.K.u..P
+00001040: 5141 6e61 6c79 7369 732e 636f 7265 2e63  QAnalysis.core.c
+00001050: 656c 6c2e 6365 6c6c 947d 9428 6818 4b00  ell.cell.}.(h.K.
+00001060: 6819 4b00 681a 4b00 681b 4b00 681c 4b01  h.K.h.K.h.K.h.K.
+00001070: 681d 4b53 681e 4b00 758c 1d50 5141 6e61  h.KSh.K.u..PQAna
+00001080: 6c79 7369 732e 636f 7265 2e63 656c 6c2e  lysis.core.cell.
+00001090: 5f5f 696e 6974 5f5f 947d 9428 6818 4b00  __init__.}.(h.K.
+000010a0: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
+000010b0: 681d 4b01 681e 4b00 758c 2950 5141 6e61  h.K.h.K.u.)PQAna
+000010c0: 6c79 7369 732e 636f 7265 2e63 656c 6c2e  lysis.core.cell.
+000010d0: 5f73 7461 6e64 6172 645f 7072 6f70 6572  _standard_proper
+000010e0: 7469 6573 947d 9428 6818 4b00 6819 4b00  ties.}.(h.K.h.K.
+000010f0: 681a 4b00 681b 4b00 681c 4b00 681d 4b24  h.K.h.K.h.K.h.K$
+00001100: 681e 4b00 758c 1e50 5141 6e61 6c79 7369  h.K.u..PQAnalysi
+00001110: 732e 746f 706f 6c6f 6779 2e65 7863 6570  s.topology.excep
+00001120: 7469 6f6e 7394 7d94 2868 184b 0068 194b  tions.}.(h.K.h.K
+00001130: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
+00001140: 0568 1e4b 0075 8c1c 5051 416e 616c 7973  .h.K.u..PQAnalys
+00001150: 6973 2e74 6f70 6f6c 6f67 792e 746f 706f  is.topology.topo
+00001160: 6c6f 6779 947d 9428 6818 4b00 6819 4b00  logy.}.(h.K.h.K.
+00001170: 681a 4b00 681b 4b00 681c 4b02 681d 4ba7  h.K.h.K.h.K.h.K.
+00001180: 681e 4b00 758c 1750 5141 6e61 6c79 7369  h.K.u..PQAnalysi
+00001190: 732e 746f 706f 6c6f 6779 2e61 7069 947d  s.topology.api.}
+000011a0: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+000011b0: 4b00 681c 4b00 681d 4b11 681e 4b00 758c  K.h.K.h.K.h.K.u.
+000011c0: 1c50 5141 6e61 6c79 7369 732e 746f 706f  .PQAnalysis.topo
+000011d0: 6c6f 6779 2e5f 5f69 6e69 745f 5f94 7d94  logy.__init__.}.
+000011e0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+000011f0: 0068 1c4b 0068 1d4b 0768 1e4b 0275 8c1d  .h.K.h.K.h.K.u..
+00001200: 5051 416e 616c 7973 6973 2e74 6f70 6f6c  PQAnalysis.topol
+00001210: 6f67 792e 7365 6c65 6374 696f 6e94 7d94  ogy.selection.}.
+00001220: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+00001230: 0068 1c4b 0168 1d4b 9268 1e4b 0075 8c22  .h.K.h.K.h.K.u."
+00001240: 5051 416e 616c 7973 6973 2e74 6f70 6f6c  PQAnalysis.topol
+00001250: 6f67 792e 7368 616b 655f 746f 706f 6c6f  ogy.shake_topolo
+00001260: 6779 947d 9428 6818 4b00 6819 4b00 681a  gy.}.(h.K.h.K.h.
+00001270: 4b00 681b 4b00 681c 4b00 681d 4b48 681e  K.h.K.h.K.h.KHh.
+00001280: 4b00 758c 2c50 5141 6e61 6c79 7369 732e  K.u.,PQAnalysis.
+00001290: 746f 706f 6c6f 6779 2e62 6f6e 6465 645f  topology.bonded_
+000012a0: 746f 706f 6c6f 6779 2e64 6968 6564 7261  topology.dihedra
+000012b0: 6c94 7d94 2868 184b 0068 194b 0068 1a4b  l.}.(h.K.h.K.h.K
+000012c0: 0068 1b4b 0068 1c4b 0268 1d4b 1268 1e4b  .h.K.h.K.h.K.h.K
+000012d0: 0075 8c38 5051 416e 616c 7973 6973 2e74  .u.8PQAnalysis.t
+000012e0: 6f70 6f6c 6f67 792e 626f 6e64 6564 5f74  opology.bonded_t
+000012f0: 6f70 6f6c 6f67 792e 5f74 6f70 6f6c 6f67  opology._topolog
+00001300: 795f 7072 6f70 6572 7469 6573 947d 9428  y_properties.}.(
+00001310: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+00001320: 681c 4b00 681d 4b2e 681e 4b00 758c 2c50  h.K.h.K.h.K.u.,P
+00001330: 5141 6e61 6c79 7369 732e 746f 706f 6c6f  QAnalysis.topolo
+00001340: 6779 2e62 6f6e 6465 645f 746f 706f 6c6f  gy.bonded_topolo
+00001350: 6779 2e5f 5f69 6e69 745f 5f94 7d94 2868  gy.__init__.}.(h
+00001360: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+00001370: 1c4b 0068 1d4b 0068 1e4b 0075 8c28 5051  .K.h.K.h.K.u.(PQ
+00001380: 416e 616c 7973 6973 2e74 6f70 6f6c 6f67  Analysis.topolog
+00001390: 792e 626f 6e64 6564 5f74 6f70 6f6c 6f67  y.bonded_topolog
+000013a0: 792e 626f 6e64 947d 9428 6818 4b00 6819  y.bond.}.(h.K.h.
+000013b0: 4b00 681a 4b00 681b 4b00 681c 4b01 681d  K.h.K.h.K.h.K.h.
+000013c0: 4b10 681e 4b00 758c 3350 5141 6e61 6c79  K.h.K.u.3PQAnaly
+000013d0: 7369 732e 746f 706f 6c6f 6779 2e62 6f6e  sis.topology.bon
+000013e0: 6465 645f 746f 706f 6c6f 6779 2e62 6f6e  ded_topology.bon
+000013f0: 6465 645f 746f 706f 6c6f 6779 947d 9428  ded_topology.}.(
 00001400: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-00001410: 681c 4b05 681d 4b9b 681e 4b02 758c 2050  h.K.h.K.h.K.u. P
-00001420: 5141 6e61 6c79 7369 732e 696f 2e74 7261  QAnalysis.io.tra
-00001430: 6a5f 6669 6c65 2e5f 5f69 6e69 745f 5f94  j_file.__init__.
-00001440: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00001450: 1b4b 0068 1c4b 0068 1d4b 0368 1e4b 0075  .K.h.K.h.K.h.K.u
-00001460: 8c29 5051 416e 616c 7973 6973 2e69 6f2e  .)PQAnalysis.io.
-00001470: 7472 616a 5f66 696c 652e 7472 616a 6563  traj_file.trajec
-00001480: 746f 7279 5f77 7269 7465 7294 7d94 2868  tory_writer.}.(h
-00001490: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-000014a0: 1c4b 0068 1d4b 4f68 1e4b 0075 8c22 5051  .K.h.KOh.K.u."PQ
-000014b0: 416e 616c 7973 6973 2e69 6f2e 7472 616a  Analysis.io.traj
-000014c0: 5f66 696c 652e 6578 6365 7074 696f 6e73  _file.exceptions
-000014d0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-000014e0: 681b 4b00 681c 4b00 681d 4b03 681e 4b00  h.K.h.K.h.K.h.K.
-000014f0: 758c 2450 5141 6e61 6c79 7369 732e 696f  u.$PQAnalysis.io
-00001500: 2e74 7261 6a5f 6669 6c65 2e66 7261 6d65  .traj_file.frame
-00001510: 5f72 6561 6465 7294 7d94 2868 184b 0068  _reader.}.(h.K.h
-00001520: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0268  .K.h.K.h.K.h.K.h
-00001530: 1d4b 6e68 1e4b 0075 8c1c 5051 416e 616c  .Knh.K.u..PQAnal
-00001540: 7973 6973 2e69 6f2e 6e65 702e 6e65 705f  ysis.io.nep.nep_
-00001550: 7772 6974 6572 947d 9428 6818 4b01 6819  writer.}.(h.K.h.
-00001560: 4b00 681a 4b00 681b 4b00 681c 4b08 681d  K.h.K.h.K.h.K.h.
-00001570: 4d15 0168 1e4b 0075 8c1a 5051 416e 616c  M..h.K.u..PQAnal
-00001580: 7973 6973 2e69 6f2e 6e65 702e 5f5f 696e  ysis.io.nep.__in
-00001590: 6974 5f5f 947d 9428 6818 4b00 6819 4b00  it__.}.(h.K.h.K.
-000015a0: 681a 4b00 681b 4b00 681c 4b00 681d 4b00  h.K.h.K.h.K.h.K.
-000015b0: 681e 4b00 758c 1c50 5141 6e61 6c79 7369  h.K.u..PQAnalysi
-000015c0: 732e 696f 2e6e 6570 2e65 7863 6570 7469  s.io.nep.excepti
-000015d0: 6f6e 7394 7d94 2868 184b 0068 194b 0068  ons.}.(h.K.h.K.h
-000015e0: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0268  .K.h.K.h.K.h.K.h
-000015f0: 1e4b 0075 8c1a 5051 416e 616c 7973 6973  .K.u..PQAnalysis
-00001600: 2e69 6f2e 6765 6e5f 6669 6c65 2e61 7069  .io.gen_file.api
-00001610: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00001620: 681b 4b00 681c 4b00 681d 4b09 681e 4b00  h.K.h.K.h.K.h.K.
-00001630: 758c 2650 5141 6e61 6c79 7369 732e 696f  u.&PQAnalysis.io
-00001640: 2e67 656e 5f66 696c 652e 6765 6e5f 6669  .gen_file.gen_fi
-00001650: 6c65 5f72 6561 6465 7294 7d94 2868 184b  le_reader.}.(h.K
-00001660: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-00001670: 0068 1d4b 2f68 1e4b 0075 8c1f 5051 416e  .h.K/h.K.u..PQAn
-00001680: 616c 7973 6973 2e69 6f2e 6765 6e5f 6669  alysis.io.gen_fi
-00001690: 6c65 2e5f 5f69 6e69 745f 5f94 7d94 2868  le.__init__.}.(h
-000016a0: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-000016b0: 1c4b 0068 1d4b 0368 1e4b 0075 8c26 5051  .K.h.K.h.K.u.&PQ
-000016c0: 416e 616c 7973 6973 2e69 6f2e 6765 6e5f  Analysis.io.gen_
-000016d0: 6669 6c65 2e67 656e 5f66 696c 655f 7772  file.gen_file_wr
-000016e0: 6974 6572 947d 9428 6818 4b00 6819 4b00  iter.}.(h.K.h.K.
-000016f0: 681a 4b00 681b 4b00 681c 4b00 681d 4b2c  h.K.h.K.h.K.h.K,
-00001700: 681e 4b00 758c 2150 5141 6e61 6c79 7369  h.K.u.!PQAnalysi
-00001710: 732e 696f 2e67 656e 5f66 696c 652e 6578  s.io.gen_file.ex
-00001720: 6365 7074 696f 6e73 947d 9428 6818 4b00  ceptions.}.(h.K.
-00001730: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
-00001740: 681d 4b02 681e 4b00 758c 1f50 5141 6e61  h.K.h.K.u..PQAna
-00001750: 6c79 7369 732e 696f 2e74 6f70 6f6c 6f67  lysis.io.topolog
-00001760: 795f 6669 6c65 2e61 7069 947d 9428 6818  y_file.api.}.(h.
-00001770: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
-00001780: 4b00 681d 4b09 681e 4b00 758c 3050 5141  K.h.K.h.K.u.0PQA
-00001790: 6e61 6c79 7369 732e 696f 2e74 6f70 6f6c  nalysis.io.topol
-000017a0: 6f67 795f 6669 6c65 2e74 6f70 6f6c 6f67  ogy_file.topolog
-000017b0: 795f 6669 6c65 5f72 6561 6465 7294 7d94  y_file_reader.}.
-000017c0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-000017d0: 0068 1c4b 0068 1d4b 7168 1e4b 0075 8c30  .h.K.h.Kqh.K.u.0
-000017e0: 5051 416e 616c 7973 6973 2e69 6f2e 746f  PQAnalysis.io.to
-000017f0: 706f 6c6f 6779 5f66 696c 652e 746f 706f  pology_file.topo
-00001800: 6c6f 6779 5f66 696c 655f 7772 6974 6572  logy_file_writer
-00001810: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00001820: 681b 4b00 681c 4b00 681d 4b6b 681e 4b00  h.K.h.K.h.Kkh.K.
-00001830: 758c 2450 5141 6e61 6c79 7369 732e 696f  u.$PQAnalysis.io
-00001840: 2e74 6f70 6f6c 6f67 795f 6669 6c65 2e5f  .topology_file._
-00001850: 5f69 6e69 745f 5f94 7d94 2868 184b 0068  _init__.}.(h.K.h
-00001860: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
-00001870: 1d4b 0268 1e4b 0075 8c26 5051 416e 616c  .K.h.K.u.&PQAnal
-00001880: 7973 6973 2e69 6f2e 746f 706f 6c6f 6779  ysis.io.topology
-00001890: 5f66 696c 652e 6578 6365 7074 696f 6e73  _file.exceptions
-000018a0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-000018b0: 681b 4b00 681c 4b00 681d 4b02 681e 4b00  h.K.h.K.h.K.h.K.
-000018c0: 758c 1850 5141 6e61 6c79 7369 732e 696f  u..PQAnalysis.io
-000018d0: 2e76 6972 6961 6c2e 6170 6994 7d94 2868  .virial.api.}.(h
-000018e0: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-000018f0: 1c4b 0068 1d4b 0968 1e4b 0075 8c1d 5051  .K.h.K.h.K.u..PQ
-00001900: 416e 616c 7973 6973 2e69 6f2e 7669 7269  Analysis.io.viri
-00001910: 616c 2e5f 5f69 6e69 745f 5f94 7d94 2868  al.__init__.}.(h
-00001920: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-00001930: 1c4b 0068 1d4b 0168 1e4b 0075 8c22 5051  .K.h.K.h.K.u."PQ
-00001940: 416e 616c 7973 6973 2e69 6f2e 7669 7269  Analysis.io.viri
-00001950: 616c 2e76 6972 6961 6c5f 7265 6164 6572  al.virial_reader
-00001960: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00001970: 681b 4b00 681c 4b00 681d 4b14 681e 4b00  h.K.h.K.h.K.h.K.
-00001980: 758c 1d50 5141 6e61 6c79 7369 732e 636c  u..PQAnalysis.cl
-00001990: 692e 6275 696c 645f 6e65 705f 7472 616a  i.build_nep_traj
-000019a0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-000019b0: 681b 4b00 681c 4b00 681d 4b1f 681e 4b00  h.K.h.K.h.K.h.K.
-000019c0: 758c 1d50 5141 6e61 6c79 7369 732e 636c  u..PQAnalysis.cl
-000019d0: 692e 636f 6e74 696e 7565 5f69 6e70 7574  i.continue_input
-000019e0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-000019f0: 681b 4b00 681c 4b00 681d 4b1a 681e 4b00  h.K.h.K.h.K.h.K.
-00001a00: 758c 1650 5141 6e61 6c79 7369 732e 636c  u..PQAnalysis.cl
-00001a10: 692e 6765 6e32 7879 7a94 7d94 2868 184b  i.gen2xyz.}.(h.K
-00001a20: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-00001a30: 0068 1d4b 1b68 1e4b 0075 8c16 5051 416e  .h.K.h.K.u..PQAn
-00001a40: 616c 7973 6973 2e63 6c69 2e78 797a 3267  alysis.cli.xyz2g
-00001a50: 656e 947d 9428 6818 4b00 6819 4b00 681a  en.}.(h.K.h.K.h.
-00001a60: 4b00 681b 4b00 681c 4b00 681d 4b1b 681e  K.h.K.h.K.h.K.h.
-00001a70: 4b00 758c 1c50 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
-00001a80: 636c 692e 6164 645f 6d6f 6c65 6375 6c65  cli.add_molecule
-00001a90: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
-00001aa0: 0068 1b4b 0068 1c4b 0068 1d4b 2868 1e4b  .h.K.h.K.h.K(h.K
-00001ab0: 0075 8c19 5051 416e 616c 7973 6973 2e63  .u..PQAnalysis.c
-00001ac0: 6c69 2e74 7261 6a32 716d 6366 6394 7d94  li.traj2qmcfc.}.
-00001ad0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-00001ae0: 0068 1c4b 0068 1d4b 1968 1e4b 0075 8c18  .h.K.h.K.h.K.u..
-00001af0: 5051 416e 616c 7973 6973 2e63 6c69 2e5f  PQAnalysis.cli._
-00001b00: 636c 695f 6261 7365 947d 9428 6818 4b00  cli_base.}.(h.K.
-00001b10: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
-00001b20: 681d 4b05 681e 4b00 758c 1750 5141 6e61  h.K.h.K.u..PQAna
-00001b30: 6c79 7369 732e 636c 692e 5f5f 696e 6974  lysis.cli.__init
-00001b40: 5f5f 947d 9428 6818 4b00 6819 4b00 681a  __.}.(h.K.h.K.h.
-00001b50: 4b00 681b 4b00 681c 4b00 681d 4b02 681e  K.h.K.h.K.h.K.h.
-00001b60: 4b00 758c 1250 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
-00001b70: 636c 692e 7264 6694 7d94 2868 184b 0068  cli.rdf.}.(h.K.h
-00001b80: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
-00001b90: 1d4b 1f68 1e4b 0075 8c17 5051 416e 616c  .K.h.K.u..PQAnal
-00001ba0: 7973 6973 2e63 6c69 2e74 7261 6a32 626f  ysis.cli.traj2bo
-00001bb0: 7894 7d94 2868 184b 0068 194b 0068 1a4b  x.}.(h.K.h.K.h.K
-00001bc0: 0068 1b4b 0068 1c4b 0068 1d4b 1a68 1e4b  .h.K.h.K.h.K.h.K
-00001bd0: 0075 8c13 5051 416e 616c 7973 6973 2e63  .u..PQAnalysis.c
-00001be0: 6c69 2e6d 6169 6e94 7d94 2868 184b 0068  li.main.}.(h.K.h
-00001bf0: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
-00001c00: 1d4b 1c68 1e4b 0075 8c16 5051 416e 616c  .K.h.K.u..PQAnal
-00001c10: 7973 6973 2e63 6c69 2e72 7374 3278 797a  ysis.cli.rst2xyz
-00001c20: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00001c30: 681b 4b00 681c 4b00 681d 4b1b 681e 4b00  h.K.h.K.h.K.h.K.
-00001c40: 758c 1f50 5141 6e61 6c79 7369 732e 636c  u..PQAnalysis.cl
-00001c50: 692e 5f61 7267 756d 656e 745f 7061 7273  i._argument_pars
-00001c60: 6572 947d 9428 6818 4b00 6819 4b00 681a  er.}.(h.K.h.K.h.
-00001c70: 4b00 681b 4b00 681c 4b00 681d 4b31 681e  K.h.K.h.K.h.K1h.
-00001c80: 4b00 758c 1350 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
-00001c90: 7472 616a 2e61 7069 947d 9428 6818 4b00  traj.api.}.(h.K.
-00001ca0: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
-00001cb0: 681d 4b08 681e 4b00 758c 1850 5141 6e61  h.K.h.K.u..PQAna
-00001cc0: 6c79 7369 732e 7472 616a 2e5f 5f69 6e69  lysis.traj.__ini
-00001cd0: 745f 5f94 7d94 2868 184b 0068 194b 0068  t__.}.(h.K.h.K.h
-00001ce0: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0468  .K.h.K.h.K.h.K.h
-00001cf0: 1e4b 0075 8c1a 5051 416e 616c 7973 6973  .K.u..PQAnalysis
-00001d00: 2e74 7261 6a2e 7472 616a 6563 746f 7279  .traj.trajectory
-00001d10: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00001d20: 681b 4b00 681c 4b00 681d 4b61 681e 4b00  h.K.h.K.h.Kah.K.
-00001d30: 758c 1a50 5141 6e61 6c79 7369 732e 7472  u..PQAnalysis.tr
-00001d40: 616a 2e65 7863 6570 7469 6f6e 7394 7d94  aj.exceptions.}.
-00001d50: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-00001d60: 0068 1c4b 0068 1d4b 0768 1e4b 0075 8c17  .h.K.h.K.h.K.u..
-00001d70: 5051 416e 616c 7973 6973 2e74 7261 6a2e  PQAnalysis.traj.
-00001d80: 666f 726d 6174 7394 7d94 2868 184b 0068  formats.}.(h.K.h
-00001d90: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0168  .K.h.K.h.K.h.K.h
-00001da0: 1d4b 2d68 1e4b 0075 8c17 5051 416e 616c  .K-h.K.u..PQAnal
-00001db0: 7973 6973 2e75 7469 6c73 2e72 616e 646f  ysis.utils.rando
-00001dc0: 6d94 7d94 2868 184b 0068 194b 0068 1a4b  m.}.(h.K.h.K.h.K
-00001dd0: 0068 1b4b 0068 1c4b 0068 1d4b 0668 1e4b  .h.K.h.K.h.K.h.K
-00001de0: 0075 8c1b 5051 416e 616c 7973 6973 2e75  .u..PQAnalysis.u
-00001df0: 7469 6c73 2e64 6563 6f72 6174 6f72 7394  tils.decorators.
-00001e00: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00001e10: 1b4b 0068 1c4b 0068 1d4b 2068 1e4b 0075  .K.h.K.h.K h.K.u
-00001e20: 8c17 5051 416e 616c 7973 6973 2e75 7469  ..PQAnalysis.uti
-00001e30: 6c73 2e63 6f6d 6d6f 6e94 7d94 2868 184b  ls.common.}.(h.K
-00001e40: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-00001e50: 0068 1d4b 0968 1e4b 0075 8c1f 5051 416e  .h.K.h.K.u..PQAn
-00001e60: 616c 7973 6973 2e75 7469 6c73 2e63 7573  alysis.utils.cus
-00001e70: 746f 6d5f 6c6f 6767 696e 6794 7d94 2868  tom_logging.}.(h
-00001e80: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-00001e90: 1c4b 0068 1d4b 6568 1e4b 0075 8c19 5051  .K.h.Keh.K.u..PQ
-00001ea0: 416e 616c 7973 6973 2e75 7469 6c73 2e5f  Analysis.utils._
-00001eb0: 5f69 6e69 745f 5f94 7d94 2868 184b 0068  _init__.}.(h.K.h
-00001ec0: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
-00001ed0: 1d4b 0268 1e4b 0075 8c16 5051 416e 616c  .K.h.K.u..PQAnal
-00001ee0: 7973 6973 2e75 7469 6c73 2e66 696c 6573  ysis.utils.files
-00001ef0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00001f00: 681b 4b00 681c 4b00 681d 4b0a 681e 4b00  h.K.h.K.h.K.h.K.
-00001f10: 758c 1650 5141 6e61 6c79 7369 732e 7574  u..PQAnalysis.ut
-00001f20: 696c 732e 756e 6974 7394 7d94 2868 184b  ils.units.}.(h.K
-00001f30: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-00001f40: 0068 1d4b 0768 1e4b 0075 8c13 5051 416e  .h.K.h.K.u..PQAn
-00001f50: 616c 7973 6973 2e63 6f72 652e 6170 6994  alysis.core.api.
-00001f60: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00001f70: 1b4b 0068 1c4b 0068 1d4b 0968 1e4b 0175  .K.h.K.h.K.h.K.u
-00001f80: 8c17 5051 416e 616c 7973 6973 2e63 6f72  ..PQAnalysis.cor
-00001f90: 652e 7265 7369 6475 6594 7d94 2868 184b  e.residue.}.(h.K
-00001fa0: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-00001fb0: 0268 1d4b 5068 1e4b 0075 8c18 5051 416e  .h.KPh.K.u..PQAn
-00001fc0: 616c 7973 6973 2e63 6f72 652e 5f5f 696e  alysis.core.__in
-00001fd0: 6974 5f5f 947d 9428 6818 4b00 6819 4b00  it__.}.(h.K.h.K.
-00001fe0: 681a 4b00 681b 4b00 681c 4b00 681d 4b05  h.K.h.K.h.K.h.K.
-00001ff0: 681e 4b00 758c 1a50 5141 6e61 6c79 7369  h.K.u..PQAnalysi
-00002000: 732e 636f 7265 2e65 7863 6570 7469 6f6e  s.core.exception
-00002010: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
-00002020: 0068 1b4b 0068 1c4b 0068 1d4b 1068 1e4b  .h.K.h.K.h.K.h.K
-00002030: 0075 8c29 5051 416e 616c 7973 6973 2e63  .u.)PQAnalysis.c
-00002040: 6f72 652e 6365 6c6c 2e5f 7374 616e 6461  ore.cell._standa
-00002050: 7264 5f70 726f 7065 7274 6965 7394 7d94  rd_properties.}.
-00002060: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-00002070: 0068 1c4b 0068 1d4b 2468 1e4b 0075 8c1d  .h.K.h.K$h.K.u..
-00002080: 5051 416e 616c 7973 6973 2e63 6f72 652e  PQAnalysis.core.
-00002090: 6365 6c6c 2e5f 5f69 6e69 745f 5f94 7d94  cell.__init__.}.
-000020a0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-000020b0: 0068 1c4b 0068 1d4b 0168 1e4b 0075 8c19  .h.K.h.K.h.K.u..
-000020c0: 5051 416e 616c 7973 6973 2e63 6f72 652e  PQAnalysis.core.
-000020d0: 6365 6c6c 2e63 656c 6c94 7d94 2868 184b  cell.cell.}.(h.K
-000020e0: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-000020f0: 0168 1d4b 5168 1e4b 0075 8c1d 5051 416e  .h.KQh.K.u..PQAn
-00002100: 616c 7973 6973 2e63 6f72 652e 6174 6f6d  alysis.core.atom
-00002110: 2e5f 5f69 6e69 745f 5f94 7d94 2868 184b  .__init__.}.(h.K
-00002120: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-00002130: 0068 1d4b 0268 1e4b 0075 8c19 5051 416e  .h.K.h.K.u..PQAn
-00002140: 616c 7973 6973 2e63 6f72 652e 6174 6f6d  alysis.core.atom
-00002150: 2e61 746f 6d94 7d94 2868 184b 0068 194b  .atom.}.(h.K.h.K
-00002160: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
-00002170: 3268 1e4b 0075 8c1c 5051 416e 616c 7973  2h.K.u..PQAnalys
-00002180: 6973 2e63 6f72 652e 6174 6f6d 2e65 6c65  is.core.atom.ele
-00002190: 6d65 6e74 947d 9428 6818 4b00 6819 4b00  ment.}.(h.K.h.K.
-000021a0: 681a 4b00 681b 4b00 681c 4b00 681d 4b2d  h.K.h.K.h.K.h.K-
-000021b0: 681e 4b00 758c 2150 5141 6e61 6c79 7369  h.K.u.!PQAnalysi
-000021c0: 732e 7068 7973 6963 616c 5f64 6174 612e  s.physical_data.
-000021d0: 5f5f 696e 6974 5f5f 947d 9428 6818 4b00  __init__.}.(h.K.
-000021e0: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
-000021f0: 681d 4b02 681e 4b00 758c 2350 5141 6e61  h.K.h.K.u.#PQAna
-00002200: 6c79 7369 732e 7068 7973 6963 616c 5f64  lysis.physical_d
-00002210: 6174 612e 6578 6365 7074 696f 6e73 947d  ata.exceptions.}
-00002220: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-00002230: 4b00 681c 4b00 681d 4b05 681e 4b00 758c  K.h.K.h.K.h.K.u.
-00002240: 1f50 5141 6e61 6c79 7369 732e 7068 7973  .PQAnalysis.phys
-00002250: 6963 616c 5f64 6174 612e 656e 6572 6779  ical_data.energy
-00002260: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00002270: 681b 4b00 681c 4b03 681d 4b3e 681e 4b00  h.K.h.K.h.K>h.K.
-00002280: 7575 8c06 6279 5f6d 7367 947d 9428 8c05  uu..by_msg.}.(..
-00002290: 6669 786d 6594 4b0b 8c1c 746f 6f2d 6d61  fixme.K...too-ma
-000022a0: 6e79 2d69 6e73 7461 6e63 652d 6174 7472  ny-instance-attr
-000022b0: 6962 7574 6573 944b 0a8c 1274 6f6f 2d6d  ibutes.K...too-m
-000022c0: 616e 792d 6172 6775 6d65 6e74 7394 4b12  any-arguments.K.
-000022d0: 8c1e 696e 636f 6e73 6973 7465 6e74 2d72  ..inconsistent-r
-000022e0: 6574 7572 6e2d 7374 6174 656d 656e 7473  eturn-statements
-000022f0: 944b 098c 1174 7261 696c 696e 672d 6e65  .K...trailing-ne
-00002300: 776c 696e 6573 944b 018c 0f74 6f6f 2d6d  wlines.K...too-m
-00002310: 616e 792d 6c6f 6361 6c73 944b 038c 1774  any-locals.K...t
-00002320: 6f6f 2d6d 616e 792d 7075 626c 6963 2d6d  oo-many-public-m
-00002330: 6574 686f 6473 944b 018c 1a74 6f6f 2d6d  ethods.K...too-m
-00002340: 616e 792d 7265 7475 726e 2d73 7461 7465  any-return-state
-00002350: 6d65 6e74 7394 4b01 8c0b 746f 6f2d 636f  ments.K...too-co
-00002360: 6d70 6c65 7894 4b03 8c11 746f 6f2d 6d61  mplex.K...too-ma
-00002370: 6e79 2d62 7261 6e63 6865 7394 4b02 8c0e  ny-branches.K...
-00002380: 746f 6f2d 6d61 6e79 2d6c 696e 6573 944b  too-many-lines.K
-00002390: 018c 1374 6f6f 2d6d 616e 792d 7374 6174  ...too-many-stat
-000023a0: 656d 656e 7473 944b 018c 0f75 6e75 7365  ements.K...unuse
-000023b0: 642d 6172 6775 6d65 6e74 944b 018c 0e64  d-argument.K...d
-000023c0: 7570 6c69 6361 7465 2d63 6f64 6594 4b03  uplicate-code.K.
-000023d0: 758c 0f63 6f64 655f 7479 7065 5f63 6f75  u..code_type_cou
-000023e0: 6e74 947d 9428 8c04 636f 6465 944d c01d  nt.}.(..code.M..
-000023f0: 8c07 636f 6d6d 656e 7494 4d05 018c 0964  ..comment.M....d
-00002400: 6f63 7374 7269 6e67 944d e720 8c05 656d  ocstring.M. ..em
-00002410: 7074 7994 4df0 0a8c 0574 6f74 616c 944d  pty.M....total.M
-00002420: 9c4a 758c 0c64 6570 656e 6465 6e63 6965  .Ju..dependencie
-00002430: 7394 7d94 288c 0d62 6561 7274 7970 652e  s.}.(..beartype.
-00002440: 636c 6177 948f 9428 6823 908c 1150 5141  claw...(h#...PQA
-00002450: 6e61 6c79 7369 732e 636f 6e66 6967 948f  nalysis.config..
-00002460: 9428 68e3 68d3 68df 6865 68f9 68cf 68e7  .(h.h.h.heh.h.h.
-00002470: 68af 68d1 68a5 68e1 68d9 68e5 6823 68d7  h.h.h.h.h.h.h#h.
-00002480: 68d5 908c 1f50 5141 6e61 6c79 7369 732e  h....PQAnalysis.
-00002490: 7574 696c 732e 6375 7374 6f6d 5f6c 6f67  utils.custom_log
-000024a0: 6769 6e67 948f 9428 8c12 5051 416e 616c  ging...(..PQAnal
-000024b0: 7973 6973 2e69 6f2e 6261 7365 946a 1101  ysis.io.base.j..
-000024c0: 0000 8c24 5051 416e 616c 7973 6973 2e69  ...$PQAnalysis.i
-000024d0: 6f2e 7472 616a 5f66 696c 652e 6672 616d  o.traj_file.fram
-000024e0: 655f 7265 6164 6572 948c 4850 5141 6e61  e_reader..HPQAna
-000024f0: 6c79 7369 732e 696f 2e69 6e70 7574 5f66  lysis.io.input_f
-00002500: 696c 655f 7265 6164 6572 2e70 715f 616e  ile_reader.pq_an
-00002510: 616c 7973 6973 2e70 7161 6e61 6c79 7369  alysis.pqanalysi
-00002520: 735f 696e 7075 745f 6669 6c65 5f72 6561  s_input_file_rea
-00002530: 6465 7294 68a1 6869 6871 8c26 5051 416e  der.h.hihq.&PQAn
-00002540: 616c 7973 6973 2e69 6f2e 6765 6e5f 6669  alysis.io.gen_fi
-00002550: 6c65 2e67 656e 5f66 696c 655f 7265 6164  le.gen_file_read
-00002560: 6572 9468 8768 3b68 c18c 2950 5141 6e61  er.h.h;h..)PQAna
-00002570: 6c79 7369 732e 696f 2e72 6573 7461 7274  lysis.io.restart
-00002580: 5f66 696c 652e 7265 7374 6172 745f 7265  _file.restart_re
-00002590: 6164 6572 9468 7768 856a 1901 0000 68a5  ader.hwh.j....h.
-000025a0: 6847 6a13 0100 006a 0301 0000 68f1 6875  hGj....j....h.hu
-000025b0: 6853 68af 6833 6895 6823 6861 687d 6831  hSh.h3h.h#hah}h1
-000025c0: 6865 6825 68bb 68ed 686f 686d 68c3 908c  heh%h.h.hohmh...
-000025d0: 0964 6563 6f72 6174 6f72 948f 9428 8c24  .decorator...(.$
-000025e0: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
-000025f0: 635f 7379 7374 656d 2e5f 6465 636f 7261  c_system._decora
-00002600: 746f 7273 9468 2568 f590 8c0d 6265 6172  tors.h%h....bear
-00002610: 7479 7065 2e64 6f6f 7294 8f94 2868 2590  type.door...(h%.
-00002620: 8c0f 6265 6172 7479 7065 2e74 7970 696e  ..beartype.typin
-00002630: 6794 8f94 286a 3a01 0000 6a11 0100 0068  g...(j:...j....h
-00002640: a368 e76a 3b01 0000 6a3c 0100 0068 a16a  .h.j;...j<...h.j
-00002650: 3d01 0000 68c1 6829 683b 6887 6879 68c9  =...h.h)h;h.hyh.
-00002660: 6a3e 0100 0068 7768 8568 ed8c 1a50 5141  j>...hwh.h...PQA
-00002670: 6e61 6c79 7369 732e 636f 7265 2e65 7863  nalysis.core.exc
-00002680: 6570 7469 6f6e 7394 6a19 0100 0068 a968  eptions.j....h.h
-00002690: a568 476a 1301 0000 6a03 0100 0068 f168  .hGj....j....h.h
-000026a0: 5f68 3768 758c 3750 5141 6e61 6c79 7369  _h7hu.7PQAnalysi
-000026b0: 732e 696f 2e69 6e70 7574 5f66 696c 655f  s.io.input_file_
-000026c0: 7265 6164 6572 2e70 715f 616e 616c 7973  reader.pq_analys
-000026d0: 6973 2e5f 6669 6c65 5f6d 6978 696e 9468  is._file_mixin.h
-000026e0: 8368 5368 2f68 af68 f568 3368 4f68 5168  .hSh/h.h.h3hOhQh
-000026f0: 7d68 318c 3850 5141 6e61 6c79 7369 732e  }h1.8PQAnalysis.
-00002700: 746f 706f 6c6f 6779 2e62 6f6e 6465 645f  topology.bonded_
-00002710: 746f 706f 6c6f 6779 2e5f 746f 706f 6c6f  topology._topolo
-00002720: 6779 5f70 726f 7065 7274 6965 7394 68f9  gy_properties.h.
-00002730: 6865 6825 682d 68fd 6a41 0100 0068 6f68  heh%h-h.jA...hoh
-00002740: c36a 0d01 0000 908c 1550 5141 6e61 6c79  .j.......PQAnaly
-00002750: 7369 732e 6578 6365 7074 696f 6e73 948f  sis.exceptions..
-00002760: 9428 6a3a 0100 0068 6968 7168 8768 3b68  .(j:...hihqh.h;h
-00002770: 856a 4601 0000 68bd 8c23 5051 416e 616c  .jF...h..#PQAnal
-00002780: 7973 6973 2e61 746f 6d69 635f 7379 7374  ysis.atomic_syst
-00002790: 656d 2e65 7863 6570 7469 6f6e 7394 68a5  em.exceptions.h.
-000027a0: 6847 8c22 5051 416e 616c 7973 6973 2e61  hG."PQAnalysis.a
-000027b0: 6e61 6c79 7369 732e 7264 662e 6578 6365  nalysis.rdf.exce
-000027c0: 7074 696f 6e73 9468 9f68 7568 7b68 ef68  ptions.h.huh{h.h
-000027d0: b368 3368 9568 c768 3968 8168 ab68 9368  .h3h.h.h9h.h.h.h
-000027e0: f968 2568 bb68 ed6a 1701 0000 908c 1050  .h%h.h.j.......P
-000027f0: 5141 6e61 6c79 7369 732e 7479 7065 7394  QAnalysis.types.
-00002800: 8f94 286a 3b01 0000 684d 6869 68a1 6a3d  ..(j;...hMhih.j=
-00002810: 0100 0068 8768 3b68 cd68 8568 ed6a 1901  ...h.h;h.h.h.j..
-00002820: 0000 68a9 6a01 0100 0068 476a 0301 0000  ..h.j....hGj....
-00002830: 685f 6837 6843 6853 8c3c 5051 416e 616c  h_h7hChS.<PQAnal
-00002840: 7973 6973 2e69 6f2e 696e 7075 745f 6669  ysis.io.input_fi
-00002850: 6c65 5f72 6561 6465 722e 7071 5f61 6e61  le_reader.pq_ana
-00002860: 6c79 7369 732e 5f70 6f73 6974 696f 6e73  lysis._positions
-00002870: 5f6d 6978 696e 9468 2f68 af68 3368 4f68  _mixin.h/h.h3hOh
-00002880: 9568 456a 0901 0000 6831 6a48 0100 0068  .hEj....h1jH...h
-00002890: 6568 2568 4168 516a 0d01 0000 908c 056e  eh%hAhQj.......n
-000028a0: 756d 7079 948f 9428 6a3b 0100 0068 a16a  umpy...(j;...h.j
-000028b0: 3d01 0000 6871 6829 6a3e 0100 0068 cd68  =...hqh)j>...h.h
-000028c0: ed6a 1901 0000 6a01 0100 0068 476a 0301  .j....j....hGj..
-000028d0: 0000 6837 6853 68af 6833 684f 6a09 0100  ..h7hSh.h3hOj...
-000028e0: 0068 5168 3168 6568 fd68 bb6a 4101 0000  .hQh1heh.h.jA...
-000028f0: 686f 6a0d 0100 0090 8c0d 6265 6172 7479  hoj.......bearty
-00002900: 7065 2e76 616c 6594 8f94 286a 1301 0000  pe.vale...(j....
-00002910: 6829 6a0d 0100 0090 8c0b 6d75 6c74 696d  h)j.......multim
-00002920: 6574 686f 6494 8f94 2868 2b90 8c0f 5051  ethod...(h+...PQ
-00002930: 416e 616c 7973 6973 2e74 7261 6a94 8f94  Analysis.traj...
-00002940: 2868 a368 e76a 3b01 0000 68a1 6871 6879  (h.h.j;...h.hqhy
-00002950: 6a3e 0100 0068 7768 4b68 a968 a568 4768  j>...hwhKh.h.hGh
-00002960: 3768 7568 2f68 af8c 1e50 5141 6e61 6c79  7huh/h...PQAnaly
-00002970: 7369 732e 696f 2e72 6573 7461 7274 5f66  sis.io.restart_f
-00002980: 696c 652e 6170 6994 685d 6865 686d 908c  ile.api.h]hehm..
-00002990: 0d50 5141 6e61 6c79 7369 732e 696f 948f  .PQAnalysis.io..
-000029a0: 9428 685d 68d3 6865 68cd 682f 68af 68d1  .(h]h.heh.h/h.h.
-000029b0: 68e1 6847 68d9 68e5 6861 685f 6837 68d5  h.hGh.h.hah_h7h.
-000029c0: 908c 1850 5141 6e61 6c79 7369 732e 7479  ...PQAnalysis.ty
-000029d0: 7065 5f63 6865 636b 696e 6794 8f94 286a  pe_checking...(j
-000029e0: 1101 0000 68a3 686f 684d 6869 6871 68a1  ....h.hohMhihqh.
-000029f0: 6a3d 0100 0068 3b68 c168 7968 c96a 3e01  j=...h;h.hyh.j>.
-00002a00: 0000 68cd 6877 68ed 6a19 0100 0068 4b68  ..h.hwh.j....hKh
-00002a10: a96a 0101 0000 68a5 6847 6a13 0100 006a  .j....h.hGj....j
-00002a20: 0301 0000 68e9 8c1a 5051 416e 616c 7973  ....h...PQAnalys
-00002a30: 6973 2e69 6f2e 6765 6e5f 6669 6c65 2e61  is.io.gen_file.a
-00002a40: 7069 9468 5f68 3768 7568 4368 5368 2f68  pi.h_h7huhChSh/h
-00002a50: af68 336a 5801 0000 6845 6a09 0100 0068  .h3jX...hEj....h
-00002a60: 3168 5d68 6568 bf68 4168 bb68 5168 6168  1h]heh.hAh.hQhah
-00002a70: 6d68 c36a 0d01 0000 908c 1d50 5141 6e61  mh.j.......PQAna
-00002a80: 6c79 7369 732e 746f 706f 6c6f 6779 2e73  lysis.topology.s
-00002a90: 656c 6563 7469 6f6e 948f 9428 682f 6837  election...(h/h7
-00002aa0: 8c13 5051 416e 616c 7973 6973 2e74 6f70  ..PQAnalysis.top
-00002ab0: 6f6c 6f67 7994 908c 2250 5141 6e61 6c79  ology..."PQAnaly
-00002ac0: 7369 732e 746f 706f 6c6f 6779 2e73 6861  sis.topology.sha
-00002ad0: 6b65 5f74 6f70 6f6c 6f67 7994 8f94 2868  ke_topology...(h
-00002ae0: 2f90 8c1a 5051 416e 616c 7973 6973 2e63  /...PQAnalysis.c
-00002af0: 6f72 652e 6578 6365 7074 696f 6e73 948f  ore.exceptions..
-00002b00: 9428 6a11 0100 008c 0f50 5141 6e61 6c79  .(j......PQAnaly
-00002b10: 7369 732e 636f 7265 946a 1301 0000 6a03  sis.core.j....j.
-00002b20: 0100 0068 3190 8c0f 5051 416e 616c 7973  ...h1...PQAnalys
-00002b30: 6973 2e63 6f72 6594 8f94 2868 a968 5368  is.core...(h.hSh
-00002b40: 656a 3b01 0000 68a5 684d 68a1 6a3d 0100  ej;...h.hMh.j=..
-00002b50: 0068 3368 4f68 e96a 5801 0000 6879 6851  .h3hOh.jX...hyhQ
-00002b60: 6a3e 0100 0068 6f68 ed68 3190 8c0a 5051  j>...hoh.h1...PQ
-00002b70: 416e 616c 7973 6973 948f 9428 6a3a 0100  Analysis...(j:..
-00002b80: 006a 1101 0000 6a3b 0100 006a 3c01 0000  .j....j;...j<...
-00002b90: 68a1 6869 6871 6a3d 0100 0068 8768 3b68  h.hihqj=...h.h;h
-00002ba0: c16a 3e01 0000 6877 6885 6a19 0100 0068  .j>...hwh.j....h
-00002bb0: a568 476a 1301 0000 6a03 0100 0068 f168  .hGj....j....h.h
-00002bc0: 7568 5368 af68 3368 9568 6168 7d68 3168  uhSh.h3h.hah}h1h
-00002bd0: 6568 bb68 ed68 6f68 6d68 c390 8c1e 5051  eh.h.hohmh....PQ
-00002be0: 416e 616c 7973 6973 2e74 6f70 6f6c 6f67  Analysis.topolog
-00002bf0: 792e 6578 6365 7074 696f 6e73 948f 9428  y.exceptions...(
-00002c00: 6a60 0100 0068 3190 8c33 5051 416e 616c  j`...h1..3PQAnal
-00002c10: 7973 6973 2e74 6f70 6f6c 6f67 792e 626f  ysis.topology.bo
-00002c20: 6e64 6564 5f74 6f70 6f6c 6f67 792e 626f  nded_topology.bo
-00002c30: 6e64 6564 5f74 6f70 6f6c 6f67 7994 8f94  nded_topology...
-00002c40: 286a 6001 0000 6831 908c 046c 6172 6b94  (j`...h1...lark.
-00002c50: 8f94 2868 3368 8590 8c1c 5051 416e 616c  ..(h3h....PQAnal
-00002c60: 7973 6973 2e74 6f70 6f6c 6f67 792e 746f  ysis.topology.to
-00002c70: 706f 6c6f 6779 948f 9428 6833 6a60 0100  pology...(h3j`..
-00002c80: 0090 8c28 5051 416e 616c 7973 6973 2e74  ...(PQAnalysis.t
-00002c90: 6f70 6f6c 6f67 792e 626f 6e64 6564 5f74  opology.bonded_t
-00002ca0: 6f70 6f6c 6f67 792e 626f 6e64 948f 9428  opology.bond...(
-00002cb0: 6a48 0100 0068 3b6a 6001 0000 908c 2950  jH...h;j`.....)P
-00002cc0: 5141 6e61 6c79 7369 732e 746f 706f 6c6f  QAnalysis.topolo
-00002cd0: 6779 2e62 6f6e 6465 645f 746f 706f 6c6f  gy.bonded_topolo
-00002ce0: 6779 2e61 6e67 6c65 948f 9428 6a48 0100  gy.angle...(jH..
-00002cf0: 0068 3b6a 6001 0000 908c 2c50 5141 6e61  .h;j`.....,PQAna
-00002d00: 6c79 7369 732e 746f 706f 6c6f 6779 2e62  lysis.topology.b
-00002d10: 6f6e 6465 645f 746f 706f 6c6f 6779 2e64  onded_topology.d
-00002d20: 6968 6564 7261 6c94 8f94 286a 4801 0000  ihedral...(jH...
-00002d30: 683b 6a60 0100 0090 8c38 5051 416e 616c  h;j`.....8PQAnal
-00002d40: 7973 6973 2e74 6f70 6f6c 6f67 792e 626f  ysis.topology.bo
-00002d50: 6e64 6564 5f74 6f70 6f6c 6f67 792e 5f74  nded_topology._t
-00002d60: 6f70 6f6c 6f67 795f 7072 6f70 6572 7469  opology_properti
-00002d70: 6573 948f 9428 683b 908c 1550 5141 6e61  es...(h;...PQAna
-00002d80: 6c79 7369 732e 696f 2e66 6f72 6d61 7473  lysis.io.formats
-00002d90: 948f 9428 6a3a 0100 0068 a968 a38c 0d50  ...(j:...h.h...P
-00002da0: 5141 6e61 6c79 7369 732e 696f 9468 bf68  QAnalysis.io.h.h
-00002db0: e768 4768 a168 d76a 5d01 0000 68bb 6879  .hGh.h.j]...h.hy
-00002dc0: 686d 68c3 6875 908c 1850 5141 6e61 6c79  hmh.hu...PQAnaly
-00002dd0: 7369 732e 6174 6f6d 6963 5f73 7973 7465  sis.atomic_syste
-00002de0: 6d94 8f94 2868 a968 a36a 3b01 0000 68af  m...(h.h.j;...h.
-00002df0: 68a5 6847 68a1 6a3d 0100 006a 5801 0000  h.hGh.j=...jX...
-00002e00: 6a5d 0100 0068 bb68 ed6a 3e01 0000 6875  j]...h.h.j>...hu
-00002e10: 908c 2150 5141 6e61 6c79 7369 732e 746f  ..!PQAnalysis.to
-00002e20: 6f6c 732e 7472 616a 5f74 6f5f 636f 6d5f  ols.traj_to_com_
-00002e30: 7472 616a 948f 9428 8c10 5051 416e 616c  traj...(..PQAnal
-00002e40: 7973 6973 2e74 6f6f 6c73 9490 8c13 5051  ysis.tools....PQ
-00002e50: 416e 616c 7973 6973 2e74 6f70 6f6c 6f67  Analysis.topolog
-00002e60: 7994 8f94 2868 5d68 5368 6568 a368 bf6a  y...(h]hSheh.h.j
-00002e70: 3b01 0000 68a5 68ed 684d 68c1 6851 6a3e  ;...h.h.hMh.hQj>
-00002e80: 0100 0068 c390 8c24 5051 416e 616c 7973  ...h...$PQAnalys
-00002e90: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
-00002ea0: 2e5f 6465 636f 7261 746f 7273 948f 9428  ._decorators...(
-00002eb0: 684d 6851 684f 908c 2350 5141 6e61 6c79  hMhQhO..#PQAnaly
-00002ec0: 7369 732e 6174 6f6d 6963 5f73 7973 7465  sis.atomic_syste
-00002ed0: 6d2e 6578 6365 7074 696f 6e73 948f 9428  m.exceptions...(
-00002ee0: 6a41 0100 0068 4f68 538c 1850 5141 6e61  jA...hOhS..PQAna
-00002ef0: 6c79 7369 732e 6174 6f6d 6963 5f73 7973  lysis.atomic_sys
-00002f00: 7465 6d94 908c 1773 6369 7079 2e73 7061  tem....scipy.spa
-00002f10: 7469 616c 2e74 7261 6e73 666f 726d 948f  tial.transform..
-00002f20: 9428 6853 908c 1750 5141 6e61 6c79 7369  .(hS...PQAnalysi
-00002f30: 732e 7574 696c 732e 7261 6e64 6f6d 948f  s.utils.random..
-00002f40: 9428 68af 6853 908c 2450 5141 6e61 6c79  .(h.hS..$PQAnaly
-00002f50: 7369 732e 6174 6f6d 6963 5f73 7973 7465  sis.atomic_syste
-00002f60: 6d2e 5f70 726f 7065 7274 6965 7394 8f94  m._properties...
-00002f70: 2868 5390 8c2d 5051 416e 616c 7973 6973  (hS..-PQAnalysis
-00002f80: 2e61 746f 6d69 635f 7379 7374 656d 2e5f  .atomic_system._
-00002f90: 7374 616e 6461 7264 5f70 726f 7065 7274  standard_propert
-00002fa0: 6965 7394 8f94 2868 5390 8c23 5051 416e  ies...(hS..#PQAn
-00002fb0: 616c 7973 6973 2e61 746f 6d69 635f 7379  alysis.atomic_sy
-00002fc0: 7374 656d 2e5f 706f 7369 7469 6f6e 7394  stem._positions.
-00002fd0: 8f94 2868 5390 8c26 5051 416e 616c 7973  ..(hS..&PQAnalys
-00002fe0: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
-00002ff0: 2e61 746f 6d69 635f 7379 7374 656d 948f  .atomic_system..
-00003000: 9428 6a88 0100 0090 8c17 5051 416e 616c  .(j.......PQAnal
-00003010: 7973 6973 2e61 6e61 6c79 7369 732e 7264  ysis.analysis.rd
-00003020: 6694 8f94 288c 1350 5141 6e61 6c79 7369  f...(..PQAnalysi
-00003030: 732e 616e 616c 7973 6973 9490 8c1b 5051  s.analysis....PQ
-00003040: 416e 616c 7973 6973 2e61 6e61 6c79 7369  Analysis.analysi
-00003050: 732e 7264 662e 7264 6694 8f94 2868 5d68  s.rdf.rdf...(h]h
-00003060: df68 5f8c 1750 5141 6e61 6c79 7369 732e  .h_..PQAnalysis.
-00003070: 616e 616c 7973 6973 2e72 6466 946a 9701  analysis.rdf.j..
-00003080: 0000 908c 2d50 5141 6e61 6c79 7369 732e  ....-PQAnalysis.
-00003090: 616e 616c 7973 6973 2e72 6466 2e72 6466  analysis.rdf.rdf
-000030a0: 5f69 6e70 7574 5f66 696c 655f 7265 6164  _input_file_read
-000030b0: 6572 948f 9428 685d 6a9a 0100 0068 df90  er...(h]j....h..
-000030c0: 8c2e 5051 416e 616c 7973 6973 2e61 6e61  ..PQAnalysis.ana
-000030d0: 6c79 7369 732e 7264 662e 7264 665f 6f75  lysis.rdf.rdf_ou
-000030e0: 7470 7574 5f66 696c 655f 7772 6974 6572  tput_file_writer
-000030f0: 948f 9428 685d 6a9a 0100 0090 8c10 5051  ...(h]j.......PQ
-00003100: 416e 616c 7973 6973 2e75 7469 6c73 948f  Analysis.utils..
-00003110: 9428 68f9 6865 685f 686d 8c0e 5051 416e  .(h.heh_hm..PQAn
-00003120: 616c 7973 6973 2e63 6c69 9490 8c2a 5051  alysis.cli...*PQ
-00003130: 416e 616c 7973 6973 2e69 6f2e 696e 7075  Analysis.io.inpu
-00003140: 745f 6669 6c65 5f72 6561 6465 722e 6578  t_file_reader.ex
-00003150: 6365 7074 696f 6e73 948f 9428 6887 6861  ceptions...(h.ha
-00003160: 6883 6a3c 0100 0090 8c1b 5051 416e 616c  h.j<......PQAnal
-00003170: 7973 6973 2e61 6e61 6c79 7369 732e 7264  ysis.analysis.rd
-00003180: 662e 6170 6994 8f94 286a 9a01 0000 906a  f.api...(j.....j
-00003190: 4c01 0000 8f94 286a 9a01 0000 6865 908c  L.....(j....he..
-000031a0: 0974 7164 6d2e 6175 746f 948f 9428 68a5  .tqdm.auto...(h.
-000031b0: 6865 908c 1f50 5141 6e61 6c79 7369 732e  he...PQAnalysis.
-000031c0: 696f 2e69 6e70 7574 5f66 696c 655f 7265  io.input_file_re
-000031d0: 6164 6572 948f 9428 6869 6a7c 0100 0090  ader...(hij|....
-000031e0: 8c27 5051 416e 616c 7973 6973 2e69 6f2e  .'PQAnalysis.io.
-000031f0: 696e 7075 745f 6669 6c65 5f72 6561 6465  input_file_reade
-00003200: 722e 666f 726d 6174 7394 8f94 286a 3c01  r.formats...(j<.
-00003210: 0000 8c1f 5051 416e 616c 7973 6973 2e69  ....PQAnalysis.i
-00003220: 6f2e 696e 7075 745f 6669 6c65 5f72 6561  o.input_file_rea
-00003230: 6465 7294 6869 6895 6885 908c 1850 5141  der.hih.h....PQA
-00003240: 6e61 6c79 7369 732e 696f 2e65 7863 6570  nalysis.io.excep
-00003250: 7469 6f6e 7394 8f94 2868 6f68 6d6a 3a01  tions...(hohmj:.
-00003260: 0000 687d 908c 1250 5141 6e61 6c79 7369  ..h}...PQAnalysi
-00003270: 732e 696f 2e62 6173 6594 8f94 2868 a968  s.io.base...(h.h
-00003280: 8568 a568 a16a 3d01 0000 6871 68c1 68c3  .h.h.j=...hqh.h.
-00003290: 68bb 6a3e 0100 0068 6f68 6d68 776a 7c01  h.j>...hohmhwj|.
-000032a0: 0000 908c 1850 5141 6e61 6c79 7369 732e  .....PQAnalysis.
-000032b0: 7068 7973 6963 616c 5f64 6174 6194 8f94  physical_data...
-000032c0: 2868 7190 8c1e 5051 416e 616c 7973 6973  (hq...PQAnalysis
-000032d0: 2e69 6f2e 696e 666f 5f66 696c 655f 7265  .io.info_file_re
-000032e0: 6164 6572 948f 9428 6871 6a7c 0100 0090  ader...(hqj|....
-000032f0: 8c22 5051 416e 616c 7973 6973 2e69 6f2e  ."PQAnalysis.io.
-00003300: 6d6f 6c64 6573 6372 6970 746f 725f 7265  moldescriptor_re
-00003310: 6164 6572 948f 9428 6a3e 0100 006a 7c01  ader...(j>...j|.
-00003320: 0000 908c 2950 5141 6e61 6c79 7369 732e  ....)PQAnalysis.
-00003330: 696f 2e72 6573 7461 7274 5f66 696c 652e  io.restart_file.
-00003340: 7265 7374 6172 745f 7772 6974 6572 948f  restart_writer..
-00003350: 9428 8c1a 5051 416e 616c 7973 6973 2e69  .(..PQAnalysis.i
-00003360: 6f2e 7265 7374 6172 745f 6669 6c65 946a  o.restart_file.j
-00003370: 7c01 0000 908c 2950 5141 6e61 6c79 7369  |.....)PQAnalysi
-00003380: 732e 696f 2e72 6573 7461 7274 5f66 696c  s.io.restart_fil
-00003390: 652e 7265 7374 6172 745f 7265 6164 6572  e.restart_reader
-000033a0: 948f 9428 6aba 0100 006a 5801 0000 6a7c  ...(j....jX...j|
-000033b0: 0100 0090 8c1e 5051 416e 616c 7973 6973  ......PQAnalysis
-000033c0: 2e69 6f2e 7265 7374 6172 745f 6669 6c65  .io.restart_file
-000033d0: 2e61 7069 948f 9428 6879 6a7c 0100 0090  .api...(hyj|....
-000033e0: 8c29 5051 416e 616c 7973 6973 2e69 6f2e  .)PQAnalysis.io.
-000033f0: 7472 616a 5f66 696c 652e 7472 616a 6563  traj_file.trajec
-00003400: 746f 7279 5f72 6561 6465 7294 8f94 288c  tory_reader...(.
-00003410: 1750 5141 6e61 6c79 7369 732e 696f 2e74  .PQAnalysis.io.t
-00003420: 7261 6a5f 6669 6c65 946a 7c01 0000 908c  raj_file.j|.....
-00003430: 2950 5141 6e61 6c79 7369 732e 696f 2e74  )PQAnalysis.io.t
-00003440: 7261 6a5f 6669 6c65 2e74 7261 6a65 6374  raj_file.traject
-00003450: 6f72 795f 7772 6974 6572 948f 9428 6ac1  ory_writer...(j.
-00003460: 0100 006a 7c01 0000 908c 2450 5141 6e61  ...j|.....$PQAna
-00003470: 6c79 7369 732e 696f 2e74 7261 6a5f 6669  lysis.io.traj_fi
-00003480: 6c65 2e66 7261 6d65 5f72 6561 6465 7294  le.frame_reader.
-00003490: 8f94 286a c101 0000 68a5 6a7c 0100 0090  ..(j....h.j|....
-000034a0: 8c1b 5051 416e 616c 7973 6973 2e69 6f2e  ..PQAnalysis.io.
-000034b0: 7472 616a 5f66 696c 652e 6170 6994 8f94  traj_file.api...
-000034c0: 2868 7968 756a 7c01 0000 908c 2650 5141  (hyhuj|.....&PQA
-000034d0: 6e61 6c79 7369 732e 696f 2e67 656e 5f66  nalysis.io.gen_f
-000034e0: 696c 652e 6765 6e5f 6669 6c65 5f72 6561  ile.gen_file_rea
-000034f0: 6465 7294 8f94 288c 1650 5141 6e61 6c79  der...(..PQAnaly
-00003500: 7369 732e 696f 2e67 656e 5f66 696c 6594  sis.io.gen_file.
-00003510: 6a5d 0100 006a 7c01 0000 908c 2650 5141  j]...j|.....&PQA
-00003520: 6e61 6c79 7369 732e 696f 2e67 656e 5f66  nalysis.io.gen_f
-00003530: 696c 652e 6765 6e5f 6669 6c65 5f77 7269  ile.gen_file_wri
-00003540: 7465 7294 8f94 286a ca01 0000 6a5d 0100  ter...(j....j]..
-00003550: 006a 7c01 0000 908c 1a50 5141 6e61 6c79  .j|......PQAnaly
-00003560: 7369 732e 696f 2e67 656e 5f66 696c 652e  sis.io.gen_file.
-00003570: 6170 6994 8f94 286a ca01 0000 6a7c 0100  api...(j....j|..
-00003580: 0090 8c1b 5051 416e 616c 7973 6973 2e69  ....PQAnalysis.i
-00003590: 6f2e 746f 706f 6c6f 6779 5f66 696c 6594  o.topology_file.
-000035a0: 8f94 286a 7c01 0000 908c 1f50 5141 6e61  ..(j|......PQAna
-000035b0: 6c79 7369 732e 696f 2e74 6f70 6f6c 6f67  lysis.io.topolog
-000035c0: 795f 6669 6c65 2e61 7069 948f 9428 6a7c  y_file.api...(j|
-000035d0: 0100 0090 8c20 5051 416e 616c 7973 6973  ..... PQAnalysis
-000035e0: 2e69 6f2e 656e 6572 6779 5f66 696c 655f  .io.energy_file_
-000035f0: 7265 6164 6572 948f 9428 6a7c 0100 0090  reader...(j|....
-00003600: 8c18 5051 416e 616c 7973 6973 2e69 6f2e  ..PQAnalysis.io.
-00003610: 626f 785f 7772 6974 6572 948f 9428 6879  box_writer...(hy
-00003620: 6875 6a7c 0100 0090 8c11 5051 416e 616c  huj|......PQAnal
-00003630: 7973 6973 2e69 6f2e 6170 6994 8f94 286a  ysis.io.api...(j
-00003640: 7c01 0000 908c 1c50 5141 6e61 6c79 7369  |......PQAnalysi
-00003650: 732e 696f 2e63 6f6e 7665 7273 696f 6e5f  s.io.conversion_
-00003660: 6170 6994 8f94 286a 7c01 0000 908c 1750  api...(j|......P
-00003670: 5141 6e61 6c79 7369 732e 696f 2e77 7269  QAnalysis.io.wri
-00003680: 7465 5f61 7069 948f 9428 6a7c 0100 0090  te_api...(j|....
-00003690: 8c17 5051 416e 616c 7973 6973 2e69 6f2e  ..PQAnalysis.io.
-000036a0: 7472 616a 5f66 696c 6594 8f94 2868 7968  traj_file...(hyh
-000036b0: a390 8c16 5051 416e 616c 7973 6973 2e69  ....PQAnalysis.i
-000036c0: 6f2e 6765 6e5f 6669 6c65 948f 9428 6879  o.gen_file...(hy
-000036d0: 908c 1250 5141 6e61 6c79 7369 732e 666f  ...PQAnalysis.fo
-000036e0: 726d 6174 7394 8f94 2868 8368 7d68 f190  rmats...(h.h}h..
-000036f0: 8c31 5051 416e 616c 7973 6973 2e69 6f2e  .1PQAnalysis.io.
-00003700: 696e 7075 745f 6669 6c65 5f72 6561 6465  input_file_reade
-00003710: 722e 696e 7075 745f 6669 6c65 5f70 6172  r.input_file_par
-00003720: 7365 7294 8f94 2868 9568 876a 3c01 0000  ser...(h.h.j<...
-00003730: 6aad 0100 0090 8c22 5051 416e 616c 7973  j......"PQAnalys
-00003740: 6973 2e69 6f2e 696e 7075 745f 6669 6c65  is.io.input_file
-00003750: 5f72 6561 6465 722e 7071 948f 9428 6aad  _reader.pq...(j.
-00003760: 0100 0090 8c2b 5051 416e 616c 7973 6973  .....+PQAnalysis
-00003770: 2e69 6f2e 696e 7075 745f 6669 6c65 5f72  .io.input_file_r
-00003780: 6561 6465 722e 7071 5f61 6e61 6c79 7369  eader.pq_analysi
-00003790: 7394 8f94 286a ad01 0000 908c 3250 5141  s...(j......2PQA
-000037a0: 6e61 6c79 7369 732e 696f 2e69 6e70 7574  nalysis.io.input
-000037b0: 5f66 696c 655f 7265 6164 6572 2e70 715f  _file_reader.pq_
-000037c0: 616e 616c 7973 6973 2e5f 7061 7273 6594  analysis._parse.
-000037d0: 8f94 286a 4f01 0000 6a47 0100 008c 3c50  ..(jO...jG....<P
-000037e0: 5141 6e61 6c79 7369 732e 696f 2e69 6e70  QAnalysis.io.inp
-000037f0: 7574 5f66 696c 655f 7265 6164 6572 2e70  ut_file_reader.p
-00003800: 715f 616e 616c 7973 6973 2e5f 7365 6c65  q_analysis._sele
-00003810: 6374 696f 6e5f 6d69 7869 6e94 908c 4850  ction_mixin...HP
-00003820: 5141 6e61 6c79 7369 732e 696f 2e69 6e70  QAnalysis.io.inp
-00003830: 7574 5f66 696c 655f 7265 6164 6572 2e70  ut_file_reader.p
-00003840: 715f 616e 616c 7973 6973 2e70 7161 6e61  q_analysis.pqana
-00003850: 6c79 7369 735f 696e 7075 745f 6669 6c65  lysis_input_file
-00003860: 5f72 6561 6465 7294 8f94 288c 2b50 5141  _reader...(.+PQA
-00003870: 6e61 6c79 7369 732e 696f 2e69 6e70 7574  nalysis.io.input
-00003880: 5f66 696c 655f 7265 6164 6572 2e70 715f  _file_reader.pq_
-00003890: 616e 616c 7973 6973 9490 8c37 5051 416e  analysis...7PQAn
-000038a0: 616c 7973 6973 2e69 6f2e 696e 7075 745f  alysis.io.input_
-000038b0: 6669 6c65 5f72 6561 6465 722e 7071 5f61  file_reader.pq_a
-000038c0: 6e61 6c79 7369 732e 5f66 696c 655f 6d69  nalysis._file_mi
-000038d0: 7869 6e94 8f94 286a 3c01 0000 908c 3c50  xin...(j<.....<P
-000038e0: 5141 6e61 6c79 7369 732e 696f 2e69 6e70  QAnalysis.io.inp
-000038f0: 7574 5f66 696c 655f 7265 6164 6572 2e70  ut_file_reader.p
-00003900: 715f 616e 616c 7973 6973 2e5f 7365 6c65  q_analysis._sele
-00003910: 6374 696f 6e5f 6d69 7869 6e94 8f94 286a  ction_mixin...(j
-00003920: 3c01 0000 908c 3c50 5141 6e61 6c79 7369  <.....<PQAnalysi
-00003930: 732e 696f 2e69 6e70 7574 5f66 696c 655f  s.io.input_file_
-00003940: 7265 6164 6572 2e70 715f 616e 616c 7973  reader.pq_analys
-00003950: 6973 2e5f 706f 7369 7469 6f6e 735f 6d69  is._positions_mi
-00003960: 7869 6e94 8f94 286a 3c01 0000 908c 2f50  xin...(j<...../P
-00003970: 5141 6e61 6c79 7369 732e 696f 2e69 6e70  QAnalysis.io.inp
-00003980: 7574 5f66 696c 655f 7265 6164 6572 2e70  ut_file_reader.p
-00003990: 712e 6f75 7470 7574 5f66 696c 6573 948f  q.output_files..
-000039a0: 9428 6895 908c 3750 5141 6e61 6c79 7369  .(h...7PQAnalysi
-000039b0: 732e 696f 2e69 6e70 7574 5f66 696c 655f  s.io.input_file_
-000039c0: 7265 6164 6572 2e70 712e 7071 5f69 6e70  reader.pq.pq_inp
-000039d0: 7574 5f66 696c 655f 7265 6164 6572 948f  ut_file_reader..
-000039e0: 9428 8c22 5051 416e 616c 7973 6973 2e69  .(."PQAnalysis.i
-000039f0: 6f2e 696e 7075 745f 6669 6c65 5f72 6561  o.input_file_rea
-00003a00: 6465 722e 7071 9490 8c25 5051 416e 616c  der.pq...%PQAnal
-00003a10: 7973 6973 2e69 6f2e 7265 7374 6172 745f  ysis.io.restart_
-00003a20: 6669 6c65 2e65 7863 6570 7469 6f6e 7394  file.exceptions.
-00003a30: 8f94 2868 a16a 3e01 0000 908c 2250 5141  ..(h.j>....."PQA
-00003a40: 6e61 6c79 7369 732e 696f 2e74 7261 6a5f  nalysis.io.traj_
-00003a50: 6669 6c65 2e65 7863 6570 7469 6f6e 7394  file.exceptions.
-00003a60: 8f94 286a 3b01 0000 68a5 908c 1850 5141  ..(j;...h....PQA
-00003a70: 6e61 6c79 7369 732e 696f 2e76 6972 6961  nalysis.io.viria
-00003a80: 6c2e 6170 6994 8f94 2868 af90 8c16 5051  l.api...(h....PQ
-00003a90: 416e 616c 7973 6973 2e75 7469 6c73 2e75  Analysis.utils.u
-00003aa0: 6e69 7473 948f 9428 68af 908c 1650 5141  nits...(h....PQA
-00003ab0: 6e61 6c79 7369 732e 7574 696c 732e 6669  nalysis.utils.fi
-00003ac0: 6c65 7394 8f94 2868 af90 8c1c 5051 416e  les...(h....PQAn
-00003ad0: 616c 7973 6973 2e69 6f2e 6e65 702e 6578  alysis.io.nep.ex
-00003ae0: 6365 7074 696f 6e73 948f 9428 68af 908c  ceptions...(h...
-00003af0: 2150 5141 6e61 6c79 7369 732e 696f 2e67  !PQAnalysis.io.g
-00003b00: 656e 5f66 696c 652e 6578 6365 7074 696f  en_file.exceptio
-00003b10: 6e73 948f 9428 6a3d 0100 0090 8c30 5051  ns...(j=.....0PQ
-00003b20: 416e 616c 7973 6973 2e69 6f2e 746f 706f  Analysis.io.topo
-00003b30: 6c6f 6779 5f66 696c 652e 746f 706f 6c6f  logy_file.topolo
-00003b40: 6779 5f66 696c 655f 7772 6974 6572 948f  gy_file_writer..
-00003b50: 9428 68bf 8c1b 5051 416e 616c 7973 6973  .(h...PQAnalysis
-00003b60: 2e69 6f2e 746f 706f 6c6f 6779 5f66 696c  .io.topology_fil
-00003b70: 6594 908c 3050 5141 6e61 6c79 7369 732e  e...0PQAnalysis.
-00003b80: 696f 2e74 6f70 6f6c 6f67 795f 6669 6c65  io.topology_file
-00003b90: 2e74 6f70 6f6c 6f67 795f 6669 6c65 5f72  .topology_file_r
-00003ba0: 6561 6465 7294 8f94 2868 bf6a 0a02 0000  eader...(h.j....
-00003bb0: 908c 2650 5141 6e61 6c79 7369 732e 696f  ..&PQAnalysis.io
-00003bc0: 2e74 6f70 6f6c 6f67 795f 6669 6c65 2e65  .topology_file.e
-00003bd0: 7863 6570 7469 6f6e 7394 8f94 2868 c168  xceptions...(h.h
-00003be0: c390 8c22 5051 416e 616c 7973 6973 2e69  ..."PQAnalysis.i
-00003bf0: 6f2e 7669 7269 616c 2e76 6972 6961 6c5f  o.virial.virial_
-00003c00: 7265 6164 6572 948f 9428 68c9 8c14 5051  reader...(h...PQ
-00003c10: 416e 616c 7973 6973 2e69 6f2e 7669 7269  Analysis.io.viri
-00003c20: 616c 9490 8c1c 5051 416e 616c 7973 6973  al....PQAnalysis
-00003c30: 2e69 6f2e 6e65 702e 6e65 705f 7772 6974  .io.nep.nep_writ
-00003c40: 6572 948f 9428 68cf 908c 1f50 5141 6e61  er...(h....PQAna
-00003c50: 6c79 7369 732e 636c 692e 5f61 7267 756d  lysis.cli._argum
-00003c60: 656e 745f 7061 7273 6572 948f 9428 68e3  ent_parser...(h.
-00003c70: 68d3 68df 68cf 68d1 68e1 68e5 68d9 68d7  h.h.h.h.h.h.h.h.
-00003c80: 68d5 908c 1850 5141 6e61 6c79 7369 732e  h....PQAnalysis.
-00003c90: 636c 692e 5f63 6c69 5f62 6173 6594 8f94  cli._cli_base...
-00003ca0: 2868 d368 df68 cf68 d168 e168 e568 d968  (h.h.h.h.h.h.h.h
-00003cb0: d768 d590 8c1d 5051 416e 616c 7973 6973  .h....PQAnalysis
-00003cc0: 2e74 6f6f 6c73 2e61 6464 5f6d 6f6c 6563  .tools.add_molec
-00003cd0: 756c 6594 8f94 2868 d790 8c16 5051 416e  ule...(h....PQAn
-00003ce0: 616c 7973 6973 2e63 6c69 2e78 797a 3267  alysis.cli.xyz2g
-00003cf0: 656e 948f 9428 68e3 908c 1950 5141 6e61  en...(h....PQAna
-00003d00: 6c79 7369 732e 636c 692e 7472 616a 3271  lysis.cli.traj2q
-00003d10: 6d63 6663 948f 9428 68e3 908c 1750 5141  mcfc...(h....PQA
-00003d20: 6e61 6c79 7369 732e 636c 692e 7472 616a  nalysis.cli.traj
-00003d30: 3262 6f78 948f 9428 68e3 908c 1650 5141  2box...(h....PQA
-00003d40: 6e61 6c79 7369 732e 636c 692e 7273 7432  nalysis.cli.rst2
-00003d50: 7879 7a94 8f94 2868 e390 8c12 5051 416e  xyz...(h....PQAn
-00003d60: 616c 7973 6973 2e63 6c69 2e72 6466 948f  alysis.cli.rdf..
-00003d70: 9428 68e3 908c 1650 5141 6e61 6c79 7369  .(h....PQAnalysi
-00003d80: 732e 636c 692e 6765 6e32 7879 7a94 8f94  s.cli.gen2xyz...
-00003d90: 2868 e390 8c1d 5051 416e 616c 7973 6973  (h....PQAnalysis
-00003da0: 2e63 6c69 2e63 6f6e 7469 6e75 655f 696e  .cli.continue_in
-00003db0: 7075 7494 8f94 2868 e390 8c1c 5051 416e  put...(h....PQAn
-00003dc0: 616c 7973 6973 2e63 6c69 2e61 6464 5f6d  alysis.cli.add_m
-00003dd0: 6f6c 6563 756c 6573 948f 9428 68e3 908c  olecules...(h...
-00003de0: 1d50 5141 6e61 6c79 7369 732e 636c 692e  .PQAnalysis.cli.
-00003df0: 6275 696c 645f 6e65 705f 7472 616a 948f  build_nep_traj..
-00003e00: 9428 68e3 908c 0b61 7267 636f 6d70 6c65  .(h....argcomple
-00003e10: 7465 948f 9428 68e7 908c 0d72 6963 685f  te...(h....rich_
-00003e20: 6172 6770 6172 7365 948f 9428 68e7 908c  argparse...(h...
-00003e30: 1750 5141 6e61 6c79 7369 732e 7574 696c  .PQAnalysis.util
-00003e40: 732e 636f 6d6d 6f6e 948f 9428 8c10 5051  s.common...(..PQ
-00003e50: 416e 616c 7973 6973 2e75 7469 6c73 9468  Analysis.utils.h
-00003e60: e790 8c13 5051 416e 616c 7973 6973 2e5f  ....PQAnalysis._
-00003e70: 7665 7273 696f 6e94 8f94 2868 e768 f790  version...(h.h..
-00003e80: 8c1a 5051 416e 616c 7973 6973 2e74 7261  ..PQAnalysis.tra
-00003e90: 6a2e 6578 6365 7074 696f 6e73 948f 9428  j.exceptions...(
-00003ea0: 8c0f 5051 416e 616c 7973 6973 2e74 7261  ..PQAnalysis.tra
-00003eb0: 6a94 68f1 908c 1750 5141 6e61 6c79 7369  j.h....PQAnalysi
-00003ec0: 732e 7472 616a 2e66 6f72 6d61 7473 948f  s.traj.formats..
-00003ed0: 9428 6a37 0200 0090 8c1a 5051 416e 616c  .(j7......PQAnal
-00003ee0: 7973 6973 2e74 7261 6a2e 7472 616a 6563  ysis.traj.trajec
-00003ef0: 746f 7279 948f 9428 6a37 0200 0090 68e9  tory...(j7....h.
-00003f00: 8f94 286a 3702 0000 908c 1b50 5141 6e61  ..(j7......PQAna
-00003f10: 6c79 7369 732e 7574 696c 732e 6465 636f  lysis.utils.deco
-00003f20: 7261 746f 7273 948f 9428 6a32 0200 0090  rators...(j2....
-00003f30: 8c14 5051 416e 616c 7973 6973 2e63 6f72  ..PQAnalysis.cor
-00003f40: 652e 6365 6c6c 948f 9428 6a65 0100 006a  e.cell...(je...j
-00003f50: 0101 0000 908c 1450 5141 6e61 6c79 7369  .......PQAnalysi
-00003f60: 732e 636f 7265 2e61 746f 6d94 8f94 286a  s.core.atom...(j
-00003f70: 0301 0000 6a65 0100 0090 8c17 5051 416e  ....je......PQAn
-00003f80: 616c 7973 6973 2e63 6f72 652e 7265 7369  alysis.core.resi
-00003f90: 6475 6594 8f94 286a 6501 0000 908c 1350  due...(je......P
-00003fa0: 5141 6e61 6c79 7369 732e 636f 7265 2e61  QAnalysis.core.a
-00003fb0: 7069 948f 9428 6a65 0100 0090 8c19 5051  pi...(je......PQ
-00003fc0: 416e 616c 7973 6973 2e63 6f72 652e 6365  Analysis.core.ce
-00003fd0: 6c6c 2e63 656c 6c94 8f94 288c 1450 5141  ll.cell...(..PQA
-00003fe0: 6e61 6c79 7369 732e 636f 7265 2e63 656c  nalysis.core.cel
-00003ff0: 6c94 908c 2950 5141 6e61 6c79 7369 732e  l...)PQAnalysis.
-00004000: 636f 7265 2e63 656c 6c2e 5f73 7461 6e64  core.cell._stand
-00004010: 6172 645f 7072 6f70 6572 7469 6573 948f  ard_properties..
-00004020: 9428 6a0d 0100 0090 8c1c 5051 416e 616c  .(j.......PQAnal
-00004030: 7973 6973 2e63 6f72 652e 6174 6f6d 2e65  ysis.core.atom.e
-00004040: 6c65 6d65 6e74 948f 9428 6a11 0100 008c  lement...(j.....
-00004050: 1450 5141 6e61 6c79 7369 732e 636f 7265  .PQAnalysis.core
-00004060: 2e61 746f 6d94 908c 1950 5141 6e61 6c79  .atom....PQAnaly
-00004070: 7369 732e 636f 7265 2e61 746f 6d2e 6174  sis.core.atom.at
-00004080: 6f6d 948f 9428 6a4e 0200 0090 8c23 5051  om...(jN.....#PQ
-00004090: 416e 616c 7973 6973 2e70 6879 7369 6361  Analysis.physica
-000040a0: 6c5f 6461 7461 2e65 7863 6570 7469 6f6e  l_data.exception
-000040b0: 7394 8f94 288c 1850 5141 6e61 6c79 7369  s...(..PQAnalysi
-000040c0: 732e 7068 7973 6963 616c 5f64 6174 6194  s.physical_data.
-000040d0: 6a19 0100 0090 8c1f 5051 416e 616c 7973  j.......PQAnalys
-000040e0: 6973 2e70 6879 7369 6361 6c5f 6461 7461  is.physical_data
-000040f0: 2e65 6e65 7267 7994 8f94 286a 5302 0000  .energy...(jS...
-00004100: 9075 8c10 6475 706c 6963 6174 6564 5f6c  .u..duplicated_l
-00004110: 696e 6573 947d 9428 8c13 6e62 5f64 7570  ines.}.(..nb_dup
-00004120: 6c69 6361 7465 645f 6c69 6e65 7394 4b00  licated_lines.K.
-00004130: 8c18 7065 7263 656e 745f 6475 706c 6963  ..percent_duplic
-00004140: 6174 6564 5f6c 696e 6573 9447 0000 0000  ated_lines.G....
-00004150: 0000 0000 758c 0a6e 6f64 655f 636f 756e  ....u..node_coun
-00004160: 7494 7d94 2868 0e4b 4b68 094b 7468 0f4d  t.}.(h.KKh.Kth.M
-00004170: 0602 6810 4b7c 758c 0c75 6e64 6f63 756d  ..h.K|u..undocum
-00004180: 656e 7465 6494 7d94 2868 0e4b 0068 094b  ented.}.(h.K.h.K
-00004190: 0068 0f4b 0068 104b 0075 6818 4b02 6819  .h.K.h.K.uh.K.h.
-000041a0: 4b00 681a 4b00 681b 4b00 681c 4b33 681d  K.h.K.h.K.h.K3h.
-000041b0: 4d73 1168 1e4b 0c8c 0b67 6c6f 6261 6c5f  Ms.h.K...global_
-000041c0: 6e6f 7465 9447 4023 b57f 834b 973d 6a58  note.G@#...K.=jX
-000041d0: 0200 004b 196a 5902 0000 473f c101 0c25  ...K.jY...G?...%
-000041e0: d12d 7375 622e                           .-sub.
+00001410: 681c 4b01 681d 4b24 681e 4b00 758c 2950  h.K.h.K$h.K.u.)P
+00001420: 5141 6e61 6c79 7369 732e 746f 706f 6c6f  QAnalysis.topolo
+00001430: 6779 2e62 6f6e 6465 645f 746f 706f 6c6f  gy.bonded_topolo
+00001440: 6779 2e61 6e67 6c65 947d 9428 6818 4b00  gy.angle.}.(h.K.
+00001450: 6819 4b00 681a 4b00 681b 4b00 681c 4b01  h.K.h.K.h.K.h.K.
+00001460: 681d 4b10 681e 4b00 758c 1850 5141 6e61  h.K.h.K.u..PQAna
+00001470: 6c79 7369 732e 696f 2e65 7863 6570 7469  lysis.io.excepti
+00001480: 6f6e 7394 7d94 2868 184b 0068 194b 0068  ons.}.(h.K.h.K.h
+00001490: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0668  .K.h.K.h.K.h.K.h
+000014a0: 1e4b 0075 8c15 5051 416e 616c 7973 6973  .K.u..PQAnalysis
+000014b0: 2e69 6f2e 666f 726d 6174 7394 7d94 2868  .io.formats.}.(h
+000014c0: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+000014d0: 1c4b 0168 1d4b 5168 1e4b 0075 8c11 5051  .K.h.KQh.K.u..PQ
+000014e0: 416e 616c 7973 6973 2e69 6f2e 6170 6994  Analysis.io.api.
+000014f0: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00001500: 1b4b 0068 1c4b 0068 1d4b 1168 1e4b 0075  .K.h.K.h.K.h.K.u
+00001510: 8c20 5051 416e 616c 7973 6973 2e69 6f2e  . PQAnalysis.io.
+00001520: 656e 6572 6779 5f66 696c 655f 7265 6164  energy_file_read
+00001530: 6572 947d 9428 6818 4b00 6819 4b00 681a  er.}.(h.K.h.K.h.
+00001540: 4b00 681b 4b00 681c 4b00 681d 4b2e 681e  K.h.K.h.K.h.K.h.
+00001550: 4b00 758c 1c50 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
+00001560: 696f 2e63 6f6e 7665 7273 696f 6e5f 6170  io.conversion_ap
+00001570: 6994 7d94 2868 184b 0068 194b 0068 1a4b  i.}.(h.K.h.K.h.K
+00001580: 0068 1b4b 0068 1c4b 0068 1d4b 2768 1e4b  .h.K.h.K.h.K'h.K
+00001590: 0075 8c12 5051 416e 616c 7973 6973 2e69  .u..PQAnalysis.i
+000015a0: 6f2e 6261 7365 947d 9428 6818 4b00 6819  o.base.}.(h.K.h.
+000015b0: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
+000015c0: 4b32 681e 4b00 758c 1e50 5141 6e61 6c79  K2h.K.u..PQAnaly
+000015d0: 7369 732e 696f 2e69 6e66 6f5f 6669 6c65  sis.io.info_file
+000015e0: 5f72 6561 6465 7294 7d94 2868 184b 0068  _reader.}.(h.K.h
+000015f0: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0168  .K.h.K.h.K.h.K.h
+00001600: 1d4b 3768 1e4b 0075 8c16 5051 416e 616c  .K7h.K.u..PQAnal
+00001610: 7973 6973 2e69 6f2e 5f5f 696e 6974 5f5f  ysis.io.__init__
+00001620: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+00001630: 681b 4b00 681c 4b00 681d 4b1a 681e 4b00  h.K.h.K.h.K.h.K.
+00001640: 758c 1750 5141 6e61 6c79 7369 732e 696f  u..PQAnalysis.io
+00001650: 2e77 7269 7465 5f61 7069 947d 9428 6818  .write_api.}.(h.
+00001660: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
+00001670: 4b00 681d 4b14 681e 4b01 758c 1850 5141  K.h.K.h.K.u..PQA
+00001680: 6e61 6c79 7369 732e 696f 2e62 6f78 5f77  nalysis.io.box_w
+00001690: 7269 7465 7294 7d94 2868 184b 0068 194b  riter.}.(h.K.h.K
+000016a0: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
+000016b0: 2c68 1e4b 0075 8c22 5051 416e 616c 7973  ,h.K.u."PQAnalys
+000016c0: 6973 2e69 6f2e 6d6f 6c64 6573 6372 6970  is.io.moldescrip
+000016d0: 746f 725f 7265 6164 6572 947d 9428 6818  tor_reader.}.(h.
+000016e0: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
+000016f0: 4b00 681d 4b39 681e 4b02 758c 2250 5141  K.h.K9h.K.u."PQA
+00001700: 6e61 6c79 7369 732e 696f 2e74 7261 6a5f  nalysis.io.traj_
+00001710: 6669 6c65 2e65 7863 6570 7469 6f6e 7394  file.exceptions.
+00001720: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00001730: 1b4b 0068 1c4b 0068 1d4b 0368 1e4b 0075  .K.h.K.h.K.h.K.u
+00001740: 8c29 5051 416e 616c 7973 6973 2e69 6f2e  .)PQAnalysis.io.
+00001750: 7472 616a 5f66 696c 652e 7472 616a 6563  traj_file.trajec
+00001760: 746f 7279 5f77 7269 7465 7294 7d94 2868  tory_writer.}.(h
+00001770: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+00001780: 1c4b 0068 1d4b 4f68 1e4b 0075 8c1b 5051  .K.h.KOh.K.u..PQ
+00001790: 416e 616c 7973 6973 2e69 6f2e 7472 616a  Analysis.io.traj
+000017a0: 5f66 696c 652e 6170 6994 7d94 2868 184b  _file.api.}.(h.K
+000017b0: 0068 194b 0168 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
+000017c0: 0068 1d4b 1368 1e4b 0075 8c20 5051 416e  .h.K.h.K.u. PQAn
+000017d0: 616c 7973 6973 2e69 6f2e 7472 616a 5f66  alysis.io.traj_f
+000017e0: 696c 652e 5f5f 696e 6974 5f5f 947d 9428  ile.__init__.}.(
+000017f0: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+00001800: 681c 4b00 681d 4b03 681e 4b00 758c 2450  h.K.h.K.h.K.u.$P
+00001810: 5141 6e61 6c79 7369 732e 696f 2e74 7261  QAnalysis.io.tra
+00001820: 6a5f 6669 6c65 2e66 7261 6d65 5f72 6561  j_file.frame_rea
+00001830: 6465 7294 7d94 2868 184b 0068 194b 0268  der.}.(h.K.h.K.h
+00001840: 1a4b 0068 1b4b 0068 1c4b 0268 1d4b 6e68  .K.h.K.h.K.h.Knh
+00001850: 1e4b 0075 8c29 5051 416e 616c 7973 6973  .K.u.)PQAnalysis
+00001860: 2e69 6f2e 7472 616a 5f66 696c 652e 7472  .io.traj_file.tr
+00001870: 616a 6563 746f 7279 5f72 6561 6465 7294  ajectory_reader.
+00001880: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00001890: 1b4b 0068 1c4b 0568 1d4b a768 1e4b 0075  .K.h.K.h.K.h.K.u
+000018a0: 8c21 5051 416e 616c 7973 6973 2e69 6f2e  .!PQAnalysis.io.
+000018b0: 6765 6e5f 6669 6c65 2e65 7863 6570 7469  gen_file.excepti
+000018c0: 6f6e 7394 7d94 2868 184b 0068 194b 0068  ons.}.(h.K.h.K.h
+000018d0: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0268  .K.h.K.h.K.h.K.h
+000018e0: 1e4b 0075 8c1a 5051 416e 616c 7973 6973  .K.u..PQAnalysis
+000018f0: 2e69 6f2e 6765 6e5f 6669 6c65 2e61 7069  .io.gen_file.api
+00001900: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+00001910: 681b 4b00 681c 4b00 681d 4b09 681e 4b00  h.K.h.K.h.K.h.K.
+00001920: 758c 1f50 5141 6e61 6c79 7369 732e 696f  u..PQAnalysis.io
+00001930: 2e67 656e 5f66 696c 652e 5f5f 696e 6974  .gen_file.__init
+00001940: 5f5f 947d 9428 6818 4b00 6819 4b00 681a  __.}.(h.K.h.K.h.
+00001950: 4b00 681b 4b00 681c 4b00 681d 4b03 681e  K.h.K.h.K.h.K.h.
+00001960: 4b00 758c 2650 5141 6e61 6c79 7369 732e  K.u.&PQAnalysis.
+00001970: 696f 2e67 656e 5f66 696c 652e 6765 6e5f  io.gen_file.gen_
+00001980: 6669 6c65 5f77 7269 7465 7294 7d94 2868  file_writer.}.(h
+00001990: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+000019a0: 1c4b 0068 1d4b 2c68 1e4b 0075 8c26 5051  .K.h.K,h.K.u.&PQ
+000019b0: 416e 616c 7973 6973 2e69 6f2e 6765 6e5f  Analysis.io.gen_
+000019c0: 6669 6c65 2e67 656e 5f66 696c 655f 7265  file.gen_file_re
+000019d0: 6164 6572 947d 9428 6818 4b00 6819 4b01  ader.}.(h.K.h.K.
+000019e0: 681a 4b00 681b 4b00 681c 4b00 681d 4b2f  h.K.h.K.h.K.h.K/
+000019f0: 681e 4b00 758c 1850 5141 6e61 6c79 7369  h.K.u..PQAnalysi
+00001a00: 732e 696f 2e76 6972 6961 6c2e 6170 6994  s.io.virial.api.
+00001a10: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00001a20: 1b4b 0068 1c4b 0068 1d4b 0968 1e4b 0075  .K.h.K.h.K.h.K.u
+00001a30: 8c1d 5051 416e 616c 7973 6973 2e69 6f2e  ..PQAnalysis.io.
+00001a40: 7669 7269 616c 2e5f 5f69 6e69 745f 5f94  virial.__init__.
+00001a50: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00001a60: 1b4b 0068 1c4b 0068 1d4b 0168 1e4b 0075  .K.h.K.h.K.h.K.u
+00001a70: 8c22 5051 416e 616c 7973 6973 2e69 6f2e  ."PQAnalysis.io.
+00001a80: 7669 7269 616c 2e76 6972 6961 6c5f 7265  virial.virial_re
+00001a90: 6164 6572 947d 9428 6818 4b00 6819 4b00  ader.}.(h.K.h.K.
+00001aa0: 681a 4b00 681b 4b00 681c 4b00 681d 4b14  h.K.h.K.h.K.h.K.
+00001ab0: 681e 4b00 758c 2650 5141 6e61 6c79 7369  h.K.u.&PQAnalysi
+00001ac0: 732e 696f 2e74 6f70 6f6c 6f67 795f 6669  s.io.topology_fi
+00001ad0: 6c65 2e65 7863 6570 7469 6f6e 7394 7d94  le.exceptions.}.
+00001ae0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+00001af0: 0068 1c4b 0068 1d4b 0268 1e4b 0075 8c1f  .h.K.h.K.h.K.u..
+00001b00: 5051 416e 616c 7973 6973 2e69 6f2e 746f  PQAnalysis.io.to
+00001b10: 706f 6c6f 6779 5f66 696c 652e 6170 6994  pology_file.api.
+00001b20: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00001b30: 1b4b 0068 1c4b 0068 1d4b 0968 1e4b 0075  .K.h.K.h.K.h.K.u
+00001b40: 8c30 5051 416e 616c 7973 6973 2e69 6f2e  .0PQAnalysis.io.
+00001b50: 746f 706f 6c6f 6779 5f66 696c 652e 746f  topology_file.to
+00001b60: 706f 6c6f 6779 5f66 696c 655f 7265 6164  pology_file_read
+00001b70: 6572 947d 9428 6818 4b00 6819 4b15 681a  er.}.(h.K.h.K.h.
+00001b80: 4b00 681b 4b00 681c 4b00 681d 4b71 681e  K.h.K.h.K.h.Kqh.
+00001b90: 4b00 758c 2450 5141 6e61 6c79 7369 732e  K.u.$PQAnalysis.
+00001ba0: 696f 2e74 6f70 6f6c 6f67 795f 6669 6c65  io.topology_file
+00001bb0: 2e5f 5f69 6e69 745f 5f94 7d94 2868 184b  .__init__.}.(h.K
+00001bc0: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
+00001bd0: 0068 1d4b 0268 1e4b 0075 8c30 5051 416e  .h.K.h.K.u.0PQAn
+00001be0: 616c 7973 6973 2e69 6f2e 746f 706f 6c6f  alysis.io.topolo
+00001bf0: 6779 5f66 696c 652e 746f 706f 6c6f 6779  gy_file.topology
+00001c00: 5f66 696c 655f 7772 6974 6572 947d 9428  _file_writer.}.(
+00001c10: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+00001c20: 681c 4b00 681d 4b6b 681e 4b00 758c 2550  h.K.h.Kkh.K.u.%P
+00001c30: 5141 6e61 6c79 7369 732e 696f 2e72 6573  QAnalysis.io.res
+00001c40: 7461 7274 5f66 696c 652e 6578 6365 7074  tart_file.except
+00001c50: 696f 6e73 947d 9428 6818 4b00 6819 4b00  ions.}.(h.K.h.K.
+00001c60: 681a 4b00 681b 4b00 681c 4b00 681d 4b03  h.K.h.K.h.K.h.K.
+00001c70: 681e 4b00 758c 2950 5141 6e61 6c79 7369  h.K.u.)PQAnalysi
+00001c80: 732e 696f 2e72 6573 7461 7274 5f66 696c  s.io.restart_fil
+00001c90: 652e 7265 7374 6172 745f 7265 6164 6572  e.restart_reader
+00001ca0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+00001cb0: 681b 4b00 681c 4b01 681d 4b49 681e 4b00  h.K.h.K.h.KIh.K.
+00001cc0: 758c 2950 5141 6e61 6c79 7369 732e 696f  u.)PQAnalysis.io
+00001cd0: 2e72 6573 7461 7274 5f66 696c 652e 7265  .restart_file.re
+00001ce0: 7374 6172 745f 7772 6974 6572 947d 9428  start_writer.}.(
+00001cf0: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+00001d00: 681c 4b00 681d 4b3d 681e 4b00 758c 1e50  h.K.h.K=h.K.u..P
+00001d10: 5141 6e61 6c79 7369 732e 696f 2e72 6573  QAnalysis.io.res
+00001d20: 7461 7274 5f66 696c 652e 6170 6994 7d94  tart_file.api.}.
+00001d30: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+00001d40: 0068 1c4b 0068 1d4b 0868 1e4b 0075 8c23  .h.K.h.K.h.K.u.#
+00001d50: 5051 416e 616c 7973 6973 2e69 6f2e 7265  PQAnalysis.io.re
+00001d60: 7374 6172 745f 6669 6c65 2e5f 5f69 6e69  start_file.__ini
+00001d70: 745f 5f94 7d94 2868 184b 0068 194b 0068  t__.}.(h.K.h.K.h
+00001d80: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0268  .K.h.K.h.K.h.K.h
+00001d90: 1e4b 0075 8c2a 5051 416e 616c 7973 6973  .K.u.*PQAnalysis
+00001da0: 2e69 6f2e 696e 7075 745f 6669 6c65 5f72  .io.input_file_r
+00001db0: 6561 6465 722e 6578 6365 7074 696f 6e73  eader.exceptions
+00001dc0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+00001dd0: 681b 4b00 681c 4b00 681d 4b0e 681e 4b00  h.K.h.K.h.K.h.K.
+00001de0: 758c 2750 5141 6e61 6c79 7369 732e 696f  u.'PQAnalysis.io
+00001df0: 2e69 6e70 7574 5f66 696c 655f 7265 6164  .input_file_read
+00001e00: 6572 2e66 6f72 6d61 7473 947d 9428 6818  er.formats.}.(h.
+00001e10: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
+00001e20: 4b00 681d 4b0f 681e 4b00 758c 2850 5141  K.h.K.h.K.u.(PQA
+00001e30: 6e61 6c79 7369 732e 696f 2e69 6e70 7574  nalysis.io.input
+00001e40: 5f66 696c 655f 7265 6164 6572 2e5f 5f69  _file_reader.__i
+00001e50: 6e69 745f 5f94 7d94 2868 184b 0068 194b  nit__.}.(h.K.h.K
+00001e60: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
+00001e70: 0468 1e4b 0075 8c31 5051 416e 616c 7973  .h.K.u.1PQAnalys
+00001e80: 6973 2e69 6f2e 696e 7075 745f 6669 6c65  is.io.input_file
+00001e90: 5f72 6561 6465 722e 696e 7075 745f 6669  _reader.input_fi
+00001ea0: 6c65 5f70 6172 7365 7294 7d94 2868 184b  le_parser.}.(h.K
+00001eb0: 0068 194b 0168 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
+00001ec0: 0168 1d4b 7f68 1e4b 0075 8c32 5051 416e  .h.K.h.K.u.2PQAn
+00001ed0: 616c 7973 6973 2e69 6f2e 696e 7075 745f  alysis.io.input_
+00001ee0: 6669 6c65 5f72 6561 6465 722e 7071 5f61  file_reader.pq_a
+00001ef0: 6e61 6c79 7369 732e 5f70 6172 7365 947d  nalysis._parse.}
+00001f00: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+00001f10: 4b00 681c 4b01 681d 4b44 681e 4b00 758c  K.h.K.h.KDh.K.u.
+00001f20: 3450 5141 6e61 6c79 7369 732e 696f 2e69  4PQAnalysis.io.i
+00001f30: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
+00001f40: 2e70 715f 616e 616c 7973 6973 2e5f 5f69  .pq_analysis.__i
+00001f50: 6e69 745f 5f94 7d94 2868 184b 0068 194b  nit__.}.(h.K.h.K
+00001f60: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
+00001f70: 0168 1e4b 0075 8c48 5051 416e 616c 7973  .h.K.u.HPQAnalys
+00001f80: 6973 2e69 6f2e 696e 7075 745f 6669 6c65  is.io.input_file
+00001f90: 5f72 6561 6465 722e 7071 5f61 6e61 6c79  _reader.pq_analy
+00001fa0: 7369 732e 7071 616e 616c 7973 6973 5f69  sis.pqanalysis_i
+00001fb0: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
+00001fc0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+00001fd0: 681b 4b00 681c 4b00 681d 4b3b 681e 4b00  h.K.h.K.h.K;h.K.
+00001fe0: 758c 3c50 5141 6e61 6c79 7369 732e 696f  u.<PQAnalysis.io
+00001ff0: 2e69 6e70 7574 5f66 696c 655f 7265 6164  .input_file_read
+00002000: 6572 2e70 715f 616e 616c 7973 6973 2e5f  er.pq_analysis._
+00002010: 7365 6c65 6374 696f 6e5f 6d69 7869 6e94  selection_mixin.
+00002020: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00002030: 1b4b 0068 1c4b 0068 1d4b 0c68 1e4b 0075  .K.h.K.h.K.h.K.u
+00002040: 8c3c 5051 416e 616c 7973 6973 2e69 6f2e  .<PQAnalysis.io.
+00002050: 696e 7075 745f 6669 6c65 5f72 6561 6465  input_file_reade
+00002060: 722e 7071 5f61 6e61 6c79 7369 732e 5f70  r.pq_analysis._p
+00002070: 6f73 6974 696f 6e73 5f6d 6978 696e 947d  ositions_mixin.}
+00002080: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+00002090: 4b00 681c 4b00 681d 4b0b 681e 4b00 758c  K.h.K.h.K.h.K.u.
+000020a0: 3750 5141 6e61 6c79 7369 732e 696f 2e69  7PQAnalysis.io.i
+000020b0: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
+000020c0: 2e70 715f 616e 616c 7973 6973 2e5f 6669  .pq_analysis._fi
+000020d0: 6c65 5f6d 6978 696e 947d 9428 6818 4b00  le_mixin.}.(h.K.
+000020e0: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
+000020f0: 681d 4b0d 681e 4b00 758c 3750 5141 6e61  h.K.h.K.u.7PQAna
+00002100: 6c79 7369 732e 696f 2e69 6e70 7574 5f66  lysis.io.input_f
+00002110: 696c 655f 7265 6164 6572 2e70 712e 7071  ile_reader.pq.pq
+00002120: 5f69 6e70 7574 5f66 696c 655f 7265 6164  _input_file_read
+00002130: 6572 947d 9428 6818 4b00 6819 4b00 681a  er.}.(h.K.h.K.h.
+00002140: 4b00 681b 4b00 681c 4b01 681d 4b58 681e  K.h.K.h.K.h.KXh.
+00002150: 4b00 758c 2b50 5141 6e61 6c79 7369 732e  K.u.+PQAnalysis.
+00002160: 696f 2e69 6e70 7574 5f66 696c 655f 7265  io.input_file_re
+00002170: 6164 6572 2e70 712e 5f5f 696e 6974 5f5f  ader.pq.__init__
+00002180: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+00002190: 681b 4b00 681c 4b00 681d 4b01 681e 4b00  h.K.h.K.h.K.h.K.
+000021a0: 758c 2f50 5141 6e61 6c79 7369 732e 696f  u./PQAnalysis.io
+000021b0: 2e69 6e70 7574 5f66 696c 655f 7265 6164  .input_file_read
+000021c0: 6572 2e70 712e 6f75 7470 7574 5f66 696c  er.pq.output_fil
+000021d0: 6573 947d 9428 6818 4b00 6819 4b00 681a  es.}.(h.K.h.K.h.
+000021e0: 4b00 681b 4b00 681c 4b00 681d 4b32 681e  K.h.K.h.K.h.K2h.
+000021f0: 4b00 758c 1c50 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
+00002200: 696f 2e6e 6570 2e65 7863 6570 7469 6f6e  io.nep.exception
+00002210: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
+00002220: 0068 1b4b 0068 1c4b 0068 1d4b 0268 1e4b  .h.K.h.K.h.K.h.K
+00002230: 0075 8c1a 5051 416e 616c 7973 6973 2e69  .u..PQAnalysis.i
+00002240: 6f2e 6e65 702e 5f5f 696e 6974 5f5f 947d  o.nep.__init__.}
+00002250: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+00002260: 4b00 681c 4b00 681d 4b00 681e 4b00 758c  K.h.K.h.K.h.K.u.
+00002270: 1c50 5141 6e61 6c79 7369 732e 696f 2e6e  .PQAnalysis.io.n
+00002280: 6570 2e6e 6570 5f77 7269 7465 7294 7d94  ep.nep_writer.}.
+00002290: 2868 184b 0168 194b 0468 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+000022a0: 0068 1c4b 0b68 1d4d 1601 681e 4b00 7575  .h.K.h.M..h.K.uu
+000022b0: 8c06 6279 5f6d 7367 947d 9428 8c05 6669  ..by_msg.}.(..fi
+000022c0: 786d 6594 4b09 8c1f 706f 7373 6962 6c79  xme.K...possibly
+000022d0: 2d75 7365 642d 6265 666f 7265 2d61 7373  -used-before-ass
+000022e0: 6967 6e6d 656e 7494 4b1e 8c1c 746f 6f2d  ignment.K...too-
+000022f0: 6d61 6e79 2d69 6e73 7461 6e63 652d 6174  many-instance-at
+00002300: 7472 6962 7574 6573 944b 0a8c 1274 6f6f  tributes.K...too
+00002310: 2d6d 616e 792d 6172 6775 6d65 6e74 7394  -many-arguments.
+00002320: 4b12 8c0f 746f 6f2d 6d61 6e79 2d6c 6f63  K...too-many-loc
+00002330: 616c 7394 4b03 8c1a 746f 6f2d 6d61 6e79  als.K...too-many
+00002340: 2d72 6574 7572 6e2d 7374 6174 656d 656e  -return-statemen
+00002350: 7473 944b 018c 1774 6f6f 2d6d 616e 792d  ts.K...too-many-
+00002360: 7075 626c 6963 2d6d 6574 686f 6473 944b  public-methods.K
+00002370: 018c 1e69 6e63 6f6e 7369 7374 656e 742d  ...inconsistent-
+00002380: 7265 7475 726e 2d73 7461 7465 6d65 6e74  return-statement
+00002390: 7394 4b09 8c0f 756e 7573 6564 2d61 7267  s.K...unused-arg
+000023a0: 756d 656e 7494 4b01 8c09 6e6f 2d6d 656d  ument.K...no-mem
+000023b0: 6265 7294 4b01 8c0b 746f 6f2d 636f 6d70  ber.K...too-comp
+000023c0: 6c65 7894 4b03 8c11 746f 6f2d 6d61 6e79  lex.K...too-many
+000023d0: 2d62 7261 6e63 6865 7394 4b02 8c0e 746f  -branches.K...to
+000023e0: 6f2d 6d61 6e79 2d6c 696e 6573 944b 018c  o-many-lines.K..
+000023f0: 1374 6f6f 2d6d 616e 792d 7374 6174 656d  .too-many-statem
+00002400: 656e 7473 944b 018c 0e64 7570 6c69 6361  ents.K...duplica
+00002410: 7465 2d63 6f64 6594 4b03 758c 0f63 6f64  te-code.K.u..cod
+00002420: 655f 7479 7065 5f63 6f75 6e74 947d 9428  e_type_count.}.(
+00002430: 8c04 636f 6465 944d 811e 8c07 636f 6d6d  ..code.M....comm
+00002440: 656e 7494 4d09 018c 0964 6f63 7374 7269  ent.M....docstri
+00002450: 6e67 944d 9621 8c05 656d 7074 7994 4d36  ng.M.!..empty.M6
+00002460: 0b8c 0574 6f74 616c 944d 564c 758c 0c64  ...total.MVLu..d
+00002470: 6570 656e 6465 6e63 6965 7394 7d94 288c  ependencies.}.(.
+00002480: 0d62 6561 7274 7970 652e 636c 6177 948f  .beartype.claw..
+00002490: 9428 6823 908c 1150 5141 6e61 6c79 7369  .(h#...PQAnalysi
+000024a0: 732e 636f 6e66 6967 948f 9428 6869 686b  s.config...(hihk
+000024b0: 6855 685d 6857 68d7 685b 6a1b 0100 0068  hUh]hWh.h[j....h
+000024c0: 5368 6568 4568 2368 6768 6168 6368 3790  ShehEh#hghahch7.
+000024d0: 8c1f 5051 416e 616c 7973 6973 2e75 7469  ..PQAnalysis.uti
+000024e0: 6c73 2e63 7573 746f 6d5f 6c6f 6767 696e  ls.custom_loggin
+000024f0: 6794 8f94 2868 b968 ed68 f18c 2950 5141  g...(h.h.h..)PQA
+00002500: 6e61 6c79 7369 732e 696f 2e72 6573 7461  nalysis.io.resta
+00002510: 7274 5f66 696c 652e 7265 7374 6172 745f  rt_file.restart_
+00002520: 7265 6164 6572 948c 1250 5141 6e61 6c79  reader...PQAnaly
+00002530: 7369 732e 696f 2e62 6173 6594 68d5 6a1b  sis.io.base.h.j.
+00002540: 0100 006a 1101 0000 6851 6897 6a05 0100  ...j....hQh.j...
+00002550: 0068 bb68 4768 b368 c968 2368 6f68 c38c  .h.hGh.h.h#hoh..
+00002560: 4850 5141 6e61 6c79 7369 732e 696f 2e69  HPQAnalysis.io.i
+00002570: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
+00002580: 2e70 715f 616e 616c 7973 6973 2e70 7161  .pq_analysis.pqa
+00002590: 6e61 6c79 7369 735f 696e 7075 745f 6669  nalysis_input_fi
+000025a0: 6c65 5f72 6561 6465 7294 6895 68c7 68a1  le_reader.h.h.h.
+000025b0: 6877 68bd 68d7 68a9 68cb 68a7 68df 6883  hwh.h.h.h.h.h.h.
+000025c0: 6a03 0100 0068 8768 8f68 458c 2650 5141  j....h.h.hE.&PQA
+000025d0: 6e61 6c79 7369 732e 696f 2e67 656e 5f66  nalysis.io.gen_f
+000025e0: 696c 652e 6765 6e5f 6669 6c65 5f72 6561  ile.gen_file_rea
+000025f0: 6465 7294 68f7 682d 908c 0b6d 756c 7469  der.h.h-...multi
+00002600: 6d65 7468 6f64 948f 9428 6825 908c 0f62  method...(h%...b
+00002610: 6561 7274 7970 652e 7479 7069 6e67 948f  eartype.typing..
+00002620: 9428 68b9 68ed 683b 68f1 6a3d 0100 006a  .(h.h.h;h.j=...j
+00002630: 3e01 0000 68d5 6a1b 0100 0068 a368 5168  >...h.j....h.hQh
+00002640: cf68 4368 976a 0501 0000 8c37 5051 416e  .hCh.j.....7PQAn
+00002650: 616c 7973 6973 2e69 6f2e 696e 7075 745f  alysis.io.input_
+00002660: 6669 6c65 5f72 6561 6465 722e 7071 5f61  file_reader.pq_a
+00002670: 6e61 6c79 7369 732e 5f66 696c 655f 6d69  nalysis._file_mi
+00002680: 7869 6e94 68b3 68ad 688b 686f 682b 6869  xin.h.h.h.hoh+hi
+00002690: 68c3 6a3f 0100 0068 9568 c768 2f68 a168  h.j?...h.h.h/h.h
+000026a0: 7768 d768 7568 a968 cb68 a768 998c 2350  wh.huh.h.h.h..#P
+000026b0: 5141 6e61 6c79 7369 732e 6174 6f6d 6963  QAnalysis.atomic
+000026c0: 5f73 7973 7465 6d2e 5f70 6f73 6974 696f  _system._positio
+000026d0: 6e73 9468 e368 ff68 838c 2450 5141 6e61  ns.h.h.h..$PQAna
+000026e0: 6c79 7369 732e 6174 6f6d 6963 5f73 7973  lysis.atomic_sys
+000026f0: 7465 6d2e 5f70 726f 7065 7274 6965 7394  tem._properties.
+00002700: 6829 68bf 6887 6a03 0100 0068 8f68 d168  h)h.h.j....h.h.h
+00002710: 456a 4001 0000 68f7 6837 682d 908c 056e  Ej@...h.h7h-...n
+00002720: 756d 7079 948f 9428 6a3d 0100 0068 3968  umpy...(j=...h9h
+00002730: d56a 1b01 0000 6851 688d 8c29 5051 416e  .j....hQh..)PQAn
+00002740: 616c 7973 6973 2e63 6f72 652e 6365 6c6c  alysis.core.cell
+00002750: 2e5f 7374 616e 6461 7264 5f70 726f 7065  ._standard_prope
+00002760: 7274 6965 7394 686f 682b 682f 68a1 6877  rties.hoh+h/h.hw
+00002770: 68bd 6875 68e7 68a9 68cb 68a7 68df 6899  h.huh.h.h.h.h.h.
+00002780: 6a46 0100 006a 4701 0000 6887 688f 6845  jF...jG...h.h.hE
+00002790: 6a40 0100 0068 f790 8c0d 6265 6172 7479  j@...h....bearty
+000027a0: 7065 2e76 616c 6594 8f94 2868 9768 2b68  pe.vale...(h.h+h
+000027b0: 9990 8c09 6465 636f 7261 746f 7294 8f94  ....decorator...
+000027c0: 2868 7568 3b68 2d90 8c0d 6265 6172 7479  (huh;h-...bearty
+000027d0: 7065 2e64 6f6f 7294 8f94 2868 2d90 8c15  pe.door...(h-...
+000027e0: 5051 416e 616c 7973 6973 2e65 7863 6570  PQAnalysis.excep
+000027f0: 7469 6f6e 7394 8f94 286a 1701 0000 6a3e  tions...(j....j>
+00002800: 0100 0068 f368 7368 fd68 b768 5168 6d6a  ...h.hsh.h.hQhmj
+00002810: 0501 0000 68bb 68cd 68b3 688b 8c2f 5051  ....h.h.h.h../PQ
+00002820: 416e 616c 7973 6973 2e69 6f2e 696e 7075  Analysis.io.inpu
+00002830: 745f 6669 6c65 5f72 6561 6465 722e 7071  t_file_reader.pq
+00002840: 2e6f 7574 7075 745f 6669 6c65 7394 6881  .output_files.h.
+00002850: 6895 68c7 6877 68bd 68d7 68a9 68a7 68df  h.h.hwh.h.h.h.h.
+00002860: 6841 689f 6a03 0100 0068 8768 d968 e96a  hAh.j....h.h.h.j
+00002870: 1101 0000 6837 682d 908c 1050 5141 6e61  ....h7h-...PQAna
+00002880: 6c79 7369 732e 7479 7065 7394 8f94 2868  lysis.types...(h
+00002890: ab68 b568 3968 d56a 1b01 0000 68a3 6a11  .h.h9h.j....h.j.
+000028a0: 0100 0068 5168 cf68 4368 8d6a 4a01 0000  ...hQh.hCh.jJ...
+000028b0: 68bb 6a05 0100 0068 b168 b368 ad68 6f8c  h.j....h.h.h.ho.
+000028c0: 3c50 5141 6e61 6c79 7369 732e 696f 2e69  <PQAnalysis.io.i
+000028d0: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
+000028e0: 2e70 715f 616e 616c 7973 6973 2e5f 706f  .pq_analysis._po
+000028f0: 7369 7469 6f6e 735f 6d69 7869 6e94 8c2d  sitions_mixin..-
+00002900: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
+00002910: 635f 7379 7374 656d 2e5f 7374 616e 6461  c_system._standa
+00002920: 7264 5f70 726f 7065 7274 6965 7394 68a1  rd_properties.h.
+00002930: 6877 68e7 68a9 68a7 6899 6a46 0100 006a  hwh.h.h.h.jF...j
+00002940: 4701 0000 6a03 0100 0068 8768 8f68 456a  G...j....h.h.hEj
+00002950: 4001 0000 68f7 682d 908c 1750 5141 6e61  @...h.h-...PQAna
+00002960: 6c79 7369 732e 7574 696c 732e 636f 6d6d  lysis.utils.comm
+00002970: 6f6e 948f 9428 8c10 5051 416e 616c 7973  on...(..PQAnalys
+00002980: 6973 2e75 7469 6c73 9468 6990 8c1b 5051  is.utils.hi...PQ
+00002990: 416e 616c 7973 6973 2e75 7469 6c73 2e64  Analysis.utils.d
+000029a0: 6563 6f72 6174 6f72 7394 8f94 286a 5a01  ecorators...(jZ.
+000029b0: 0000 908c 1350 5141 6e61 6c79 7369 732e  .....PQAnalysis.
+000029c0: 5f76 6572 7369 6f6e 948f 9428 6835 6869  _version...(h5hi
+000029d0: 908c 1050 5141 6e61 6c79 7369 732e 7574  ...PQAnalysis.ut
+000029e0: 696c 7394 8f94 2868 4368 c98c 0e50 5141  ils...(hCh...PQA
+000029f0: 6e61 6c79 7369 732e 636c 6994 6845 6837  nalysis.cli.hEh7
+00002a00: 908c 1750 5141 6e61 6c79 7369 732e 616e  ...PQAnalysis.an
+00002a10: 616c 7973 6973 2e72 6466 948f 9428 8c13  alysis.rdf...(..
+00002a20: 5051 416e 616c 7973 6973 2e61 6e61 6c79  PQAnalysis.analy
+00002a30: 7369 7394 908c 1b50 5141 6e61 6c79 7369  sis....PQAnalysi
+00002a40: 732e 616e 616c 7973 6973 2e72 6466 2e72  s.analysis.rdf.r
+00002a50: 6466 948f 9428 6843 6a64 0100 0068 5368  df...(hCjd...hSh
+00002a60: 498c 1750 5141 6e61 6c79 7369 732e 616e  I..PQAnalysis.an
+00002a70: 616c 7973 6973 2e72 6466 9490 8c0d 5051  alysis.rdf....PQ
+00002a80: 416e 616c 7973 6973 2e69 6f94 8f94 2868  Analysis.io...(h
+00002a90: 4368 6b68 5768 4768 5b68 a968 e76a 1b01  ChkhWhGh[h.h.j..
+00002aa0: 0000 68a3 6865 6851 6845 6861 6863 6849  ..h.hehQhEhahchI
+00002ab0: 908c 1850 5141 6e61 6c79 7369 732e 7479  ...PQAnalysis.ty
+00002ac0: 7065 5f63 6865 636b 696e 6794 8f94 2868  pe_checking...(h
+00002ad0: ab68 ed68 f16a 3d01 0000 68b5 6a1b 0100  .h.h.j=...h.j...
+00002ae0: 0068 a368 5168 cf68 4368 8d68 978c 1e50  .h.hQh.hCh.h...P
+00002af0: 5141 6e61 6c79 7369 732e 696f 2e72 6573  QAnalysis.io.res
+00002b00: 7461 7274 5f66 696c 652e 6170 6994 6a4a  tart_file.api.jJ
+00002b10: 0100 0068 bb68 4768 b168 b368 c968 8568  ...h.hGh.h.h.h.h
+00002b20: 6f68 c368 9568 c76a 5701 0000 68a1 6877  oh.h.h.jW...h.hw
+00002b30: 68bd 68d7 684f 8c1a 5051 416e 616c 7973  h.h.hO..PQAnalys
+00002b40: 6973 2e69 6f2e 6765 6e5f 6669 6c65 2e61  is.io.gen_file.a
+00002b50: 7069 9468 e768 a968 cb68 a768 df68 eb68  pi.h.h.h.h.h.h.h
+00002b60: 996a 4601 0000 68e3 68bf 6887 688f 68d1  .jF...h.h.h.h.h.
+00002b70: 6845 6849 6a40 0100 0068 f790 8c09 7471  hEhIj@...h....tq
+00002b80: 646d 2e61 7574 6f94 8f94 2868 4568 d790  dm.auto...(hEh..
+00002b90: 8c0f 5051 416e 616c 7973 6973 2e63 6f72  ..PQAnalysis.cor
+00002ba0: 6594 8f94 286a 6c01 0000 6a57 0100 0068  e...(jl...jW...h
+00002bb0: a168 776a 4701 0000 68d7 68bf 6887 6a3d  .hwjG...h.h.h.j=
+00002bc0: 0100 0068 cb68 d568 a768 8568 4568 cf6a  ...h.h.h.h.hEh.j
+00002bd0: 4001 0000 68f7 6a46 0100 0090 8c0f 5051  @...h.jF......PQ
+00002be0: 416e 616c 7973 6973 2e74 7261 6a94 8f94  Analysis.traj...
+00002bf0: 286a 3d01 0000 68d5 6a1b 0100 0068 a368  (j=...h.j....h.h
+00002c00: 5168 cf6a 6c01 0000 68c9 6869 68c3 68c7  Qh.jl...h.hih.h.
+00002c10: 68d7 68bd 684f 68a9 68bf 68d1 6845 6849  h.h.hOh.h.h.hEhI
+00002c20: 68f7 908c 1350 5141 6e61 6c79 7369 732e  h....PQAnalysis.
+00002c30: 746f 706f 6c6f 6779 948f 9428 6a57 0100  topology...(jW..
+00002c40: 0068 ed68 7768 d768 f16a 3d01 0000 6887  .h.hwh.h.j=...h.
+00002c50: 68d5 68d1 6845 6849 68eb 6a46 0100 0090  h.h.hEhIh.jF....
+00002c60: 8c0a 5051 416e 616c 7973 6973 948f 9428  ..PQAnalysis...(
+00002c70: 68b9 68ed 68f1 6a3d 0100 006a 3e01 0000  h.h.h.j=...j>...
+00002c80: 68d5 6a1b 0100 006a 1101 0000 6851 6897  h.j....j....hQh.
+00002c90: 6a05 0100 0068 bb68 4768 b368 c968 6f68  j....h.hGh.h.hoh
+00002ca0: c36a 3f01 0000 6895 68c7 68a1 6877 68bd  .j?...h.h.h.hwh.
+00002cb0: 68d7 68a9 68cb 68a7 68df 6883 6a03 0100  h.h.h.h.h.h.j...
+00002cc0: 0068 8768 8f68 456a 4001 0000 68f7 908c  .h.h.hEj@...h...
+00002cd0: 2250 5141 6e61 6c79 7369 732e 616e 616c  "PQAnalysis.anal
+00002ce0: 7973 6973 2e72 6466 2e65 7863 6570 7469  ysis.rdf.excepti
+00002cf0: 6f6e 7394 8f94 286a 6701 0000 6845 908c  ons...(jg...hE..
+00002d00: 2a50 5141 6e61 6c79 7369 732e 696f 2e69  *PQAnalysis.io.i
+00002d10: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
+00002d20: 2e65 7863 6570 7469 6f6e 7394 8f94 2868  .exceptions...(h
+00002d30: ff6a 3f01 0000 6847 6a05 0100 0090 8c2d  .j?...hGj......-
+00002d40: 5051 416e 616c 7973 6973 2e61 6e61 6c79  PQAnalysis.analy
+00002d50: 7369 732e 7264 662e 7264 665f 696e 7075  sis.rdf.rdf_inpu
+00002d60: 745f 6669 6c65 5f72 6561 6465 7294 8f94  t_file_reader...
+00002d70: 286a 6701 0000 6853 6849 908c 2e50 5141  (jg...hShI...PQA
+00002d80: 6e61 6c79 7369 732e 616e 616c 7973 6973  nalysis.analysis
+00002d90: 2e72 6466 2e72 6466 5f6f 7574 7075 745f  .rdf.rdf_output_
+00002da0: 6669 6c65 5f77 7269 7465 7294 8f94 286a  file_writer...(j
+00002db0: 6701 0000 6849 908c 1b50 5141 6e61 6c79  g...hI...PQAnaly
+00002dc0: 7369 732e 616e 616c 7973 6973 2e72 6466  sis.analysis.rdf
+00002dd0: 2e61 7069 948f 9428 6a67 0100 0090 8c21  .api...(jg.....!
+00002de0: 5051 416e 616c 7973 6973 2e74 6f6f 6c73  PQAnalysis.tools
+00002df0: 2e74 7261 6a5f 746f 5f63 6f6d 5f74 7261  .traj_to_com_tra
+00002e00: 6a94 8f94 288c 1050 5141 6e61 6c79 7369  j...(..PQAnalysi
+00002e10: 732e 746f 6f6c 7394 908c 1550 5141 6e61  s.tools....PQAna
+00002e20: 6c79 7369 732e 696f 2e66 6f72 6d61 7473  lysis.io.formats
+00002e30: 948f 9428 68c7 685d 68f1 68eb 68bf 6a6d  ...(h.h]h.h.h.jm
+00002e40: 0100 006a 3e01 0000 8c0d 5051 416e 616c  ...j>.....PQAnal
+00002e50: 7973 6973 2e69 6f94 68c9 68d1 6851 68cf  ysis.io.h.h.hQh.
+00002e60: 68df 68f7 6869 908c 1850 5141 6e61 6c79  h.h.hi...PQAnaly
+00002e70: 7369 732e 6174 6f6d 6963 5f73 7973 7465  sis.atomic_syste
+00002e80: 6d94 8f94 286a 6c01 0000 68c7 68d7 6a3d  m...(jl...h.h.j=
+00002e90: 0100 0068 876a 6d01 0000 68d5 68d1 6a1b  ...h.jm...h.h.j.
+00002ea0: 0100 0068 5168 cf68 df6a 4001 0000 68f7  ...hQh.h.j@...h.
+00002eb0: 908c 1f50 5141 6e61 6c79 7369 732e 636c  ...PQAnalysis.cl
+00002ec0: 692e 5f61 7267 756d 656e 745f 7061 7273  i._argument_pars
+00002ed0: 6572 948f 9428 686b 6855 685d 6857 685b  er...(hkhUh]hWh[
+00002ee0: 6853 6865 6867 6861 6863 908c 1850 5141  hShehghahc...PQA
+00002ef0: 6e61 6c79 7369 732e 636c 692e 5f63 6c69  nalysis.cli._cli
+00002f00: 5f62 6173 6594 8f94 2868 6b68 5568 5d68  _base...(hkhUh]h
+00002f10: 5768 5b68 5368 6568 6168 6390 8c1c 5051  Wh[hShehahc...PQ
+00002f20: 416e 616c 7973 6973 2e69 6f2e 6e65 702e  Analysis.io.nep.
+00002f30: 6e65 705f 7772 6974 6572 948f 9428 6855  nep_writer...(hU
+00002f40: 908c 1d50 5141 6e61 6c79 7369 732e 746f  ...PQAnalysis.to
+00002f50: 6f6c 732e 6164 645f 6d6f 6c65 6375 6c65  ols.add_molecule
+00002f60: 948f 9428 685d 908c 1650 5141 6e61 6c79  ...(h]...PQAnaly
+00002f70: 7369 732e 636c 692e 7879 7a32 6765 6e94  sis.cli.xyz2gen.
+00002f80: 8f94 2868 6790 8c19 5051 416e 616c 7973  ..(hg...PQAnalys
+00002f90: 6973 2e63 6c69 2e74 7261 6a32 716d 6366  is.cli.traj2qmcf
+00002fa0: 6394 8f94 2868 6790 8c17 5051 416e 616c  c...(hg...PQAnal
+00002fb0: 7973 6973 2e63 6c69 2e74 7261 6a32 626f  ysis.cli.traj2bo
+00002fc0: 7894 8f94 2868 6790 8c16 5051 416e 616c  x...(hg...PQAnal
+00002fd0: 7973 6973 2e63 6c69 2e72 7374 3278 797a  ysis.cli.rst2xyz
+00002fe0: 948f 9428 6867 908c 1250 5141 6e61 6c79  ...(hg...PQAnaly
+00002ff0: 7369 732e 636c 692e 7264 6694 8f94 2868  sis.cli.rdf...(h
+00003000: 6790 8c16 5051 416e 616c 7973 6973 2e63  g...PQAnalysis.c
+00003010: 6c69 2e67 656e 3278 797a 948f 9428 6867  li.gen2xyz...(hg
+00003020: 908c 1d50 5141 6e61 6c79 7369 732e 636c  ...PQAnalysis.cl
+00003030: 692e 636f 6e74 696e 7565 5f69 6e70 7574  i.continue_input
+00003040: 948f 9428 6867 908c 1c50 5141 6e61 6c79  ...(hg...PQAnaly
+00003050: 7369 732e 636c 692e 6164 645f 6d6f 6c65  sis.cli.add_mole
+00003060: 6375 6c65 7394 8f94 2868 6790 8c1d 5051  cules...(hg...PQ
+00003070: 416e 616c 7973 6973 2e63 6c69 2e62 7569  Analysis.cli.bui
+00003080: 6c64 5f6e 6570 5f74 7261 6a94 8f94 2868  ld_nep_traj...(h
+00003090: 6790 8c0b 6172 6763 6f6d 706c 6574 6594  g...argcomplete.
+000030a0: 8f94 2868 6990 8c0d 7269 6368 5f61 7267  ..(hi...rich_arg
+000030b0: 7061 7273 6594 8f94 2868 6990 8c23 5051  parse...(hi..#PQ
+000030c0: 416e 616c 7973 6973 2e70 6879 7369 6361  Analysis.physica
+000030d0: 6c5f 6461 7461 2e65 7863 6570 7469 6f6e  l_data.exception
+000030e0: 7394 8f94 288c 1850 5141 6e61 6c79 7369  s...(..PQAnalysi
+000030f0: 732e 7068 7973 6963 616c 5f64 6174 6194  s.physical_data.
+00003100: 686f 908c 1f50 5141 6e61 6c79 7369 732e  ho...PQAnalysis.
+00003110: 7068 7973 6963 616c 5f64 6174 612e 656e  physical_data.en
+00003120: 6572 6779 948f 9428 6aaa 0100 0090 8c23  ergy...(j......#
+00003130: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
+00003140: 635f 7379 7374 656d 2e65 7863 6570 7469  c_system.excepti
+00003150: 6f6e 7394 8f94 286a 4701 0000 6875 8c18  ons...(jG...hu..
+00003160: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
+00003170: 635f 7379 7374 656d 9468 7790 8c17 7363  c_system.hw...sc
+00003180: 6970 792e 7370 6174 6961 6c2e 7472 616e  ipy.spatial.tran
+00003190: 7366 6f72 6d94 8f94 2868 7790 8c17 5051  sform...(hw...PQ
+000031a0: 416e 616c 7973 6973 2e75 7469 6c73 2e72  Analysis.utils.r
+000031b0: 616e 646f 6d94 8f94 286a 1b01 0000 6877  andom...(j....hw
+000031c0: 908c 1550 5141 6e61 6c79 7369 732e 7574  ...PQAnalysis.ut
+000031d0: 696c 732e 6d61 7468 948f 9428 6899 6877  ils.math...(h.hw
+000031e0: 908c 2450 5141 6e61 6c79 7369 732e 6174  ..$PQAnalysis.at
+000031f0: 6f6d 6963 5f73 7973 7465 6d2e 5f70 726f  omic_system._pro
+00003200: 7065 7274 6965 7394 8f94 2868 7790 8c2d  perties...(hw..-
+00003210: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
+00003220: 635f 7379 7374 656d 2e5f 7374 616e 6461  c_system._standa
+00003230: 7264 5f70 726f 7065 7274 6965 7394 8f94  rd_properties...
+00003240: 2868 7790 8c23 5051 416e 616c 7973 6973  (hw..#PQAnalysis
+00003250: 2e61 746f 6d69 635f 7379 7374 656d 2e5f  .atomic_system._
+00003260: 706f 7369 7469 6f6e 7394 8f94 2868 7790  positions...(hw.
+00003270: 8c26 5051 416e 616c 7973 6973 2e61 746f  .&PQAnalysis.ato
+00003280: 6d69 635f 7379 7374 656d 2e61 746f 6d69  mic_system.atomi
+00003290: 635f 7379 7374 656d 948f 9428 6aaf 0100  c_system...(j...
+000032a0: 0090 8c24 5051 416e 616c 7973 6973 2e61  ...$PQAnalysis.a
+000032b0: 746f 6d69 635f 7379 7374 656d 2e5f 6465  tomic_system._de
+000032c0: 636f 7261 746f 7273 948f 9428 6a47 0100  corators...(jG..
+000032d0: 006a 5701 0000 6a46 0100 0090 8c12 5051  .jW...jF......PQ
+000032e0: 416e 616c 7973 6973 2e66 6f72 6d61 7473  Analysis.formats
+000032f0: 948f 9428 68ff 6883 68b9 908c 1a50 5141  ...(h.h.h....PQA
+00003300: 6e61 6c79 7369 732e 7472 616a 2e65 7863  nalysis.traj.exc
+00003310: 6570 7469 6f6e 7394 8f94 2868 838c 0f50  eptions...(h...P
+00003320: 5141 6e61 6c79 7369 732e 7472 616a 9490  QAnalysis.traj..
+00003330: 8c17 5051 416e 616c 7973 6973 2e74 7261  ..PQAnalysis.tra
+00003340: 6a2e 666f 726d 6174 7394 8f94 286a c401  j.formats...(j..
+00003350: 0000 908c 1a50 5141 6e61 6c79 7369 732e  .....PQAnalysis.
+00003360: 7472 616a 2e74 7261 6a65 6374 6f72 7994  traj.trajectory.
+00003370: 8f94 286a c401 0000 9068 858f 9428 6ac4  ..(j.....h...(j.
+00003380: 0100 0090 8c14 5051 416e 616c 7973 6973  ......PQAnalysis
+00003390: 2e63 6f72 652e 6365 6c6c 948f 9428 688d  .core.cell...(h.
+000033a0: 8c0f 5051 416e 616c 7973 6973 2e63 6f72  ..PQAnalysis.cor
+000033b0: 6594 908c 1450 5141 6e61 6c79 7369 732e  e....PQAnalysis.
+000033c0: 636f 7265 2e61 746f 6d94 8f94 286a cc01  core.atom...(j..
+000033d0: 0000 688f 908c 1a50 5141 6e61 6c79 7369  ..h....PQAnalysi
+000033e0: 732e 636f 7265 2e65 7863 6570 7469 6f6e  s.core.exception
+000033f0: 7394 8f94 2868 9768 9568 a168 8f6a cc01  s...(h.h.h.h.j..
+00003400: 0000 908c 1750 5141 6e61 6c79 7369 732e  .....PQAnalysis.
+00003410: 636f 7265 2e72 6573 6964 7565 948f 9428  core.residue...(
+00003420: 6acc 0100 0090 8c13 5051 416e 616c 7973  j.......PQAnalys
+00003430: 6973 2e63 6f72 652e 6170 6994 8f94 286a  is.core.api...(j
+00003440: cc01 0000 908c 1c50 5141 6e61 6c79 7369  .......PQAnalysi
+00003450: 732e 636f 7265 2e61 746f 6d2e 656c 656d  s.core.atom.elem
+00003460: 656e 7494 8f94 2868 958c 1450 5141 6e61  ent...(h...PQAna
+00003470: 6c79 7369 732e 636f 7265 2e61 746f 6d94  lysis.core.atom.
+00003480: 908c 1950 5141 6e61 6c79 7369 732e 636f  ...PQAnalysis.co
+00003490: 7265 2e61 746f 6d2e 6174 6f6d 948f 9428  re.atom.atom...(
+000034a0: 6ad7 0100 0090 8c29 5051 416e 616c 7973  j......)PQAnalys
+000034b0: 6973 2e63 6f72 652e 6365 6c6c 2e5f 7374  is.core.cell._st
+000034c0: 616e 6461 7264 5f70 726f 7065 7274 6965  andard_propertie
+000034d0: 7394 8f94 2868 9990 8c19 5051 416e 616c  s...(h....PQAnal
+000034e0: 7973 6973 2e63 6f72 652e 6365 6c6c 2e63  ysis.core.cell.c
+000034f0: 656c 6c94 8f94 288c 1450 5141 6e61 6c79  ell...(..PQAnaly
+00003500: 7369 732e 636f 7265 2e63 656c 6c94 908c  sis.core.cell...
+00003510: 1e50 5141 6e61 6c79 7369 732e 746f 706f  .PQAnalysis.topo
+00003520: 6c6f 6779 2e65 7863 6570 7469 6f6e 7394  logy.exceptions.
+00003530: 8f94 288c 1350 5141 6e61 6c79 7369 732e  ..(..PQAnalysis.
+00003540: 746f 706f 6c6f 6779 9468 a190 8c33 5051  topology.h...3PQ
+00003550: 416e 616c 7973 6973 2e74 6f70 6f6c 6f67  Analysis.topolog
+00003560: 792e 626f 6e64 6564 5f74 6f70 6f6c 6f67  y.bonded_topolog
+00003570: 792e 626f 6e64 6564 5f74 6f70 6f6c 6f67  y.bonded_topolog
+00003580: 7994 8f94 286a e101 0000 68a1 908c 1d50  y...(j....h....P
+00003590: 5141 6e61 6c79 7369 732e 746f 706f 6c6f  QAnalysis.topolo
+000035a0: 6779 2e73 656c 6563 7469 6f6e 948f 9428  gy.selection...(
+000035b0: 68a3 6ae1 0100 0068 a990 8c22 5051 416e  h.j....h..."PQAn
+000035c0: 616c 7973 6973 2e74 6f70 6f6c 6f67 792e  alysis.topology.
+000035d0: 7368 616b 655f 746f 706f 6c6f 6779 948f  shake_topology..
+000035e0: 9428 68a3 908c 2850 5141 6e61 6c79 7369  .(h...(PQAnalysi
+000035f0: 732e 746f 706f 6c6f 6779 2e62 6f6e 6465  s.topology.bonde
+00003600: 645f 746f 706f 6c6f 6779 2e62 6f6e 6494  d_topology.bond.
+00003610: 8f94 286a e101 0000 68ad 68b3 908c 2950  ..(j....h.h...)P
+00003620: 5141 6e61 6c79 7369 732e 746f 706f 6c6f  QAnalysis.topolo
+00003630: 6779 2e62 6f6e 6465 645f 746f 706f 6c6f  gy.bonded_topolo
+00003640: 6779 2e61 6e67 6c65 948f 9428 6ae1 0100  gy.angle...(j...
+00003650: 0068 ad68 b390 8c2c 5051 416e 616c 7973  .h.h...,PQAnalys
+00003660: 6973 2e74 6f70 6f6c 6f67 792e 626f 6e64  is.topology.bond
+00003670: 6564 5f74 6f70 6f6c 6f67 792e 6469 6865  ed_topology.dihe
+00003680: 6472 616c 948f 9428 6ae1 0100 0068 ad68  dral...(j....h.h
+00003690: b390 8c1c 5051 416e 616c 7973 6973 2e74  ....PQAnalysis.t
+000036a0: 6f70 6f6c 6f67 792e 746f 706f 6c6f 6779  opology.topology
+000036b0: 948f 9428 68a7 6ae1 0100 0090 8c04 6c61  ...(h.j.......la
+000036c0: 726b 948f 9428 6a03 0100 0068 a790 8c38  rk...(j....h...8
+000036d0: 5051 416e 616c 7973 6973 2e74 6f70 6f6c  PQAnalysis.topol
+000036e0: 6f67 792e 626f 6e64 6564 5f74 6f70 6f6c  ogy.bonded_topol
+000036f0: 6f67 792e 5f74 6f70 6f6c 6f67 795f 7072  ogy._topology_pr
+00003700: 6f70 6572 7469 6573 948f 9428 68b3 908c  operties...(h...
+00003710: 1850 5141 6e61 6c79 7369 732e 696f 2e65  .PQAnalysis.io.e
+00003720: 7863 6570 7469 6f6e 7394 8f94 2868 cb68  xceptions...(h.h
+00003730: b96a 3e01 0000 68c9 908c 1f50 5141 6e61  .j>...h....PQAna
+00003740: 6c79 7369 732e 696f 2e69 6e70 7574 5f66  lysis.io.input_f
+00003750: 696c 655f 7265 6164 6572 948f 9428 6a87  ile_reader...(j.
+00003760: 0100 0068 bb90 8c27 5051 416e 616c 7973  ...h...'PQAnalys
+00003770: 6973 2e69 6f2e 696e 7075 745f 6669 6c65  is.io.input_file
+00003780: 5f72 6561 6465 722e 666f 726d 6174 7394  _reader.formats.
+00003790: 8f94 286a 3f01 0000 68bb 6a03 0100 008c  ..(j?...h.j.....
+000037a0: 1f50 5141 6e61 6c79 7369 732e 696f 2e69  .PQAnalysis.io.i
+000037b0: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
+000037c0: 946a 1101 0000 908c 1850 5141 6e61 6c79  .j.......PQAnaly
+000037d0: 7369 732e 7068 7973 6963 616c 5f64 6174  sis.physical_dat
+000037e0: 6194 8f94 2868 bd90 8c12 5051 416e 616c  a...(h....PQAnal
+000037f0: 7973 6973 2e69 6f2e 6261 7365 948f 9428  ysis.io.base...(
+00003800: 68c3 68ed 68f1 68d7 68bd 6a03 0100 006a  h.h.h.h.h.j....j
+00003810: 3d01 0000 6a87 0100 0068 c968 cb68 cf68  =...j....h.h.h.h
+00003820: df6a 4001 0000 68f7 908c 1e50 5141 6e61  .j@...h....PQAna
+00003830: 6c79 7369 732e 696f 2e69 6e66 6f5f 6669  lysis.io.info_fi
+00003840: 6c65 5f72 6561 6465 7294 8f94 2868 bd6a  le_reader...(h.j
+00003850: 8701 0000 908c 1750 5141 6e61 6c79 7369  .......PQAnalysi
+00003860: 732e 696f 2e74 7261 6a5f 6669 6c65 948f  s.io.traj_file..
+00003870: 9428 68d1 68bf 908c 1850 5141 6e61 6c79  .(h.h....PQAnaly
+00003880: 7369 732e 696f 2e62 6f78 5f77 7269 7465  sis.io.box_write
+00003890: 7294 8f94 2868 bf68 c76a 8701 0000 908c  r...(h.h.j......
+000038a0: 1650 5141 6e61 6c79 7369 732e 696f 2e67  .PQAnalysis.io.g
+000038b0: 656e 5f66 696c 6594 8f94 2868 bf90 8c1e  en_file...(h....
+000038c0: 5051 416e 616c 7973 6973 2e69 6f2e 7265  PQAnalysis.io.re
+000038d0: 7374 6172 745f 6669 6c65 2e61 7069 948f  start_file.api..
+000038e0: 9428 68bf 6a87 0100 0090 8c1b 5051 416e  .(h.j.......PQAn
+000038f0: 616c 7973 6973 2e69 6f2e 7472 616a 5f66  alysis.io.traj_f
+00003900: 696c 652e 6170 6994 8f94 2868 bf68 c76a  ile.api...(h.h.j
+00003910: 8701 0000 908c 2250 5141 6e61 6c79 7369  ......"PQAnalysi
+00003920: 732e 696f 2e6d 6f6c 6465 7363 7269 7074  s.io.moldescript
+00003930: 6f72 5f72 6561 6465 7294 8f94 286a 3d01  or_reader...(j=.
+00003940: 0000 6a87 0100 0090 8c29 5051 416e 616c  ..j......)PQAnal
+00003950: 7973 6973 2e69 6f2e 7265 7374 6172 745f  ysis.io.restart_
+00003960: 6669 6c65 2e72 6573 7461 7274 5f77 7269  file.restart_wri
+00003970: 7465 7294 8f94 288c 1a50 5141 6e61 6c79  ter...(..PQAnaly
+00003980: 7369 732e 696f 2e72 6573 7461 7274 5f66  sis.io.restart_f
+00003990: 696c 6594 6a87 0100 0090 8c29 5051 416e  ile.j......)PQAn
+000039a0: 616c 7973 6973 2e69 6f2e 7265 7374 6172  alysis.io.restar
+000039b0: 745f 6669 6c65 2e72 6573 7461 7274 5f72  t_file.restart_r
+000039c0: 6561 6465 7294 8f94 286a 6c01 0000 6a0f  eader...(jl...j.
+000039d0: 0200 006a 8701 0000 908c 2950 5141 6e61  ...j......)PQAna
+000039e0: 6c79 7369 732e 696f 2e74 7261 6a5f 6669  lysis.io.traj_fi
+000039f0: 6c65 2e74 7261 6a65 6374 6f72 795f 7265  le.trajectory_re
+00003a00: 6164 6572 948f 9428 8c17 5051 416e 616c  ader...(..PQAnal
+00003a10: 7973 6973 2e69 6f2e 7472 616a 5f66 696c  ysis.io.traj_fil
+00003a20: 6594 6a87 0100 0090 8c29 5051 416e 616c  e.j......)PQAnal
+00003a30: 7973 6973 2e69 6f2e 7472 616a 5f66 696c  ysis.io.traj_fil
+00003a40: 652e 7472 616a 6563 746f 7279 5f77 7269  e.trajectory_wri
+00003a50: 7465 7294 8f94 286a 1402 0000 6a87 0100  ter...(j....j...
+00003a60: 0090 8c24 5051 416e 616c 7973 6973 2e69  ...$PQAnalysis.i
+00003a70: 6f2e 7472 616a 5f66 696c 652e 6672 616d  o.traj_file.fram
+00003a80: 655f 7265 6164 6572 948f 9428 6a14 0200  e_reader...(j...
+00003a90: 006a 8701 0000 68d7 908c 2650 5141 6e61  .j....h...&PQAna
+00003aa0: 6c79 7369 732e 696f 2e67 656e 5f66 696c  lysis.io.gen_fil
+00003ab0: 652e 6765 6e5f 6669 6c65 5f72 6561 6465  e.gen_file_reade
+00003ac0: 7294 8f94 288c 1650 5141 6e61 6c79 7369  r...(..PQAnalysi
+00003ad0: 732e 696f 2e67 656e 5f66 696c 6594 6a6d  s.io.gen_file.jm
+00003ae0: 0100 006a 8701 0000 908c 2650 5141 6e61  ...j......&PQAna
+00003af0: 6c79 7369 732e 696f 2e67 656e 5f66 696c  lysis.io.gen_fil
+00003b00: 652e 6765 6e5f 6669 6c65 5f77 7269 7465  e.gen_file_write
+00003b10: 7294 8f94 286a 1b02 0000 6a6d 0100 006a  r...(j....jm...j
+00003b20: 8701 0000 908c 1a50 5141 6e61 6c79 7369  .......PQAnalysi
+00003b30: 732e 696f 2e67 656e 5f66 696c 652e 6170  s.io.gen_file.ap
+00003b40: 6994 8f94 286a 1b02 0000 6a87 0100 0090  i...(j....j.....
+00003b50: 8c1b 5051 416e 616c 7973 6973 2e69 6f2e  ..PQAnalysis.io.
+00003b60: 746f 706f 6c6f 6779 5f66 696c 6594 8f94  topology_file...
+00003b70: 286a 8701 0000 908c 1f50 5141 6e61 6c79  (j.......PQAnaly
+00003b80: 7369 732e 696f 2e74 6f70 6f6c 6f67 795f  sis.io.topology_
+00003b90: 6669 6c65 2e61 7069 948f 9428 6a87 0100  file.api...(j...
+00003ba0: 0090 8c20 5051 416e 616c 7973 6973 2e69  ... PQAnalysis.i
+00003bb0: 6f2e 656e 6572 6779 5f66 696c 655f 7265  o.energy_file_re
+00003bc0: 6164 6572 948f 9428 6a87 0100 0090 8c11  ader...(j.......
+00003bd0: 5051 416e 616c 7973 6973 2e69 6f2e 6170  PQAnalysis.io.ap
+00003be0: 6994 8f94 286a 8701 0000 908c 1c50 5141  i...(j.......PQA
+00003bf0: 6e61 6c79 7369 732e 696f 2e63 6f6e 7665  nalysis.io.conve
+00003c00: 7273 696f 6e5f 6170 6994 8f94 286a 8701  rsion_api...(j..
+00003c10: 0000 908c 1750 5141 6e61 6c79 7369 732e  .....PQAnalysis.
+00003c20: 696f 2e77 7269 7465 5f61 7069 948f 9428  io.write_api...(
+00003c30: 6a87 0100 0090 8c22 5051 416e 616c 7973  j......"PQAnalys
+00003c40: 6973 2e69 6f2e 7472 616a 5f66 696c 652e  is.io.traj_file.
+00003c50: 6578 6365 7074 696f 6e73 948f 9428 68d7  exceptions...(h.
+00003c60: 68d5 908c 2150 5141 6e61 6c79 7369 732e  h...!PQAnalysis.
+00003c70: 696f 2e67 656e 5f66 696c 652e 6578 6365  io.gen_file.exce
+00003c80: 7074 696f 6e73 948f 9428 6a40 0100 0090  ptions...(j@....
+00003c90: 8c22 5051 416e 616c 7973 6973 2e69 6f2e  ."PQAnalysis.io.
+00003ca0: 7669 7269 616c 2e76 6972 6961 6c5f 7265  virial.virial_re
+00003cb0: 6164 6572 948f 9428 8c14 5051 416e 616c  ader...(..PQAnal
+00003cc0: 7973 6973 2e69 6f2e 7669 7269 616c 9468  ysis.io.virial.h
+00003cd0: e390 8c30 5051 416e 616c 7973 6973 2e69  ...0PQAnalysis.i
+00003ce0: 6f2e 746f 706f 6c6f 6779 5f66 696c 652e  o.topology_file.
+00003cf0: 746f 706f 6c6f 6779 5f66 696c 655f 7772  topology_file_wr
+00003d00: 6974 6572 948f 9428 8c1b 5051 416e 616c  iter...(..PQAnal
+00003d10: 7973 6973 2e69 6f2e 746f 706f 6c6f 6779  ysis.io.topology
+00003d20: 5f66 696c 6594 68eb 908c 3050 5141 6e61  _file.h...0PQAna
+00003d30: 6c79 7369 732e 696f 2e74 6f70 6f6c 6f67  lysis.io.topolog
+00003d40: 795f 6669 6c65 2e74 6f70 6f6c 6f67 795f  y_file.topology_
+00003d50: 6669 6c65 5f72 6561 6465 7294 8f94 286a  file_reader...(j
+00003d60: 3502 0000 68eb 908c 2650 5141 6e61 6c79  5...h...&PQAnaly
+00003d70: 7369 732e 696f 2e74 6f70 6f6c 6f67 795f  sis.io.topology_
+00003d80: 6669 6c65 2e65 7863 6570 7469 6f6e 7394  file.exceptions.
+00003d90: 8f94 2868 ed68 f190 8c25 5051 416e 616c  ..(h.h...%PQAnal
+00003da0: 7973 6973 2e69 6f2e 7265 7374 6172 745f  ysis.io.restart_
+00003db0: 6669 6c65 2e65 7863 6570 7469 6f6e 7394  file.exceptions.
+00003dc0: 8f94 286a 3d01 0000 68f7 908c 3150 5141  ..(j=...h...1PQA
+00003dd0: 6e61 6c79 7369 732e 696f 2e69 6e70 7574  nalysis.io.input
+00003de0: 5f66 696c 655f 7265 6164 6572 2e69 6e70  _file_reader.inp
+00003df0: 7574 5f66 696c 655f 7061 7273 6572 948f  ut_file_parser..
+00003e00: 9428 6afa 0100 006a 3f01 0000 6a11 0100  .(j....j?...j...
+00003e10: 006a 0501 0000 908c 2250 5141 6e61 6c79  .j......"PQAnaly
+00003e20: 7369 732e 696f 2e69 6e70 7574 5f66 696c  sis.io.input_fil
+00003e30: 655f 7265 6164 6572 2e70 7194 8f94 286a  e_reader.pq...(j
+00003e40: fa01 0000 908c 2b50 5141 6e61 6c79 7369  ......+PQAnalysi
+00003e50: 732e 696f 2e69 6e70 7574 5f66 696c 655f  s.io.input_file_
+00003e60: 7265 6164 6572 2e70 715f 616e 616c 7973  reader.pq_analys
+00003e70: 6973 948f 9428 6afa 0100 0090 8c48 5051  is...(j......HPQ
+00003e80: 416e 616c 7973 6973 2e69 6f2e 696e 7075  Analysis.io.inpu
+00003e90: 745f 6669 6c65 5f72 6561 6465 722e 7071  t_file_reader.pq
+00003ea0: 5f61 6e61 6c79 7369 732e 7071 616e 616c  _analysis.pqanal
+00003eb0: 7973 6973 5f69 6e70 7574 5f66 696c 655f  ysis_input_file_
+00003ec0: 7265 6164 6572 948f 9428 8c2b 5051 416e  reader...(.+PQAn
+00003ed0: 616c 7973 6973 2e69 6f2e 696e 7075 745f  alysis.io.input_
+00003ee0: 6669 6c65 5f72 6561 6465 722e 7071 5f61  file_reader.pq_a
+00003ef0: 6e61 6c79 7369 7394 908c 3750 5141 6e61  nalysis...7PQAna
+00003f00: 6c79 7369 732e 696f 2e69 6e70 7574 5f66  lysis.io.input_f
+00003f10: 696c 655f 7265 6164 6572 2e70 715f 616e  ile_reader.pq_an
+00003f20: 616c 7973 6973 2e5f 6669 6c65 5f6d 6978  alysis._file_mix
+00003f30: 696e 948f 9428 6a3f 0100 0090 8c3c 5051  in...(j?.....<PQ
+00003f40: 416e 616c 7973 6973 2e69 6f2e 696e 7075  Analysis.io.inpu
+00003f50: 745f 6669 6c65 5f72 6561 6465 722e 7071  t_file_reader.pq
+00003f60: 5f61 6e61 6c79 7369 732e 5f73 656c 6563  _analysis._selec
+00003f70: 7469 6f6e 5f6d 6978 696e 948f 9428 6a3f  tion_mixin...(j?
+00003f80: 0100 0090 8c3c 5051 416e 616c 7973 6973  .....<PQAnalysis
+00003f90: 2e69 6f2e 696e 7075 745f 6669 6c65 5f72  .io.input_file_r
+00003fa0: 6561 6465 722e 7071 5f61 6e61 6c79 7369  eader.pq_analysi
+00003fb0: 732e 5f70 6f73 6974 696f 6e73 5f6d 6978  s._positions_mix
+00003fc0: 696e 948f 9428 6a3f 0100 0090 8c32 5051  in...(j?.....2PQ
+00003fd0: 416e 616c 7973 6973 2e69 6f2e 696e 7075  Analysis.io.inpu
+00003fe0: 745f 6669 6c65 5f72 6561 6465 722e 7071  t_file_reader.pq
+00003ff0: 5f61 6e61 6c79 7369 732e 5f70 6172 7365  _analysis._parse
+00004000: 948f 9428 8c3c 5051 416e 616c 7973 6973  ...(.<PQAnalysis
+00004010: 2e69 6f2e 696e 7075 745f 6669 6c65 5f72  .io.input_file_r
+00004020: 6561 6465 722e 7071 5f61 6e61 6c79 7369  eader.pq_analysi
+00004030: 732e 5f73 656c 6563 7469 6f6e 5f6d 6978  s._selection_mix
+00004040: 696e 946a 5601 0000 6a45 0100 0090 8c2f  in.jV...jE...../
+00004050: 5051 416e 616c 7973 6973 2e69 6f2e 696e  PQAnalysis.io.in
+00004060: 7075 745f 6669 6c65 5f72 6561 6465 722e  put_file_reader.
+00004070: 7071 2e6f 7574 7075 745f 6669 6c65 7394  pq.output_files.
+00004080: 8f94 286a 1101 0000 908c 3750 5141 6e61  ..(j......7PQAna
+00004090: 6c79 7369 732e 696f 2e69 6e70 7574 5f66  lysis.io.input_f
+000040a0: 696c 655f 7265 6164 6572 2e70 712e 7071  ile_reader.pq.pq
+000040b0: 5f69 6e70 7574 5f66 696c 655f 7265 6164  _input_file_read
+000040c0: 6572 948f 9428 8c22 5051 416e 616c 7973  er...(."PQAnalys
+000040d0: 6973 2e69 6f2e 696e 7075 745f 6669 6c65  is.io.input_file
+000040e0: 5f72 6561 6465 722e 7071 9490 8c18 5051  _reader.pq....PQ
+000040f0: 416e 616c 7973 6973 2e69 6f2e 7669 7269  Analysis.io.viri
+00004100: 616c 2e61 7069 948f 9428 6a1b 0100 0090  al.api...(j.....
+00004110: 8c16 5051 416e 616c 7973 6973 2e75 7469  ..PQAnalysis.uti
+00004120: 6c73 2e75 6e69 7473 948f 9428 6a1b 0100  ls.units...(j...
+00004130: 0090 8c16 5051 416e 616c 7973 6973 2e75  ....PQAnalysis.u
+00004140: 7469 6c73 2e66 696c 6573 948f 9428 6a1b  tils.files...(j.
+00004150: 0100 0090 8c1c 5051 416e 616c 7973 6973  ......PQAnalysis
+00004160: 2e69 6f2e 6e65 702e 6578 6365 7074 696f  .io.nep.exceptio
+00004170: 6e73 948f 9428 6a1b 0100 0090 758c 1064  ns...(j.....u..d
+00004180: 7570 6c69 6361 7465 645f 6c69 6e65 7394  uplicated_lines.
+00004190: 7d94 288c 136e 625f 6475 706c 6963 6174  }.(..nb_duplicat
+000041a0: 6564 5f6c 696e 6573 944b 008c 1870 6572  ed_lines.K...per
+000041b0: 6365 6e74 5f64 7570 6c69 6361 7465 645f  cent_duplicated_
+000041c0: 6c69 6e65 7394 4700 0000 0000 0000 0075  lines.G........u
+000041d0: 8c0a 6e6f 6465 5f63 6f75 6e74 947d 9428  ..node_count.}.(
+000041e0: 680e 4b4c 6809 4b75 680f 4d12 0268 104b  h.KLh.Kuh.M..h.K
+000041f0: 7d75 8c0c 756e 646f 6375 6d65 6e74 6564  }u..undocumented
+00004200: 947d 9428 680e 4b00 6809 4b00 680f 4b00  .}.(h.K.h.K.h.K.
+00004210: 6810 4b00 7568 184b 0168 194b 1f68 1a4b  h.K.uh.K.h.K.h.K
+00004220: 0068 1b4b 0068 1c4b 3368 1d4d de11 681e  .h.K.h.K3h.M..h.
+00004230: 4b0a 8c0b 676c 6f62 616c 5f6e 6f74 6594  K...global_note.
+00004240: 4740 230d 18bc f320 936a 5d02 0000 4b1b  G@#.... .j]...K.
+00004250: 6a5e 0200 0047 3fc1 f1e2 2523 a31d 7562  j^...G?...%#..ub
+00004260: 2e                                       .
```

### Comparing `pqanalysis-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md` & `pqanalysis-1.0.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/.github/scripts/parse_pylint.py` & `pqanalysis-1.0.6/.github/scripts/parse_pylint.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/.github/workflows/ci.yml` & `pqanalysis-1.0.6/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     - name: Generate coverage report
       run: |
         bash pytest.sh
       shell: bash
 
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         env_vars: OS,PYTHON
         fail_ci_if_error: true
         flags: unittests
         verbose: true
```

### Comparing `pqanalysis-1.0.5/.github/workflows/docs.yml` & `pqanalysis-1.0.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/.github/workflows/pylint.yml` & `pqanalysis-1.0.6/.github/workflows/pylint.yml`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,20 @@
       - main
       - dev
   pull_request:
     branches:
       - '*'
   workflow_dispatch:
 
-permissions:
-  contents: read
-  pull-requests: write
-
 jobs:
   pylint:
 
     runs-on: ubuntu-latest
 
-    permissions:                # Job-level permissions configuration starts here
-      contents: write           # 'write' access to repository contents
-      pull-requests: write      # 'write' access to pull requests
+    permissions: write-all      # Job-level permissions configuration starts here
 
     steps:
     - uses: actions/checkout@master
       with:
         persist-credentials: false # otherwise, the token used is the GITHUB_TOKEN, instead of your personal access token.
         fetch-depth: 0 # otherwise, there would be errors pushing refs to the destination repository.
 
@@ -59,18 +53,18 @@
     - name: Check if pylint score is higher than 9.75
       id: check_pylint_score
       run: |
         head -n3 comment.txt | tail -n 1
         head -n3 comment.txt | tail -n 1 | awk '{print $7}'
         head -n3 comment.txt | tail -n 1 | awk '{print $7}' | cut -d '/' -f 1
         score=$(head -n3 comment.txt | tail -n 1 | awk '{print $7}' | cut -d '/' -f 1)
-        if (( $(echo "$score > 9.75" | bc -l) )); then
-          echo "Pylint score is higher than 9.75 and is $score"
+        if (( $(echo "$score > 9.5" | bc -l) )); then
+          echo "Pylint score is higher than 9.5 and is $score"
         else
-          echo "Pylint score is lower than 9.75 and is $score"
+          echo "Pylint score is lower than 9.5 and is $score"
           exit 1
         fi
       shell: bash
 
     #check if previous scor is not empty
     #if it is not empty then fail if change is lower than -0.05
     - name: Check if previous score is not empty
@@ -95,15 +89,15 @@
         path: comment.txt
     - if: (success() || failure()) && !github.event.pull_request
       run: |
         cat comment.txt >> "${GITHUB_STEP_SUMMARY}"
 
     #add changes of .github/.pylint_cache to the commit if it is based on push event
     - name: Add .github/.pylint_cache to the commit
-      if: github.event_name == 'push' && github.ref_name != 'main'
+      if: (github.event_name == 'push' || github.event.pull_request.merged == true) && github.ref_name != 'main'
       run: |
         git config --global user.email "github-actions[bot]@users.noreply.github.com"
         git config --global user.name "github-actions[bot]"
 
         git add .github/.pylint_cache
         git commit -m "Add .github/.pylint_cache on push event"
```

### Comparing `pqanalysis-1.0.5/.github/workflows/release.yml` & `pqanalysis-1.0.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/.pylintrc` & `pqanalysis-1.0.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/CODE_OF_CONDUCT.md` & `pqanalysis-1.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/LICENSE` & `pqanalysis-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PKG-INFO` & `pqanalysis-1.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PQAnalysis
-Version: 1.0.5
+Version: 1.0.6
 Summary: PQAnalysis is a python package for the analysis of PQ simulations.
 Author-email: Jakob Gamper <97gamjak@gmail.com>, "Josef M. Gallmetzer" <gallmetzer.josef@gmail.com>, "Clarissa A. Seidler" <clarissa.seidler@gmail.com>
 Project-URL: Homepage, https://github.com/MolarVerse/PQAnalysis
 Project-URL: PQ, https://github.com/MolarVerse/PQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,7 +43,24 @@
 [![Docs](https://github.com/MolarVerse/PQAnalysis/actions/workflows/docs.yml/badge.svg)](https://MolarVerse.github.io/PQAnalysis/)
 [![codecov](https://codecov.io/gh/MolarVerse/PQAnalysis/graph/badge.svg?token=IDFK8L6IIQ)](https://codecov.io/gh/MolarVerse/PQAnalysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 The main purpose of this package is to provide useful tools for the analysis of the Molecular Dynamics software package [PQ](https://github.com/MolarVerse/PQ). Furthermore, the intent of this package is to enable straightforward implementations of newly developed analysis tools on top of the provided API.
 
 The future development of this package focuses on two main goals. On the one hand the enhancement of the provided analysis tools and extending its API to be compatible with many other different Molecular Dynamics engines. As this project is only a *hobby* project of the maintainers, any contributions considering enhancement or bug fixes are highly welcomed.
+
+## Installation
+
+Install with pip:
+
+    pip install pqanalysis
+
+## Development
+
+Clone the PQAnalysis GitHub repository and navigate into the directory:
+
+    git clone https://github.com/MolarVerse/PQAnalysis.git
+    cd PQAnalysis
+
+Install with pip:
+
+    pip install .
```

### Comparing `pqanalysis-1.0.5/PQAnalysis/__init__.py` & `pqanalysis-1.0.6/PQAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/analysis/rdf/__init__.py` & `pqanalysis-1.0.6/PQAnalysis/analysis/rdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/analysis/rdf/api.py` & `pqanalysis-1.0.6/PQAnalysis/analysis/rdf/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/analysis/rdf/exceptions.py` & `pqanalysis-1.0.6/PQAnalysis/analysis/rdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/analysis/rdf/rdf.py` & `pqanalysis-1.0.6/PQAnalysis/analysis/rdf/rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/analysis/rdf/rdf_input_file_reader.py` & `pqanalysis-1.0.6/PQAnalysis/analysis/rdf/rdf_input_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/analysis/rdf/rdf_output_file_writer.py` & `pqanalysis-1.0.6/PQAnalysis/analysis/rdf/rdf_output_file_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/atomic_system/_decorators.py` & `pqanalysis-1.0.6/PQAnalysis/atomic_system/_decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/atomic_system/_positions.py` & `pqanalysis-1.0.6/PQAnalysis/atomic_system/_positions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/atomic_system/_properties.py` & `pqanalysis-1.0.6/PQAnalysis/atomic_system/_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/atomic_system/_standard_properties.py` & `pqanalysis-1.0.6/PQAnalysis/atomic_system/_standard_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/atomic_system/atomic_system.py` & `pqanalysis-1.0.6/PQAnalysis/atomic_system/atomic_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 from beartype.typing import Any
 
 # just for forwardref type hinting
 from beartype.typing import List  # pylint: disable=unused-import
 
 from PQAnalysis.core import Atom, Atoms, Cell, distance
 from PQAnalysis.topology import Topology
-from PQAnalysis.types import PositiveReal, PositiveInt
+from PQAnalysis.types import PositiveReal, PositiveInt, Bool
 from PQAnalysis.type_checking import runtime_type_checking
 from PQAnalysis.exceptions import PQNotImplementedError
 from PQAnalysis.utils.random import get_random_seed
 from PQAnalysis.utils.custom_logging import setup_logger
+from PQAnalysis.utils.math import allclose_vectorized
 from PQAnalysis import __package_name__
 
 from PQAnalysis.types import (
     Np2DNumberArray,
     Np1DNumberArray,
     Np1DIntArray,
     Np3x3NumberArray,
@@ -529,50 +530,82 @@
             vel=self.vel,
             forces=self.forces,
             charges=self.charges,
             cell=self.cell,
             topology=self.topology
         )
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: Any) -> Bool:
         """
         Checks whether the AtomicSystem is equal to another AtomicSystem.
 
         Parameters
         ----------
         other : AtomicSystem
             The other AtomicSystem to compare to.
 
         Returns
         -------
         bool
             Whether the AtomicSystem is equal to the other AtomicSystem.
         """
+
+        return self.isclose(other)
+
+    @runtime_type_checking
+    def isclose(
+        self,
+        other: Any,
+        rtol: PositiveReal = 1e-9,
+        atol: PositiveReal = 0.0,
+    ) -> Bool:
+        """
+        Checks whether the AtomicSystem is close to another AtomicSystem.
+
+        Parameters
+        ----------
+        other : AtomicSystem
+            The other AtomicSystem to compare to.
+        rtol : PositiveReal, optional
+            The relative tolerance, by default 1e-9
+        atol : PositiveReal, optional
+            The absolute tolerance, by default 0.0
+
+        Returns
+        -------
+        bool
+            Whether the AtomicSystem is close to the other AtomicSystem.
+        """
+
         if not isinstance(other, AtomicSystem):
             return False
 
         if self.n_atoms != other.n_atoms:
             return False
 
         if self.topology != other.topology:
             return False
 
-        if self.cell != other.cell:
+        if not self.cell.isclose(other.cell, rtol=rtol, atol=atol):
             return False
 
-        if not np.allclose(self.pos, other.pos):
+        if not allclose_vectorized(self.pos, other.pos, rtol=rtol, atol=atol):
             return False
 
-        if not np.allclose(self.vel, other.vel):
+        if not allclose_vectorized(self.vel, other.vel, rtol=rtol, atol=atol):
             return False
 
-        if not np.allclose(self.forces, other.forces):
+        if not allclose_vectorized(
+            self.forces, other.forces, rtol=rtol, atol=atol
+        ):
             return False
 
-        if not np.allclose(self.charges, other.charges):
+        if not allclose_vectorized(
+            self.charges, other.charges, rtol=rtol, atol=atol
+        ):
             return False
 
         return True
 
     def __getitem__(
         self, key: Atom | int | slice | Np1DIntArray
     ) -> "AtomicSystem":
```

### Comparing `pqanalysis-1.0.5/PQAnalysis/atomic_system/exceptions.py` & `pqanalysis-1.0.6/PQAnalysis/atomic_system/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/cli/_argument_parser.py` & `pqanalysis-1.0.6/PQAnalysis/cli/_argument_parser.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/cli/_cli_base.py` & `pqanalysis-1.0.6/PQAnalysis/cli/_cli_base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/cli/add_molecules.py` & `pqanalysis-1.0.6/PQAnalysis/cli/add_molecules.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/cli/build_nep_traj.py` & `pqanalysis-1.0.6/PQAnalysis/cli/build_nep_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/cli/continue_input.py` & `pqanalysis-1.0.6/PQAnalysis/cli/continue_input.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/cli/gen2xyz.py` & `pqanalysis-1.0.6/PQAnalysis/cli/gen2xyz.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/cli/main.py` & `pqanalysis-1.0.6/PQAnalysis/cli/main.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/cli/rdf.py` & `pqanalysis-1.0.6/PQAnalysis/cli/rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/cli/rst2xyz.py` & `pqanalysis-1.0.6/PQAnalysis/cli/rst2xyz.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/cli/traj2box.py` & `pqanalysis-1.0.6/PQAnalysis/cli/traj2box.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/cli/traj2qmcfc.py` & `pqanalysis-1.0.6/PQAnalysis/cli/traj2qmcfc.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/cli/xyz2gen.py` & `pqanalysis-1.0.6/PQAnalysis/cli/xyz2gen.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/core/__init__.py` & `pqanalysis-1.0.6/PQAnalysis/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/core/api.py` & `pqanalysis-1.0.6/PQAnalysis/core/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/core/atom/atom.py` & `pqanalysis-1.0.6/PQAnalysis/core/atom/atom.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/core/atom/element.py` & `pqanalysis-1.0.6/PQAnalysis/core/atom/element.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/core/cell/_standard_properties.py` & `pqanalysis-1.0.6/PQAnalysis/core/cell/_standard_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/core/cell/cell.py` & `pqanalysis-1.0.6/PQAnalysis/core/cell/cell.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 import numpy as np
 
 from beartype.typing import Any, NewType, Annotated
 from beartype.vale import Is
 
 from PQAnalysis.type_checking import runtime_type_checking
-from PQAnalysis.types import Np3x3NumberArray, Np2DNumberArray, NpnDNumberArray
+from PQAnalysis.types import Np3x3NumberArray, Np2DNumberArray, NpnDNumberArray, PositiveReal, Bool
+from PQAnalysis.utils.math import allclose_vectorized
 
 from ._standard_properties import _StandardPropertiesMixin
 
 
 
 class Cell(_StandardPropertiesMixin):
 
@@ -94,25 +95,25 @@
     @property
     def bounding_edges(self) -> Np2DNumberArray:
         """Np2DNumberArray: The 8 corners of the bounding box of the unit cell."""
         edges = np.zeros((8, 3))
         for i, x in enumerate([-0.5, 0.5]):
             for j, y in enumerate([-0.5, 0.5]):
                 for k, z in enumerate([-0.5, 0.5]):
-                    edges[i*4+j*2+k, :] = self.box_matrix @ np.array([x, y, z])
+                    edges[i * 4 + j * 2 +
+                          k, :] = self.box_matrix @ np.array([x, y, z])
 
         return edges
 
     @property
     def volume(self) -> Real:
         """volume: The volume of the unit cell."""
         with warnings.catch_warnings():
             warnings.filterwarnings(
-                "ignore",
-                message="overflow encountered in det"
+                "ignore", message="overflow encountered in det"
             )
             volume = np.linalg.det(self.box_matrix)
 
         return volume
 
     @property
     def is_vacuum(self) -> bool:
@@ -150,35 +151,73 @@
 
             fractional_pos -= np.round(fractional_pos)
 
             pos = fractional_pos @ self.box_matrix.T
 
         return np.reshape(pos, original_shape)
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: Any) -> Bool:
         """
         Checks if the Cell is equal to another Cell.
 
         Parameters
         ----------
         other : Cell
             The Cell to compare with.
 
         Returns
         -------
-        bool
+        Bool
             True if the Cells are equal, False otherwise.
         """
 
+        return self.isclose(other)
+
+    @runtime_type_checking
+    def isclose(
+        self,
+        other: Any,
+        rtol: PositiveReal = 1e-9,
+        atol: PositiveReal = 0.0,
+    ) -> Bool:
+        """
+        Checks if the Cell is close to another Cell.
+
+        Parameters
+        ----------
+        other : Cell
+            The Cell to compare with.
+        rtol : PositiveReal, optional
+            The relative tolerance parameter. Default is 1e-9.
+        atol : PositiveReal, optional
+            The absolute tolerance parameter. Default is 0.0.
+
+        Returns
+        -------
+        Bool
+            True if the Cells are close, False otherwise.
+        """
+
         if not isinstance(other, Cell):
             return False
 
-        is_equal = True
-        is_equal &= np.allclose(self.box_lengths, other.box_lengths)
-        is_equal &= np.allclose(self.box_angles, other.box_angles)
+        is_equal = allclose_vectorized(
+            self.box_lengths,
+            other.box_lengths,
+            rtol=rtol,
+            atol=atol,
+        )
+
+        is_equal &= allclose_vectorized(
+            self.box_angles,
+            other.box_angles,
+            rtol=rtol,
+            atol=atol,
+        )
+
         return is_equal
 
     def __str__(self) -> str:
         """
         Returns a string representation of the Cell.
 
         Returns
@@ -229,33 +268,27 @@
         y = np.linalg.norm(np.transpose(box_matrix)[1])
         z = np.linalg.norm(np.transpose(box_matrix)[2])
 
         gamma = np.arccos(box_matrix[0][1] / y)
         beta = np.arccos(box_matrix[0][2] / z)
         alpha = np.arccos(
             (
-            box_matrix[0][1] * box_matrix[0][2] +
-            box_matrix[1][1] * box_matrix[1][2]
+                box_matrix[0][1] * box_matrix[0][2] +
+                box_matrix[1][1] * box_matrix[1][2]
             ) / (y * z)
         )
 
         print(alpha, beta, gamma)
         print(np.rad2deg(alpha), np.rad2deg(beta), np.rad2deg(gamma))
 
         return cls(
-            x,
-            y,
-            z,
-            np.rad2deg(alpha),
-            np.rad2deg(beta),
-            np.rad2deg(gamma)
+            x, y, z, np.rad2deg(alpha), np.rad2deg(beta), np.rad2deg(gamma)
         )
 
 
 
 #: A type hint for a list of cells
 Cells = NewType(
     "Cells",
     Annotated[list,
-    Is[lambda list: all(isinstance(atom,
-    Cell) for atom in list)]]
+              Is[lambda list: all(isinstance(atom, Cell) for atom in list)]]
 )
```

### Comparing `pqanalysis-1.0.5/PQAnalysis/core/exceptions.py` & `pqanalysis-1.0.6/PQAnalysis/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/core/residue.py` & `pqanalysis-1.0.6/PQAnalysis/core/residue.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/exceptions.py` & `pqanalysis-1.0.6/PQAnalysis/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/formats.py` & `pqanalysis-1.0.6/PQAnalysis/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/grammar/inputGrammar.lark` & `pqanalysis-1.0.6/PQAnalysis/grammar/inputGrammar.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/grammar/rules.lark` & `pqanalysis-1.0.6/PQAnalysis/grammar/rules.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/grammar/selection.lark` & `pqanalysis-1.0.6/PQAnalysis/grammar/selection.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/__init__.py` & `pqanalysis-1.0.6/PQAnalysis/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/api.py` & `pqanalysis-1.0.6/PQAnalysis/io/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/base.py` & `pqanalysis-1.0.6/PQAnalysis/io/base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/box_writer.py` & `pqanalysis-1.0.6/PQAnalysis/io/box_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/conversion_api.py` & `pqanalysis-1.0.6/PQAnalysis/io/conversion_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/energy_file_reader.py` & `pqanalysis-1.0.6/PQAnalysis/io/energy_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/exceptions.py` & `pqanalysis-1.0.6/PQAnalysis/io/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/formats.py` & `pqanalysis-1.0.6/PQAnalysis/io/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/gen_file/api.py` & `pqanalysis-1.0.6/PQAnalysis/io/gen_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/gen_file/gen_file_reader.py` & `pqanalysis-1.0.6/PQAnalysis/io/gen_file/gen_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/gen_file/gen_file_writer.py` & `pqanalysis-1.0.6/PQAnalysis/io/gen_file/gen_file_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/info_file_reader.py` & `pqanalysis-1.0.6/PQAnalysis/io/info_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/exceptions.py` & `pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/formats.py` & `pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/input_file_parser.py` & `pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/input_file_parser.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq/output_files.py` & `pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq/output_files.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py` & `pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py` & `pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py` & `pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py` & `pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py` & `pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py` & `pqanalysis-1.0.6/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/moldescriptor_reader.py` & `pqanalysis-1.0.6/PQAnalysis/io/moldescriptor_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/nep/nep_writer.py` & `pqanalysis-1.0.6/PQAnalysis/io/nep/nep_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/restart_file/api.py` & `pqanalysis-1.0.6/PQAnalysis/io/restart_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/restart_file/restart_reader.py` & `pqanalysis-1.0.6/PQAnalysis/io/restart_file/restart_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/restart_file/restart_writer.py` & `pqanalysis-1.0.6/PQAnalysis/io/restart_file/restart_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/topology_file/api.py` & `pqanalysis-1.0.6/PQAnalysis/io/topology_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/topology_file/topology_file_reader.py` & `pqanalysis-1.0.6/PQAnalysis/io/topology_file/topology_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/topology_file/topology_file_writer.py` & `pqanalysis-1.0.6/PQAnalysis/io/topology_file/topology_file_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/traj_file/api.py` & `pqanalysis-1.0.6/PQAnalysis/io/traj_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/traj_file/frame_reader.py` & `pqanalysis-1.0.6/PQAnalysis/io/traj_file/frame_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/traj_file/trajectory_reader.py` & `pqanalysis-1.0.6/PQAnalysis/io/traj_file/trajectory_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/traj_file/trajectory_writer.py` & `pqanalysis-1.0.6/PQAnalysis/io/traj_file/trajectory_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/virial/api.py` & `pqanalysis-1.0.6/PQAnalysis/io/virial/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/virial/virial_reader.py` & `pqanalysis-1.0.6/PQAnalysis/io/virial/virial_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/io/write_api.py` & `pqanalysis-1.0.6/PQAnalysis/io/write_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/physical_data/energy.py` & `pqanalysis-1.0.6/PQAnalysis/physical_data/energy.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/tools/add_molecule.py` & `pqanalysis-1.0.6/PQAnalysis/tools/add_molecule.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/tools/traj_to_com_traj.py` & `pqanalysis-1.0.6/PQAnalysis/tools/traj_to_com_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/topology/__init__.py` & `pqanalysis-1.0.6/PQAnalysis/topology/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/topology/api.py` & `pqanalysis-1.0.6/PQAnalysis/topology/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/topology/bonded_topology/_topology_properties.py` & `pqanalysis-1.0.6/PQAnalysis/topology/bonded_topology/_topology_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/topology/bonded_topology/angle.py` & `pqanalysis-1.0.6/PQAnalysis/topology/bonded_topology/angle.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/topology/bonded_topology/bond.py` & `pqanalysis-1.0.6/PQAnalysis/topology/bonded_topology/bond.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/topology/bonded_topology/bonded_topology.py` & `pqanalysis-1.0.6/PQAnalysis/topology/bonded_topology/bonded_topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/topology/bonded_topology/dihedral.py` & `pqanalysis-1.0.6/PQAnalysis/topology/bonded_topology/dihedral.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/topology/selection.py` & `pqanalysis-1.0.6/PQAnalysis/topology/selection.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/topology/shake_topology.py` & `pqanalysis-1.0.6/PQAnalysis/topology/shake_topology.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 """
 A module containing the ShakeTopologyGenerator class.
 """
 
+import logging
 import numpy as np
 
 from beartype.typing import List
 
 from PQAnalysis.traj import Trajectory
 from PQAnalysis.types import Np1DIntArray, Np2DIntArray
 from PQAnalysis.io import BaseWriter, FileWritingMode
 from PQAnalysis.type_checking import runtime_type_checking
+from PQAnalysis.utils.custom_logging import setup_logger
+from PQAnalysis.exceptions import PQValueError
+from PQAnalysis import __package_name__
 
 from .selection import SelectionCompatible, Selection
 
 
 
 class ShakeTopologyGenerator:
 
     """
     A class for generating the shake topology for a given trajectory
     """
 
+    logger = logging.getLogger(__package_name__).getChild(__qualname__)
+    logger = setup_logger(logger)
+
     @runtime_type_checking
     def __init__(
         self,
         selection: SelectionCompatible = None,
         use_full_atom_info: bool = False
     ) -> None:
         """
@@ -42,14 +49,15 @@
         self._use_full_atom_info = use_full_atom_info
         self.selection = Selection(selection)
 
         self.indices = None
         self.target_indices = None
         self.distances = None
         self._topology = None
+        self.line_comments = None
 
     @runtime_type_checking
     def generate_topology(self, trajectory: Trajectory) -> None:
         """
         Generates a tuple of indices, target_indices, and distances for the given trajectory.
 
         The generated numpy arrays represent all important information about the shake
@@ -65,16 +73,15 @@
             The trajectory to generate the shake topology for.
         """
 
         atomic_system = trajectory[0]
         self._topology = trajectory.topology
 
         indices = self.selection.select(
-            self._topology,
-            self._use_full_atom_info
+            self._topology, self._use_full_atom_info
         )
 
         target_indices, distances = atomic_system.nearest_neighbours(
             n=1, selection=indices, use_full_atom_info=self._use_full_atom_info)
 
         target_indices = target_indices.flatten()
         distances = [distances.flatten()]
@@ -92,36 +99,79 @@
         self.indices = indices
         self.target_indices = target_indices
         self.distances = np.mean(np.array(distances), axis=0)
 
     @runtime_type_checking
     def average_equivalents(
         self,
-        indices: List[Np1DIntArray] | Np2DIntArray
+        indices: List[Np1DIntArray] | Np2DIntArray,
+        comments: List[str] | None = None
     ) -> None:
         """
         Averages the distances for equivalent atoms.
 
         The parameter indices is a numpy 2d array of equivalent atom indices.
         Each row of the array contains the indices of equivalent atoms.
         All of the equivalent atoms will be averaged to a single distance.
 
         Parameters
         ----------
         indices : List[Np1DIntArray] | Np2DIntArray
             The indices of the equivalent atoms.
+        comments : List[str], optional
+            The line comments for the averaged distances, by default None
         """
 
         for equivalent_indices in indices:
             _indices = np.nonzero(np.in1d(self.indices, equivalent_indices))[0]
 
             mean_distance = np.mean(self.distances[_indices])
 
             self.distances[_indices] = mean_distance
 
+        if comments is not None:
+            if len(comments) != len(indices):
+                self.logger.error(
+                    "The number of comments does not match the number of indices.",
+                    exception=PQValueError
+                )
+
+            self.line_comments = [""] * len(self.indices)
+
+            for i, equivalent_indices in enumerate(indices):
+                _indices = np.nonzero(
+                    np.in1d(self.indices, equivalent_indices)
+                )[0]
+
+                for index in _indices:
+                    self.line_comments[index] = comments[i]
+
+    @runtime_type_checking
+    def add_comments(self, comments: List[str]) -> None:
+        """
+        Adds comments to the topology.
+
+        Parameters
+        ----------
+        comments : List[str]
+            The comments to add to each line of the shake topology.
+        """
+
+        if self.indices is None or len(comments) != len(self.indices):
+            self.logger.error(
+                "The number of comments does not match the number of indices.",
+                exception=PQValueError
+            )
+
+        if self.line_comments is None:
+            self.line_comments = [""] * len(self.indices)
+
+        for i, comment in enumerate(comments):
+            self.line_comments[i] = comment
+
     @runtime_type_checking
     def write_topology(
         self,
         filename: str | None = None,
         mode: FileWritingMode | str = "w"
     ) -> None:
         """
@@ -143,25 +193,34 @@
         """
 
         writer = BaseWriter(filename, mode=mode)
         writer.open()
 
         print(
             (
-            f"SHAKE {len(self.indices)}  "
-            f"{len(np.unique(self.target_indices))}  0"
+                f"SHAKE {len(self.indices)}  "
+                f"{len(np.unique(self.target_indices))}  0"
             ),
             file=writer.file
         )
 
         for i, index in enumerate(self.indices):
             target_index = self.target_indices[i]
             distance = self.distances[i]
 
-            print(f"{index+1} {target_index+1} {distance}", file=writer.file)
+            print(
+                f"{index+1} {target_index+1} {distance}",
+                end="",
+                file=writer.file
+            )
+
+            if self.line_comments is not None:
+                print(f"  # {self.line_comments[i]}", file=writer.file)
+            else:
+                print("", file=writer.file)
 
         print("END", file=writer.file)
 
     @property
     def selection_object(self) -> SelectionCompatible:
         """SelectionCompatible: The selection object."""
         return self.selection.selection_object
```

### Comparing `pqanalysis-1.0.5/PQAnalysis/topology/topology.py` & `pqanalysis-1.0.6/PQAnalysis/topology/topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/traj/api.py` & `pqanalysis-1.0.6/PQAnalysis/traj/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/traj/exceptions.py` & `pqanalysis-1.0.6/PQAnalysis/traj/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/traj/formats.py` & `pqanalysis-1.0.6/PQAnalysis/traj/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/traj/trajectory.py` & `pqanalysis-1.0.6/PQAnalysis/traj/trajectory.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,25 @@
 
 import logging
 import numpy as np
 
 from beartype.typing import List, Any, Iterable
 
 from PQAnalysis.topology import Topology
-from PQAnalysis.types import Np2DNumberArray, Np1DNumberArray
 from PQAnalysis.exceptions import PQIndexError, PQTypeError
 from PQAnalysis.core import Cell
 from PQAnalysis.atomic_system import AtomicSystem
 from PQAnalysis.utils.custom_logging import setup_logger
 from PQAnalysis import __package_name__
+from PQAnalysis.types import (
+    Np2DNumberArray,
+    Np1DNumberArray,
+    PositiveReal,
+    Bool,
+)
 from PQAnalysis.type_checking import (
     runtime_type_checking,
     runtime_type_checking_setter,
 )
 
 
 
@@ -330,31 +335,67 @@
             self.logger.error(
                 "Only Trajectory objects can be added to a Trajectory.",
                 exception=PQTypeError,
             )
 
         return Trajectory(self.frames + other.frames)
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: Any) -> Bool:
         """
         This method allows two trajectories to be compared for equality.
 
         Parameters
         ----------
         other : Trajectory
             The other trajectory to compare.
+
+        Returns
+        -------
+        Bool
+            Whether the two trajectories are equal.
+        """
+
+        return self.isclose(other)
+
+    def isclose(
+        self,
+        other: Any,
+        rtol: PositiveReal = 1e-9,
+        atol: PositiveReal = 0.0,
+    ) -> Bool:
+        """
+        This method allows two trajectories to be compared for closeness.
+
+        Parameters
+        ----------
+        other : Any
+            The other object to compare with.
+        rtol : PositiveReal, optional
+            The relative tolerance parameter, by default 1e-9
+        atol : PositiveReal, optional
+            The absolute tolerance parameter, by default 0.0
+
+        Returns
+        -------
+        Bool
+            Whether the two trajectories are close.
         """
 
         if not isinstance(other, Trajectory):
             return False
 
         if len(self.frames) != len(other.frames):
             return False
 
-        return self.frames == other.frames
+        return np.all(
+            [
+                self.frames[i].isclose(other.frames[i], rtol=rtol, atol=atol)
+                for i in np.arange(len(self.frames))
+            ]
+        )
 
     def __str__(self) -> str:
         """
         This method allows the string representation of a trajectory to be retrieved.
 
         Returns
         -------
```

### Comparing `pqanalysis-1.0.5/PQAnalysis/type_checking.py` & `pqanalysis-1.0.6/PQAnalysis/type_checking.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/types.py` & `pqanalysis-1.0.6/PQAnalysis/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,72 +6,90 @@
 
 import numpy as np
 
 from beartype.vale import Is
 from beartype.typing import NewType
 
 #: A type hint for positive integers
-PositiveInt = NewType("PositiveInt", Annotated[int, Is[lambda int: int > 0]])
+PositiveInt = NewType(
+    "PositiveInt",
+    Annotated[int, Is[lambda int: int > 0]],
+)
 
 # :A type hint for positive real numbers
 PositiveReal = NewType(
-    "PositiveReal",
-    Annotated[Real,
-    Is[lambda real: real >= 0.0]]
+    "PositiveReal", Annotated[
+        Real,
+        Is[lambda real: real >= 0.0],
+    ]
 )
 
 #: A type variable for a 1D np.ndarray with dtype np.number
 Np1DNumberArray = NewType(
     "Np1DNumberArray",
-    Annotated[np.ndarray,
-    Is[lambda array: array.ndim == 1 and
-    (np.issubdtype(array.dtype,
-    np.number)) or len(array) == 0]]
+    Annotated[
+        np.ndarray,
+        Is[lambda array: array.ndim == 1 and
+           (np.issubdtype(array.dtype, np.number)) or len(array) == 0],
+    ]
 )
 
 #: A type hint for a 2D np.ndarray with dtype np.number
 Np2DNumberArray = NewType(
     "Np2DNumberArray",
-    Annotated[np.ndarray,
-    Is[lambda array: array.ndim == 2 and
-    (np.issubdtype(array.dtype,
-    np.number))]]
+    Annotated[
+        np.ndarray,
+        Is[lambda array: array.ndim == 2 and
+           (np.issubdtype(array.dtype, np.number))],
+    ]
 )
 
 #: A type hint for a nD np.ndarray with dtype np.number
 NpnDNumberArray = NewType(
     "NpnDNumberArray",
-    Annotated[np.ndarray,
-    Is[lambda array: array.ndim > 0 and
-    (np.issubdtype(array.dtype,
-    np.number))]]
+    Annotated[
+        np.ndarray,
+        Is[lambda array: array.ndim > 0 and
+           (np.issubdtype(array.dtype, np.number))],
+    ]
 )
 
 #: A type hint for a 3x3 np.ndarray matrix with dtype np.number
 Np3x3NumberArray = NewType(
     "Np2x2NumberArray",
-    Annotated[np.ndarray,
-    Is[lambda array: array.ndim == 2 and array.shape == (3,
-    3) and (np.issubdtype(array.dtype,
-    np.number))]]
+    Annotated[
+        np.ndarray,
+        Is[lambda array: array.ndim == 2 and array.shape == (3, 3) and
+           (np.issubdtype(array.dtype, np.number))],
+    ]
 )
 
 #: A type hint for a 2D np.ndarray with dtype np.integer
 Np2DIntArray = NewType(
     "Np2DIntArray",
-    Annotated[np.ndarray,
-    Is[lambda array: array.ndim == 2 and
-    (np.issubdtype(array.dtype,
-    np.integer))]]
+    Annotated[
+        np.ndarray,
+        Is[lambda array: array.ndim == 2 and
+           (np.issubdtype(array.dtype, np.integer))],
+    ]
 )
 
 #: A type hint for a 1D np.ndarray with dtype np.integer
 Np1DIntArray = NewType(
     "Np1DIntArray",
-    Annotated[np.ndarray,
-    Is[lambda array: array.ndim == 1 and
-    (np.issubdtype(array.dtype,
-    np.integer)) or len(array) == 0]]
+    Annotated[
+        np.ndarray,
+        Is[lambda array: array.ndim == 1 and
+           (np.issubdtype(array.dtype, np.integer)) or len(array) == 0],
+    ]
 )
 
 #: A type hint for a range object
 Range = NewType("Range", Annotated[range, Is[lambda r: isinstance(r, range)]])
+
+Bool = NewType(
+    "Bool",
+    Annotated[
+        bool | np.bool_,
+        Is[lambda b: isinstance(b, (bool, np.bool_))],
+    ]
+)
```

### Comparing `pqanalysis-1.0.5/PQAnalysis/utils/common.py` & `pqanalysis-1.0.6/PQAnalysis/utils/common.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/utils/custom_logging.py` & `pqanalysis-1.0.6/PQAnalysis/utils/custom_logging.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/utils/decorators.py` & `pqanalysis-1.0.6/PQAnalysis/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/utils/files.py` & `pqanalysis-1.0.6/PQAnalysis/utils/files.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis/utils/random.py` & `pqanalysis-1.0.6/PQAnalysis/utils/random.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/PQAnalysis.egg-info/PKG-INFO` & `pqanalysis-1.0.6/PQAnalysis.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PQAnalysis
-Version: 1.0.5
+Version: 1.0.6
 Summary: PQAnalysis is a python package for the analysis of PQ simulations.
 Author-email: Jakob Gamper <97gamjak@gmail.com>, "Josef M. Gallmetzer" <gallmetzer.josef@gmail.com>, "Clarissa A. Seidler" <clarissa.seidler@gmail.com>
 Project-URL: Homepage, https://github.com/MolarVerse/PQAnalysis
 Project-URL: PQ, https://github.com/MolarVerse/PQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,7 +43,24 @@
 [![Docs](https://github.com/MolarVerse/PQAnalysis/actions/workflows/docs.yml/badge.svg)](https://MolarVerse.github.io/PQAnalysis/)
 [![codecov](https://codecov.io/gh/MolarVerse/PQAnalysis/graph/badge.svg?token=IDFK8L6IIQ)](https://codecov.io/gh/MolarVerse/PQAnalysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 The main purpose of this package is to provide useful tools for the analysis of the Molecular Dynamics software package [PQ](https://github.com/MolarVerse/PQ). Furthermore, the intent of this package is to enable straightforward implementations of newly developed analysis tools on top of the provided API.
 
 The future development of this package focuses on two main goals. On the one hand the enhancement of the provided analysis tools and extending its API to be compatible with many other different Molecular Dynamics engines. As this project is only a *hobby* project of the maintainers, any contributions considering enhancement or bug fixes are highly welcomed.
+
+## Installation
+
+Install with pip:
+
+    pip install pqanalysis
+
+## Development
+
+Clone the PQAnalysis GitHub repository and navigate into the directory:
+
+    git clone https://github.com/MolarVerse/PQAnalysis.git
+    cd PQAnalysis
+
+Install with pip:
+
+    pip install .
```

### Comparing `pqanalysis-1.0.5/PQAnalysis.egg-info/SOURCES.txt` & `pqanalysis-1.0.6/PQAnalysis.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
 PQAnalysis/traj/formats.py
 PQAnalysis/traj/trajectory.py
 PQAnalysis/utils/__init__.py
 PQAnalysis/utils/common.py
 PQAnalysis/utils/custom_logging.py
 PQAnalysis/utils/decorators.py
 PQAnalysis/utils/files.py
+PQAnalysis/utils/math.py
 PQAnalysis/utils/random.py
 PQAnalysis/utils/units.py
 benchmarks/pytest.ini
 benchmarks/core/benchmark_cell.py
 benchmarks/core/benchmark_traj_reader.py
 docs/Makefile
 docs/autodoc.sh
@@ -375,8 +376,9 @@
 tests/topology/bonded_topology/test_bondedTopology.py
 tests/topology/bonded_topology/test_dihedral.py
 tests/traj/__init__.py
 tests/traj/test_api.py
 tests/traj/test_trajectory.py
 tests/utils/__init__.py
 tests/utils/test_common.py
-tests/utils/test_decorators.py
+tests/utils/test_decorators.py
+tests/utils/test_math.py
```

### Comparing `pqanalysis-1.0.5/README.md` & `pqanalysis-1.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -3,8 +3,25 @@
 [![CI](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml/badge.svg)](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml)
 [![Docs](https://github.com/MolarVerse/PQAnalysis/actions/workflows/docs.yml/badge.svg)](https://MolarVerse.github.io/PQAnalysis/)
 [![codecov](https://codecov.io/gh/MolarVerse/PQAnalysis/graph/badge.svg?token=IDFK8L6IIQ)](https://codecov.io/gh/MolarVerse/PQAnalysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 The main purpose of this package is to provide useful tools for the analysis of the Molecular Dynamics software package [PQ](https://github.com/MolarVerse/PQ). Furthermore, the intent of this package is to enable straightforward implementations of newly developed analysis tools on top of the provided API.
 
-The future development of this package focuses on two main goals. On the one hand the enhancement of the provided analysis tools and extending its API to be compatible with many other different Molecular Dynamics engines. As this project is only a *hobby* project of the maintainers, any contributions considering enhancement or bug fixes are highly welcomed.
+The future development of this package focuses on two main goals. On the one hand the enhancement of the provided analysis tools and extending its API to be compatible with many other different Molecular Dynamics engines. As this project is only a *hobby* project of the maintainers, any contributions considering enhancement or bug fixes are highly welcomed.
+
+## Installation
+
+Install with pip:
+
+    pip install pqanalysis
+
+## Development
+
+Clone the PQAnalysis GitHub repository and navigate into the directory:
+
+    git clone https://github.com/MolarVerse/PQAnalysis.git
+    cd PQAnalysis
+
+Install with pip:
+
+    pip install .
```

### Comparing `pqanalysis-1.0.5/benchmarks/core/benchmark_traj_reader.py` & `pqanalysis-1.0.6/benchmarks/core/benchmark_traj_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import pytest
+
 from PQAnalysis.io.traj_file import TrajectoryReader
 
 
 
+@pytest.mark.benchmark(group="TrajectoryReader")
 class BenchmarkTrajReader:
 
     def benchmark_read_2frames(self, benchmark):
         traj_reader = TrajectoryReader(
             "tests/data/traj2box/test.xyz"
         )  # 2 frames
         benchmark(traj_reader.read)
```

### Comparing `pqanalysis-1.0.5/docs/Makefile` & `pqanalysis-1.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/make.bat` & `pqanalysis-1.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/_templates/module.rst` & `pqanalysis-1.0.6/docs/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/_templates/package.rst` & `pqanalysis-1.0.6/docs/source/_templates/package.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/code/PQAnalysis.atomic_system.exceptions.rst` & `pqanalysis-1.0.6/docs/source/code/PQAnalysis.atomic_system.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.exceptions.rst` & `pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst` & `pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst` & `pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst` & `pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.input_file_reader.rst` & `pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.input_file_reader.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.rst` & `pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst` & `pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/code/PQAnalysis.io.traj_file.api.rst` & `pqanalysis-1.0.6/docs/source/code/PQAnalysis.io.traj_file.api.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/code/PQAnalysis.rst` & `pqanalysis-1.0.6/docs/source/code/PQAnalysis.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/code/PQAnalysis.tools.add_molecule.rst` & `pqanalysis-1.0.6/docs/source/code/PQAnalysis.tools.add_molecule.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/code/PQAnalysis.topology.api.rst` & `pqanalysis-1.0.6/docs/source/code/PQAnalysis.topology.api.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/code/PQAnalysis.utils.custom_logging.rst` & `pqanalysis-1.0.6/docs/source/code/PQAnalysis.utils.custom_logging.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/conf.py` & `pqanalysis-1.0.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/developerGuide/developerGuide.rst` & `pqanalysis-1.0.6/docs/source/developerGuide/developerGuide.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/logo/PQAnalysis.png` & `pqanalysis-1.0.6/docs/source/logo/PQAnalysis.png`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/userGuide/inputFile.rst` & `pqanalysis-1.0.6/docs/source/userGuide/inputFile.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/docs/source/userGuide/userGuide.rst` & `pqanalysis-1.0.6/docs/source/userGuide/userGuide.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/examples/traj2box/acof_triclinic.xyz` & `pqanalysis-1.0.6/examples/traj2box/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/examples/traj2box/acof_triclinic_2.xyz` & `pqanalysis-1.0.6/examples/traj2box/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/examples/traj2comtraj/umcm-9-md-01.xyz` & `pqanalysis-1.0.6/examples/traj2comtraj/umcm-9-md-01.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/pyproject.toml` & `pqanalysis-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/analysis/rdf/test_api.py` & `pqanalysis-1.0.6/tests/analysis/rdf/test_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/analysis/rdf/test_rdf.py` & `pqanalysis-1.0.6/tests/analysis/rdf/test_rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/analysis/rdf/test_rdfInputFileReader.py` & `pqanalysis-1.0.6/tests/analysis/rdf/test_rdfInputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/analysis/rdf/test_rdfOutputFileReader.py` & `pqanalysis-1.0.6/tests/analysis/rdf/test_rdfOutputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/atomicSystem/test_atomic_system.py` & `pqanalysis-1.0.6/tests/atomicSystem/test_atomic_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,56 @@
 
         system1 = AtomicSystem(charges=np.array([1]))
         system2 = AtomicSystem(charges=np.array([0]))
 
         assert system1 != system2
         assert system3 != system5
 
+    def test_isclose(self):
+        system3 = AtomicSystem(
+            pos=np.array([[0, 0, 0], [1, 1, 1]]),
+            atoms=[Atom('C'), Atom('H')],
+            cell=Cell(0.75, 0.75, 0.75)
+        )
+        system4 = AtomicSystem(
+            pos=np.array([[0.00001, 0, 0], [1, 1.00001, 1]]),
+            atoms=[Atom('C'), Atom('H')],
+            cell=Cell(0.75, 0.750001, 0.75)
+        )
+        system5 = AtomicSystem(
+            pos=np.array([[0, 0.01, 0], [1, 1.01, 1]]),
+            atoms=[Atom('C'), Atom('H')],
+            cell=Cell(0.75, 0.76, 0.75)
+        )
+
+        assert system3.isclose(system4, atol=1.0001e-5)
+        assert system3.isclose(system4, rtol=1)
+        assert not system3.isclose(system4, atol=1e-6)
+        assert not system3.isclose(system4, rtol=1e-6)
+
+        assert system3.isclose(system5, atol=1e-1)
+        assert not system3.isclose(system5, rtol=1e-1)
+        assert not system3.isclose(system5, atol=1e-3)
+        assert not system3.isclose(system5, rtol=1e-2)
+
+        system1 = AtomicSystem(
+            pos=np.array([[0.0, 0, 0], [1, 100.1, 1]]),
+            atoms=[Atom('C'), Atom('H')]
+        )
+
+        system2 = AtomicSystem(
+            pos=np.array([[0.0, 0, 0], [1, 100.11, 1]]),
+            atoms=[Atom('C'), Atom('H')]
+        )
+
+        assert system1.isclose(system2, atol=1.1e-2)
+        assert system1.isclose(system2, rtol=1.1e-4)
+        assert not system1.isclose(system2, atol=1.0e-3)
+        assert not system1.isclose(system2, rtol=1.0e-5)
+
     def test__getitem__(self):
         system = AtomicSystem(
             pos=np.array([[0, 0, 0], [1, 1, 1]]),
             atoms=[Atom('C'), Atom('H')],
             cell=Cell(0.75, 0.75, 0.75)
         )
```

### Comparing `pqanalysis-1.0.5/tests/atomicSystem/test_decorators.py` & `pqanalysis-1.0.6/tests/atomicSystem/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/atomicSystem/test_positions.py` & `pqanalysis-1.0.6/tests/atomicSystem/test_positions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/cli/test_continue_input.py` & `pqanalysis-1.0.6/tests/cli/test_continue_input.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/cli/test_rst2xyz.py` & `pqanalysis-1.0.6/tests/cli/test_rst2xyz.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/cli/test_traj2box.py` & `pqanalysis-1.0.6/tests/cli/test_traj2box.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/cli/test_traj2qmcfc.py` & `pqanalysis-1.0.6/tests/cli/test_traj2qmcfc.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/conftest.py` & `pqanalysis-1.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/core/atom/test_atom.py` & `pqanalysis-1.0.6/tests/core/atom/test_atom.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/core/atom/test_element.py` & `pqanalysis-1.0.6/tests/core/atom/test_element.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/core/test_residue.py` & `pqanalysis-1.0.6/tests/core/test_residue.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/n_not_matching.in` & `pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/n_not_matching.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in` & `pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/no_output_files.in` & `pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/no_output_files.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/no_start_file.in` & `pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/no_start_file.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in` & `pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/run-08.in` & `pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/run-08.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/run-08.rpmd.in` & `pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/run-08.rpmd.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/run-09.in.ref` & `pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/run-09.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref` & `pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/run-10.in.ref` & `pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/run-10.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref` & `pqanalysis-1.0.6/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/readEnergyFile/md-01.info` & `pqanalysis-1.0.6/tests/data/readEnergyFile/md-01.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/readInfoFile/md-01.info` & `pqanalysis-1.0.6/tests/data/readInfoFile/md-01.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/readInfoFile/md-01.qmcfc.info` & `pqanalysis-1.0.6/tests/data/readInfoFile/md-01.qmcfc.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/traj2qmcfc/acof_triclinic.xyz` & `pqanalysis-1.0.6/tests/data/traj2qmcfc/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/traj2qmcfc/acof_triclinic_2.xyz` & `pqanalysis-1.0.6/tests/data/traj2qmcfc/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/data/traj2qmcfc/traj.qmcfc.xyz` & `pqanalysis-1.0.6/tests/data/traj2qmcfc/traj.qmcfc.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py` & `pqanalysis-1.0.6/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/inputFileReader/PQAnalysis/test_parse.py` & `pqanalysis-1.0.6/tests/io/inputFileReader/PQAnalysis/test_parse.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/inputFileReader/test_inputDictionary.py` & `pqanalysis-1.0.6/tests/io/inputFileReader/test_inputDictionary.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/inputFileReader/test_inputFileParser.py` & `pqanalysis-1.0.6/tests/io/inputFileReader/test_inputFileParser.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/inputFileReader/test_transformers.py` & `pqanalysis-1.0.6/tests/io/inputFileReader/test_transformers.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/inputFileReader/test_visitors.py` & `pqanalysis-1.0.6/tests/io/inputFileReader/test_visitors.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/test_base.py` & `pqanalysis-1.0.6/tests/io/test_base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/test_boxWriter.py` & `pqanalysis-1.0.6/tests/io/test_boxWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/test_energyFileReader.py` & `pqanalysis-1.0.6/tests/io/test_energyFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/test_frameReader.py` & `pqanalysis-1.0.6/tests/io/test_frameReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/test_infoFileReader.py` & `pqanalysis-1.0.6/tests/io/test_infoFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/test_moldescriptorReader.py` & `pqanalysis-1.0.6/tests/io/test_moldescriptorReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/test_restartReader.py` & `pqanalysis-1.0.6/tests/io/test_restartReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/test_restartWriter.py` & `pqanalysis-1.0.6/tests/io/test_restartWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/test_trajectoryReader.py` & `pqanalysis-1.0.6/tests/io/test_trajectoryReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/test_trajectoryWriter.py` & `pqanalysis-1.0.6/tests/io/test_trajectoryWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/io/test_write_api.py` & `pqanalysis-1.0.6/tests/io/test_write_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/physicalData/test_energy.py` & `pqanalysis-1.0.6/tests/physicalData/test_energy.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/tools/test_traj_to_com_traj.py` & `pqanalysis-1.0.6/tests/tools/test_traj_to_com_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/topology/bonded_topology/test_angle.py` & `pqanalysis-1.0.6/tests/topology/bonded_topology/test_angle.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/topology/bonded_topology/test_bond.py` & `pqanalysis-1.0.6/tests/topology/bonded_topology/test_bond.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/topology/bonded_topology/test_bondedTopology.py` & `pqanalysis-1.0.6/tests/topology/bonded_topology/test_bondedTopology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/topology/bonded_topology/test_dihedral.py` & `pqanalysis-1.0.6/tests/topology/bonded_topology/test_dihedral.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/topology/test_selection.py` & `pqanalysis-1.0.6/tests/topology/test_selection.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/topology/test_selectionTransformer.py` & `pqanalysis-1.0.6/tests/topology/test_selectionTransformer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/topology/test_topology.py` & `pqanalysis-1.0.6/tests/topology/test_topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/traj/test_api.py` & `pqanalysis-1.0.6/tests/traj/test_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.5/tests/traj/test_trajectory.py` & `pqanalysis-1.0.6/tests/traj/test_trajectory.py`

 * *Files 3% similar despite different names*

```diff
@@ -305,14 +305,41 @@
 
         assert Trajectory() == Trajectory()
         assert traj1 != Trajectory()
         assert Trajectory() != traj1
 
         assert Trajectory() != 1
 
+    def test_isclose(self):
+        frame1 = AtomicSystem(
+            atoms=self.atoms1,
+            pos=np.array([[1.0001, 1.0002, 2.0003]]),
+            cell=Cell(100.1, 100.1, 100.1)
+        )
+        frame2 = AtomicSystem(
+            atoms=self.atoms1,
+            pos=np.array([[1.0002, 1.0003, 2.0004]]),
+            cell=Cell(100.1001, 100.1001, 100.1001)
+        )
+        frame3 = AtomicSystem(
+            atoms=self.atoms1,
+            pos=np.array([[1.0001, 1.0002, 2.0003]]),
+            cell=Cell(100.2, 100.2, 100.2)
+        )
+
+        traj1 = Trajectory([frame1, frame1])
+        traj2 = Trajectory([frame2, frame2])
+        traj3 = Trajectory([frame3, frame3])
+
+        assert traj1.isclose(traj2, atol=1.0001e-4)
+        assert not traj1.isclose(traj2, atol=1e-5)
+
+        assert traj1.isclose(traj3, rtol=1e-3)
+        assert not traj1.isclose(traj3, rtol=1e-4)
+
     def test_append(self):
         traj = Trajectory()
         print(len(traj))
         traj.append(self.frame1)
         print(len(traj))
 
         assert traj.frames == [self.frame1]
```

### Comparing `pqanalysis-1.0.5/tests/utils/test_common.py` & `pqanalysis-1.0.6/tests/utils/test_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import pytest
 
 from _pytest.capture import CaptureFixture
 
 from PQAnalysis.utils import print_header
 from PQAnalysis._version import __version__
 
+from . import pytestmark
+
 
 
 def test_print_header(capsys: CaptureFixture):
     print_header()
 
     captured = capsys.readouterr()
```

### Comparing `pqanalysis-1.0.5/tests/utils/test_decorators.py` & `pqanalysis-1.0.6/tests/utils/test_decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from PQAnalysis.utils import count_decorator, instance_function_count_decorator
 
+from . import pytestmark
+
 
 
 def test_count_decorator():
 
     @count_decorator
     def test_func(reset_counter=False):
         pass
```

