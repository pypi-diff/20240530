# Comparing `tmp/wgse_ng-1.0.0a8.tar.gz` & `tmp/wgse_ng-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgse_ng-1.0.0a8.tar", last modified: Tue May 21 17:26:35 2024, max compression
+gzip compressed data, was "wgse_ng-1.0.0a9.tar", last modified: Tue May 21 19:39:04 2024, max compression
```

## Comparing `wgse_ng-1.0.0a8.tar` & `wgse_ng-1.0.0a9.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.701771 wgse_ng-1.0.0a8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.653771 wgse_ng-1.0.0a8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.657771 wgse_ng-1.0.0a8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.github/ISSUE_TEMPLATE/add-a-new-reference.md
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.657771 wgse_ng-1.0.0a8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.github/workflows/python-pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.657771 wgse_ng-1.0.0a8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-21 17:26:35.701771 wgse_ng-1.0.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.701771 wgse_ng-1.0.0a8/WGSE_NG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-21 17:26:35.000000 wgse_ng-1.0.0a8/WGSE_NG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-21 17:26:35.000000 wgse_ng-1.0.0a8/WGSE_NG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:26:35.000000 wgse_ng-1.0.0a8/WGSE_NG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-21 17:26:35.000000 wgse_ng-1.0.0a8/WGSE_NG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 17:26:35.000000 wgse_ng-1.0.0a8/WGSE_NG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 17:26:35.000000 wgse_ng-1.0.0a8/WGSE_NG.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.661771 wgse_ng-1.0.0a8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/basic-usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/reference-genome.md
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/docs/wgse-library.md
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/main.spec
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 17:26:35.701771 wgse_ng-1.0.0a8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.661771 wgse_ng-1.0.0a8/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   116407 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/fake_genome.fasta
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_fasta_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_letter_run_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_raw_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/test_unknown_bases_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/test/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.661771 wgse_ng-1.0.0a8/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/tools/fake_reference_genome_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/tools/import_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/tools/last_file_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/tools/reference_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.665771 wgse_ng-1.0.0a8/wgse/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-21 17:26:35.000000 wgse_ng-1.0.0a8/wgse/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.665771 wgse_ng-1.0.0a8/wgse/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/adapters/alignment_map_file_info_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/adapters/alignment_stats_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/adapters/header_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/adapters/index_stats_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/adapters/reference_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.665771 wgse_ng-1.0.0a8/wgse/alignment_map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/alignment_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/alignment_map/alignment_map_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/alignment_map/alignment_map_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/alignment_map/alignment_map_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/alignment_map/alignment_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/alignment_map/depth_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/alignment_map/index_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.669771 wgse_ng-1.0.0a8/wgse/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.669771 wgse_ng-1.0.0a8/wgse/data/alignment_map/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/alignment_map/alignment_map_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/alignment_map/alignment_map_header_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/alignment_map/alignment_map_header_program.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/alignment_map/alignment_map_header_read_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/alignment_map/alignment_map_header_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/alignment_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/chromosome_name_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/genome.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/mitochondrial_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/mitochondrial_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/mitochondrial_name_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/read_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/sequence_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/data/tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.669771 wgse_ng-1.0.0a8/wgse/fasta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fasta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fasta/fasta_letter_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fasta/fasta_stats_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fasta/letter_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fasta/letter_run_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fasta/letter_run_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fasta/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.669771 wgse_ng-1.0.0a8/wgse/fastq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/fastq/fastq_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.673771 wgse_ng-1.0.0a8/wgse/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/WGSE-NG.pyproject
--rw-r--r--   0 runner    (1001) docker     (127)    11778 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/WGSE-NG.pyproject.user
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.673771 wgse_ng-1.0.0a8/wgse/gui/extract/
--rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/extract/extract_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/extract/format_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/extract/microarray_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/extract/sequence_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/form.ui
--rw-r--r--   0 runner    (1001) docker     (127)    14690 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/reference.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.673771 wgse_ng-1.0.0a8/wgse/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67343 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/resources/logo.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   327118 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/resources/logo_nXP_icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/resources.qrc
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/table_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/gui/ui_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.681771 wgse_ng-1.0.0a8/wgse/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.693771 wgse_ng-1.0.0a8/wgse/metadata/bed_templates/
--rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/bed_templates/19_wes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/bed_templates/19_y_mt.csv
--rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/bed_templates/38_wes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/bed_templates/38_y_mt.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/bed_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/builds.json
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/mtdna.json
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/ploidy.txt
--rw-r--r--   0 runner    (1001) docker     (127)  4213157 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/references.json
--rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/references_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.693771 wgse_ng-1.0.0a8/wgse/metadata/report_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/report_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/report_templates/table_macro.html
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/report_templates/table_simple.html
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/report_templates/table_tab.html
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/sequencers.json
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/metadata/sources.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.693771 wgse_ng-1.0.0a8/wgse/microarray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/microarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/microarray/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/microarray/microarray_line_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/microarray/raw_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.697771 wgse_ng-1.0.0a8/wgse/mtDNA/
--rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/mtDNA/CRS.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    17129 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/mtDNA/RSRS.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/mtDNA/Yoruba.fasta
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/mtDNA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/mtDNA/rCRS.fasta
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.697771 wgse_ng-1.0.0a8/wgse/reference_genome/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/reference_genome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/reference_genome/bgzip_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/reference_genome/decompressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/reference_genome/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/reference_genome/genome_metadata_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/reference_genome/repository_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.697771 wgse_ng-1.0.0a8/wgse/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/renderers/csv_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/renderers/html_aligned_file_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/renderers/html_simple_table_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:35.701771 wgse_ng-1.0.0a8/wgse/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/check_prerequisites.py
--rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/external.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/file_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/mt_dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/process_io_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/sequence_orderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/sequencers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/shortcut.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/simple_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/unit_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/utility/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-21 17:26:30.000000 wgse_ng-1.0.0a8/wgse/variant_caller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.278692 wgse_ng-1.0.0a9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.234691 wgse_ng-1.0.0a9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.238692 wgse_ng-1.0.0a9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/.github/ISSUE_TEMPLATE/add-a-new-reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.238692 wgse_ng-1.0.0a9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/.github/workflows/python-pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.238692 wgse_ng-1.0.0a9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-21 19:39:04.278692 wgse_ng-1.0.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.278692 wgse_ng-1.0.0a9/WGSE_NG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-21 19:39:04.000000 wgse_ng-1.0.0a9/WGSE_NG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-21 19:39:04.000000 wgse_ng-1.0.0a9/WGSE_NG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:39:04.000000 wgse_ng-1.0.0a9/WGSE_NG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-21 19:39:04.000000 wgse_ng-1.0.0a9/WGSE_NG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 19:39:04.000000 wgse_ng-1.0.0a9/WGSE_NG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 19:39:04.000000 wgse_ng-1.0.0a9/WGSE_NG.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.242692 wgse_ng-1.0.0a9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/docs/basic-usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/docs/reference-genome.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/docs/wgse-library.md
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/main.spec
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 19:39:04.278692 wgse_ng-1.0.0a9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.242692 wgse_ng-1.0.0a9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116407 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/test/fake_genome.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/test/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/test/test_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/test/test_fasta_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/test/test_letter_run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/test/test_microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/test/test_raw_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/test/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/test/test_unknown_bases_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/test/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.242692 wgse_ng-1.0.0a9/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/tools/fake_reference_genome_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/tools/import_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/tools/last_file_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/tools/reference_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.242692 wgse_ng-1.0.0a9/wgse/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-21 19:39:04.000000 wgse_ng-1.0.0a9/wgse/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.246692 wgse_ng-1.0.0a9/wgse/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/adapters/alignment_map_file_info_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/adapters/alignment_stats_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/adapters/header_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/adapters/index_stats_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/adapters/reference_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.246692 wgse_ng-1.0.0a9/wgse/alignment_map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/alignment_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/alignment_map/alignment_map_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/alignment_map/alignment_map_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/alignment_map/alignment_map_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/alignment_map/alignment_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/alignment_map/depth_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/alignment_map/index_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.246692 wgse_ng-1.0.0a9/wgse/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.250692 wgse_ng-1.0.0a9/wgse/data/alignment_map/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/alignment_map/alignment_map_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/alignment_map/alignment_map_header_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/alignment_map/alignment_map_header_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/alignment_map/alignment_map_header_read_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/alignment_map/alignment_map_header_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/alignment_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/chromosome_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/mitochondrial_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/mitochondrial_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/mitochondrial_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/read_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/sequence_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/data/tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.250692 wgse_ng-1.0.0a9/wgse/fasta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/fasta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/fasta/fasta_letter_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/fasta/fasta_stats_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/fasta/letter_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/fasta/letter_run_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/fasta/letter_run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/fasta/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.250692 wgse_ng-1.0.0a9/wgse/fastq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/fastq/fastq_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.250692 wgse_ng-1.0.0a9/wgse/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/WGSE-NG.pyproject
+-rw-r--r--   0 runner    (1001) docker     (127)    11778 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/WGSE-NG.pyproject.user
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.254692 wgse_ng-1.0.0a9/wgse/gui/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/extract/extract_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/extract/format_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/extract/microarray_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/extract/sequence_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/form.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    14690 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/reference.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.254692 wgse_ng-1.0.0a9/wgse/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67343 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/resources/logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   327118 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/resources/logo_nXP_icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/resources.qrc
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/table_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/gui/ui_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.258692 wgse_ng-1.0.0a9/wgse/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.270692 wgse_ng-1.0.0a9/wgse/metadata/bed_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/bed_templates/19_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/bed_templates/19_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/bed_templates/38_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/bed_templates/38_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/bed_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/builds.json
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/mtdna.json
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/ploidy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  4213157 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/references.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/references_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.274692 wgse_ng-1.0.0a9/wgse/metadata/report_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/report_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/report_templates/table_macro.html
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/report_templates/table_simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/report_templates/table_tab.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/sequencers.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/metadata/sources.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.274692 wgse_ng-1.0.0a9/wgse/microarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/microarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/microarray/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/microarray/microarray_line_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/microarray/raw_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.274692 wgse_ng-1.0.0a9/wgse/mtDNA/
+-rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/mtDNA/CRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    17129 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/mtDNA/RSRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/mtDNA/Yoruba.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/mtDNA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/mtDNA/rCRS.fasta
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.274692 wgse_ng-1.0.0a9/wgse/reference_genome/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/reference_genome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/reference_genome/bgzip_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/reference_genome/decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/reference_genome/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/reference_genome/genome_metadata_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/reference_genome/repository_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.274692 wgse_ng-1.0.0a9/wgse/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/renderers/csv_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/renderers/html_aligned_file_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/renderers/html_simple_table_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:39:04.278692 wgse_ng-1.0.0a9/wgse/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/utility/check_prerequisites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/utility/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/utility/file_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/utility/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/utility/mt_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/utility/process_io_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/utility/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/utility/sequence_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/utility/sequencers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/utility/shortcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/utility/simple_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/utility/unit_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/utility/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-21 19:38:59.000000 wgse_ng-1.0.0a9/wgse/variant_caller.py
```

### Comparing `wgse_ng-1.0.0a8/.github/ISSUE_TEMPLATE/bug_report.md` & `wgse_ng-1.0.0a9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/.github/ISSUE_TEMPLATE/feature_request.md` & `wgse_ng-1.0.0a9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/.github/workflows/python-app.yml` & `wgse_ng-1.0.0a9/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/.github/workflows/python-publish.yml` & `wgse_ng-1.0.0a9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/.vscode/settings.json` & `wgse_ng-1.0.0a9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/LICENSE` & `wgse_ng-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/PKG-INFO` & `wgse_ng-1.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Whole Genome Sequencing data manipulation tool
 Author-email: Multiple <unavailable@wgse-ng.com>
 License: MIT License
         
         Copyright (c) 2024 chaplin89
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `wgse_ng-1.0.0a8/README.md` & `wgse_ng-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/WGSE_NG.egg-info/PKG-INFO` & `wgse_ng-1.0.0a9/WGSE_NG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Whole Genome Sequencing data manipulation tool
 Author-email: Multiple <unavailable@wgse-ng.com>
 License: MIT License
         
         Copyright (c) 2024 chaplin89
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `wgse_ng-1.0.0a8/WGSE_NG.egg-info/SOURCES.txt` & `wgse_ng-1.0.0a9/WGSE_NG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/docs/Makefile` & `wgse_ng-1.0.0a9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/docs/basic-usage.md` & `wgse_ng-1.0.0a9/docs/basic-usage.md`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/docs/conf.py` & `wgse_ng-1.0.0a9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/docs/make.bat` & `wgse_ng-1.0.0a9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/docs/reference-genome.md` & `wgse_ng-1.0.0a9/docs/reference-genome.md`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/docs/requirements.txt` & `wgse_ng-1.0.0a9/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/main.spec` & `wgse_ng-1.0.0a9/main.spec`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/pyproject.toml` & `wgse_ng-1.0.0a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/test/fake_genome.fasta` & `wgse_ng-1.0.0a9/test/fake_genome.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/test/test_buckets.py` & `wgse_ng-1.0.0a9/test/test_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/test/test_fasta.py` & `wgse_ng-1.0.0a9/test/test_fasta.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/test/test_fasta_dictionary.py` & `wgse_ng-1.0.0a9/test/test_fasta_dictionary.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/test/test_letter_run_collection.py` & `wgse_ng-1.0.0a9/test/test_letter_run_collection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/test/test_microarray_converter.py` & `wgse_ng-1.0.0a9/test/test_microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/test/test_raw_file.py` & `wgse_ng-1.0.0a9/test/test_raw_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/test/test_unknown_bases_stats.py` & `wgse_ng-1.0.0a9/test/test_unknown_bases_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/test/utility.py` & `wgse_ng-1.0.0a9/test/utility.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/tools/fake_reference_genome_generator.py` & `wgse_ng-1.0.0a9/tools/fake_reference_genome_generator.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/tools/import_scanner.py` & `wgse_ng-1.0.0a9/tools/import_scanner.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/tools/last_file_export.py` & `wgse_ng-1.0.0a9/tools/last_file_export.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/tools/reference_stats.py` & `wgse_ng-1.0.0a9/tools/reference_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/__init__.py` & `wgse_ng-1.0.0a9/wgse/__init__.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/adapters/alignment_map_file_info_adapter.py` & `wgse_ng-1.0.0a9/wgse/adapters/alignment_map_file_info_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/adapters/alignment_stats_adapter.py` & `wgse_ng-1.0.0a9/wgse/adapters/alignment_stats_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/adapters/header_adapter.py` & `wgse_ng-1.0.0a9/wgse/adapters/header_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/adapters/index_stats_adapter.py` & `wgse_ng-1.0.0a9/wgse/adapters/index_stats_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/adapters/reference_adapter.py` & `wgse_ng-1.0.0a9/wgse/adapters/reference_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             ref_map = stats.reference_map
         max_columns = max([len(x) for x in ref_map.values()])
         genome_index_map = {}
         headers = ["Loaded file"]
         max_index = 0
         rows = []
         for key, value in ref_map.items():
-            row = [None for x in range(max_columns + 1)]
+            row = [None for x in range(max_columns + 2)]
             row[0] = key
             for sequence in value:
                 if sequence.parent not in genome_index_map:
                     genome_index_map[sequence.parent] = max_index
                     headers.append(str(sequence.parent))
                     max_index += 1
                 row[genome_index_map[sequence.parent] + 1] = sequence
```

### Comparing `wgse_ng-1.0.0a8/wgse/alignment_map/alignment_map_file.py` & `wgse_ng-1.0.0a9/wgse/alignment_map/alignment_map_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/alignment_map/alignment_map_header.py` & `wgse_ng-1.0.0a9/wgse/alignment_map/alignment_map_header.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/alignment_map/alignment_map_row.py` & `wgse_ng-1.0.0a9/wgse/alignment_map/alignment_map_row.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/alignment_map/alignment_stats_calculator.py` & `wgse_ng-1.0.0a9/wgse/alignment_map/alignment_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/alignment_map/depth_analyzer.py` & `wgse_ng-1.0.0a9/wgse/alignment_map/depth_analyzer.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/alignment_map/index_stats_calculator.py` & `wgse_ng-1.0.0a9/wgse/alignment_map/index_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/configuration.py` & `wgse_ng-1.0.0a9/wgse/configuration.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/data/alignment_map/alignment_map_file_info.py` & `wgse_ng-1.0.0a9/wgse/data/alignment_map/alignment_map_file_info.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/data/alignment_map/alignment_map_header_read_group.py` & `wgse_ng-1.0.0a9/wgse/data/alignment_map/alignment_map_header_read_group.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/data/alignment_map/alignment_map_header_sequence.py` & `wgse_ng-1.0.0a9/wgse/data/alignment_map/alignment_map_header_sequence.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/data/alignment_stats.py` & `wgse_ng-1.0.0a9/wgse/data/alignment_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/data/genome.py` & `wgse_ng-1.0.0a9/wgse/data/genome.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/data/microarray_converter.py` & `wgse_ng-1.0.0a9/wgse/data/microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/data/mitochondrial_model.py` & `wgse_ng-1.0.0a9/wgse/data/mitochondrial_model.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/data/sequence.py` & `wgse_ng-1.0.0a9/wgse/data/sequence.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/fasta/fasta_letter_counter.py` & `wgse_ng-1.0.0a9/wgse/fasta/fasta_letter_counter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/fasta/fasta_stats_files.py` & `wgse_ng-1.0.0a9/wgse/fasta/fasta_stats_files.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/fasta/letter_run_buckets.py` & `wgse_ng-1.0.0a9/wgse/fasta/letter_run_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/fasta/letter_run_collection.py` & `wgse_ng-1.0.0a9/wgse/fasta/letter_run_collection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/fasta/reference.py` & `wgse_ng-1.0.0a9/wgse/fasta/reference.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from wgse.data.sequence import Sequence
 
 
 class ReferenceStatus(enum.Enum):
     Available = enum.auto()
     Downloadable = enum.auto()
     Buildable = enum.auto()
+    Ambiguous = enum.auto()
     Unknown = enum.auto()
 
 
 class Reference:
     """This class represent a reference genome."""
 
     def __init__(
@@ -21,15 +22,26 @@
         reference_map: OrderedDict[Sequence, list[Sequence]],
         logger=logging.getLogger(__name__),
     ):
         self._logger = logger
         self.reference_map = reference_map
         self._genome_map = self._index_by_genome()
         self.matching: list[Genome] = self._get_matching_genomes()
-        self.build = set(x.build for x in self.matching)
+        sorted = list([x for x in self._genome_map.keys() if x is not None])
+        sorted.sort(
+            key=lambda x: len(
+                [y for y in self._genome_map[x].values() if y is not None]
+            )
+        )
+        self.build = []
+        if len(self.matching) > 0:
+            self.build = set(x.build for x in self.matching)
+        elif len(sorted) > 0:
+            self.build = [f"Likely {sorted[-1].build}"]
+
         if len(self.build) > 1:
             self._logger.warn(
                 "Found more than one valid builds for the reference of the file. "
                 + "This is likely an issue with the reference genome metadata. "
                 + "Please open a bug report."
             )
         self.build = " ".join(self.build)
@@ -68,36 +80,34 @@
         for query, reference_match in self.reference_map.items():
             unique_parents: set[Genome] = set(x.parent for x in reference_match)
             for parent in unique_parents:
                 if parent not in genome_map:
                     genome_map[parent] = {x: None for x in parent.sequences}
             for match in reference_match:
                 genome_map[match.parent][match] = query
-
-        # Remove genomes that match only by 1 sequence.
-        # It's likely to be an mtDNA sequence and it can create
-        # a lot of noise. We don't care about them anyway as
-        # MtDNA sequences are shipped with the software itself.
-        # TODO: improve this procedure to make sure we're really
-        # removing an MtDNA sequence and not a random one.
-        genome_map_no_mitochondrial = {}
-        for key, value in genome_map.items():
-            valid = len([x for x in value.values() if x is not None])
-            if valid > 1:
-                genome_map_no_mitochondrial[key] = value
-        return genome_map_no_mitochondrial
+            if len(reference_match) == 0:
+                if None not in genome_map:
+                    genome_map[None] = []
+                genome_map[None].append(query)
+        return genome_map
 
     def _get_matching_genomes(self):
         """Return a list of genomes that are guaranteed to match the input sequence
         by name, length or MD5 (if available in the input sequence).
 
         Returns:
             list[Genome]: list of matching genomes.
         """
         match_list = []
+        # None is a special key for all the sequences
+        # that have 0 matches among all the known references.
+        # If None is in _genome_map means we didn't find a
+        # reference and is not possible to build it.
+        if None in self._genome_map:
+            return match_list
         for genome, matches in self._genome_map.items():
             matching = True
             for genome_sequence, query_sequence in matches.items():
                 if query_sequence is None:
                     matching = False
                     break
                 if genome_sequence.name != query_sequence.name:
```

### Comparing `wgse_ng-1.0.0a8/wgse/fastq/fastq_file.py` & `wgse_ng-1.0.0a9/wgse/fastq/fastq_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/gui/WGSE-NG.pyproject.user` & `wgse_ng-1.0.0a9/wgse/gui/WGSE-NG.pyproject.user`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/gui/extract/extract_wizard.py` & `wgse_ng-1.0.0a9/wgse/gui/extract/extract_wizard.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/gui/extract/format_selection.py` & `wgse_ng-1.0.0a9/wgse/gui/extract/format_selection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/gui/extract/microarray_selection.py` & `wgse_ng-1.0.0a9/wgse/gui/extract/microarray_selection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/gui/extract/sequence_selection.py` & `wgse_ng-1.0.0a9/wgse/gui/extract/sequence_selection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/gui/form.ui` & `wgse_ng-1.0.0a9/wgse/gui/form.ui`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/gui/main.py` & `wgse_ng-1.0.0a9/wgse/gui/main.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/gui/reference.ui` & `wgse_ng-1.0.0a9/wgse/gui/reference.ui`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/gui/resources/logo.jpg` & `wgse_ng-1.0.0a9/wgse/gui/resources/logo.jpg`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/gui/resources/logo_nXP_icon.ico` & `wgse_ng-1.0.0a9/wgse/gui/resources/logo_nXP_icon.ico`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/gui/table_dialog.py` & `wgse_ng-1.0.0a9/wgse/gui/table_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/gui/ui_form.py` & `wgse_ng-1.0.0a9/wgse/gui/ui_form.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/metadata/bed_templates/19_wes.csv` & `wgse_ng-1.0.0a9/wgse/metadata/bed_templates/19_wes.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/metadata/bed_templates/38_wes.csv` & `wgse_ng-1.0.0a9/wgse/metadata/bed_templates/38_wes.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/metadata/bed_templates/38_y_mt.csv` & `wgse_ng-1.0.0a9/wgse/metadata/bed_templates/38_y_mt.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/metadata/mtdna.json` & `wgse_ng-1.0.0a9/wgse/metadata/mtdna.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/metadata/references.json` & `wgse_ng-1.0.0a9/wgse/metadata/references.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/metadata/references_template.json` & `wgse_ng-1.0.0a9/wgse/metadata/references_template.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/metadata/report_templates/table_macro.html` & `wgse_ng-1.0.0a9/wgse/metadata/report_templates/table_macro.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/metadata/report_templates/table_simple.html` & `wgse_ng-1.0.0a9/wgse/metadata/report_templates/table_simple.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/metadata/report_templates/table_tab.html` & `wgse_ng-1.0.0a9/wgse/metadata/report_templates/table_tab.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/metadata/sequencers.json` & `wgse_ng-1.0.0a9/wgse/metadata/sequencers.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/metadata/sources.json` & `wgse_ng-1.0.0a9/wgse/metadata/sources.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/microarray/microarray_converter.py` & `wgse_ng-1.0.0a9/wgse/microarray/microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/microarray/microarray_line_formatter.py` & `wgse_ng-1.0.0a9/wgse/microarray/microarray_line_formatter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/microarray/raw_file.py` & `wgse_ng-1.0.0a9/wgse/microarray/raw_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/mtDNA/CRS.fasta` & `wgse_ng-1.0.0a9/wgse/mtDNA/CRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/mtDNA/RSRS.fasta` & `wgse_ng-1.0.0a9/wgse/mtDNA/RSRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/mtDNA/Yoruba.fasta` & `wgse_ng-1.0.0a9/wgse/mtDNA/Yoruba.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/mtDNA/rCRS.fasta` & `wgse_ng-1.0.0a9/wgse/mtDNA/rCRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/reference_genome/bgzip_compressor.py` & `wgse_ng-1.0.0a9/wgse/reference_genome/bgzip_compressor.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/reference_genome/decompressor.py` & `wgse_ng-1.0.0a9/wgse/reference_genome/decompressor.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/reference_genome/downloader.py` & `wgse_ng-1.0.0a9/wgse/reference_genome/downloader.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/reference_genome/genome_metadata_loader.py` & `wgse_ng-1.0.0a9/wgse/reference_genome/genome_metadata_loader.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/reference_genome/repository_manager.py` & `wgse_ng-1.0.0a9/wgse/reference_genome/repository_manager.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/renderers/html_aligned_file_report.py` & `wgse_ng-1.0.0a9/wgse/renderers/html_aligned_file_report.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/renderers/html_simple_table_report.py` & `wgse_ng-1.0.0a9/wgse/renderers/html_simple_table_report.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/utility/check_prerequisites.py` & `wgse_ng-1.0.0a9/wgse/utility/check_prerequisites.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/utility/external.py` & `wgse_ng-1.0.0a9/wgse/utility/external.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/utility/file_type_checker.py` & `wgse_ng-1.0.0a9/wgse/utility/file_type_checker.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/utility/mt_dna.py` & `wgse_ng-1.0.0a9/wgse/utility/mt_dna.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/utility/process_io_monitor.py` & `wgse_ng-1.0.0a9/wgse/utility/process_io_monitor.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/utility/regions.py` & `wgse_ng-1.0.0a9/wgse/utility/regions.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/utility/sequence_orderer.py` & `wgse_ng-1.0.0a9/wgse/utility/sequence_orderer.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/utility/sequencers.py` & `wgse_ng-1.0.0a9/wgse/utility/sequencers.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/utility/shortcut.py` & `wgse_ng-1.0.0a9/wgse/utility/shortcut.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/utility/simple_worker.py` & `wgse_ng-1.0.0a9/wgse/utility/simple_worker.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/utility/updater.py` & `wgse_ng-1.0.0a9/wgse/utility/updater.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a8/wgse/variant_caller.py` & `wgse_ng-1.0.0a9/wgse/variant_caller.py`

 * *Files identical despite different names*

